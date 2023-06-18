# Comparing `tmp/cropnet-0.1.2.tar.gz` & `tmp/cropnet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropnet-0.1.2.tar", last modified: Sat Jun 17 22:41:53 2023, max compression
+gzip compressed data, was "cropnet-0.1.3.tar", last modified: Sun Jun 18 02:13:09 2023, max compression
```

## Comparing `cropnet-0.1.2.tar` & `cropnet-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 22:41:53.370139 cropnet-0.1.2/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      643 2023-06-17 22:41:53.370139 cropnet-0.1.2/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       13 2023-06-17 02:52:22.000000 cropnet-0.1.2/README.md
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 22:41:53.370139 cropnet-0.1.2/cropnet.egg-info/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      643 2023-06-17 22:41:53.000000 cropnet-0.1.2/cropnet.egg-info/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      283 2023-06-17 22:41:53.000000 cropnet-0.1.2/cropnet.egg-info/SOURCES.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-17 22:41:53.000000 cropnet-0.1.2/cropnet.egg-info/dependency_links.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-17 22:41:53.000000 cropnet-0.1.2/cropnet.egg-info/requires.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-17 22:41:53.000000 cropnet-0.1.2/cropnet.egg-info/top_level.txt
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 22:41:53.370139 cropnet-0.1.2/dataset/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 22:41:39.000000 cropnet-0.1.2/dataset/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6253 2023-06-17 22:36:51.000000 cropnet-0.1.2/dataset/hrrr_computed_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.2/dataset/sentinel2_imagery.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2435 2023-06-17 22:36:51.000000 cropnet-0.1.2/dataset/usda_crop_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-17 22:41:53.370139 cropnet-0.1.2/setup.cfg
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      927 2023-06-17 22:41:39.000000 cropnet-0.1.2/setup.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 02:13:09.878758 cropnet-0.1.3/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4718 2023-06-18 02:13:09.878758 cropnet-0.1.3/PKG-INFO
+-rw-r--r--   0 fudong    (1000) fudong    (1000)     4033 2023-06-18 02:04:05.000000 cropnet-0.1.3/README.md
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 02:13:09.878758 cropnet-0.1.3/cropnet.egg-info/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4718 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      283 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/requires.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/top_level.txt
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 02:13:09.878758 cropnet-0.1.3/dataset/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 22:41:39.000000 cropnet-0.1.3/dataset/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6253 2023-06-17 22:36:51.000000 cropnet-0.1.3/dataset/hrrr_computed_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.3/dataset/sentinel2_imagery.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2435 2023-06-17 22:36:51.000000 cropnet-0.1.3/dataset/usda_crop_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-18 02:13:09.878758 cropnet-0.1.3/setup.cfg
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1183 2023-06-18 02:11:41.000000 cropnet-0.1.3/setup.py
```

### Comparing `cropnet-0.1.2/dataset/hrrr_computed_dataset.py` & `cropnet-0.1.3/dataset/hrrr_computed_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.2/dataset/sentinel2_imagery.py` & `cropnet-0.1.3/dataset/sentinel2_imagery.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.2/dataset/usda_crop_dataset.py` & `cropnet-0.1.3/dataset/usda_crop_dataset.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.2/setup.py` & `cropnet-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from setuptools import setup
+from pathlib import Path
+
+# read the contents of the README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cropnet',
-    version='0.1.2',
+    version='0.1.3',
     description='A Python package for the CropNet dataset',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Anonymous AI4Science',
     author_email='anonymous.ai4science@gmail.com',
     license='Free for non-commercial use',
     packages=['dataset'],
     install_requires=[
         'torch >= 1.11.0',
         'numpy',
```

