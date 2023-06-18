# Comparing `tmp/autonomy_dev-0.1.4.tar.gz` & `tmp/autonomy_dev-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.4.tar", max compression
+gzip compressed data, was "autonomy_dev-0.1.5.tar", max compression
```

## Comparing `autonomy_dev-0.1.4.tar` & `autonomy_dev-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      578 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/LICENSE
--rw-r--r--   0        0        0      117 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/__init__.py
--rw-r--r--   0        0        0     3151 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/cli.py
--rw-r--r--   0        0        0     2732 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/cli_executor.py
--rw-r--r--   0        0        0      301 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/constants.py
--rw-r--r--   0        0        0      577 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      464 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/test.py
--rw-r--r--   0        0        0     1083 2023-05-28 17:46:15.829622 autonomy_dev-0.1.4/auto_dev/utils.py
--rw-r--r--   0        0        0     2518 2023-05-28 17:46:15.833622 autonomy_dev-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1187 2023-05-28 17:46:15.833622 autonomy_dev-0.1.4/tests/test_cli.py
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 autonomy_dev-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/LICENSE
+-rw-r--r--   0        0        0      117 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/__init__.py
+-rw-r--r--   0        0        0     3151 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/cli.py
+-rw-r--r--   0        0        0     2732 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0      301 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/constants.py
+-rw-r--r--   0        0        0      629 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      464 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/lint.py
+-rw-r--r--   0        0        0      438 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/test.py
+-rw-r--r--   0        0        0     1083 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/utils.py
+-rw-r--r--   0        0        0     2518 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1187 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/tests/test_cli.py
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 autonomy_dev-0.1.5/PKG-INFO
```

### Comparing `autonomy_dev-0.1.4/LICENSE` & `autonomy_dev-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.4/auto_dev/cli.py` & `autonomy_dev-0.1.5/auto_dev/cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.4/auto_dev/cli_executor.py` & `autonomy_dev-0.1.5/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.4/auto_dev/data/pylama.ini` & `autonomy_dev-0.1.5/auto_dev/data/pylama.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [pylama]
 format = pylint
 skip = */.tox/*,*/.env/*,*/__pycache__/*
 
-linters = mypy,pylint,eradicate,radon,vulture,isort
+linters = pylint,eradicate,radon,vulture,isort
 max-complexity = 18
 ignore = E203, E266, W503, R0913, W0621, W1203,R0901,E5110,R0903
 max_line_length = 120
 docstring-convention = google
 per-file-ignores = __init__.py:F401
 exclude = .git,
     __pycache__,
@@ -23,12 +23,13 @@
     .github,
     .history,
     .idea
 
 [pylama:vulture]
 min-confidence = 90
 
-
 [pylama:mypy]
 ignore_missing_imports = True
-
-
+strict = False
+exclude =
+    .*_pb2\.py$
+    .*message\.py$
```

### Comparing `autonomy_dev-0.1.4/auto_dev/utils.py` & `autonomy_dev-0.1.5/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.4/pyproject.toml` & `autonomy_dev-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `autonomy_dev-0.1.4/tests/test_cli.py` & `autonomy_dev-0.1.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.4/PKG-INFO` & `autonomy_dev-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

