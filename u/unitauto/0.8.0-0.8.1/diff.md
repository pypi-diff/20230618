# Comparing `tmp/unitauto-0.8.0.tar.gz` & `tmp/unitauto-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitauto-0.8.0.tar", last modified: Sun Jun 18 15:39:54 2023, max compression
+gzip compressed data, was "unitauto-0.8.1.tar", last modified: Sun Jun 18 15:57:45 2023, max compression
```

## Comparing `unitauto-0.8.0.tar` & `unitauto-0.8.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:39:54.612152 unitauto-0.8.0/
--rw-r--r--   0 tommylemon   (501) staff       (20)    11373 2023-06-18 10:48:56.000000 unitauto-0.8.0/LICENSE
--rw-r--r--   0 tommylemon   (501) staff       (20)     1299 2023-06-18 15:39:54.612203 unitauto-0.8.0/PKG-INFO
--rw-r--r--   0 tommylemon   (501) staff       (20)      777 2023-06-18 15:15:19.000000 unitauto-0.8.0/README.md
--rw-rw-r--   0 tommylemon   (501) staff       (20)      103 2023-06-14 01:55:33.000000 unitauto-0.8.0/pyproject.toml
--rw-rw-r--   0 tommylemon   (501) staff       (20)      583 2023-06-18 15:39:54.612754 unitauto-0.8.0/setup.cfg
-drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:39:54.610778 unitauto-0.8.0/unitauto/
--rw-r--r--   0 tommylemon   (501) staff       (20)       18 2023-06-18 12:16:25.000000 unitauto-0.8.0/unitauto/__init__.py
--rw-r--r--   0 tommylemon   (501) staff       (20)    11817 2023-06-18 11:07:33.000000 unitauto-0.8.0/unitauto/methodutil.py
-drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:39:54.611996 unitauto-0.8.0/unitauto/test/
--rw-r--r--   0 tommylemon   (501) staff       (20)     1009 2023-06-17 17:22:10.000000 unitauto-0.8.0/unitauto/test/__init__.py
--rw-r--r--   0 tommylemon   (501) staff       (20)     1009 2023-06-17 17:22:10.000000 unitauto-0.8.0/unitauto/test/testutil.py
-drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:39:54.611595 unitauto-0.8.0/unitauto.egg-info/
--rw-r--r--   0 tommylemon   (501) staff       (20)     1299 2023-06-18 15:39:54.000000 unitauto-0.8.0/unitauto.egg-info/PKG-INFO
--rw-r--r--   0 tommylemon   (501) staff       (20)      266 2023-06-18 15:39:54.000000 unitauto-0.8.0/unitauto.egg-info/SOURCES.txt
--rw-r--r--   0 tommylemon   (501) staff       (20)        1 2023-06-18 15:39:54.000000 unitauto-0.8.0/unitauto.egg-info/dependency_links.txt
--rw-r--r--   0 tommylemon   (501) staff       (20)        9 2023-06-18 15:39:54.000000 unitauto-0.8.0/unitauto.egg-info/top_level.txt
+drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:57:45.340474 unitauto-0.8.1/
+-rw-r--r--   0 tommylemon   (501) staff       (20)     1066 2023-06-18 15:42:15.000000 unitauto-0.8.1/LICENSE
+-rw-r--r--   0 tommylemon   (501) staff       (20)     1299 2023-06-18 15:57:45.340535 unitauto-0.8.1/PKG-INFO
+-rw-r--r--   0 tommylemon   (501) staff       (20)      777 2023-06-18 15:55:28.000000 unitauto-0.8.1/README.md
+-rw-rw-r--   0 tommylemon   (501) staff       (20)      103 2023-06-14 01:55:33.000000 unitauto-0.8.1/pyproject.toml
+-rw-rw-r--   0 tommylemon   (501) staff       (20)      583 2023-06-18 15:57:45.340876 unitauto-0.8.1/setup.cfg
+drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:57:45.337973 unitauto-0.8.1/unitauto/
+-rw-r--r--   0 tommylemon   (501) staff       (20)       18 2023-06-18 12:16:25.000000 unitauto-0.8.1/unitauto/__init__.py
+-rw-r--r--   0 tommylemon   (501) staff       (20)    11817 2023-06-18 11:07:33.000000 unitauto-0.8.1/unitauto/methodutil.py
+-rw-r--r--   0 tommylemon   (501) staff       (20)     3355 2023-06-18 09:31:49.000000 unitauto-0.8.1/unitauto/server.py
+drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:57:45.340349 unitauto-0.8.1/unitauto/test/
+-rw-r--r--   0 tommylemon   (501) staff       (20)     1009 2023-06-17 17:22:10.000000 unitauto-0.8.1/unitauto/test/__init__.py
+-rw-r--r--   0 tommylemon   (501) staff       (20)     1009 2023-06-17 17:22:10.000000 unitauto-0.8.1/unitauto/test/testutil.py
+drwxr-xr-x   0 tommylemon   (501) staff       (20)        0 2023-06-18 15:57:45.339924 unitauto-0.8.1/unitauto.egg-info/
+-rw-r--r--   0 tommylemon   (501) staff       (20)     1299 2023-06-18 15:57:45.000000 unitauto-0.8.1/unitauto.egg-info/PKG-INFO
+-rw-r--r--   0 tommylemon   (501) staff       (20)      285 2023-06-18 15:57:45.000000 unitauto-0.8.1/unitauto.egg-info/SOURCES.txt
+-rw-r--r--   0 tommylemon   (501) staff       (20)        1 2023-06-18 15:57:45.000000 unitauto-0.8.1/unitauto.egg-info/dependency_links.txt
+-rw-r--r--   0 tommylemon   (501) staff       (20)        9 2023-06-18 15:57:45.000000 unitauto-0.8.1/unitauto.egg-info/top_level.txt
```

### Comparing `unitauto-0.8.0/PKG-INFO` & `unitauto-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.8.0
+Version: 0.8.1
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `unitauto-0.8.0/README.md` & `unitauto-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `unitauto-0.8.0/setup.cfg` & `unitauto-0.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unitauto
-version = 0.8.0
+version = 0.8.1
 author = TommyLemon
 author_email = tommylemon@qq.com
 description = An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TommyLemon/unitauto-py
 classifiers =
```

### Comparing `unitauto-0.8.0/unitauto/methodutil.py` & `unitauto-0.8.1/unitauto/methodutil.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.8.0/unitauto/test/__init__.py` & `unitauto-0.8.1/unitauto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.8.0/unitauto/test/testutil.py` & `unitauto-0.8.1/unitauto/test/testutil.py`

 * *Files identical despite different names*

### Comparing `unitauto-0.8.0/unitauto.egg-info/PKG-INFO` & `unitauto-0.8.1/unitauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitauto
-Version: 0.8.0
+Version: 0.8.1
 Summary: An unit testing platform powered by machine learning. Coding-free, comprehensive and automatic testing for methods/functions
 Home-page: https://github.com/TommyLemon/unitauto-py
 Author: TommyLemon
 Author-email: tommylemon@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

