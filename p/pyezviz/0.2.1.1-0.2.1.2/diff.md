# Comparing `tmp/pyezviz-0.2.1.1.tar.gz` & `tmp/pyezviz-0.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.1.tar", last modified: Sun Jun 18 10:03:01 2023, max compression
+gzip compressed data, was "pyezviz-0.2.1.2.tar", last modified: Sun Jun 18 17:17:33 2023, max compression
```

## Comparing `pyezviz-0.2.1.1.tar` & `pyezviz-0.2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:03:01.523026 pyezviz-0.2.1.1/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    53667 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 10:03:01.000000 pyezviz-0.2.1.1/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 10:03:01.527027 pyezviz-0.2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-18 10:02:51.000000 pyezviz-0.2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:33.994405 pyezviz-0.2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 17:17:33.990405 pyezviz-0.2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:33.990405 pyezviz-0.2.1.2/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53961 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:17:33.990405 pyezviz-0.2.1.2/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 17:17:33.000000 pyezviz-0.2.1.2/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:17:33.994405 pyezviz-0.2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-18 17:17:25.000000 pyezviz-0.2.1.2/setup.py
```

### Comparing `pyezviz-0.2.1.1/LICENSE.md` & `pyezviz-0.2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/README.md` & `pyezviz-0.2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/__init__.py` & `pyezviz-0.2.1.2/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/__main__.py` & `pyezviz-0.2.1.2/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/api_endpoints.py` & `pyezviz-0.2.1.2/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/camera.py` & `pyezviz-0.2.1.2/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/cas.py` & `pyezviz-0.2.1.2/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/client.py` & `pyezviz-0.2.1.2/pyezviz/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,14 +360,21 @@
                 "Impossible to decode response: "
                 + str(err)
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"].get("code") != 200:
+            if json_output["meta"].get("code") == 500:
+                _LOGGER.debug(
+                    "Retry getting alarm info, server returned busy: %s",
+                    json_output["meta"],
+                )
+                return self.get_alarminfo(serial, limit, max_retries + 1)
+
             raise PyEzvizError(
                 f"Could not get data from alarm api: Got {json_output['meta']})"
             )
 
         return json_output
 
     def get_device_messages_list(
```

### Comparing `pyezviz-0.2.1.1/pyezviz/constants.py` & `pyezviz-0.2.1.2/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/exceptions.py` & `pyezviz-0.2.1.2/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/mqtt.py` & `pyezviz-0.2.1.2/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.2/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/pyezviz/utils.py` & `pyezviz-0.2.1.2/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.1/setup.py` & `pyezviz-0.2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.1",
+    version="0.2.1.2",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

