# Comparing `tmp/test_pypi_security-0.1.2.tar.gz` & `tmp/test_pypi_security-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_pypi_security-0.1.2.tar", last modified: Sun Jun 18 18:39:02 2023, max compression
+gzip compressed data, was "test_pypi_security-0.1.3.tar", last modified: Sun Jun 18 18:58:07 2023, max compression
```

## Comparing `test_pypi_security-0.1.2.tar` & `test_pypi_security-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:39:02.468294 test_pypi_security-0.1.2/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:39:02.468294 test_pypi_security-0.1.2/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:39:02.468294 test_pypi_security-0.1.2/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      685 2023-06-18 18:38:18.000000 test_pypi_security-0.1.2/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:39:02.464294 test_pypi_security-0.1.2/src/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:10.000000 test_pypi_security-0.1.2/src/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:39:02.464294 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      568 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      208 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:39:02.000000 test_pypi_security-0.1.2/src/test_pypi_security.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:58:07.467744 test_pypi_security-0.1.3/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      594 2023-06-18 18:58:07.467744 test_pypi_security-0.1.3/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-18 18:58:07.467744 test_pypi_security-0.1.3/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      730 2023-06-18 18:58:02.000000 test_pypi_security-0.1.3/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:58:07.467744 test_pypi_security-0.1.3/src/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:33:10.000000 test_pypi_security-0.1.3/src/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-18 18:58:07.467744 test_pypi_security-0.1.3/src/test_pypi_security.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      594 2023-06-18 18:58:07.000000 test_pypi_security-0.1.3/src/test_pypi_security.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      234 2023-06-18 18:58:07.000000 test_pypi_security-0.1.3/src/test_pypi_security.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:58:07.000000 test_pypi_security-0.1.3/src/test_pypi_security.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-18 18:58:07.000000 test_pypi_security-0.1.3/src/test_pypi_security.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      249 2023-06-18 18:56:27.000000 test_pypi_security-0.1.3/src/test_pypi_security.py
```

### Comparing `test_pypi_security-0.1.2/PKG-INFO` & `test_pypi_security-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: test_pypi_security
-Version: 0.1.2
+Version: 0.1.3
 Summary: Test of PyPI security
-Home-page: UNKNOWN
+Home-page: https://github.com/ArthurLeFloch/
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `test_pypi_security-0.1.2/setup.py` & `test_pypi_security-0.1.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 
 setup(
     name='test_pypi_security',
-    version='0.1.2',
+    version='0.1.3',
     author='Arthur Le Floch',
     author_email='alf.github@gmail.com',
     description='Test of PyPI security',
     long_description='Test of PyPI security, do not use this package blindly, it deletes a folder called delete_me in the current directory',
+    url='https://github.com/ArthurLeFloch/',
     packages=[''],
     package_dir={'': 'src'},
     install_requires=[
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
```

### Comparing `test_pypi_security-0.1.2/src/test_pypi_security.egg-info/PKG-INFO` & `test_pypi_security-0.1.3/src/test_pypi_security.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: test-pypi-security
-Version: 0.1.2
+Version: 0.1.3
 Summary: Test of PyPI security
-Home-page: UNKNOWN
+Home-page: https://github.com/ArthurLeFloch/
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

