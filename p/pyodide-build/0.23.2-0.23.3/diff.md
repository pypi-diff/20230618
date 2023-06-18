# Comparing `tmp/pyodide-build-0.23.2.tar.gz` & `tmp/pyodide-build-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-build-0.23.2.tar", last modified: Wed May  3 06:08:44 2023, max compression
+gzip compressed data, was "pyodide-build-0.23.3.tar", last modified: Sun Jun 18 02:24:12 2023, max compression
```

## Comparing `pyodide-build-0.23.2.tar` & `pyodide-build-0.23.3.tar`

### file list

```diff
@@ -1,56 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/_f2c_fixes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/_py_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/buildall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31135 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/buildpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/build_recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/create_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/py_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/cli/xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/create_pypa_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/create_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/install_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/mkpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/out_of_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/pypi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/out_of_tree/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/pypabuild.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/pywasmcross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/pyzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.731597 pyodide-build-0.23.2/pyodide_build/tools/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.731597 pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/Platform/
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyodide_build/tools/pyo3_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:44.739598 pyodide-build-0.23.2/pyodide_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 06:08:44.000000 pyodide-build-0.23.2/pyodide_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-03 06:08:44.743598 pyodide-build-0.23.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 06:08:28.000000 pyodide-build-0.23.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.486356 pyodide-build-0.23.3/pyodide_build/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1408 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17625 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/_f2c_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/_py_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27665 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/buildall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30522 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/buildpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/build_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/create_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/py_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/cli/xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/create_pypa_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/create_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/install_xbuildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8595 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/mkpkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/out_of_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/out_of_tree/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/pypabuild.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20853 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/pywasmcross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/pyzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tests/replace_so_abi_tags_test_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tools/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.482355 pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/Platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyodide_build/tools/pyo3_config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/pyodide_build.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 02:24:12.000000 pyodide-build-0.23.3/pyodide_build.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-18 02:24:12.490356 pyodide-build-0.23.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 02:23:58.000000 pyodide-build-0.23.3/setup.py
```

### Comparing `pyodide-build-0.23.2/LICENSE` & `pyodide-build-0.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/PKG-INFO` & `pyodide-build-0.23.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-build
-Version: 0.23.2
+Version: 0.23.3
 Summary: "Tools for building Pyodide"
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyodide-build-0.23.2/pyodide_build/__main__.py` & `pyodide-build-0.23.3/pyodide_build/__main__.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/_f2c_fixes.py` & `pyodide-build-0.23.3/pyodide_build/_f2c_fixes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/_py_compile.py` & `pyodide-build-0.23.3/pyodide_build/_py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/buildall.py` & `pyodide-build-0.23.3/pyodide_build/buildall.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/buildpkg.py` & `pyodide-build-0.23.3/pyodide_build/buildpkg.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import cgi
 import fnmatch
 import json
 import os
 import shutil
 import subprocess
 import sys
-import sysconfig
 import textwrap
 import urllib
 from collections.abc import Iterator
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from textwrap import dedent
@@ -28,14 +27,16 @@
 from .common import (
     _get_sha256_checksum,
     chdir,
     exit_with_stdio,
     find_matching_wheels,
     find_missing_executables,
     make_zip_archive,
+    modify_wheel,
+    replace_so_abi_tags,
     set_build_environment,
 )
 from .io import MetaConfig, _BuildSpec, _SourceSpec
 from .logger import logger
 from .pywasmcross import BuildArgs
 
 
@@ -425,26 +426,14 @@
 
         from .pypabuild import build
 
         outpath = srcpath / "dist"
         build(srcpath, outpath, build_env, backend_flags)
 
 
-def replace_so_abi_tags(wheel_dir: Path) -> None:
-    """Replace native abi tag with emscripten abi tag in .so file names"""
-    build_soabi = sysconfig.get_config_var("SOABI")
-    assert build_soabi
-    ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
-    assert ext_suffix
-    build_triplet = "-".join(build_soabi.split("-")[2:])
-    host_triplet = common.get_make_flag("PLATFORM_TRIPLET")
-    for file in wheel_dir.glob(f"**/*{ext_suffix}"):
-        file.rename(file.with_name(file.name.replace(build_triplet, host_triplet)))
-
-
 def copy_sharedlibs(
     wheel_file: Path, wheel_dir: Path, lib_dir: Path
 ) -> dict[str, Path]:
     from auditwheel_emscripten import copylib, resolve_sharedlib  # type: ignore[import]
     from auditwheel_emscripten.wheel_utils import WHEEL_INFO_RE  # type: ignore[import]
 
     match = WHEEL_INFO_RE.match(wheel_file.name)
@@ -504,63 +493,58 @@
     distdir = srcpath / "dist"
     wheel, *rest = find_matching_wheels(distdir.glob("*.whl"))
     if rest:
         raise Exception(
             f"Unexpected number of wheels {len(rest) + 1} when building {pkg_name}"
         )
     logger.info(f"Unpacking wheel to {str(wheel)}")
-    unpack_wheel(wheel)
-    wheel.unlink()
+
     name, ver, _ = wheel.name.split("-", 2)
-    wheel_dir_name = f"{name}-{ver}"
-    wheel_dir = distdir / wheel_dir_name
 
-    # update so abi tags after build is complete but before running post script
-    # to maximize sanity.
-    replace_so_abi_tags(wheel_dir)
-
-    post = build_metadata.post
-    if post:
-        logger.info(f"Running post script in {Path.cwd().absolute()}")
-        bash_runner.env.update({"WHEELDIR": str(wheel_dir)})
-        result = bash_runner.run(post)
-        if result.returncode != 0:
-            logger.error("ERROR: post failed")
-            exit_with_stdio(result)
+    with modify_wheel(wheel) as wheel_dir:
+        # update so abi tags after build is complete but before running post script
+        # to maximize sanity.
+        replace_so_abi_tags(wheel_dir)
+
+        post = build_metadata.post
+        if post:
+            logger.info(f"Running post script in {Path.cwd().absolute()}")
+            bash_runner.env.update({"WHEELDIR": str(wheel_dir)})
+            result = bash_runner.run(post)
+            if result.returncode != 0:
+                logger.error("ERROR: post failed")
+                exit_with_stdio(result)
 
-    vendor_sharedlib = build_metadata.vendor_sharedlib
-    if vendor_sharedlib:
-        lib_dir = Path(common.get_make_flag("WASM_LIBRARY_DIR"))
-        copy_sharedlibs(wheel, wheel_dir, lib_dir)
-
-    python_dir = f"python{sys.version_info.major}.{sys.version_info.minor}"
-    host_site_packages = Path(host_install_dir) / f"lib/{python_dir}/site-packages"
-    if build_metadata.cross_build_env:
-        subprocess.check_call(
-            ["pip", "install", "-t", str(host_site_packages), f"{name}=={ver}"]
-        )
+        vendor_sharedlib = build_metadata.vendor_sharedlib
+        if vendor_sharedlib:
+            lib_dir = Path(common.get_make_flag("WASM_LIBRARY_DIR"))
+            copy_sharedlibs(wheel, wheel_dir, lib_dir)
+
+        python_dir = f"python{sys.version_info.major}.{sys.version_info.minor}"
+        host_site_packages = Path(host_install_dir) / f"lib/{python_dir}/site-packages"
+        if build_metadata.cross_build_env:
+            subprocess.check_call(
+                ["pip", "install", "-t", str(host_site_packages), f"{name}=={ver}"]
+            )
 
-    cross_build_files = build_metadata.cross_build_files
-    if cross_build_files:
-        for file_ in cross_build_files:
-            shutil.copy((wheel_dir / file_), host_site_packages / file_)
-
-    test_dir = distdir / "tests"
-    nmoved = 0
-    if build_metadata.unvendor_tests:
-        nmoved = unvendor_tests(wheel_dir, test_dir)
-    if nmoved:
-        with chdir(distdir):
-            shutil.make_archive(f"{pkg_name}-tests", "tar", test_dir)
-    pack_wheel(wheel_dir)
-    # wheel_dir causes pytest collection failures for in-tree packages like
-    # micropip. To prevent these, we get rid of wheel_dir after repacking the
-    # wheel.
-    shutil.rmtree(wheel_dir)
-    shutil.rmtree(test_dir, ignore_errors=True)
+        cross_build_files = build_metadata.cross_build_files
+        if cross_build_files:
+            for file_ in cross_build_files:
+                shutil.copy((wheel_dir / file_), host_site_packages / file_)
+
+        try:
+            test_dir = distdir / "tests"
+            nmoved = 0
+            if build_metadata.unvendor_tests:
+                nmoved = unvendor_tests(wheel_dir, test_dir)
+            if nmoved:
+                with chdir(distdir):
+                    shutil.make_archive(f"{pkg_name}-tests", "tar", test_dir)
+        finally:
+            shutil.rmtree(test_dir, ignore_errors=True)
 
 
 def unvendor_tests(install_prefix: Path, test_install_prefix: Path) -> int:
     """Unvendor test files and folders
 
     This function recursively walks through install_prefix and moves anything
     that looks like a test folder under test_install_prefix.
```

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/build.py` & `pyodide-build-0.23.3/pyodide_build/cli/build.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/build_recipes.py` & `pyodide-build-0.23.3/pyodide_build/cli/build_recipes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/config.py` & `pyodide-build-0.23.3/pyodide_build/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/create_zipfile.py` & `pyodide-build-0.23.3/pyodide_build/cli/create_zipfile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/py_compile.py` & `pyodide-build-0.23.3/pyodide_build/cli/py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/skeleton.py` & `pyodide-build-0.23.3/pyodide_build/cli/skeleton.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/cli/xbuildenv.py` & `pyodide-build-0.23.3/pyodide_build/cli/xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/common.py` & `pyodide-build-0.23.3/pyodide_build/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -490,7 +490,68 @@
     with open(archive, "rb") as fd:
         while True:
             chunk = fd.read(CHUNK_SIZE)
             h.update(chunk)
             if len(chunk) < CHUNK_SIZE:
                 break
     return h.hexdigest()
+
+
+def unpack_wheel(wheel_path: Path, target_dir: Path | None = None) -> None:
+    if target_dir is None:
+        target_dir = wheel_path.parent
+    result = subprocess.run(
+        [sys.executable, "-m", "wheel", "unpack", wheel_path, "-d", target_dir],
+        check=False,
+        encoding="utf-8",
+    )
+    if result.returncode != 0:
+        logger.error(f"ERROR: Unpacking wheel {wheel_path.name} failed")
+        exit_with_stdio(result)
+
+
+def pack_wheel(wheel_dir: Path, target_dir: Path | None = None) -> None:
+    if target_dir is None:
+        target_dir = wheel_dir.parent
+    result = subprocess.run(
+        [sys.executable, "-m", "wheel", "pack", wheel_dir, "-d", target_dir],
+        check=False,
+        encoding="utf-8",
+    )
+    if result.returncode != 0:
+        logger.error(f"ERROR: Packing wheel {wheel_dir} failed")
+        exit_with_stdio(result)
+
+
+@contextmanager
+def modify_wheel(wheel: Path) -> Iterator[Path]:
+    """Unpacks the wheel into a temp directory and yields the path to the
+    unpacked directory.
+
+    The body of the with block is expected to inspect the wheel contents and
+    possibly change it. If the body of the "with" block is successful, on
+    exiting the with block the wheel contents are replaced with the updated
+    contents of unpacked directory. If an exception is raised, then the original
+    wheel is left unchanged.
+    """
+    with TemporaryDirectory() as temp_dir:
+        unpack_wheel(wheel, Path(temp_dir))
+        name, ver, _ = wheel.name.split("-", 2)
+        wheel_dir_name = f"{name}-{ver}"
+        wheel_dir = Path(temp_dir) / wheel_dir_name
+        yield wheel_dir
+        wheel.unlink()
+        pack_wheel(wheel_dir, wheel.parent)
+
+
+def replace_so_abi_tags(wheel_dir: Path) -> None:
+    """Replace native abi tag with emscripten abi tag in .so file names"""
+    import sysconfig
+
+    build_soabi = sysconfig.get_config_var("SOABI")
+    assert build_soabi
+    ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
+    assert ext_suffix
+    build_triplet = "-".join(build_soabi.split("-")[2:])
+    host_triplet = get_make_flag("PLATFORM_TRIPLET")
+    for file in wheel_dir.glob(f"**/*{ext_suffix}"):
+        file.rename(file.with_name(file.name.replace(build_triplet, host_triplet)))
```

### Comparing `pyodide-build-0.23.2/pyodide_build/create_pypa_index.py` & `pyodide-build-0.23.3/pyodide_build/create_pypa_index.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/create_xbuildenv.py` & `pyodide-build-0.23.3/pyodide_build/create_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/install_xbuildenv.py` & `pyodide-build-0.23.3/pyodide_build/install_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/io.py` & `pyodide-build-0.23.3/pyodide_build/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,14 +172,16 @@
         """
         import yaml
 
         stream = path.read_bytes()
         config_raw = yaml.safe_load(stream)
 
         config = cls(**config_raw)
+        if config.source.path:
+            config.source.path = path.parent / config.source.path
         return config
 
     def to_yaml(self, path: Path) -> None:
         """Serialize the configuration to meta.yaml file
 
         Parameters
         ----------
```

### Comparing `pyodide-build-0.23.2/pyodide_build/logger.py` & `pyodide-build-0.23.3/pyodide_build/logger.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/mkpkg.py` & `pyodide-build-0.23.3/pyodide_build/mkpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/out_of_tree/build.py` & `pyodide-build-0.23.3/pyodide_build/out_of_tree/build.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,13 @@
         ldflags=ldflags,
         target_install_dir="",
         exports=exports,
     )
 
     with build_env_ctx as env:
         built_wheel = pypabuild.build(srcdir, outdir, env, " ".join(args))
-    return Path(built_wheel)
+
+    wheel_path = Path(built_wheel)
+    with common.modify_wheel(wheel_path) as wheel_dir:
+        common.replace_so_abi_tags(wheel_dir)
+
+    return wheel_path
```

### Comparing `pyodide-build-0.23.2/pyodide_build/out_of_tree/pypi.py` & `pyodide-build-0.23.3/pyodide_build/out_of_tree/pypi.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/out_of_tree/utils.py` & `pyodide-build-0.23.3/pyodide_build/out_of_tree/utils.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/out_of_tree/venv.py` & `pyodide-build-0.23.3/pyodide_build/out_of_tree/venv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/pypabuild.py` & `pyodide-build-0.23.3/pyodide_build/pypabuild.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/pywasmcross.py` & `pyodide-build-0.23.3/pyodide_build/pywasmcross.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/pyzip.py` & `pyodide-build-0.23.3/pyodide_build/pyzip.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/recipe.py` & `pyodide-build-0.23.3/pyodide_build/recipe.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/serve.py` & `pyodide-build-0.23.3/pyodide_build/serve.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake` & `pyodide-build-0.23.3/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.23.2/pyodide_build.egg-info/PKG-INFO` & `pyodide-build-0.23.3/pyodide_build.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-build
-Version: 0.23.2
+Version: 0.23.3
 Summary: "Tools for building Pyodide"
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 License: MPL-2.0
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyodide-build-0.23.2/pyodide_build.egg-info/SOURCES.txt` & `pyodide-build-0.23.3/pyodide_build.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 ./pyodide_build/cli/venv.py
 ./pyodide_build/cli/xbuildenv.py
 ./pyodide_build/out_of_tree/__init__.py
 ./pyodide_build/out_of_tree/build.py
 ./pyodide_build/out_of_tree/pypi.py
 ./pyodide_build/out_of_tree/utils.py
 ./pyodide_build/out_of_tree/venv.py
+./pyodide_build/tests/replace_so_abi_tags_test_package/mypkg/__init__.py
 ./pyodide_build/tools/pyo3_config.ini
 ./pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
 pyodide_build.egg-info/PKG-INFO
 pyodide_build.egg-info/SOURCES.txt
 pyodide_build.egg-info/dependency_links.txt
 pyodide_build.egg-info/entry_points.txt
 pyodide_build.egg-info/requires.txt
```

### Comparing `pyodide-build-0.23.2/setup.cfg` & `pyodide-build-0.23.3/setup.cfg`

 * *Files identical despite different names*

