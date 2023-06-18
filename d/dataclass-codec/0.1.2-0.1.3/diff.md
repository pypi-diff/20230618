# Comparing `tmp/dataclass_codec-0.1.2.tar.gz` & `tmp/dataclass_codec-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.2.tar", max compression
+gzip compressed data, was "dataclass_codec-0.1.3.tar", max compression
```

## Comparing `dataclass_codec-0.1.2.tar` & `dataclass_codec-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.2/README.md
--rw-r--r--   0        0        0      600 2023-06-18 00:59:07.432829 dataclass_codec-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-17 23:22:01.983362 dataclass_codec-0.1.2/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0     5981 2023-06-18 00:54:44.332834 dataclass_codec-0.1.2/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.2/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.2/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    10686 2023-06-18 00:45:49.662903 dataclass_codec-0.1.2/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.2/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.3/README.md
+-rw-r--r--   0        0        0      600 2023-06-18 02:08:33.062440 dataclass_codec-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.3/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0     8596 2023-06-18 02:07:06.752454 dataclass_codec-0.1.3/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.3/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.3/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    12306 2023-06-18 02:07:53.282450 dataclass_codec-0.1.3/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.3/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.3/PKG-INFO
```

### Comparing `dataclass_codec-0.1.2/pyproject.toml` & `dataclass_codec-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.1.2/src/dataclass_codec/encode.py` & `dataclass_codec-0.1.3/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.2/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.1.3/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 from datetime import date, datetime, time, timezone
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Dict, List, NewType, Optional, Union
 
 import pytest
 
-from dataclass_codec import encode, decode
+from dataclass_codec import (
+    encode,
+    decode,
+    decode_context_scope,
+    DecodeContext,
+    error_list_scope,
+)
 
 
 def optional(cls: Any) -> Any:
     raise NotImplementedError
 
 
 def get_class_or_type_name(cls: Any) -> str:
@@ -292,15 +298,15 @@
 
         @dataclass
         class Dummy2:
             dummy: Dummy
 
         assert encode(Dummy2(Dummy(1))) == {"dummy": {"a": 1}}
 
-    def test_cu(self) -> None:
+    def test_complex_case(self) -> None:
         a = {
             "id": 7,
             "created_on": "2023-06-18 00:40:24",
             "modified_on": "2023-06-18 00:40:24",
             "owner_user_id": 1,
             "domain_names": [
                 "brutus.example.com",
@@ -377,7 +383,64 @@
             # certificate: Optional[Certificate]
             # owner: User
             # access_list: AccessList
             use_default_location: bool
             ipv6: bool
 
         decode(a, ProxyHostAddResponse)
+
+    def test_decode_dataclass_with_optional(self) -> None:
+        @dataclass
+        class Dummy:
+            a: Optional[int]
+
+        assert decode({"a": 1}, Dummy) == Dummy(1)
+        assert decode({}, Dummy) == Dummy(None)
+
+    def test_raises_on_decode_dataclass_with_required(self) -> None:
+        @dataclass
+        class Dummy:
+            a: int
+
+        with pytest.raises(ValueError):
+            with decode_context_scope(
+                DecodeContext(
+                    dataclass_unset_as_none=False,
+                )
+            ):
+                decode({}, Dummy)
+
+    def test_decode_collect_errors(self) -> None:
+        @dataclass
+        class Dummy:
+            a: int
+
+        with error_list_scope() as errors, decode_context_scope(
+            DecodeContext(
+                collect_errors=True,
+                dataclass_unset_as_none=False,
+            )
+        ):
+            decode({}, Dummy)
+
+            assert len(errors) == 1
+            assert errors[0][0] == "$.a"
+
+    def test_decode_collect_errors_with_complex_case(self) -> None:
+        @dataclass
+        class Dummy:
+            a: int
+
+        @dataclass
+        class Dummy2:
+            dummy: Dummy
+
+        with error_list_scope() as errors, decode_context_scope(
+            DecodeContext(
+                collect_errors=True,
+                dataclass_unset_as_none=False,
+            )
+        ):
+            decode({"dummy": {}}, Dummy2)
+
+            assert len(errors) == 1
+            assert errors[0][0] == "$.dummy.a"
```

### Comparing `dataclass_codec-0.1.2/PKG-INFO` & `dataclass_codec-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

