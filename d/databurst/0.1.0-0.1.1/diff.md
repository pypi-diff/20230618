# Comparing `tmp/databurst-0.1.0.tar.gz` & `tmp/databurst-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databurst-0.1.0.tar", last modified: Sat Jun 17 22:19:22 2023, max compression
+gzip compressed data, was "databurst-0.1.1.tar", last modified: Sat Jun 17 22:37:38 2023, max compression
```

## Comparing `databurst-0.1.0.tar` & `databurst-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-17 22:19:22.827298 databurst-0.1.0/
--rw-r--r--   0 elias      (501) staff       (20)     1215 2023-06-17 22:19:22.827158 databurst-0.1.0/PKG-INFO
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-17 22:19:22.826899 databurst-0.1.0/databurst.egg-info/
--rw-r--r--   0 elias      (501) staff       (20)     1215 2023-06-17 22:19:22.000000 databurst-0.1.0/databurst.egg-info/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)      172 2023-06-17 22:19:22.000000 databurst-0.1.0/databurst.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (501) staff       (20)        1 2023-06-17 22:19:22.000000 databurst-0.1.0/databurst.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (501) staff       (20)        9 2023-06-17 22:19:22.000000 databurst-0.1.0/databurst.egg-info/requires.txt
--rw-r--r--   0 elias      (501) staff       (20)        1 2023-06-17 22:19:22.000000 databurst-0.1.0/databurst.egg-info/top_level.txt
--rw-r--r--   0 elias      (501) staff       (20)       38 2023-06-17 22:19:22.827347 databurst-0.1.0/setup.cfg
--rw-r--r--   0 elias      (501) staff       (20)     1379 2023-06-17 22:11:18.000000 databurst-0.1.0/setup.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-17 22:37:38.606147 databurst-0.1.1/
+-rw-r--r--   0 elias      (501) staff       (20)     1269 2023-06-17 22:37:38.605937 databurst-0.1.1/PKG-INFO
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-06-17 22:37:38.605572 databurst-0.1.1/databurst.egg-info/
+-rw-r--r--   0 elias      (501) staff       (20)     1269 2023-06-17 22:37:38.000000 databurst-0.1.1/databurst.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)      172 2023-06-17 22:37:38.000000 databurst-0.1.1/databurst.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-06-17 22:37:38.000000 databurst-0.1.1/databurst.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (501) staff       (20)       32 2023-06-17 22:37:38.000000 databurst-0.1.1/databurst.egg-info/requires.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-06-17 22:37:38.000000 databurst-0.1.1/databurst.egg-info/top_level.txt
+-rw-r--r--   0 elias      (501) staff       (20)       38 2023-06-17 22:37:38.606222 databurst-0.1.1/setup.cfg
+-rw-r--r--   0 elias      (501) staff       (20)     1477 2023-06-17 22:36:44.000000 databurst-0.1.1/setup.py
```

### Comparing `databurst-0.1.0/PKG-INFO` & `databurst-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: databurst
-Version: 0.1.0
+Version: 0.1.1
 Summary: Databurst is a Python package for generating random data such as names, addresses, phone numbers, and email addresses. It utilizes external APIs to retrieve realistic and randomized data for testing purposes.
 Home-page: https://github.com/Elias-mathisen/databurst
 Author: Elias Mathisen
+Author-email: elias-mathisen@hotmail.com
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `databurst-0.1.0/databurst.egg-info/PKG-INFO` & `databurst-0.1.1/databurst.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: databurst
-Version: 0.1.0
+Version: 0.1.1
 Summary: Databurst is a Python package for generating random data such as names, addresses, phone numbers, and email addresses. It utilizes external APIs to retrieve realistic and randomized data for testing purposes.
 Home-page: https://github.com/Elias-mathisen/databurst
 Author: Elias Mathisen
+Author-email: elias-mathisen@hotmail.com
+License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `databurst-0.1.0/setup.py` & `databurst-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='databurst',
-    version='0.1.0',
+    version='0.1.1',
     author='Elias Mathisen',
+    author_email='elias-mathisen@hotmail.com',
+    license='MIT',
     description='Databurst is a Python package for generating random data such as names, addresses, phone numbers, and email addresses. It utilizes external APIs to retrieve realistic and randomized data for testing purposes.',
     long_description='Databurst is a Python package that provides a simple and convenient way to generate random data for testing and development purposes. It includes functions to generate random names, addresses, phone numbers, and email addresses. The package leverages external APIs to fetch realistic and randomized data, ensuring the generated data is diverse and representative. Databurst is designed to be easy to use, making it ideal for generating sample data or populating test databases.',
     url='https://github.com/Elias-mathisen/databurst',
     packages=find_packages(),
-    install_requires=['requests'],
+    install_requires=['requests', 'random', 'string', 'datetime'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

