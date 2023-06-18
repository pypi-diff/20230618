# Comparing `tmp/ezsession-0.0.6.tar.gz` & `tmp/ezsession-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsession-0.0.6.tar", last modified: Tue May 30 16:36:26 2023, max compression
+gzip compressed data, was "ezsession-0.0.7.tar", last modified: Sun Jun 18 12:20:29 2023, max compression
```

## Comparing `ezsession-0.0.6.tar` & `ezsession-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 16:36:13.000000 ezsession-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-30 16:36:26.982659 ezsession-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-30 16:36:13.000000 ezsession-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 16:36:13.000000 ezsession-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 16:36:13.000000 ezsession-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:36:26.982659 ezsession-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-30 16:36:13.000000 ezsession-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/src/ezsession/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-30 16:36:13.000000 ezsession-0.0.6/src/ezsession/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:36:26.982659 ezsession-0.0.6/src/ezsession.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 16:36:26.000000 ezsession-0.0.6/src/ezsession.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:20:29.659453 ezsession-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 12:20:16.000000 ezsession-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-18 12:20:29.659453 ezsession-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-18 12:20:16.000000 ezsession-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 12:20:16.000000 ezsession-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 12:20:16.000000 ezsession-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 12:20:29.659453 ezsession-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-18 12:20:16.000000 ezsession-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:20:29.655453 ezsession-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:20:29.655453 ezsession-0.0.7/src/ezsession/
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-18 12:20:16.000000 ezsession-0.0.7/src/ezsession/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:20:29.659453 ezsession-0.0.7/src/ezsession.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-18 12:20:29.000000 ezsession-0.0.7/src/ezsession.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-18 12:20:29.000000 ezsession-0.0.7/src/ezsession.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:20:29.000000 ezsession-0.0.7/src/ezsession.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-18 12:20:29.000000 ezsession-0.0.7/src/ezsession.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 12:20:29.000000 ezsession-0.0.7/src/ezsession.egg-info/top_level.txt
```

### Comparing `ezsession-0.0.6/PKG-INFO` & `ezsession-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
```

### Comparing `ezsession-0.0.6/README.md` & `ezsession-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ezsession-0.0.6/setup.py` & `ezsession-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 with open(os.path.join(this_directory, "requirements.txt")) as f:
     requirements = f.read().splitlines()
 
 setup(
     name="ezsession",
-    version="0.0.6",
+    version="0.0.7",
     description="A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `ezsession-0.0.6/src/ezsession/__init__.py` & `ezsession-0.0.7/src/ezsession/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import requests
 import json
 import base64
-from requests.auth import HTTPBasicAuth
+from requests.auth import HTTPBasicAuth, HTTPDigestAuth
 
 
-def get_session(auth):
+def get_session(**auth):
     session = requests.Session()
     session = session
     session.headers = {"Content-Type": "application/json", "Accept": "application/json"}
+    input_keys = [
+        "auth_uri",
+        "client_id",
+        "client_secret",
+        "audience",
+        "username",
+        "password",
+        "type",
+        "api_key",
+    ]
+    if "auth" in auth:
+        auth.update(**auth["auth"])
     if auth != None:
-        if auth["type"] == "oauth":
+        if auth["type"] == "digest":
+            session.auth = HTTPDigestAuth(auth["username"], auth["password"])
+        elif auth["type"] == "oauth":
             body = {
                 "client_id": auth["client_id"],
                 "client_secret": auth["client_secret"],
                 "audience": auth["audience"],
                 "grant_type": "client_credentials",
             }
             response = session.post(
@@ -101,8 +115,11 @@
                 + " "
                 + auth_request["access_token"],
                 "Content-Type": "application/json",
                 "Accept": "application/json",
             }
         else:
             session.headers.update(auth)
+    for key in auth:
+        if key not in input_keys:
+            session.headers.update({key: auth[key]})
     return session
```

### Comparing `ezsession-0.0.6/src/ezsession.egg-info/PKG-INFO` & `ezsession-0.0.7/src/ezsession.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
```

