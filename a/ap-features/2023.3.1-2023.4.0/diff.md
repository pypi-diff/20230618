# Comparing `tmp/ap_features-2023.3.1.tar.gz` & `tmp/ap_features-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ap_features-2023.3.1.tar", last modified: Wed Jun  7 07:49:21 2023, max compression
+gzip compressed data, was "ap_features-2023.4.0.tar", last modified: Sun Jun 18 14:21:25 2023, max compression
```

## Comparing `ap_features-2023.3.1.tar` & `ap_features-2023.4.0.tar`

### file list

```diff
@@ -1,62 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.358227 ap_features-2023.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 07:48:47.000000 ap_features-2023.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-07 07:48:47.000000 ap_features-2023.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-07 07:48:47.000000 ap_features-2023.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 07:48:47.000000 ap_features-2023.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-07 07:49:21.358227 ap_features-2023.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-07 07:48:47.000000 ap_features-2023.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-07 07:48:47.000000 ap_features-2023.3.1/docs/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-06-07 07:48:47.000000 ap_features-2023.3.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-07 07:48:47.000000 ap_features-2023.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 07:49:21.358227 ap_features-2023.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/c/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/c/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cmake/BuildType.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/common.h
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cost_terms.c
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cost_terms.h
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/c/cost_terms_main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/python/ap_features/
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/_numba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/average.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    39251 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/beat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    28479 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-07 07:48:47.000000 ap_features-2023.3.1/src/python/ap_features/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/src/python/ap_features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 07:49:21.000000 ap_features-2023.3.1/src/python/ap_features.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.354227 ap_features-2023.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.350227 ap_features-2023.3.1/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 07:49:21.358227 ap_features-2023.3.1/tests/baseline_images/test_plot/
--rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/beats.png
--rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/beats_aligned.png
--rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/poincare.png
--rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat.png
--rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_background.png
--rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_pacing.png
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/cost_terms.npy
--rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/data.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/real_data.npy
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_beat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_chopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-07 07:48:47.000000 ap_features-2023.3.1/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.671556 ap_features-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-18 14:20:46.000000 ap_features-2023.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-18 14:20:46.000000 ap_features-2023.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-18 14:20:46.000000 ap_features-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-18 14:20:46.000000 ap_features-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-18 14:21:25.671556 ap_features-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-18 14:20:46.000000 ap_features-2023.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.663555 ap_features-2023.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-18 14:20:46.000000 ap_features-2023.4.0/docs/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-18 14:20:46.000000 ap_features-2023.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-18 14:20:46.000000 ap_features-2023.4.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-18 14:20:46.000000 ap_features-2023.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:21:25.671556 ap_features-2023.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.663555 ap_features-2023.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.667556 ap_features-2023.4.0/src/ap_features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/_numba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39210 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21125 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-18 14:20:46.000000 ap_features-2023.4.0/src/ap_features/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.667556 ap_features-2023.4.0/src/ap_features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 14:21:25.000000 ap_features-2023.4.0/src/ap_features.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.667556 ap_features-2023.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.663555 ap_features-2023.4.0/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:21:25.671556 ap_features-2023.4.0/tests/baseline_images/test_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)    61987 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/beats.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79471 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/beats_aligned.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47169 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/poincare.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61269 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66463 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/cost_terms.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    32184 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/real_data.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_beat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_chopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-18 14:20:46.000000 ap_features-2023.4.0/tests/test_plot.py
```

### Comparing `ap_features-2023.3.1/CONTRIBUTING.md` & `ap_features-2023.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/LICENSE` & `ap_features-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/PKG-INFO` & `ap_features-2023.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ap_features
-Version: 2023.3.1
+Version: 2023.4.0
 Summary: Package to compute features of traces from action potential models
 Author-email: Henrik Finsberg <henriknf@simula.no>, "Kristian G. Hustad" <kghustad@simula.no>
 License: LGPL-2.1
 Project-URL: Homepage, https://computationalphysiology.github.io/ap_features
 Project-URL: Documentation, https://computationalphysiology.github.io/ap_features
 Project-URL: Source, https://github.com/ComputationalPhysiology/ap_features
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/ap_features/issues
 Keywords: action potential,cell,models,features
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: array
 Provides-Extra: dev
 Provides-Extra: plot
 Provides-Extra: pypi
 Provides-Extra: docs
+Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![image](https://img.shields.io/pypi/v/ap_features.svg)](https://pypi.python.org/pypi/ap_features)
 ![CI](https://github.com/ComputationalPhysiology/ap_features/workflows/CI/badge.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComputationalPhysiology/ap_features/main.svg)](https://results.pre-commit.ci/latest/github/ComputationalPhysiology/ap_features/main)
```

### Comparing `ap_features-2023.3.1/README.md` & `ap_features-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/docs/INSTALL.md` & `ap_features-2023.4.0/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/pyproject.toml` & `ap_features-2023.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "oldest-supported-numpy; python_version>='3.5'",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "ap_features"
-version = "2023.3.1"
+version = "2023.4.0"
 description = "Package to compute features of traces from action potential models"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}, {name = "Kristian G. Hustad", email = "kghustad@simula.no" }]
 license = {text = "LGPL-2.1"}
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["action potential", "cell", "models", "features"]
 dependencies = [
@@ -27,20 +27,14 @@
 [project.urls]
 Homepage = "https://computationalphysiology.github.io/ap_features"
 Documentation = "https://computationalphysiology.github.io/ap_features"
 Source = "https://github.com/ComputationalPhysiology/ap_features"
 Tracker = "https://github.com/ComputationalPhysiology/ap_features/issues"
 
 [project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-cov",
-    "ap_features[plot]",
-    "ap_features[array]"
-]
 array = [
     "h5py",
     "dask[array]"
 ]
 dev = [
     "pdbpp",
     "ipython",
@@ -52,43 +46,46 @@
 ]
 pypi = [
     "twine",
     "build"
 ]
 docs = [
    "jupyter-book",
+   "ap_features[plot]",
+]
+test = [
+    "pytest",
+    "pytest-cov",
+    "ap_features[plot]",
+    "ap_features[array]"
 ]
 all = [
    "ap_features[test]",
    "ap_features[docs]",
    "ap_features[pypi]",
    "ap_features[dev]",
    "ap_features[array]",
    "ap_features[plot]",
 ]
 
 
-[tool.setuptools.packages.find]
-where = ["src/python"]
-
-
 [tool.pytest.ini_options]
 addopts = [
    "--cov=ap_features",
    "--cov-report=html",
    "--cov-report=term-missing",
    "-v"
 ]
 
 testpaths = [
     "tests"
 ]
 
 [tool.mypy]
-files = ["src/python/ap_features","tests"]
+files = ["src/ap_features","tests"]
 ignore_missing_imports = true
 exclude = "docs"
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 ignore = ["E402", "E741", "E731"]
```

### Comparing `ap_features-2023.3.1/src/python/ap_features/__init__.py` & `ap_features-2023.4.0/src/ap_features/__init__.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/_numba.py` & `ap_features-2023.4.0/src/ap_features/_numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,35 +82,35 @@
             t_o = T[idx2 - 1]
             t_end = (t_o - t_u) / (v_o - v_u) * (th - (t_o * v_u - t_u * v_o) / (t_o - t_u))
             break
     return t_end, idx2
 
 
 @numba.njit(numba.float64(float_1D_array, float_1D_array, numba.int64, numba.int64))
-def apd_up_xy(y: np.ndarray, t: np.ndarray, factor_x: int, factor_y: int) -> float:
+def apd_up_xy(y: np.ndarray, t: np.ndarray, low: int, high: int) -> float:
     """Compute time from first intersection of
     APDx line to first intersection of APDy line
     """
-    if factor_x > factor_y:
-        # factor_x has to be larger than factor_y
+    if low > high:
+        # low has to be larger than high
         return -np.inf
-    if factor_x == factor_y:
+    if low == high:
         return 0
 
     t_half = t.max() / 2
     idx_t_half = int(np.argmin(np.abs(t - t_half)))
 
     # Set up threshold
     y_max = np.max(y[:idx_t_half])
     max_idx = np.argmax(y[:idx_t_half])
     y_min = np.min(y)
 
-    thx = y_min + (1 - factor_x / 100) * (y_max - y_min)
+    thx = y_min + (1 - low / 100) * (y_max - y_min)
     tx, idx1 = get_t_start(max_idx, y, t, thx, t_start=0)
-    thy = y_min + (1 - factor_y / 100) * (y_max - y_min)
+    thy = y_min + (1 - high / 100) * (y_max - y_min)
     ty, idx1 = get_t_start(max_idx, y, t, thy, t_start=tx)
     return tx - ty
 
 
 @numba.njit(numba.float64(float_1D_array, float_1D_array, numba.int64))
 def compute_integral(V, T, factor):
     dt = T[1] - T[0]
```

### Comparing `ap_features-2023.3.1/src/python/ap_features/average.py` & `ap_features-2023.4.0/src/ap_features/average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/background.py` & `ap_features-2023.4.0/src/ap_features/background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/beat.py` & `ap_features-2023.4.0/src/ap_features/beat.py`

 * *Files 1% similar despite different names*

```diff
@@ -608,32 +608,32 @@
         """
         return features.detect_ead(
             self.y,
             sigma=sigma,
             prominence_level=prominence_level,
         )
 
-    def apd_up_xy(self, factor_x, factor_y):
+    def apd_up_xy(self, low, high):
         """Find the duration between first intersection (i.e
         during the upstroke) of two APD lines
 
         Arguments
         ---------
-        factor_x: int
+        low: int
             First APD line (value between 0 and 100)
-        factor_y: int
+        high: int
             Second APD line (value between 0 and 100)
 
         Returns
         -------
         float:
-            The time between `factor_x` to `factor_y`
+            The time between `low` to `high`
 
         """
-        return features.apd_up_xy(self.y, self.y, factor_x=factor_x, factor_y=factor_y)
+        return features.apd_up_xy(y=self.y, t=self.t, low=low, high=high)
 
     @property
     def cost_terms(self):
         return features.cost_terms_trace(y=self.y, t=self.t, backend=self._backend)
 
 
 def remove_bad_indices(feature_list: List[List[float]], bad_indices: Set[int]):
```

### Comparing `ap_features-2023.3.1/src/python/ap_features/chopping.py` & `ap_features-2023.4.0/src/ap_features/chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/features.py` & `ap_features-2023.4.0/src/ap_features/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     .. math::
         \mathrm{APD} \; p = \min \mathcal{T} / \min \mathcal{T}  - \min \mathcal{T}
 
     """ ""
 
     assert backend in Backend.__members__
 
-    if isinstance(factor, float) and 0 < factor < 1:
+    if isinstance(factor, (float, np.float_)) and 0 < factor < 1:
         # Factor should be multiplied with 100
         factor = int(factor * 100)
     _check_factor(factor)
 
     y = np.array(V)
     x = np.array(t)
     if y.shape != x.shape:
@@ -284,15 +284,15 @@
 ) -> APDCoords:
     """Return the coordinates of the start and stop
         of the APD, and not the duration itself
 
     Parameters
     ----------
     factor : int
-        The APD factor between 0 and 100
+        The APD factor between 0 and 100.
     V : Array
         The signal
     t : Array
         The time stamps
     v_r : Optional[float], optional
         Resting value, by default None. Only applicable for python Backend.
     use_spline : bool, optional
@@ -330,28 +330,32 @@
     Parameters
     ----------
     x : Array
         The time stamps
     y : Array
         The signal
     a : float, optional
-        The value for which you want to estimate the time decay, by default 0.75
+        The value for which you want to estimate the time decay, by default 0.75.
+        If the value is larger than 1.0 it will be divided by 100
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
         Choices, 'python', 'numba'
 
     Returns
     -------
     float
         Decay time
 
     """
     if backend != Backend.python:
         logger.warning("Method currently only implemented for python backend")
 
+    if a > 1.0:
+        a /= 100
+
     Y = UnivariateSpline(x, utils.normalize_signal(y) - a, s=0, k=3)
     t_max = x[int(np.argmax(y))]
     r = Y.roots()
     if len(r) >= 2:
         t_a = r[1]
     elif len(r) == 1:
         logger.warning(
@@ -444,15 +448,16 @@
     Parameters
     ----------
     x : Array
         The time stamps
     y : Array
         The signal
     a : float, optional
-        Fraction of signal amplitude, by default 0.8
+        Fraction of signal amplitude, by default 0.8.
+        If the value is larger than 1.0 it will be divided by 100
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
         Choices, 'python', 'numba'
 
     Returns
     -------
     float
@@ -462,14 +467,17 @@
     ------
     ValueError
         If a is outside the range of (0, 1)
     """
     if backend != Backend.python:
         logger.warning("Method currently only implemented for python backend")
 
+    if a > 1.0:
+        a /= 100.0
+
     if not 0 < a < 1:
         raise ValueError("'a' has to be between 0.0 and 1.0")
 
     Y = UnivariateSpline(x, utils.normalize_signal(y) - (1 - a), s=0, k=3)
     t_max = x[int(np.argmax(y))]
     r = Y.roots()
     if len(r) >= 1:
@@ -582,58 +590,58 @@
 
     return upstroke
 
 
 def apd_up_xy(
     y: Array,
     t: Array,
-    factor_x: int,
-    factor_y: int,
+    low: int,
+    high: int,
     backend: Backend = Backend.python,
 ) -> float:
     """Find the duration between first intersection (i.e
     during the upstroke) of two APD lines
 
     Arguments
     ---------
     t : np.ndarray
         Time values
     y : np.ndarray
         The trace
-    from_APD: int
+    low: int
         First APD line (value between 0 and 100)
-    to_APD: int
+    high: int
         Second APD line (value between 0 and 100)
     backend : utils.Backend, optional
         Which backend to use by default Backend.python.
         Choices, 'python', 'numba'
 
     Returns
     -------
     float:
-        The time between `factor_x` to `factor_y`
+        The time between `low` to `high`
 
 
 
     """
-    _check_factor(factor_x)
-    _check_factor(factor_y)
+    _check_factor(low)
+    _check_factor(high)
 
     y = numpyfy(y)
     t = numpyfy(t)
 
     if backend == Backend.numba:
-        return _numba.apd_up_xy(y=y, t=t, factor_x=factor_x, factor_y=factor_y)
+        return _numba.apd_up_xy(y=y, t=t, low=low, high=high)
 
     y_norm = utils.normalize_signal(y)
 
-    y_from = UnivariateSpline(t, y_norm - factor_x / 100, s=0, k=3)
+    y_from = UnivariateSpline(t, y_norm - low / 100, s=0, k=3)
     t_from = y_from.roots()[0]
 
-    y_to = UnivariateSpline(t, y_norm - factor_y / 100, s=0, k=3)
+    y_to = UnivariateSpline(t, y_norm - high / 100, s=0, k=3)
     t_to = y_to.roots()[0]
 
     return t_to - t_from
 
 
 def max_relative_upstroke_velocity(
     t: np.ndarray,
```

### Comparing `ap_features-2023.3.1/src/python/ap_features/filters.py` & `ap_features-2023.4.0/src/ap_features/filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/plot.py` & `ap_features-2023.4.0/src/ap_features/plot.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/testing.py` & `ap_features-2023.4.0/src/ap_features/testing.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features/utils.py` & `ap_features-2023.4.0/src/ap_features/utils.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/src/python/ap_features.egg-info/PKG-INFO` & `ap_features-2023.4.0/src/ap_features.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: ap-features
-Version: 2023.3.1
+Version: 2023.4.0
 Summary: Package to compute features of traces from action potential models
 Author-email: Henrik Finsberg <henriknf@simula.no>, "Kristian G. Hustad" <kghustad@simula.no>
 License: LGPL-2.1
 Project-URL: Homepage, https://computationalphysiology.github.io/ap_features
 Project-URL: Documentation, https://computationalphysiology.github.io/ap_features
 Project-URL: Source, https://github.com/ComputationalPhysiology/ap_features
 Project-URL: Tracker, https://github.com/ComputationalPhysiology/ap_features/issues
 Keywords: action potential,cell,models,features
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
 Provides-Extra: array
 Provides-Extra: dev
 Provides-Extra: plot
 Provides-Extra: pypi
 Provides-Extra: docs
+Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![image](https://img.shields.io/pypi/v/ap_features.svg)](https://pypi.python.org/pypi/ap_features)
 ![CI](https://github.com/ComputationalPhysiology/ap_features/workflows/CI/badge.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ComputationalPhysiology/ap_features/main.svg)](https://results.pre-commit.ci/latest/github/ComputationalPhysiology/ap_features/main)
```

### Comparing `ap_features-2023.3.1/tests/baseline_images/test_plot/beats.png` & `ap_features-2023.4.0/tests/baseline_images/test_plot/beats.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/baseline_images/test_plot/beats_aligned.png` & `ap_features-2023.4.0/tests/baseline_images/test_plot/beats_aligned.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/baseline_images/test_plot/poincare.png` & `ap_features-2023.4.0/tests/baseline_images/test_plot/poincare.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat.png` & `ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_background.png` & `ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_background.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/baseline_images/test_plot/simple_beat_with_pacing.png` & `ap_features-2023.4.0/tests/baseline_images/test_plot/simple_beat_with_pacing.png`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/conftest.py` & `ap_features-2023.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/cost_terms.npy` & `ap_features-2023.4.0/tests/cost_terms.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/data.npy` & `ap_features-2023.4.0/tests/data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/real_data.npy` & `ap_features-2023.4.0/tests/real_data.npy`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/test_average.py` & `ap_features-2023.4.0/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/test_background.py` & `ap_features-2023.4.0/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/test_beat.py` & `ap_features-2023.4.0/tests/test_beat.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/test_chopping.py` & `ap_features-2023.4.0/tests/test_chopping.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/test_features.py` & `ap_features-2023.4.0/tests/test_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 
     apd = apf.apd(V=y, t=x, factor=factor, backend=backend)
 
     assert abs(apd - 2 * factor) < 1e-10
 
 
 @pytest.mark.parametrize(
-    "factor_x, factor_y, backend",
+    "low, high, backend",
     it.product(range(10, 95, 20), range(10, 95, 20), apf.Backend),
 )
-def test_apdxy_triangle_signal(factor_x, factor_y, backend, triangle_signal):
+def test_apdxy_triangle_signal(low, high, backend, triangle_signal):
     x, y = triangle_signal
 
-    apd = apf.apd_up_xy(y, x, factor_x, factor_y)
+    apd = apf.apd_up_xy(y, x, low, high)
 
-    if factor_x == factor_y:
+    if low == high:
         assert abs(apd) < 1e-12
     else:
-        assert abs(apd - (factor_y - factor_x)) < 1e-10
+        assert abs(apd - (high - low)) < 1e-10
 
 
 def test_number_of_cost_terms():
     assert apf.NUM_COST_TERMS == len(apf.list_cost_function_terms())
 
 
 def test_number_of_cost_terms_trace():
```

### Comparing `ap_features-2023.3.1/tests/test_filters.py` & `ap_features-2023.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ap_features-2023.3.1/tests/test_plot.py` & `ap_features-2023.4.0/tests/test_plot.py`

 * *Files identical despite different names*

