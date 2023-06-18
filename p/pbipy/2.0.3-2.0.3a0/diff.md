# Comparing `tmp/pbipy-2.0.3.tar.gz` & `tmp/pbipy-2.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.0.3.tar", last modified: Sun Jun 18 06:21:14 2023, max compression
+gzip compressed data, was "pbipy-2.0.3a0.tar", last modified: Sun Jun 18 05:31:15 2023, max compression
```

## Comparing `pbipy-2.0.3.tar` & `pbipy-2.0.3a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 06:21:14.441040 pbipy-2.0.3/
--rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     8989 2023-06-18 06:21:14.441040 pbipy-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     8205 2023-06-18 05:21:13.000000 pbipy-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 06:21:14.432424 pbipy-2.0.3/pbipy/
--rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.0.3/pbipy/__init__.py
--rw-rw-rw-   0        0        0      335 2023-06-18 06:20:09.000000 pbipy-2.0.3/pbipy/__version__.py
--rw-rw-rw-   0        0        0     4240 2023-06-18 05:21:13.000000 pbipy-2.0.3/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    20774 2023-06-18 05:21:13.000000 pbipy-2.0.3/pbipy/resources.py
--rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.0.3/pbipy/settings.py
--rw-rw-rw-   0        0        0    10220 2023-06-18 05:21:13.000000 pbipy-2.0.3/pbipy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:21:14.439036 pbipy-2.0.3/pbipy.egg-info/
--rw-rw-rw-   0        0        0     8989 2023-06-18 06:21:14.000000 pbipy-2.0.3/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-18 06:21:14.000000 pbipy-2.0.3/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 06:21:14.000000 pbipy-2.0.3/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-18 06:21:14.000000 pbipy-2.0.3/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 06:21:14.000000 pbipy-2.0.3/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 06:21:14.441040 pbipy-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.364409 pbipy-2.0.3a0/
+-rw-rw-rw-   0        0        0    11523 2022-10-28 08:16:15.000000 pbipy-2.0.3a0/LICENSE
+-rw-rw-rw-   0        0        0     8991 2023-06-18 05:31:15.363410 pbipy-2.0.3a0/PKG-INFO
+-rw-rw-rw-   0        0        0     8205 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.355410 pbipy-2.0.3a0/pbipy/
+-rw-rw-rw-   0        0        0       29 2022-10-28 07:52:32.000000 pbipy-2.0.3a0/pbipy/__init__.py
+-rw-rw-rw-   0        0        0      341 2023-06-18 05:25:30.000000 pbipy-2.0.3a0/pbipy/__version__.py
+-rw-rw-rw-   0        0        0     4240 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/powerbi.py
+-rw-rw-rw-   0        0        0    20774 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/resources.py
+-rw-rw-rw-   0        0        0      110 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/settings.py
+-rw-rw-rw-   0        0        0    10220 2023-06-18 05:21:13.000000 pbipy-2.0.3a0/pbipy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:31:15.362409 pbipy-2.0.3a0/pbipy.egg-info/
+-rw-rw-rw-   0        0        0     8991 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-18 05:31:15.000000 pbipy-2.0.3a0/pbipy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 05:31:15.364409 pbipy-2.0.3a0/setup.cfg
+-rw-rw-rw-   0        0        0     3594 2022-12-05 03:27:44.000000 pbipy-2.0.3a0/setup.py
```

### Comparing `pbipy-2.0.3/LICENSE` & `pbipy-2.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.0.3/PKG-INFO` & `pbipy-2.0.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.0.3
+Version: 2.0.3a0
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `pbipy-2.0.3/README.md` & `pbipy-2.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `pbipy-2.0.3/pbipy/powerbi.py` & `pbipy-2.0.3a0/pbipy/powerbi.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.0.3/pbipy/resources.py` & `pbipy-2.0.3a0/pbipy/resources.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.0.3/pbipy/utils.py` & `pbipy-2.0.3a0/pbipy/utils.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.0.3/pbipy.egg-info/PKG-INFO` & `pbipy-2.0.3a0/pbipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbipy
-Version: 2.0.3
+Version: 2.0.3a0
 Summary: A Python Library for interacting with the Power BI Rest API.
 Home-page: https://github.com/andrewvillazon/pbipy
 Author: Andrew Villazon
 Author-email: andrew.villazon@gmail.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `pbipy-2.0.3/setup.py` & `pbipy-2.0.3a0/setup.py`

 * *Files identical despite different names*

