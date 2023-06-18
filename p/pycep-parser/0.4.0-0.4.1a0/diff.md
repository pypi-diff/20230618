# Comparing `tmp/pycep_parser-0.4.0.tar.gz` & `tmp/pycep_parser-0.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycep_parser-0.4.0.tar", max compression
+gzip compressed data, was "pycep_parser-0.4.1a0.tar", max compression
```

## Comparing `pycep_parser-0.4.0.tar` & `pycep_parser-0.4.1a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10834 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/LICENSE
--rw-r--r--   0        0        0     1511 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/README.md
--rw-r--r--   0        0        0       57 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/__init__.py
--rw-r--r--   0        0        0    12350 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/bicep.lark
--rw-r--r--   0        0        0     1854 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/main.py
--rw-r--r--   0        0        0        0 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/py.typed
--rw-r--r--   0        0        0    55529 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/transformer.py
--rw-r--r--   0        0        0    23875 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/typing.py
--rw-r--r--   0        0        0      274 2023-04-30 03:42:48.164494 pycep_parser-0.4.0/pycep/validator.py
--rw-r--r--   0        0        0     1459 2023-04-30 03:43:08.180629 pycep_parser-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 pycep_parser-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10834 2023-06-18 14:07:47.318496 pycep_parser-0.4.1a0/LICENSE
+-rw-r--r--   0        0        0     1511 2023-06-18 14:07:47.318496 pycep_parser-0.4.1a0/README.md
+-rw-r--r--   0        0        0       57 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/__init__.py
+-rw-r--r--   0        0        0    12506 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/bicep.lark
+-rw-r--r--   0        0        0     1854 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/main.py
+-rw-r--r--   0        0        0        0 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/py.typed
+-rw-r--r--   0        0        0    56086 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/transformer.py
+-rw-r--r--   0        0        0    23875 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/typing.py
+-rw-r--r--   0        0        0      274 2023-06-18 14:07:47.322496 pycep_parser-0.4.1a0/pycep/validator.py
+-rw-r--r--   0        0        0     1461 2023-06-18 14:08:08.542814 pycep_parser-0.4.1a0/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 pycep_parser-0.4.1a0/PKG-INFO
```

### Comparing `pycep_parser-0.4.0/LICENSE` & `pycep_parser-0.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.0/README.md` & `pycep_parser-0.4.1a0/README.md`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.0/pycep/bicep.lark` & `pycep_parser-0.4.1a0/pycep/bicep.lark`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 element: "targetScope" "=" QUOTED_INTERPOLATION                                         -> scope
        | [decorator] "param" STRING data_type ["=" value_brackets]                      -> param
        | [decorator] "var" STRING "=" var_value                                         -> var
        | [decorator] "output" STRING data_type "=" output_value                         -> output
        | [decorator] "resource" STRING type_api_pair [EXISTING] "=" resource_value      -> resource
        | [decorator] "module" STRING module_path "=" module_value                       -> module
 
-?value: "null"                      -> null
-      | "true"                      -> true
-      | "false"                     -> false
-      | INT                         -> int
-      | STRING                      -> string
-      | QUOTED_INTERPOLATION        -> string
-      | INDEXED                     -> string
-      | MULTI_LINE_STRING           -> multi_line_string
+?value: _NEWLINE? "null"                      -> null
+      | _NEWLINE? "true"                      -> true
+      | _NEWLINE? "false"                     -> false
+      | _NEWLINE? INT                         -> int
+      | _NEWLINE? STRING                      -> string
+      | _NEWLINE? QUOTED_INTERPOLATION        -> string
+      | _NEWLINE? INDEXED                     -> string
+      | MULTI_LINE_STRING                     -> multi_line_string
       | array
       | object
-      | function
+      | _NEWLINE? function
       | operator
 
 ?value_brackets: (value | "(" value ")") "!"?
 
 // element values
 
 ?var_value: value_brackets | loop
@@ -84,15 +84,15 @@
 
 deco_max_len: "maxLength" "(" /\d+/ ")"
 
 deco_min_val: "minValue" "(" /-?\d+/ ")"
 
 deco_max_val: "maxValue" "(" /\d+/ ")"
 
-deco_metadata: "metadata" "(" object ")"
+deco_metadata: "metadata" "(" _CPP_COMMENT_NL? object _CPP_COMMENT_NL? ")"
 
 deco_secure: "secure" "(" ")"
 
 // functions
 
 function: function_any | function_array | function_date | function_deployment | function_file | function_lambda
         | function_logical | function_numeric | function_object | function_resource | function_scope | function_string
@@ -198,24 +198,25 @@
 // functions - resource
 
 ?function_resource: extension_resource_id | list_keys | management_group_resource_id | pick_zones | reference
                   | resource_id | subscription_resource_id | tenant_resource_id
 
 extension_resource_id: ("extensionResourceId" | "az.extensionResourceId") "(" value_brackets ("," value_brackets)~2..3 ")"
 
-list_keys: ("listKeys" | "az.listKeys") "(" value_brackets "," value_brackets ")" [["[" STRING "]"] "." (STRING | INDEXED)]
+_LIST_KEYS.1: ("listKeys" | "az.listKeys") "("
+list_keys: _LIST_KEYS value_brackets "," value_brackets ")" [["[" STRING "]"] "." (STRING | INDEXED)]
 
 management_group_resource_id: ("managementGroupResourceId" | "az.managementGroupResourceId") "(" value_brackets ("," value_brackets)~1..2 ")"
 
 pick_zones: ("pickZones" | "az.pickZones") "(" value_brackets ("," value_brackets)~2..4 ")"
 
 reference: ("reference" | "az.reference") "(" value_brackets ["," value_brackets ["," value_brackets]] ")" ["." STRING]
 
 _RESOURCE_ID.1: ("resourceId" | "az.resourceId") "("
-resource_id: _RESOURCE_ID value_brackets ("," value_brackets)~1..4 ")"
+resource_id: _RESOURCE_ID value_brackets ("," value_brackets)~1..9 _CPP_COMMENT_NL? ")"
 
 subscription_resource_id: ("subscriptionResourceId" | "az.subscriptionResourceId") "(" value_brackets ("," value_brackets)~1..3 ")"
 
 tenant_resource_id: ("tenantResourceId" | "az.tenantResourceId") "(" value_brackets ("," value_brackets)~1..2 ")"
 
 // functions - scope
 
@@ -347,15 +348,15 @@
 
 // Terms
 
 EXISTING: "existing"
 
 STRING: /[a-zA-Z_](::|[\w_.])*/
 QUOTED_STRING: "'" STRING "'"
-INDEXED: /(?=[\w][\w_.]+(.(get|list)[a-zA-Z]*\(('[\w-]+'|[\w.]+)?\)|[\[\]])+)(.(get|list)[a-zA-Z]*\(('[\w-]+'|[\w.]+)?\)|\[[\w\[\]_().']+\]!?|[\w_\-\/.,'= ])+/
+INDEXED: /(?=[\w][\w_.]+(.(get|list)[a-zA-Z]*\(([\w., '-]+)?\)|[\[\]])+)(.(get|list)[a-zA-Z]*\(([\w., '-]+)?\)|\[[\w\[\]_().']+\]!?|[\w_\-\/.,'= ])+/
 QUOTED_INTERPOLATION: /(?!.*''')'(\${(?:[^}'{]+|(?R))*+}|\\'|[^'])*'/
 
 MULTI_LINE_STRING: "'''" (/.*?/ | NEWLINE)+ "'''"
 
 _NEWLINE: NEWLINE
 _CPP_COMMENT_NL: [CPP_COMMENT] NEWLINE
```

### Comparing `pycep_parser-0.4.0/pycep/main.py` & `pycep_parser-0.4.1a0/pycep/main.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.0/pycep/transformer.py` & `pycep_parser-0.4.1a0/pycep/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1023,19 +1023,31 @@
             # 0 -> subscription_id, 1 -> resource_group_name, 2 -> resource_type, 3 -> resource_name_1
             subscription_id = None
             resource_group_name = str(args[0])
             resource_type = str(args[1])
             resource_name_1 = str(args[2])
             resource_name_2 = str(args[3])
         else:
+            # in theory there could be many resource_name parameters, but it is currently limited to 7
             subscription_id = str(args[0])
             resource_group_name = str(args[1])
             resource_type = str(args[2])
-            resource_name_1 = str(args[3])
-            resource_name_2 = str(args[4])
+
+            return {
+                "type": "resource_id",
+                "parameters": {
+                    "resource_type": resource_type,
+                    **{  # type: ignore[misc] # dynamic operand creation
+                        f"resource_name_{idx}": str(resource_name)
+                        for idx, resource_name in enumerate(args[3:], start=1)
+                    },
+                    "resource_group_name": resource_group_name,
+                    "subscription_id": subscription_id,
+                },
+            }
 
         return {
             "type": "resource_id",
             "parameters": {
                 "resource_type": resource_type,
                 "resource_name_1": resource_name_1,
                 "resource_name_2": resource_name_2,
```

### Comparing `pycep_parser-0.4.0/pycep/typing.py` & `pycep_parser-0.4.1a0/pycep/typing.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.0/pyproject.toml` & `pycep_parser-0.4.1a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycep-parser"
-version = "0.4.0"
+version = "0.4.1a0"
 description = "A Python based Bicep parser"
 authors = ["Anton Grübel <anton.gruebel@gmail.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 
 packages = [
```

### Comparing `pycep_parser-0.4.0/PKG-INFO` & `pycep_parser-0.4.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycep-parser
-Version: 0.4.0
+Version: 0.4.1a0
 Summary: A Python based Bicep parser
 Home-page: https://github.com/gruebel/pycep
 License: Apache-2.0
 Keywords: bicep,parser,lark
 Author: Anton Grübel
 Author-email: anton.gruebel@gmail.com
 Requires-Python: >=3.7,<4.0
```

