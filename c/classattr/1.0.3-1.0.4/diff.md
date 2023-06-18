# Comparing `tmp/classattr-1.0.3.tar.gz` & `tmp/classattr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classattr-1.0.3.tar", last modified: Sun Jun 18 18:04:32 2023, max compression
+gzip compressed data, was "classattr-1.0.4.tar", last modified: Sun Jun 18 18:16:48 2023, max compression
```

## Comparing `classattr-1.0.3.tar` & `classattr-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:04:32.269217 classattr-1.0.3/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.3/LICENSE
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:04:32.269217 classattr-1.0.3/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     2345 2023-06-18 17:53:49.000000 classattr-1.0.3/README.md
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:04:32.269217 classattr-1.0.3/classattr.egg-info/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/SOURCES.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/dependency_links.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 18:04:32.000000 classattr-1.0.3/classattr.egg-info/top_level.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 18:04:32.269217 classattr-1.0.3/setup.cfg
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      581 2023-06-18 18:04:18.000000 classattr-1.0.3/setup.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:16:48.164215 classattr-1.0.4/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.4/LICENSE
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:16:48.164215 classattr-1.0.4/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     2345 2023-06-18 17:53:49.000000 classattr-1.0.4/README.md
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:16:48.164215 classattr-1.0.4/classattr/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      107 2023-06-18 18:15:18.000000 classattr-1.0.4/classattr/__init__.py
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     8240 2023-06-18 18:03:56.000000 classattr-1.0.4/classattr/classattr.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 18:16:48.164215 classattr-1.0.4/classattr.egg-info/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     2755 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      203 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       10 2023-06-18 18:16:48.000000 classattr-1.0.4/classattr.egg-info/top_level.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 18:16:48.168216 classattr-1.0.4/setup.cfg
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      609 2023-06-18 18:14:44.000000 classattr-1.0.4/setup.py
```

### Comparing `classattr-1.0.3/LICENSE` & `classattr-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `classattr-1.0.3/PKG-INFO` & `classattr-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classattr
-Version: 1.0.3
+Version: 1.0.4
 Summary: classattr provides tools to manage class and object attributes
 Home-page: https://framagit.org/makeforartandscience/classattr
 Author: Thierry Dassé
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `classattr-1.0.3/README.md` & `classattr-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `classattr-1.0.3/classattr.egg-info/PKG-INFO` & `classattr-1.0.4/classattr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classattr
-Version: 1.0.3
+Version: 1.0.4
 Summary: classattr provides tools to manage class and object attributes
 Home-page: https://framagit.org/makeforartandscience/classattr
 Author: Thierry Dassé
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `classattr-1.0.3/setup.py` & `classattr-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,13 +6,14 @@
     version = classattr.__version__,
     author = classattr.__author__,
     url = 'https://framagit.org/makeforartandscience/classattr',
     license = classattr.__license__,
     description = 'classattr provides tools to manage class and object attributes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
+    packages=['classattr'],
     install_requires=[],
     classifiers = [
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
 )
```

