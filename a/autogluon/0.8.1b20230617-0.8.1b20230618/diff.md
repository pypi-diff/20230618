# Comparing `tmp/autogluon-0.8.1b20230617.tar.gz` & `tmp/autogluon-0.8.1b20230618.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.8.1b20230617.tar", last modified: Sat Jun 17 09:04:40 2023, max compression
+gzip compressed data, was "autogluon-0.8.1b20230618.tar", last modified: Sun Jun 18 09:04:39 2023, max compression
```

## Comparing `autogluon-0.8.1b20230617.tar` & `autogluon-0.8.1b20230618.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:40.759968 autogluon-0.8.1b20230617/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-17 09:04:40.759968 autogluon-0.8.1b20230617/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 09:04:40.759968 autogluon-0.8.1b20230617/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-17 09:03:58.000000 autogluon-0.8.1b20230617/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:40.755968 autogluon-0.8.1b20230617/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:40.755968 autogluon-0.8.1b20230617/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:40.759968 autogluon-0.8.1b20230617/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 09:03:58.000000 autogluon-0.8.1b20230617/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:40.759968 autogluon-0.8.1b20230617/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:04:40.000000 autogluon-0.8.1b20230617/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:04:39.601989 autogluon-0.8.1b20230618/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-18 09:04:39.601989 autogluon-0.8.1b20230618/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 09:04:39.605990 autogluon-0.8.1b20230618/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-18 09:03:53.000000 autogluon-0.8.1b20230618/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:04:39.601989 autogluon-0.8.1b20230618/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:04:39.601989 autogluon-0.8.1b20230618/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:04:39.601989 autogluon-0.8.1b20230618/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 09:03:53.000000 autogluon-0.8.1b20230618/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:04:39.601989 autogluon-0.8.1b20230618/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:04:39.000000 autogluon-0.8.1b20230618/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.8.1b20230617/PKG-INFO` & `autogluon-0.8.1b20230618/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230617
+Version: 0.8.1b20230618
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.8.1b20230617/setup.py` & `autogluon-0.8.1b20230618/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.8.1b20230617/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.8.1b20230618/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.8.1b20230617
+Version: 0.8.1b20230618
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

