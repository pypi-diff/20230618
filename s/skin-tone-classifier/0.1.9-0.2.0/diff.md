# Comparing `tmp/skin-tone-classifier-0.1.9.tar.gz` & `tmp/skin-tone-classifier-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skin-tone-classifier-0.1.9.tar", last modified: Tue Jan 10 06:09:26 2023, max compression
+gzip compressed data, was "skin-tone-classifier-0.2.0.tar", last modified: Sun Jun 18 14:57:23 2023, max compression
```

## Comparing `skin-tone-classifier-0.1.9.tar` & `skin-tone-classifier-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/src/stone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/src/stone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/src/stone/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17695 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.143686 skin-tone-classifier-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:57:22.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 14:57:23.000000 skin-tone-classifier-0.2.0/src/skin_tone_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:57:23.147686 skin-tone-classifier-0.2.0/src/stone/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-18 14:57:13.000000 skin-tone-classifier-0.2.0/src/stone/utils.py
```

### Comparing `skin-tone-classifier-0.1.9/LICENSE` & `skin-tone-classifier-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skin-tone-classifier-0.1.9/setup.py` & `skin-tone-classifier-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.1.9'
+VERSION = '0.2.0'
 
 with open('README.md') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='skin-tone-classifier',
     version=VERSION,
@@ -28,15 +28,14 @@
     entry_points={
         'console_scripts': [
             'stone = stone.__main__:main'
         ],
     },
     install_requires=[
         "opencv-python>=4.6.0.66",
-        "imutils>=0.5.4",
         "numpy>=1.21.5",
         "colormath>=3.0.0",
         "tqdm>=4.64.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

