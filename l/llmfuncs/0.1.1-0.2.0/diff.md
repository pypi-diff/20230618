# Comparing `tmp/llmfuncs-0.1.1.tar.gz` & `tmp/llmfuncs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfuncs-0.1.1.tar", last modified: Sat Jun 17 23:32:38 2023, max compression
+gzip compressed data, was "llmfuncs-0.2.0.tar", last modified: Sun Jun 18 05:08:33 2023, max compression
```

## Comparing `llmfuncs-0.1.1.tar` & `llmfuncs-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.178808 llmfuncs-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-17 23:32:38.178808 llmfuncs-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 23:32:38.178808 llmfuncs-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/src/llmfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/src/llmfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/src/llmfuncs/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/src/llmfuncs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/src/llmfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/src/llmfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/src/llmfuncs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/src/llmfuncs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/src/llmfuncs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/tests/test_schema.py
```

### Comparing `llmfuncs-0.1.1/LICENSE` & `llmfuncs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.1.1/PKG-INFO` & `llmfuncs-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.1.1
+Version: 0.2.0
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,22 +40,33 @@
 
 If you have an existing module that you want to work with `llmfuncs`, you can try passing it through an LLM
 to generate the type hints and docstrings for any functions missing them. For example:
 ```
 Please update this module to add type hints to all function parameters and Google style docstrings to each function.
 ```
 
-
 ## Features
 
 - Extracts function name, description (from docstring), parameters, and their types
 - Includes default values for parameters in the description
 - Supports functions with arguments that have type hints
 - Converts Python types to corresponding JSON schema types
 
+## Validating Arguments and Calling Functions
+```python
+from llmfuncs import schema, validator
+
+def my_function(x: int, y: int) -> int:
+    return x + y
+
+schema = schema.from_function(my_function)
+args = {"x": 10, "y": 20}
+result = validator.call_function_with_validation(schema, my_function, args)
+```
+
 ## Contributing
 
 To contribute to `llmfuncs`, fork the repository and submit a Pull Request!
 
 ## License
 
 MIT
```

### Comparing `llmfuncs-0.1.1/README.md` & `llmfuncs-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,22 +29,33 @@
 
 If you have an existing module that you want to work with `llmfuncs`, you can try passing it through an LLM
 to generate the type hints and docstrings for any functions missing them. For example:
 ```
 Please update this module to add type hints to all function parameters and Google style docstrings to each function.
 ```
 
-
 ## Features
 
 - Extracts function name, description (from docstring), parameters, and their types
 - Includes default values for parameters in the description
 - Supports functions with arguments that have type hints
 - Converts Python types to corresponding JSON schema types
 
+## Validating Arguments and Calling Functions
+```python
+from llmfuncs import schema, validator
+
+def my_function(x: int, y: int) -> int:
+    return x + y
+
+schema = schema.from_function(my_function)
+args = {"x": 10, "y": 20}
+result = validator.call_function_with_validation(schema, my_function, args)
+```
+
 ## Contributing
 
 To contribute to `llmfuncs`, fork the repository and submit a Pull Request!
 
 ## License
 
-MIT
+MIT
```

### Comparing `llmfuncs-0.1.1/src/llmfuncs.egg-info/PKG-INFO` & `llmfuncs-0.2.0/src/llmfuncs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.1.1
+Version: 0.2.0
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -40,22 +40,33 @@
 
 If you have an existing module that you want to work with `llmfuncs`, you can try passing it through an LLM
 to generate the type hints and docstrings for any functions missing them. For example:
 ```
 Please update this module to add type hints to all function parameters and Google style docstrings to each function.
 ```
 
-
 ## Features
 
 - Extracts function name, description (from docstring), parameters, and their types
 - Includes default values for parameters in the description
 - Supports functions with arguments that have type hints
 - Converts Python types to corresponding JSON schema types
 
+## Validating Arguments and Calling Functions
+```python
+from llmfuncs import schema, validator
+
+def my_function(x: int, y: int) -> int:
+    return x + y
+
+schema = schema.from_function(my_function)
+args = {"x": 10, "y": 20}
+result = validator.call_function_with_validation(schema, my_function, args)
+```
+
 ## Contributing
 
 To contribute to `llmfuncs`, fork the repository and submit a Pull Request!
 
 ## License
 
 MIT
```

### Comparing `llmfuncs-0.1.1/tests/test_schema.py` & `llmfuncs-0.2.0/tests/test_schema.py`

 * *Files identical despite different names*

