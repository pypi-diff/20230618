# Comparing `tmp/gamchanger-0.1.8.tar.gz` & `tmp/gamchanger-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/JayWong/Programs/msr/gam-changer/notebook-widget/dist/tmpus2xuf7a/gamchanger-0.1.8.tar", last modified: Fri Aug 12 11:24:36 2022, max compression
+gzip compressed data, was "/Users/JayWong/Programs/msr/gam-changer/notebook-widget/dist/tmpdwhvgafw/gamchanger-0.1.9.tar", last modified: Fri Aug 12 11:34:20 2022, max compression
```

## Comparing `gamchanger-0.1.8.tar` & `gamchanger-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:24:36.000000 gamchanger-0.1.8/
--rw-r--r--   0 JayWong    (503) staff       (20)      273 2021-08-24 21:18:36.000000 gamchanger-0.1.8/MANIFEST.in
--rw-r--r--   0 JayWong    (503) staff       (20)      755 2022-08-12 11:24:36.000000 gamchanger-0.1.8/PKG-INFO
--rw-r--r--   0 JayWong    (503) staff       (20)       82 2021-08-16 15:04:08.000000 gamchanger-0.1.8/README.md
-drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger/
--rw-r--r--   0 JayWong    (503) staff       (20)     6148 2021-08-16 16:02:41.000000 gamchanger-0.1.8/gamchanger/.DS_Store
--rw-r--r--   0 JayWong    (503) staff       (20)      159 2022-08-12 11:24:25.000000 gamchanger-0.1.8/gamchanger/__init__.py
-drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger/__pycache__/
--rw-r--r--   0 JayWong    (503) staff       (20)      341 2022-06-14 07:30:02.000000 gamchanger-0.1.8/gamchanger/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 JayWong    (503) staff       (20)    14710 2022-06-14 07:30:02.000000 gamchanger-0.1.8/gamchanger/__pycache__/gamchanger.cpython-37.pyc
--rw-r--r--   0 JayWong    (503) staff       (20)   511415 2022-02-10 04:17:54.000000 gamchanger-0.1.8/gamchanger/gamchanger.js
--rw-r--r--   0 JayWong    (503) staff       (20)    22699 2022-08-02 16:24:41.000000 gamchanger-0.1.8/gamchanger/gamchanger.py
--rw-r--r--   0 JayWong    (503) staff       (20)     1022 2021-08-24 22:33:33.000000 gamchanger-0.1.8/gamchanger/index.html
-drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger.egg-info/
--rw-r--r--   0 JayWong    (503) staff       (20)      755 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger.egg-info/PKG-INFO
--rw-r--r--   0 JayWong    (503) staff       (20)      497 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger.egg-info/SOURCES.txt
--rw-r--r--   0 JayWong    (503) staff       (20)        1 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger.egg-info/dependency_links.txt
--rw-r--r--   0 JayWong    (503) staff       (20)        1 2021-08-16 15:13:53.000000 gamchanger-0.1.8/gamchanger.egg-info/not-zip-safe
--rw-r--r--   0 JayWong    (503) staff       (20)       21 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger.egg-info/requires.txt
--rw-r--r--   0 JayWong    (503) staff       (20)       11 2022-08-12 11:24:36.000000 gamchanger-0.1.8/gamchanger.egg-info/top_level.txt
--rw-r--r--   0 JayWong    (503) staff       (20)      382 2022-08-12 11:24:36.000000 gamchanger-0.1.8/setup.cfg
--rw-r--r--   0 JayWong    (503) staff       (20)     1208 2022-08-12 11:24:25.000000 gamchanger-0.1.8/setup.py
-drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:24:36.000000 gamchanger-0.1.8/tests/
--rw-r--r--   0 JayWong    (503) staff       (20)       40 2022-08-02 16:24:44.000000 gamchanger-0.1.8/tests/__init__.py
--rw-r--r--   0 JayWong    (503) staff       (20)      402 2022-08-02 16:24:46.000000 gamchanger-0.1.8/tests/test_gamchanger.py
+drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:34:20.000000 gamchanger-0.1.9/
+-rw-r--r--   0 JayWong    (503) staff       (20)      273 2021-08-24 21:18:36.000000 gamchanger-0.1.9/MANIFEST.in
+-rw-r--r--   0 JayWong    (503) staff       (20)      755 2022-08-12 11:34:20.000000 gamchanger-0.1.9/PKG-INFO
+-rw-r--r--   0 JayWong    (503) staff       (20)       82 2021-08-16 15:04:08.000000 gamchanger-0.1.9/README.md
+drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger/
+-rw-r--r--   0 JayWong    (503) staff       (20)     6148 2021-08-16 16:02:41.000000 gamchanger-0.1.9/gamchanger/.DS_Store
+-rw-r--r--   0 JayWong    (503) staff       (20)      158 2022-08-12 11:34:09.000000 gamchanger-0.1.9/gamchanger/__init__.py
+drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger/__pycache__/
+-rw-r--r--   0 JayWong    (503) staff       (20)      341 2022-06-14 07:30:02.000000 gamchanger-0.1.9/gamchanger/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 JayWong    (503) staff       (20)    14710 2022-06-14 07:30:02.000000 gamchanger-0.1.9/gamchanger/__pycache__/gamchanger.cpython-37.pyc
+-rw-r--r--   0 JayWong    (503) staff       (20)   511415 2022-02-10 04:17:54.000000 gamchanger-0.1.9/gamchanger/gamchanger.js
+-rw-r--r--   0 JayWong    (503) staff       (20)    22699 2022-08-02 16:24:41.000000 gamchanger-0.1.9/gamchanger/gamchanger.py
+-rw-r--r--   0 JayWong    (503) staff       (20)     1022 2021-08-24 22:33:33.000000 gamchanger-0.1.9/gamchanger/index.html
+drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger.egg-info/
+-rw-r--r--   0 JayWong    (503) staff       (20)      755 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger.egg-info/PKG-INFO
+-rw-r--r--   0 JayWong    (503) staff       (20)      497 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger.egg-info/SOURCES.txt
+-rw-r--r--   0 JayWong    (503) staff       (20)        1 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger.egg-info/dependency_links.txt
+-rw-r--r--   0 JayWong    (503) staff       (20)        1 2021-08-16 15:13:53.000000 gamchanger-0.1.9/gamchanger.egg-info/not-zip-safe
+-rw-r--r--   0 JayWong    (503) staff       (20)       21 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger.egg-info/requires.txt
+-rw-r--r--   0 JayWong    (503) staff       (20)       11 2022-08-12 11:34:20.000000 gamchanger-0.1.9/gamchanger.egg-info/top_level.txt
+-rw-r--r--   0 JayWong    (503) staff       (20)      382 2022-08-12 11:34:20.000000 gamchanger-0.1.9/setup.cfg
+-rw-r--r--   0 JayWong    (503) staff       (20)     1208 2022-08-12 11:34:09.000000 gamchanger-0.1.9/setup.py
+drwxr-xr-x   0 JayWong    (503) staff       (20)        0 2022-08-12 11:34:20.000000 gamchanger-0.1.9/tests/
+-rw-r--r--   0 JayWong    (503) staff       (20)       40 2022-08-02 16:24:44.000000 gamchanger-0.1.9/tests/__init__.py
+-rw-r--r--   0 JayWong    (503) staff       (20)      402 2022-08-02 16:24:46.000000 gamchanger-0.1.9/tests/test_gamchanger.py
```

### Comparing `gamchanger-0.1.8/PKG-INFO` & `gamchanger-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamchanger
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package to run GAM Changer in your computation notebooks.
 Home-page: https://github.com/xiaohk/gam-changer
 Author: Jay Wang
 Author-email: jayw@zijie.wang
 License: MIT license
 Keywords: gamchanger
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gamchanger-0.1.8/gamchanger/.DS_Store` & `gamchanger-0.1.9/gamchanger/.DS_Store`

 * *Files identical despite different names*

### Comparing `gamchanger-0.1.8/gamchanger/__pycache__/gamchanger.cpython-37.pyc` & `gamchanger-0.1.9/gamchanger/__pycache__/gamchanger.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `gamchanger-0.1.8/gamchanger/gamchanger.js` & `gamchanger-0.1.9/gamchanger/gamchanger.js`

 * *Files identical despite different names*

### Comparing `gamchanger-0.1.8/gamchanger/gamchanger.py` & `gamchanger-0.1.9/gamchanger/gamchanger.py`

 * *Files identical despite different names*

### Comparing `gamchanger-0.1.8/gamchanger/index.html` & `gamchanger-0.1.9/gamchanger/index.html`

 * *Files identical despite different names*

### Comparing `gamchanger-0.1.8/gamchanger.egg-info/PKG-INFO` & `gamchanger-0.1.9/gamchanger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamchanger
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python package to run GAM Changer in your computation notebooks.
 Home-page: https://github.com/xiaohk/gam-changer
 Author: Jay Wang
 Author-email: jayw@zijie.wang
 License: MIT license
 Keywords: gamchanger
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gamchanger-0.1.8/setup.py` & `gamchanger-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     include_package_data=True,
     keywords="gamchanger",
     name="gamchanger",
     packages=find_packages(include=["gamchanger", "gamchanger.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/xiaohk/gam-changer",
-    version="0.1.8",
+    version="0.1.9",
     zip_safe=False,
 )
```

