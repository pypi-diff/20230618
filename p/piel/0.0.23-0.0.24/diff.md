# Comparing `tmp/piel-0.0.23.tar.gz` & `tmp/piel-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.23.tar", last modified: Sun Jun 18 13:13:12 2023, max compression
+gzip compressed data, was "piel-0.0.24.tar", last modified: Sun Jun 18 13:16:18 2023, max compression
```

## Comparing `piel-0.0.23.tar` & `piel-0.0.24.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-18 13:12:54.000000 piel-0.0.23/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-18 13:12:54.000000 piel-0.0.23/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 13:12:54.000000 piel-0.0.23/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 13:12:54.000000 piel-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 13:12:54.000000 piel-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:13:12.217463 piel-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-18 13:12:54.000000 piel-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-18 13:12:54.000000 piel-0.0.23/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:12:54.000000 piel-0.0.23/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/file_system/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/gdsfactory/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/openlane_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/openlane_v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/autoapi/piel/openlane_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/openlane_v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/docs/autoapi/piel/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/docs/autoapi/piel/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 13:12:54.000000 piel-0.0.23/docs/autoapi/piel/simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-18 13:12:54.000000 piel-0.0.23/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 13:12:54.000000 piel-0.0.23/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/examples/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/docs/examples/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 13:12:54.000000 piel-0.0.23/docs/examples/simple_design/tb/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:12:54.000000 piel-0.0.23/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-18 13:12:54.000000 piel-0.0.23/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 13:12:54.000000 piel-0.0.23/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 13:12:54.000000 piel-0.0.23/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.213463 piel-0.0.23/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 13:12:54.000000 piel-0.0.23/docs/sections/environment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 13:12:54.000000 piel-0.0.23/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 13:12:54.000000 piel-0.0.23/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 13:12:54.000000 piel-0.0.23/piel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-18 13:12:54.000000 piel-0.0.23/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 13:12:54.000000 piel-0.0.23/piel/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 13:12:54.000000 piel-0.0.23/piel/gdsfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-18 13:12:54.000000 piel-0.0.23/piel/openlane_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-18 13:12:54.000000 piel-0.0.23/piel/openlane_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-18 13:12:54.000000 piel-0.0.23/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 13:12:54.000000 piel-0.0.23/piel/piel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 13:12:54.000000 piel-0.0.23/piel/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 13:13:12.000000 piel-0.0.23/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:13:12.217463 piel-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:12:54.000000 piel-0.0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:13:12.217463 piel-0.0.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 13:12:54.000000 piel-0.0.23/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 13:12:54.000000 piel-0.0.23/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-18 13:16:03.000000 piel-0.0.24/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-18 13:16:03.000000 piel-0.0.24/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 13:16:03.000000 piel-0.0.24/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 13:16:03.000000 piel-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 13:16:03.000000 piel-0.0.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:16:18.735264 piel-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-18 13:16:03.000000 piel-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-18 13:16:03.000000 piel-0.0.24/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:16:03.000000 piel-0.0.24/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/file_system/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/gdsfactory/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/openlane_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/openlane_v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/openlane_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/openlane_v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-18 13:16:03.000000 piel-0.0.24/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 13:16:03.000000 piel-0.0.24/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.731264 piel-0.0.24/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.731264 piel-0.0.24/docs/examples/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/examples/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 13:16:03.000000 piel-0.0.24/docs/examples/simple_design/tb/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:16:03.000000 piel-0.0.24/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-18 13:16:03.000000 piel-0.0.24/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 13:16:03.000000 piel-0.0.24/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 13:16:03.000000 piel-0.0.24/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.731264 piel-0.0.24/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 13:16:03.000000 piel-0.0.24/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 13:16:03.000000 piel-0.0.24/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 13:16:03.000000 piel-0.0.24/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 13:16:03.000000 piel-0.0.24/piel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-18 13:16:03.000000 piel-0.0.24/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 13:16:03.000000 piel-0.0.24/piel/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 13:16:03.000000 piel-0.0.24/piel/gdsfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-18 13:16:03.000000 piel-0.0.24/piel/openlane_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-18 13:16:03.000000 piel-0.0.24/piel/openlane_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-18 13:16:03.000000 piel-0.0.24/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 13:16:03.000000 piel-0.0.24/piel/piel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 13:16:03.000000 piel-0.0.24/piel/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:16:18.735264 piel-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:16:03.000000 piel-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 13:16:03.000000 piel-0.0.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 13:16:03.000000 piel-0.0.24/tests/test_piel.py
```

### Comparing `piel-0.0.23/CONTRIBUTING.rst` & `piel-0.0.24/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/LICENSE` & `piel-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/PKG-INFO` & `piel-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.23
+Version: 0.0.24
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.23/README.md` & `piel-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/Makefile` & `piel-0.0.24/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.24/docs/autoapi/piel/file_system/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/autoapi/piel/index.rst` & `piel-0.0.24/docs/autoapi/piel/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.24/docs/autoapi/piel/parametric/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/autoapi/piel/simulation/index.rst` & `piel-0.0.24/docs/autoapi/piel/simulation/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/conf.py` & `piel-0.0.24/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/examples/simple_design/tb/Makefile` & `piel-0.0.24/docs/examples/simple_design/tb/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/docs/make.bat` & `piel-0.0.24/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel/defaults.py` & `piel-0.0.24/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel/file_system.py` & `piel-0.0.24/piel/file_system.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel/gdsfactory.py` & `piel-0.0.24/piel/gdsfactory.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel/openlane_v2.py` & `piel-0.0.24/piel/openlane_v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel/parametric.py` & `piel-0.0.24/piel/parametric.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel/simulation.py` & `piel-0.0.24/piel/simulation.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/piel.egg-info/PKG-INFO` & `piel-0.0.24/piel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.23
+Version: 0.0.24
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.23/piel.egg-info/SOURCES.txt` & `piel-0.0.24/piel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piel-0.0.23/setup.py` & `piel-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url='https://github.com/daquintero/piel',
-    version='0.0.23',
+    version='0.0.24',
     zip_safe=False,
 )
```

### Comparing `piel-0.0.23/tests/test_piel.py` & `piel-0.0.24/tests/test_piel.py`

 * *Files identical despite different names*

