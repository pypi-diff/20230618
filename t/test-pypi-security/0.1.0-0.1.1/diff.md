# Comparing `tmp/test_pypi_security-0.1.0.tar.gz` & `tmp/test_pypi_security-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_pypi_security-0.1.0.tar", last modified: Sun Jun 18 18:30:37 2023, max compression
+gzip compressed data, was "test_pypi_security-0.1.1.tar", last modified: Sun Jun 18 18:33:56 2023, max compression
```

## Comparing `test_pypi_security-0.1.0.tar` & `test_pypi_security-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:30:37.032332 test_pypi_security-0.1.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:30:37.032332 test_pypi_security-0.1.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:16:00.000000 test_pypi_security-0.1.0/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:30:37.032332 test_pypi_security-0.1.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      683 2023-06-18 18:30:29.000000 test_pypi_security-0.1.0/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:30:37.032332 test_pypi_security-0.1.0/test_pypi_security.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:30:37.000000 test_pypi_security-0.1.0/test_pypi_security.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      190 2023-06-18 18:30:37.000000 test_pypi_security-0.1.0/test_pypi_security.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:30:37.000000 test_pypi_security-0.1.0/test_pypi_security.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:30:37.000000 test_pypi_security-0.1.0/test_pypi_security.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:16:00.000000 test_pypi_security-0.1.1/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      683 2023-06-18 18:33:40.000000 test_pypi_security-0.1.1/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/test_pypi_security.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      190 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/top_level.txt
```

### Comparing `test_pypi_security-0.1.0/PKG-INFO` & `test_pypi_security-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_pypi_security
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test of PyPI security
 Home-page: UNKNOWN
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `test_pypi_security-0.1.0/setup.py` & `test_pypi_security-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='test_pypi_security',
-    version='0.1.0',
+    version='0.1.1',
     author='Arthur Le Floch',
     author_email='alf.github@gmail.com',
     description='Test of PyPI security',
     long_description='Test of PyPI security, do not use this package blindly, it deletes a folder called delete_me in the current directory',
     packages=[''],
     package_dir={'': '.'},
     install_requires=[
```

### Comparing `test_pypi_security-0.1.0/test_pypi_security.egg-info/PKG-INFO` & `test_pypi_security-0.1.1/test_pypi_security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pypi-security
-Version: 0.1.0
+Version: 0.1.1
 Summary: Test of PyPI security
 Home-page: UNKNOWN
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

