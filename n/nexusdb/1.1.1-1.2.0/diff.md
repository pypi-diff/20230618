# Comparing `tmp/nexusdb-1.1.1.tar.gz` & `tmp/nexusdb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexusdb-1.1.1.tar", last modified: Fri Jun 16 19:40:07 2023, max compression
+gzip compressed data, was "nexusdb-1.2.0.tar", last modified: Sun Jun 18 10:03:58 2023, max compression
```

## Comparing `nexusdb-1.1.1.tar` & `nexusdb-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 19:40:07.626627 nexusdb-1.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-16 19:40:07.626627 nexusdb-1.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.1.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 19:40:07.626627 nexusdb-1.1.1/nexusdb.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-16 19:40:07.000000 nexusdb-1.1.1/nexusdb.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      183 2023-06-16 19:40:07.000000 nexusdb-1.1.1/nexusdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-16 19:40:07.000000 nexusdb-1.1.1/nexusdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-06-16 19:40:07.000000 nexusdb-1.1.1/nexusdb.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-16 19:40:07.000000 nexusdb-1.1.1/nexusdb.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17003 2023-06-16 10:41:15.000000 nexusdb-1.1.1/nexusdb.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-16 19:40:07.626627 nexusdb-1.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1008 2023-06-16 19:39:45.000000 nexusdb-1.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 10:03:58.412605 nexusdb-1.2.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-18 10:03:58.412605 nexusdb-1.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      261 2023-06-16 19:39:12.000000 nexusdb-1.2.0/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 10:03:58.412605 nexusdb-1.2.0/nexusdb.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      183 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-06-18 10:03:58.000000 nexusdb-1.2.0/nexusdb.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13905 2023-06-18 10:02:05.000000 nexusdb-1.2.0/nexusdb.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-18 10:03:58.412605 nexusdb-1.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      990 2023-06-18 10:02:10.000000 nexusdb-1.2.0/setup.py
```

### Comparing `nexusdb-1.1.1/PKG-INFO` & `nexusdb-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.1.1
+Version: 1.2.0
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.1.1/nexusdb.egg-info/PKG-INFO` & `nexusdb-1.2.0/nexusdb.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexusdb
-Version: 1.1.1
+Version: 1.2.0
 Summary: A lightweight JSON-based database system for Python
 Home-page: https://github.com/E491K8/nexusdb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nexusdb-1.1.1/setup.py` & `nexusdb-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nexusdb",
-    version="1.1.1",
+    version="1.2.0",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     description="A lightweight JSON-based database system for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/nexusdb",
     packages=find_packages(),
     py_modules=['nexusdb'],
         install_requires=[
-        "bcrypt",
         "uuid",
         "pytz",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

