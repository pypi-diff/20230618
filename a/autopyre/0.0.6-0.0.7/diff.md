# Comparing `tmp/autopyre-0.0.6.tar.gz` & `tmp/autopyre-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.6.tar", last modified: Sun Jun 18 13:53:03 2023, max compression
+gzip compressed data, was "autopyre-0.0.7.tar", last modified: Sun Jun 18 14:00:53 2023, max compression
```

## Comparing `autopyre-0.0.6.tar` & `autopyre-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 13:53:03.950159 autopyre-0.0.6/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.6/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 13:53:03.949713 autopyre-0.0.6/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.6/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 13:53:03.948906 autopyre-0.0.6/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 13:53:03.000000 autopyre-0.0.6/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191634 2023-06-18 13:53:01.000000 autopyre-0.0.6/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 13:53:03.950301 autopyre-0.0.6/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 13:13:06.000000 autopyre-0.0.6/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:00:53.123075 autopyre-0.0.7/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.7/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:00:53.122012 autopyre-0.0.7/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.7/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:00:53.120051 autopyre-0.0.7/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 14:00:53.000000 autopyre-0.0.7/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 14:00:52.000000 autopyre-0.0.7/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   191748 2023-06-18 14:00:36.000000 autopyre-0.0.7/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 14:00:53.123297 autopyre-0.0.7/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 14:00:07.000000 autopyre-0.0.7/setup.py
```

### Comparing `autopyre-0.0.6/LICENSE` & `autopyre-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.6/PKG-INFO` & `autopyre-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.6/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.7/autopyre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.6/autopyre.py` & `autopyre-0.0.7/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.6'
+__version__ = '0.0.7'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -1948,14 +1948,16 @@
     except SyntaxError:
         return False
     
     for node in ast.walk(tree):
         if isinstance(node, ast.Import):
             for alias in node.names:
                 imported_module = alias.name
+                print('imported_module : ', imported_module)
+                print('target_file : ', target_file)
                 if target_file == imported_module or '.' + target_file in imported_module:
                     return True
         elif isinstance(node, ast.ImportFrom):
             if node.module == target_file or '.' + target_file in node.module:
                 return True
 
     return False
```

### Comparing `autopyre-0.0.6/setup.py` & `autopyre-0.0.7/setup.py`

 * *Files identical despite different names*

