# Comparing `tmp/openapi_dto-0.1.6.tar.gz` & `tmp/openapi_dto-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_dto-0.1.6.tar", max compression
+gzip compressed data, was "openapi_dto-0.1.7.tar", max compression
```

## Comparing `openapi_dto-0.1.6.tar` & `openapi_dto-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/LICENSE
--rw-r--r--   0        0        0      358 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/README.md
--rw-r--r--   0        0        0      751 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       51 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/__init__.py
--rw-r--r--   0        0        0       70 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/__main__.py
--rw-r--r--   0        0        0     2633 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/cli.py
--rw-r--r--   0        0        0      160 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/config.py
--rw-r--r--   0        0        0        0 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/engine/__init__.py
--rw-r--r--   0        0        0     1196 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/engine/base.py
--rw-r--r--   0        0        0    13257 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/engine/dataclasses.py
--rw-r--r--   0        0        0     1751 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/models.py
--rw-r--r--   0        0        0     1639 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/registry.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/LICENSE
+-rw-r--r--   0        0        0      358 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/README.md
+-rw-r--r--   0        0        0      751 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/__main__.py
+-rw-r--r--   0        0        0     2768 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/cli.py
+-rw-r--r--   0        0        0      160 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/config.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/engine/__init__.py
+-rw-r--r--   0        0        0     1196 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/engine/base.py
+-rw-r--r--   0        0        0    13695 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/engine/dataclasses.py
+-rw-r--r--   0        0        0     1835 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/models.py
+-rw-r--r--   0        0        0     1639 2023-06-18 12:13:20.891261 openapi_dto-0.1.7/src/openapi_dto/registry.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.7/PKG-INFO
```

### Comparing `openapi_dto-0.1.6/LICENSE` & `openapi_dto-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.6/pyproject.toml` & `openapi_dto-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-dto"
-version = "0.1.6"
+version = "0.1.7"
 description = "A CLI tool for automated DTO generation using OpenAPI schema"
 authors = ["Kacper Łukawski <kacper.lukawsk@embassy.ai>"]
 packages = [
     {include = "openapi_dto", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
```

### Comparing `openapi_dto-0.1.6/src/openapi_dto/engine/base.py` & `openapi_dto-0.1.7/src/openapi_dto/engine/base.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.6/src/openapi_dto/engine/dataclasses.py` & `openapi_dto-0.1.7/src/openapi_dto/engine/dataclasses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import keyword
 from typing import Optional
 
 from openapi_dto.config import NamingConvention
 from openapi_dto.engine.base import BaseDTOEngine
 from openapi_dto.models import TypeDefinition
 from openapi_dto.registry import TypeRegistry
 
@@ -75,32 +76,41 @@
                     ctx=ast.Load(),
                 ),
                 ctx=ast.Load(),
             ),
             lineno=0,
         )
 
-    def generate_type(self, name: str, type_schema: TypeDefinition) -> ast.AST:
-        # TODO: see https://swagger.io/docs/specification/data-models/dictionaries/
+    def generate_type(
+        self, name: str, type_schema: TypeDefinition, *, docstring: Optional[str] = None
+    ) -> ast.AST:
+        if type_schema.schema is not None:
+            return self.generate_type(
+                name, type_schema.schema, docstring=type_schema.description
+            )
         if type_schema.enum is not None:
             return self._generate_enum(name, type_schema)
         if type_schema.additional_properties is not None:
             return self._generate_dictionary(name, type_schema)
         if type_schema.all_of is not None:
             # In some cases there is just a $ref attribute provided as the first
             # entry and then the second one is a proper definition. There is no
             # need to create a union then.
             if (
                 2 == len(type_schema.all_of)
                 and type_schema.all_of[0].ref is not None
                 and "object" == type_schema.all_of[1].type
             ):
-                return self._generate_class(name, type_schema.all_of[1])
+                return self._generate_class(
+                    name, type_schema.all_of[1], docstring=type_schema.description
+                )
             return self._generate_union(name, type_schema)
-        return self._generate_class(name, type_schema)
+        return self._generate_class(
+            name, type_schema, docstring=type_schema.description
+        )
 
     def _generate_union(
         self,
         name: str,
         type_schema: TypeDefinition,
     ) -> ast.AST:
         union_options = []
@@ -139,34 +149,35 @@
             return union_member.title
         # ValueError indicates there is no way to extract the name of a union member,
         # so it is possibly not a name of a type, but some sort of dictionary-like
         # object and has to be handled externally
         raise ValueError
 
     def _generate_class(
-        self,
-        name: str,
-        type_schema: TypeDefinition,
+        self, name: str, type_schema: TypeDefinition, *, docstring: Optional[str] = None
     ) -> ast.AST:
+        class_body = []
+
+        # TODO: append the docstring to a class
+
         if type_schema.properties is not None:
-            class_body = []
             nullable_groups = [
                 (
                     False,
                     None,
                 ),  # First all the non-nullable fields
                 (True,),  # Then the nullable ones
             ]
             for nullable_group in nullable_groups:
-                for type_name, type_def in type_schema.properties.items():
+                for field_name, type_def in type_schema.properties.items():
                     if type_def.nullable not in nullable_group:
                         continue
-                    class_body.append(self._generate_field(name, type_name, type_def))
+                    class_body.append(self._generate_field(name, field_name, type_def))
         else:
-            class_body = [ast.Pass()]
+            class_body.append(ast.Pass())
 
         return ast.ClassDef(
             name=name,
             bases=[],
             keywords=[],
             body=class_body,
             decorator_list=[
@@ -179,15 +190,18 @@
 
     def _generate_field(
         self,
         class_name: str,
         field_name: str,
         type_def: TypeDefinition,
     ) -> ast.AST:
-        normalized_field_name = self.convert_name(field_name)
+        normalized_field_name = self.convert_name(
+            field_name if not keyword.iskeyword(field_name) else f"{field_name}_val"
+        )
+
         type_annotation = self._get_field_type_annotation(
             class_name,
             field_name,
             type_def,
         )
 
         args, keywords = [], []
@@ -346,8 +360,7 @@
                     value=ast.Constant(value=value),
                     lineno=0,
                 )
                 for value in type_schema.enum
             ],
             decorator_list=[],
         )
-
```

### Comparing `openapi_dto-0.1.6/src/openapi_dto/models.py` & `openapi_dto-0.1.7/src/openapi_dto/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,7 +43,9 @@
     maximum: Optional[int] = None
     minimum: Optional[int] = None
     example: Optional[ValueExample] = None
     required: Optional[List[str]] = None
     additional_properties: Optional["TypeDefinition"] = field(
         default=None, metadata=config(field_name="additionalProperties")
     )
+    description: Optional[str] = None
+    schema: Optional["TypeDefinition"] = None
```

### Comparing `openapi_dto-0.1.6/src/openapi_dto/registry.py` & `openapi_dto-0.1.7/src/openapi_dto/registry.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.6/PKG-INFO` & `openapi_dto-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-dto
-Version: 0.1.6
+Version: 0.1.7
 Summary: A CLI tool for automated DTO generation using OpenAPI schema
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawsk@embassy.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

