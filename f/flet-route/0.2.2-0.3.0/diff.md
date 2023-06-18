# Comparing `tmp/flet_route-0.2.2.tar.gz` & `tmp/flet_route-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_route-0.2.2.tar", last modified: Sun Apr  9 10:39:55 2023, max compression
+gzip compressed data, was "flet_route-0.3.0.tar", last modified: Sun Jun 18 15:29:25 2023, max compression
```

## Comparing `flet_route-0.2.2.tar` & `flet_route-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 10:39:55.986899 flet_route-0.2.2/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1072 2023-03-09 16:43:16.000000 flet_route-0.2.2/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1125 2023-04-09 10:39:55.986899 flet_route-0.2.2/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      642 2023-04-09 10:39:43.000000 flet_route-0.2.2/README.md
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 10:39:55.985898 flet_route-0.2.2/flet_route/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      128 2023-04-02 00:50:24.000000 flet_route-0.2.2/flet_route/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      646 2023-04-02 01:06:15.000000 flet_route-0.2.2/flet_route/basket.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      405 2023-04-02 00:45:42.000000 flet_route-0.2.2/flet_route/not_found_view.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      716 2023-04-02 01:09:18.000000 flet_route-0.2.2/flet_route/params.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     4177 2023-04-06 16:28:44.000000 flet_route-0.2.2/flet_route/routing.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 10:39:55.986899 flet_route-0.2.2/flet_route.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1125 2023-04-09 10:39:55.000000 flet_route-0.2.2/flet_route.egg-info/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      278 2023-04-09 10:39:55.000000 flet_route-0.2.2/flet_route.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)        1 2023-04-09 10:39:55.000000 flet_route-0.2.2/flet_route.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       11 2023-04-09 10:39:55.000000 flet_route-0.2.2/flet_route.egg-info/top_level.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       38 2023-04-09 10:39:55.986899 flet_route-0.2.2/setup.cfg
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      753 2023-04-09 10:39:50.000000 flet_route-0.2.2/setup.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.090535 flet_route-0.3.0/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1072 2023-06-16 04:23:36.000000 flet_route-0.3.0/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1093 2023-06-18 15:29:25.090535 flet_route-0.3.0/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      642 2023-06-16 04:23:36.000000 flet_route-0.3.0/README.md
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.088535 flet_route-0.3.0/cli/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-16 05:00:09.000000 flet_route-0.3.0/cli/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2642 2023-06-18 15:00:26.000000 flet_route-0.3.0/cli/ac_class_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2217 2023-06-18 14:43:18.000000 flet_route-0.3.0/cli/ac_func_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2381 2023-06-18 14:11:32.000000 flet_route-0.3.0/cli/class_contents.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2181 2023-06-18 14:34:00.000000 flet_route-0.3.0/cli/cli.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2025 2023-06-18 14:50:39.000000 flet_route-0.3.0/cli/func_contents.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.089535 flet_route-0.3.0/flet_route/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      128 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      646 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/basket.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      854 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/not_found_view.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      716 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/params.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     6993 2023-06-16 04:23:36.000000 flet_route-0.3.0/flet_route/routing.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-06-18 15:29:25.090535 flet_route-0.3.0/flet_route.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     1093 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      467 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)        1 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       44 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/entry_points.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       25 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/requires.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       15 2023-06-18 15:29:25.000000 flet_route-0.3.0/flet_route.egg-info/top_level.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)       38 2023-06-18 15:29:25.090535 flet_route-0.3.0/setup.cfg
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)      936 2023-06-18 15:28:37.000000 flet_route-0.3.0/setup.py
```

### Comparing `flet_route-0.2.2/LICENSE` & `flet_route-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.2/PKG-INFO` & `flet_route-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: flet_route
-Version: 0.2.2
+Version: 0.3.0
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
-Requires: flet
-Requires: repath
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Build Status](flet-route.png)
 # This makes it easy to manage multiple views with dynamic routing.
 
 This is an utility class based on repath library which allows matching ExpressJS-like routes and parsing their parameters, for example `/account/:account_id/orders/:order_id`.
```

### Comparing `flet_route-0.2.2/README.md` & `flet_route-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.2/flet_route/basket.py` & `flet_route-0.3.0/flet_route/basket.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.2/flet_route/params.py` & `flet_route-0.3.0/flet_route/params.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.2/flet_route.egg-info/PKG-INFO` & `flet_route-0.3.0/flet_route.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: flet-route
-Version: 0.2.2
+Version: 0.3.0
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
-Requires: flet
-Requires: repath
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Build Status](flet-route.png)
 # This makes it easy to manage multiple views with dynamic routing.
 
 This is an utility class based on repath library which allows matching ExpressJS-like routes and parsing their parameters, for example `/account/:account_id/orders/:order_id`.
```

### Comparing `flet_route-0.2.2/setup.py` & `flet_route-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,20 +2,29 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = "flet_route",
-    version = "0.2.2",
+    version = "0.3.0",
     author="Saurabh Wadekar [ INDIA ]",
-    packages=["flet_route"],
+    packages=["flet_route","cli"],
     license="MIT",
-    requires=["flet","repath"],
     maintainer="Saurabh Wadekar",
     maintainer_email="saurabhwadekar420@gmail.com",
     keywords=["flet","routing","flet_route","routes","flet app","flet-route","flet simple routing"],
     description="This makes it easy to manage multiple views with dynamic routing.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url="https://github.com/saurabhwadekar/flet_route"   
+    url="https://github.com/saurabhwadekar/flet_route",
+    include_package_data=True,
+    install_requires=[
+        'click==8.1.3',
+        "repath",
+        "flet",
+    ],
+    entry_points= {
+        'console_scripts': 
+        ['flet-route=cli:make_app']
+    }, 
 )
```

