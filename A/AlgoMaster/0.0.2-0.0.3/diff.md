# Comparing `tmp/AlgoMaster-0.0.2.tar.gz` & `tmp/AlgoMaster-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoMaster-0.0.2.tar", last modified: Sat Jun 17 16:55:40 2023, max compression
+gzip compressed data, was "AlgoMaster-0.0.3.tar", last modified: Sun Jun 18 13:57:21 2023, max compression
```

## Comparing `AlgoMaster-0.0.2.tar` & `AlgoMaster-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:55:40.036460 AlgoMaster-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-06-17 16:55:39.922454 AlgoMaster-0.0.2/AlgoMaster/
--rw-rw-rw-   0        0        0       29 2023-06-17 16:53:15.000000 AlgoMaster-0.0.2/AlgoMaster/__init__.py
--rw-rw-rw-   0        0        0      342 2023-06-17 16:54:46.000000 AlgoMaster-0.0.2/AlgoMaster/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:55:40.022462 AlgoMaster-0.0.2/AlgoMaster.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-17 16:55:39.000000 AlgoMaster-0.0.2/AlgoMaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-17 16:55:39.000000 AlgoMaster-0.0.2/AlgoMaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:55:39.000000 AlgoMaster-0.0.2/AlgoMaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-17 16:55:39.000000 AlgoMaster-0.0.2/AlgoMaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 16:55:39.000000 AlgoMaster-0.0.2/AlgoMaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      534 2023-06-17 16:55:40.025461 AlgoMaster-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-17 16:12:45.000000 AlgoMaster-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 16:55:40.037463 AlgoMaster-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-06-17 16:53:55.000000 AlgoMaster-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:57:21.360303 AlgoMaster-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-06-18 13:57:21.190186 AlgoMaster-0.0.3/AlgoMaster/
+-rw-rw-rw-   0        0        0       35 2023-06-17 17:09:22.000000 AlgoMaster-0.0.3/AlgoMaster/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-06-18 13:42:53.000000 AlgoMaster-0.0.3/AlgoMaster/classifier.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:57:21.356303 AlgoMaster-0.0.3/AlgoMaster.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-18 13:57:21.000000 AlgoMaster-0.0.3/AlgoMaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-18 13:57:21.000000 AlgoMaster-0.0.3/AlgoMaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:57:21.000000 AlgoMaster-0.0.3/AlgoMaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-18 13:57:21.000000 AlgoMaster-0.0.3/AlgoMaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 13:57:21.000000 AlgoMaster-0.0.3/AlgoMaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      534 2023-06-18 13:57:21.358303 AlgoMaster-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:12:45.000000 AlgoMaster-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:57:21.361304 AlgoMaster-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-06-18 13:57:07.000000 AlgoMaster-0.0.3/setup.py
```

### Comparing `AlgoMaster-0.0.2/AlgoMaster.egg-info/PKG-INFO` & `AlgoMaster-0.0.3/AlgoMaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.0.2
+Version: 0.0.3
 Summary: Learning models make simple
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: python,classification,regression,machine learning models,hyper parameter turning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgoMaster-0.0.2/PKG-INFO` & `AlgoMaster-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgoMaster
-Version: 0.0.2
+Version: 0.0.3
 Summary: Learning models make simple
 Author: sajo sam
 Author-email: <sajosamambalakara@gmail.com>
 Keywords: python,classification,regression,machine learning models,hyper parameter turning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AlgoMaster-0.0.2/setup.py` & `AlgoMaster-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Learning models make simple'
 # LONG_DESCRIPTION = '''
 #                                         Learning models
 #                                     (single-file, easy-to-use)'''
 
 # Setting up
 setup(
```

