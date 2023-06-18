# Comparing `tmp/datawise-0.0.3.tar.gz` & `tmp/datawise-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.3.tar", max compression
+gzip compressed data, was "datawise-0.0.4.tar", max compression
```

## Comparing `datawise-0.0.3.tar` & `datawise-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.3/LICENSE
--rw-r--r--   0        0        0     2958 2023-06-18 11:33:26.090801 datawise-0.0.3/datawise/__init__.py
--rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.3/datawise/exceptions.py
--rw-r--r--   0        0        0      485 2023-06-18 11:30:59.853996 datawise-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 datawise-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2958 2023-06-18 11:33:26.090801 datawise-0.0.4/datawise/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.4/datawise/exceptions.py
+-rw-r--r--   0        0        0      490 2023-06-18 11:54:42.191364 datawise-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 datawise-0.0.4/PKG-INFO
```

### Comparing `datawise-0.0.3/LICENSE` & `datawise-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.3/datawise/__init__.py` & `datawise-0.0.4/datawise/__init__.py`

 * *Files identical despite different names*

