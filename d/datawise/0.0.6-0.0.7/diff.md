# Comparing `tmp/datawise-0.0.6.tar.gz` & `tmp/datawise-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawise-0.0.6.tar", max compression
+gzip compressed data, was "datawise-0.0.7.tar", max compression
```

## Comparing `datawise-0.0.6.tar` & `datawise-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.6/LICENSE
--rw-r--r--   0        0        0     4287 2023-06-18 13:09:36.174443 datawise-0.0.6/README.md
--rw-r--r--   0        0        0     3133 2023-06-18 12:58:49.702867 datawise-0.0.6/datawise/__init__.py
--rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.6/datawise/exceptions.py
--rw-r--r--   0        0        0      518 2023-06-18 13:26:43.075006 datawise-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4662 1970-01-01 00:00:00.000000 datawise-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datawise-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4287 2023-06-18 13:09:36.174443 datawise-0.0.7/README.md
+-rw-r--r--   0        0        0     3133 2023-06-18 12:58:49.702867 datawise-0.0.7/datawise/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-18 12:46:33.125357 datawise-0.0.7/datawise/exceptions.py
+-rw-r--r--   0        0        0      517 2023-06-18 13:33:56.718918 datawise-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4813 1970-01-01 00:00:00.000000 datawise-0.0.7/PKG-INFO
```

### Comparing `datawise-0.0.6/LICENSE` & `datawise-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datawise-0.0.6/README.md` & `datawise-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `datawise-0.0.6/datawise/__init__.py` & `datawise-0.0.7/datawise/__init__.py`

 * *Files identical despite different names*

### Comparing `datawise-0.0.6/pyproject.toml` & `datawise-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "datawise"
-version = "0.0.6"
+version = "0.0.7"
 description = "Testing"
 authors = ["DataWise Team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11.4"
+python = "^3.9.0"
 python-dotenv = "^1.0.0"
 requests = "2.31.0"
 retry = "^0.9.2"
 urllib3 = "^1.26.6"
 
 [tool.poetry.dev-dependencies]
 black = "^21.9b0"
```

### Comparing `datawise-0.0.6/PKG-INFO` & `datawise-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: datawise
-Version: 0.0.6
+Version: 0.0.7
 Summary: Testing
 Author: DataWise Team
-Requires-Python: >=3.11.4,<4.0.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # DataWise
```

