# Comparing `tmp/pyfiredb-0.0.3.tar.gz` & `tmp/pyfiredb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfiredb-0.0.3.tar", last modified: Sun Jun 18 04:00:42 2023, max compression
+gzip compressed data, was "pyfiredb-0.0.4.tar", last modified: Sun Jun 18 04:15:20 2023, max compression
```

## Comparing `pyfiredb-0.0.3.tar` & `pyfiredb-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:00:42.406646 pyfiredb-0.0.3/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 pyfiredb-0.0.3/LICENSE.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-18 04:00:42.406646 pyfiredb-0.0.3/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)     1295 2023-06-09 02:20:03.000000 pyfiredb-0.0.3/README.md
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:00:42.402646 pyfiredb-0.0.3/pyfiredb/
--rw-rw-r--   0 andres    (1000) andres    (1000)      128 2023-06-09 02:15:32.000000 pyfiredb-0.0.3/pyfiredb/__init__.py
--rw-rw-r--   0 andres    (1000) andres    (1000)     1776 2023-06-18 03:57:48.000000 pyfiredb-0.0.3/pyfiredb/database.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      666 2023-06-09 00:39:10.000000 pyfiredb-0.0.3/pyfiredb/session.py
--rw-rw-r--   0 andres    (1000) andres    (1000)      299 2023-06-09 21:36:30.000000 pyfiredb-0.0.3/pyfiredb/settings.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:00:42.406646 pyfiredb-0.0.3/pyfiredb.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-18 04:00:42.000000 pyfiredb-0.0.3/pyfiredb.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      272 2023-06-18 04:00:42.000000 pyfiredb-0.0.3/pyfiredb.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-18 04:00:42.000000 pyfiredb-0.0.3/pyfiredb.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-18 04:00:42.000000 pyfiredb-0.0.3/pyfiredb.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-18 04:00:42.000000 pyfiredb-0.0.3/pyfiredb.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-18 04:00:42.406646 pyfiredb-0.0.3/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)     1089 2023-06-18 04:00:35.000000 pyfiredb-0.0.3/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:15:20.143664 pyfiredb-0.0.4/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1084 2023-03-09 17:21:54.000000 pyfiredb-0.0.4/LICENSE.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-18 04:15:20.139664 pyfiredb-0.0.4/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1295 2023-06-09 02:20:03.000000 pyfiredb-0.0.4/README.md
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:15:20.139664 pyfiredb-0.0.4/pyfiredb/
+-rw-rw-r--   0 andres    (1000) andres    (1000)      128 2023-06-09 02:15:32.000000 pyfiredb-0.0.4/pyfiredb/__init__.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1776 2023-06-18 03:57:48.000000 pyfiredb-0.0.4/pyfiredb/database.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      666 2023-06-09 00:39:10.000000 pyfiredb-0.0.4/pyfiredb/session.py
+-rw-rw-r--   0 andres    (1000) andres    (1000)      299 2023-06-09 21:36:30.000000 pyfiredb-0.0.4/pyfiredb/settings.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-18 04:15:20.139664 pyfiredb-0.0.4/pyfiredb.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1970 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      272 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        9 2023-06-18 04:15:20.000000 pyfiredb-0.0.4/pyfiredb.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-18 04:15:20.143664 pyfiredb-0.0.4/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1089 2023-06-18 04:15:08.000000 pyfiredb-0.0.4/setup.py
```

### Comparing `pyfiredb-0.0.3/LICENSE.txt` & `pyfiredb-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.3/PKG-INFO` & `pyfiredb-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfiredb
-Version: 0.0.3
+Version: 0.0.4
 Summary: pyfire is a package that simplifies querying with Pyrebase,    making interactions with Firebase databases effortless.
 Home-page: https://github.com/andresroh/pyfire
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
```

### Comparing `pyfiredb-0.0.3/README.md` & `pyfiredb-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.3/pyfiredb/database.py` & `pyfiredb-0.0.4/pyfiredb/database.py`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.3/pyfiredb/session.py` & `pyfiredb-0.0.4/pyfiredb/session.py`

 * *Files identical despite different names*

### Comparing `pyfiredb-0.0.3/pyfiredb.egg-info/PKG-INFO` & `pyfiredb-0.0.4/pyfiredb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfiredb
-Version: 0.0.3
+Version: 0.0.4
 Summary: pyfire is a package that simplifies querying with Pyrebase,    making interactions with Firebase databases effortless.
 Home-page: https://github.com/andresroh/pyfire
 Author: Camilo Andrés Rodríguez
 Author-email: andres.roh@gmail.com
 License: MIT
 Keywords: python,alegra,alegra.com
 Platform: UNKNOWN
```

### Comparing `pyfiredb-0.0.3/setup.py` & `pyfiredb-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'pyfire is a package that simplifies querying with Pyrebase,\
     making interactions with Firebase databases effortless.'
 PACKAGE_NAME = 'pyfiredb'
 AUTHOR = 'Camilo Andrés Rodríguez'
 EMAIL = 'andres.roh@gmail.com'
 GITHUB_URL = 'https://github.com/andresroh/pyfire'
```

