# Comparing `tmp/convertio_python-0.1.0.tar.gz` & `tmp/convertio_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convertio_python-0.1.0.tar", max compression
+gzip compressed data, was "convertio_python-0.1.1.tar", max compression
```

## Comparing `convertio_python-0.1.0.tar` & `convertio_python-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-17 20:41:00.725851 convertio_python-0.1.0/convertio/__init__.py
--rw-r--r--   0        0        0     6971 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/client.py
--rw-r--r--   0        0        0    11614 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/client_test.py
--rw-r--r--   0        0        0     1868 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/languages.py
--rw-r--r--   0        0        0        0 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/models/models_test.py
--rw-r--r--   0        0        0     4611 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/models/parameters.py
--rw-r--r--   0        0        0     6210 2023-06-17 20:41:00.733449 convertio_python-0.1.0/convertio/models/responses.py
--rw-r--r--   0        0        0      444 2023-06-18 11:32:49.447932 convertio_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       14 2023-06-18 11:38:05.398878 convertio_python-0.1.0/README.md
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 convertio_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 20:41:00.725851 convertio_python-0.1.1/convertio/__init__.py
+-rw-r--r--   0        0        0     6971 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/client.py
+-rw-r--r--   0        0        0    11614 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/client_test.py
+-rw-r--r--   0        0        0     1868 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/languages.py
+-rw-r--r--   0        0        0        0 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/models/models_test.py
+-rw-r--r--   0        0        0     4611 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/models/parameters.py
+-rw-r--r--   0        0        0     6210 2023-06-17 20:41:00.733449 convertio_python-0.1.1/convertio/models/responses.py
+-rw-r--r--   0        0        0      444 2023-06-18 11:57:44.077682 convertio_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2396 2023-06-18 11:57:11.308792 convertio_python-0.1.1/README.md
+-rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 convertio_python-0.1.1/PKG-INFO
```

### Comparing `convertio_python-0.1.0/convertio/client.py` & `convertio_python-0.1.1/convertio/client.py`

 * *Files identical despite different names*

### Comparing `convertio_python-0.1.0/convertio/client_test.py` & `convertio_python-0.1.1/convertio/client_test.py`

 * *Files identical despite different names*

### Comparing `convertio_python-0.1.0/convertio/languages.py` & `convertio_python-0.1.1/convertio/languages.py`

 * *Files identical despite different names*

### Comparing `convertio_python-0.1.0/convertio/models/models_test.py` & `convertio_python-0.1.1/convertio/models/models_test.py`

 * *Files identical despite different names*

### Comparing `convertio_python-0.1.0/convertio/models/parameters.py` & `convertio_python-0.1.1/convertio/models/parameters.py`

 * *Files identical despite different names*

### Comparing `convertio_python-0.1.0/convertio/models/responses.py` & `convertio_python-0.1.1/convertio/models/responses.py`

 * *Files identical despite different names*

