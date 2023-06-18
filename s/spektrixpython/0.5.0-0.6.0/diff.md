# Comparing `tmp/spektrixpython-0.5.0.tar.gz` & `tmp/spektrixpython-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spektrixpython-0.5.0.tar", last modified: Thu Oct  4 17:20:17 2018, max compression
+gzip compressed data, was "spektrixpython-0.6.0.tar", max compression
```

## Comparing `spektrixpython-0.5.0.tar` & `spektrixpython-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2018-10-04 17:20:17.000000 spektrixpython-0.5.0/
--rw-r--r--   0 hugh       (501) staff       (20)      378 2018-10-04 17:20:17.000000 spektrixpython-0.5.0/PKG-INFO
--rw-r--r--   0 hugh       (501) staff       (20)      508 2018-10-04 17:13:30.000000 spektrixpython-0.5.0/setup.py
-drwxr-xr-x   0 hugh       (501) staff       (20)        0 2018-10-04 17:20:17.000000 spektrixpython-0.5.0/spektrixpython/
--rw-r--r--   0 hugh       (501) staff       (20)     2963 2018-10-04 17:13:02.000000 spektrixpython-0.5.0/spektrixpython/spektrixpython.py
--rw-r--r--   0 hugh       (501) staff       (20)       65 2018-10-04 17:12:02.000000 spektrixpython-0.5.0/spektrixpython/__init__.py
--rw-r--r--   0 hugh       (501) staff       (20)       40 2018-03-06 20:58:11.000000 spektrixpython-0.5.0/setup.cfg
+-rw-r--r--   0        0        0     1076 2023-06-18 15:18:41.900106 spektrixpython-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1276 2023-06-18 15:18:41.900281 spektrixpython-0.6.0/README.md
+-rw-r--r--   0        0        0      514 2023-06-18 15:21:57.428065 spektrixpython-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-06-18 15:18:41.900606 spektrixpython-0.6.0/spektrixpython/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-18 15:18:41.900699 spektrixpython-0.6.0/spektrixpython/spektrixpython.py
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 spektrixpython-0.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spektrixpython-0.5.0/spektrixpython/spektrixpython.py` & `spektrixpython-0.6.0/spektrixpython/spektrixpython.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,33 @@
 from datetime import datetime
 from hashlib import sha1, md5
 import hmac
 from base64 import b64encode, b64decode
 
 
 class SpektrixCredentials(object):
-
     def __init__(self, client_name, api_user, api_key):
         self.client_name = client_name
         self.api_user = api_user
         self.api_key = api_key
 
 
-class SpektrixRequest(object):
+class SpektrixAnonymous(object):
+    def __init__(self, client_name):
+        self.client_name = client_name
+        self.api_user = None
+        self.api_key = None
 
+
+class SpektrixRequest(object):
     def __init__(self, endpoint, credentials):
 
         self.spektrix_api_user = credentials.api_user
         self.spektrix_api_key = credentials.api_key
+        self.has_credentials = isinstance(credentials, SpektrixCredentials)
 
         base_url = "https://system.spektrix.com/" + credentials.client_name + "/api/v3/"
         self.url = base_url + endpoint
 
     def get(self):
         self.method = "GET"
         response = self._make_request()
@@ -47,14 +53,17 @@
 
     def delete(self, payload=None):
         self.method = "DELETE"
         response = self._make_request(payload)
         return response
 
     def _generate_auth_headers(self, payload=None):
+        if not self.has_credentials:
+            return {}
+
         date = datetime.utcnow().strftime("%a, %d %b %Y %H:%M:%S GMT")
 
         string_to_sign = self.method + "\n" + self.url + "\n" + date
 
         if self.method != "GET":
             body_string = dumps(payload).encode("utf-8")
             body_string = md5(body_string).digest()
```

