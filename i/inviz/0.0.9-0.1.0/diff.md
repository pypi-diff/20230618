# Comparing `tmp/inviz-0.0.9.tar.gz` & `tmp/inviz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.9.tar", last modified: Thu Jun 15 14:05:06 2023, max compression
+gzip compressed data, was "inviz-0.1.0.tar", last modified: Sun Jun 18 03:23:29 2023, max compression
```

## Comparing `inviz-0.0.9.tar` & `inviz-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 14:05:06.205949 inviz-0.0.9/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.0.9/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.0.9/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 14:05:06.205949 inviz-0.0.9/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1669 2023-06-12 23:22:44.000000 inviz-0.0.9/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 14:05:06.195949 inviz-0.0.9/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 14:05:06.205949 inviz-0.0.9/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       75 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)     8997 2023-06-15 13:55:49.000000 inviz-0.0.9/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-06-15 14:05:06.205949 inviz-0.0.9/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1090 2023-06-15 14:04:05.000000 inviz-0.0.9/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-18 03:23:29.022444 inviz-0.1.0/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.1.0/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.1.0/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-06-18 03:23:29.022444 inviz-0.1.0/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1643 2023-06-15 14:20:14.000000 inviz-0.1.0/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-18 03:23:29.022444 inviz-0.1.0/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-18 03:23:29.022444 inviz-0.1.0/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2165 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       89 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-06-18 03:23:28.000000 inviz-0.1.0/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)     6472 2023-06-18 03:02:43.000000 inviz-0.1.0/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-06-18 03:23:29.022444 inviz-0.1.0/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1100 2023-06-18 03:02:43.000000 inviz-0.1.0/setup.py
```

### Comparing `inviz-0.0.9/LICENSE` & `inviz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.9/PKG-INFO` & `inviz-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.9
-Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
+Version: 0.1.0
+Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,18 +34,17 @@
 - Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
 
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
-from inviz import *
-hv.extension('bokeh')
-pn.extension()
+import inviz as nv
 ```
 If no errors appear, all the dependencies were installed correctly and we're ready to start visualizing!
 
 ### Example
-Download and run the tutorial notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
+Download and run the `live_data_example` notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
 
 Here's an example of InViz in an astrophysics context! The parameters come from a specific dark matter model, and the observables are the matter power spectrum and CMB anisotropy power spectra.
+
 ![example output](images/example2.png)
```

### Comparing `inviz-0.0.9/README.md` & `inviz-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 - Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
 
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
-from inviz import *
-hv.extension('bokeh')
-pn.extension()
+import inviz as nv
 ```
 If no errors appear, all the dependencies were installed correctly and we're ready to start visualizing!
 
 ### Example
-Download and run the tutorial notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
+Download and run the `live_data_example` notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
 
 Here's an example of InViz in an astrophysics context! The parameters come from a specific dark matter model, and the observables are the matter power spectrum and CMB anisotropy power spectra.
+
 ![example output](images/example2.png)
```

### Comparing `inviz-0.0.9/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.1.0/inviz/inviz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.9
-Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
+Version: 0.1.0
+Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,18 +34,17 @@
 - Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
 
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
-from inviz import *
-hv.extension('bokeh')
-pn.extension()
+import inviz as nv
 ```
 If no errors appear, all the dependencies were installed correctly and we're ready to start visualizing!
 
 ### Example
-Download and run the tutorial notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
+Download and run the `live_data_example` notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
 
 Here's an example of InViz in an astrophysics context! The parameters come from a specific dark matter model, and the observables are the matter power spectrum and CMB anisotropy power spectra.
+
 ![example output](images/example2.png)
```

### Comparing `inviz-0.0.9/setup.py` & `inviz-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.9",
+    version = "0.1.0",
     author = "James Wen",
     author_email = "jswen@usc.edu",
-    description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
+    description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
     package_dir={'': 'inviz'},
 #    packages=['inviz'],
     #package_dir={'': 'inviz'},
@@ -22,12 +22,13 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.8',
     install_requires=["holoviews==1.15.4",
+                      "panel==0.14.4",
                       "spatialpandas==0.4.7",
                       "numpy>=1.20, <1.24",
                       "matplotlib==3.7.1"]
     )
```

