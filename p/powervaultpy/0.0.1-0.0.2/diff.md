# Comparing `tmp/powervaultpy-0.0.1.tar.gz` & `tmp/powervaultpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powervaultpy-0.0.1.tar", last modified: Sat Jun 17 22:31:15 2023, max compression
+gzip compressed data, was "powervaultpy-0.0.2.tar", last modified: Sat Jun 17 23:07:48 2023, max compression
```

## Comparing `powervaultpy-0.0.1.tar` & `powervaultpy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 22:31:15.682004 powervaultpy-0.0.1/
--rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-17 22:31:15.681669 powervaultpy-0.0.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1432 2023-06-17 22:29:30.000000 powervaultpy-0.0.1/pyproject.toml
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-17 22:31:15.682163 powervaultpy-0.0.1/setup.cfg
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 22:31:15.677244 powervaultpy-0.0.1/src/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 22:31:15.678412 powervaultpy-0.0.1/src/powervaultpy/
--rw-r--r--   0 adam       (501) staff       (20)        0 2023-06-17 22:24:58.000000 powervaultpy-0.0.1/src/powervaultpy/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 22:31:15.681112 powervaultpy-0.0.1/src/powervaultpy.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-17 22:31:15.000000 powervaultpy-0.0.1/src/powervaultpy.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      242 2023-06-17 22:31:15.000000 powervaultpy-0.0.1/src/powervaultpy.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-17 22:31:15.000000 powervaultpy-0.0.1/src/powervaultpy.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)       68 2023-06-17 22:31:15.000000 powervaultpy-0.0.1/src/powervaultpy.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       13 2023-06-17 22:31:15.000000 powervaultpy-0.0.1/src/powervaultpy.egg-info/top_level.txt
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:07:48.293228 powervaultpy-0.0.2/
+-rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-17 23:07:48.292807 powervaultpy-0.0.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     1468 2023-06-17 23:07:38.000000 powervaultpy-0.0.2/pyproject.toml
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-17 23:07:48.293394 powervaultpy-0.0.2/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:07:48.286988 powervaultpy-0.0.2/src/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:07:48.288242 powervaultpy-0.0.2/src/powervaultpy/
+-rw-r--r--   0 adam       (501) staff       (20)       47 2023-06-17 23:03:23.000000 powervaultpy-0.0.2/src/powervaultpy/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     2917 2023-06-17 22:58:44.000000 powervaultpy-0.0.2/src/powervaultpy/powervault.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-17 23:07:48.291968 powervaultpy-0.0.2/src/powervaultpy.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      701 2023-06-17 23:07:48.000000 powervaultpy-0.0.2/src/powervaultpy.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      273 2023-06-17 23:07:48.000000 powervaultpy-0.0.2/src/powervaultpy.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-17 23:07:48.000000 powervaultpy-0.0.2/src/powervaultpy.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)       94 2023-06-17 23:07:48.000000 powervaultpy-0.0.2/src/powervaultpy.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       13 2023-06-17 23:07:48.000000 powervaultpy-0.0.2/src/powervaultpy.egg-info/top_level.txt
```

### Comparing `powervaultpy-0.0.1/PKG-INFO` & `powervaultpy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

### Comparing `powervaultpy-0.0.1/pyproject.toml` & `powervaultpy-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "powervaultpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Adam McDonagh", email="adam@elitemonkey.net" },
 ]
 license = { text = "GPLv3" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -23,14 +23,16 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
   "black >= 23.1.0",
   "isort",
   "pytest",
+  "pytest-env",
+  "pytest-asyncio",
   "bumpver",
   "pre-commit"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/adammcdonagh/powervaultpy"
 "Bug Tracker" = "https://github.com/adammcdonagh/powervaultpy/issues"
```

### Comparing `powervaultpy-0.0.1/src/powervaultpy.egg-info/PKG-INFO` & `powervaultpy-0.0.2/src/powervaultpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powervaultpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: An integration to control the Powervault battery
 Author-email: Adam McDonagh <adam@elitemonkey.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/adammcdonagh/powervaultpy
 Project-URL: Bug Tracker, https://github.com/adammcdonagh/powervaultpy/issues
 Project-URL: Changelog, https://github.com/adammcdonagh/powervaultpy/blob/main/CHANGELOG.md
 Keywords: powervault,home,automation
```

