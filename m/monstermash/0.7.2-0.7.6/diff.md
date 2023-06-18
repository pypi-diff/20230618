# Comparing `tmp/monstermash-0.7.2.tar.gz` & `tmp/monstermash-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-0.7.2.tar", max compression
+gzip compressed data, was "monstermash-0.7.6.tar", max compression
```

## Comparing `monstermash-0.7.2.tar` & `monstermash-0.7.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1366 2023-04-06 10:44:23.532484 monstermash-0.7.2/README.md
--rw-r--r--   0        0        0     1046 2023-04-06 10:44:23.532484 monstermash-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       86 2023-04-06 10:44:23.532484 monstermash-0.7.2/src/monstermash/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-06 10:44:23.532484 monstermash-0.7.2/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1530 2023-04-06 10:44:23.536484 monstermash-0.7.2/src/monstermash/crypt.py
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1366 2023-06-18 05:34:43.840450 monstermash-0.7.6/README.md
+-rw-r--r--   0        0        0     1046 2023-06-18 05:34:43.840450 monstermash-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-18 05:34:43.840450 monstermash-0.7.6/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     1968 2023-06-18 05:34:43.840450 monstermash-0.7.6/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1530 2023-06-18 05:34:43.840450 monstermash-0.7.6/src/monstermash/crypt.py
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-0.7.6/PKG-INFO
```

### Comparing `monstermash-0.7.2/README.md` & `monstermash-0.7.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 0.7.2
+> 1️⃣ version: 0.7.6
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-0.7.2/pyproject.toml` & `monstermash-0.7.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monstermash"
-version = "0.7.2"
+version = "0.7.6"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `monstermash-0.7.2/src/monstermash/__main__.py` & `monstermash-0.7.6/src/monstermash/__main__.py`

 * *Files identical despite different names*

### Comparing `monstermash-0.7.2/src/monstermash/crypt.py` & `monstermash-0.7.6/src/monstermash/crypt.py`

 * *Files identical despite different names*

### Comparing `monstermash-0.7.2/PKG-INFO` & `monstermash-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 0.7.2
+Version: 0.7.6
 Summary: 
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ##  🧟 Monstermash
 
-> 1️⃣ version: 0.7.2
+> 1️⃣ version: 0.7.6
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

