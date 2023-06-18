# Comparing `tmp/autopyre-0.0.8.tar.gz` & `tmp/autopyre-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.8.tar", last modified: Sun Jun 18 14:50:35 2023, max compression
+gzip compressed data, was "autopyre-0.0.9.tar", last modified: Sun Jun 18 15:01:02 2023, max compression
```

## Comparing `autopyre-0.0.8.tar` & `autopyre-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:50:35.924500 autopyre-0.0.8/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.8/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:50:35.922359 autopyre-0.0.8/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.8/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 14:50:35.920190 autopyre-0.0.8/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 14:50:35.000000 autopyre-0.0.8/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191843 2023-06-18 14:50:06.000000 autopyre-0.0.8/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 14:50:35.942019 autopyre-0.0.8/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 14:00:07.000000 autopyre-0.0.8/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 15:01:02.722979 autopyre-0.0.9/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.9/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 15:01:02.720747 autopyre-0.0.9/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.9/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 15:01:02.718770 autopyre-0.0.9/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1158 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       51 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 15:01:02.000000 autopyre-0.0.9/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   191861 2023-06-18 15:00:44.000000 autopyre-0.0.9/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 15:01:02.728448 autopyre-0.0.9/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2098 2023-06-18 14:00:07.000000 autopyre-0.0.9/setup.py
```

### Comparing `autopyre-0.0.8/LICENSE` & `autopyre-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.8/PKG-INFO` & `autopyre-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.8/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.9/autopyre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/autopyre.py
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.8/autopyre.py` & `autopyre-0.0.9/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -1957,18 +1957,19 @@
         if isinstance(node, ast.Import):
             
             for alias in node.names:
                 imported_module = alias.name
                 if target_file == imported_module or '.' + target_file in imported_module:
                     return True
         elif isinstance(node, ast.ImportFrom):
-            if node.module is None: 
+            try:
+                if node.module == target_file or '.' + target_file in node.module:
+                    return True
+            except TypeError:
                 pass
-            if node.module == target_file or '.' + target_file in node.module:
-                return True
     
     return False
 
 
 # 추가한 부분 - 김위성 - 식별자, 참조되는 식별자를 모두 저장
 def analyze_file(file_path):
     with open(file_path, 'r', errors='ignore') as file:
```

### Comparing `autopyre-0.0.8/setup.py` & `autopyre-0.0.9/setup.py`

 * *Files identical despite different names*

