# Comparing `tmp/classattr-1.0.2.tar.gz` & `tmp/classattr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classattr-1.0.2.tar", last modified: Sun Jun 18 17:25:46 2023, max compression
+gzip compressed data, was "classattr-1.0.3.tar", last modified: Sun Jun 18 18:04:32 2023, max compression
```

## Comparing `classattr-1.0.2.tar` & `classattr-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 17:25:46.885137 classattr-1.0.2/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.2/LICENSE
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1460 2023-06-18 17:25:46.885137 classattr-1.0.2/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1050 2023-06-18 15:26:45.000000 classattr-1.0.2/README.md
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 17:25:46.885137 classattr-1.0.2/classattr.egg-info/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1460 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/SOURCES.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/dependency_links.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/top_level.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 17:25:46.885137 classattr-1.0.2/setup.cfg
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      539 2023-06-18 17:18:31.000000 classattr-1.0.2/setup.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:04:32.269217 classattr-1.0.3/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.3/LICENSE
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:04:32.269217 classattr-1.0.3/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     2345 2023-06-18 17:53:49.000000 classattr-1.0.3/README.md
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:04:32.269217 classattr-1.0.3/classattr.egg-info/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/top_level.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 18:04:32.269217 classattr-1.0.3/setup.cfg
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      581 2023-06-18 18:04:18.000000 classattr-1.0.3/setup.py
```

### Comparing `classattr-1.0.2/LICENSE` & `classattr-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `classattr-1.0.2/setup.py` & `classattr-1.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import setuptools
+import classattr
 
 setuptools.setup(
     name = 'classattr',
-    version = '1.0.2',
-    author = 'Thierry Dassé',
+    version = classattr.__version__,
+    author = classattr.__author__,
     url = 'https://framagit.org/makeforartandscience/classattr',
-    license = 'MIT License',
+    license = classattr.__license__,
     description = 'classattr provides tools to manage class and object attributes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[],
     classifiers = [
-        "Programming Language :: Python :: 3",
-         "Operating System :: OS Independent",
+        'Programming Language :: Python :: 3',
+        'Operating System :: OS Independent',
     ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

