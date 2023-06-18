# Comparing `tmp/dataclass_codec-0.1.1.tar.gz` & `tmp/dataclass_codec-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.1.tar", max compression
+gzip compressed data, was "dataclass_codec-0.1.2.tar", max compression
```

## Comparing `dataclass_codec-0.1.1.tar` & `dataclass_codec-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.1/README.md
--rw-r--r--   0        0        0      600 2023-06-18 00:34:21.382966 dataclass_codec-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-17 23:22:01.983362 dataclass_codec-0.1.1/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0     5822 2023-06-18 00:10:39.823091 dataclass_codec-0.1.1/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.1/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.1/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0     8007 2023-06-18 00:10:39.823091 dataclass_codec-0.1.1/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.1/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-06-18 00:09:53.423097 dataclass_codec-0.1.2/README.md
+-rw-r--r--   0        0        0      600 2023-06-18 00:59:07.432829 dataclass_codec-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-17 23:22:01.983362 dataclass_codec-0.1.2/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0     5981 2023-06-18 00:54:44.332834 dataclass_codec-0.1.2/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2729 2023-06-18 00:08:14.743112 dataclass_codec-0.1.2/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.2/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    10686 2023-06-18 00:45:49.662903 dataclass_codec-0.1.2/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.2/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 dataclass_codec-0.1.2/PKG-INFO
```

### Comparing `dataclass_codec-0.1.1/pyproject.toml` & `dataclass_codec-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-codec"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["lucas.silva <lucas.silva@jeaholding.com.br>"]
 readme = "README.md"
 packages = [{include = "dataclass_codec", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `dataclass_codec-0.1.1/src/dataclass_codec/decode.py` & `dataclass_codec-0.1.2/src/dataclass_codec/decode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import base64
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Callable, Dict, List, Tuple, Type, TypeVar, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 
 from dataclass_codec.types_predicates import (
     is_dataclass_predicate,
     is_enum_predicate,
 )
 
+
 ANYTYPE = Type[Any]
 
 
 TYPEMATCHPREDICATE = Callable[[ANYTYPE], bool]
 DECODEIT = Callable[[Any, ANYTYPE], Any]
 TYPEDECODER = Callable[[Any, ANYTYPE, DECODEIT], Any]
 
@@ -85,16 +96,21 @@
     obj: Any, _type: ANYTYPE, decode_it: DECODEIT
 ) -> Any:
     assert is_dataclass_predicate(_type)
     assert isinstance(obj, dict)
 
     return _type(
         **{
-            k: decode_it(v, _type.__dataclass_fields__[k].type)
-            for k, v in obj.items()
+            k: decode_it(
+                obj[k],
+                _type.__dataclass_fields__[k].type,
+            )
+            if k in obj
+            else None
+            for k in _type.__dataclass_fields__.keys()
         }
     )
 
 
 def decimal_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
     assert isinstance(obj, (str, int, float))
     return Decimal(obj)
```

### Comparing `dataclass_codec-0.1.1/src/dataclass_codec/encode.py` & `dataclass_codec-0.1.2/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.1/PKG-INFO` & `dataclass_codec-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

