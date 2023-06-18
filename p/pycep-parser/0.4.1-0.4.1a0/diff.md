# Comparing `tmp/pycep_parser-0.4.1.tar.gz` & `tmp/pycep_parser-0.4.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycep_parser-0.4.1.tar", max compression
+gzip compressed data, was "pycep_parser-0.4.1a0.tar", max compression
```

## Comparing `pycep_parser-0.4.1.tar` & `pycep_parser-0.4.1a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10834 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/LICENSE
--rw-r--r--   0        0        0     1511 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/README.md
--rw-r--r--   0        0        0       57 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/__init__.py
--rw-r--r--   0        0        0    12506 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/bicep.lark
--rw-r--r--   0        0        0     1854 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/main.py
--rw-r--r--   0        0        0        0 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/py.typed
--rw-r--r--   0        0        0    56086 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/transformer.py
--rw-r--r--   0        0        0    23875 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/typing.py
--rw-r--r--   0        0        0      274 2023-06-18 17:51:25.692396 pycep_parser-0.4.1/pycep/validator.py
--rw-r--r--   0        0        0     1459 2023-06-18 17:51:39.316426 pycep_parser-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 pycep_parser-0.4.1/PKG-INFO
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

### Comparing `pycep_parser-0.4.1/LICENSE` & `pycep_parser-0.4.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.1/README.md` & `pycep_parser-0.4.1a0/README.md`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.1/pycep/bicep.lark` & `pycep_parser-0.4.1a0/pycep/bicep.lark`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.1/pycep/main.py` & `pycep_parser-0.4.1a0/pycep/main.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.1/pycep/transformer.py` & `pycep_parser-0.4.1a0/pycep/transformer.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.1/pycep/typing.py` & `pycep_parser-0.4.1a0/pycep/typing.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.4.1/pyproject.toml` & `pycep_parser-0.4.1a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycep-parser"
-version = "0.4.1"
+version = "0.4.1a0"
 description = "A Python based Bicep parser"
 authors = ["Anton Grübel <anton.gruebel@gmail.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 
 packages = [
```

### Comparing `pycep_parser-0.4.1/PKG-INFO` & `pycep_parser-0.4.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycep-parser
-Version: 0.4.1
+Version: 0.4.1a0
 Summary: A Python based Bicep parser
 Home-page: https://github.com/gruebel/pycep
 License: Apache-2.0
 Keywords: bicep,parser,lark
 Author: Anton Grübel
 Author-email: anton.gruebel@gmail.com
 Requires-Python: >=3.7,<4.0
```

