# Comparing `tmp/paraxial-0.9.0.tar.gz` & `tmp/paraxial-0.9.1.tar.gz`

## Comparing `paraxial-0.9.0.tar` & `paraxial-0.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 paraxial-0.9.0/src/paraxial/__about__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 paraxial-0.9.0/src/paraxial/__init__.py
--rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 paraxial-0.9.0/src/paraxial/equations.py
--rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 paraxial-0.9.0/src/paraxial/materials.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 paraxial-0.9.0/src/paraxial/sources.py
--rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 paraxial-0.9.0/src/paraxial/surfaces.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_abcd_matrix.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_composite_surfaces.py
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_equations.py
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_gaussian_beam.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_materials.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_numpy_sympy_integration.py
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_ray.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 paraxial-0.9.0/tests/test_surfaces.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 paraxial-0.9.0/.gitignore
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 paraxial-0.9.0/LICENSE
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 paraxial-0.9.0/README.md
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 paraxial-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 paraxial-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 paraxial-0.9.1/src/paraxial/__about__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 paraxial-0.9.1/src/paraxial/__init__.py
+-rw-r--r--   0        0        0    10908 2020-02-02 00:00:00.000000 paraxial-0.9.1/src/paraxial/equations.py
+-rw-r--r--   0        0        0     8173 2020-02-02 00:00:00.000000 paraxial-0.9.1/src/paraxial/materials.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 paraxial-0.9.1/src/paraxial/sources.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 paraxial-0.9.1/src/paraxial/surfaces.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_abcd_matrix.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_composite_surfaces.py
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_equations.py
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_gaussian_beam.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_materials.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_numpy_sympy_integration.py
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_ray.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 paraxial-0.9.1/tests/test_surfaces.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 paraxial-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 paraxial-0.9.1/LICENSE
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 paraxial-0.9.1/README.md
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 paraxial-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 paraxial-0.9.1/PKG-INFO
```

### Comparing `paraxial-0.9.0/src/paraxial/equations.py` & `paraxial-0.9.1/src/paraxial/equations.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/src/paraxial/materials.py` & `paraxial-0.9.1/src/paraxial/materials.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/src/paraxial/sources.py` & `paraxial-0.9.1/src/paraxial/sources.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/src/paraxial/surfaces.py` & `paraxial-0.9.1/src/paraxial/surfaces.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_abcd_matrix.py` & `paraxial-0.9.1/tests/test_abcd_matrix.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_composite_surfaces.py` & `paraxial-0.9.1/tests/test_composite_surfaces.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_equations.py` & `paraxial-0.9.1/tests/test_equations.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_gaussian_beam.py` & `paraxial-0.9.1/tests/test_gaussian_beam.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_materials.py` & `paraxial-0.9.1/tests/test_materials.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_numpy_sympy_integration.py` & `paraxial-0.9.1/tests/test_numpy_sympy_integration.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_ray.py` & `paraxial-0.9.1/tests/test_ray.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/tests/test_surfaces.py` & `paraxial-0.9.1/tests/test_surfaces.py`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/.gitignore` & `paraxial-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `paraxial-0.9.0/pyproject.toml` & `paraxial-0.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "paraxial"
 dynamic = ["version"]
 description = 'A library for nontrivial paraxial optics calculations'
 readme = "README.md"
 requires-python = ">=3.8"
-license = "BSD-3-Clause"
+license = "MIT"
 keywords = []
 authors = [
   { name = "danieldmulkey", email = "danieldmulkey@users.noreply.github.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
@@ -22,17 +22,17 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['numpy', 'sympy']
 
 [project.urls]
-Documentation = "https://github.com/unknown/paraxial#readme"
-Issues = "https://github.com/unknown/paraxial/issues"
-Source = "https://github.com/unknown/paraxial"
+Documentation = "https://github.com/danieldmulkey/paraxial#readme"
+Issues = "https://github.com/danieldmulkey/paraxial/issues"
+Source = "https://github.com/danieldmulkey/paraxial"
 
 [tool.hatch.version]
 path = "src/paraxial/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
```

### Comparing `paraxial-0.9.0/PKG-INFO` & `paraxial-0.9.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: paraxial
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for nontrivial paraxial optics calculations
-Project-URL: Documentation, https://github.com/unknown/paraxial#readme
-Project-URL: Issues, https://github.com/unknown/paraxial/issues
-Project-URL: Source, https://github.com/unknown/paraxial
+Project-URL: Documentation, https://github.com/danieldmulkey/paraxial#readme
+Project-URL: Issues, https://github.com/danieldmulkey/paraxial/issues
+Project-URL: Source, https://github.com/danieldmulkey/paraxial
 Author-email: danieldmulkey <danieldmulkey@users.noreply.github.com>
-License-Expression: BSD-3-Clause
+License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

