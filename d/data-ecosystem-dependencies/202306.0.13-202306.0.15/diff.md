# Comparing `tmp/data_ecosystem_dependencies-202306.0.13.tar.gz` & `tmp/data_ecosystem_dependencies-202306.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202306.0.13.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202306.0.15.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202306.0.13.tar` & `data_ecosystem_dependencies-202306.0.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-06-17 14:22:41.784976 data_ecosystem_dependencies-202306.0.13/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-06-17 14:22:41.784976 data_ecosystem_dependencies-202306.0.13/license.md
--rw-r--r--   0        0        0     2740 2023-06-17 14:26:16.637386 data_ecosystem_dependencies-202306.0.13/pyproject.toml
--rw-r--r--   0        0        0      341 2023-06-17 14:22:41.784976 data_ecosystem_dependencies-202306.0.13/readme.md
--rw-r--r--   0        0        0      160 2023-06-17 14:22:41.784976 data_ecosystem_dependencies-202306.0.13/setup.cfg
--rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.13/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-06-18 02:59:16.360164 data_ecosystem_dependencies-202306.0.15/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-06-18 02:59:16.360164 data_ecosystem_dependencies-202306.0.15/license.md
+-rw-r--r--   0        0        0     2740 2023-06-18 03:03:11.890695 data_ecosystem_dependencies-202306.0.15/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-06-18 02:59:16.360164 data_ecosystem_dependencies-202306.0.15/readme.md
+-rw-r--r--   0        0        0      160 2023-06-18 02:59:16.360164 data_ecosystem_dependencies-202306.0.15/setup.cfg
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.15/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202306.0.13/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202306.0.15/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.13/license.md` & `data_ecosystem_dependencies-202306.0.15/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.13/pyproject.toml` & `data_ecosystem_dependencies-202306.0.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202306.0.13"
+version="202306.0.15"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
```

### Comparing `data_ecosystem_dependencies-202306.0.13/PKG-INFO` & `data_ecosystem_dependencies-202306.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202306.0.13
+Version: 202306.0.15
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

