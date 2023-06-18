# Comparing `tmp/random-otp-0.1.tar.gz` & `tmp/random-otp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\random-otp-0.1.tar", last modified: Sun Jun 18 10:50:37 2023, max compression
+gzip compressed data, was "dist\random-otp-0.1.1.tar", last modified: Sun Jun 18 11:00:57 2023, max compression
```

## Comparing `random-otp-0.1.tar` & `random-otp-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 10:50:37.000000 random-otp-0.1/
--rw-rw-rw-   0        0        0      384 2023-06-18 10:50:37.000000 random-otp-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-18 10:25:38.000000 random-otp-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 10:50:37.000000 random-otp-0.1/random_otp/
--rw-rw-rw-   0        0        0        0 2023-06-18 10:26:42.000000 random-otp-0.1/random_otp/__init__.py
--rw-rw-rw-   0        0        0     1329 2023-06-18 10:33:39.000000 random-otp-0.1/random_otp/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-18 10:50:37.000000 random-otp-0.1/random_otp.egg-info/
--rw-rw-rw-   0        0        0      384 2023-06-18 10:50:36.000000 random-otp-0.1/random_otp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-06-18 10:50:37.000000 random-otp-0.1/random_otp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 10:50:36.000000 random-otp-0.1/random_otp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-06-18 10:50:36.000000 random-otp-0.1/random_otp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-06-18 10:50:36.000000 random-otp-0.1/random_otp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 10:50:36.000000 random-otp-0.1/random_otp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 10:50:37.000000 random-otp-0.1/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-06-18 10:49:12.000000 random-otp-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 10:50:37.000000 random-otp-0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-18 10:26:42.000000 random-otp-0.1/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-18 10:27:27.000000 random-otp-0.1/tests/test_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:00:57.000000 random-otp-0.1.1/
+-rw-rw-rw-   0        0        0      386 2023-06-18 11:00:57.000000 random-otp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-06-18 10:59:09.000000 random-otp-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp/
+-rw-rw-rw-   0        0        0        0 2023-06-18 10:26:42.000000 random-otp-0.1.1/random_otp/__init__.py
+-rw-rw-rw-   0        0        0     1329 2023-06-18 10:33:39.000000 random-otp-0.1.1/random_otp/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-18 11:00:57.000000 random-otp-0.1.1/random_otp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 11:00:57.000000 random-otp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-06-18 11:00:26.000000 random-otp-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 11:00:57.000000 random-otp-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-18 10:26:42.000000 random-otp-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 10:27:27.000000 random-otp-0.1.1/tests/test_generator.py
```

### Comparing `random-otp-0.1/random_otp/generator.py` & `random-otp-0.1.1/random_otp/generator.py`

 * *Files identical despite different names*

### Comparing `random-otp-0.1/setup.py` & `random-otp-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='random-otp',
-    version='0.1',
+    version='0.1.1',
     author='Abhijith',
     author_email='abhis@tuta.io',
     description='A Python package for generating random OTPs',
     packages=find_packages(),
     install_requires=[
         'pycryptodome>=3.10.1',
     ],
```

