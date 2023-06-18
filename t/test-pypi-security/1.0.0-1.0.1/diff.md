# Comparing `tmp/test_pypi_security-1.0.0.tar.gz` & `tmp/test_pypi_security-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_pypi_security-1.0.0.tar", last modified: Sun Jun 18 18:11:05 2023, max compression
+gzip compressed data, was "test_pypi_security-1.0.1.tar", last modified: Sun Jun 18 18:13:38 2023, max compression
```

## Comparing `test_pypi_security-1.0.0.tar` & `test_pypi_security-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:11:05.970990 test_pypi_security-1.0.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:11:05.970990 test_pypi_security-1.0.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:03:09.000000 test_pypi_security-1.0.0/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:11:05.970990 test_pypi_security-1.0.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      700 2023-06-18 18:11:04.000000 test_pypi_security-1.0.0/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:11:05.970990 test_pypi_security-1.0.0/test_pypi_security.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:11:05.000000 test_pypi_security-1.0.0/test_pypi_security.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      231 2023-06-18 18:11:05.000000 test_pypi_security-1.0.0/test_pypi_security.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:11:05.000000 test_pypi_security-1.0.0/test_pypi_security.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        7 2023-06-18 18:11:05.000000 test_pypi_security-1.0.0/test_pypi_security.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:11:05.000000 test_pypi_security-1.0.0/test_pypi_security.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:13:38.700406 test_pypi_security-1.0.1/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:13:38.700406 test_pypi_security-1.0.1/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:03:09.000000 test_pypi_security-1.0.1/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:13:38.700406 test_pypi_security-1.0.1/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      683 2023-06-18 18:13:29.000000 test_pypi_security-1.0.1/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:13:38.700406 test_pypi_security-1.0.1/test_pypi_security.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:13:38.000000 test_pypi_security-1.0.1/test_pypi_security.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      190 2023-06-18 18:13:38.000000 test_pypi_security-1.0.1/test_pypi_security.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:13:38.000000 test_pypi_security-1.0.1/test_pypi_security.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:13:38.000000 test_pypi_security-1.0.1/test_pypi_security.egg-info/top_level.txt
```

### Comparing `test_pypi_security-1.0.0/PKG-INFO` & `test_pypi_security-1.0.1/test_pypi_security.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test_pypi_security
-Version: 1.0.0
+Name: test-pypi-security
+Version: 1.0.1
 Summary: Test of PyPI security
 Home-page: UNKNOWN
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `test_pypi_security-1.0.0/setup.py` & `test_pypi_security-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup
 
 setup(
     name='test_pypi_security',
-    version='1.0.0',
+    version='1.0.1',
     author='Arthur Le Floch',
     author_email='alf.github@gmail.com',
     description='Test of PyPI security',
     long_description='Test of PyPI security, do not use this package blindly, it deletes a folder called delete_me in the current directory',
     packages=[''],
     package_dir={'': '.'},
     install_requires=[
-        'pygame'
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `test_pypi_security-1.0.0/test_pypi_security.egg-info/PKG-INFO` & `test_pypi_security-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test-pypi-security
-Version: 1.0.0
+Name: test_pypi_security
+Version: 1.0.1
 Summary: Test of PyPI security
 Home-page: UNKNOWN
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

