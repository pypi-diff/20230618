# Comparing `tmp/aiorobonect-0.2.2.tar.gz` & `tmp/aiorobonect-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.2.2.tar", last modified: Sun Jun 18 12:17:23 2023, max compression
+gzip compressed data, was "aiorobonect-0.2.3.tar", last modified: Sun Jun 18 12:48:31 2023, max compression
```

## Comparing `aiorobonect-0.2.2.tar` & `aiorobonect-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:17:23.430046 aiorobonect-0.2.2/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 12:16:52.000000 aiorobonect-0.2.2/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 12:17:23.000000 aiorobonect-0.2.2/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 12:17:23.434046 aiorobonect-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 12:16:55.000000 aiorobonect-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:48:31.282889 aiorobonect-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 12:48:09.000000 aiorobonect-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 12:48:31.282889 aiorobonect-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 12:48:09.000000 aiorobonect-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:48:31.282889 aiorobonect-0.2.3/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 12:48:09.000000 aiorobonect-0.2.3/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-18 12:48:09.000000 aiorobonect-0.2.3/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 12:48:09.000000 aiorobonect-0.2.3/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 12:48:09.000000 aiorobonect-0.2.3/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 12:48:31.282889 aiorobonect-0.2.3/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 12:48:31.000000 aiorobonect-0.2.3/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 12:48:31.000000 aiorobonect-0.2.3/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 12:48:31.000000 aiorobonect-0.2.3/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 12:48:31.000000 aiorobonect-0.2.3/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 12:48:31.000000 aiorobonect-0.2.3/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 12:48:31.282889 aiorobonect-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 12:48:12.000000 aiorobonect-0.2.3/setup.py
```

### Comparing `aiorobonect-0.2.2/LICENSE` & `aiorobonect-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.2/PKG-INFO` & `aiorobonect-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.2
+Version: 0.2.3
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.2/README.md` & `aiorobonect-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.2/aiorobonect/client.py` & `aiorobonect-0.2.3/aiorobonect/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .const import TIMEOUT
 from .utils import transform_json_to_single_depth
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def encode_dict_values_to_utf8(dictionary):
+    """Encode dict values to utf8."""
     encoded_dict = {}
     for key, value in dictionary.items():
         if isinstance(value, dict):
             encoded_dict[key] = encode_dict_values_to_utf8(value)
         elif isinstance(value, str):
             encoded_dict[key] = value.encode("utf-8")
         else:
@@ -36,15 +37,16 @@
         return False
 
 
 class RobonectException(Exception):
     """Raised when an update has failed."""
 
     def __init__(self, cmd, exception):
-        self.message = f"Robonect call for cmd {cmd} failed: {exception.message}"
+        """Init the Robonect Exception."""
+        self.message = f"Robonect call for cmd {cmd} failed: {exception}"
         super().__init__(self.message)
 
 
 class RobonectClient:
     """Class to communicate with the Robonect API."""
 
     def __init__(self, host, username, password, transform_json=False) -> None:
```

### Comparing `aiorobonect-0.2.2/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.2.3/aiorobonect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.2
+Version: 0.2.3
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.2/setup.cfg` & `aiorobonect-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.2/setup.py` & `aiorobonect-0.2.3/setup.py`

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
-    version="v0.2.2",
+    version="v0.2.3",
 )
```

