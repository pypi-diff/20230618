# Comparing `tmp/PyFixedReps-andnp-4.0.1.tar.gz` & `tmp/PyFixedReps-andnp-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFixedReps-andnp-4.0.1.tar", last modified: Wed May 24 03:45:34 2023, max compression
+gzip compressed data, was "PyFixedReps-andnp-4.0.2.tar", last modified: Sun Jun 18 04:47:36 2023, max compression
```

## Comparing `PyFixedReps-andnp-4.0.1.tar` & `PyFixedReps-andnp-4.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      181 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/BaseRepresentation.py
--rw-r--r--   0        0        0      751 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/RBF.py
--rw-r--r--   0        0        0     2869 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/TileCoder.py
--rw-r--r--   0        0        0      220 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/__init__.py
--rw-r--r--   0        0        0      477 2023-05-24 03:44:52.497887 PyFixedReps-andnp-4.0.1/PyFixedReps/_jit.py
--rw-r--r--   0        0        0     2931 2023-05-24 03:45:32.829988 PyFixedReps-andnp-4.0.1/README.md
--rw-r--r--   0        0        0      945 2023-05-24 03:45:32.833988 PyFixedReps-andnp-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 03:44:52.501887 PyFixedReps-andnp-4.0.1/tests/__init__.py
--rw-r--r--   0        0        0      437 2023-05-24 03:44:52.501887 PyFixedReps-andnp-4.0.1/tests/test_RBF.py
--rw-r--r--   0        0        0     3907 2023-05-24 03:44:52.501887 PyFixedReps-andnp-4.0.1/tests/test_TileCoder.py
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0      181 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/BaseRepresentation.py
+-rw-r--r--   0        0        0      751 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/RBF.py
+-rw-r--r--   0        0        0     2869 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/TileCoder.py
+-rw-r--r--   0        0        0      220 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/__init__.py
+-rw-r--r--   0        0        0      477 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/PyFixedReps/_jit.py
+-rw-r--r--   0        0        0     2931 2023-06-18 04:47:35.073283 PyFixedReps-andnp-4.0.2/README.md
+-rw-r--r--   0        0        0      945 2023-06-18 04:47:35.081283 PyFixedReps-andnp-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/tests/test_RBF.py
+-rw-r--r--   0        0        0     3907 2023-06-18 04:47:03.289198 PyFixedReps-andnp-4.0.2/tests/test_TileCoder.py
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 PyFixedReps-andnp-4.0.2/PKG-INFO
```

### Comparing `PyFixedReps-andnp-4.0.1/PyFixedReps/RBF.py` & `PyFixedReps-andnp-4.0.2/PyFixedReps/RBF.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.1/PyFixedReps/TileCoder.py` & `PyFixedReps-andnp-4.0.2/PyFixedReps/TileCoder.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.1/README.md` & `PyFixedReps-andnp-4.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==4.0.1
+pip install PyFixedReps-andnp==4.0.2
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
```

### Comparing `PyFixedReps-andnp-4.0.1/pyproject.toml` & `PyFixedReps-andnp-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "4.0.1"
+version = "4.0.2"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
     "README.md",
 ]
 
 [tool.pdm]
@@ -24,23 +24,23 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "PyFixedReps-andnp"
-version = "4.0.1"
+version = "4.0.2"
 description = ""
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numpy>=1.23.5",
     "numba>=0.56.4",
-    "tile-coder-rs==0.1.0",
+    "tile-coder-rs==0.3.1",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `PyFixedReps-andnp-4.0.1/tests/test_TileCoder.py` & `PyFixedReps-andnp-4.0.2/tests/test_TileCoder.py`

 * *Files identical despite different names*

### Comparing `PyFixedReps-andnp-4.0.1/PKG-INFO` & `PyFixedReps-andnp-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: PyFixedReps-andnp
-Version: 4.0.1
+Version: 4.0.2
 License: MIT
 Author-email: Andy Patterson <andnpatterson@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # PyFixedReps
 Short for: Python Fixed Representations.
 This is a collection of unit tested implementations of common fixed representations commonly used with linear (in features) RL systems.
 
 ## Installing
 Can be installed using `pip` by including this in your `requirements.txt`:
 ```
-pip install PyFixedReps-andnp==4.0.1
+pip install PyFixedReps-andnp==4.0.2
 ```
 I highly recommend specifying the version number when installing in order to ensure reproducibility of experiments.
 This library is fairly stable, so does not change often and there is little risk of missing an important change.
 
 ## Tile-coder
 ```python
 from PyFixedReps import TileCoder
```

