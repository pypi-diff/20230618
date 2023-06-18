# Comparing `tmp/strip-tags-0.3.tar.gz` & `tmp/strip-tags-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strip-tags-0.3.tar", last modified: Fri May 19 05:20:18 2023, max compression
+gzip compressed data, was "strip-tags-0.4.tar", last modified: Sun Jun 18 08:09:05 2023, max compression
```

## Comparing `strip-tags-0.3.tar` & `strip-tags-0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.746920 strip-tags-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 05:19:55.000000 strip-tags-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-19 05:20:18.746920 strip-tags-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-19 05:19:55.000000 strip-tags-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 05:20:18.746920 strip-tags-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-19 05:19:55.000000 strip-tags-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.742920 strip-tags-0.3/strip_tags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 05:19:55.000000 strip-tags-0.3/strip_tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-19 05:19:55.000000 strip-tags-0.3/strip_tags/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-19 05:19:55.000000 strip-tags-0.3/strip_tags/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.746920 strip-tags-0.3/strip_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 05:20:18.000000 strip-tags-0.3/strip_tags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 05:20:18.746920 strip-tags-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-19 05:19:55.000000 strip-tags-0.3/tests/test_strip_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 08:08:47.000000 strip-tags-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-18 08:09:05.822164 strip-tags-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-18 08:08:47.000000 strip-tags-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:09:05.822164 strip-tags-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 08:08:47.000000 strip-tags-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/strip_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-18 08:08:47.000000 strip-tags-0.4/strip_tags/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/strip_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-18 08:09:05.000000 strip-tags-0.4/strip_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:09:05.822164 strip-tags-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-18 08:08:47.000000 strip-tags-0.4/tests/test_strip_tags.py
```

### Comparing `strip-tags-0.3/LICENSE` & `strip-tags-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strip-tags-0.3/setup.py` & `strip-tags-0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,10 +28,10 @@
     version=VERSION,
     packages=["strip_tags"],
     entry_points="""
         [console_scripts]
         strip-tags=strip_tags.cli:cli
     """,
     install_requires=["click", "beautifulsoup4", "html5lib"],
-    extras_require={"test": ["pytest"]},
+    extras_require={"test": ["pytest", "pytest-icdiff"]},
     python_requires=">=3.7",
 )
```

