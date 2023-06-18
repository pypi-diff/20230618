# Comparing `tmp/fastapi_throttling-0.1.7.tar.gz` & `tmp/fastapi_throttling-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.7.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.8.tar", max compression
```

## Comparing `fastapi_throttling-0.1.7.tar` & `fastapi_throttling-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/LICENSE
--rw-r--r--   0        0        0     1347 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/README.md
--rw-r--r--   0        0        0     1753 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     2949 2023-06-14 17:56:21.981858 fastapi_throttling-0.1.7/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1347 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/README.md
+-rw-r--r--   0        0        0     1753 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     4435 2023-06-18 20:13:51.703935 fastapi_throttling-0.1.8/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.8/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.7/LICENSE` & `fastapi_throttling-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.7/README.md` & `fastapi_throttling-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.7/pyproject.toml` & `fastapi_throttling-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.7"
+version = "0.1.8"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `fastapi_throttling-0.1.7/PKG-INFO` & `fastapi_throttling-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.7
+Version: 0.1.8
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

