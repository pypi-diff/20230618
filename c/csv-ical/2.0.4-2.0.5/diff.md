# Comparing `tmp/csv-ical-2.0.4.tar.gz` & `tmp/csv-ical-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv-ical-2.0.4.tar", last modified: Thu Mar 17 06:57:03 2022, max compression
+gzip compressed data, was "csv-ical-2.0.5.tar", last modified: Sun Jun 18 05:34:51 2023, max compression
```

## Comparing `csv-ical-2.0.4.tar` & `csv-ical-2.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 06:57:03.165257 csv-ical-2.0.4/
--rw-r--r--   0 root         (0) root         (0)     1175 2022-03-17 06:56:37.000000 csv-ical-2.0.4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)       39 2022-03-17 06:56:37.000000 csv-ical-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1943 2022-03-17 06:57:03.165257 csv-ical-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1106 2022-03-17 06:56:37.000000 csv-ical-2.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 06:57:03.165257 csv-ical-2.0.4/csv_ical/
--rw-r--r--   0 root         (0) root         (0)       31 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/__version__.py
--rw-r--r--   0 root         (0) root         (0)     3867 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/convert.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 06:57:03.165257 csv-ical-2.0.4/csv_ical/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2796 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/tests/test_convert.py
--rw-r--r--   0 root         (0) root         (0)      163 2022-03-17 06:56:37.000000 csv-ical-2.0.4/csv_ical/tests/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 06:57:03.165257 csv-ical-2.0.4/csv_ical.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1943 2022-03-17 06:57:03.000000 csv-ical-2.0.4/csv_ical.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      374 2022-03-17 06:57:03.000000 csv-ical-2.0.4/csv_ical.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-17 06:57:03.000000 csv-ical-2.0.4/csv_ical.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-03-17 06:57:03.000000 csv-ical-2.0.4/csv_ical.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-03-17 06:57:03.000000 csv-ical-2.0.4/csv_ical.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-17 06:57:03.165257 csv-ical-2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1755 2022-03-17 06:56:37.000000 csv-ical-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 05:34:51.242524 csv-ical-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-06-18 05:34:35.000000 csv-ical-2.0.5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-18 05:34:35.000000 csv-ical-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-06-18 05:34:51.242524 csv-ical-2.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-06-18 05:34:35.000000 csv-ical-2.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 05:34:51.242524 csv-ical-2.0.5/csv_ical/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/convert.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 05:34:51.242524 csv-ical-2.0.5/csv_ical/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/tests/test_convert.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-18 05:34:35.000000 csv-ical-2.0.5/csv_ical/tests/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 05:34:51.242524 csv-ical-2.0.5/csv_ical.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-06-18 05:34:51.000000 csv-ical-2.0.5/csv_ical.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-18 05:34:51.000000 csv-ical-2.0.5/csv_ical.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 05:34:51.000000 csv-ical-2.0.5/csv_ical.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-18 05:34:51.000000 csv-ical-2.0.5/csv_ical.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-18 05:34:51.000000 csv-ical-2.0.5/csv_ical.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 05:34:51.242524 csv-ical-2.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-18 05:34:35.000000 csv-ical-2.0.5/setup.py
```

### Comparing `csv-ical-2.0.4/CHANGELOG.md` & `csv-ical-2.0.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+v2.0.5
+------
+
+ - Add support for python 3.11
+ - Dependency updates
+ - Updates to python publishing
+
+
 v2.0.4
 ------
 
  - Add full type annotations and add strict mypy typing
  - Switch README to markdown
```

### Comparing `csv-ical-2.0.4/PKG-INFO` & `csv-ical-2.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: csv-ical
-Version: 2.0.4
+Version: 2.0.5
 Summary: Convert between CSV and iCal
 Home-page: https://github.com/albertyw/csv-ical
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
 # CSV/iCal Converter
@@ -47,14 +47,12 @@
 
 See the example files.
 
 ## Development
 
 ```bash
 pip install -r requirements-test.txt
-flake8
+ruff check .
 mypy . --strict --ignore-missing-imports
 coverage run -m unittest
 coverage report -m
 ```
-
-
```

### Comparing `csv-ical-2.0.4/README.md` & `csv-ical-2.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 See the example files.
 
 ## Development
 
 ```bash
 pip install -r requirements-test.txt
-flake8
+ruff check .
 mypy . --strict --ignore-missing-imports
 coverage run -m unittest
 coverage report -m
 ```
```

### Comparing `csv-ical-2.0.4/csv_ical/convert.py` & `csv-ical-2.0.5/csv_ical/convert.py`

 * *Files identical despite different names*

### Comparing `csv-ical-2.0.4/csv_ical/tests/test_convert.py` & `csv-ical-2.0.5/csv_ical/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `csv-ical-2.0.4/csv_ical.egg-info/PKG-INFO` & `csv-ical-2.0.5/csv_ical.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: csv-ical
-Version: 2.0.4
+Version: 2.0.5
 Summary: Convert between CSV and iCal
 Home-page: https://github.com/albertyw/csv-ical
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 
 # CSV/iCal Converter
@@ -47,14 +47,12 @@
 
 See the example files.
 
 ## Development
 
 ```bash
 pip install -r requirements-test.txt
-flake8
+ruff check .
 mypy . --strict --ignore-missing-imports
 coverage run -m unittest
 coverage report -m
 ```
-
-
```

### Comparing `csv-ical-2.0.4/setup.py` & `csv-ical-2.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         'Typing :: Typed',
     ],
 
     keywords='',
 
     package_data={"csv_ical": ["py.typed"]},
@@ -58,14 +59,12 @@
     python_requires='>=3.5',
     install_requires=[
         'icalendar>=4.0.1,<5.0.0',
     ],
 
     test_suite="csv_ical.tests",
 
-    # testing requires flake8 and coverage but they're listed separately
-    # because they need to wrap setup.py
     extras_require={
         'dev': [],
         'test': [],
     },
 )
```

