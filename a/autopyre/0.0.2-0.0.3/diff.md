# Comparing `tmp/autopyre-0.0.2.tar.gz` & `tmp/autopyre-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopyre-0.0.2.tar", last modified: Sun Jun 18 10:20:58 2023, max compression
+gzip compressed data, was "autopyre-0.0.3.tar", last modified: Sun Jun 18 11:38:31 2023, max compression
```

## Comparing `autopyre-0.0.2.tar` & `autopyre-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-18 10:20:58.410599 autopyre-0.0.2/
--rw-r--r--   0 root         (0) staff       (20)     1229 2023-06-17 05:07:33.000000 autopyre-0.0.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     1146 2023-06-18 10:20:58.410086 autopyre-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)        0 2023-06-18 10:12:27.000000 autopyre-0.0.2/README.rst
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-18 10:20:58.392303 autopyre-0.0.2/autopyre.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1146 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      632 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       43 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-06-17 06:09:36.000000 autopyre-0.0.2/autopyre.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       34 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       19 2023-06-18 10:20:58.000000 autopyre-0.0.2/autopyre.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)   191696 2023-06-18 10:16:48.000000 autopyre-0.0.2/autopyre.py
--rw-r--r--   0 root         (0) staff       (20)       86 2023-06-18 08:17:48.000000 autopyre-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)   107905 2023-06-18 10:16:39.000000 autopyre-0.0.2/pyrestyle.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-06-18 10:20:58.410759 autopyre-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     3611 2023-06-18 10:03:42.000000 autopyre-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-18 10:20:58.409232 autopyre-0.0.2/test/
--rw-r--r--   0 root         (0) staff       (20)     1002 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_W701.py
--rw-r--r--   0 root         (0) staff       (20)      683 2023-06-17 12:18:53.000000 autopyre-0.0.2/test/test_W702.py
--rw-r--r--   0 root         (0) staff       (20)     1383 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_W7_comment.py
--rw-r--r--   0 root         (0) staff       (20)     1046 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_aliasing.py
--rw-r--r--   0 root         (0) staff       (20)      977 2023-06-17 11:33:16.000000 autopyre-0.0.2/test/test_all.py
--rw-r--r--   0 root         (0) staff       (20)     4570 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_ast.py
--rw-r--r--   0 root         (0) staff       (20)      999 2023-06-17 08:05:17.000000 autopyre-0.0.2/test/test_import_user.py
--rw-r--r--   0 root         (0) staff       (20)      760 2023-06-17 08:15:01.000000 autopyre-0.0.2/test/test_import_userlib.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_overriding_other_file.py
--rw-r--r--   0 root         (0) staff       (20)      113 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_overriding_other_file_super.py
--rw-r--r--   0 root         (0) staff       (20)     1287 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_overriding_same_file.py
--rw-r--r--   0 root         (0) staff       (20)      584 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_same_class_name.py
--rw-r--r--   0 root         (0) staff       (20)      501 2023-06-17 05:37:52.000000 autopyre-0.0.2/test/test_same_function_name.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 11:38:31.765377 autopyre-0.0.3/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1229 2023-06-17 05:07:33.000000 autopyre-0.0.3/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1136 2023-06-18 11:38:31.764649 autopyre-0.0.3/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 10:12:27.000000 autopyre-0.0.3/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 11:38:31.750143 autopyre-0.0.3/autopyre.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1136 2023-06-18 11:38:31.000000 autopyre-0.0.3/autopyre.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      617 2023-06-18 11:38:31.000000 autopyre-0.0.3/autopyre.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 11:38:31.000000 autopyre-0.0.3/autopyre.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       43 2023-06-18 11:38:31.000000 autopyre-0.0.3/autopyre.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-17 06:09:36.000000 autopyre-0.0.3/autopyre.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       34 2023-06-18 11:38:31.000000 autopyre-0.0.3/autopyre.egg-info/requires.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        9 2023-06-18 11:38:31.000000 autopyre-0.0.3/autopyre.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   191696 2023-06-18 11:21:47.000000 autopyre-0.0.3/autopyre.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-18 11:21:53.000000 autopyre-0.0.3/pyrestyle.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 11:38:31.765524 autopyre-0.0.3/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     3533 2023-06-18 11:35:54.000000 autopyre-0.0.3/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 11:38:31.763646 autopyre-0.0.3/test/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1002 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_W701.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      683 2023-06-17 12:18:53.000000 autopyre-0.0.3/test/test_W702.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1383 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_W7_comment.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1046 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_aliasing.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      977 2023-06-17 11:33:16.000000 autopyre-0.0.3/test/test_all.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     4570 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_ast.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      999 2023-06-17 08:05:17.000000 autopyre-0.0.3/test/test_import_user.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      760 2023-06-17 08:15:01.000000 autopyre-0.0.3/test/test_import_userlib.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      255 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_overriding_other_file.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      113 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_overriding_other_file_super.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1287 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_overriding_same_file.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      584 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_same_class_name.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      501 2023-06-17 05:37:52.000000 autopyre-0.0.3/test/test_same_function_name.py
```

### Comparing `autopyre-0.0.2/LICENSE` & `autopyre-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/PKG-INFO` & `autopyre-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
-Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
+Keywords: automation,pep8,format,pycodestyle,autopyre
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopyre-0.0.2/autopyre.egg-info/PKG-INFO` & `autopyre-0.0.3/autopyre.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autopyre
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool that automatically formats Python code to conform to the PEP 8 style guide and This project based on autopep8
 Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
 Author: Hideo Hattori, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: MIT
-Keywords: automation,pep8,format,pycodestyle,autopyre,pyrestyle
+Keywords: automation,pep8,format,pycodestyle,autopyre
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `autopyre-0.0.2/autopyre.egg-info/SOURCES.txt` & `autopyre-0.0.3/autopyre.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.rst
 autopyre.py
-pyproject.toml
 pyrestyle.py
 setup.py
 autopyre.egg-info/PKG-INFO
 autopyre.egg-info/SOURCES.txt
 autopyre.egg-info/dependency_links.txt
 autopyre.egg-info/entry_points.txt
 autopyre.egg-info/not-zip-safe
```

### Comparing `autopyre-0.0.2/autopyre.py` & `autopyre-0.0.3/autopyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 import pyrestyle
 from pyrestyle import STARTSWITH_INDENT_STATEMENT_REGEX
 
 import libcst as cst  # pip install libcst
 import string
 from termcolor import colored  # pip install termcolor
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 CR = '\r'
 LF = '\n'
 CRLF = '\r\n'
```

### Comparing `autopyre-0.0.2/pyrestyle.py` & `autopyre-0.0.3/pyrestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
```

### Comparing `autopyre-0.0.2/setup.py` & `autopyre-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,38 +51,36 @@
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Topic :: Software Development :: Libraries :: Python Modules',
             'Topic :: Software Development :: Quality Assurance',
         ],
-        keywords='automation, pep8, format, pycodestyle, autopyre, pyrestyle',
+        keywords='automation, pep8, format, pycodestyle, autopyre',
         install_requires=INSTALL_REQUIRES,
         python_requires=">=3.6",
         test_suite='test.test_autopyre',
-        py_modules=['autopyre', 'pyrestyle'],
+        py_modules=['autopyre'],
         zip_safe=False,
         entry_points={'console_scripts': ['autopyre = autopyre:main']},
     )
     setup(
         name='pyrestyle',
         version=get_version(),
-        description="Python style guide checker",
+        description="Python style guide checker and This project based on autopep8",
         long_description=readme.read(),
         keywords='pyrestyle, pep8, PEP 8, PEP-8, PEP8',
         author='Johann C. Rocholl',
-        author_email='johann@rocholl.net',
-        maintainer='Ian Lee',
-        maintainer_email='IanLee1521@gmail.com',
+        author_email='kys00919@gmail.com',
         url='https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08',
-        license='Expat license',
+        license='MIT',
         py_modules=['pyrestyle'],
         include_package_data=True,
         zip_safe=False,
-        python_requires='>=3.7',
+        python_requires='>=3.6',
         entry_points={
             'console_scripts': [
                 'pyrestyle = pyrestyle:_main',
             ],
         },
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `autopyre-0.0.2/test/test_W701.py` & `autopyre-0.0.3/test/test_W701.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_W702.py` & `autopyre-0.0.3/test/test_W702.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_W7_comment.py` & `autopyre-0.0.3/test/test_W7_comment.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_aliasing.py` & `autopyre-0.0.3/test/test_aliasing.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_all.py` & `autopyre-0.0.3/test/test_all.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_ast.py` & `autopyre-0.0.3/test/test_ast.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_import_user.py` & `autopyre-0.0.3/test/test_import_user.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_import_userlib.py` & `autopyre-0.0.3/test/test_import_userlib.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_overriding_same_file.py` & `autopyre-0.0.3/test/test_overriding_same_file.py`

 * *Files identical despite different names*

### Comparing `autopyre-0.0.2/test/test_same_class_name.py` & `autopyre-0.0.3/test/test_same_class_name.py`

 * *Files identical despite different names*

