# Comparing `tmp/PyCodeBook-0.0.2.tar.gz` & `tmp/PyCodeBook-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCodeBook-0.0.2.tar", last modified: Sat Jun 17 18:32:31 2023, max compression
+gzip compressed data, was "PyCodeBook-0.0.3.tar", last modified: Sun Jun 18 04:00:17 2023, max compression
```

## Comparing `PyCodeBook-0.0.2.tar` & `PyCodeBook-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.454017 PyCodeBook-0.0.2/
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.452839 PyCodeBook-0.0.2/CodeBook/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      243 2023-06-17 18:32:13.000000 PyCodeBook-0.0.2/CodeBook/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PyCodeBook-0.0.2/CodeBook/__version__.py
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.453207 PyCodeBook-0.0.2/CodeBook/variable/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PyCodeBook-0.0.2/CodeBook/variable/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-01-07 02:10:39.000000 PyCodeBook-0.0.2/CodeBook/variable/__version__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PyCodeBook-0.0.2/CodeBook/variable/variable.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PyCodeBook-0.0.2/LICENSE
--rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PyCodeBook-0.0.2/MANIFEST.in
--rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-17 18:32:31.453903 PyCodeBook-0.0.2/PKG-INFO
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.453738 PyCodeBook-0.0.2/PyCodeBook.egg-info/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/PKG-INFO
--rw-r--r--   0 huangjiabao   (501) staff       (20)      312 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/SOURCES.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/dependency_links.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/top_level.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)       60 2023-06-17 18:30:39.000000 PyCodeBook-0.0.2/README.md
--rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:32:31.454059 PyCodeBook-0.0.2/setup.cfg
--rw-r--r--   0 huangjiabao   (501) staff       (20)     3894 2023-06-17 18:32:24.000000 PyCodeBook-0.0.2/setup.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.498589 PyCodeBook-0.0.3/
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.497302 PyCodeBook-0.0.3/CodeBook/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      243 2023-06-17 18:32:13.000000 PyCodeBook-0.0.3/CodeBook/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PyCodeBook-0.0.3/CodeBook/__version__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      305 2023-06-18 02:50:23.000000 PyCodeBook-0.0.3/CodeBook/engine.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.497698 PyCodeBook-0.0.3/CodeBook/variable/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PyCodeBook-0.0.3/CodeBook/variable/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-06-18 02:51:23.000000 PyCodeBook-0.0.3/CodeBook/variable/__version__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PyCodeBook-0.0.3/CodeBook/variable/variable.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PyCodeBook-0.0.3/LICENSE
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PyCodeBook-0.0.3/MANIFEST.in
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-18 04:00:17.498449 PyCodeBook-0.0.3/PKG-INFO
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-18 04:00:17.498254 PyCodeBook-0.0.3/PyCodeBook.egg-info/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/PKG-INFO
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      331 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-18 04:00:17.000000 PyCodeBook-0.0.3/PyCodeBook.egg-info/top_level.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       60 2023-06-17 18:30:39.000000 PyCodeBook-0.0.3/README.md
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-18 04:00:17.498637 PyCodeBook-0.0.3/setup.cfg
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     3894 2023-06-18 04:00:01.000000 PyCodeBook-0.0.3/setup.py
```

### Comparing `PyCodeBook-0.0.2/CodeBook/__version__.py` & `PyCodeBook-0.0.3/CodeBook/__version__.py`

 * *Files identical despite different names*

### Comparing `PyCodeBook-0.0.2/LICENSE` & `PyCodeBook-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCodeBook-0.0.2/PKG-INFO` & `PyCodeBook-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCodeBook
-Version: 0.0.2
+Version: 0.0.3
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyCodeBook-0.0.2/PyCodeBook.egg-info/PKG-INFO` & `PyCodeBook-0.0.3/PyCodeBook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCodeBook
-Version: 0.0.2
+Version: 0.0.3
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyCodeBook-0.0.2/setup.py` & `PyCodeBook-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyCodeBook'
 DESCRIPTION = '方便学员查询 Python 相关知识点,辅助考试。'
 URL = 'https://github.com/AndersonHJB/PyNoteBook'
 EMAIL = 'bornforthis@bornforthis.com'
 AUTHOR = 'Bornforthis'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

