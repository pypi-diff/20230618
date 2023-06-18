# Comparing `tmp/llmfuncs-0.2.0.tar.gz` & `tmp/llmfuncs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfuncs-0.2.0.tar", last modified: Sun Jun 18 05:08:33 2023, max compression
+gzip compressed data, was "llmfuncs-0.2.1.tar", last modified: Sun Jun 18 05:25:45 2023, max compression
```

## Comparing `llmfuncs-0.2.0.tar` & `llmfuncs-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/src/llmfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/src/llmfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/src/llmfuncs/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/src/llmfuncs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/src/llmfuncs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 05:08:33.000000 llmfuncs-0.2.0/src/llmfuncs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:08:33.182496 llmfuncs-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-18 05:08:23.000000 llmfuncs-0.2.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.862763 llmfuncs-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.862763 llmfuncs-0.2.1/src/llmfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/src/llmfuncs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/tests/test_schema.py
```

### Comparing `llmfuncs-0.2.0/LICENSE` & `llmfuncs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.0/setup.py` & `llmfuncs-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="llmfuncs",
-    version="0.2.0",
+    version="0.2.1",
     url="https://github.com/FyZyX/llmfuncs",
     author="Lucas Lofaro",
     author_email="lucasmlofaro@gmail.com",
     description="Dynamically generate JSON Schema from Python code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `llmfuncs-0.2.0/tests/test_schema.py` & `llmfuncs-0.2.1/tests/test_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import types
 import unittest
 from typing import List, Optional
 
-from llmfuncs.schema import from_module
+from llmfuncs.tool import ToolCollection
 
 import example
 
 
 def test_function1(x: int, y: str = "hello") -> str:
     """This is a test function.
 
@@ -37,18 +37,19 @@
 dummy_module = types.ModuleType("dummy_module")
 dummy_module.test_function1 = test_function1
 dummy_module.test_function2 = test_function2
 
 
 class TestSchemaExtraction(unittest.TestCase):
     def test_schema_from_module(self):
-        schema = from_module(dummy_module)
-        self.assertEqual(len(schema), 2)
+        collection = ToolCollection()
+        collection.add_tools_from_module(dummy_module)
+        self.assertEqual(len(collection), 2)
 
-        schema_dict = {s["name"]: s for s in schema}
+        schema_dict = {s["name"]: s for s in collection.schema()}
 
         self.assertIn("test_function1", schema_dict)
         self.assertIn("test_function2", schema_dict)
 
         schema1 = schema_dict["test_function1"]
         self.assertEqual(schema1["description"], "This is a test function.")
         self.assertIn("parameters", schema1)
@@ -58,15 +59,17 @@
         schema2 = schema_dict["test_function2"]
         self.assertEqual(schema2["description"], "This is another test function.")
         self.assertIn("parameters", schema2)
         self.assertIn("a", schema2["parameters"]["properties"])
         self.assertEqual(schema2["parameters"]["properties"]["a"]["type"], "number")
 
     def test_schema_from_module_example(self):
-        actual_schema = from_module(example)
+        collection = ToolCollection()
+        collection.add_tools_from_module(example)
+        actual_schema = collection.schema()
         expected_schema = [
             {
                 "name": "append_file",
                 "description": "Appends content to a file.",
                 "parameters": {
                     "type": "object",
                     "properties": {
```

