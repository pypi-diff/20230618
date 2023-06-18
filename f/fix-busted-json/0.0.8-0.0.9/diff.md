# Comparing `tmp/fix-busted-json-0.0.8.tar.gz` & `tmp/fix-busted-json-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fix-busted-json-0.0.8.tar", last modified: Sun Jun 18 12:58:23 2023, max compression
+gzip compressed data, was "dist/fix-busted-json-0.0.9.tar", last modified: Sun Jun 18 13:00:55 2023, max compression
```

## Comparing `fix-busted-json-0.0.8.tar` & `fix-busted-json-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1069 2023-06-17 15:46:10.000000 fix-busted-json-0.0.8/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)     3367 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3013 2023-06-18 12:56:37.000000 fix-busted-json-0.0.8/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1212 2023-06-18 12:57:03.000000 fix-busted-json-0.0.8/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     3367 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      255 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       16 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    20566 2023-06-18 12:08:01.000000 fix-busted-json-0.0.8/src/fix_busted_json.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/tests/
--rwxrwxr-x   0 tim       (1000) tim       (1000)      731 2023-06-18 12:11:37.000000 fix-busted-json-0.0.8/tests/testfocus.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    15939 2023-06-18 12:11:29.000000 fix-busted-json-0.0.8/tests/tests.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1069 2023-06-17 15:46:10.000000 fix-busted-json-0.0.9/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3408 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3054 2023-06-18 13:00:28.000000 fix-busted-json-0.0.9/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1212 2023-06-18 13:00:50.000000 fix-busted-json-0.0.9/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/src/fix_busted_json.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3408 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/src/fix_busted_json.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      255 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/src/fix_busted_json.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/src/fix_busted_json.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       16 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/src/fix_busted_json.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    20566 2023-06-18 12:08:01.000000 fix-busted-json-0.0.9/src/fix_busted_json.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 13:00:55.000000 fix-busted-json-0.0.9/tests/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      731 2023-06-18 12:11:37.000000 fix-busted-json-0.0.9/tests/testfocus.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    15939 2023-06-18 12:11:29.000000 fix-busted-json-0.0.9/tests/tests.py
```

### Comparing `fix-busted-json-0.0.8/LICENSE` & `fix-busted-json-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fix-busted-json-0.0.8/PKG-INFO` & `fix-busted-json-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix-busted-json
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fixes broken JSON string objects
 Author: Tim Buckland
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -28,14 +28,16 @@
 -   Missing commas between key-value pairs and array elements
 -   Trailing comma after last key-value pair
 -   Concatenation of string fields
 -   Replace Python True/False/None with JSON true/false/null
 
 Utility functions are also provided for finding JSON objects in text.
 
+https://github.com/Qarj/fix-busted-json
+
 https://pypi.org/project/fix-busted-json
 
 ## Quickstart
 
 ```sh
 pip install fix-busted-json
 ```
```

### Comparing `fix-busted-json-0.0.8/README.md` & `fix-busted-json-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 -   Missing commas between key-value pairs and array elements
 -   Trailing comma after last key-value pair
 -   Concatenation of string fields
 -   Replace Python True/False/None with JSON true/false/null
 
 Utility functions are also provided for finding JSON objects in text.
 
+https://github.com/Qarj/fix-busted-json
+
 https://pypi.org/project/fix-busted-json
 
 ## Quickstart
 
 ```sh
 pip install fix-busted-json
 ```
```

### Comparing `fix-busted-json-0.0.8/setup.py` & `fix-busted-json-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fix-busted-json",                 # This is the name of the package
-    version="0.0.8",                        # The initial release version
+    version="0.0.9",                        # The initial release version
     author="Tim Buckland",                  # Full name of the author
     description="Fixes broken JSON string objects",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `fix-busted-json-0.0.8/src/fix_busted_json.egg-info/PKG-INFO` & `fix-busted-json-0.0.9/src/fix_busted_json.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix-busted-json
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fixes broken JSON string objects
 Author: Tim Buckland
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -28,14 +28,16 @@
 -   Missing commas between key-value pairs and array elements
 -   Trailing comma after last key-value pair
 -   Concatenation of string fields
 -   Replace Python True/False/None with JSON true/false/null
 
 Utility functions are also provided for finding JSON objects in text.
 
+https://github.com/Qarj/fix-busted-json
+
 https://pypi.org/project/fix-busted-json
 
 ## Quickstart
 
 ```sh
 pip install fix-busted-json
 ```
```

### Comparing `fix-busted-json-0.0.8/src/fix_busted_json.py` & `fix-busted-json-0.0.9/src/fix_busted_json.py`

 * *Files identical despite different names*

### Comparing `fix-busted-json-0.0.8/tests/testfocus.py` & `fix-busted-json-0.0.9/tests/testfocus.py`

 * *Files identical despite different names*

### Comparing `fix-busted-json-0.0.8/tests/tests.py` & `fix-busted-json-0.0.9/tests/tests.py`

 * *Files identical despite different names*

