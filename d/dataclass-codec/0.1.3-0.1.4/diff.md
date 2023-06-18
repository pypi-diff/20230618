# Comparing `tmp/dataclass_codec-0.1.3.tar.gz` & `tmp/dataclass_codec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.3.tar", max compression
+gzip compressed data, was "dataclass_codec-0.1.4.tar", max compression
```

## Comparing `dataclass_codec-0.1.3.tar` & `dataclass_codec-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.3/README.md
--rw-r--r--   0        0        0      600 2023-06-18 02:08:33.062440 dataclass_codec-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.3/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0     8596 2023-06-18 02:07:06.752454 dataclass_codec-0.1.3/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.3/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.3/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    12306 2023-06-18 02:07:53.282450 dataclass_codec-0.1.3/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.3/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.4/README.md
+-rw-r--r--   0        0        0      600 2023-06-18 02:49:57.842218 dataclass_codec-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.4/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0     8899 2023-06-18 02:49:41.022220 dataclass_codec-0.1.4/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.4/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.4/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    14799 2023-06-18 02:43:02.922253 dataclass_codec-0.1.4/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.4/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.4/PKG-INFO
```

### Comparing `dataclass_codec-0.1.3/pyproject.toml` & `dataclass_codec-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.1.3/src/dataclass_codec/decode.py` & `dataclass_codec-0.1.4/src/dataclass_codec/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,27 @@
 
 def primitive_hook(_type: ANYTYPE) -> TYPEDECODER:
     def decode_primitive(
         obj: Any, _type: ANYTYPE, _decode_it: DECODEIT
     ) -> Any:
         ctx = decode_context()
 
-        if ctx.primitive_cast_values:
+        def type_can_cast(_type: ANYTYPE) -> bool:
+            return _type in (
+                str,
+                int,
+                float,
+                Decimal,
+                bool,
+                date,
+                datetime,
+                time,
+            )
+
+        if ctx.primitive_cast_values and type_can_cast(_type):
             return _type(obj)
 
         if ctx.strict and _type(obj) != obj:
             raise TypeError(f"Cannot decode {obj} as {_type}")
 
         return obj
```

### Comparing `dataclass_codec-0.1.3/src/dataclass_codec/encode.py` & `dataclass_codec-0.1.4/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.3/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.1.4/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 from dataclasses import dataclass
 from datetime import date, datetime, time, timezone
 from decimal import Decimal
 from enum import Enum
+import json
 from typing import Any, Dict, List, NewType, Optional, Union
 
 import pytest
 
 from dataclass_codec import (
     encode,
     decode,
@@ -440,7 +441,100 @@
                 dataclass_unset_as_none=False,
             )
         ):
             decode({"dummy": {}}, Dummy2)
 
             assert len(errors) == 1
             assert errors[0][0] == "$.dummy.a"
+
+    def test_another_complex_data(self) -> None:
+        @dataclass
+        class Location:
+            path: str
+            advanced_config: str
+            forward_scheme: str
+            forward_host: str
+            forward_port: str
+
+        @dataclass
+        class ProxyHostAddResponse:
+            id: int
+            created_on: str
+            modified_on: str
+            owner_user_id: int
+            domain_names: List[str]
+            forward_host: str
+            forward_port: int
+            access_list_id: int
+            certificate_id: int
+            ssl_forced: int
+            caching_enabled: int
+            block_exploits: int
+            advanced_config: str
+            meta: Dict[str, Union[bool, str, int, None]]
+            allow_websocket_upgrade: int
+            http2_support: int
+            forward_scheme: str
+            enabled: int
+            locations: List[Location]
+            hsts_enabled: int
+            hsts_subdomains: int
+            # certificate: Optional[Certificate]
+            # owner: User
+            # access_list: AccessList
+            use_default_location: bool
+            ipv6: bool
+
+        json_data = json.loads(
+            """{
+    "id": 16,
+    "created_on": "2023-06-18 02:36:05",
+    "modified_on": "2023-06-18 02:36:11",
+    "owner_user_id": 1,
+    "domain_names": [
+        "brutus.example.com",
+        "casca.example.com",
+        "cassius.example.com",
+        "decius.example.com",
+        "metellus.example.com"
+    ],
+    "forward_host": "localhost",
+    "forward_port": 8081,
+    "access_list_id": 0,
+    "certificate_id": 0,
+    "ssl_forced": 0,
+    "caching_enabled": 0,
+    "block_exploits": 0,
+    "advanced_config": "",
+    "meta": {
+        "nginx_online": true,
+        "nginx_err": null
+    },
+    "allow_websocket_upgrade": 0,
+    "http2_support": 0,
+    "forward_scheme": "http",
+    "enabled": 1,
+    "locations": [],
+    "hsts_enabled": 0,
+    "hsts_subdomains": 0,
+    "owner": {
+        "id": 1,
+        "created_on": "2023-06-17 20:01:58",
+        "modified_on": "2023-06-17 20:01:58",
+        "is_deleted": 0,
+        "is_disabled": 0,
+        "email": "admin@example.com",
+        "name": "Administrator",
+        "nickname": "Admin",
+        "avatar": "",
+        "roles": [
+            "admin"
+        ]
+    },
+    "certificate": null,
+    "access_list": null,
+    "use_default_location": true,
+    "ipv6": true
+}"""
+        )
+
+        decode(json_data, ProxyHostAddResponse)
```

### Comparing `dataclass_codec-0.1.3/PKG-INFO` & `dataclass_codec-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

