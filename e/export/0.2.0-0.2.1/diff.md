# Comparing `tmp/export-0.2.0.tar.gz` & `tmp/export-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export-0.2.0.tar", max compression
+gzip compressed data, was "export-0.2.1.tar", max compression
```

## Comparing `export-0.2.0.tar` & `export-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1067 2022-03-13 19:40:57.547891 export-0.2.0/LICENSE
--rw-r--r--   0        0        0      769 2022-03-13 19:40:57.547891 export-0.2.0/README.md
--rw-r--r--   0        0        0      148 2022-03-13 19:40:57.551891 export-0.2.0/export/__init__.py
--rw-r--r--   0        0        0     1208 2022-03-13 19:40:57.551891 export-0.2.0/export/api.py
--rw-r--r--   0        0        0      176 2022-03-13 19:40:57.551891 export-0.2.0/export/enums.py
--rw-r--r--   0        0        0      280 2022-03-13 19:40:57.551891 export-0.2.0/export/models.py
--rw-r--r--   0        0        0      605 2022-03-13 19:46:39.551987 export-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1399 2022-03-13 19:46:42.743670 export-0.2.0/setup.py
--rw-r--r--   0        0        0     1472 2022-03-13 19:46:42.743880 export-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-18 16:59:30.993251 export-0.2.1/LICENSE
+-rw-r--r--   0        0        0      816 2023-06-18 16:59:30.993251 export-0.2.1/README.md
+-rw-r--r--   0        0        0      130 2023-06-18 17:53:33.980841 export-0.2.1/export/__init__.py
+-rw-r--r--   0        0        0     1345 2023-06-18 17:53:33.984841 export-0.2.1/export/api.py
+-rw-r--r--   0        0        0      243 2023-06-18 17:53:33.984841 export-0.2.1/export/enums.py
+-rw-r--r--   0        0        0      302 2023-06-18 17:53:33.984841 export-0.2.1/export/models.py
+-rw-r--r--   0        0        0      118 2023-06-18 17:53:33.984841 export-0.2.1/export/protocols.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:04:44.729802 export-0.2.1/export/py.typed
+-rw-r--r--   0        0        0     1126 2023-06-18 17:53:33.984841 export-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 export-0.2.1/PKG-INFO
```

### Comparing `export-0.2.0/LICENSE` & `export-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `export-0.2.0/README.md` & `export-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # export
 Control module exports
 
 ## About
 This library dynamically generates an `__all__` attribute for modules
 
+## Install
+```console
+pip install export
+```
+
 ## Usage
 
 ### Private by Default
 *Does* export objects marked **public**, *doesn't* export everything else
 
 ```python
 # lib.py
@@ -57,8 +62,8 @@
 ```
 
 ```python
 >>> import lib
 >>> 
 >>> lib.__all__
 ['export', 'foo']
-```
+```
```

### Comparing `export-0.2.0/export/api.py` & `export-0.2.1/export/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,54 @@
 import inspect
 import sys
-import types
-import typing
+from types import ModuleType
+from typing import List, Mapping, Optional, Sequence, Set, TypeVar
 
-from . import enums, models
+from .enums import Access
+from .models import Scope
+from .protocols import Named
 
+__all__: Sequence[str] = ("init", "public", "private")
 
-def init(*, default: enums.Access = enums.Access.PRIVATE) -> None:
-    module: types.ModuleType = inspect.getmodule(inspect.stack()[1][0])
 
-    class Module(types.ModuleType):
-        _scope: models.Scope = models.Scope(default=default)
+T = TypeVar("T", bound=Named)
+
+
+def init(*, default: Access = Access.PRIVATE) -> None:
+    module: Optional[ModuleType] = inspect.getmodule(inspect.stack()[1][0])
+
+    class Module(ModuleType):
+        _scope: Scope = Scope(default=default)
 
         @property
-        def __all__(self) -> typing.List[str]:
-            attributes: typing.Set[str] = {
-                key for key in dir(self) if not key.startswith("_")
-            }
+        def __all__(self) -> List[str]:
+            attributes: Set[str] = {key for key in dir(self) if not key.startswith("_")}
 
-            if self._scope.default == enums.Access.PUBLIC:
+            if self._scope.default is Access.PUBLIC:
                 return sorted(attributes - self._scope.private)
 
             return sorted(self._scope.public)
 
     module.__class__ = Module
 
 
-def public(obj: typing.T) -> typing.T:
-    return _export(obj, access=enums.Access.PUBLIC)
+def public(obj: T, /) -> T:
+    return _export(obj, access=Access.PUBLIC)
+
 
+def private(obj: T, /) -> T:
+    return _export(obj, access=Access.PRIVATE)
 
-def private(obj: typing.T) -> typing.T:
-    return _export(obj, access=enums.Access.PRIVATE)
 
+def _export(obj: T, /, access: Access) -> T:
+    module: ModuleType = sys.modules[obj.__module__]
 
-def _export(obj: typing.T, access: enums.Access) -> typing.T:
-    module: types.ModuleType = sys.modules[obj.__module__]
+    collections: Mapping[Access, Set[str]] = {
+        Access.PUBLIC: module._scope.public,
+        Access.PRIVATE: module._scope.private,
+    }
 
-    collection: typing.Set[str] = (
-        module._scope.public if access is enums.Access.PUBLIC else module._scope.private
-    )
+    collection: Set[str] = collections[access]
 
     collection.add(obj.__name__)
 
     return obj
```

### Comparing `export-0.2.0/PKG-INFO` & `export-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: export
-Version: 0.2.0
+Version: 0.2.1
 Summary: Control module exports
 Home-page: https://github.com/tombulled/export
 License: MIT
 Keywords: python,export,public,private
 Author: Tom Bulled
 Author-email: 26026015+tombulled@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://github.com/tombulled/export
 Project-URL: Repository, https://github.com/tombulled/export
 Description-Content-Type: text/markdown
 
 # export
 Control module exports
 
 ## About
 This library dynamically generates an `__all__` attribute for modules
 
+## Install
+```console
+pip install export
+```
+
 ## Usage
 
 ### Private by Default
 *Does* export objects marked **public**, *doesn't* export everything else
 
 ```python
 # lib.py
@@ -77,7 +83,8 @@
 
 ```python
 >>> import lib
 >>> 
 >>> lib.__all__
 ['export', 'foo']
 ```
+
```

