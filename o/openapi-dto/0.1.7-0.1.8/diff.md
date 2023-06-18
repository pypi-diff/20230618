# Comparing `tmp/openapi_dto-0.1.7.tar.gz` & `tmp/openapi_dto-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_dto-0.1.7.tar", max compression
+gzip compressed data, was "openapi_dto-0.1.8.tar", max compression
```

## Comparing `openapi_dto-0.1.7.tar` & `openapi_dto-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/LICENSE
--rw-r--r--   0        0        0      358 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/README.md
--rw-r--r--   0        0        0      751 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       51 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/__init__.py
--rw-r--r--   0        0        0       70 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/__main__.py
--rw-r--r--   0        0        0     2768 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/cli.py
--rw-r--r--   0        0        0      160 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/config.py
--rw-r--r--   0        0        0        0 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/engine/__init__.py
--rw-r--r--   0        0        0     1196 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/engine/base.py
--rw-r--r--   0        0        0    13695 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/engine/dataclasses.py
--rw-r--r--   0        0        0     1835 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/models.py
--rw-r--r--   0        0        0     1639 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/registry.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/LICENSE
+-rw-r--r--   0        0        0      358 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/README.md
+-rw-r--r--   0        0        0      751 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/__main__.py
+-rw-r--r--   0        0        0     2768 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/cli.py
+-rw-r--r--   0        0        0      160 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/config.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/engine/__init__.py
+-rw-r--r--   0        0        0     1196 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/engine/base.py
+-rw-r--r--   0        0        0    13710 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/engine/dataclasses.py
+-rw-r--r--   0        0        0     1835 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/models.py
+-rw-r--r--   0        0        0     1639 2023-06-18 12:21:40.077417 openapi_dto-0.1.8/src/openapi_dto/registry.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.8/PKG-INFO
```

### Comparing `openapi_dto-0.1.7/LICENSE` & `openapi_dto-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.7/pyproject.toml` & `openapi_dto-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-dto"
-version = "0.1.7"
+version = "0.1.8"
 description = "A CLI tool for automated DTO generation using OpenAPI schema"
 authors = ["Kacper Łukawski <kacper.lukawsk@embassy.ai>"]
 packages = [
     {include = "openapi_dto", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
```

### Comparing `openapi_dto-0.1.7/src/openapi_dto/cli.py` & `openapi_dto-0.1.8/src/openapi_dto/cli.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.7/src/openapi_dto/engine/base.py` & `openapi_dto-0.1.8/src/openapi_dto/engine/base.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.7/src/openapi_dto/engine/dataclasses.py` & `openapi_dto-0.1.8/src/openapi_dto/engine/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,17 +100,15 @@
                 and type_schema.all_of[0].ref is not None
                 and "object" == type_schema.all_of[1].type
             ):
                 return self._generate_class(
                     name, type_schema.all_of[1], docstring=type_schema.description
                 )
             return self._generate_union(name, type_schema)
-        return self._generate_class(
-            name, type_schema, docstring=type_schema.description
-        )
+        return self._generate_class(name, type_schema, docstring=docstring)
 
     def _generate_union(
         self,
         name: str,
         type_schema: TypeDefinition,
     ) -> ast.AST:
         union_options = []
@@ -153,15 +151,16 @@
         raise ValueError
 
     def _generate_class(
         self, name: str, type_schema: TypeDefinition, *, docstring: Optional[str] = None
     ) -> ast.AST:
         class_body = []
 
-        # TODO: append the docstring to a class
+        if docstring:
+            class_body.append(ast.Expr(value=ast.Constant(value=docstring)))
 
         if type_schema.properties is not None:
             nullable_groups = [
                 (
                     False,
                     None,
                 ),  # First all the non-nullable fields
```

### Comparing `openapi_dto-0.1.7/src/openapi_dto/models.py` & `openapi_dto-0.1.8/src/openapi_dto/models.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.7/src/openapi_dto/registry.py` & `openapi_dto-0.1.8/src/openapi_dto/registry.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.7/PKG-INFO` & `openapi_dto-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-dto
-Version: 0.1.7
+Version: 0.1.8
 Summary: A CLI tool for automated DTO generation using OpenAPI schema
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawsk@embassy.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

