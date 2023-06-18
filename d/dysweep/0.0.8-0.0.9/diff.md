# Comparing `tmp/dysweep-0.0.8.tar.gz` & `tmp/dysweep-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.8.tar", last modified: Mon Jun 12 16:57:04 2023, max compression
+gzip compressed data, was "dysweep-0.0.9.tar", last modified: Sun Jun 18 12:24:51 2023, max compression
```

## Comparing `dysweep-0.0.8.tar` & `dysweep-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:57:04.072711 dysweep-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 16:54:49.000000 dysweep-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 16:57:04.072711 dysweep-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 16:54:49.000000 dysweep-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:57:04.068711 dysweep-0.0.8/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-12 16:54:49.000000 dysweep-0.0.8/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:57:04.068711 dysweep-0.0.8/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 16:57:04.000000 dysweep-0.0.8/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:57:04.072711 dysweep-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-12 16:54:49.000000 dysweep-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:24:51.837873 dysweep-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 12:22:29.000000 dysweep-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 12:24:51.837873 dysweep-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-18 12:22:29.000000 dysweep-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:24:51.837873 dysweep-0.0.9/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21511 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-18 12:22:29.000000 dysweep-0.0.9/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:24:51.837873 dysweep-0.0.9/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:24:51.000000 dysweep-0.0.9/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:24:51.837873 dysweep-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-18 12:22:29.000000 dysweep-0.0.9/setup.py
```

### Comparing `dysweep-0.0.8/LICENSE` & `dysweep-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.8/dysweep/parallel.py` & `dysweep-0.0.9/dysweep/parallel.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.8/dysweep/utils.py` & `dysweep-0.0.9/dysweep/utils.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.8/dysweep/wandbX.py` & `dysweep-0.0.9/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.8/setup.py` & `dysweep-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 from dysweep import __version__
 
-with open("README.md", encoding="utf-8") as f:
+with open("readme_pypi.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="dysweep",
     packages=find_packages(include=["dysweep", "dysweep.*"]),
     version=__version__,
     license="Apache License 2.0",
-    description="A toolset for dynamic python code manipulations",
+    description="Use Weights and Biases Sweeps for Dynamic Configuration generation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hamid Kamkari",
     author_email="hamidrezakamkari@gmail.com",
     url="https://github.com/HamidrezaKmK/dysweep",
     keywords=[
         "dynamic configurations",
+        "large scale experiments",
         "deep learning",
         "sweeps",
         "hyperparameter tuning",
         "lazy evaluation"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
```

