# Comparing `tmp/piel-0.0.24.tar.gz` & `tmp/piel-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piel-0.0.24.tar", last modified: Sun Jun 18 13:16:18 2023, max compression
+gzip compressed data, was "piel-0.0.25.tar", last modified: Sun Jun 18 13:59:18 2023, max compression
```

## Comparing `piel-0.0.24.tar` & `piel-0.0.25.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-18 13:16:03.000000 piel-0.0.24/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-18 13:16:03.000000 piel-0.0.24/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 13:16:03.000000 piel-0.0.24/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 13:16:03.000000 piel-0.0.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 13:16:03.000000 piel-0.0.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:16:18.735264 piel-0.0.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-18 13:16:03.000000 piel-0.0.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-18 13:16:03.000000 piel-0.0.24/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:16:03.000000 piel-0.0.24/docs/authors.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/cli/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/defaults/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/file_system/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/gdsfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/gdsfactory/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/openlane_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/openlane_v1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/openlane_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/openlane_v2/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/parametric/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/parametric/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/piel/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/autoapi/piel/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 13:16:03.000000 piel-0.0.24/docs/autoapi/piel/simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-18 13:16:03.000000 piel-0.0.24/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 13:16:03.000000 piel-0.0.24/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.731264 piel-0.0.24/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.731264 piel-0.0.24/docs/examples/simple_design/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/examples/simple_design/tb/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 13:16:03.000000 piel-0.0.24/docs/examples/simple_design/tb/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:16:03.000000 piel-0.0.24/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-18 13:16:03.000000 piel-0.0.24/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 13:16:03.000000 piel-0.0.24/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 13:16:03.000000 piel-0.0.24/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.731264 piel-0.0.24/docs/sections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/docs/sections/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 13:16:03.000000 piel-0.0.24/docs/sections/environment/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 13:16:03.000000 piel-0.0.24/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/piel/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-18 13:16:03.000000 piel-0.0.24/piel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 13:16:03.000000 piel-0.0.24/piel/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-18 13:16:03.000000 piel-0.0.24/piel/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-18 13:16:03.000000 piel-0.0.24/piel/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 13:16:03.000000 piel-0.0.24/piel/gdsfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-18 13:16:03.000000 piel-0.0.24/piel/openlane_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-18 13:16:03.000000 piel-0.0.24/piel/openlane_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-18 13:16:03.000000 piel-0.0.24/piel/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 13:16:03.000000 piel-0.0.24/piel/piel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 13:16:03.000000 piel-0.0.24/piel/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/piel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 13:16:18.000000 piel-0.0.24/piel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:16:18.735264 piel-0.0.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:16:03.000000 piel-0.0.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:16:18.735264 piel-0.0.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 13:16:03.000000 piel-0.0.24/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 13:16:03.000000 piel-0.0.24/tests/test_piel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.652661 piel-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-18 13:59:03.000000 piel-0.0.25/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-18 13:59:03.000000 piel-0.0.25/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-18 13:59:03.000000 piel-0.0.25/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 13:59:03.000000 piel-0.0.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-18 13:59:03.000000 piel-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:59:18.652661 piel-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-18 13:59:03.000000 piel-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-18 13:59:03.000000 piel-0.0.25/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:59:03.000000 piel-0.0.25/docs/authors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/cli/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/defaults/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/file_system/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/gdsfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/gdsfactory/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/openlane_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/openlane_v1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/openlane_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/openlane_v2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/parametric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/parametric/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/piel/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/autoapi/piel/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 13:59:03.000000 piel-0.0.25/docs/autoapi/piel/simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-18 13:59:03.000000 piel-0.0.25/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-18 13:59:03.000000 piel-0.0.25/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.644661 piel-0.0.25/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.644661 piel-0.0.25/docs/examples/simple_design/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/examples/simple_design/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 13:59:03.000000 piel-0.0.25/docs/examples/simple_design/tb/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 13:59:03.000000 piel-0.0.25/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 13:59:03.000000 piel-0.0.25/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-18 13:59:03.000000 piel-0.0.25/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-18 13:59:03.000000 piel-0.0.25/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-18 13:59:03.000000 piel-0.0.25/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.644661 piel-0.0.25/docs/sections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/docs/sections/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-18 13:59:03.000000 piel-0.0.25/docs/sections/environment/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-18 13:59:03.000000 piel-0.0.25/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.648661 piel-0.0.25/piel/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-18 13:59:03.000000 piel-0.0.25/piel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-18 13:59:03.000000 piel-0.0.25/piel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-18 13:59:03.000000 piel-0.0.25/piel/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-18 13:59:03.000000 piel-0.0.25/piel/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-18 13:59:03.000000 piel-0.0.25/piel/gdsfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-18 13:59:03.000000 piel-0.0.25/piel/openlane_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-18 13:59:03.000000 piel-0.0.25/piel/openlane_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 13:59:03.000000 piel-0.0.25/piel/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 13:59:03.000000 piel-0.0.25/piel/piel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 13:59:03.000000 piel-0.0.25/piel/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.652661 piel-0.0.25/piel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 13:59:18.000000 piel-0.0.25/piel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:59:18.652661 piel-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-18 13:59:03.000000 piel-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:59:18.652661 piel-0.0.25/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-18 13:59:03.000000 piel-0.0.25/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 13:59:03.000000 piel-0.0.25/tests/test_piel.py
```

### Comparing `piel-0.0.24/CONTRIBUTING.rst` & `piel-0.0.25/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/LICENSE` & `piel-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/PKG-INFO` & `piel-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.24
+Version: 0.0.25
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.24/README.md` & `piel-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/docs/Makefile` & `piel-0.0.25/docs/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/docs/autoapi/piel/file_system/index.rst` & `piel-0.0.25/docs/autoapi/piel/file_system/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -18,15 +18,15 @@
    piel.file_system.check_example_design
 
 
 
 .. py:function:: copy_source_folder(source_directory: str, target_directory: str)
 
 
-.. py:function:: setup_example_design(example_name: str = 'simple_design')
+.. py:function:: setup_example_design(project_source: Literal[piel, openlane] = 'piel', example_name: str = 'simple_design')
 
    We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
 
 
 .. py:function:: check_example_design(example_name: str = 'simple_design')
 
    We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
```

### Comparing `piel-0.0.24/docs/autoapi/piel/index.rst` & `piel-0.0.25/docs/autoapi/piel/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 .. autoapisummary::
 
    piel.copy_source_folder
    piel.setup_example_design
    piel.check_example_design
    piel.write_openlane_configuration
-   piel.run_openlane
+   piel.run_openlane_flow
    piel.single_parameter_sweep
    piel.multi_parameter_sweep
    piel.configure_cocotb_simulation
    piel.run_cocotb_simulation
 
 
 
@@ -68,55 +68,65 @@
 
 .. py:data:: __email__
    :value: 'darioaquintero@gmail.com'
 
    
 
 .. py:data:: __version__
-   :value: '0.0.20'
+   :value: '0.0.24'
 
    
 
 .. py:data:: test_spm_open_lane_configuration
 
    
 
 .. py:data:: example_open_lane_configuration
 
    
 
 .. py:function:: copy_source_folder(source_directory: str, target_directory: str)
 
 
-.. py:function:: setup_example_design(example_name: str = 'simple_design')
+.. py:function:: setup_example_design(project_source: Literal[piel, openlane] = 'piel', example_name: str = 'simple_design')
 
    We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
 
 
 .. py:function:: check_example_design(example_name: str = 'simple_design')
 
    We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
 
 
 .. py:function:: write_openlane_configuration(project_directory=None, configuration=dict())
 
 
-.. py:function:: run_openlane(design_directory: str = '.', configuration: dict = test_spm_open_lane_configuration)
+.. py:function:: run_openlane_flow(configuration: dict | None = test_spm_open_lane_configuration, design_directory: str = '/foss/designs/spm') -> None
+
+   Runs the OpenLane flow.
+
+   :param configuration: OpenLane configuration dictionary. If none is present it will default to the config.json file on the design_directory.
+   :type configuration: dict
+   :param design_directory: Design directory PATH.
+   :type design_directory: str
+
+   :returns: None
 
 
 .. py:function:: single_parameter_sweep(base_design_configuration: dict, parameter_name: str, parameter_sweep_values: list)
 
 
 .. py:function:: multi_parameter_sweep(base_design_configuration: dict, parameter_sweep_dictionary: dict)
 
-   This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping parameter_1 = np.arange(0, 2) = array([0, 1]), and parameter_2 = np.arange(2, 4) = array([2, 3]), then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
+   This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping `parameter_1 = np.arange(0, 2) = array([0, 1])`, and `parameter_2 = np.arange(2, 4) = array([2, 3])`, then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
 
    For the example above, there arould be 4 combinations [(0, 2), (0, 3), (1, 2), (1, 3)].
 
-   If you were instead sweeping for parameter_1 = np.arange(0, 5) and parameter_2 = np.arange(0, 5), the dictionary generated would correspond to these parameter combinations of [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
+   If you were instead sweeping for `parameter_1 = np.arange(0, 5)` and `parameter_2 = np.arange(0, 5)`, the dictionary generated would correspond to these parameter combinations of::
+       [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
 
    Make sure to use the parameter_names from default_design when writing up the parameter_sweep dictionary key name.
 
    Example project_structure formats::
 
        example_parameter_sweep_dictionary = {
            "parameter_1": np.arange(1, -40, 1),
```

### Comparing `piel-0.0.24/docs/autoapi/piel/parametric/index.rst` & `piel-0.0.25/docs/autoapi/piel/parametric/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 
 
 .. py:function:: single_parameter_sweep(base_design_configuration: dict, parameter_name: str, parameter_sweep_values: list)
 
 
 .. py:function:: multi_parameter_sweep(base_design_configuration: dict, parameter_sweep_dictionary: dict)
 
-   This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping parameter_1 = np.arange(0, 2) = array([0, 1]), and parameter_2 = np.arange(2, 4) = array([2, 3]), then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
+   This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping `parameter_1 = np.arange(0, 2) = array([0, 1])`, and `parameter_2 = np.arange(2, 4) = array([2, 3])`, then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
 
    For the example above, there arould be 4 combinations [(0, 2), (0, 3), (1, 2), (1, 3)].
 
-   If you were instead sweeping for parameter_1 = np.arange(0, 5) and parameter_2 = np.arange(0, 5), the dictionary generated would correspond to these parameter combinations of [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
+   If you were instead sweeping for `parameter_1 = np.arange(0, 5)` and `parameter_2 = np.arange(0, 5)`, the dictionary generated would correspond to these parameter combinations of::
+       [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
 
    Make sure to use the parameter_names from default_design when writing up the parameter_sweep dictionary key name.
 
    Example project_structure formats::
 
        example_parameter_sweep_dictionary = {
            "parameter_1": np.arange(1, -40, 1),
```

### Comparing `piel-0.0.24/docs/autoapi/piel/simulation/index.rst` & `piel-0.0.25/docs/autoapi/piel/simulation/index.rst`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/docs/conf.py` & `piel-0.0.25/docs/conf.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/docs/examples/simple_design/tb/Makefile` & `piel-0.0.25/docs/examples/simple_design/tb/Makefile`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/docs/make.bat` & `piel-0.0.25/docs/make.bat`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/piel/defaults.py` & `piel-0.0.25/piel/defaults.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/piel/file_system.py` & `piel-0.0.25/piel/file_system.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 import os
 import shutil
 import pathlib
 import openlane
 from typing import Literal
 
+
 def copy_source_folder(source_directory: str, target_directory: str):
     if os.path.exists(target_directory):
         answer = input("Confirm deletion of: " + target_directory)
         if answer.upper() in ["Y", "YES"]:
             shutil.rmtree(target_directory)
-        elif answer.upper() in["N", "NO"]:
-            print("Copying files now from: " + source_directory + " to " + target_directory)
+        elif answer.upper() in ["N", "NO"]:
+            print(
+                "Copying files now from: "
+                + source_directory
+                + " to "
+                + target_directory
+            )
 
     shutil.copytree(
         source_directory,
         target_directory,
         symlinks=False,
         ignore=None,
         copy_function=shutil.copy2,
         ignore_dangling_symlinks=False,
         dirs_exist_ok=False,
     )
 
 
 def setup_example_design(
     project_source: Literal["piel", "openlane"] = "piel",
-    example_name:str="simple_design"
+    example_name: str = "simple_design",
 ):
     """
     We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
     """
     if project_source == "piel":
-        example_design_folder = os.environ["PIEL_PACKAGE_DIRECTORY"] + "/docs/examples/" + example_name
+        example_design_folder = (
+            os.environ["PIEL_PACKAGE_DIRECTORY"] + "/docs/examples/" + example_name
+        )
     elif project_source == "openlane":
-        example_design_folder = pathlib.Path(openlane.__file__).parent.resolve() / example_name
+        example_design_folder = (
+            pathlib.Path(openlane.__file__).parent.resolve() / example_name
+        )
     design_folder = os.environ["DESIGNS"] + "/" + example_name
     copy_source_folder(
-        source_directory=example_design_folder,
-        target_directory=design_folder
+        source_directory=example_design_folder, target_directory=design_folder
     )
 
-def check_example_design(
-    example_name:str="simple_design"
-):
+
+def check_example_design(example_name: str = "simple_design"):
     """
     We copy the example simple_design from docs to the `/foss/designs` in the `iic-osic-tools` environment.
     """
-    design_folder = os.environ["DESIGNS"] + "/" + example_name # TODO verify this copying operation
+    design_folder = (
+        os.environ["DESIGNS"] + "/" + example_name
+    )  # TODO verify this copying operation
     return os.path.exists(design_folder)
 
-__all__ = [
-    "copy_source_folder",
-    "setup_example_design",
-    "check_example_design"
-]
+
+__all__ = ["copy_source_folder", "setup_example_design", "check_example_design"]
```

### Comparing `piel-0.0.24/piel/gdsfactory.py` & `piel-0.0.25/piel/gdsfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 * SKY130nm https://gdsfactory.github.io/skywater130/
 * GF180nm https://gdsfactory.github.io/gf180/
 
 """
 
 import gdsfactory as gf
 
+
 def create_gdsfactory_component(
-    design_directory:str,
+    design_directory: str,
 ) -> gf.Component:
     """
     This function cretes a gdsfactory component that can be included in the network codesign of the device, or that can be used for interconnection codesign.
     """
     pass
-
-
```

### Comparing `piel-0.0.24/piel/openlane_v2.py` & `piel-0.0.25/piel/openlane_v2.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/piel/parametric.py` & `piel-0.0.25/piel/parametric.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     return parameter_sweep_design_dictionary_array
 
 
 def multi_parameter_sweep(
     base_design_configuration: dict, parameter_sweep_dictionary: dict
 ):
     """
-    This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping parameter_1 = np.arange(0, 2) = array([0, 1]), and parameter_2 = np.arange(2, 4) = array([2, 3]), then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
+    This multiparameter sweep is pretty cool, as it will generate designer list of dictionaries that comprise of all the possible combinations of your parameter sweeps. For example, if you are sweeping `parameter_1 = np.arange(0, 2) = array([0, 1])`, and `parameter_2 = np.arange(2, 4) = array([2, 3])`, then this function will generate list of dictionaries based on the default_design dictionary, but that will comprise of all the potential parameter combinations within this list.
 
     For the example above, there arould be 4 combinations [(0, 2), (0, 3), (1, 2), (1, 3)].
 
-    If you were instead sweeping for parameter_1 = np.arange(0, 5) and parameter_2 = np.arange(0, 5), the dictionary generated would correspond to these parameter combinations of [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
+    If you were instead sweeping for `parameter_1 = np.arange(0, 5)` and `parameter_2 = np.arange(0, 5)`, the dictionary generated would correspond to these parameter combinations of::
+        [(0, 0), (0, 1), (0, 2), (0, 3), (0, 4), (1, 0), (1, 1), (1, 2), (1, 3), (1, 4), (2, 0), (2, 1), (2, 2), (2, 3), (2, 4), (3, 0), (3, 1), (3, 2), (3, 3), (3, 4), (4, 0), (4, 1), (4, 2), (4, 3), (4, 4)].
 
     Make sure to use the parameter_names from default_design when writing up the parameter_sweep dictionary key name.
 
     Example project_structure formats::
 
         example_parameter_sweep_dictionary = {
             "parameter_1": np.arange(1, -40, 1),
@@ -53,11 +54,12 @@
         for parameter in parameter_combination:
             design[parameter_names_sweep_list[parameter_index]] = parameter
             parameter_index += 1
         parameter_sweep_design_dictionary_array.extend([design])
 
     return parameter_sweep_design_dictionary_array
 
+
 __all__ = [
     "single_parameter_sweep",
     "multi_parameter_sweep",
 ]
```

### Comparing `piel-0.0.24/piel/simulation.py` & `piel-0.0.25/piel/simulation.py`

 * *Files identical despite different names*

### Comparing `piel-0.0.24/piel.egg-info/PKG-INFO` & `piel-0.0.25/piel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piel
-Version: 0.0.24
+Version: 0.0.25
 Summary: Photonic and electronic co-simulation system design tools interfaced with open-source design software like GDSFactory and OpenROAD.
 Home-page: https://github.com/daquintero/piel
 Author: Dario Quintero
 Author-email: darioaquintero@gmail.com
 License: MIT license
 Keywords: piel
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `piel-0.0.24/piel.egg-info/SOURCES.txt` & `piel-0.0.25/piel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
+docs/examples.rst
 docs/history.rst
 docs/index.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 docs/autoapi/index.rst
 docs/autoapi/piel/index.rst
```

### Comparing `piel-0.0.24/setup.py` & `piel-0.0.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,10 +62,10 @@
     include_package_data=True,
     keywords="piel",
     name="piel",
     packages=find_packages(include=["piel", "piel.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url='https://github.com/daquintero/piel',
-    version='0.0.24',
+    version="0.0.25",
     zip_safe=False,
 )
```

### Comparing `piel-0.0.24/tests/test_piel.py` & `piel-0.0.25/tests/test_piel.py`

 * *Files identical despite different names*

