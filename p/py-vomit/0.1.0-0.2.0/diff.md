# Comparing `tmp/py-vomit-0.1.0.tar.gz` & `tmp/py-vomit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-vomit-0.1.0.tar", last modified: Thu Jun  8 15:07:50 2023, max compression
+gzip compressed data, was "py-vomit-0.2.0.tar", last modified: Sun Jun 18 18:10:19 2023, max compression
```

## Comparing `py-vomit-0.1.0.tar` & `py-vomit-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-08 15:07:50.184786 py-vomit-0.1.0/
--rw-r--r--   0 roko      (1000) roko      (1000)     1060 2023-06-08 11:40:04.000000 py-vomit-0.1.0/LICENSE
--rw-r--r--   0 roko      (1000) roko      (1000)      667 2023-06-08 15:07:50.184786 py-vomit-0.1.0/PKG-INFO
--rw-r--r--   0 roko      (1000) roko      (1000)      244 2023-06-08 15:07:26.000000 py-vomit-0.1.0/README.md
--rw-r--r--   0 roko      (1000) roko      (1000)      496 2023-06-08 11:55:20.000000 py-vomit-0.1.0/pyproject.toml
--rw-r--r--   0 roko      (1000) roko      (1000)      704 2023-06-08 15:07:50.188120 py-vomit-0.1.0/setup.cfg
--rw-r--r--   0 roko      (1000) roko      (1000)       68 2023-06-08 11:32:05.000000 py-vomit-0.1.0/setup.py
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-08 15:07:50.181453 py-vomit-0.1.0/src/
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-08 15:07:50.184786 py-vomit-0.1.0/src/py_vomit.egg-info/
--rw-r--r--   0 roko      (1000) roko      (1000)      667 2023-06-08 15:07:50.000000 py-vomit-0.1.0/src/py_vomit.egg-info/PKG-INFO
--rw-r--r--   0 roko      (1000) roko      (1000)      355 2023-06-08 15:07:50.000000 py-vomit-0.1.0/src/py_vomit.egg-info/SOURCES.txt
--rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-08 15:07:50.000000 py-vomit-0.1.0/src/py_vomit.egg-info/dependency_links.txt
--rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-08 15:02:31.000000 py-vomit-0.1.0/src/py_vomit.egg-info/not-zip-safe
--rw-r--r--   0 roko      (1000) roko      (1000)       80 2023-06-08 15:07:50.000000 py-vomit-0.1.0/src/py_vomit.egg-info/requires.txt
--rw-r--r--   0 roko      (1000) roko      (1000)        6 2023-06-08 15:07:50.000000 py-vomit-0.1.0/src/py_vomit.egg-info/top_level.txt
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-08 15:07:50.184786 py-vomit-0.1.0/src/vomit/
--rw-r--r--   0 roko      (1000) roko      (1000)     5545 2023-06-08 12:33:11.000000 py-vomit-0.1.0/src/vomit/__init__.py
--rw-r--r--   0 roko      (1000) roko      (1000)     1519 2023-06-08 11:45:09.000000 py-vomit-0.1.0/src/vomit/__main__.py
--rw-r--r--   0 roko      (1000) roko      (1000)        0 2023-06-08 11:28:38.000000 py-vomit-0.1.0/src/vomit/py.typed
-drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-08 15:07:50.184786 py-vomit-0.1.0/tests/
--rw-r--r--   0 roko      (1000) roko      (1000)     1506 2023-06-08 12:36:06.000000 py-vomit-0.1.0/tests/test_fuctionality.py
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.983970 py-vomit-0.2.0/
+-rw-r--r--   0 roko      (1000) roko      (1000)     1060 2023-06-08 11:40:04.000000 py-vomit-0.2.0/LICENSE
+-rw-r--r--   0 roko      (1000) roko      (1000)     1921 2023-06-18 18:10:19.983970 py-vomit-0.2.0/PKG-INFO
+-rw-r--r--   0 roko      (1000) roko      (1000)     1497 2023-06-18 18:00:10.000000 py-vomit-0.2.0/README.md
+-rw-r--r--   0 roko      (1000) roko      (1000)      496 2023-06-08 11:55:20.000000 py-vomit-0.2.0/pyproject.toml
+-rw-r--r--   0 roko      (1000) roko      (1000)      704 2023-06-18 18:10:19.987303 py-vomit-0.2.0/setup.cfg
+-rw-r--r--   0 roko      (1000) roko      (1000)       68 2023-06-08 11:32:05.000000 py-vomit-0.2.0/setup.py
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.973970 py-vomit-0.2.0/src/
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.980636 py-vomit-0.2.0/src/py_vomit.egg-info/
+-rw-r--r--   0 roko      (1000) roko      (1000)     1921 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/PKG-INFO
+-rw-r--r--   0 roko      (1000) roko      (1000)      376 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/SOURCES.txt
+-rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/dependency_links.txt
+-rw-r--r--   0 roko      (1000) roko      (1000)        1 2023-06-08 15:02:31.000000 py-vomit-0.2.0/src/py_vomit.egg-info/not-zip-safe
+-rw-r--r--   0 roko      (1000) roko      (1000)       80 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/requires.txt
+-rw-r--r--   0 roko      (1000) roko      (1000)        6 2023-06-18 18:10:19.000000 py-vomit-0.2.0/src/py_vomit.egg-info/top_level.txt
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.983970 py-vomit-0.2.0/src/vomit/
+-rw-r--r--   0 roko      (1000) roko      (1000)     5791 2023-06-18 17:57:07.000000 py-vomit-0.2.0/src/vomit/__init__.py
+-rw-r--r--   0 roko      (1000) roko      (1000)     2048 2023-06-18 18:04:49.000000 py-vomit-0.2.0/src/vomit/__main__.py
+-rw-r--r--   0 roko      (1000) roko      (1000)        0 2023-06-08 11:28:38.000000 py-vomit-0.2.0/src/vomit/py.typed
+drwxr-xr-x   0 roko      (1000) roko      (1000)        0 2023-06-18 18:10:19.983970 py-vomit-0.2.0/tests/
+-rw-r--r--   0 roko      (1000) roko      (1000)     1506 2023-06-18 17:58:18.000000 py-vomit-0.2.0/tests/test_fuctionality.py
+-rw-r--r--   0 roko      (1000) roko      (1000)      587 2023-06-18 18:03:31.000000 py-vomit-0.2.0/tests/test_walker.py
```

### Comparing `py-vomit-0.1.0/LICENSE` & `py-vomit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-vomit-0.1.0/src/vomit/__init__.py` & `py-vomit-0.2.0/src/vomit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import ast
 import unicodedata
 from random import choice
+from os import walk, path
+from typing import Iterator
 
 
 def to_utf8(code: str) -> str:
     visitor = _Visitor(fw=False)
     return _action(code, visitor)
 
 
 def to_unicode(code: str) -> str:
     visitor = _Visitor()
     return _action(code, visitor)
 
 
+def walker(source: str) -> Iterator[str]:
+    for root, _, files in walk(source):
+        for name in files:
+            if name.endswith('.py'):
+                yield path.join(root, name)
+
+
 def _action(code: str, visitor: ast.NodeVisitor) -> str:
     tree = ast.parse(code)
     visitor.visit(tree)
     return ast.unparse(tree)
 
 
 class _Visitor(ast.NodeVisitor):
```

### Comparing `py-vomit-0.1.0/tests/test_fuctionality.py` & `py-vomit-0.2.0/tests/test_fuctionality.py`

 * *Files identical despite different names*

