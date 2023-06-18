# Comparing `tmp/spektrixpython-0.6.0.tar.gz` & `tmp/spektrixpython-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spektrixpython-0.6.0.tar", max compression
+gzip compressed data, was "spektrixpython-0.6.1.tar", max compression
```

## Comparing `spektrixpython-0.6.0.tar` & `spektrixpython-0.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-06-18 15:18:41.900106 spektrixpython-0.6.0/LICENSE
--rw-r--r--   0        0        0     1276 2023-06-18 15:18:41.900281 spektrixpython-0.6.0/README.md
--rw-r--r--   0        0        0      514 2023-06-18 15:21:57.428065 spektrixpython-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       65 2023-06-18 15:18:41.900606 spektrixpython-0.6.0/spektrixpython/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-18 15:18:41.900699 spektrixpython-0.6.0/spektrixpython/spektrixpython.py
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 spektrixpython-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 15:18:41.900106 spektrixpython-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1276 2023-06-18 15:18:41.900281 spektrixpython-0.6.1/README.md
+-rw-r--r--   0        0        0      514 2023-06-18 15:29:56.714476 spektrixpython-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-06-18 15:28:40.667982 spektrixpython-0.6.1/spektrixpython/__init__.py
+-rw-r--r--   0        0        0     3263 2023-06-18 15:29:06.171468 spektrixpython-0.6.1/spektrixpython/spektrixpython.py
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 spektrixpython-0.6.1/PKG-INFO
```

### Comparing `spektrixpython-0.6.0/LICENSE` & `spektrixpython-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spektrixpython-0.6.0/README.md` & `spektrixpython-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `spektrixpython-0.6.0/pyproject.toml` & `spektrixpython-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spektrixpython"
-version = "0.6.0"
+version = "0.6.1"
 description = "A Python 3 module for interacting with Spektrix API v3. This module is written by a third party and is not supported by or affiliated with Spektrix."
 authors = ["Hugh Topping <hugh@crowdengage.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `spektrixpython-0.6.0/spektrixpython/spektrixpython.py` & `spektrixpython-0.6.1/spektrixpython/spektrixpython.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.client_name = client_name
         self.api_user = None
         self.api_key = None
 
 
 class SpektrixRequest(object):
     def __init__(self, endpoint, credentials):
-
         self.spektrix_api_user = credentials.api_user
         self.spektrix_api_key = credentials.api_key
         self.has_credentials = isinstance(credentials, SpektrixCredentials)
 
         base_url = "https://system.spektrix.com/" + credentials.client_name + "/api/v3/"
         self.url = base_url + endpoint
 
@@ -82,15 +81,14 @@
         headers["Authorization"] = "SpektrixAPI3 {}:{}".format(
             self.spektrix_api_user, signature
         )
 
         return headers
 
     def _make_request(self, payload=None):
-
         if payload == None:
             # Spektrix assumes any non-GET request must have a body.
             payload = {}
         else:
             payload = [payload]
 
         headers = self._generate_auth_headers(payload)
```

### Comparing `spektrixpython-0.6.0/PKG-INFO` & `spektrixpython-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spektrixpython
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Python 3 module for interacting with Spektrix API v3. This module is written by a third party and is not supported by or affiliated with Spektrix.
 License: MIT
 Author: Hugh Topping
 Author-email: hugh@crowdengage.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

