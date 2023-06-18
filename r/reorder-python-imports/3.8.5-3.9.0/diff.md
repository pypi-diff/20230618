# Comparing `tmp/reorder_python_imports-3.8.5.tar.gz` & `tmp/reorder_python_imports-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reorder_python_imports-3.8.5.tar", last modified: Thu Oct 13 23:56:24 2022, max compression
+gzip compressed data, was "reorder_python_imports-3.9.0.tar", last modified: Mon Oct 24 23:48:44 2022, max compression
```

## Comparing `reorder_python_imports-3.8.5.tar` & `reorder_python_imports-3.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-13 23:56:24.539815 reorder_python_imports-3.8.5/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-10-13 23:38:24.000000 reorder_python_imports-3.8.5/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7965 2022-10-13 23:56:24.539815 reorder_python_imports-3.8.5/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7341 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-13 23:56:24.539815 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7965 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      340 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       71 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       22 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       23 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)    27105 2022-10-13 23:56:24.000000 reorder_python_imports-3.8.5/reorder_python_imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1217 2022-10-13 23:56:24.539815 reorder_python_imports-3.8.5/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-10-13 23:38:24.000000 reorder_python_imports-3.8.5/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-24 23:48:44.462218 reorder_python_imports-3.9.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-07-01 18:25:36.000000 reorder_python_imports-3.9.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7965 2022-10-24 23:48:44.466216 reorder_python_imports-3.9.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7341 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2022-10-24 23:48:44.462218 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7965 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      340 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       71 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       22 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       23 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    27859 2022-10-24 23:48:44.000000 reorder_python_imports-3.9.0/reorder_python_imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1217 2022-10-24 23:48:44.466216 reorder_python_imports-3.9.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-07-01 18:25:36.000000 reorder_python_imports-3.9.0/setup.py
```

### Comparing `reorder_python_imports-3.8.5/LICENSE` & `reorder_python_imports-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reorder_python_imports-3.8.5/PKG-INFO` & `reorder_python_imports-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reorder_python_imports
-Version: 3.8.5
+Version: 3.9.0
 Summary: Tool for reordering python imports
 Home-page: https://github.com/asottile/reorder_python_imports
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.8.5
+    rev: v3.9.0
     hooks:
     -   id: reorder-python-imports
 ```
 
 ## What does it do?
 
 ### Separates imports into three sections
```

### Comparing `reorder_python_imports-3.8.5/README.md` & `reorder_python_imports-3.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.8.5
+    rev: v3.9.0
     hooks:
     -   id: reorder-python-imports
 ```
 
 ## What does it do?
 
 ### Separates imports into three sections
```

### Comparing `reorder_python_imports-3.8.5/reorder_python_imports.egg-info/PKG-INFO` & `reorder_python_imports-3.9.0/reorder_python_imports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reorder-python-imports
-Version: 3.8.5
+Version: 3.9.0
 Summary: Tool for reordering python imports
 Home-page: https://github.com/asottile/reorder_python_imports
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -58,15 +58,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.8.5
+    rev: v3.9.0
     hooks:
     -   id: reorder-python-imports
 ```
 
 ## What does it do?
 
 ### Separates imports into three sections
```

### Comparing `reorder_python_imports-3.8.5/reorder_python_imports.py` & `reorder_python_imports-3.9.0/reorder_python_imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -415,15 +415,15 @@
     'from __future__ import unicode_literals',
 ))
 REMOVALS[(3, 7)].add('from __future__ import generator_stop')
 # END GENERATED
 
 # GENERATED VIA generate-typing-rewrite-info
 # Using:
-#     flake8-typing-imports==1.13.0
+#     flake8-typing-imports==1.14.0
 #     mypy-extensions==0.4.3
 #     typing-extensions==4.4.0
 REPLACES[(3, 6)].update((
     'typing_extensions=typing:AsyncIterable',
     'typing_extensions=typing:AsyncIterator',
     'typing_extensions=typing:Awaitable',
     'typing_extensions=typing:ClassVar',
@@ -463,14 +463,33 @@
     'typing_extensions=typing:ParamSpecKwargs',
     'typing_extensions=typing:TypeAlias',
     'typing_extensions=typing:TypeGuard',
     'typing_extensions=typing:get_args',
     'typing_extensions=typing:get_origin',
     'typing_extensions=typing:is_typeddict',
 ))
+REPLACES[(3, 11)].update((
+    'typing_extensions=typing:Any',
+    'typing_extensions=typing:LiteralString',
+    'typing_extensions=typing:NamedTuple',
+    'typing_extensions=typing:Never',
+    'typing_extensions=typing:NotRequired',
+    'typing_extensions=typing:Required',
+    'typing_extensions=typing:Self',
+    'typing_extensions=typing:TypedDict',
+    'typing_extensions=typing:Unpack',
+    'typing_extensions=typing:assert_never',
+    'typing_extensions=typing:assert_type',
+    'typing_extensions=typing:clear_overloads',
+    'typing_extensions=typing:dataclass_transform',
+    'typing_extensions=typing:final',
+    'typing_extensions=typing:get_overloads',
+    'typing_extensions=typing:overload',
+    'typing_extensions=typing:reveal_type',
+))
 # END GENERATED
 
 # GENERATED VIA generate-typing-pep585-rewrites
 REPLACES[(3, 9)].update((
     'typing=collections.abc:AsyncGenerator',
     'typing=collections.abc:AsyncIterable',
     'typing=collections.abc:AsyncIterator',
@@ -532,15 +551,15 @@
     'from builtins import str',
     'from builtins import super',
     'from builtins import zip',
 ))
 # END GENERATED
 
 # GENERATED VIA generate-six-info
-# Using six==1.15.0
+# Using six==1.16.0
 REMOVALS[(3,)].update((
     'from six import callable',
     'from six import next',
     'from six.moves import filter',
     'from six.moves import input',
     'from six.moves import map',
     'from six.moves import range',
```

### Comparing `reorder_python_imports-3.8.5/setup.cfg` & `reorder_python_imports-3.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = reorder_python_imports
-version = 3.8.5
+version = 3.9.0
 description = Tool for reordering python imports
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/reorder_python_imports
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

