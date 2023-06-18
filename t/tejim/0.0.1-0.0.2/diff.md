# Comparing `tmp/tejim-0.0.1.tar.gz` & `tmp/tejim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tejim-0.0.1.tar", last modified: Sun Jun 18 17:52:29 2023, max compression
+gzip compressed data, was "tejim-0.0.2.tar", last modified: Sun Jun 18 18:28:32 2023, max compression
```

## Comparing `tejim-0.0.1.tar` & `tejim-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 spaceginner  (1000) spaceginner  (1000)        0 2023-06-18 17:52:29.353916 tejim-0.0.1/
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)      903 2023-06-18 17:52:29.353916 tejim-0.0.1/PKG-INFO
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)      651 2023-06-18 17:50:24.000000 tejim-0.0.1/pyproject.toml
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)      346 2023-06-16 18:04:42.000000 tejim-0.0.1/readme.md
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)       38 2023-06-18 17:52:29.353916 tejim-0.0.1/setup.cfg
-drwxr-xr-x   0 spaceginner  (1000) spaceginner  (1000)        0 2023-06-18 17:52:29.352916 tejim-0.0.1/tejim/
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)     2880 2023-06-16 18:18:20.000000 tejim-0.0.1/tejim/__init__.py
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)      692 2023-06-16 13:33:19.000000 tejim-0.0.1/tejim/data_convert.py
-drwxr-xr-x   0 spaceginner  (1000) spaceginner  (1000)        0 2023-06-18 17:52:29.353916 tejim-0.0.1/tejim.egg-info/
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)      903 2023-06-18 17:52:29.000000 tejim-0.0.1/tejim.egg-info/PKG-INFO
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)      180 2023-06-18 17:52:29.000000 tejim-0.0.1/tejim.egg-info/SOURCES.txt
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)        1 2023-06-18 17:52:29.000000 tejim-0.0.1/tejim.egg-info/dependency_links.txt
--rw-r--r--   0 spaceginner  (1000) spaceginner  (1000)        6 2023-06-18 17:52:29.000000 tejim-0.0.1/tejim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:28:32.282929 tejim-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-18 18:28:32.282929 tejim-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 18:28:22.000000 tejim-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 18:28:22.000000 tejim-0.0.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:28:32.282929 tejim-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:28:32.282929 tejim-0.0.2/tejim/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-18 18:28:22.000000 tejim-0.0.2/tejim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-18 18:28:22.000000 tejim-0.0.2/tejim/_data_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:28:32.282929 tejim-0.0.2/tejim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/top_level.txt
```

### Comparing `tejim-0.0.1/PKG-INFO` & `tejim-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tejim
-Version: 0.0.1
+Version: 0.0.2
 Summary: A configuration file standart the goal of which is to be simpistic, yet still robust enough.
 Author-email: "Ivan \"Spaceginner\"" <ivan.demian2009@gmail.com>
 Project-URL: Homepage, https://github.com/Spaceginner/tejim
 Project-URL: Bug Tracker, https://github.com/Spaceginner/tejim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tejim-0.0.1/pyproject.toml` & `tejim-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tejim"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ivan \"Spaceginner\"", email="ivan.demian2009@gmail.com" },
 ]
 description = "A configuration file standart the goal of which is to be simpistic, yet still robust enough."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `tejim-0.0.1/tejim/__init__.py` & `tejim-0.0.2/tejim/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import os
 
-from .data_convert import convert
+from ._data_convert import convert
 
 
 def parse(content: str) -> dict:
+    """
+    will parse contents of the tejim file and return its dictionary representation
+
+    :param content: the contents representing tejim file
+    :return: dictionary representation of the contents
+    """
     tokens = []
 
     # adapted from Spaceginner/opyn
     # splitter
     buffer, skip = "", 0
     for i in range(len(content)):
         if skip: skip -= 1; continue  # NOQA E702
@@ -58,14 +64,20 @@
             stored[tokens[i].strip()] = convert(tokens[i+2].strip())
             skip = 2
 
     return stored
 
 
 def generate(store: dict, _level: int = 0) -> str:
+    """
+    generates a tejim file based on the store dictionary
+
+    :param store: dictionary which has to be converted into a tejim file's representation
+    :return: contents of the tejim file representing the store dictionary
+    """
     contents = ""
 
     for key in store:
         if isinstance(store[key], str) and '\n' in store[key]:
             contents += "    " * _level + key + '!=\n\n' \
                         + store[key].strip() + '\n\n' \
                         + "    " * _level + f'\\{key}\n'
```

### Comparing `tejim-0.0.1/tejim/data_convert.py` & `tejim-0.0.2/tejim/_data_convert.py`

 * *Files identical despite different names*

### Comparing `tejim-0.0.1/tejim.egg-info/PKG-INFO` & `tejim-0.0.2/tejim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tejim
-Version: 0.0.1
+Version: 0.0.2
 Summary: A configuration file standart the goal of which is to be simpistic, yet still robust enough.
 Author-email: "Ivan \"Spaceginner\"" <ivan.demian2009@gmail.com>
 Project-URL: Homepage, https://github.com/Spaceginner/tejim
 Project-URL: Bug Tracker, https://github.com/Spaceginner/tejim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

