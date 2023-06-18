# Comparing `tmp/autonomy_dev-0.1.5.tar.gz` & `tmp/autonomy_dev-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.5.tar", max compression
+gzip compressed data, was "autonomy_dev-0.1.6.tar", max compression
```

## Comparing `autonomy_dev-0.1.5.tar` & `autonomy_dev-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      578 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/LICENSE
--rw-r--r--   0        0        0      117 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/__init__.py
--rw-r--r--   0        0        0     3151 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/cli.py
--rw-r--r--   0        0        0     2732 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/cli_executor.py
--rw-r--r--   0        0        0      301 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/constants.py
--rw-r--r--   0        0        0      629 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      464 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/test.py
--rw-r--r--   0        0        0     1083 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/auto_dev/utils.py
--rw-r--r--   0        0        0     2518 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1187 2023-06-18 13:49:52.178465 autonomy_dev-0.1.5/tests/test_cli.py
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 autonomy_dev-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/__init__.py
+-rw-r--r--   0        0        0     3151 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/cli.py
+-rw-r--r--   0        0        0     2822 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0      301 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/constants.py
+-rw-r--r--   0        0        0      642 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      464 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/lint.py
+-rw-r--r--   0        0        0      438 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/test.py
+-rw-r--r--   0        0        0     1083 2023-06-18 14:35:10.770490 autonomy_dev-0.1.6/auto_dev/utils.py
+-rw-r--r--   0        0        0     2518 2023-06-18 14:35:10.774490 autonomy_dev-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1187 2023-06-18 14:35:10.774490 autonomy_dev-0.1.6/tests/test_cli.py
+-rw-r--r--   0        0        0     2569 1970-01-01 00:00:00.000000 autonomy_dev-0.1.6/PKG-INFO
```

### Comparing `autonomy_dev-0.1.5/LICENSE` & `autonomy_dev-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.5/auto_dev/cli.py` & `autonomy_dev-0.1.6/auto_dev/cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.5/auto_dev/cli_executor.py` & `autonomy_dev-0.1.6/auto_dev/cli_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This is a simple command execution class.
 It is used to execute commands in a subprocess and return the output.
 It is also used to check if a command was successful or not.
 It is used by the lint and test functions.
 
 """
 
+import os
 import subprocess
 from typing import List, Optional, Union
 
 from .utils import get_logger
 
 logger = get_logger()
 
@@ -25,15 +26,19 @@
     def execute(self, stream=False, verbose: bool = True):
         """Execute the command."""
         if stream:
             return self._execute_stream(verbose)
         logger.debug(f"Executing command:\n\"\"\n{' '.join(self.command)}\n\"\"")
         try:
             result = subprocess.run(
-                self.command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=self.cwd, check=False
+                self.command,
+                stdout=subprocess.PIPE,
+                stderr=subprocess.PIPE,
+                cwd=self.cwd, check=False,
+                env=os.environ
             )
             if verbose:
                 if len(result.stdout) > 0:
                     logger.info(result.stdout.decode("utf-8"))
                 if len(result.stderr) > 0:
                     logger.error(result.stderr.decode("utf-8"))
```

### Comparing `autonomy_dev-0.1.5/auto_dev/data/pylama.ini` & `autonomy_dev-0.1.6/auto_dev/data/pylama.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [pylama]
 format = pylint
-skip = */.tox/*,*/.env/*,*/__pycache__/*
+skip = */.tox/*,
+    */.env/*,
+    */__pycache__/*
+    **/*_pb2.py
 
 linters = pylint,eradicate,radon,vulture,isort
 max-complexity = 18
 ignore = E203, E266, W503, R0913, W0621, W1203,R0901,E5110,R0903
 max_line_length = 120
 docstring-convention = google
 per-file-ignores = __init__.py:F401
@@ -20,16 +23,17 @@
     .mypy_cache,
     .pytest_cache,
     .vscode,
     .github,
     .history,
     .idea
 
+
 [pylama:vulture]
 min-confidence = 90
 
 [pylama:mypy]
 ignore_missing_imports = True
 strict = False
-exclude =
-    .*_pb2\.py$
-    .*message\.py$
+
+[pylama:radon]
+complexity = 18
```

### Comparing `autonomy_dev-0.1.5/auto_dev/utils.py` & `autonomy_dev-0.1.6/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.5/pyproject.toml` & `autonomy_dev-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.5"
+version = "0.1.6"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `autonomy_dev-0.1.5/tests/test_cli.py` & `autonomy_dev-0.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.5/PKG-INFO` & `autonomy_dev-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.5
+Version: 0.1.6
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -51,8 +51,18 @@
 Tooling to speed up autonomy development.
 
 # Installation
 
 ```bash
 pip install autonomy-dev[all]
 ```
+# Release
+bump the version in pyoproject and create a new branch and tag
 
+```bash
+export new_version=v0.1.5
+git checkout -b $new_version
+git add .
+git tag $new_version
+git push --set-upstream origin (git rev-parse --abbrev-ref HEAD)
+git push --tag
+```
```

