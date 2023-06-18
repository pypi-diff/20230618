# Comparing `tmp/joltedmod-0.2.1.1.tar.gz` & `tmp/joltedmod-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joltedmod-0.2.1.1.tar", max compression
+gzip compressed data, was "joltedmod-0.2.2.tar", max compression
```

## Comparing `joltedmod-0.2.1.1.tar` & `joltedmod-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.2.1.1/LICENSE
--rw-r--r--   0        0        0     2012 2023-06-18 07:56:10.874764 joltedmod-0.2.1.1/README.md
--rw-r--r--   0        0        0     1344 2023-06-17 15:04:17.835987 joltedmod-0.2.1.1/jolted_mod/LLM_service.py
--rw-r--r--   0        0        0      412 2023-06-18 14:40:05.820570 joltedmod-0.2.1.1/jolted_mod/__init__.py
--rw-r--r--   0        0        0     3749 2023-06-18 08:19:58.255349 joltedmod-0.2.1.1/jolted_mod/block.py
--rw-r--r--   0        0        0      606 2023-06-18 08:18:31.554627 joltedmod-0.2.1.1/jolted_mod/block_factory.py
--rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.2.1.1/jolted_mod/cell_type.py
--rw-r--r--   0        0        0     1934 2023-06-17 17:42:19.311605 joltedmod-0.2.1.1/jolted_mod/config.py
--rw-r--r--   0        0        0     7925 2023-06-18 08:24:25.496650 joltedmod-0.2.1.1/jolted_mod/content_generator.py
--rw-r--r--   0        0        0     4855 2023-06-18 08:25:07.509677 joltedmod-0.2.1.1/jolted_mod/main.py
--rw-r--r--   0        0        0       93 2023-06-17 15:54:34.751488 joltedmod-0.2.1.1/jolted_mod/module_types.py
--rw-r--r--   0        0        0     9644 2023-06-18 14:57:03.509185 joltedmod-0.2.1.1/jolted_mod/template_generator.py
--rw-r--r--   0        0        0      687 2023-06-18 14:57:18.808895 joltedmod-0.2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 joltedmod-0.2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2023-06-01 12:22:59.095108 joltedmod-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2012 2023-06-18 07:56:10.874764 joltedmod-0.2.2/README.md
+-rw-r--r--   0        0        0     1344 2023-06-17 15:04:17.835987 joltedmod-0.2.2/jolted_mod/LLM_service.py
+-rw-r--r--   0        0        0      412 2023-06-18 14:40:05.820570 joltedmod-0.2.2/jolted_mod/__init__.py
+-rw-r--r--   0        0        0     3749 2023-06-18 08:19:58.255349 joltedmod-0.2.2/jolted_mod/block.py
+-rw-r--r--   0        0        0      606 2023-06-18 08:18:31.554627 joltedmod-0.2.2/jolted_mod/block_factory.py
+-rw-r--r--   0        0        0       91 2023-06-01 12:22:59.233084 joltedmod-0.2.2/jolted_mod/cell_type.py
+-rw-r--r--   0        0        0     1934 2023-06-17 17:42:19.311605 joltedmod-0.2.2/jolted_mod/config.py
+-rw-r--r--   0        0        0     7925 2023-06-18 08:24:25.496650 joltedmod-0.2.2/jolted_mod/content_generator.py
+-rw-r--r--   0        0        0     4855 2023-06-18 08:25:07.509677 joltedmod-0.2.2/jolted_mod/main.py
+-rw-r--r--   0        0        0       93 2023-06-17 15:54:34.751488 joltedmod-0.2.2/jolted_mod/module_types.py
+-rw-r--r--   0        0        0     9644 2023-06-18 14:57:03.509185 joltedmod-0.2.2/jolted_mod/template_generator.py
+-rw-r--r--   0        0        0      685 2023-06-18 15:03:38.707349 joltedmod-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 joltedmod-0.2.2/PKG-INFO
```

### Comparing `joltedmod-0.2.1.1/LICENSE` & `joltedmod-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/README.md` & `joltedmod-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/LLM_service.py` & `joltedmod-0.2.2/jolted_mod/LLM_service.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/block.py` & `joltedmod-0.2.2/jolted_mod/block.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/block_factory.py` & `joltedmod-0.2.2/jolted_mod/block_factory.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/config.py` & `joltedmod-0.2.2/jolted_mod/config.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/content_generator.py` & `joltedmod-0.2.2/jolted_mod/content_generator.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/main.py` & `joltedmod-0.2.2/jolted_mod/main.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/jolted_mod/template_generator.py` & `joltedmod-0.2.2/jolted_mod/template_generator.py`

 * *Files identical despite different names*

### Comparing `joltedmod-0.2.1.1/pyproject.toml` & `joltedmod-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JoltEdMod"
-version = "0.2.1.1"
+version = "0.2.2"
 description = "JoltEd self-documenting learning module"
 authors = ["Nathan Laundry"]
 license = "MIT" 
 readme = "README.md"
 packages = [{include = "jolted_mod"}]
 
 [tool.poetry.dependencies]
```

### Comparing `joltedmod-0.2.1.1/PKG-INFO` & `joltedmod-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joltedmod
-Version: 0.2.1.1
+Version: 0.2.2
 Summary: JoltEd self-documenting learning module
 License: MIT
 Author: Nathan Laundry
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

