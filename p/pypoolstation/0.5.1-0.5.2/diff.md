# Comparing `tmp/pypoolstation-0.5.1.tar.gz` & `tmp/pypoolstation-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypoolstation-0.5.1.tar", max compression
+gzip compressed data, was "pypoolstation-0.5.2.tar", max compression
```

## Comparing `pypoolstation-0.5.1.tar` & `pypoolstation-0.5.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1055 2022-05-27 14:55:13.547093 pypoolstation-0.5.1/LICENSE
--rw-r--r--   0        0        0     8767 2023-06-18 09:10:00.063730 pypoolstation-0.5.1/pypoolstation/__init__.py
--rw-r--r--   0        0        0      444 2023-06-18 09:10:45.855157 pypoolstation-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pypoolstation-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-05-27 14:55:13.547093 pypoolstation-0.5.2/LICENSE
+-rw-r--r--   0        0        0     8693 2023-06-18 20:03:44.452041 pypoolstation-0.5.2/pypoolstation/__init__.py
+-rw-r--r--   0        0        0      444 2023-06-18 20:04:10.359437 pypoolstation-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 pypoolstation-0.5.2/PKG-INFO
```

### Comparing `pypoolstation-0.5.1/LICENSE` & `pypoolstation-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypoolstation-0.5.1/pypoolstation/__init__.py` & `pypoolstation-0.5.2/pypoolstation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import json
 from aiohttp import ClientError, ClientResponseError
 import logging
-from importlib_metadata import version
 
-__version__ = version(__package__)
 DOMAIN = 'https://api.idegis.net'
 LOGIN_URL = DOMAIN + '/session/login'
 POOL_LIST_URL = DOMAIN + '/devices/10/0'
 POOL_INFO_URL = DOMAIN + '/devices/'
 UPDATE_URL = DOMAIN + '/devices/saveSign'
 
 API_SIGNS = {
```

### Comparing `pypoolstation-0.5.1/PKG-INFO` & `pypoolstation-0.5.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypoolstation
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python library to interact with the API of the Poolstation (https://poolstation.net) domotic platform for pool equipment
 License: MIT
 Author: cibernox
 Author-email: miguel.camba@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

