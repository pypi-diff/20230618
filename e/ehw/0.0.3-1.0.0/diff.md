# Comparing `tmp/ehw-0.0.3.tar.gz` & `tmp/ehw-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehw-0.0.3.tar", last modified: Thu Oct 13 06:07:59 2022, max compression
+gzip compressed data, was "ehw-1.0.0.tar", last modified: Sat Jun 17 22:49:07 2023, max compression
```

## Comparing `ehw-0.0.3.tar` & `ehw-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 06:07:59.297909 ehw-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-10-13 06:07:59.297909 ehw-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-13 06:07:41.000000 ehw-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 06:07:59.297909 ehw-0.0.3/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 06:07:59.297909 ehw-0.0.3/pkg/ehw/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-13 06:07:49.000000 ehw-0.0.3/pkg/ehw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-13 06:07:49.000000 ehw-0.0.3/pkg/ehw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-10-13 06:07:49.000000 ehw-0.0.3/pkg/ehw/ehw.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 06:07:59.297909 ehw-0.0.3/pkg/ehw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-10-13 06:07:59.000000 ehw-0.0.3/pkg/ehw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-10-13 06:07:59.000000 ehw-0.0.3/pkg/ehw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 06:07:59.000000 ehw-0.0.3/pkg/ehw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-13 06:07:59.000000 ehw-0.0.3/pkg/ehw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-13 06:07:59.000000 ehw-0.0.3/pkg/ehw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-13 06:07:59.000000 ehw-0.0.3/pkg/ehw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-13 06:07:49.000000 ehw-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-10-13 06:07:59.301909 ehw-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:49:07.278105 ehw-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-17 22:49:07.278105 ehw-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 22:48:51.000000 ehw-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:49:07.274105 ehw-1.0.0/exe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:49:07.274105 ehw-1.0.0/exe/ehw/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-17 22:48:59.000000 ehw-1.0.0/exe/ehw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-17 22:48:59.000000 ehw-1.0.0/exe/ehw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-17 22:48:59.000000 ehw-1.0.0/exe/ehw/ehw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:49:07.278105 ehw-1.0.0/exe/ehw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-17 22:49:07.000000 ehw-1.0.0/exe/ehw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-17 22:49:07.000000 ehw-1.0.0/exe/ehw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:49:07.000000 ehw-1.0.0/exe/ehw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 22:49:07.000000 ehw-1.0.0/exe/ehw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 22:49:07.000000 ehw-1.0.0/exe/ehw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-17 22:49:07.000000 ehw-1.0.0/exe/ehw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 22:48:59.000000 ehw-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-17 22:49:07.278105 ehw-1.0.0/setup.cfg
```

### Comparing `ehw-0.0.3/PKG-INFO` & `ehw-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehw
-Version: 0.0.3
+Version: 1.0.0
 Summary: eons hardware
 Home-page: https://github.com/eons-dev/bin_ehw
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_ehw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ehw-0.0.3/pkg/ehw.egg-info/PKG-INFO` & `ehw-1.0.0/exe/ehw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehw
-Version: 0.0.3
+Version: 1.0.0
 Summary: eons hardware
 Home-page: https://github.com/eons-dev/bin_ehw
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/bin_ehw/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ehw-0.0.3/setup.cfg` & `ehw-1.0.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ehw
-version = v0.0.3
+version = 1.0.0
 author = eons
 author_email = support@eons.llc
 description = eons hardware
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/bin_ehw
@@ -14,23 +14,22 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Development Status :: 3 - Alpha
 
 [options]
 package_dir = 
-	= pkg
+	= exe
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	eons
-	jsonpickle
+	requests
 
 [options.packages.find]
-where = pkg
+where = exe
 
 [options.entry_points]
 console_scripts = 
 	ehw = ehw:ehw
 
 [egg_info]
 tag_build =
```

