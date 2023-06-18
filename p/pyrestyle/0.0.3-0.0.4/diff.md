# Comparing `tmp/pyrestyle-0.0.3.tar.gz` & `tmp/pyrestyle-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestyle-0.0.3.tar", last modified: Sun Jun 18 11:38:32 2023, max compression
+gzip compressed data, was "pyrestyle-0.0.4.tar", last modified: Sun Jun 18 12:43:45 2023, max compression
```

## Comparing `pyrestyle-0.0.3.tar` & `pyrestyle-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,14 @@
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 11:38:32.834766 pyrestyle-0.0.3/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1229 2023-06-17 05:07:33.000000 pyrestyle-0.0.3/LICENSE
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      880 2023-06-18 11:38:32.834321 pyrestyle-0.0.3/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 10:12:27.000000 pyrestyle-0.0.3/README.rst
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 11:38:32.816212 pyrestyle-0.0.3/pyrestyle.egg-info/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      880 2023-06-18 11:38:32.000000 pyrestyle-0.0.3/pyrestyle.egg-info/PKG-INFO
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      580 2023-06-18 11:38:32.000000 pyrestyle-0.0.3/pyrestyle.egg-info/SOURCES.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 11:38:32.000000 pyrestyle-0.0.3/pyrestyle.egg-info/dependency_links.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-18 11:38:32.000000 pyrestyle-0.0.3/pyrestyle.egg-info/entry_points.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 09:26:11.000000 pyrestyle-0.0.3/pyrestyle.egg-info/not-zip-safe
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-18 11:38:32.000000 pyrestyle-0.0.3/pyrestyle.egg-info/top_level.txt
--rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-18 11:21:53.000000 pyrestyle-0.0.3/pyrestyle.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 11:38:32.834873 pyrestyle-0.0.3/setup.cfg
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     3533 2023-06-18 11:35:54.000000 pyrestyle-0.0.3/setup.py
-drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 11:38:32.833823 pyrestyle-0.0.3/test/
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1002 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_W701.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      683 2023-06-17 12:18:53.000000 pyrestyle-0.0.3/test/test_W702.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1383 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_W7_comment.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1046 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_aliasing.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      977 2023-06-17 11:33:16.000000 pyrestyle-0.0.3/test/test_all.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     4570 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_ast.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      999 2023-06-17 08:05:17.000000 pyrestyle-0.0.3/test/test_import_user.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      760 2023-06-17 08:15:01.000000 pyrestyle-0.0.3/test/test_import_userlib.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      255 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_overriding_other_file.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      113 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_overriding_other_file_super.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)     1287 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_overriding_same_file.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      584 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_same_class_name.py
--rw-r--r--   0 kim-wiseong   (501) staff       (20)      501 2023-06-17 05:37:52.000000 pyrestyle-0.0.3/test/test_same_function_name.py
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:43:45.274356 pyrestyle-0.0.4/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1324 2023-06-18 12:32:26.000000 pyrestyle-0.0.4/LICENSE
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      914 2023-06-18 12:43:45.273976 pyrestyle-0.0.4/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:39:22.000000 pyrestyle-0.0.4/README.rst
+drwxr-xr-x   0 kim-wiseong   (501) staff       (20)        0 2023-06-18 12:43:45.272784 pyrestyle-0.0.4/pyrestyle.egg-info/
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      914 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/PKG-INFO
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)      240 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/SOURCES.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/dependency_links.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       46 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/entry_points.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)        1 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/not-zip-safe
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       10 2023-06-18 12:43:45.000000 pyrestyle-0.0.4/pyrestyle.egg-info/top_level.txt
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)   107905 2023-06-18 12:37:59.000000 pyrestyle-0.0.4/pyrestyle.py
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)       38 2023-06-18 12:43:45.274458 pyrestyle-0.0.4/setup.cfg
+-rw-r--r--   0 kim-wiseong   (501) staff       (20)     1678 2023-06-18 12:43:41.000000 pyrestyle-0.0.4/setup.py
```

### Comparing `pyrestyle-0.0.3/LICENSE` & `pyrestyle-0.0.4/LICENSE`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 MIT License
 
-Copyright (C) 2010-2011 Hideo Hattori
-Copyright (C) 2011-2013 Hideo Hattori, Steven Myint
-Copyright (C) 2013-2016 Hideo Hattori, Steven Myint, Bill Wendling
-Copyright (C) 2023 컴공쏘년단
+Copyright © 2006-2009 Johann C. Rocholl <johann@rocholl.net>
+Copyright © 2009-2014 Florent Xicluna <florent.xicluna@gmail.com>
+Copyright © 2014-2020 Ian Lee <IanLee1521@gmail.com>
+Copyright (C) 2023 2023-1-OPPS1-CGS-08, 컴공쏘년단 
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Licensed under the terms of the Expat License
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files
+(the "Software"), to deal in the Software without restriction,
+including without limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
+BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
+ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `pyrestyle-0.0.3/pyrestyle.py` & `pyrestyle-0.0.4/pyrestyle.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: no cover (<py310)
     tokenize._compile = lru_cache()(tokenize._compile)  # type: ignore
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 DEFAULT_EXCLUDE = '.svn,CVS,.bzr,.hg,.git,__pycache__,.tox'
 DEFAULT_IGNORE = 'E121,E123,E126,E226,E24,E704,W503,W504'
 try:
     if sys.platform == 'win32':
         USER_CONFIG = os.path.expanduser(r'~\.pycodestyle')
     else:
```

