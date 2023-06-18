# Comparing `tmp/flet_route-0.3.0.tar.gz` & `tmp/flet_route-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_route-0.3.0.tar", last modified: Sun Jun 18 15:29:25 2023, max compression
+gzip compressed data, was "flet_route-0.3.1.tar", last modified: Sun Jun 18 15:45:01 2023, max compression
```

## Comparing `flet_route-0.3.0.tar` & `flet_route-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.090535 flet_route-0.3.0/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-06-16 04:23:36.000000 flet_route-0.3.0/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1093 2023-06-18 15:29:25.090535 flet_route-0.3.0/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      642 2023-06-16 04:23:36.000000 flet_route-0.3.0/README.md
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.088535 flet_route-0.3.0/cli/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-16 05:00:09.000000 flet_route-0.3.0/cli/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2642 2023-06-18 15:00:26.000000 flet_route-0.3.0/cli/ac_class_contents.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2217 2023-06-18 14:43:18.000000 flet_route-0.3.0/cli/ac_func_contents.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2381 2023-06-18 14:11:32.000000 flet_route-0.3.0/cli/class_contents.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2181 2023-06-18 14:34:00.000000 flet_route-0.3.0/cli/cli.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2025 2023-06-18 14:50:39.000000 flet_route-0.3.0/cli/func_contents.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.089535 flet_route-0.3.0/flet_route/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      128 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      646 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/basket.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      854 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/not_found_view.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      716 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/params.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     6993 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/routing.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.090535 flet_route-0.3.0/flet_route.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1093 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      467 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       44 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/entry_points.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/requires.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       15 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/top_level.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2023-06-18 15:29:25.090535 flet_route-0.3.0/setup.cfg
--rw-r--r--   0 saurabh   (1000) saurabh   (1000)      936 2023-06-18 15:28:37.000000 flet_route-0.3.0/setup.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:45:01.311362 flet_route-0.3.1/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-06-16 04:23:36.000000 flet_route-0.3.1/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1285 2023-06-18 15:45:01.311362 flet_route-0.3.1/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      834 2023-06-18 15:43:54.000000 flet_route-0.3.1/README.md
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:45:01.309362 flet_route-0.3.1/cli/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-16 05:00:09.000000 flet_route-0.3.1/cli/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2642 2023-06-18 15:00:26.000000 flet_route-0.3.1/cli/ac_class_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2217 2023-06-18 14:43:18.000000 flet_route-0.3.1/cli/ac_func_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2381 2023-06-18 14:11:32.000000 flet_route-0.3.1/cli/class_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2181 2023-06-18 14:34:00.000000 flet_route-0.3.1/cli/cli.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2025 2023-06-18 14:50:39.000000 flet_route-0.3.1/cli/func_contents.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:45:01.310362 flet_route-0.3.1/flet_route/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      128 2023-06-16 04:23:36.000000 flet_route-0.3.1/flet_route/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      646 2023-06-16 04:23:36.000000 flet_route-0.3.1/flet_route/basket.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      854 2023-06-16 04:23:36.000000 flet_route-0.3.1/flet_route/not_found_view.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      716 2023-06-16 04:23:36.000000 flet_route-0.3.1/flet_route/params.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     6993 2023-06-16 04:23:36.000000 flet_route-0.3.1/flet_route/routing.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:45:01.311362 flet_route-0.3.1/flet_route.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1285 2023-06-18 15:45:01.000000 flet_route-0.3.1/flet_route.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      467 2023-06-18 15:45:01.000000 flet_route-0.3.1/flet_route.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2023-06-18 15:45:01.000000 flet_route-0.3.1/flet_route.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       44 2023-06-18 15:45:01.000000 flet_route-0.3.1/flet_route.egg-info/entry_points.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-18 15:45:01.000000 flet_route-0.3.1/flet_route.egg-info/requires.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       15 2023-06-18 15:45:01.000000 flet_route-0.3.1/flet_route.egg-info/top_level.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2023-06-18 15:45:01.311362 flet_route-0.3.1/setup.cfg
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      936 2023-06-18 15:44:13.000000 flet_route-0.3.1/setup.py
```

### Comparing `flet_route-0.3.0/LICENSE` & `flet_route-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/PKG-INFO` & `flet_route-0.3.1/flet_route.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 Metadata-Version: 2.1
-Name: flet_route
-Version: 0.3.0
+Name: flet-route
+Version: 0.3.1
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Build Status](flet-route.png)
 # This makes it easy to manage multiple views with dynamic routing.
+[![Downloads](https://static.pepy.tech/badge/flet-route)](https://pepy.tech/project/flet-route)
 
 This is an utility class based on repath library which allows matching ExpressJS-like routes and parsing their parameters, for example `/account/:account_id/orders/:order_id`.
 
 ## Installation
 ```
 pip install flet-route
 ```
 
 ## Upgradation
 ```
 pip install flet-route --upgrade
 ```
 
+## Create New App
+```
+flet-route init
+```
+### or
+```
+flet-route init --appname my_flet_app
+```
+
 #### [📖 Read the documentation ](https://saurabhwadekar.github.io/flet-route-doc)
 
 
 ## Author
 
 <b>Name :</b> Saurabh Wadekar<br>
 <b>Email :</b> saurabhwadekar420@gmail.com<br>
```

### Comparing `flet_route-0.3.0/cli/ac_class_contents.py` & `flet_route-0.3.1/cli/ac_class_contents.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/cli/ac_func_contents.py` & `flet_route-0.3.1/cli/ac_func_contents.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/cli/class_contents.py` & `flet_route-0.3.1/cli/class_contents.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/cli/cli.py` & `flet_route-0.3.1/cli/cli.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/cli/func_contents.py` & `flet_route-0.3.1/cli/func_contents.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/flet_route/basket.py` & `flet_route-0.3.1/flet_route/basket.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/flet_route/not_found_view.py` & `flet_route-0.3.1/flet_route/not_found_view.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/flet_route/params.py` & `flet_route-0.3.1/flet_route/params.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/flet_route/routing.py` & `flet_route-0.3.1/flet_route/routing.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.3.0/flet_route.egg-info/PKG-INFO` & `flet_route-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 Metadata-Version: 2.1
-Name: flet-route
-Version: 0.3.0
+Name: flet_route
+Version: 0.3.1
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Build Status](flet-route.png)
 # This makes it easy to manage multiple views with dynamic routing.
+[![Downloads](https://static.pepy.tech/badge/flet-route)](https://pepy.tech/project/flet-route)
 
 This is an utility class based on repath library which allows matching ExpressJS-like routes and parsing their parameters, for example `/account/:account_id/orders/:order_id`.
 
 ## Installation
 ```
 pip install flet-route
 ```
 
 ## Upgradation
 ```
 pip install flet-route --upgrade
 ```
 
+## Create New App
+```
+flet-route init
+```
+### or
+```
+flet-route init --appname my_flet_app
+```
+
 #### [📖 Read the documentation ](https://saurabhwadekar.github.io/flet-route-doc)
 
 
 ## Author
 
 <b>Name :</b> Saurabh Wadekar<br>
 <b>Email :</b> saurabhwadekar420@gmail.com<br>
```

### Comparing `flet_route-0.3.0/setup.py` & `flet_route-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = "flet_route",
-    version = "0.3.0",
+    version = "0.3.1",
     author="Saurabh Wadekar [ INDIA ]",
     packages=["flet_route","cli"],
     license="MIT",
     maintainer="Saurabh Wadekar",
     maintainer_email="saurabhwadekar420@gmail.com",
     keywords=["flet","routing","flet_route","routes","flet app","flet-route","flet simple routing"],
     description="This makes it easy to manage multiple views with dynamic routing.",
```

