# Comparing `tmp/dal_python-0.2.6-cp39-none-any.whl.zip` & `tmp/dal_python-0.3.0-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 3080027 bytes, number of entries: 9
+Zip file size: 3082623 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      153 b- defN 23-Jun-18 03:15 dal/__init__.py
--rwxr-xr-x  2.0 unx  8192424 b- defN 23-Jun-18 03:37 dal/_dal.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  8192424 b- defN 23-Jun-18 04:38 dal/_dal.cpython-39-x86_64-linux-gnu.so
 -rw-r--r--  2.0 unx      355 b- defN 23-Jun-18 03:15 dal/api.py
--rw-r--r--  2.0 unx    62110 b- defN 23-Jun-18 03:37 dal/dal.py
--rw-r--r--  2.0 unx   724519 b- defN 23-Jun-18 03:37 dal/dal_wrap.cpp
--rw-r--r--  2.0 unx      799 b- defN 23-Jun-18 04:11 dal_python-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-18 04:11 dal_python-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-18 04:11 dal_python-0.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      688 b- defN 23-Jun-18 04:11 dal_python-0.2.6.dist-info/RECORD
-9 files, 8981155 bytes uncompressed, 3078861 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx    62110 b- defN 23-Jun-18 04:38 dal/dal.py
+-rw-r--r--  2.0 unx   724519 b- defN 23-Jun-18 04:38 dal/dal_wrap.cpp
+-rw-r--r--  2.0 unx      554 b- defN 23-Jun-18 04:36 dal/examples/001.european.py
+-rw-r--r--  2.0 unx     1399 b- defN 23-Jun-18 04:20 dal/examples/002.uoc.py
+-rw-r--r--  2.0 unx     2461 b- defN 23-Jun-18 04:20 dal/examples/003.snowball.py
+-rw-r--r--  2.0 unx      799 b- defN 23-Jun-18 04:38 dal_python-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-18 04:38 dal_python-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-18 04:38 dal_python-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      937 b- defN 23-Jun-18 04:38 dal_python-0.3.0.dist-info/RECORD
+12 files, 8985818 bytes uncompressed, 3081071 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,20 +9,29 @@
 
 Filename: dal/dal.py
 Comment: 
 
 Filename: dal/dal_wrap.cpp
 Comment: 
 
-Filename: dal_python-0.2.6.dist-info/METADATA
+Filename: dal/examples/001.european.py
 Comment: 
 
-Filename: dal_python-0.2.6.dist-info/WHEEL
+Filename: dal/examples/002.uoc.py
 Comment: 
 
-Filename: dal_python-0.2.6.dist-info/top_level.txt
+Filename: dal/examples/003.snowball.py
 Comment: 
 
-Filename: dal_python-0.2.6.dist-info/RECORD
+Filename: dal_python-0.3.0.dist-info/METADATA
+Comment: 
+
+Filename: dal_python-0.3.0.dist-info/WHEEL
+Comment: 
+
+Filename: dal_python-0.3.0.dist-info/top_level.txt
+Comment: 
+
+Filename: dal_python-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `dal_python-0.2.6.dist-info/METADATA` & `dal_python-0.3.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dal-python
-Version: 0.2.6
+Version: 0.3.0
 Summary: Python bindings for the DAL library
 Author: cheng li
 Author-email: wegamekinglc@hotmail.copm
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

