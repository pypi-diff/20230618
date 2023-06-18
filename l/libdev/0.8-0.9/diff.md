# Comparing `tmp/libdev-0.8.tar.gz` & `tmp/libdev-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libdev-0.8.tar", last modified: Thu Dec  9 14:03:44 2021, max compression
+gzip compressed data, was "dist/libdev-0.9.tar", last modified: Thu Dec  9 19:58:17 2021, max compression
```

## Comparing `libdev-0.8.tar` & `libdev-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kosyachniy   (502) wheel        (0)        0 2021-12-09 14:03:44.000000 libdev-0.8/
--rw-r--r--   0 kosyachniy   (502) wheel        (0)     1264 2021-12-09 14:03:44.000000 libdev-0.8/PKG-INFO
--rw-r--r--   0 kosyachniy   (502) wheel        (0)      339 2021-11-07 09:46:26.000000 libdev-0.8/README.md
-drwxr-xr-x   0 kosyachniy   (502) wheel        (0)        0 2021-12-09 14:03:44.000000 libdev-0.8/libdev/
--rw-r--r--   0 kosyachniy   (502) wheel        (0)       95 2021-12-09 14:03:37.000000 libdev-0.8/libdev/__init__.py
--rw-r--r--   0 kosyachniy   (502) wheel        (0)      383 2021-10-05 21:16:51.000000 libdev-0.8/libdev/cfg.py
--rw-r--r--   0 kosyachniy   (502) wheel        (0)      940 2021-11-18 13:39:10.000000 libdev-0.8/libdev/check.py
--rw-r--r--   0 kosyachniy   (502) wheel        (0)     1333 2021-12-05 20:41:38.000000 libdev-0.8/libdev/codes.py
--rw-r--r--   0 kosyachniy   (502) wheel        (0)     1038 2021-12-09 14:03:28.000000 libdev-0.8/libdev/gen.py
--rw-r--r--   0 kosyachniy   (502) wheel        (0)      307 2021-12-09 13:59:02.000000 libdev-0.8/libdev/lang.py
--rw-r--r--   0 kosyachniy   (502) wheel        (0)      174 2021-10-05 09:40:35.000000 libdev-0.8/libdev/time.py
-drwxr-xr-x   0 kosyachniy   (502) wheel        (0)        0 2021-12-09 14:03:44.000000 libdev-0.8/libdev.egg-info/
--rw-r--r--   0 kosyachniy   (502) wheel        (0)     1264 2021-12-09 14:03:44.000000 libdev-0.8/libdev.egg-info/PKG-INFO
--rw-r--r--   0 kosyachniy   (502) wheel        (0)      247 2021-12-09 14:03:44.000000 libdev-0.8/libdev.egg-info/SOURCES.txt
--rw-r--r--   0 kosyachniy   (502) wheel        (0)        1 2021-12-09 14:03:44.000000 libdev-0.8/libdev.egg-info/dependency_links.txt
--rw-r--r--   0 kosyachniy   (502) wheel        (0)        7 2021-12-09 14:03:44.000000 libdev-0.8/libdev.egg-info/top_level.txt
--rw-r--r--   0 kosyachniy   (502) wheel        (0)       38 2021-12-09 14:03:44.000000 libdev-0.8/setup.cfg
--rw-r--r--   0 kosyachniy   (502) wheel        (0)     1578 2021-10-05 21:17:31.000000 libdev-0.8/setup.py
+drwxr-xr-x   0 kosyachniy   (502) wheel        (0)        0 2021-12-09 19:58:17.000000 libdev-0.9/
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)     1264 2021-12-09 19:58:17.000000 libdev-0.9/PKG-INFO
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)      339 2021-11-07 09:46:26.000000 libdev-0.9/README.md
+drwxr-xr-x   0 kosyachniy   (502) wheel        (0)        0 2021-12-09 19:58:17.000000 libdev-0.9/libdev/
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)       95 2021-12-09 19:58:09.000000 libdev-0.9/libdev/__init__.py
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)      383 2021-10-05 21:16:51.000000 libdev-0.9/libdev/cfg.py
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)      940 2021-11-18 13:39:10.000000 libdev-0.9/libdev/check.py
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)     1333 2021-12-05 20:41:38.000000 libdev-0.9/libdev/codes.py
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)     1038 2021-12-09 14:03:28.000000 libdev-0.9/libdev/gen.py
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)      970 2021-12-09 19:57:55.000000 libdev-0.9/libdev/lang.py
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)      174 2021-10-05 09:40:35.000000 libdev-0.9/libdev/time.py
+drwxr-xr-x   0 kosyachniy   (502) wheel        (0)        0 2021-12-09 19:58:17.000000 libdev-0.9/libdev.egg-info/
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)     1264 2021-12-09 19:58:17.000000 libdev-0.9/libdev.egg-info/PKG-INFO
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)      247 2021-12-09 19:58:17.000000 libdev-0.9/libdev.egg-info/SOURCES.txt
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)        1 2021-12-09 19:58:17.000000 libdev-0.9/libdev.egg-info/dependency_links.txt
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)        7 2021-12-09 19:58:17.000000 libdev-0.9/libdev.egg-info/top_level.txt
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)       38 2021-12-09 19:58:17.000000 libdev-0.9/setup.cfg
+-rw-r--r--   0 kosyachniy   (502) wheel        (0)     1578 2021-10-05 21:17:31.000000 libdev-0.9/setup.py
```

### Comparing `libdev-0.8/PKG-INFO` & `libdev-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdev
-Version: 0.8
+Version: 0.9
 Summary: Set of standard functions for development
 Home-page: https://github.com/kosyachniy/lib
 Author: Alexey Poloz
 Author-email: polozhev@mail.ru
 License: MIT
 Project-URL: Source, https://github.com/kosyachniy/lib
 Description: # Dev lib [Libdev]
```

### Comparing `libdev-0.8/libdev/check.py` & `libdev-0.9/libdev/check.py`

 * *Files identical despite different names*

### Comparing `libdev-0.8/libdev/codes.py` & `libdev-0.9/libdev/codes.py`

 * *Files identical despite different names*

### Comparing `libdev-0.8/libdev/gen.py` & `libdev-0.9/libdev/gen.py`

 * *Files identical despite different names*

### Comparing `libdev-0.8/libdev.egg-info/PKG-INFO` & `libdev-0.9/libdev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdev
-Version: 0.8
+Version: 0.9
 Summary: Set of standard functions for development
 Home-page: https://github.com/kosyachniy/lib
 Author: Alexey Poloz
 Author-email: polozhev@mail.ru
 License: MIT
 Project-URL: Source, https://github.com/kosyachniy/lib
 Description: # Dev lib [Libdev]
```

### Comparing `libdev-0.8/setup.py` & `libdev-0.9/setup.py`

 * *Files identical despite different names*

