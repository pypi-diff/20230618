# Comparing `tmp/rabbitmq-api-admin-0.3.0.tar.gz` & `tmp/rabbitmq_api_admin-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq-api-admin-0.3.0.tar", max compression
+gzip compressed data, was "rabbitmq_api_admin-0.4.0.tar", max compression
```

## Comparing `rabbitmq-api-admin-0.3.0.tar` & `rabbitmq_api_admin-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11333 2022-08-23 21:18:12.193390 rabbitmq-api-admin-0.3.0/LICENSE
--rw-r--r--   0        0        0      601 2022-08-23 21:18:12.193390 rabbitmq-api-admin-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       47 2022-08-23 21:18:12.193390 rabbitmq-api-admin-0.3.0/rabbitmq_admin/__init__.py
--rw-r--r--   0        0        0    20118 2022-08-23 21:18:12.193390 rabbitmq-api-admin-0.3.0/rabbitmq_admin/api.py
--rw-r--r--   0        0        0     4704 2022-08-23 21:18:12.193390 rabbitmq-api-admin-0.3.0/rabbitmq_admin/base.py
--rw-r--r--   0        0        0      694 2022-08-23 21:18:22.148939 rabbitmq-api-admin-0.3.0/setup.py
--rw-r--r--   0        0        0      655 2022-08-23 21:18:22.149229 rabbitmq-api-admin-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11333 2023-06-18 18:04:46.260356 rabbitmq_api_admin-0.4.0/LICENSE
+-rw-r--r--   0        0        0      601 2023-06-18 18:04:46.260356 rabbitmq_api_admin-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-18 18:04:46.260356 rabbitmq_api_admin-0.4.0/rabbitmq_admin/__init__.py
+-rw-r--r--   0        0        0    20118 2023-06-18 18:04:46.260356 rabbitmq_api_admin-0.4.0/rabbitmq_admin/api.py
+-rw-r--r--   0        0        0     4704 2023-06-18 18:04:46.260356 rabbitmq_api_admin-0.4.0/rabbitmq_admin/base.py
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 rabbitmq_api_admin-0.4.0/PKG-INFO
```

### Comparing `rabbitmq-api-admin-0.3.0/LICENSE` & `rabbitmq_api_admin-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabbitmq-api-admin-0.3.0/pyproject.toml` & `rabbitmq_api_admin-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabbitmq-api-admin"
-version = "0.3.0"
+version = "0.4.0"
 description = "A python interface for the RabbitMQ Admin HTTP API"
 authors = ["UMA.TECH <developers@uma.tech>"]
 license = "Apache License 2.0"
 repository = "https://github.com/Uma-Tech/rabbitmq-api-admin"
 exclude = ["rabbitmq_admin/tests"]
 packages = [
     { include = "rabbitmq_admin" },
@@ -12,16 +12,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
 # tests
-coverage = "^6.4"
-pika = "~1.3.0"
+coverage = "^7.2"
+pika = "~1.3.2"
 
 # linting
 flake8 = "~5.0.4"
 
 [build-system]
 requires = ["poetry>=1.0.5"]
 build-backend = "poetry.masonry.api"
```

### Comparing `rabbitmq-api-admin-0.3.0/rabbitmq_admin/api.py` & `rabbitmq_api_admin-0.4.0/rabbitmq_admin/api.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-api-admin-0.3.0/rabbitmq_admin/base.py` & `rabbitmq_api_admin-0.4.0/rabbitmq_admin/base.py`

 * *Files identical despite different names*

### Comparing `rabbitmq-api-admin-0.3.0/PKG-INFO` & `rabbitmq_api_admin-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: rabbitmq-api-admin
-Version: 0.3.0
+Version: 0.4.0
 Summary: A python interface for the RabbitMQ Admin HTTP API
 Home-page: https://github.com/Uma-Tech/rabbitmq-api-admin
 License: Apache-2.0
 Author: UMA.TECH
 Author-email: developers@uma.tech
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/Uma-Tech/rabbitmq-api-admin
```

