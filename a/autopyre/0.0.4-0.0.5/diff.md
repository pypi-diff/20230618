# Comparing `tmp/autopyre-0.0.4.tar.gz` & `tmp/autopyre-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.4.tar", last modified: Sun Jun 18 12:51:45 2023, max compression
+gzip compressed data, was "autopyre-0.0.5.tar", last modified: Sun Jun 18 12:54:38 2023, max compression
```

## Comparing `autopyre-0.0.4.tar` & `autopyre-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:51:45.402835 autopyre-0.0.4/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.4/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 12:51:45.401415 autopyre-0.0.4/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.4/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:51:45.395429 autopyre-0.0.4/autopyre.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 12:51:44.000000 autopyre-0.0.4/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 12:51:45.000000 autopyre-0.0.4/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:51:44.000000 autopyre-0.0.4/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 12:51:44.000000 autopyre-0.0.4/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:51:44.000000 autopyre-0.0.4/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       34 2023-06-18 12:51:44.000000 autopyre-0.0.4/autopyre.egg-info/requires.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       19 2023-06-18 12:51:44.000000 autopyre-0.0.4/autopyre.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   191777 2023-06-18 12:51:09.000000 autopyre-0.0.4/autopyre.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 12:51:45.406189 autopyre-0.0.4/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     2077 2023-06-18 12:48:42.000000 autopyre-0.0.4/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:54:38.898283 autopyre-0.0.5/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1250 2023-06-18 12:46:39.000000 autopyre-0.0.5/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 12:54:38.897501 autopyre-0.0.5/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:48:08.000000 autopyre-0.0.5/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:54:38.894724 autopyre-0.0.5/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1146 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      264 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       34 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 12:54:38.000000 autopyre-0.0.5/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   191821 2023-06-18 12:53:59.000000 autopyre-0.0.5/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 12:54:38.904288 autopyre-0.0.5/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     2064 2023-06-18 12:54:20.000000 autopyre-0.0.5/setup.py
```

### Comparing `autopyre-0.0.4/LICENSE` & `autopyre-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.4/PKG-INFO` & `autopyre-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.4/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.5/autopyre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
 Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autopyre-0.0.4/autopyre.py` & `autopyre-0.0.5/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
 
 
@@ -1953,14 +1953,15 @@
         if isinstance(node, ast.Import):
             for alias in node.names:
                 imported_module = alias.name
                 print(target_file, imported_module)
                 if target_file == imported_module or '.' + target_file in imported_module:
                     return True
         elif isinstance(node, ast.ImportFrom):
+            print(node.module, target_file)
             if node.module == target_file or '.' + target_file in node.module:
                 return True
 
     return False
 
 
 # 추가한 부분 - 김위성 - 식별자, 참조되는 식별자를 모두 저장
```

### Comparing `autopyre-0.0.4/setup.py` & `autopyre-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,11 +49,11 @@
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Quality Assurance',
         ],
         keywords='automation, pep8, format, pycodestyle, autopyre, pyrestyle',
         install_requires=INSTALL_REQUIRES,
         python_requires=">=3.6",
         test_suite='test.test_autopyre',
-        py_modules=['autopyre', 'pyrestyle'],
+        py_modules=['autopyre'],
         zip_safe=False,
         entry_points={'console_scripts': ['autopyre = autopyre:main']},
     )
```

