# Comparing `tmp/cc_dwh_streaming_pkg-1.0.0.tar.gz` & `tmp/cc_dwh_streaming_pkg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cc_dwh_streaming_pkg-1.0.0.tar", last modified: Sun Jun 18 11:34:56 2023, max compression
+gzip compressed data, was "dist/cc_dwh_streaming_pkg-1.0.1.tar", last modified: Sun Jun 18 14:10:06 2023, max compression
```

## Comparing `cc_dwh_streaming_pkg-1.0.0.tar` & `cc_dwh_streaming_pkg-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/
--rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/PKG-INFO
--rw-r--r--   0 asafshe    (501) staff       (20)       23 2023-06-18 11:33:36.000000 cc_dwh_streaming_pkg-1.0.0/README.md
-drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg/
--rw-r--r--   0 asafshe    (501) staff       (20)        0 2023-06-18 08:53:35.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg/__init__.py
--rw-r--r--   0 asafshe    (501) staff       (20)    10758 2023-06-13 08:15:17.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg/py_utils.py
--rw-r--r--   0 asafshe    (501) staff       (20)    11973 2023-06-18 09:10:07.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg/spark_utils.py
-drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg.egg-info/
--rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg.egg-info/PKG-INFO
--rw-r--r--   0 asafshe    (501) staff       (20)      339 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 asafshe    (501) staff       (20)        1 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 asafshe    (501) staff       (20)       17 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg.egg-info/requires.txt
--rw-r--r--   0 asafshe    (501) staff       (20)       21 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg.egg-info/top_level.txt
--rw-r--r--   0 asafshe    (501) staff       (20)       38 2023-06-18 11:34:56.000000 cc_dwh_streaming_pkg-1.0.0/setup.cfg
--rw-r--r--   0 asafshe    (501) staff       (20)      276 2023-06-18 11:19:31.000000 cc_dwh_streaming_pkg-1.0.0/setup.py
+drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/
+-rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/PKG-INFO
+-rw-r--r--   0 asafshe    (501) staff       (20)      299 2023-06-18 13:19:36.000000 cc_dwh_streaming_pkg-1.0.1/README.md
+drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/
+-rw-r--r--   0 asafshe    (501) staff       (20)        0 2023-06-18 08:53:35.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/__init__.py
+-rw-r--r--   0 asafshe    (501) staff       (20)    10758 2023-06-13 08:15:17.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/py_utils.py
+-rw-r--r--   0 asafshe    (501) staff       (20)    11973 2023-06-18 09:10:07.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/spark_utils.py
+drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/
+-rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 asafshe    (501) staff       (20)      339 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)        1 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)       21 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/requires.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)       21 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/top_level.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)       38 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/setup.cfg
+-rw-r--r--   0 asafshe    (501) staff       (20)      280 2023-06-18 14:09:58.000000 cc_dwh_streaming_pkg-1.0.1/setup.py
```

### Comparing `cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg/py_utils.py` & `cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/py_utils.py`

 * *Files identical despite different names*

### Comparing `cc_dwh_streaming_pkg-1.0.0/cc_dwh_streaming_pkg/spark_utils.py` & `cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/spark_utils.py`

 * *Files identical despite different names*

