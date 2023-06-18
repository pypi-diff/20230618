# Comparing `tmp/pyrepresent-0.1.0.tar.gz` & `tmp/pyrepresent-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.1.0.tar", last modified: Sat Jun 17 15:04:53 2023, max compression
+gzip compressed data, was "pyrepresent-0.1.1.tar", last modified: Sun Jun 18 08:02:32 2023, max compression
```

## Comparing `pyrepresent-0.1.0.tar` & `pyrepresent-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:04:53.178463 pyrepresent-0.1.0/
--rw-rw-rw-   0        0        0      115 2023-06-17 15:04:52.000000 pyrepresent-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-06-17 15:04:53.177463 pyrepresent-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.0/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.0/build.py
--rw-rw-rw-   0        0        0      715 2023-06-17 15:04:52.000000 pyrepresent-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-17 15:04:53.171461 pyrepresent-0.1.0/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 15:04:53.176462 pyrepresent-0.1.0/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.0/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.0/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.0/represent/document.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.0/represent/indentation.py
--rw-rw-rw-   0        0        0    17977 2023-06-17 15:03:59.000000 pyrepresent-0.1.0/represent/object.py
--rw-rw-rw-   0        0        0    20797 2023-06-17 15:02:03.000000 pyrepresent-0.1.0/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 15:04:53.178463 pyrepresent-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-17 15:04:48.000000 pyrepresent-0.1.0/setup.py
--rw-rw-rw-   0        0        0      971 2023-06-13 13:18:42.000000 pyrepresent-0.1.0/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:02:32.227963 pyrepresent-0.1.1/
+-rw-rw-rw-   0        0        0      115 2023-06-18 08:02:31.000000 pyrepresent-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-06-18 08:02:32.227963 pyrepresent-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.1/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.1/build.py
+-rw-rw-rw-   0        0        0      715 2023-06-18 08:02:31.000000 pyrepresent-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-18 08:02:32.198450 pyrepresent-0.1.1/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-18 08:02:32.000000 pyrepresent-0.1.1/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 08:02:32.226963 pyrepresent-0.1.1/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.1/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.1/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.1/represent/document.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.1/represent/indentation.py
+-rw-rw-rw-   0        0        0    19307 2023-06-18 08:01:33.000000 pyrepresent-0.1.1/represent/object.py
+-rw-rw-rw-   0        0        0    20797 2023-06-17 15:02:03.000000 pyrepresent-0.1.1/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 08:02:32.228963 pyrepresent-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-18 08:01:40.000000 pyrepresent-0.1.1/setup.py
+-rw-rw-rw-   0        0        0      971 2023-06-13 13:18:42.000000 pyrepresent-0.1.1/test.py
```

### Comparing `pyrepresent-0.1.0/PKG-INFO` & `pyrepresent-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.0/README.md` & `pyrepresent-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.0/build.py` & `pyrepresent-0.1.1/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.0/pyproject.toml` & `pyrepresent-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.1.0'
+version = '0.1.1'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.1.0/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.1.1/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.1.0
+Version: 0.1.1
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.1.0/represent/base.py` & `pyrepresent-0.1.1/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.0/represent/indentation.py` & `pyrepresent-0.1.1/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.0/represent/object.py` & `pyrepresent-0.1.1/represent/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # object.py
 
 import inspect
 import builtins
 import types
 import datetime as dt
-from abc import ABCMeta
 from itertools import chain
 from typing import (
     Any, Optional, Union, Iterable, Type, Dict, Tuple
 )
 
 from represent.base import is_bound_method
 from represent.indentation import indent
 from represent.structures import (
     structures, HiddenStructure, StringWrapper, colorize,
     CircularReferenceStructure, DataStructure, TypeStructure,
-    ObjectStructure, FunctionStructure
+    ObjectStructure, FunctionStructure, SetStructure,
+    ListStructure, DictStructure
 )
 
 import pandas as pd
 import numpy as np
 
 __all__ = [
     "to_string",
@@ -123,15 +123,15 @@
         :return: The string representation of the model.
         """
 
         return to_string(self)
     # end __str__
 # end BaseModel
 
-class FrozenHashable(metaclass=ABCMeta):
+class FrozenHashable:
     """A hashable dict structure."""
 
     def __hash__(self) -> int:
         """
         Returns the hash of the signature for hashing the object.
 
         :return: The hash of the object.
@@ -202,15 +202,15 @@
     clear = _immutable
     update = _immutable
     setdefault = _immutable
     pop = _immutable
     popitem = _immutable
 # end HashableDict
 
-class HashableDict(FrozenHashable, dict):
+class HashableDict(DictStructure, FrozenHashable, dict):
     """A hashable dict structure."""
 
     @property
     def _signature(self) -> Tuple[Tuple[Any, Any], ...]:
         """
         Returns a hashable dict signature.
 
@@ -253,17 +253,33 @@
             data.append((key, value))
         # end for
 
         data.sort(key=lambda v: hash(v))
 
         return tuple(data)
     # end __signature
+
+    def __str__(self) -> str:
+        """
+        Returns a string to represent the object.
+
+        :return: A string representation for the commands of the object.
+        """
+
+        content = DictStructure.__str__(self)
+
+        if self.__type__ is None:
+            return HashableDict.__name__ + "(" + content + ")"
+        # end if
+
+        return content
+    # end __str__
 # end HashableDict
 
-class HashableList(FrozenHashable, list):
+class HashableList(ListStructure, FrozenHashable, list):
     """A hashable list structure."""
 
     @property
     def _signature(self) -> Tuple[Any, ...]:
         """
         Returns a hashable dict signature.
 
@@ -293,17 +309,33 @@
             data.append(value)
         # end for
 
         data.sort(key=lambda v: hash(v))
 
         return tuple(data)
     # end __signature
+
+    def __str__(self) -> str:
+        """
+        Returns a string to represent the object.
+
+        :return: A string representation for the commands of the object.
+        """
+
+        content = ListStructure.__str__(self)
+
+        if self.__type__ is None:
+            return HashableList.__name__ + "(" + content + ")"
+        # end if
+
+        return content
+    # end __str__
 # end HashableDict
 
-class HashableSet(FrozenHashable, set):
+class HashableSet(SetStructure, FrozenHashable, set):
     """A hashable list structure."""
 
     @property
     def _signature(self) -> Tuple[Any, ...]:
         """
         Returns a hashable dict signature.
 
@@ -333,14 +365,30 @@
             data.append(value)
         # end for
 
         data.sort(key=lambda v: hash(v))
 
         return tuple(data)
     # end __signature
+
+    def __str__(self) -> str:
+        """
+        Returns a string to represent the object.
+
+        :return: A string representation for the commands of the object.
+        """
+
+        content = SetStructure.__str__(self)
+
+        if self.__type__ is None:
+            return HashableSet.__name__ + "(" + content + ")"
+        # end if
+
+        return content
+    # end __str__
 # end HashableDict
 
 def unwrap(
         data: Any, /, *,
         hidden: Optional[Union[Dict[Any, Any], Iterable[Any]]] = None,
         assign: Optional[bool] = False,
         properties: Optional[bool] = False,
@@ -369,18 +417,18 @@
     """
 
     if inspect.isclass(data):
         return TypeStructure(data)
     # end if
 
     if (
-            isinstance(data, BaseModel) and
-            hasattr(data, "modifiers") and
-            isinstance(data.modifiers, Modifiers) and
-            ids and (not force)
+        isinstance(data, BaseModel) and
+        hasattr(data, "modifiers") and
+        isinstance(data.modifiers, Modifiers) and
+        ids and (not force)
     ):
         modifiers = data.modifiers
 
         assign = modifiers.assign
         excluded = modifiers.excluded
         properties = modifiers.properties
         protected = modifiers.protected
@@ -520,15 +568,16 @@
                     bool_value = True
                 # end try
 
                 if (
                     (
                         (excluded is not None) and
                         ((key in excluded) or (type(value) in excluded))
-                    ) or (
+                    ) or
+                    (
                         defined and
                         (not (isinstance(value, bool) or bool_value))
                     )
                 ):
                     continue
                 # end if
 
@@ -541,28 +590,31 @@
                         value = hidden[key]
 
                     else:
                         value = HiddenStructure()
                     # end if
                 # end if
 
+                base = type(key)
+
                 key = unwrap(
                     key, assign=assign, ids=ids, excluded=excluded,
                     properties=properties, protected=protected,
                     hidden=hidden, legalize=legalize, force=force,
                     defined=defined
                 )
                 # end if
 
                 if isinstance(key, dict):
                     try:
                         {key: None}
 
                     except TypeError:
                         key = HashableDict(key)
+                        key.__type__ = base
                     # end try
                 # end if
 
                 results[key] = unwrap(
                     value, assign=assign, ids=ids, excluded=excluded,
                     properties=properties, protected=protected,
                     hidden=hidden, legalize=legalize, force=force,
```

### Comparing `pyrepresent-0.1.0/represent/structures.py` & `pyrepresent-0.1.1/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.0/setup.py` & `pyrepresent-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.1.0',
+        version='0.1.1',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.1.0/test.py` & `pyrepresent-0.1.1/test.py`

 * *Files identical despite different names*

