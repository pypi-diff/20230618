# Comparing `tmp/openapi_dto-0.1.4.tar.gz` & `tmp/openapi_dto-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_dto-0.1.4.tar", max compression
+gzip compressed data, was "openapi_dto-0.1.5.tar", max compression
```

## Comparing `openapi_dto-0.1.4.tar` & `openapi_dto-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/LICENSE
--rw-r--r--   0        0        0      358 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/README.md
--rw-r--r--   0        0        0      733 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       51 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/__init__.py
--rw-r--r--   0        0        0       70 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/__main__.py
--rw-r--r--   0        0        0     2617 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/cli.py
--rw-r--r--   0        0        0      160 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/config.py
--rw-r--r--   0        0        0        0 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/engine/__init__.py
--rw-r--r--   0        0        0     1196 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/engine/base.py
--rw-r--r--   0        0        0    10362 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/engine/dataclasses.py
--rw-r--r--   0        0        0     1962 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/models.py
--rw-r--r--   0        0        0     1639 2022-12-14 12:10:49.772400 openapi_dto-0.1.4/src/openapi_dto/registry.py
--rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 openapi_dto-0.1.4/setup.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/LICENSE
+-rw-r--r--   0        0        0      358 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/README.md
+-rw-r--r--   0        0        0      751 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/__main__.py
+-rw-r--r--   0        0        0     2633 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/cli.py
+-rw-r--r--   0        0        0      160 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/config.py
+-rw-r--r--   0        0        0        0 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/engine/__init__.py
+-rw-r--r--   0        0        0     1196 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/engine/base.py
+-rw-r--r--   0        0        0    12841 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/engine/dataclasses.py
+-rw-r--r--   0        0        0     1751 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/models.py
+-rw-r--r--   0        0        0     1639 2023-06-18 10:19:45.655220 openapi_dto-0.1.5/src/openapi_dto/registry.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 openapi_dto-0.1.5/PKG-INFO
```

### Comparing `openapi_dto-0.1.4/LICENSE` & `openapi_dto-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.4/pyproject.toml` & `openapi_dto-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-dto"
-version = "0.1.4"
+version = "0.1.5"
 description = "A CLI tool for automated DTO generation using OpenAPI schema"
 authors = ["Kacper Łukawski <kacper.lukawsk@embassy.ai>"]
 packages = [
     {include = "openapi_dto", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
@@ -14,14 +14,15 @@
 dataclasses-json = "^0.5.7"
 typer = "^0.7.0"
 camel-converter = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pre-commit = "^2.20.0"
+black = "^23.3.0"
 
 [tool.poetry.scripts]
 openapi_dto = "openapi_dto.cli:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openapi_dto-0.1.4/src/openapi_dto/cli.py` & `openapi_dto-0.1.5/src/openapi_dto/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import typer
 import logging
 
 from openapi_dto.config import NamingConvention, OutputEngine
 from openapi_dto.engine.base import BaseDTOEngine
 from openapi_dto.engine.dataclasses import DataclassesEngine
-from openapi_dto.models import Schema
+from openapi_dto.models import TypeDefinition
 from openapi_dto.registry import TypeRegistry
 
 logger = logging.getLogger(__name__)
 
 app = typer.Typer()
 
 
@@ -69,13 +69,13 @@
     # Process the types one by one
     registry = TypeRegistry()
     engine: BaseDTOEngine = ENGINE_MAPPING.get(output_engine)(
         type_registry=registry,
         naming_convention=naming_convention,
     )
     for type_name, type_schema in schemas.items():
-        schema = Schema.from_dict(type_schema)
+        schema = TypeDefinition.from_dict(type_schema)
         generated_type = engine.generate_type(type_name, schema)
         registry.map(type_name, generated_type)
 
     # Display the complete source code
     print(registry.to_source_code())
```

### Comparing `openapi_dto-0.1.4/src/openapi_dto/engine/base.py` & `openapi_dto-0.1.5/src/openapi_dto/engine/base.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.4/src/openapi_dto/engine/dataclasses.py` & `openapi_dto-0.1.5/src/openapi_dto/engine/dataclasses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import ast
+from typing import Optional
+
 from openapi_dto.config import NamingConvention
 from openapi_dto.engine.base import BaseDTOEngine
-from openapi_dto.models import TypeDefinition, Schema
+from openapi_dto.models import TypeDefinition
 from openapi_dto.registry import TypeRegistry
 
 
 class DataclassesEngine(BaseDTOEngine):
     """
     Engine using Python built-in dataclasses with dataclasses-json to generate
     the DTOs.
     """
 
+    UNKNOWN_MEMBERS_COUNTER = 0
+
     def __init__(
         self, type_registry: TypeRegistry, naming_convention: NamingConvention
     ):
         super().__init__(type_registry, naming_convention)
         self.type_registry.add_import(
             ast.ImportFrom(
                 module="dataclasses",
@@ -37,22 +41,55 @@
         self.type_registry.add_import(
             ast.ImportFrom(
                 module="typing",
                 names=[
                     ast.alias(name="List"),
                     ast.alias(name="Union"),
                     ast.alias(name="Optional"),
+                    ast.alias(name="Dict"),
+                    ast.alias(name="Any"),
+                ],
+                level=0,
+            )
+        )
+        self.type_registry.add_import(
+            ast.ImportFrom(
+                module="enum",
+                names=[
+                    ast.alias(name="Enum"),
                 ],
                 level=0,
             )
         )
 
-    def generate_type(self, name: str, type_schema: Schema) -> ast.AST:
+    def _generate_dictionary(self, name: str, type_schema: TypeDefinition) -> ast.AST:
+        # TODO: extract the value type from type_schema (ref or type)
+        return ast.Assign(
+            targets=[
+                ast.Name(id=name, ctx=ast.Store()),
+            ],
+            value=ast.Subscript(
+                value=ast.Name(id="Dict", ctx=ast.Load()),
+                slice=ast.Tuple(
+                    elts=[
+                        ast.Name(id="Any", ctx=ast.Load()),
+                        ast.Name(id="Any", ctx=ast.Load()),
+                    ],
+                    ctx=ast.Load(),
+                ),
+                ctx=ast.Load(),
+            ),
+            lineno=0,
+        )
+
+    def generate_type(self, name: str, type_schema: TypeDefinition) -> ast.AST:
         if type_schema.enum is not None:
             return self._generate_enum(name, type_schema)
+        if type_schema.additional_properties is not None:
+            return self._generate_dictionary(name, type_schema)
         if type_schema.all_of is not None:
             # In some cases there is just a $ref attribute provided as the first
             # entry and then the second one is a proper definition. There is no
             # need to create a union then.
             if (
                 2 == len(type_schema.all_of)
                 and type_schema.all_of[0].ref is not None
@@ -61,15 +98,15 @@
                 return self._generate_class(name, type_schema.all_of[1])
             return self._generate_union(name, type_schema)
         return self._generate_class(name, type_schema)
 
     def _generate_union(
         self,
         name: str,
-        type_schema: Schema,
+        type_schema: TypeDefinition,
     ) -> ast.AST:
         union_options = [
             self._parse_union_member_name(union_member)
             for union_member in type_schema.all_of
         ]
         return ast.Assign(
             targets=[ast.Name(id=name, ctx=ast.Store())],
@@ -83,25 +120,27 @@
                     ctx=ast.Load(),
                 ),
                 ctx=ast.Load(),
             ),
             lineno=0,
         )
 
-    def _parse_union_member_name(self, union_member: Schema) -> str:
+    def _parse_union_member_name(self, union_member: TypeDefinition) -> str:
         if union_member.ref is not None:
             return self._parse_ref_name(union_member.ref)
         if union_member.title is not None:
             return union_member.title
-        raise ValueError
+        # As a fallback, any name might be generated, as such a union member won't
+        # be ever referred anywhere else in the code
+        return self._generate_type_name()
 
     def _generate_class(
         self,
         name: str,
-        type_schema: Schema,
+        type_schema: TypeDefinition,
     ) -> ast.AST:
         if type_schema.properties is not None:
             class_body = []
             nullable_groups = [
                 (
                     False,
                     None,
@@ -153,15 +192,15 @@
                         func=ast.Name(id="config", ctx=ast.Load()),
                         args=[],
                         keywords=[
                             ast.keyword(
                                 arg="field_name",
                                 value=ast.Constant(value=field_name),
                             ),
-                        ]
+                        ],
                     ),
                 ),
             )
         value = ast.Call(
             func=ast.Name(id="field", ctx=ast.Load()),
             args=args,
             keywords=keywords,
@@ -200,16 +239,25 @@
                 type_def.items,
             )
             type_annotation = ast.Subscript(
                 value=ast.Name(id="List", ctx=ast.Load()),
                 slice=subfield_type_annotation,
                 ctx=ast.Load(),
             )
+        elif type_def.properties is not None:
+            # This is a nested definition of a type with a set of attributes. Sometimes
+            # those inner structures do not have a proper name provided, and they have
+            # to be generated from the parent class and the attribute name.
+            type_name = type_def.title or f"{class_name}_{field_name}"
+            generated_type = self.generate_type(type_name, type_def)
+            self.type_registry.map(type_name, generated_type)
+            type_annotation = ast.Name(id=type_name, ctx=ast.Load())
         elif type_def.all_of is not None:
-            # In some cases there might be multiple types accepted
+            # In some cases there might be multiple types accepted, so we need to use
+            # a union of all the accepted subtypes
             subfield_type_annotations = [
                 self._get_field_type_annotation(
                     class_name,
                     field_name,
                     item,
                 )
                 for item in type_def.all_of
@@ -229,25 +277,33 @@
 
             type_annotation = ast.Subscript(
                 value=ast.Name(id="Union", ctx=ast.Load()),
                 slice=ast.Tuple(elts=auto_types),
                 ctx=ast.Load(),
             )
         elif "object" == type_def.type:
+            # Accepts any JSON-like object, without specifying the field names and
+            # accepted types of values
             type_annotation = ast.Subscript(
                 value=ast.Name(id="Dict", ctx=ast.Load()),
                 slice=ast.Tuple(
                     elts=[
                         ast.Name(id="Any", ctx=ast.Load()),
                         ast.Name(id="Any", ctx=ast.Load()),
                     ],
                     ctx=ast.Load(),
                 ),
                 ctx=ast.Load(),
             )
+        elif type_def.additional_properties is not None:
+            # This is a name over a different type, usually a primitive with an example
+            # of usage, thus we do not need to create an alias
+            type_annotation = self._get_field_type_annotation(
+                class_name, field_name, type_def.additional_properties
+            )
         else:
             field_type_name = self.type_registry[type_def.type].__name__
             type_annotation = ast.Name(id=field_type_name, ctx=ast.Load())
 
         if type_def.nullable is True:
             # Nullable fields are marked as optional, so they accept None
             type_annotation = ast.Subscript(
@@ -264,23 +320,15 @@
 
     def _parse_ref_name(self, ref_value: str) -> str:
         field_type_name = ref_value.split("/")[-1]
         if field_type_name not in self.type_registry:
             field_type_name = f'"{field_type_name}"'
         return field_type_name
 
-    def _generate_enum(self, name: str, type_schema: Schema) -> ast.AST:
-        self.type_registry.add_import(
-            ast.ImportFrom(
-                module="enum",
-                names=[ast.alias(name="Enum")],
-                level=0,
-            )
-        )
-
+    def _generate_enum(self, name: str, type_schema: TypeDefinition) -> ast.AST:
         return ast.ClassDef(
             name=name,
             bases=[ast.Name(id="Enum", ctx=ast.Load())],
             keywords=[],
             body=[
                 ast.Assign(
                     targets=[
@@ -289,7 +337,11 @@
                     value=ast.Constant(value=value),
                     lineno=0,
                 )
                 for value in type_schema.enum
             ],
             decorator_list=[],
         )
+
+    def _generate_type_name(self) -> str:
+        DataclassesEngine.UNKNOWN_MEMBERS_COUNTER += 1
+        return f"Type_{DataclassesEngine.UNKNOWN_MEMBERS_COUNTER}"
```

### Comparing `openapi_dto-0.1.4/src/openapi_dto/models.py` & `openapi_dto-0.1.5/src/openapi_dto/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 ]
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclass
 class TypeDefinition:
     type: Optional[str] = None
+    enum: Optional[List[str]] = None
+    properties: Optional[Dict[str, "TypeDefinition"]] = None
+    title: Optional[str] = None
     ref: Optional[str] = field(default=None, metadata=config(field_name="$ref"))
     format: Optional[str] = None
-    title: Optional[str] = None
     nullable: bool = False
     items: Optional["TypeDefinition"] = None
     all_of: Optional[List["TypeDefinition"]] = field(
         default=None, metadata=config(field_name="allOf")
     )
-    one_of: Optional[List["Schema"]] = field(
+    one_of: Optional[List["TypeDefinition"]] = field(
         default=None, metadata=config(field_name="oneOf")
     )
     read_only: Optional[bool] = field(
         default=None, metadata=config(field_name="readOnly")
     )
     write_only: Optional[bool] = field(
         default=None, metadata=config(field_name="writeOnly")
@@ -37,22 +39,11 @@
     )
     max_items: Optional[int] = field(
         default=None, metadata=config(field_name="maxItems")
     )
     maximum: Optional[int] = None
     minimum: Optional[int] = None
     example: Optional[ValueExample] = None
-    enum: Optional[List[str]] = None
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclass
-class Schema:
-    type: Optional[str] = None
-    enum: Optional[List[str]] = None
-    properties: Optional[Dict[str, TypeDefinition]] = None
     required: Optional[List[str]] = None
-    all_of: Optional[List["Schema"]] = field(
-        default=None, metadata=config(field_name="allOf")
+    additional_properties: Optional["TypeDefinition"] = field(
+        default=None, metadata=config(field_name="additionalProperties")
     )
-    title: Optional[str] = None
-    ref: Optional[str] = field(default=None, metadata=config(field_name="$ref"))
```

### Comparing `openapi_dto-0.1.4/src/openapi_dto/registry.py` & `openapi_dto-0.1.5/src/openapi_dto/registry.py`

 * *Files identical despite different names*

### Comparing `openapi_dto-0.1.4/PKG-INFO` & `openapi_dto-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-dto
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool for automated DTO generation using OpenAPI schema
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawsk@embassy.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

