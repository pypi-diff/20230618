# Comparing `tmp/tangens-0.1.1.tar.gz` & `tmp/tangens-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangens-0.1.1.tar", max compression
+gzip compressed data, was "tangens-0.1.2.tar", max compression
```

## Comparing `tangens-0.1.1.tar` & `tangens-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-17 21:51:00.344118 tangens-0.1.1/LICENSE
--rw-r--r--   0        0        0      357 2023-06-17 21:57:18.153299 tangens-0.1.1/README.md
--rw-r--r--   0        0        0      598 2023-06-18 00:48:46.608638 tangens-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       64 2023-06-18 00:37:39.660433 tangens-0.1.1/tangens/__init__.py
--rw-r--r--   0        0        0       93 2023-06-18 00:38:03.918922 tangens-0.1.1/tangens/base/__init__.py
--rw-r--r--   0        0        0     2584 2023-06-18 00:39:04.896331 tangens-0.1.1/tangens/base/delta.py
--rw-r--r--   0        0        0      204 2023-06-17 21:51:38.128243 tangens-0.1.1/tangens/base/dual.py
--rw-r--r--   0        0        0     1459 2023-06-17 21:51:38.189633 tangens-0.1.1/tangens/base/eval.py
--rw-r--r--   0        0        0      708 2023-06-17 21:51:38.189881 tangens-0.1.1/tangens/base/expression.py
--rw-r--r--   0        0        0     2045 2023-06-18 00:38:12.716462 tangens-0.1.1/tangens/base/num.py
--rw-r--r--   0        0        0       34 2023-06-17 21:51:38.116502 tangens-0.1.1/tangens/floats/__init__.py
--rw-r--r--   0        0        0     3432 2023-06-18 00:46:14.481325 tangens-0.1.1/tangens/floats/first.py
--rw-r--r--   0        0        0        0 2023-06-17 21:51:38.189997 tangens-0.1.1/tangens/py.typed
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 tangens-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-17 21:51:00.344118 tangens-0.1.2/LICENSE
+-rw-r--r--   0        0        0      357 2023-06-17 21:57:18.153299 tangens-0.1.2/README.md
+-rw-r--r--   0        0        0      598 2023-06-18 01:11:54.749492 tangens-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-06-18 00:37:39.660433 tangens-0.1.2/tangens/__init__.py
+-rw-r--r--   0        0        0       93 2023-06-18 00:38:03.918922 tangens-0.1.2/tangens/base/__init__.py
+-rw-r--r--   0        0        0     2584 2023-06-18 00:39:04.896331 tangens-0.1.2/tangens/base/delta.py
+-rw-r--r--   0        0        0      204 2023-06-17 21:51:38.128243 tangens-0.1.2/tangens/base/dual.py
+-rw-r--r--   0        0        0     1459 2023-06-17 21:51:38.189633 tangens-0.1.2/tangens/base/eval.py
+-rw-r--r--   0        0        0      708 2023-06-17 21:51:38.189881 tangens-0.1.2/tangens/base/expression.py
+-rw-r--r--   0        0        0     2045 2023-06-18 00:38:12.716462 tangens-0.1.2/tangens/base/num.py
+-rw-r--r--   0        0        0       34 2023-06-17 21:51:38.116502 tangens-0.1.2/tangens/floats/__init__.py
+-rw-r--r--   0        0        0     3607 2023-06-18 01:12:15.509711 tangens-0.1.2/tangens/floats/first.py
+-rw-r--r--   0        0        0        0 2023-06-17 21:51:38.189997 tangens-0.1.2/tangens/py.typed
+-rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 tangens-0.1.2/PKG-INFO
```

### Comparing `tangens-0.1.1/LICENSE` & `tangens-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tangens-0.1.1/pyproject.toml` & `tangens-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tangens"
-version = "0.1.1"
+version = "0.1.2"
 repository = "https://github.com/cospectrum/tangens"
 description = "Automatic differentiation library for python"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `tangens-0.1.1/tangens/base/delta.py` & `tangens-0.1.2/tangens/base/delta.py`

 * *Files identical despite different names*

### Comparing `tangens-0.1.1/tangens/base/eval.py` & `tangens-0.1.2/tangens/base/eval.py`

 * *Files identical despite different names*

### Comparing `tangens-0.1.1/tangens/base/expression.py` & `tangens-0.1.2/tangens/base/expression.py`

 * *Files identical despite different names*

### Comparing `tangens-0.1.1/tangens/base/num.py` & `tangens-0.1.2/tangens/base/num.py`

 * *Files identical despite different names*

### Comparing `tangens-0.1.1/tangens/floats/first.py` & `tangens-0.1.2/tangens/floats/first.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,9 +111,15 @@
             val = math.log(x, base)
             delta = d if d.is_zero() else d.scale(1 / (x * math.log(base)))
         return Float.new(val, delta)
 
     def sqrt(self) -> Float:
         a, b = self.astuple()
         val = math.sqrt(a)
-        delta = b if b.is_zero() else b.scale(1 / (2 * val))
+        delta = b if b.is_zero() else b.scale(0.5 / val)
         return Float.new(val, delta)
+
+    def tan(self) -> Float:
+        a, b = self.astuple()
+        tg = math.tan(a)
+        delta = b if b.is_zero() else b.scale(1 + tg * tg)
+        return Float.new(tg, delta)
```

### Comparing `tangens-0.1.1/PKG-INFO` & `tangens-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangens
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automatic differentiation library for python
 Home-page: https://github.com/cospectrum/tangens
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

