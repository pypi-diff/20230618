# Comparing `tmp/lacuscore-1.5.7.tar.gz` & `tmp/lacuscore-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.7.tar", max compression
+gzip compressed data, was "lacuscore-1.5.8.tar", max compression
```

## Comparing `lacuscore-1.5.7.tar` & `lacuscore-1.5.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.7/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.7/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.7/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.7/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    30864 2023-06-12 13:01:08.565874 lacuscore-1.5.7/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.7/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-15 16:21:38.611923 lacuscore-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.8/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.8/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.8/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.8/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    30814 2023-06-18 13:39:39.893648 lacuscore-1.5.8/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.8/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-18 13:42:16.542337 lacuscore-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.8/PKG-INFO
```

### Comparing `lacuscore-1.5.7/LICENSE` & `lacuscore-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.7/README.md` & `lacuscore-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.7/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.8/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.7/lacuscore/lacuscore.py` & `lacuscore-1.5.8/lacuscore/lacuscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,17 +334,17 @@
         p.hset(f'lacus:capture_settings:{perma_uuid}', mapping=mapping_capture)  # type: ignore
         p.zadd('lacus:to_capture', {perma_uuid: priority})
         p.execute()
         return perma_uuid
 
     def _encode_response(self, capture: CaptureResponse) -> CaptureResponseJson:
         encoded_capture = cast(CaptureResponseJson, capture)
-        if capture.get('png') and capture['png']:
+        if capture.get('png'):
             encoded_capture['png'] = b64encode(capture['png']).decode()
-        if capture.get('downloaded_file') and capture['downloaded_file']:
+        if capture.get('downloaded_file'):
             encoded_capture['downloaded_file'] = b64encode(capture['downloaded_file']).decode()
         if capture.get('children') and capture['children']:
             for child in capture['children']:
                 child = self._encode_response(child)
         return encoded_capture
 
     @overload
```

### Comparing `lacuscore-1.5.7/pyproject.toml` & `lacuscore-1.5.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.7"
+version = "1.5.8"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
```

### Comparing `lacuscore-1.5.7/PKG-INFO` & `lacuscore-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.7
+Version: 1.5.8
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

