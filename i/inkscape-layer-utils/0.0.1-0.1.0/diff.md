# Comparing `tmp/inkscape_layer_utils-0.0.1.tar.gz` & `tmp/inkscape_layer_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_layer_utils-0.0.1.tar", last modified: Mon Apr  3 22:32:29 2023, max compression
+gzip compressed data, was "inkscape_layer_utils-0.1.0.tar", last modified: Sat Jun 17 23:19:04 2023, max compression
```

## Comparing `inkscape_layer_utils-0.0.1.tar` & `inkscape_layer_utils-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-04-03 22:32:29.636532 inkscape_layer_utils-0.0.1/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)    35149 2023-03-29 20:57:10.000000 inkscape_layer_utils-0.0.1/LICENSE
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      845 2023-04-03 22:32:29.636532 inkscape_layer_utils-0.0.1/PKG-INFO
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      535 2023-03-29 20:57:10.000000 inkscape_layer_utils-0.0.1/README.md
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-04-03 22:32:29.636532 inkscape_layer_utils-0.0.1/inkscape_layer_utils/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      585 2023-04-03 13:21:27.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils/__init__.py
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       51 2023-04-01 17:54:47.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils/__main__.py
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)     5480 2023-04-03 06:47:04.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils/image.py
-drwxrwxr-x   0 twyleg   (30000) twyleg   (30003)        0 2023-04-03 22:32:29.636532 inkscape_layer_utils-0.0.1/inkscape_layer_utils.egg-info/
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      845 2023-04-03 22:32:29.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils.egg-info/PKG-INFO
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      298 2023-04-03 22:32:29.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)        1 2023-04-03 22:32:29.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       21 2023-04-03 22:32:29.000000 inkscape_layer_utils-0.0.1/inkscape_layer_utils.egg-info/top_level.txt
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)       38 2023-04-03 22:32:29.636532 inkscape_layer_utils-0.0.1/setup.cfg
--rw-rw-r--   0 twyleg   (30000) twyleg   (30003)      608 2023-04-03 08:37:05.000000 inkscape_layer_utils-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/inkscape_layer_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/inkscape_layer_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/versioneer.py
```

### Comparing `inkscape_layer_utils-0.0.1/LICENSE` & `inkscape_layer_utils-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.0.1/setup.py` & `inkscape_layer_utils-0.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+# Copyright (C) 2023 twyleg
 import os
+import versioneer
 from setuptools import find_packages, setup
 
 
-NAME = 'inkscape_layer_utils'
-VERSION = '0.0.1'
-
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+
 setup(
-    name=NAME,
-    version=VERSION,
+    name="inkscape_layer_utils",
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     author="Torsten Wylegala",
     author_email="mail@twyleg.de",
-    description=("SImple library to extract and manipulate layers from inscape SVGs"),
+    description=("Simple library to extract and manipulate layers in inkscape SVGs"),
     license="GPL 3.0",
     keywords="inkscape svg layer utilities",
-    url="https://github.com/twyleg",
+    url="https://github.com/twyleg/inkscape_layer_utils",
     packages=find_packages(),
-    long_description=read('README.md'),
+    long_description=read("README.rst"),
     install_requires=[],
-    cmdclass={}
+    entry_points={
+        "console_scripts": [
+            "inkscape_layer_utils = inkscape_layer_utils.main:main",
+        ]
+    },
 )
```

