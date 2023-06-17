# Comparing `tmp/prefecto-0.0.1.tar.gz` & `tmp/prefecto-0.0.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefecto-0.0.1.tar", last modified: Sat Jun 17 19:39:22 2023, max compression
+gzip compressed data, was "prefecto-0.0.1.post0.tar", last modified: Sat Jun 17 22:18:06 2023, max compression
```

## Comparing `prefecto-0.0.1.tar` & `prefecto-0.0.1.post0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:39:22.408808 prefecto-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-17 19:38:33.000000 prefecto-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-17 19:39:22.408808 prefecto-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 19:38:33.000000 prefecto-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-17 19:38:33.000000 prefecto-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-17 19:39:22.408808 prefecto-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-17 19:38:33.000000 prefecto-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:39:22.404808 prefecto-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:39:22.408808 prefecto-0.0.1/src/prefecto/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-17 19:39:22.408808 prefecto-0.0.1/src/prefecto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:39:22.408808 prefecto-0.0.1/src/prefecto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/serializers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/serializers/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/serializers/polars.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 19:38:33.000000 prefecto-0.0.1/src/prefecto/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:39:22.408808 prefecto-0.0.1/src/prefecto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-17 19:39:22.000000 prefecto-0.0.1/src/prefecto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-17 19:39:22.000000 prefecto-0.0.1/src/prefecto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:39:22.000000 prefecto-0.0.1/src/prefecto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-17 19:39:22.000000 prefecto-0.0.1/src/prefecto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 19:39:22.000000 prefecto-0.0.1/src/prefecto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:38:44.000000 prefecto-0.0.1/src/prefecto.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:39:22.408808 prefecto-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 19:38:33.000000 prefecto-0.0.1/tests/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-17 19:38:33.000000 prefecto-0.0.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-17 19:38:33.000000 prefecto-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/serializers/polars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/src/prefecto/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/src/prefecto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 22:18:06.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:17:32.000000 prefecto-0.0.1.post0/src/prefecto.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:18:06.132142 prefecto-0.0.1.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/tests/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-17 22:17:26.000000 prefecto-0.0.1.post0/versioneer.py
```

### Comparing `prefecto-0.0.1/LICENSE` & `prefecto-0.0.1.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/pyproject.toml` & `prefecto-0.0.1.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/setup.py` & `prefecto-0.0.1.post0/setup.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto/concurrency.py` & `prefecto-0.0.1.post0/src/prefecto/concurrency.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto/logging.py` & `prefecto-0.0.1.post0/src/prefecto/logging.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto/serializers/core.py` & `prefecto-0.0.1.post0/src/prefecto/serializers/core.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto/serializers/pandas.py` & `prefecto-0.0.1.post0/src/prefecto/serializers/pandas.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto/serializers/polars.py` & `prefecto-0.0.1.post0/src/prefecto/serializers/polars.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto/states.py` & `prefecto-0.0.1.post0/src/prefecto/states.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/src/prefecto.egg-info/SOURCES.txt` & `prefecto-0.0.1.post0/src/prefecto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/tests/test_concurrency.py` & `prefecto-0.0.1.post0/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `prefecto-0.0.1/versioneer.py` & `prefecto-0.0.1.post0/versioneer.py`

 * *Files identical despite different names*

