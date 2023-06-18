# Comparing `tmp/pyodide-py-0.23.2.tar.gz` & `tmp/pyodide-py-0.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-py-0.23.2.tar", last modified: Wed May  3 06:08:45 2023, max compression
+gzip compressed data, was "pyodide-py-0.23.3.tar", last modified: Sun Jun 18 02:24:23 2023, max compression
```

## Comparing `pyodide-py-0.23.2.tar` & `pyodide-py-0.23.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:45.345158 pyodide-py-0.23.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 06:08:45.345158 pyodide-py-0.23.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:45.341158 pyodide-py-0.23.2/_pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/_pyodide/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42449 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/_pyodide/_core_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/_pyodide/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/_pyodide/docs_argspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/_pyodide/docstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:45.341158 pyodide-py-0.23.2/pyodide/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/_package_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/_run_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/code.py
--rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:45.341158 pyodide-py-0.23.2/pyodide/ffi/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/ffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/ffi/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyodide/webloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:08:45.341158 pyodide-py-0.23.2/pyodide_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-03 06:08:45.000000 pyodide-py-0.23.2/pyodide_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-03 06:08:45.000000 pyodide-py-0.23.2/pyodide_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:08:45.000000 pyodide-py-0.23.2/pyodide_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 06:08:45.000000 pyodide-py-0.23.2/pyodide_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-03 06:08:45.345158 pyodide-py-0.23.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-05-03 06:08:26.000000 pyodide-py-0.23.2/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.975789 pyodide-py-0.23.3/_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42449 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/_core_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/docs_argspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/_pyodide/docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.979789 pyodide-py-0.23.3/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_package_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_run_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20421 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.979789 pyodide-py-0.23.3/pyodide/ffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/ffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/ffi/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyodide/webloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/pyodide_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-18 02:24:23.000000 pyodide-py-0.23.3/pyodide_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-18 02:24:23.983789 pyodide-py-0.23.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-06-18 02:24:04.000000 pyodide-py-0.23.3/webbrowser.py
```

### Comparing `pyodide-py-0.23.2/PKG-INFO` & `pyodide-py-0.23.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.23.2
+Version: 0.23.3
 Summary: "A Python package providing core interpreter functionality for Pyodide."
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.23.2/README.md` & `pyodide-py-0.23.3/README.md`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/_pyodide/_base.py` & `pyodide-py-0.23.3/_pyodide/_base.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/_pyodide/_core_docs.py` & `pyodide-py-0.23.3/_pyodide/_core_docs.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/_pyodide/_importhook.py` & `pyodide-py-0.23.3/_pyodide/_importhook.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/_pyodide/docs_argspec.py` & `pyodide-py-0.23.3/_pyodide/docs_argspec.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/_pyodide/docstring.py` & `pyodide-py-0.23.3/_pyodide/docstring.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/__init__.py` & `pyodide-py-0.23.3/pyodide/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # All pure Python code that does not require js or pyodide_js should go in
 # the _pyodide package.
 #
 # This package is imported by the test suite as well, and currently we don't use
 # pytest mocks for js or pyodide_js, so make sure to test "if IN_BROWSER" before
 # importing from these.
-__version__ = "0.23.2"
+__version__ = "0.23.3"
 
 __all__ = ["__version__", "console", "code", "ffi", "http", "webloop"]
 
 from . import _state  # noqa: F401
 from .webloop import _initialize_event_loop
 
 _initialize_event_loop()
```

### Comparing `pyodide-py-0.23.2/pyodide/_package_loader.py` & `pyodide-py-0.23.3/pyodide/_package_loader.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/_state.py` & `pyodide-py-0.23.3/pyodide/_state.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/code.py` & `pyodide-py-0.23.3/pyodide/code.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/console.py` & `pyodide-py-0.23.3/pyodide/console.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/ffi/__init__.py` & `pyodide-py-0.23.3/pyodide/ffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/ffi/wrappers.py` & `pyodide-py-0.23.3/pyodide/ffi/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/http.py` & `pyodide-py-0.23.3/pyodide/http.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide/webloop.py` & `pyodide-py-0.23.3/pyodide/webloop.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/pyodide_py.egg-info/PKG-INFO` & `pyodide-py-0.23.3/pyodide_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.23.2
+Version: 0.23.3
 Summary: "A Python package providing core interpreter functionality for Pyodide."
 Home-page: https://github.com/pyodide/pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.23.2/pyodide_py.egg-info/SOURCES.txt` & `pyodide-py-0.23.3/pyodide_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.23.2/setup.cfg` & `pyodide-py-0.23.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyodide-py
-version = 0.23.2
+version = 0.23.3
 author = Pyodide developers
 description = "A Python package providing core interpreter functionality for Pyodide."
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyodide/pyodide
 project_urls = 
 	Bug Tracker = https://github.com/pyodide/pyodide/issues
```

