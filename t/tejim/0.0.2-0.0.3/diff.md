# Comparing `tmp/tejim-0.0.2.tar.gz` & `tmp/tejim-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tejim-0.0.2.tar", last modified: Sun Jun 18 18:28:32 2023, max compression
+gzip compressed data, was "tejim-0.0.3.tar", last modified: Sun Jun 18 18:45:17 2023, max compression
```

## Comparing `tejim-0.0.2.tar` & `tejim-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:28:32.282929 tejim-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-18 18:28:32.282929 tejim-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 18:28:22.000000 tejim-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-18 18:28:22.000000 tejim-0.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:28:32.282929 tejim-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:28:32.282929 tejim-0.0.2/tejim/
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-18 18:28:22.000000 tejim-0.0.2/tejim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-18 18:28:22.000000 tejim-0.0.2/tejim/_data_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:28:32.282929 tejim-0.0.2/tejim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 18:28:32.000000 tejim-0.0.2/tejim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:45:17.239444 tejim-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 18:45:17.239444 tejim-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-18 18:45:07.000000 tejim-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-18 18:45:07.000000 tejim-0.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:45:17.239444 tejim-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:45:17.239444 tejim-0.0.3/tejim/
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-18 18:45:07.000000 tejim-0.0.3/tejim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-18 18:45:07.000000 tejim-0.0.3/tejim/_data_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:45:17.239444 tejim-0.0.3/tejim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 18:45:17.000000 tejim-0.0.3/tejim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-18 18:45:17.000000 tejim-0.0.3/tejim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:45:17.000000 tejim-0.0.3/tejim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 18:45:17.000000 tejim-0.0.3/tejim.egg-info/top_level.txt
```

### Comparing `tejim-0.0.2/PKG-INFO` & `tejim-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tejim
-Version: 0.0.2
-Summary: A configuration file standart the goal of which is to be simpistic, yet still robust enough.
+Version: 0.0.3
+Summary: the next YAML killer!!111!!!!111!
 Author-email: "Ivan \"Spaceginner\"" <ivan.demian2009@gmail.com>
 Project-URL: Homepage, https://github.com/Spaceginner/tejim
 Project-URL: Bug Tracker, https://github.com/Spaceginner/tejim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # tejim
 
 ## about
 
-this is a configuration file standart the goal of which is to be simpistic, yet still robust enough.
+a configuration file standart the goal of which is to be simpistic, yet still robust enough.
 
 its specification you can find [here](https://github.com/Spaceginner/tejim/wiki/Specification)
 
 ## features
 
 - dictionary
 - different value types
```

### Comparing `tejim-0.0.2/pyproject.toml` & `tejim-0.0.3/tejim.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,33 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "tejim"
-version = "0.0.2"
-authors = [
-  { name="Ivan \"Spaceginner\"", email="ivan.demian2009@gmail.com" },
-]
-description = "A configuration file standart the goal of which is to be simpistic, yet still robust enough."
-readme = "readme.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Spaceginner/tejim"
-"Bug Tracker" = "https://github.com/Spaceginner/tejim/issues"
+Metadata-Version: 2.1
+Name: tejim
+Version: 0.0.3
+Summary: the next YAML killer!!111!!!!111!
+Author-email: "Ivan \"Spaceginner\"" <ivan.demian2009@gmail.com>
+Project-URL: Homepage, https://github.com/Spaceginner/tejim
+Project-URL: Bug Tracker, https://github.com/Spaceginner/tejim/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# tejim
+
+## about
+
+a configuration file standart the goal of which is to be simpistic, yet still robust enough.
+
+its specification you can find [here](https://github.com/Spaceginner/tejim/wiki/Specification)
+
+## features
+
+- dictionary
+- different value types
+  - boolean
+  - integer
+  - floating-point
+  - string
+
+## why?
+
+why not™ duh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tejim-0.0.2/tejim/__init__.py` & `tejim-0.0.3/tejim/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+a configuration file standart the goal of which is to be simpistic, yet still robust enough.
+"""
+
 import os
 
 from ._data_convert import convert
 
 
 def parse(content: str) -> dict:
     """
```

### Comparing `tejim-0.0.2/tejim/_data_convert.py` & `tejim-0.0.3/tejim/_data_convert.py`

 * *Files identical despite different names*

