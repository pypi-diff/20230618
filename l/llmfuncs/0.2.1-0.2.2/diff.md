# Comparing `tmp/llmfuncs-0.2.1.tar.gz` & `tmp/llmfuncs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfuncs-0.2.1.tar", last modified: Sun Jun 18 05:25:45 2023, max compression
+gzip compressed data, was "llmfuncs-0.2.2.tar", last modified: Sun Jun 18 05:32:08 2023, max compression
```

## Comparing `llmfuncs-0.2.1.tar` & `llmfuncs-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.862763 llmfuncs-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.862763 llmfuncs-0.2.1/src/llmfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/src/llmfuncs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/src/llmfuncs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 05:25:45.000000 llmfuncs-0.2.1/src/llmfuncs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:25:45.866763 llmfuncs-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-18 05:25:30.000000 llmfuncs-0.2.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.546379 llmfuncs-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:32:08.546379 llmfuncs-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/src/llmfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/src/llmfuncs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/tests/test_schema.py
```

### Comparing `llmfuncs-0.2.1/LICENSE` & `llmfuncs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.1/PKG-INFO` & `llmfuncs-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llmfuncs-0.2.1/README.md` & `llmfuncs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.1/setup.py` & `llmfuncs-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="llmfuncs",
-    version="0.2.1",
+    version="0.2.2",
     url="https://github.com/FyZyX/llmfuncs",
     author="Lucas Lofaro",
     author_email="lucasmlofaro@gmail.com",
     description="Dynamically generate JSON Schema from Python code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `llmfuncs-0.2.1/src/llmfuncs/schema.py` & `llmfuncs-0.2.2/src/llmfuncs/schema.py`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.1/src/llmfuncs/tool.py` & `llmfuncs-0.2.2/src/llmfuncs/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             func_schema["return"] = schema_type
 
         return func_schema
 
 
 class ToolCollection:
     def __init__(self, tools: typing.List[Tool] = None):
-        self._tools = {}
+        self._tools: typing.Dict[str, Tool] = {}
         for tool in tools or []:
             self.add_tool(tool)
 
     def __len__(self):
         return len(self._tools)
 
     def add_tool(self, tool: Tool):
@@ -124,16 +124,15 @@
             self.add_tools_from_module(path.absolute())
 
     def use_tool(self, tool_name: str, json_args: str | typing.Mapping) -> typing.Any:
         tool = self._tools.get(tool_name)
         if not tool:
             raise ValueError(f"No tool found with name: {tool_name}")
 
-        func = tool['function']
-        params_schema = tool['schema']['parameters']
+        params_schema = tool.schema()['parameters']
         is_string = isinstance(json_args, str)
         args = validator.parse_json(json_args) if is_string else json_args
         validator.validate_args_with_schema(args, params_schema)
-        return func(**args)
+        return tool(**args)
 
     def schema(self) -> typing.List[schema.JsonSchema]:
         return [tool.schema() for tool in self._tools.values()]
```

### Comparing `llmfuncs-0.2.1/src/llmfuncs/validator.py` & `llmfuncs-0.2.2/src/llmfuncs/validator.py`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.1/src/llmfuncs.egg-info/PKG-INFO` & `llmfuncs-0.2.2/src/llmfuncs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llmfuncs-0.2.1/tests/test_schema.py` & `llmfuncs-0.2.2/tests/test_schema.py`

 * *Files identical despite different names*

