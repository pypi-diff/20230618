# Comparing `tmp/datawise-0.0.4.tar.gz` & `tmp/datawise-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.4.tar", max compression
+gzip compressed data, was "datawise-0.0.5.tar", max compression
```

## Comparing `datawise-0.0.4.tar` & `datawise-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.4/LICENSE
--rw-r--r--   0        0        0     2958 2023-06-18 11:33:26.090801 datawise-0.0.4/datawise/__init__.py
--rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.4/datawise/exceptions.py
--rw-r--r--   0        0        0      490 2023-06-18 11:54:42.191364 datawise-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      326 1970-01-01 00:00:00.000000 datawise-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.5/LICENSE
+-rw-r--r--   0        0        0      246 2023-06-18 12:01:49.863596 datawise-0.0.5/README.md
+-rw-r--r--   0        0        0     2958 2023-06-18 11:33:26.090801 datawise-0.0.5/datawise/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-18 02:49:50.939696 datawise-0.0.5/datawise/exceptions.py
+-rw-r--r--   0        0        0      518 2023-06-18 12:02:44.548265 datawise-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 datawise-0.0.5/PKG-INFO
```

### Comparing `datawise-0.0.4/LICENSE` & `datawise-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.4/datawise/__init__.py` & `datawise-0.0.5/datawise/__init__.py`

 * *Files identical despite different names*

