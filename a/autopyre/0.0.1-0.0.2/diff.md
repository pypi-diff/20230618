# Comparing `tmp/autopyre-0.0.1.tar.gz` & `tmp/autopyre-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.1.tar", last modified: Sun Jun 18 10:12:32 2023, max compression
+gzip compressed data, was "autopyre-0.0.2.tar", last modified: Sun Jun 18 10:20:58 2023, max compression
```

## Comparing `autopyre-0.0.1.tar` & `autopyre-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 10:12:32.723572 autopyre-0.0.1/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1229 2023-06-17 05:07:33.000000 autopyre-0.0.1/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 10:12:32.722928 autopyre-0.0.1/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 10:12:27.000000 autopyre-0.0.1/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 10:12:32.704334 autopyre-0.0.1/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 10:12:32.000000 autopyre-0.0.1/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      632 2023-06-18 10:12:32.000000 autopyre-0.0.1/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 10:12:32.000000 autopyre-0.0.1/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 10:12:32.000000 autopyre-0.0.1/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-17 06:09:36.000000 autopyre-0.0.1/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       34 2023-06-18 10:12:32.000000 autopyre-0.0.1/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       19 2023-06-18 10:12:32.000000 autopyre-0.0.1/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191696 2023-06-18 07:25:16.000000 autopyre-0.0.1/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       86 2023-06-18 08:17:48.000000 autopyre-0.0.1/pyproject.toml
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-18 09:11:28.000000 autopyre-0.0.1/pyrestyle.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 10:12:32.723722 autopyre-0.0.1/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     3611 2023-06-18 10:03:42.000000 autopyre-0.0.1/setup.py
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 10:12:32.721666 autopyre-0.0.1/test/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1002 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_W701.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      683 2023-06-17 12:18:53.000000 autopyre-0.0.1/test/test_W702.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1383 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_W7_comment.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1046 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_aliasing.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      977 2023-06-17 11:33:16.000000 autopyre-0.0.1/test/test_all.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     4570 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_ast.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      999 2023-06-17 08:05:17.000000 autopyre-0.0.1/test/test_import_user.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      760 2023-06-17 08:15:01.000000 autopyre-0.0.1/test/test_import_userlib.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      255 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_overriding_other_file.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      113 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_overriding_other_file_super.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1287 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_overriding_same_file.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      584 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_same_class_name.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      501 2023-06-17 05:37:52.000000 autopyre-0.0.1/test/test_same_function_name.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-18 10:20:58.410599 autopyre-0.0.2/
+-rw-r--r--   0 root         (0) staff       (20)     1229 2023-06-17 05:07:33.000000 autopyre-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     1146 2023-06-18 10:20:58.410086 autopyre-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-06-18 10:12:27.000000 autopyre-0.0.2/README.rst
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-18 10:20:58.392303 autopyre-0.0.2/autopyre.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1146 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      632 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       43 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-17 06:09:36.000000 autopyre-0.0.2/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       34 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)   191696 2023-06-18 10:16:48.000000 autopyre-0.0.2/autopyre.py
+-rw-r--r--   0 root         (0) staff       (20)       86 2023-06-18 08:17:48.000000 autopyre-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)   107905 2023-06-18 10:16:39.000000 autopyre-0.0.2/pyrestyle.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-06-18 10:20:58.410759 autopyre-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3611 2023-06-18 10:03:42.000000 autopyre-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-18 10:20:58.409232 autopyre-0.0.2/test/
+-rw-r--r--   0 root         (0) staff       (20)     1002 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_W701.py
+-rw-r--r--   0 root         (0) staff       (20)      683 2023-06-17 12:18:53.000000 autopyre-0.0.2/test/test_W702.py
+-rw-r--r--   0 root         (0) staff       (20)     1383 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_W7_comment.py
+-rw-r--r--   0 root         (0) staff       (20)     1046 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_aliasing.py
+-rw-r--r--   0 root         (0) staff       (20)      977 2023-06-17 11:33:16.000000 autopyre-0.0.2/test/test_all.py
+-rw-r--r--   0 root         (0) staff       (20)     4570 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_ast.py
+-rw-r--r--   0 root         (0) staff       (20)      999 2023-06-17 08:05:17.000000 autopyre-0.0.2/test/test_import_user.py
+-rw-r--r--   0 root         (0) staff       (20)      760 2023-06-17 08:15:01.000000 autopyre-0.0.2/test/test_import_userlib.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_overriding_other_file.py
+-rw-r--r--   0 root         (0) staff       (20)      113 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_overriding_other_file_super.py
+-rw-r--r--   0 root         (0) staff       (20)     1287 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_overriding_same_file.py
+-rw-r--r--   0 root         (0) staff       (20)      584 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_same_class_name.py
+-rw-r--r--   0 root         (0) staff       (20)      501 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_same_function_name.py
```

### Comparing `autopyre-0.0.1/LICENSE` & `autopyre-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/PKG-INFO` & `autopyre-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.1/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.2/autopyre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.1/autopyre.egg-info/SOURCES.txt` & `autopyre-0.0.2/autopyre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/autopyre.py` & `autopyre-0.0.2/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
```

### Comparing `autopyre-0.0.1/pyrestyle.py` & `autopyre-0.0.2/pyrestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
```

### Comparing `autopyre-0.0.1/setup.py` & `autopyre-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_W701.py` & `autopyre-0.0.2/test/test_W701.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_W702.py` & `autopyre-0.0.2/test/test_W702.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_W7_comment.py` & `autopyre-0.0.2/test/test_W7_comment.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_aliasing.py` & `autopyre-0.0.2/test/test_aliasing.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_all.py` & `autopyre-0.0.2/test/test_all.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_ast.py` & `autopyre-0.0.2/test/test_ast.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_import_user.py` & `autopyre-0.0.2/test/test_import_user.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_import_userlib.py` & `autopyre-0.0.2/test/test_import_userlib.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_overriding_same_file.py` & `autopyre-0.0.2/test/test_overriding_same_file.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.1/test/test_same_class_name.py` & `autopyre-0.0.2/test/test_same_class_name.py`

 * *Files identical despite different names*

