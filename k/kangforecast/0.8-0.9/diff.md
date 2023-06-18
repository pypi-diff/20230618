# Comparing `tmp/kangforecast-0.8.tar.gz` & `tmp/kangforecast-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kangforecast-0.8.tar", last modified: Fri Jun 16 05:11:41 2023, max compression
+gzip compressed data, was "dist/kangforecast-0.9.tar", last modified: Fri Jun 16 05:40:42 2023, max compression
```

## Comparing `kangforecast-0.8.tar` & `kangforecast-0.9.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:11:41.000000 kangforecast-0.8/
--rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 05:11:41.000000 kangforecast-0.8/PKG-INFO
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      235 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)       13 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)      168 2023-06-16 05:09:46.000000 kangforecast-0.8/MANIFEST.in
--rw-r--r--   0 kang       (501) staff       (20)     6817 2023-06-16 04:56:21.000000 kangforecast-0.8/README.md
--rw-r--r--   0 kang       (501) staff       (20)      814 2023-06-16 05:06:49.000000 kangforecast-0.8/setup.py
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 05:11:41.000000 kangforecast-0.8/setup.cfg
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast/
--rw-r--r--   0 kang       (501) staff       (20)       25 2023-06-16 04:37:54.000000 kangforecast-0.8/kangforecast/__init__.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:11:41.000000 kangforecast-0.8/kangforecast/data/
--rw-r--r--   0 kang       (501) staff       (20)      123 2023-06-15 23:47:09.000000 kangforecast-0.8/kangforecast/data/special_dates.csv
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:40:42.081978 kangforecast-0.9/
+-rw-r--r--   0 kang       (501) staff       (20)      168 2023-06-16 05:09:46.000000 kangforecast-0.9/MANIFEST.in
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 05:40:42.081769 kangforecast-0.9/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     6817 2023-06-16 04:56:21.000000 kangforecast-0.9/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:40:42.080371 kangforecast-0.9/kangforecast/
+-rw-r--r--   0 kang       (501) staff       (20)       25 2023-06-16 04:37:54.000000 kangforecast-0.9/kangforecast/__init__.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:40:42.081118 kangforecast-0.9/kangforecast/__pycache__/
+-rw-r--r--   0 kang       (501) staff       (20)      191 2023-06-16 04:41:59.000000 kangforecast-0.9/kangforecast/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:40:42.081347 kangforecast-0.9/kangforecast/data/
+-rw-r--r--   0 kang       (501) staff       (20)      123 2023-06-15 23:47:09.000000 kangforecast-0.9/kangforecast/data/special_dates.csv
+-rw-r--r--   0 kang       (501) staff       (20)     1055 2023-06-16 05:38:27.000000 kangforecast-0.9/kangforecast/kangfn.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-16 05:40:42.081007 kangforecast-0.9/kangforecast.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)      642 2023-06-16 05:40:41.000000 kangforecast-0.9/kangforecast.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      342 2023-06-16 05:40:42.000000 kangforecast-0.9/kangforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-16 05:40:41.000000 kangforecast-0.9/kangforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)        8 2023-06-16 05:40:41.000000 kangforecast-0.9/kangforecast.egg-info/requires.txt
+-rw-r--r--   0 kang       (501) staff       (20)       13 2023-06-16 05:40:41.000000 kangforecast-0.9/kangforecast.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-16 05:40:42.082031 kangforecast-0.9/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      892 2023-06-16 05:40:22.000000 kangforecast-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kangforecast-0.8/PKG-INFO` & `kangforecast-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.8
+Version: 0.9
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kangforecast-0.8/kangforecast.egg-info/PKG-INFO` & `kangforecast-0.9/kangforecast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kangforecast
-Version: 0.8
+Version: 0.9
 Summary: A simple forecast package.
 Home-page: https://www.linkedin.com/in/xiaowenkang/
 Author: Xiaowen Kang
 Author-email: kangxiaowen@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `kangforecast-0.8/README.md` & `kangforecast-0.9/README.md`

 * *Files identical despite different names*

### Comparing `kangforecast-0.8/setup.py` & `kangforecast-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kangforecast',
-    version='0.8',
+    version='0.9',
     description='A simple forecast package.',
     author='Xiaowen Kang',
     author_email='kangxiaowen@gmail.com',
     url='https://www.linkedin.com/in/xiaowenkang/',  # replace with the url of your GitHub repo
     packages=find_packages(),
     package_data={'kangforecast': ['data/*.csv']},
     classifiers=[
@@ -15,8 +15,12 @@
         'License :: OSI Approved :: MIT License',  # choose a license
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    install_requires=[
+        'kanglib',
+        # other libraries...
+    ],
 )
```

