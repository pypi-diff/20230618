# Comparing `tmp/openapi_dto-0.1.5.tar.gz` & `tmp/openapi_dto-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_dto-0.1.5.tar", max compression
+gzip compressed data, was "openapi_dto-0.1.6.tar", max compression
```

## Comparing `openapi_dto-0.1.5.tar` & `openapi_dto-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/LICENSE
--rw-r--r--   0        0        0      358 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/README.md
--rw-r--r--   0        0        0      751 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       51 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/__init__.py
--rw-r--r--   0        0        0       70 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/__main__.py
--rw-r--r--   0        0        0     2633 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/cli.py
--rw-r--r--   0        0        0      160 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/config.py
--rw-r--r--   0        0        0        0 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/engine/__init__.py
--rw-r--r--   0        0        0     1196 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/engine/base.py
--rw-r--r--   0        0        0    12841 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/engine/dataclasses.py
--rw-r--r--   0        0        0     1751 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/models.py
--rw-r--r--   0        0        0     1639 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/registry.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/LICENSE
+-rw-r--r--   0        0        0      358 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/README.md
+-rw-r--r--   0        0        0      751 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/__main__.py
+-rw-r--r--   0        0        0     2633 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/cli.py
+-rw-r--r--   0        0        0      160 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/config.py
+-rw-r--r--   0        0        0        0 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/engine/__init__.py
+-rw-r--r--   0        0        0     1196 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/engine/base.py
+-rw-r--r--   0        0        0    13257 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/engine/dataclasses.py
+-rw-r--r--   0        0        0     1751 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/models.py
+-rw-r--r--   0        0        0     1639 2023-06-18 10:41:44.992524 openapi_dto-0.1.6/src/openapi_dto/registry.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.6/PKG-INFO
```

### Comparing `openapi_dto-0.1.5/LICENSE` & `openapi_dto-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.5/pyproject.toml` & `openapi_dto-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-dto"
-version = "0.1.5"
+version = "0.1.6"
 description = "A CLI tool for automated DTO generation using OpenAPI schema"
 authors = ["Kacper Łukawski <kacper.lukawsk@embassy.ai>"]
 packages = [
     {include = "openapi_dto", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
```

### Comparing `openapi_dto-0.1.5/src/openapi_dto/cli.py` & `openapi_dto-0.1.6/src/openapi_dto/cli.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.5/src/openapi_dto/engine/base.py` & `openapi_dto-0.1.6/src/openapi_dto/engine/base.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.5/src/openapi_dto/engine/dataclasses.py` & `openapi_dto-0.1.6/src/openapi_dto/engine/dataclasses.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 
 class DataclassesEngine(BaseDTOEngine):
     """
     Engine using Python built-in dataclasses with dataclasses-json to generate
     the DTOs.
     """
 
-    UNKNOWN_MEMBERS_COUNTER = 0
-
     def __init__(
         self, type_registry: TypeRegistry, naming_convention: NamingConvention
     ):
         super().__init__(type_registry, naming_convention)
         self.type_registry.add_import(
             ast.ImportFrom(
                 module="dataclasses",
@@ -78,14 +76,15 @@
                 ),
                 ctx=ast.Load(),
             ),
             lineno=0,
         )
 
     def generate_type(self, name: str, type_schema: TypeDefinition) -> ast.AST:
+        # TODO: see https://swagger.io/docs/specification/data-models/dictionaries/
         if type_schema.enum is not None:
             return self._generate_enum(name, type_schema)
         if type_schema.additional_properties is not None:
             return self._generate_dictionary(name, type_schema)
         if type_schema.all_of is not None:
             # In some cases there is just a $ref attribute provided as the first
             # entry and then the second one is a proper definition. There is no
@@ -100,18 +99,27 @@
         return self._generate_class(name, type_schema)
 
     def _generate_union(
         self,
         name: str,
         type_schema: TypeDefinition,
     ) -> ast.AST:
-        union_options = [
-            self._parse_union_member_name(union_member)
-            for union_member in type_schema.all_of
-        ]
+        union_options = []
+        for i, union_member in enumerate(type_schema.all_of):
+            try:
+                member_name = self._parse_union_member_name(union_member)
+            except ValueError:
+                # Union member might be referring to a typed structure, such as
+                # dictionary, or a different union.
+                member_name = f"{name}_{i}"
+                generated_type = self.generate_type(member_name, union_member)
+                self.type_registry.map(member_name, generated_type)
+            finally:
+                union_options.append(member_name)
+
         return ast.Assign(
             targets=[ast.Name(id=name, ctx=ast.Store())],
             value=ast.Subscript(
                 value=ast.Name(id="Union", ctx=ast.Load()),
                 slice=ast.Tuple(
                     elts=[
                         ast.Name(id=subtype_name, ctx=ast.Load())
@@ -125,17 +133,18 @@
         )
 
     def _parse_union_member_name(self, union_member: TypeDefinition) -> str:
         if union_member.ref is not None:
             return self._parse_ref_name(union_member.ref)
         if union_member.title is not None:
             return union_member.title
-        # As a fallback, any name might be generated, as such a union member won't
-        # be ever referred anywhere else in the code
-        return self._generate_type_name()
+        # ValueError indicates there is no way to extract the name of a union member,
+        # so it is possibly not a name of a type, but some sort of dictionary-like
+        # object and has to be handled externally
+        raise ValueError
 
     def _generate_class(
         self,
         name: str,
         type_schema: TypeDefinition,
     ) -> ast.AST:
         if type_schema.properties is not None:
@@ -338,10 +347,7 @@
                     lineno=0,
                 )
                 for value in type_schema.enum
             ],
             decorator_list=[],
         )
 
-    def _generate_type_name(self) -> str:
-        DataclassesEngine.UNKNOWN_MEMBERS_COUNTER += 1
-        return f"Type_{DataclassesEngine.UNKNOWN_MEMBERS_COUNTER}"
```

### Comparing `openapi_dto-0.1.5/src/openapi_dto/models.py` & `openapi_dto-0.1.6/src/openapi_dto/models.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.5/src/openapi_dto/registry.py` & `openapi_dto-0.1.6/src/openapi_dto/registry.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.5/PKG-INFO` & `openapi_dto-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-dto
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI tool for automated DTO generation using OpenAPI schema
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawsk@embassy.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

