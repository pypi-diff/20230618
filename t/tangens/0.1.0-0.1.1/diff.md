# Comparing `tmp/tangens-0.1.0.tar.gz` & `tmp/tangens-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangens-0.1.0.tar", max compression
+gzip compressed data, was "tangens-0.1.1.tar", max compression
```

## Comparing `tangens-0.1.0.tar` & `tangens-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-17 21:51:00.344118 tangens-0.1.0/LICENSE
--rw-r--r--   0        0        0      357 2023-06-17 21:57:18.153299 tangens-0.1.0/README.md
--rw-r--r--   0        0        0      598 2023-06-17 23:33:16.615131 tangens-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-17 21:51:38.127553 tangens-0.1.0/tangens/__init__.py
--rw-r--r--   0        0        0       62 2023-06-17 21:51:38.131619 tangens-0.1.0/tangens/_num/__init__.py
--rw-r--r--   0        0        0     2514 2023-06-17 21:51:38.189304 tangens-0.1.0/tangens/_num/delta.py
--rw-r--r--   0        0        0     1459 2023-06-17 21:51:38.189633 tangens-0.1.0/tangens/_num/eval.py
--rw-r--r--   0        0        0      708 2023-06-17 21:51:38.189881 tangens-0.1.0/tangens/_num/expression.py
--rw-r--r--   0        0        0     2046 2023-06-17 21:51:38.131135 tangens-0.1.0/tangens/_num/num.py
--rw-r--r--   0        0        0      204 2023-06-17 21:51:38.128243 tangens-0.1.0/tangens/dual.py
--rw-r--r--   0        0        0       34 2023-06-17 21:51:38.116502 tangens-0.1.0/tangens/floats/__init__.py
--rw-r--r--   0        0        0     3247 2023-06-17 22:48:15.878538 tangens-0.1.0/tangens/floats/first.py
--rw-r--r--   0        0        0        0 2023-06-17 21:51:38.189997 tangens-0.1.0/tangens/py.typed
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 tangens-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-17 21:51:00.344118 tangens-0.1.1/LICENSE
+-rw-r--r--   0        0        0      357 2023-06-17 21:57:18.153299 tangens-0.1.1/README.md
+-rw-r--r--   0        0        0      598 2023-06-18 00:48:46.608638 tangens-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-18 00:37:39.660433 tangens-0.1.1/tangens/__init__.py
+-rw-r--r--   0        0        0       93 2023-06-18 00:38:03.918922 tangens-0.1.1/tangens/base/__init__.py
+-rw-r--r--   0        0        0     2584 2023-06-18 00:39:04.896331 tangens-0.1.1/tangens/base/delta.py
+-rw-r--r--   0        0        0      204 2023-06-17 21:51:38.128243 tangens-0.1.1/tangens/base/dual.py
+-rw-r--r--   0        0        0     1459 2023-06-17 21:51:38.189633 tangens-0.1.1/tangens/base/eval.py
+-rw-r--r--   0        0        0      708 2023-06-17 21:51:38.189881 tangens-0.1.1/tangens/base/expression.py
+-rw-r--r--   0        0        0     2045 2023-06-18 00:38:12.716462 tangens-0.1.1/tangens/base/num.py
+-rw-r--r--   0        0        0       34 2023-06-17 21:51:38.116502 tangens-0.1.1/tangens/floats/__init__.py
+-rw-r--r--   0        0        0     3432 2023-06-18 00:46:14.481325 tangens-0.1.1/tangens/floats/first.py
+-rw-r--r--   0        0        0        0 2023-06-17 21:51:38.189997 tangens-0.1.1/tangens/py.typed
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 tangens-0.1.1/PKG-INFO
```

### Comparing `tangens-0.1.0/LICENSE` & `tangens-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tangens-0.1.0/pyproject.toml` & `tangens-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tangens"
-version = "0.1.0"
+version = "0.1.1"
 repository = "https://github.com/cospectrum/tangens"
 description = "Automatic differentiation library for python"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `tangens-0.1.0/tangens/_num/delta.py` & `tangens-0.1.1/tangens/base/delta.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,17 @@
     @staticmethod
     def zero() -> Delta[T]:
         return Delta(Zero())
 
     def is_zero(self) -> bool:
         return self.expression is Zero()
 
+    def is_not_zero(self) -> bool:
+        return not self.is_zero()
+
     def clone(self) -> Delta[T]:
         return Delta(self.expression)
 
     def eval(
         self,
         one: T,
         add: AddFn[T],
```

### Comparing `tangens-0.1.0/tangens/_num/eval.py` & `tangens-0.1.1/tangens/base/eval.py`

 * *Files identical despite different names*

### Comparing `tangens-0.1.0/tangens/_num/expression.py` & `tangens-0.1.1/tangens/base/expression.py`

 * *Files identical despite different names*

### Comparing `tangens-0.1.0/tangens/_num/num.py` & `tangens-0.1.1/tangens/base/num.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from typing import Any, Hashable, TypeVar
 
-from ..dual import Dual
+from .dual import Dual
 from .delta import (
     Delta,
     NegFn,
     OneHot,
     Grad,
     AddFn,
     MultFn,
```

### Comparing `tangens-0.1.0/tangens/floats/first.py` & `tangens-0.1.1/tangens/floats/first.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import math
 from typing import Hashable
 
-from tangens._num import Num, Delta
+from tangens.base import Num, Delta
 
 
 F = Num[float] | float
 Grad = dict[Hashable, float]
 
 
 class Float(Num[float]):
@@ -107,7 +107,13 @@
         elif isinstance(base, Num):
             msg = "log with variable base is not currently supported"
             raise TypeError(msg)
         else:
             val = math.log(x, base)
             delta = d if d.is_zero() else d.scale(1 / (x * math.log(base)))
         return Float.new(val, delta)
+
+    def sqrt(self) -> Float:
+        a, b = self.astuple()
+        val = math.sqrt(a)
+        delta = b if b.is_zero() else b.scale(1 / (2 * val))
+        return Float.new(val, delta)
```

### Comparing `tangens-0.1.0/PKG-INFO` & `tangens-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangens
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatic differentiation library for python
 Home-page: https://github.com/cospectrum/tangens
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

