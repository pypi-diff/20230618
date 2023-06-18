# Comparing `tmp/aiorobonect-0.2.1.tar.gz` & `tmp/aiorobonect-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.2.1.tar", last modified: Sun Jun 18 11:58:15 2023, max compression
+gzip compressed data, was "aiorobonect-0.2.2.tar", last modified: Sun Jun 18 12:17:23 2023, max compression
```

## Comparing `aiorobonect-0.2.1.tar` & `aiorobonect-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 11:57:53.000000 aiorobonect-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:17:23.430046 aiorobonect-0.2.2/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 12:16:55.000000 aiorobonect-0.2.2/setup.py
```

### Comparing `aiorobonect-0.2.1/LICENSE` & `aiorobonect-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.1/PKG-INFO` & `aiorobonect-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.1
+Version: 0.2.2
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.1/README.md` & `aiorobonect-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.1/aiorobonect/client.py` & `aiorobonect-0.2.2/aiorobonect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         print(error)
         return False
 
 
 class RobonectException(Exception):
     """Raised when an update has failed."""
 
+    def __init__(self, cmd, exception):
+        self.message = f"Robonect call for cmd {cmd} failed: {exception.message}"
+        super().__init__(self.message)
+
 
 class RobonectClient:
     """Class to communicate with the Robonect API."""
 
     def __init__(self, host, username, password, transform_json=False) -> None:
         """Initialize the Communication API to get data."""
         self.auth = None
@@ -97,15 +101,15 @@
                     response.raise_for_status()
             await self.session_close()
             if self.transform_json:
                 return transform_json_to_single_depth(result)
             return result
         except Exception as exception:
             await self.session_close()
-            raise exception
+            raise RobonectException(command, exception)
 
     async def async_cmds(self, commands=None, bypass_sleeping=False) -> dict:
         """Send command to mower."""
         self.session_start()
         result = await self.state()
         if result:
             result = {"status": result}
```

### Comparing `aiorobonect-0.2.1/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.2.2/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.1
+Version: 0.2.2
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.1/setup.cfg` & `aiorobonect-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.1/setup.py` & `aiorobonect-0.2.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.2.1",
+    version="v0.2.2",
 )
```

