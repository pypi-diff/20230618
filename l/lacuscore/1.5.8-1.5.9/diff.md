# Comparing `tmp/lacuscore-1.5.8.tar.gz` & `tmp/lacuscore-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.5.8.tar", max compression
+gzip compressed data, was "lacuscore-1.5.9.tar", max compression
```

## Comparing `lacuscore-1.5.8.tar` & `lacuscore-1.5.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.8/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.8/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.8/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.8/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    30814 2023-06-18 13:39:39.893648 lacuscore-1.5.8/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.8/lacuscore/py.typed
--rw-r--r--   0        0        0     1596 2023-06-18 13:42:16.542337 lacuscore-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.5.9/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.5.9/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.5.9/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.5.9/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    30838 2023-06-18 13:51:13.388781 lacuscore-1.5.9/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.5.9/lacuscore/py.typed
+-rw-r--r--   0        0        0     1596 2023-06-18 13:51:46.400929 lacuscore-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 lacuscore-1.5.9/PKG-INFO
```

### Comparing `lacuscore-1.5.8/LICENSE` & `lacuscore-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.8/README.md` & `lacuscore-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.8/lacuscore/lacus_monitoring.py` & `lacuscore-1.5.9/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.5.8/lacuscore/lacuscore.py` & `lacuscore-1.5.9/lacuscore/lacuscore.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,17 +334,17 @@
         p.hset(f'lacus:capture_settings:{perma_uuid}', mapping=mapping_capture)  # type: ignore
         p.zadd('lacus:to_capture', {perma_uuid: priority})
         p.execute()
         return perma_uuid
 
     def _encode_response(self, capture: CaptureResponse) -> CaptureResponseJson:
         encoded_capture = cast(CaptureResponseJson, capture)
-        if capture.get('png'):
+        if capture.get('png') is not None:
             encoded_capture['png'] = b64encode(capture['png']).decode()
-        if capture.get('downloaded_file'):
+        if capture.get('downloaded_file') is not None:
             encoded_capture['downloaded_file'] = b64encode(capture['downloaded_file']).decode()
         if capture.get('children') and capture['children']:
             for child in capture['children']:
                 child = self._encode_response(child)
         return encoded_capture
 
     @overload
```

### Comparing `lacuscore-1.5.8/pyproject.toml` & `lacuscore-1.5.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.5.8"
+version = "1.5.9"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
```

### Comparing `lacuscore-1.5.8/PKG-INFO` & `lacuscore-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.5.8
+Version: 1.5.9
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

