# Comparing `tmp/fix-busted-json-0.0.7.tar.gz` & `tmp/fix-busted-json-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fix-busted-json-0.0.7.tar", last modified: Sun Jun 18 12:17:50 2023, max compression
+gzip compressed data, was "dist/fix-busted-json-0.0.8.tar", last modified: Sun Jun 18 12:58:23 2023, max compression
```

## Comparing `fix-busted-json-0.0.7.tar` & `fix-busted-json-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/
--rw-rw-r--   0 tim       (1000) tim       (1000)     1069 2023-06-17 15:46:10.000000 fix-busted-json-0.0.7/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)      403 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)       49 2023-06-18 10:26:43.000000 fix-busted-json-0.0.7/README.md
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)     1212 2023-06-18 12:12:09.000000 fix-busted-json-0.0.7/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/src/fix_busted_json.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)      403 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/src/fix_busted_json.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      255 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/src/fix_busted_json.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/src/fix_busted_json.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       16 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/src/fix_busted_json.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    20566 2023-06-18 12:08:01.000000 fix-busted-json-0.0.7/src/fix_busted_json.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:17:50.000000 fix-busted-json-0.0.7/tests/
--rwxrwxr-x   0 tim       (1000) tim       (1000)      731 2023-06-18 12:11:37.000000 fix-busted-json-0.0.7/tests/testfocus.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    15939 2023-06-18 12:11:29.000000 fix-busted-json-0.0.7/tests/tests.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1069 2023-06-17 15:46:10.000000 fix-busted-json-0.0.8/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3367 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3013 2023-06-18 12:56:37.000000 fix-busted-json-0.0.8/README.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1212 2023-06-18 12:57:03.000000 fix-busted-json-0.0.8/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3367 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      255 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       16 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/src/fix_busted_json.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    20566 2023-06-18 12:08:01.000000 fix-busted-json-0.0.8/src/fix_busted_json.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-18 12:58:23.000000 fix-busted-json-0.0.8/tests/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      731 2023-06-18 12:11:37.000000 fix-busted-json-0.0.8/tests/testfocus.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    15939 2023-06-18 12:11:29.000000 fix-busted-json-0.0.8/tests/tests.py
```

### Comparing `fix-busted-json-0.0.7/LICENSE` & `fix-busted-json-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fix-busted-json-0.0.7/setup.py` & `fix-busted-json-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fix-busted-json",                 # This is the name of the package
-    version="0.0.7",                        # The initial release version
+    version="0.0.8",                        # The initial release version
     author="Tim Buckland",                  # Full name of the author
     description="Fixes broken JSON string objects",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `fix-busted-json-0.0.7/src/fix_busted_json.py` & `fix-busted-json-0.0.8/src/fix_busted_json.py`

 * *Files identical despite different names*

### Comparing `fix-busted-json-0.0.7/tests/testfocus.py` & `fix-busted-json-0.0.8/tests/testfocus.py`

 * *Files identical despite different names*

### Comparing `fix-busted-json-0.0.7/tests/tests.py` & `fix-busted-json-0.0.8/tests/tests.py`

 * *Files identical despite different names*

