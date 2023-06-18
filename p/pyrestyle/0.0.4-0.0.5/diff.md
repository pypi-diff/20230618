# Comparing `tmp/pyrestyle-0.0.4.tar.gz` & `tmp/pyrestyle-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestyle-0.0.4.tar", last modified: Sun Jun 18 12:43:45 2023, max compression
+gzip compressed data, was "pyrestyle-0.0.5.tar", last modified: Sun Jun 18 13:18:04 2023, max compression
```

## Comparing `pyrestyle-0.0.4.tar` & `pyrestyle-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:43:45.274356 pyrestyle-0.0.4/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.4/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      914 2023-06-18 12:43:45.273976 pyrestyle-0.0.4/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.4/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:43:45.272784 pyrestyle-0.0.4/pyrestyle.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      914 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      240 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-18 12:37:59.000000 pyrestyle-0.0.4/pyrestyle.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 12:43:45.274458 pyrestyle-0.0.4/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1678 2023-06-18 12:43:41.000000 pyrestyle-0.0.4/setup.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 13:18:04.402259 pyrestyle-0.0.5/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.5/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-18 13:18:04.401638 pyrestyle-0.0.5/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.5/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 13:18:04.400647 pyrestyle-0.0.5/pyrestyle.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      937 2023-06-18 13:18:03.000000 pyrestyle-0.0.5/pyrestyle.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      240 2023-06-18 13:18:04.000000 pyrestyle-0.0.5/pyrestyle.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:18:03.000000 pyrestyle-0.0.5/pyrestyle.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-18 13:18:03.000000 pyrestyle-0.0.5/pyrestyle.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 13:18:03.000000 pyrestyle-0.0.5/pyrestyle.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-18 13:18:03.000000 pyrestyle-0.0.5/pyrestyle.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-18 13:14:29.000000 pyrestyle-0.0.5/pyrestyle.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 13:18:04.402630 pyrestyle-0.0.5/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1701 2023-06-18 13:14:10.000000 pyrestyle-0.0.5/setup.py
```

### Comparing `pyrestyle-0.0.4/LICENSE` & `pyrestyle-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestyle-0.0.4/PKG-INFO` & `pyrestyle-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyrestyle
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python style guide checker and This project based on pycodestyle
-Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
+Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py
 Author: Johann C. Rocholl, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: Expat license
 Keywords: pyrestyle,pep8,PEP 8,PEP-8,PEP8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrestyle-0.0.4/pyrestyle.egg-info/PKG-INFO` & `pyrestyle-0.0.5/pyrestyle.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyrestyle
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python style guide checker and This project based on pycodestyle
-Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08
+Home-page: https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py
 Author: Johann C. Rocholl, 2023-1-OPPS1-CGS-08
 Author-email: kys00919@gmail.com
 License: Expat license
 Keywords: pyrestyle,pep8,PEP 8,PEP-8,PEP8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrestyle-0.0.4/pyrestyle.py` & `pyrestyle-0.0.5/pyrestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
```

### Comparing `pyrestyle-0.0.4/setup.py` & `pyrestyle-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         name='pyrestyle',
         version=get_version(),
         description="Python style guide checker and This project based on pycodestyle",
         long_description=readme.read(),
         keywords='pyrestyle, pep8, PEP 8, PEP-8, PEP8',
         author='Johann C. Rocholl, 2023-1-OPPS1-CGS-08',
         author_email='kys00919@gmail.com',
-        url='https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08',
+        url='https://github.com/CSID-DGU/2023-1-OPPS1-CGS-08/blob/main/pyrestyle.py',
         license='Expat license',
         py_modules=['pyrestyle'],
         include_package_data=True,
         zip_safe=False,
         python_requires='>=3.7',
         entry_points={
             'console_scripts': [
```

