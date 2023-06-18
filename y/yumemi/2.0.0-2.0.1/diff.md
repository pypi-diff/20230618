# Comparing `tmp/yumemi-2.0.0.tar.gz` & `tmp/yumemi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yumemi-2.0.0.tar", max compression
+gzip compressed data, was "yumemi-2.0.1.tar", max compression
```

## Comparing `yumemi-2.0.0.tar` & `yumemi-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,16 @@
--rw-r--r--   0        0        0     1071 2022-12-10 18:19:04.687736 yumemi-2.0.0/LICENSE
--rw-r--r--   0        0        0      416 2022-12-11 10:45:58.455509 yumemi-2.0.0/README.rst
--rw-r--r--   0        0        0     1529 2023-01-07 14:22:24.027986 yumemi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      284 2022-12-11 10:45:58.456508 yumemi-2.0.0/src/yumemi/__init__.py
--rw-r--r--   0        0        0    10557 2022-12-11 16:02:11.815902 yumemi-2.0.0/src/yumemi/anidb.py
--rw-r--r--   0        0        0     4069 2023-01-07 13:00:22.074885 yumemi-2.0.0/src/yumemi/cli.py
--rw-r--r--   0        0        0      592 2022-12-11 16:02:11.815902 yumemi-2.0.0/src/yumemi/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-07 14:31:53.120726 yumemi-2.0.0/src/yumemi/py.typed
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 yumemi-2.0.0/setup.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 yumemi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-18 14:44:10.352719 yumemi-2.0.1/LICENSE
+-rw-r--r--   0        0        0      416 2023-06-18 14:44:10.352719 yumemi-2.0.1/README.rst
+-rw-r--r--   0        0        0      921 2023-06-18 14:44:10.352719 yumemi-2.0.1/docs/api.rst
+-rw-r--r--   0        0        0       70 2023-06-18 14:44:10.352719 yumemi-2.0.1/docs/cli.rst
+-rw-r--r--   0        0        0     1326 2023-06-18 14:44:10.352719 yumemi-2.0.1/docs/conf.py
+-rw-r--r--   0        0        0      491 2023-06-18 14:44:10.352719 yumemi-2.0.1/docs/index.rst
+-rw-r--r--   0        0        0     1565 2023-06-18 14:44:10.352719 yumemi-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      284 2023-06-18 14:44:10.352719 yumemi-2.0.1/src/yumemi/__init__.py
+-rw-r--r--   0        0        0    10557 2023-06-18 14:44:10.352719 yumemi-2.0.1/src/yumemi/anidb.py
+-rw-r--r--   0        0        0     4069 2023-06-18 14:44:10.352719 yumemi-2.0.1/src/yumemi/cli.py
+-rw-r--r--   0        0        0      592 2023-06-18 14:44:10.352719 yumemi-2.0.1/src/yumemi/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-18 14:44:10.352719 yumemi-2.0.1/src/yumemi/py.typed
+-rw-r--r--   0        0        0        0 2023-06-18 14:44:10.352719 yumemi-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3351 2023-06-18 14:44:10.352719 yumemi-2.0.1/tests/test_anidb.py
+-rw-r--r--   0        0        0     2529 2023-06-18 14:44:10.352719 yumemi-2.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 yumemi-2.0.1/PKG-INFO
```

### Comparing `yumemi-2.0.0/LICENSE` & `yumemi-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.0/pyproject.toml` & `yumemi-2.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "yumemi"
-version = "2.0.0"
-description = "AniDB library and simple CLI client."
+version = "2.0.1"
+description = "AniDB API library for Python and simple CLI client"
 readme = "README.rst"
 authors = ["Filip Pobořil <tsuki@fpob.cz>"]
 license = "MIT"
-repository = "https://gitlab.com/fpob-dev/yumemi"
-documentation = "https://fpob-dev.gitlab.io/yumemi/"
+repository = "https://github.com/fpob/yumemi"
+documentation = "https://yumemi.readthedocs.io/"
 keywords = ["AniDB"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Intended Audience :: Developers",
   "Intended Audience :: End Users/Desktop",
   "Topic :: Utilities",
 ]
+include = ["tests", "docs"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1"
 attrs = "^22.1"
-cryptography = "^38.0"
+cryptography = "^39.0.1"
 rhash-rhash = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
 mypy = "^0.991"
 pyproject-flake8 = "^6.0.0"
 flake8-bugbear = "^22.12.6"
 flake8-isort = "^5.0.3"
 isort = "^5.10.1"
-furo = "^2022.12.7"
+furo = "^2023.3.27"
 sphinx = "^5.3.0"
 sphinx-click = "^4.4.0"
 poethepoet = "^0.16.5"
 
 [tool.poetry.scripts]
 yumemi = "yumemi.cli:main"
```

### Comparing `yumemi-2.0.0/src/yumemi/anidb.py` & `yumemi-2.0.1/src/yumemi/anidb.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.0/src/yumemi/cli.py` & `yumemi-2.0.1/src/yumemi/cli.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.0/src/yumemi/exceptions.py` & `yumemi-2.0.1/src/yumemi/exceptions.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.0/PKG-INFO` & `yumemi-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: yumemi
-Version: 2.0.0
-Summary: AniDB library and simple CLI client.
-Home-page: https://gitlab.com/fpob-dev/yumemi
+Version: 2.0.1
+Summary: AniDB API library for Python and simple CLI client
+Home-page: https://github.com/fpob/yumemi
 License: MIT
 Keywords: AniDB
 Author: Filip Pobořil
 Author-email: tsuki@fpob.cz
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -16,18 +16,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: attrs (>=22.1,<23.0)
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: cryptography (>=38.0,<39.0)
+Requires-Dist: cryptography (>=39.0.1,<40.0.0)
 Requires-Dist: rhash-rhash (>=1.1,<2.0)
-Project-URL: Documentation, https://fpob-dev.gitlab.io/yumemi/
-Project-URL: Repository, https://gitlab.com/fpob-dev/yumemi
+Project-URL: Documentation, https://yumemi.readthedocs.io/
+Project-URL: Repository, https://github.com/fpob/yumemi
 Description-Content-Type: text/x-rst
 
 Yumemi
 ======
 
 AniDB API library for Python and simple CLI client to add files to mylist.
```

