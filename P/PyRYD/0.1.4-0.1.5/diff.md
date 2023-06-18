# Comparing `tmp/PyRYD-0.1.4.tar.gz` & `tmp/PyRYD-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyRYD-0.1.4.tar", last modified: Fri Apr 16 09:06:32 2021, max compression
+gzip compressed data, was "PyRYD-0.1.5.tar", last modified: Sun Jun 18 06:52:40 2023, max compression
```

## Comparing `PyRYD-0.1.4.tar` & `PyRYD-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 yannikmundler   (501) staff       (20)        0 2021-04-16 09:06:32.420032 PyRYD-0.1.4/
--rw-r--r--   0 yannikmundler   (501) staff       (20)     1368 2021-04-16 09:06:32.419910 PyRYD-0.1.4/PKG-INFO
-drwxr-xr-x   0 yannikmundler   (501) staff       (20)        0 2021-04-16 09:06:32.419555 PyRYD-0.1.4/PyRYD.egg-info/
--rw-r--r--   0 yannikmundler   (501) staff       (20)     1368 2021-04-16 09:06:32.000000 PyRYD-0.1.4/PyRYD.egg-info/PKG-INFO
--rw-r--r--   0 yannikmundler   (501) staff       (20)      210 2021-04-16 09:06:32.000000 PyRYD-0.1.4/PyRYD.egg-info/SOURCES.txt
--rw-r--r--   0 yannikmundler   (501) staff       (20)        1 2021-04-16 09:06:32.000000 PyRYD-0.1.4/PyRYD.egg-info/dependency_links.txt
--rw-r--r--   0 yannikmundler   (501) staff       (20)        9 2021-04-16 09:06:32.000000 PyRYD-0.1.4/PyRYD.egg-info/requires.txt
--rw-r--r--   0 yannikmundler   (501) staff       (20)        6 2021-04-16 09:06:32.000000 PyRYD-0.1.4/PyRYD.egg-info/top_level.txt
--rw-r--r--   0 yannikmundler   (501) staff       (20)      589 2021-04-07 15:05:25.000000 PyRYD-0.1.4/README.md
--rw-r--r--   0 yannikmundler   (501) staff       (20)      103 2021-03-24 19:52:07.000000 PyRYD-0.1.4/pyproject.toml
-drwxr-xr-x   0 yannikmundler   (501) staff       (20)        0 2021-04-16 09:06:32.419760 PyRYD-0.1.4/pyryd/
--rw-r--r--   0 yannikmundler   (501) staff       (20)      402 2021-04-16 09:05:48.000000 PyRYD-0.1.4/pyryd/__init__.py
--rw-r--r--   0 yannikmundler   (501) staff       (20)     5374 2021-04-16 09:05:48.000000 PyRYD-0.1.4/pyryd/pyryd.py
--rw-r--r--   0 yannikmundler   (501) staff       (20)       38 2021-04-16 09:06:32.420073 PyRYD-0.1.4/setup.cfg
--rw-r--r--   0 yannikmundler   (501) staff       (20)     1195 2021-04-07 16:31:55.000000 PyRYD-0.1.4/setup.py
+drwxr-xr-x   0 yannikmundler   (501) staff       (20)        0 2023-06-18 06:52:40.987405 PyRYD-0.1.5/
+-rw-r--r--   0 yannikmundler   (501) staff       (20)     1065 2021-02-16 16:48:15.000000 PyRYD-0.1.5/LICENSE
+-rw-r--r--   0 yannikmundler   (501) staff       (20)     1127 2023-06-18 06:52:40.987300 PyRYD-0.1.5/PKG-INFO
+drwxr-xr-x   0 yannikmundler   (501) staff       (20)        0 2023-06-18 06:52:40.986927 PyRYD-0.1.5/PyRYD.egg-info/
+-rw-r--r--   0 yannikmundler   (501) staff       (20)     1127 2023-06-18 06:52:40.000000 PyRYD-0.1.5/PyRYD.egg-info/PKG-INFO
+-rw-r--r--   0 yannikmundler   (501) staff       (20)      218 2023-06-18 06:52:40.000000 PyRYD-0.1.5/PyRYD.egg-info/SOURCES.txt
+-rw-r--r--   0 yannikmundler   (501) staff       (20)        1 2023-06-18 06:52:40.000000 PyRYD-0.1.5/PyRYD.egg-info/dependency_links.txt
+-rw-r--r--   0 yannikmundler   (501) staff       (20)        9 2023-06-18 06:52:40.000000 PyRYD-0.1.5/PyRYD.egg-info/requires.txt
+-rw-r--r--   0 yannikmundler   (501) staff       (20)        6 2023-06-18 06:52:40.000000 PyRYD-0.1.5/PyRYD.egg-info/top_level.txt
+-rw-r--r--   0 yannikmundler   (501) staff       (20)      589 2021-04-07 15:05:25.000000 PyRYD-0.1.5/README.md
+-rw-r--r--   0 yannikmundler   (501) staff       (20)      103 2021-03-24 19:52:07.000000 PyRYD-0.1.5/pyproject.toml
+drwxr-xr-x   0 yannikmundler   (501) staff       (20)        0 2023-06-18 06:52:40.987146 PyRYD-0.1.5/pyryd/
+-rw-r--r--   0 yannikmundler   (501) staff       (20)      402 2023-06-18 06:52:08.000000 PyRYD-0.1.5/pyryd/__init__.py
+-rw-r--r--   0 yannikmundler   (501) staff       (20)     5370 2023-06-18 06:51:50.000000 PyRYD-0.1.5/pyryd/pyryd.py
+-rw-r--r--   0 yannikmundler   (501) staff       (20)       38 2023-06-18 06:52:40.987441 PyRYD-0.1.5/setup.cfg
+-rw-r--r--   0 yannikmundler   (501) staff       (20)     1195 2021-04-07 16:31:55.000000 PyRYD-0.1.5/setup.py
```

### Comparing `PyRYD-0.1.4/README.md` & `PyRYD-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PyRYD-0.1.4/pyryd/pyryd.py` & `PyRYD-0.1.5/pyryd/pyryd.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             "X-Txn-Locale": ryd_app_locale,
             "Content-Type": "application/json; charset=utf-8",
         }
         self._data = json.dumps({"email": user_email, "password": user_passwd})
 
     def fetch(self):
         response = requests.post(
-            "{}/auth%2Flogin%2Flocal".format(self._ryd_api_server),
+            "{}/auth/login/local".format(self._ryd_api_server),
             data=self._data,
             headers=self._headers,
             timeout=2000,
         )
         json_object = response.json()
 
         ryd_auth_token = json_object["auth_token"]
```

### Comparing `PyRYD-0.1.4/setup.py` & `PyRYD-0.1.5/setup.py`

 * *Files identical despite different names*

