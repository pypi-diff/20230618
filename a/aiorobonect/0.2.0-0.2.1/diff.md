# Comparing `tmp/aiorobonect-0.2.0.tar.gz` & `tmp/aiorobonect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-0.2.0.tar", last modified: Fri May 26 07:51:54 2023, max compression
+gzip compressed data, was "aiorobonect-0.2.1.tar", last modified: Sun Jun 18 11:58:15 2023, max compression
```

## Comparing `aiorobonect-0.2.0.tar` & `aiorobonect-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:51:54.279973 aiorobonect-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 07:51:54.279973 aiorobonect-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:51:54.275972 aiorobonect-0.2.0/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 07:51:27.000000 aiorobonect-0.2.0/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:51:54.275972 aiorobonect-0.2.0/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 07:51:54.000000 aiorobonect-0.2.0/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 07:51:54.279973 aiorobonect-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 07:51:30.000000 aiorobonect-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 11:57:50.000000 aiorobonect-0.2.1/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 11:58:15.000000 aiorobonect-0.2.1/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-18 11:58:15.431365 aiorobonect-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-18 11:57:53.000000 aiorobonect-0.2.1/setup.py
```

### Comparing `aiorobonect-0.2.0/LICENSE` & `aiorobonect-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.0/PKG-INFO` & `aiorobonect-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.0/README.md` & `aiorobonect-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-0.2.0/aiorobonect/client.py` & `aiorobonect-0.2.1/aiorobonect/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
         if command == "job":
             _LOGGER.debug(f"Job params: {params}")
             return
 
         self.session_start()
         try:
+            _LOGGER.debug(f"Calling http://{self.host}/json?cmd={command}&{params}")
             async with self.session.get(
                 f"http://{self.host}/json?cmd={command}&{params}"
             ) as response:
                 if response.status == 200:
                     result = await response.json(encoding="iso-8859-15")
                     _LOGGER.debug("Result mower data: %s", result)
                 if response.status >= 400:
@@ -106,43 +107,50 @@
         """Send command to mower."""
         self.session_start()
         result = await self.state()
         if result:
             result = {"status": result}
             if not self.sleeping or bypass_sleeping:
                 for cmd in commands:
-                    result.update({cmd: await self.async_cmd(cmd)})
+                    json_res = await self.async_cmd(cmd)
+                    if json_res:
+                        result.update({cmd: json_res})
             await self.session_close()
         return result
 
     async def state(self) -> dict:
         """Send status command to mower."""
         self.session_start()
         result = await self.async_cmd("status")
         if result:
             self.sleeping = result.get("status").get("status") == 17
             await self.session_close()
         return result
 
     async def async_start(self) -> bool:
         """Start the mower."""
-        return await self.async_cmd("start")
+        result = await self.async_cmd("start")
+        return result
 
     async def async_stop(self) -> bool:
         """Stop the mower."""
-        return await self.async_cmd("stop")
+        result = await self.async_cmd("stop")
+        return result
 
     async def async_reboot(self) -> bool:
         """Reboot Robonect."""
-        return await self.async_cmd("service", {"service": "reboot"})
+        result = await self.async_cmd("service", {"service": "reboot"})
+        return result
 
     async def async_shutdown(self) -> bool:
         """Shutdown Robonect."""
-        return await self.async_cmd("service", {"service": "shutdown"})
+        result = await self.async_cmd("service", {"service": "shutdown"})
+        return result
 
     async def async_sleep(self) -> bool:
         """Make Robonect sleep."""
-        return await self.async_cmd("service", {"service": "sleep"})
+        result = await self.async_cmd("service", {"service": "sleep"})
+        return result
 
     def sleeping(self) -> int:
         """Return if the mower is sleeping."""
         return self.sleeping
```

### Comparing `aiorobonect-0.2.0/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-0.2.1/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 0.2.0
+Version: 0.2.1
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-0.2.0/setup.py` & `aiorobonect-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v0.2.0",
+    version="v0.2.1",
 )
```

