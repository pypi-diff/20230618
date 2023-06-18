# Comparing `tmp/aiorobonect-0.2.4.tar.gz` & `tmp/aiorobonect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.2.4.tar", last modified: Sun Jun 18 13:45:47 2023, max compression
+gzip compressed data, was "aiorobonect-0.2.5.tar", last modified: Sun Jun 18 14:01:29 2023, max compression
```

## Comparing `aiorobonect-0.2.4.tar` & `aiorobonect-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:45:47.699581 aiorobonect-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 13:45:23.000000 aiorobonect-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 13:45:47.699581 aiorobonect-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 13:45:23.000000 aiorobonect-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:45:47.699581 aiorobonect-0.2.4/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 13:45:23.000000 aiorobonect-0.2.4/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-18 13:45:23.000000 aiorobonect-0.2.4/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 13:45:23.000000 aiorobonect-0.2.4/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 13:45:23.000000 aiorobonect-0.2.4/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:45:47.699581 aiorobonect-0.2.4/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 13:45:47.000000 aiorobonect-0.2.4/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 13:45:47.000000 aiorobonect-0.2.4/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:45:47.000000 aiorobonect-0.2.4/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 13:45:47.000000 aiorobonect-0.2.4/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 13:45:47.000000 aiorobonect-0.2.4/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 13:45:47.699581 aiorobonect-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 13:45:27.000000 aiorobonect-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:01:29.030132 aiorobonect-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 14:01:01.000000 aiorobonect-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 14:01:29.030132 aiorobonect-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 14:01:01.000000 aiorobonect-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:01:29.030132 aiorobonect-0.2.5/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 14:01:01.000000 aiorobonect-0.2.5/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-18 14:01:01.000000 aiorobonect-0.2.5/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 14:01:01.000000 aiorobonect-0.2.5/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 14:01:01.000000 aiorobonect-0.2.5/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:01:29.030132 aiorobonect-0.2.5/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 14:01:28.000000 aiorobonect-0.2.5/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 14:01:28.000000 aiorobonect-0.2.5/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:01:28.000000 aiorobonect-0.2.5/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 14:01:28.000000 aiorobonect-0.2.5/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 14:01:28.000000 aiorobonect-0.2.5/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 14:01:29.030132 aiorobonect-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 14:01:04.000000 aiorobonect-0.2.5/setup.py
```

### Comparing `aiorobonect-0.2.4/LICENSE` & `aiorobonect-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.4/PKG-INFO` & `aiorobonect-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.4
+Version: 0.2.5
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.4/README.md` & `aiorobonect-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.4/aiorobonect/client.py` & `aiorobonect-0.2.5/aiorobonect/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self.session_start()
         try:
             _LOGGER.debug(f"Calling http://{self.host}/json?cmd={command}&{params}")
             async with self.session.get(
                 f"http://{self.host}/json?cmd={command}&{params}"
             ) as response:
                 if response.status == 200:
-                    result = await response.text()
+                    result = await response.text(encoding="iso-8859-15")
                     _LOGGER.debug(f"Rest API call result for {command}: {result}")
                     result = await response.json(encoding="iso-8859-15")
                 if response.status >= 400:
                     await self.session_close()
                     response.raise_for_status()
             await self.session_close()
             if self.transform_json:
```

### Comparing `aiorobonect-0.2.4/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.2.5/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.4
+Version: 0.2.5
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.4/setup.cfg` & `aiorobonect-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.4/setup.py` & `aiorobonect-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.2.4",
+    version="v0.2.5",
 )
```

