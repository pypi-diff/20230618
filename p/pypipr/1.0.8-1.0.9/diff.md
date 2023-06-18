# Comparing `tmp/pypipr-1.0.8.tar.gz` & `tmp/pypipr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.8.tar", max compression
+gzip compressed data, was "pypipr-1.0.9.tar", max compression
```

## Comparing `pypipr-1.0.8.tar` & `pypipr-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       18 2023-06-18 04:21:11.715384 pypipr-1.0.8/README.md
--rw-r--r--   0        0        0        0 2023-06-17 13:04:18.403397 pypipr-1.0.8/pypipr/__init__.py
--rw-r--r--   0        0        0     4037 2023-06-18 07:01:19.167393 pypipr-1.0.8/pypipr/console.py
--rw-r--r--   0        0        0      854 2023-06-18 07:15:20.971392 pypipr-1.0.8/pypipr/engineering.py
--rw-r--r--   0        0        0     1148 2023-06-18 07:16:20.467392 pypipr-1.0.8/pypipr/flow.py
--rw-r--r--   0        0        0     9143 2023-06-18 07:12:55.259392 pypipr-1.0.8/pypipr/ifunctions.py
--rw-r--r--   0        0        0      436 2023-06-18 04:18:24.039384 pypipr-1.0.8/pypipr/lib.py
--rw-r--r--   0        0        0      665 2023-06-18 02:32:08.963389 pypipr-1.0.8/pypipr/libstd.py
--rw-r--r--   0        0        0      348 2023-06-18 02:32:28.879389 pypipr-1.0.8/pypipr/libvendor.py
--rw-r--r--   0        0        0    42809 2023-06-18 03:39:21.579386 pypipr-1.0.8/pypipr/pypipr copy.py
--rw-r--r--   0        0        0      332 2023-06-18 06:35:45.735394 pypipr-1.0.8/pypipr/pypipr.py
--rw-r--r--   0        0        0    25749 2023-06-18 07:13:14.523392 pypipr-1.0.8/pypipr/uncategorize.py
--rw-r--r--   0        0        0      485 2023-06-18 07:17:19.443392 pypipr-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pypipr-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-06-18 04:21:11.715384 pypipr-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 13:04:18.403397 pypipr-1.0.9/pypipr/__init__.py
+-rw-r--r--   0        0        0     4037 2023-06-18 07:01:19.167393 pypipr-1.0.9/pypipr/console.py
+-rw-r--r--   0        0        0      854 2023-06-18 07:15:20.971392 pypipr-1.0.9/pypipr/engineering.py
+-rw-r--r--   0        0        0     1699 2023-06-18 12:56:11.511688 pypipr-1.0.9/pypipr/flow.py
+-rw-r--r--   0        0        0     9143 2023-06-18 07:12:55.259392 pypipr-1.0.9/pypipr/ifunctions.py
+-rw-r--r--   0        0        0      436 2023-06-18 04:18:24.039384 pypipr-1.0.9/pypipr/lib.py
+-rw-r--r--   0        0        0      665 2023-06-18 02:32:08.963389 pypipr-1.0.9/pypipr/libstd.py
+-rw-r--r--   0        0        0      348 2023-06-18 02:32:28.879389 pypipr-1.0.9/pypipr/libvendor.py
+-rw-r--r--   0        0        0    42809 2023-06-18 03:39:21.579386 pypipr-1.0.9/pypipr/pypipr copy.py
+-rw-r--r--   0        0        0      332 2023-06-18 06:35:45.735394 pypipr-1.0.9/pypipr/pypipr.py
+-rw-r--r--   0        0        0    25749 2023-06-18 07:13:14.523392 pypipr-1.0.9/pypipr/uncategorize.py
+-rw-r--r--   0        0        0      485 2023-06-18 13:04:16.667688 pypipr-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pypipr-1.0.9/PKG-INFO
```

### Comparing `pypipr-1.0.8/pypipr/console.py` & `pypipr-1.0.9/pypipr/console.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.8/pypipr/engineering.py` & `pypipr-1.0.9/pypipr/engineering.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.8/pypipr/flow.py` & `pypipr-1.0.9/pypipr/flow.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,11 +40,24 @@
 
     ```py
     github_pull()
     ```
     """
     console_run("Git Pull", "git pull")
 
+def poetry_update_version(mayor=False, minor=False, patch=True):
+    if mayor:
+        console_run("Update version mayor", "poetry version mayor")
+    if minor:
+        console_run("Update version minor", "poetry version minor")
+    if patch:
+        console_run("Update version patch", "poetry version patch")
 
+def poetry_publish(token=None):
+    if token:
+        console_run("update token", f"poetry config pypi-token.pypi {token}")
+    console_run("Build", "poetry build")
+    console_run("Publish to PyPi.org", "poetry publish")
+    
 
 if __name__ == "__main__":
     print_colorize("Anda menjalankan module pypipr", color=colorama.Fore.RED)
```

### Comparing `pypipr-1.0.8/pypipr/ifunctions.py` & `pypipr-1.0.9/pypipr/ifunctions.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.8/pypipr/libstd.py` & `pypipr-1.0.9/pypipr/libstd.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.8/pypipr/pypipr copy.py` & `pypipr-1.0.9/pypipr/pypipr copy.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.8/pypipr/uncategorize.py` & `pypipr-1.0.9/pypipr/uncategorize.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.8/PKG-INFO` & `pypipr-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypipr
-Version: 1.0.8
+Version: 1.0.9
 Summary: The Python Package Index Project
 Author: ufiapjj
 Author-email: ufiapjj@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

