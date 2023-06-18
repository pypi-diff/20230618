# Comparing `tmp/aio-pygo-1.0.0.tar.gz` & `tmp/aio-pygo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-pygo-1.0.0.tar", last modified: Sun Jun 18 21:40:13 2023, max compression
+gzip compressed data, was "aio-pygo-1.0.1.tar", last modified: Sun Jun 18 21:51:16 2023, max compression
```

## Comparing `aio-pygo-1.0.0.tar` & `aio-pygo-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:40:13.413415 aio-pygo-1.0.0/
--rw-r--r--   0 gael       (501) staff       (20)    35149 2023-05-31 17:21:41.000000 aio-pygo-1.0.0/LICENSE
--rw-r--r--   0 gael       (501) staff       (20)     2874 2023-06-18 21:40:13.413249 aio-pygo-1.0.0/PKG-INFO
--rw-r--r--   0 gael       (501) staff       (20)     2403 2023-06-18 21:39:29.000000 aio-pygo-1.0.0/README.md
-drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:40:13.411167 aio-pygo-1.0.0/aio_pygo.egg-info/
--rw-r--r--   0 gael       (501) staff       (20)     2874 2023-06-18 21:40:13.000000 aio-pygo-1.0.0/aio_pygo.egg-info/PKG-INFO
--rw-r--r--   0 gael       (501) staff       (20)      299 2023-06-18 21:40:13.000000 aio-pygo-1.0.0/aio_pygo.egg-info/SOURCES.txt
--rw-r--r--   0 gael       (501) staff       (20)        1 2023-06-18 21:40:13.000000 aio-pygo-1.0.0/aio_pygo.egg-info/dependency_links.txt
--rw-r--r--   0 gael       (501) staff       (20)        5 2023-06-18 21:40:13.000000 aio-pygo-1.0.0/aio_pygo.egg-info/top_level.txt
-drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:40:13.412832 aio-pygo-1.0.0/pygo/
--rw-r--r--   0 gael       (501) staff       (20)     1866 2023-06-04 10:53:21.000000 aio-pygo-1.0.0/pygo/chan.py
--rw-r--r--   0 gael       (501) staff       (20)     3896 2023-06-03 19:27:51.000000 aio-pygo-1.0.0/pygo/chan_test.py
--rw-r--r--   0 gael       (501) staff       (20)      100 2023-06-03 17:41:42.000000 aio-pygo-1.0.0/pygo/conftest.py
--rw-r--r--   0 gael       (501) staff       (20)      558 2023-06-03 19:33:52.000000 aio-pygo-1.0.0/pygo/defer.py
--rw-r--r--   0 gael       (501) staff       (20)      552 2023-06-03 19:36:11.000000 aio-pygo-1.0.0/pygo/defer_test.py
--rw-r--r--   0 gael       (501) staff       (20)      537 2023-06-03 20:09:47.000000 aio-pygo-1.0.0/pygo/go.py
--rw-r--r--   0 gael       (501) staff       (20)      590 2023-06-03 19:39:32.000000 aio-pygo-1.0.0/pygo/go_test.py
--rw-r--r--   0 gael       (501) staff       (20)      375 2023-06-18 19:59:45.000000 aio-pygo-1.0.0/pygo/time.py
--rw-r--r--   0 gael       (501) staff       (20)      336 2023-06-18 19:57:32.000000 aio-pygo-1.0.0/pygo/time_test.py
--rw-r--r--   0 gael       (501) staff       (20)      571 2023-06-18 21:40:01.000000 aio-pygo-1.0.0/pyproject.toml
--rw-r--r--   0 gael       (501) staff       (20)       38 2023-06-18 21:40:13.413461 aio-pygo-1.0.0/setup.cfg
+drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:51:16.832437 aio-pygo-1.0.1/
+-rw-r--r--   0 gael       (501) staff       (20)    35149 2023-05-31 17:21:41.000000 aio-pygo-1.0.1/LICENSE
+-rw-r--r--   0 gael       (501) staff       (20)     2874 2023-06-18 21:51:16.832284 aio-pygo-1.0.1/PKG-INFO
+-rw-r--r--   0 gael       (501) staff       (20)     2403 2023-06-18 21:42:02.000000 aio-pygo-1.0.1/README.md
+drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:51:16.829617 aio-pygo-1.0.1/aio_pygo.egg-info/
+-rw-r--r--   0 gael       (501) staff       (20)     2874 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/PKG-INFO
+-rw-r--r--   0 gael       (501) staff       (20)      316 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/SOURCES.txt
+-rw-r--r--   0 gael       (501) staff       (20)        1 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/dependency_links.txt
+-rw-r--r--   0 gael       (501) staff       (20)        5 2023-06-18 21:51:16.000000 aio-pygo-1.0.1/aio_pygo.egg-info/top_level.txt
+drwxr-xr-x   0 gael       (501) staff       (20)        0 2023-06-18 21:51:16.832086 aio-pygo-1.0.1/pygo/
+-rw-r--r--   0 gael       (501) staff       (20)      227 2023-06-18 21:48:05.000000 aio-pygo-1.0.1/pygo/__init__.py
+-rw-r--r--   0 gael       (501) staff       (20)     1866 2023-06-04 10:53:21.000000 aio-pygo-1.0.1/pygo/chan.py
+-rw-r--r--   0 gael       (501) staff       (20)     3896 2023-06-03 19:27:51.000000 aio-pygo-1.0.1/pygo/chan_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      100 2023-06-03 17:41:42.000000 aio-pygo-1.0.1/pygo/conftest.py
+-rw-r--r--   0 gael       (501) staff       (20)      558 2023-06-03 19:33:52.000000 aio-pygo-1.0.1/pygo/defer.py
+-rw-r--r--   0 gael       (501) staff       (20)      552 2023-06-03 19:36:11.000000 aio-pygo-1.0.1/pygo/defer_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      537 2023-06-03 20:09:47.000000 aio-pygo-1.0.1/pygo/go.py
+-rw-r--r--   0 gael       (501) staff       (20)      590 2023-06-03 19:39:32.000000 aio-pygo-1.0.1/pygo/go_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      375 2023-06-18 19:59:45.000000 aio-pygo-1.0.1/pygo/time.py
+-rw-r--r--   0 gael       (501) staff       (20)      336 2023-06-18 19:57:32.000000 aio-pygo-1.0.1/pygo/time_test.py
+-rw-r--r--   0 gael       (501) staff       (20)      571 2023-06-18 21:48:27.000000 aio-pygo-1.0.1/pyproject.toml
+-rw-r--r--   0 gael       (501) staff       (20)       38 2023-06-18 21:51:16.832483 aio-pygo-1.0.1/setup.cfg
```

### Comparing `aio-pygo-1.0.0/LICENSE` & `aio-pygo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/PKG-INFO` & `aio-pygo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pygo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Write Python code in a Go-like fashion.
 Author: Gael Lz
 Project-URL: Homepage, https://github.com/GaelLnz/pygo
 Project-URL: Bug Tracker, https://github.com/GaelLnz/pygo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aio-pygo-1.0.0/README.md` & `aio-pygo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/aio_pygo.egg-info/PKG-INFO` & `aio-pygo-1.0.1/aio_pygo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-pygo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Write Python code in a Go-like fashion.
 Author: Gael Lz
 Project-URL: Homepage, https://github.com/GaelLnz/pygo
 Project-URL: Bug Tracker, https://github.com/GaelLnz/pygo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aio-pygo-1.0.0/pygo/chan.py` & `aio-pygo-1.0.1/pygo/chan.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/pygo/chan_test.py` & `aio-pygo-1.0.1/pygo/chan_test.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/pygo/defer.py` & `aio-pygo-1.0.1/pygo/defer.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/pygo/defer_test.py` & `aio-pygo-1.0.1/pygo/defer_test.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/pygo/go.py` & `aio-pygo-1.0.1/pygo/go.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/pygo/go_test.py` & `aio-pygo-1.0.1/pygo/go_test.py`

 * *Files identical despite different names*

### Comparing `aio-pygo-1.0.0/pyproject.toml` & `aio-pygo-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aio-pygo"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Gael Lz" },
 ]
 description = "Write Python code in a Go-like fashion."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

