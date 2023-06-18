# Comparing `tmp/test_pypi_security-0.1.1.tar.gz` & `tmp/test_pypi_security-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_pypi_security-0.1.1.tar", last modified: Sun Jun 18 18:33:56 2023, max compression
+gzip compressed data, was "test_pypi_security-0.1.2.tar", last modified: Sun Jun 18 18:39:02 2023, max compression
```

## Comparing `test_pypi_security-0.1.1.tar` & `test_pypi_security-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:16:00.000000 test_pypi_security-0.1.1/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      683 2023-06-18 18:33:40.000000 test_pypi_security-0.1.1/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:56.592827 test_pypi_security-0.1.1/test_pypi_security.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      190 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:33:56.000000 test_pypi_security-0.1.1/test_pypi_security.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:39:02.468294 test_pypi_security-0.1.2/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:39:02.468294 test_pypi_security-0.1.2/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:39:02.468294 test_pypi_security-0.1.2/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      685 2023-06-18 18:38:18.000000 test_pypi_security-0.1.2/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:39:02.464294 test_pypi_security-0.1.2/src/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:10.000000 test_pypi_security-0.1.2/src/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:39:02.464294 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      208 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/top_level.txt
```

### Comparing `test_pypi_security-0.1.1/PKG-INFO` & `test_pypi_security-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_pypi_security
-Version: 0.1.1
+Version: 0.1.2
 Summary: Test of PyPI security
 Home-page: UNKNOWN
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `test_pypi_security-0.1.1/setup.py` & `test_pypi_security-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name='test_pypi_security',
-    version='0.1.1',
+    version='0.1.2',
     author='Arthur Le Floch',
     author_email='alf.github@gmail.com',
     description='Test of PyPI security',
     long_description='Test of PyPI security, do not use this package blindly, it deletes a folder called delete_me in the current directory',
     packages=[''],
-    package_dir={'': '.'},
+    package_dir={'': 'src'},
     install_requires=[
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `test_pypi_security-0.1.1/test_pypi_security.egg-info/PKG-INFO` & `test_pypi_security-0.1.2/src/test_pypi_security.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-pypi-security
-Version: 0.1.1
+Version: 0.1.2
 Summary: Test of PyPI security
 Home-page: UNKNOWN
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

