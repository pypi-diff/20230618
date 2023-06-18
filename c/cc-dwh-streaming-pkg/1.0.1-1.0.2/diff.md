# Comparing `tmp/cc_dwh_streaming_pkg-1.0.1.tar.gz` & `tmp/cc_dwh_streaming_pkg-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cc_dwh_streaming_pkg-1.0.1.tar", last modified: Sun Jun 18 14:10:06 2023, max compression
+gzip compressed data, was "dist/cc_dwh_streaming_pkg-1.0.2.tar", last modified: Sun Jun 18 14:44:42 2023, max compression
```

## Comparing `cc_dwh_streaming_pkg-1.0.1.tar` & `cc_dwh_streaming_pkg-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/
--rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/PKG-INFO
--rw-r--r--   0 asafshe    (501) staff       (20)      299 2023-06-18 13:19:36.000000 cc_dwh_streaming_pkg-1.0.1/README.md
-drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/
--rw-r--r--   0 asafshe    (501) staff       (20)        0 2023-06-18 08:53:35.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/__init__.py
--rw-r--r--   0 asafshe    (501) staff       (20)    10758 2023-06-13 08:15:17.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/py_utils.py
--rw-r--r--   0 asafshe    (501) staff       (20)    11973 2023-06-18 09:10:07.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/spark_utils.py
-drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/
--rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/PKG-INFO
--rw-r--r--   0 asafshe    (501) staff       (20)      339 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 asafshe    (501) staff       (20)        1 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 asafshe    (501) staff       (20)       21 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/requires.txt
--rw-r--r--   0 asafshe    (501) staff       (20)       21 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg.egg-info/top_level.txt
--rw-r--r--   0 asafshe    (501) staff       (20)       38 2023-06-18 14:10:06.000000 cc_dwh_streaming_pkg-1.0.1/setup.cfg
--rw-r--r--   0 asafshe    (501) staff       (20)      280 2023-06-18 14:09:58.000000 cc_dwh_streaming_pkg-1.0.1/setup.py
+drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/
+-rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/PKG-INFO
+-rw-r--r--   0 asafshe    (501) staff       (20)      644 2023-06-18 14:42:36.000000 cc_dwh_streaming_pkg-1.0.2/README.md
+drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg/
+-rw-r--r--   0 asafshe    (501) staff       (20)        0 2023-06-18 08:53:35.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg/__init__.py
+-rw-r--r--   0 asafshe    (501) staff       (20)    10758 2023-06-13 08:15:17.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg/py_utils.py
+-rw-r--r--   0 asafshe    (501) staff       (20)    11930 2023-06-18 14:39:13.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg/spark_utils.py
+drwxr-xr-x   0 asafshe    (501) staff       (20)        0 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg.egg-info/
+-rw-r--r--   0 asafshe    (501) staff       (20)      188 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 asafshe    (501) staff       (20)      339 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)        1 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)       17 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg.egg-info/requires.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)       21 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg.egg-info/top_level.txt
+-rw-r--r--   0 asafshe    (501) staff       (20)       38 2023-06-18 14:44:42.000000 cc_dwh_streaming_pkg-1.0.2/setup.cfg
+-rw-r--r--   0 asafshe    (501) staff       (20)      276 2023-06-18 14:44:36.000000 cc_dwh_streaming_pkg-1.0.2/setup.py
```

### Comparing `cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/py_utils.py` & `cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg/py_utils.py`

 * *Files identical despite different names*

### Comparing `cc_dwh_streaming_pkg-1.0.1/cc_dwh_streaming_pkg/spark_utils.py` & `cc_dwh_streaming_pkg-1.0.2/cc_dwh_streaming_pkg/spark_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pyspark.sql.dataframe import DataFrame
 from pyspark.sql.types import StructField, StructType, StringType
 import pyspark.sql.functions as F
 from pyspark.sql.window import Window
 import argparse
-from cs.dwh_streaming.share.cc_dwh_streaming_pkg.py_utils import cs_to_list, get_table_batch_records
+from .py_utils import cs_to_list, get_table_batch_records
 
 
 class KeyValue(argparse.Action):
     """
     Custom action class for argument parsing that takes a list of
     key-value pairs and stores them as a dictionary.
     """
```

