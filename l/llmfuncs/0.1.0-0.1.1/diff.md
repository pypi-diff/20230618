# Comparing `tmp/llmfuncs-0.1.0.tar.gz` & `tmp/llmfuncs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfuncs-0.1.0.tar", last modified: Fri Jun 16 08:00:15 2023, max compression
+gzip compressed data, was "llmfuncs-0.1.1.tar", last modified: Sat Jun 17 23:32:38 2023, max compression
```

## Comparing `llmfuncs-0.1.0.tar` & `llmfuncs-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-16 07:59:58.000000 llmfuncs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-16 07:59:58.000000 llmfuncs-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-16 07:59:58.000000 llmfuncs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/src/llmfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:59:58.000000 llmfuncs-0.1.0/src/llmfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-16 07:59:58.000000 llmfuncs-0.1.0/src/llmfuncs/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/src/llmfuncs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-16 08:00:15.000000 llmfuncs-0.1.0/src/llmfuncs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-16 08:00:15.000000 llmfuncs-0.1.0/src/llmfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:00:15.000000 llmfuncs-0.1.0/src/llmfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 08:00:15.000000 llmfuncs-0.1.0/src/llmfuncs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 08:00:15.000000 llmfuncs-0.1.0/src/llmfuncs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:00:15.504644 llmfuncs-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-16 07:59:58.000000 llmfuncs-0.1.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.178808 llmfuncs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-17 23:32:38.178808 llmfuncs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 23:32:38.178808 llmfuncs-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/src/llmfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/src/llmfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/src/llmfuncs/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/src/llmfuncs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 23:32:38.000000 llmfuncs-0.1.1/src/llmfuncs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:32:38.174808 llmfuncs-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-17 23:32:28.000000 llmfuncs-0.1.1/tests/test_schema.py
```

### Comparing `llmfuncs-0.1.0/LICENSE` & `llmfuncs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.1.0/PKG-INFO` & `llmfuncs-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: llmfuncs
-Version: 0.1.0
-Summary: Dynamically generate JSON Schema from Python code.
-Home-page: https://github.com/FyZyX/llmfuncs
-Author: Lucas Lofaro
-Author-email: lucasmlofaro@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # llmfuncs
 
 `llmfuncs` is a Python package that programmatically extracts function definitions and converts them to a JSON schema format that can be used with OpenAI's language models.
 
 ## Installation
 
 You can install the package via pip:
@@ -26,26 +15,36 @@
 Import the main function `schema_from_module` from `llmfuncs` and pass in a module:
 
 ```python
 from llmfuncs import schema
 import your_module
 
 schema = schema.from_module(your_module)
-
 ```
 
+> **NOTE:** If your function parameters don't have type hints, they will be ignored!
+
 The returned `schema` will be a list of JSON schema representations of the functions in the given module.
 
+## Creating New Tools
+
+If you have an existing module that you want to work with `llmfuncs`, you can try passing it through an LLM
+to generate the type hints and docstrings for any functions missing them. For example:
+```
+Please update this module to add type hints to all function parameters and Google style docstrings to each function.
+```
+
+
 ## Features
 
 - Extracts function name, description (from docstring), parameters, and their types
 - Includes default values for parameters in the description
 - Supports functions with arguments that have type hints
 - Converts Python types to corresponding JSON schema types
 
 ## Contributing
 
 To contribute to `llmfuncs`, fork the repository and submit a Pull Request!
 
 ## License
 
-MIT
+MIT
```

### Comparing `llmfuncs-0.1.0/setup.py` & `llmfuncs-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="llmfuncs",
-    version="0.1.0",
+    version="0.1.1",
     url="https://github.com/FyZyX/llmfuncs",
     author="Lucas Lofaro",
     author_email="lucasmlofaro@gmail.com",
     description="Dynamically generate JSON Schema from Python code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `llmfuncs-0.1.0/src/llmfuncs.egg-info/PKG-INFO` & `llmfuncs-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,19 +26,29 @@
 Import the main function `schema_from_module` from `llmfuncs` and pass in a module:
 
 ```python
 from llmfuncs import schema
 import your_module
 
 schema = schema.from_module(your_module)
-
 ```
 
+> **NOTE:** If your function parameters don't have type hints, they will be ignored!
+
 The returned `schema` will be a list of JSON schema representations of the functions in the given module.
 
+## Creating New Tools
+
+If you have an existing module that you want to work with `llmfuncs`, you can try passing it through an LLM
+to generate the type hints and docstrings for any functions missing them. For example:
+```
+Please update this module to add type hints to all function parameters and Google style docstrings to each function.
+```
+
+
 ## Features
 
 - Extracts function name, description (from docstring), parameters, and their types
 - Includes default values for parameters in the description
 - Supports functions with arguments that have type hints
 - Converts Python types to corresponding JSON schema types
```

