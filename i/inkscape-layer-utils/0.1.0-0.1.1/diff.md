# Comparing `tmp/inkscape_layer_utils-0.1.0.tar.gz` & `tmp/inkscape_layer_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inkscape_layer_utils-0.1.0.tar", last modified: Sat Jun 17 23:19:04 2023, max compression
+gzip compressed data, was "inkscape_layer_utils-0.1.1.tar", last modified: Sat Jun 17 23:46:52 2023, max compression
```

## Comparing `inkscape_layer_utils-0.1.0.tar` & `inkscape_layer_utils-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/inkscape_layer_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/inkscape_layer_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 23:19:04.000000 inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:19:04.541374 inkscape_layer_utils-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-06-17 23:18:55.000000 inkscape_layer_utils-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/inkscape_layer_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/inkscape_layer_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-17 23:46:52.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-17 23:46:52.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:46:52.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 23:46:52.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 23:46:52.000000 inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:46:52.281079 inkscape_layer_utils-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83572 2023-06-17 23:46:42.000000 inkscape_layer_utils-0.1.1/versioneer.py
```

### Comparing `inkscape_layer_utils-0.1.0/LICENSE` & `inkscape_layer_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.1.0/PKG-INFO` & `inkscape_layer_utils-0.1.1/inkscape_layer_utils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: inkscape_layer_utils
-Version: 0.1.0
+Name: inkscape-layer-utils
+Version: 0.1.1
 Summary: Simple library to extract and manipulate layers in inkscape SVGs
 Home-page: https://github.com/twyleg/inkscape_layer_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: inkscape svg layer utilities
 License-File: LICENSE
@@ -14,23 +14,23 @@
 
 Simple utils to interact with Inkscape SVG images and their layers.
 Typical use case is extracting layers from an input SVG or manipulating attributes of elements in an image
 (e.g. coloring certain elements).
 
 Take the following multilayer image as an example:
 
-.. image:: docs/_static/imgs/inkscape_test_image_with_layers.png
+.. image:: https://raw.githubusercontent.com/twyleg/inkscape_layer_utils/master/docs/_static/imgs/inkscape_test_image_with_layers.png
 
 The architecture of the image can also be visualized like this:
 
-.. image:: docs/_static/imgs/example_image_stacked.svg
+.. image:: https://raw.githubusercontent.com/twyleg/inkscape_layer_utils/master/docs/_static/imgs/example_image_stacked.svg
 
 Or as a tree:
 
-.. image:: docs/_static/imgs/example_image_tree.svg
+.. image:: https://raw.githubusercontent.com/twyleg/inkscape_layer_utils/master/docs/_static/imgs/example_image_tree.svg
 
 The utilities can be used as a library or command line tool. Take a look at the examples section for further explanation.
 
 Examples
 --------
 
 All examples can be found in the `examples/ <https://github.com/twyleg/inkscape_layer_utils/tree/master/examples>`_ directory.
```

### Comparing `inkscape_layer_utils-0.1.0/README.rst` & `inkscape_layer_utils-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.1.0/inkscape_layer_utils/__init__.py` & `inkscape_layer_utils-0.1.1/inkscape_layer_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.1.0/inkscape_layer_utils/image.py` & `inkscape_layer_utils-0.1.1/inkscape_layer_utils/image.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.1.0/inkscape_layer_utils/main.py` & `inkscape_layer_utils-0.1.1/inkscape_layer_utils/main.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.1.0/inkscape_layer_utils.egg-info/PKG-INFO` & `inkscape_layer_utils-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: inkscape-layer-utils
-Version: 0.1.0
+Name: inkscape_layer_utils
+Version: 0.1.1
 Summary: Simple library to extract and manipulate layers in inkscape SVGs
 Home-page: https://github.com/twyleg/inkscape_layer_utils
 Author: Torsten Wylegala
 Author-email: mail@twyleg.de
 License: GPL 3.0
 Keywords: inkscape svg layer utilities
 License-File: LICENSE
@@ -14,23 +14,23 @@
 
 Simple utils to interact with Inkscape SVG images and their layers.
 Typical use case is extracting layers from an input SVG or manipulating attributes of elements in an image
 (e.g. coloring certain elements).
 
 Take the following multilayer image as an example:
 
-.. image:: docs/_static/imgs/inkscape_test_image_with_layers.png
+.. image:: https://raw.githubusercontent.com/twyleg/inkscape_layer_utils/master/docs/_static/imgs/inkscape_test_image_with_layers.png
 
 The architecture of the image can also be visualized like this:
 
-.. image:: docs/_static/imgs/example_image_stacked.svg
+.. image:: https://raw.githubusercontent.com/twyleg/inkscape_layer_utils/master/docs/_static/imgs/example_image_stacked.svg
 
 Or as a tree:
 
-.. image:: docs/_static/imgs/example_image_tree.svg
+.. image:: https://raw.githubusercontent.com/twyleg/inkscape_layer_utils/master/docs/_static/imgs/example_image_tree.svg
 
 The utilities can be used as a library or command line tool. Take a look at the examples section for further explanation.
 
 Examples
 --------
 
 All examples can be found in the `examples/ <https://github.com/twyleg/inkscape_layer_utils/tree/master/examples>`_ directory.
```

### Comparing `inkscape_layer_utils-0.1.0/setup.py` & `inkscape_layer_utils-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # Copyright (C) 2023 twyleg
-import os
 import versioneer
+from pathlib import Path
 from setuptools import find_packages, setup
 
 
-def read(fname):
-    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+def read(relative_filepath):
+    return open(Path(__file__).parent / relative_filepath).read()
+
+
+def read_long_description() -> str:
+    return read("README.rst").replace(
+        "docs/_static/", "https://raw.githubusercontent.com/twyleg/inkscape_layer_utils" "/master/docs/_static/"
+    )
 
 
 setup(
     name="inkscape_layer_utils",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     author="Torsten Wylegala",
     author_email="mail@twyleg.de",
     description=("Simple library to extract and manipulate layers in inkscape SVGs"),
     license="GPL 3.0",
     keywords="inkscape svg layer utilities",
     url="https://github.com/twyleg/inkscape_layer_utils",
     packages=find_packages(),
-    long_description=read("README.rst"),
+    long_description=read_long_description(),
     install_requires=[],
     entry_points={
         "console_scripts": [
             "inkscape_layer_utils = inkscape_layer_utils.main:main",
         ]
     },
 )
```

### Comparing `inkscape_layer_utils-0.1.0/tests/test_image.py` & `inkscape_layer_utils-0.1.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `inkscape_layer_utils-0.1.0/versioneer.py` & `inkscape_layer_utils-0.1.1/versioneer.py`

 * *Files identical despite different names*

