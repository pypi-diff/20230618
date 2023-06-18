# Comparing `tmp/skin-tone-classifier-0.2.0.tar.gz` & `tmp/skin-tone-classifier-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skin-tone-classifier-0.2.0.tar", last modified: Sun Jun 18 14:57:23 2023, max compression
+gzip compressed data, was "skin-tone-classifier-0.2.1.tar", last modified: Sun Jun 18 15:39:08 2023, max compression
```

## Comparing `skin-tone-classifier-0.2.0.tar` & `skin-tone-classifier-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.143686 skin-tone-classifier-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:57:22.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/src/stone/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 15:39:08.461399 skin-tone-classifier-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 15:39:08.000000 skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 15:39:08.457399 skin-tone-classifier-0.2.1/src/stone/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-18 15:38:59.000000 skin-tone-classifier-0.2.1/src/stone/utils.py
```

### Comparing `skin-tone-classifier-0.2.0/LICENSE` & `skin-tone-classifier-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skin-tone-classifier-0.2.0/PKG-INFO` & `skin-tone-classifier-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skin-tone-classifier
-Version: 0.2.0
+Version: 0.2.1
 Summary: An easy-to-use library for skin tone classification
 Home-page: https://chenglongma.com/SkinToneClassifier/
 Author: Chenglong Ma
 Author-email: chenglong.m@outlook.com
 Project-URL: Documentation, https://chenglongma.com/SkinToneClassifier/
 Project-URL: Code, https://github.com/ChenglongMa/SkinToneClassifier
 Project-URL: Issue tracker, https://github.com/ChenglongMa/SkinToneClassifier/issues
```

### Comparing `skin-tone-classifier-0.2.0/README.md` & `skin-tone-classifier-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `skin-tone-classifier-0.2.0/setup.py` & `skin-tone-classifier-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 with open('README.md') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='skin-tone-classifier',
     version=VERSION,
```

### Comparing `skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/PKG-INFO` & `skin-tone-classifier-0.2.1/src/skin_tone_classifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skin-tone-classifier
-Version: 0.2.0
+Version: 0.2.1
 Summary: An easy-to-use library for skin tone classification
 Home-page: https://chenglongma.com/SkinToneClassifier/
 Author: Chenglong Ma
 Author-email: chenglong.m@outlook.com
 Project-URL: Documentation, https://chenglongma.com/SkinToneClassifier/
 Project-URL: Code, https://github.com/ChenglongMa/SkinToneClassifier
 Project-URL: Issue tracker, https://github.com/ChenglongMa/SkinToneClassifier/issues
```

### Comparing `skin-tone-classifier-0.2.0/src/stone/__main__.py` & `skin-tone-classifier-0.2.1/src/stone/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from multiprocessing import freeze_support, cpu_count, Pool
 
 import cv2
 import numpy as np
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
-from image import process, is_black_white
-from utils import build_arguments, alphabet_id, build_filenames, is_windows
+from stone.image import process, is_black_white
+from stone.utils import build_arguments, alphabet_id, build_filenames, is_windows
 
 
 def patch_asscalar(a):
     return np.asarray(a).item()
 
 
 setattr(np, "asscalar", patch_asscalar)
```

### Comparing `skin-tone-classifier-0.2.0/src/stone/image.py` & `skin-tone-classifier-0.2.1/src/stone/image.py`

 * *Files identical despite different names*

### Comparing `skin-tone-classifier-0.2.0/src/stone/utils.py` & `skin-tone-classifier-0.2.1/src/stone/utils.py`

 * *Files identical despite different names*

