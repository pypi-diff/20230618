# Comparing `tmp/tsclustering-1.0.1.tar.gz` & `tmp/tsclustering-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsclustering-1.0.1.tar", last modified: Sun Jun 18 19:54:36 2023, max compression
+gzip compressed data, was "tsclustering-1.0.2.tar", last modified: Sun Jun 18 20:01:00 2023, max compression
```

## Comparing `tsclustering-1.0.1.tar` & `tsclustering-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 19:54:36.719365 tsclustering-1.0.1/
--rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-13 14:54:38.000000 tsclustering-1.0.1/LICENSE
--rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-18 19:54:36.719746 tsclustering-1.0.1/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)     2390 2023-06-18 19:39:13.000000 tsclustering-1.0.1/README.md
--rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-18 19:54:36.721311 tsclustering-1.0.1/setup.cfg
--rw-r--r--   0 grant      (501) staff       (20)     1058 2023-06-18 19:54:33.000000 tsclustering-1.0.1/setup.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 19:54:36.713409 tsclustering-1.0.1/tsclustering/
--rw-r--r--   0 grant      (501) staff       (20)       38 2023-06-18 19:38:33.000000 tsclustering-1.0.1/tsclustering/__init__.py
--rw-r--r--   0 grant      (501) staff       (20)     2406 2023-06-13 14:54:38.000000 tsclustering-1.0.1/tsclustering/functions.py
--rw-r--r--   0 grant      (501) staff       (20)     4285 2023-06-13 14:54:38.000000 tsclustering-1.0.1/tsclustering/kmeans.py
-drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 19:54:36.718380 tsclustering-1.0.1/tsclustering.egg-info/
--rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-18 19:54:36.000000 tsclustering-1.0.1/tsclustering.egg-info/PKG-INFO
--rw-r--r--   0 grant      (501) staff       (20)      289 2023-06-18 19:54:36.000000 tsclustering-1.0.1/tsclustering.egg-info/SOURCES.txt
--rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-18 19:54:36.000000 tsclustering-1.0.1/tsclustering.egg-info/dependency_links.txt
--rw-r--r--   0 grant      (501) staff       (20)       20 2023-06-18 19:54:36.000000 tsclustering-1.0.1/tsclustering.egg-info/requires.txt
--rw-r--r--   0 grant      (501) staff       (20)       13 2023-06-18 19:54:36.000000 tsclustering-1.0.1/tsclustering.egg-info/top_level.txt
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 20:01:00.840526 tsclustering-1.0.2/
+-rw-r--r--   0 grant      (501) staff       (20)     1068 2023-06-13 14:54:38.000000 tsclustering-1.0.2/LICENSE
+-rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-18 20:01:00.840987 tsclustering-1.0.2/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)     2390 2023-06-18 19:39:13.000000 tsclustering-1.0.2/README.md
+-rw-r--r--   0 grant      (501) staff       (20)       79 2023-06-18 20:01:00.842609 tsclustering-1.0.2/setup.cfg
+-rw-r--r--   0 grant      (501) staff       (20)     1058 2023-06-18 20:00:54.000000 tsclustering-1.0.2/setup.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 20:01:00.832950 tsclustering-1.0.2/tsclustering/
+-rw-r--r--   0 grant      (501) staff       (20)       38 2023-06-18 19:38:33.000000 tsclustering-1.0.2/tsclustering/__init__.py
+-rw-r--r--   0 grant      (501) staff       (20)     2406 2023-06-13 14:54:38.000000 tsclustering-1.0.2/tsclustering/functions.py
+-rw-r--r--   0 grant      (501) staff       (20)     4285 2023-06-13 14:54:38.000000 tsclustering-1.0.2/tsclustering/kmeans.py
+drwxr-xr-x   0 grant      (501) staff       (20)        0 2023-06-18 20:01:00.839462 tsclustering-1.0.2/tsclustering.egg-info/
+-rw-r--r--   0 grant      (501) staff       (20)      934 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/PKG-INFO
+-rw-r--r--   0 grant      (501) staff       (20)      289 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/SOURCES.txt
+-rw-r--r--   0 grant      (501) staff       (20)        1 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/dependency_links.txt
+-rw-r--r--   0 grant      (501) staff       (20)       20 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/requires.txt
+-rw-r--r--   0 grant      (501) staff       (20)       13 2023-06-18 20:01:00.000000 tsclustering-1.0.2/tsclustering.egg-info/top_level.txt
```

### Comparing `tsclustering-1.0.1/LICENSE` & `tsclustering-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsclustering-1.0.1/PKG-INFO` & `tsclustering-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsclustering
-Version: 1.0.1
+Version: 1.0.2
 Summary: A clustering tool for timeseries data with temporal distortions.
 Home-page: https://github.com/gellison321/tsclustering
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.1.tar.gz
+Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.2.tar.gz
 Keywords: timeseries,barycenter,clustering,data science,data analysis,kmeans,time series clustering
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
```

### Comparing `tsclustering-1.0.1/README.md` & `tsclustering-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tsclustering-1.0.1/setup.py` & `tsclustering-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
   name = 'tsclustering',
   packages = find_packages(),
-  version = '1.0.1',
+  version = '1.0.2',
   license='',
   description = 'A clustering tool for timeseries data with temporal distortions.',
   author = 'Grant Ellison',
   author_email = 'gellison321@gmail.com',
   url = 'https://github.com/gellison321/tsclustering',
-  download_url = 'https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.1.tar.gz',
+  download_url = 'https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.2.tar.gz',
   keywords = ['timeseries', 'barycenter', 'clustering', 'data science','data analysis', 'kmeans', 'time series clustering'],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Topic :: Software Development :: Build Tools',
     'Operating System :: OS Independent',
```

### Comparing `tsclustering-1.0.1/tsclustering/functions.py` & `tsclustering-1.0.2/tsclustering/functions.py`

 * *Files identical despite different names*

### Comparing `tsclustering-1.0.1/tsclustering/kmeans.py` & `tsclustering-1.0.2/tsclustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `tsclustering-1.0.1/tsclustering.egg-info/PKG-INFO` & `tsclustering-1.0.2/tsclustering.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsclustering
-Version: 1.0.1
+Version: 1.0.2
 Summary: A clustering tool for timeseries data with temporal distortions.
 Home-page: https://github.com/gellison321/tsclustering
 Author: Grant Ellison
 Author-email: gellison321@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.1.tar.gz
+Download-URL: https://github.com/gellison321/tsclustering/archive/refs/tags/1.0.2.tar.gz
 Keywords: timeseries,barycenter,clustering,data science,data analysis,kmeans,time series clustering
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Operating System :: OS Independent
```

