# Comparing `tmp/polar_diagrams-1.0.5.tar.gz` & `tmp/polar_diagrams-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_diagrams-1.0.5.tar", last modified: Sat Jun 17 17:04:07 2023, max compression
+gzip compressed data, was "polar_diagrams-1.0.7.tar", last modified: Sun Jun 18 08:00:25 2023, max compression
```

## Comparing `polar_diagrams-1.0.5.tar` & `polar_diagrams-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.353727 polar_diagrams-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-17 17:04:07.353727 polar_diagrams-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-17 17:04:07.353727 polar_diagrams-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/src/polar_diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/src/polar_diagrams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63198 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/src/polar_diagrams/polar_diagrams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:00:25.949009 polar_diagrams-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 08:00:12.000000 polar_diagrams-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-18 08:00:25.949009 polar_diagrams-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-18 08:00:12.000000 polar_diagrams-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-18 08:00:12.000000 polar_diagrams-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-18 08:00:25.949009 polar_diagrams-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:00:25.945009 polar_diagrams-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:00:25.945009 polar_diagrams-1.0.7/src/polar_diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-18 08:00:12.000000 polar_diagrams-1.0.7/src/polar_diagrams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63198 2023-06-18 08:00:12.000000 polar_diagrams-1.0.7/src/polar_diagrams/polar_diagrams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:00:25.949009 polar_diagrams-1.0.7/src/polar_diagrams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-18 08:00:25.000000 polar_diagrams-1.0.7/src/polar_diagrams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-18 08:00:25.000000 polar_diagrams-1.0.7/src/polar_diagrams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:00:25.000000 polar_diagrams-1.0.7/src/polar_diagrams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 08:00:25.000000 polar_diagrams-1.0.7/src/polar_diagrams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-18 08:00:25.000000 polar_diagrams-1.0.7/src/polar_diagrams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:00:25.949009 polar_diagrams-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-18 08:00:12.000000 polar_diagrams-1.0.7/tests/test.py
```

### Comparing `polar_diagrams-1.0.5/LICENSE` & `polar_diagrams-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `polar_diagrams-1.0.5/PKG-INFO` & `polar_diagrams-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polar_diagrams
-Version: 1.0.5
+Version: 1.0.7
 Summary: Interactive Polar Diagrams for Model Comparison
 Author: Aleksandar Anžel
 Author-email: aleksandar.anzel@uni-marburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `polar_diagrams-1.0.5/README.md` & `polar_diagrams-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `polar_diagrams-1.0.5/setup.cfg` & `polar_diagrams-1.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = polar_diagrams
-version = 1.0.5
+version = 1.0.7
 author = Aleksandar Anžel
 author_email = aleksandar.anzel@uni-marburg.de
 description = Interactive Polar Diagrams for Model Comparison
 long_description = file: README.md, LICENCE
 long_description_content_type = text/markdown
 Source = https://github.com/AAnzel/Polar-Diagrams-for-Model-Comparison
 Tracker = https://github.com/AAnzel/Polar-Diagrams-for-Model-Comparison/issues
```

### Comparing `polar_diagrams-1.0.5/src/polar_diagrams/__init__.py` & `polar_diagrams-1.0.7/src/polar_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `polar_diagrams-1.0.5/src/polar_diagrams/polar_diagrams.py` & `polar_diagrams-1.0.7/src/polar_diagrams/polar_diagrams.py`

 * *Files identical despite different names*

### Comparing `polar_diagrams-1.0.5/src/polar_diagrams.egg-info/PKG-INFO` & `polar_diagrams-1.0.7/src/polar_diagrams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polar-diagrams
-Version: 1.0.5
+Version: 1.0.7
 Summary: Interactive Polar Diagrams for Model Comparison
 Author: Aleksandar Anžel
 Author-email: aleksandar.anzel@uni-marburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `polar_diagrams-1.0.5/tests/test.py` & `polar_diagrams-1.0.7/tests/test.py`

 * *Files identical despite different names*

