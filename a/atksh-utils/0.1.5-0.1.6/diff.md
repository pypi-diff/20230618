# Comparing `tmp/atksh-utils-0.1.5.tar.gz` & `tmp/atksh-utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.1.5.tar", last modified: Sun Jun 18 03:01:26 2023, max compression
+gzip compressed data, was "atksh-utils-0.1.6.tar", last modified: Sun Jun 18 04:49:26 2023, max compression
```

## Comparing `atksh-utils-0.1.5.tar` & `atksh-utils-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.251397 atksh-utils-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.251397 atksh-utils-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 03:01:26.000000 atksh-utils-0.1.5/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:01:26.255397 atksh-utils-0.1.5/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 03:01:16.000000 atksh-utils-0.1.5/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.882160 atksh-utils-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.882160 atksh-utils-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-18 04:49:26.000000 atksh-utils-0.1.6/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.882160 atksh-utils-0.1.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 04:49:26.886160 atksh-utils-0.1.6/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-18 04:49:16.000000 atksh-utils-0.1.6/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.1.5/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.1.6/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/.gitignore` & `atksh-utils-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/LICENSE` & `atksh-utils-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/PKG-INFO` & `atksh-utils-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -102,15 +102,35 @@
     :type b: int
     :return: The sum of a and b.
     :rtype: int
     """
     return a // b
 
 
+def exec_python_code(code: str) -> str:
+    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
+
+    :param code: A string of Python code.
+    :type code: str
+    :return: The result of the execution of the Python code (stdout by print)
+    :rtype: str
+    """
+    import tempfile
+    import subprocess
+    with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
+        f.write(code)
+        f.flush()
+        result = subprocess.check_output(["python", f.name])
+    result = result.decode("utf-8").strip()
+    if result == "":
+        result = "NotPrintedError('The result is not printed.')"
+    return result
+
 ai.set_function(mul)
 ai.set_function(add)
 ai.set_function(sub)
 ai.set_function(div)
+ai.set_function(exec_python_code)
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
 ```
```

### Comparing `atksh-utils-0.1.5/pyproject.toml` & `atksh-utils-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/src/atksh_utils/openai/api.py` & `atksh-utils-0.1.6/src/atksh_utils/openai/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,11 +238,20 @@
                 stream_callback=stream_callback,
             )[1]
 
         return analyze, plan, act
 
     def set_react_functions(self, stream_callback=None, model_name=None):
         """Adds three OpenAI agents"""
-        analyzer, planner, actor = self._create_react_functions(stream_callback, model_name=None)
-        self.set_function(analyzer)
-        self.set_function(planner)
-        self.set_function(actor)
+        analyze, plan, act = self._create_react_functions(stream_callback, model_name=None)
+        self.add_instructions(
+            "First, call `analyze` function to identify the goal state, the current state, and the summary of the current situation and the context."
+        )
+        self.add_instructions(
+            "Second, call `plan` function to plan the sequence of actions to achieve the goal state from the current state."
+        )
+        self.add_instructions(
+            "Then, call `act` function to act the action in the current state and the summary or call any other functions."
+        )
+        self.set_function(analyze)
+        self.set_function(plan)
+        self.set_function(act)
```

### Comparing `atksh-utils-0.1.5/src/atksh_utils/openai/functional.py` & `atksh-utils-0.1.6/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.1.6/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.1.6/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.1.5
+Version: 0.1.6
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
         
@@ -102,15 +102,35 @@
     :type b: int
     :return: The sum of a and b.
     :rtype: int
     """
     return a // b
 
 
+def exec_python_code(code: str) -> str:
+    """This is a function that executes Python code and returns the stdout. Don't forget to print the result.
+
+    :param code: A string of Python code.
+    :type code: str
+    :return: The result of the execution of the Python code (stdout by print)
+    :rtype: str
+    """
+    import tempfile
+    import subprocess
+    with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as f:
+        f.write(code)
+        f.flush()
+        result = subprocess.check_output(["python", f.name])
+    result = result.decode("utf-8").strip()
+    if result == "":
+        result = "NotPrintedError('The result is not printed.')"
+    return result
+
 ai.set_function(mul)
 ai.set_function(add)
 ai.set_function(sub)
 ai.set_function(div)
+ai.set_function(exec_python_code)
 
 print(ai("Just answer the value of (5243 + 642) x (5314 - 4231) // 100"))
 # The value of (5243 + 642) x (5314 - 4231) // 100 is 63734.
 ```
```

### Comparing `atksh-utils-0.1.5/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.1.6/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/tests/openai/test_api.py` & `atksh-utils-0.1.6/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.1.5/tests/openai/test_functional.py` & `atksh-utils-0.1.6/tests/openai/test_functional.py`

 * *Files identical despite different names*

