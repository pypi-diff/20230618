# Comparing `tmp/llmfuncs-0.2.2.tar.gz` & `tmp/llmfuncs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmfuncs-0.2.2.tar", last modified: Sun Jun 18 05:32:08 2023, max compression
+gzip compressed data, was "llmfuncs-0.2.3.tar", last modified: Sun Jun 18 09:45:53 2023, max compression
```

## Comparing `llmfuncs-0.2.2.tar` & `llmfuncs-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.546379 llmfuncs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:32:08.546379 llmfuncs-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/src/llmfuncs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/src/llmfuncs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/src/llmfuncs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 05:32:08.000000 llmfuncs-0.2.2/src/llmfuncs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:32:08.542379 llmfuncs-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-18 05:31:56.000000 llmfuncs-0.2.2/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:45:53.555611 llmfuncs-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 09:45:53.555611 llmfuncs-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 09:45:53.555611 llmfuncs-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:45:53.551611 llmfuncs-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:45:53.555611 llmfuncs-0.2.3/src/llmfuncs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/src/llmfuncs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/src/llmfuncs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/src/llmfuncs/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/src/llmfuncs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:45:53.555611 llmfuncs-0.2.3/src/llmfuncs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-18 09:45:53.000000 llmfuncs-0.2.3/src/llmfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-18 09:45:53.000000 llmfuncs-0.2.3/src/llmfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:45:53.000000 llmfuncs-0.2.3/src/llmfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 09:45:53.000000 llmfuncs-0.2.3/src/llmfuncs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 09:45:53.000000 llmfuncs-0.2.3/src/llmfuncs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:45:53.555611 llmfuncs-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-06-18 09:45:43.000000 llmfuncs-0.2.3/tests/test_tool.py
```

### Comparing `llmfuncs-0.2.2/LICENSE` & `llmfuncs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.2/PKG-INFO` & `llmfuncs-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llmfuncs-0.2.2/README.md` & `llmfuncs-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.2/setup.py` & `llmfuncs-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="llmfuncs",
-    version="0.2.2",
+    version="0.2.3",
     url="https://github.com/FyZyX/llmfuncs",
     author="Lucas Lofaro",
     author_email="lucasmlofaro@gmail.com",
     description="Dynamically generate JSON Schema from Python code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `llmfuncs-0.2.2/src/llmfuncs/schema.py` & `llmfuncs-0.2.3/src/llmfuncs/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,43 +23,47 @@
         type(None): "null",
     }
 
     # Check if type is a basic type
     if py_type in mapping:
         return mapping[py_type]
 
+    # For unparameterized list and dict types
+    if py_type is list or py_type is typing.List:
+        return {"type": "array", "items": {}}
+    if py_type is dict or py_type is typing.Dict:
+        return {"type": "object", "additionalProperties": {}}
+
     origin = typing.get_origin(py_type)
     args = typing.get_args(py_type)
 
     if origin is typing.Union:
         # this is a special case to handle Optional[type] which is just syntactic sugar
         # around Union[type, None]
         if len(args) == 2 and type(None) in args:
             # Assuming the None is always last
             return json_schema_type(args[0])
         else:
             return [json_schema_type(arg) for arg in args]
 
-    if origin is tuple or origin is typing.Tuple:
-        return {"type": "array",
-                "items": [json_schema_type(arg) for arg in args]}
-
     if origin is list or origin is typing.List:
         # For simplicity, we're assuming all elements in the list are of the same type
-        return {"type": "array", "items": json_schema_type(args[0])}
-
-    if origin is set or origin is typing.Set:
-        return {"type": "array", "uniqueItems": True,
-                "items": json_schema_type(args[0])}
+        schema_type = json_schema_type(args[0])
+        if isinstance(schema_type, dict):
+            return {"type": "array", "items": schema_type}
+        return {"type": "array",
+                "items": {"type": json_schema_type(args[0])}, }
 
     if origin is dict or origin is typing.Dict:
         # For simplicity, we're assuming all keys are strings
         # and all values are of the same type
-        additional_properties = json_schema_type(args[1])
-        return {"type": "object", "additionalProperties": additional_properties}
+        schema_type = json_schema_type(args[1])
+        if isinstance(schema_type, dict):
+            return {"type": "object", "additionalProperties": schema_type}
+        return {"type": "object", "additionalProperties": {"type": schema_type}}
 
     # The type is not supported
     raise ValueError(f"Cannot convert {py_type} to a JSON schema type")
 
 
 def get_param_schema(
         param_name: str,
@@ -75,16 +79,19 @@
     descriptions = (p.description for p in doc_parsed.params
                     if p.arg_name == param_name)
     param_doc = next(descriptions, None)
     if param_doc is None:
         raise ValueError(
             f"Missing description for parameter '{param_name}' in docstring")
 
-    param_schema = {
-        "type": param_type_str,
-        "description": param_doc,
-    }
+    # Check if the param_type_str is already a dictionary.
+    if isinstance(param_type_str, dict):
+        param_schema = param_type_str
+    else:
+        param_schema = {"type": param_type_str}
+
+    param_schema["description"] = param_doc
 
     if param.default is not param.empty:
         param_schema["default"] = param.default
 
     return param_schema
```

### Comparing `llmfuncs-0.2.2/src/llmfuncs/tool.py` & `llmfuncs-0.2.3/src/llmfuncs/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,49 +15,53 @@
     def __init__(self, func: typing.Callable, include_return=False):
         self._func = func
         self._include_return = include_return
 
         doc = inspect.getdoc(func)
         if not doc:
             raise ValueError(f"Missing docstring for function '{self.name()}'")
+
         self._docstring = docstring_parser.parse(doc)
         self._signature = inspect.signature(func)
         self._type_hints = typing.get_type_hints(func)
+        self._params_schema = {}
+        self._required_params = []
+
+        self._parse_arguments()
 
     def __call__(self, *args, **kwargs):
         return self._func(*args, **kwargs)
 
+    def _parse_arguments(self):
+        for param_name, param in self._signature.parameters.items():
+            param_schema = schema.get_param_schema(
+                param_name, param, self._type_hints, self._docstring,
+            )
+            self._params_schema[param_name] = param_schema
+            if param.default is param.empty:
+                self._required_params.append(param_name)
+
     def _has_return(self):
         return self._signature.return_annotation is not self._signature.empty
 
     def name(self) -> str:
         return self._func.__name__
 
     def schema(self):
-        params_schema = {}
-        required_params = []
-        for param_name, param in self._signature.parameters.items():
-            param_schema = schema.get_param_schema(
-                param_name, param, self._type_hints, self._docstring,
-            )
-            params_schema[param_name] = param_schema
-            if param.default is param.empty:
-                required_params.append(param_name)
-
         func_schema = {
             "name": self.name(),
             "description": self._docstring.short_description,
             "parameters": {
                 "type": "object",
-                "properties": params_schema,
+                "properties": self._params_schema,
             },
         }
 
-        if required_params:
-            func_schema["parameters"]["required"] = required_params
+        if self._required_params:
+            func_schema["parameters"]["required"] = self._required_params
 
         if self._include_return and self._has_return():
             schema_type = schema.json_schema_type(self._signature.return_annotation)
             func_schema["return"] = schema_type
 
         return func_schema
 
@@ -103,15 +107,15 @@
             package: str | pathlib.Path | types.ModuleType,
             include_return: bool = False,
     ):
         """Extracts and formats function schemas for all modules in a package."""
         if isinstance(package, str):
             package = importlib.import_module(package)
         for _, module_name, _ in pkgutil.walk_packages(package.__path__):
-            module_path = f'{package.__name__}.{module_name}'
+            module_path = f"{package.__name__}.{module_name}"
             self.add_tools_from_module(module_path, include_return=include_return)
 
     def add_tools_from_glob(self, pattern: str):
         """
         Given a glob pattern, find all the Python modules that match the pattern,
         and collect the schemas from all those modules.
         """
@@ -124,15 +128,15 @@
             self.add_tools_from_module(path.absolute())
 
     def use_tool(self, tool_name: str, json_args: str | typing.Mapping) -> typing.Any:
         tool = self._tools.get(tool_name)
         if not tool:
             raise ValueError(f"No tool found with name: {tool_name}")
 
-        params_schema = tool.schema()['parameters']
+        params_schema = tool.schema()["parameters"]
         is_string = isinstance(json_args, str)
         args = validator.parse_json(json_args) if is_string else json_args
         validator.validate_args_with_schema(args, params_schema)
         return tool(**args)
 
     def schema(self) -> typing.List[schema.JsonSchema]:
         return [tool.schema() for tool in self._tools.values()]
```

### Comparing `llmfuncs-0.2.2/src/llmfuncs/validator.py` & `llmfuncs-0.2.3/src/llmfuncs/validator.py`

 * *Files identical despite different names*

### Comparing `llmfuncs-0.2.2/src/llmfuncs.egg-info/PKG-INFO` & `llmfuncs-0.2.3/src/llmfuncs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmfuncs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Dynamically generate JSON Schema from Python code.
 Home-page: https://github.com/FyZyX/llmfuncs
 Author: Lucas Lofaro
 Author-email: lucasmlofaro@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

