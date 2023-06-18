# Comparing `tmp/angola-0.12.3.tar.gz` & `tmp/angola-0.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.12.3.tar", last modified: Sun Jun 18 07:13:00 2023, max compression
+gzip compressed data, was "angola-0.12.5.tar", last modified: Sun Jun 18 07:27:57 2023, max compression
```

## Comparing `angola-0.12.3.tar` & `angola-0.12.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.972939 angola-0.12.3/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.3/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.3/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:13:00.973035 angola-0.12.3/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.3/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-18 07:13:00.973378 angola-0.12.3/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-18 07:12:54.000000 angola-0.12.3/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.965994 angola-0.12.3/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.969958 angola-0.12.3/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.3/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-11 22:47:22.000000 angola-0.12.3/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.3/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.3/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.3/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    19679 2023-06-18 07:12:48.000000 angola-0.12.3/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.971285 angola-0.12.3/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.972836 angola-0.12.3/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.3/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.3/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.3/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.3/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.3/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.959443 angola-0.12.5/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.5/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.5/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:27:57.959529 angola-0.12.5/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.5/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-18 07:27:57.959814 angola-0.12.5/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-18 07:27:51.000000 angola-0.12.5/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.951307 angola-0.12.5/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.955516 angola-0.12.5/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.5/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-11 22:47:22.000000 angola-0.12.5/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.5/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.5/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.5/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    20046 2023-06-18 07:26:19.000000 angola-0.12.5/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.957184 angola-0.12.5/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-18 07:27:57.000000 angola-0.12.5/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:27:57.959319 angola-0.12.5/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.5/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.5/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.5/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.5/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.5/tests/test_query.py
```

### Comparing `angola-0.12.3/LICENSE` & `angola-0.12.5/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/PKG-INFO` & `angola-0.12.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.3
+Version: 0.12.5
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.3/README.md` & `angola-0.12.5/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/setup.py` & `angola-0.12.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.12.3"
+VERSION = "0.12.5"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.12.3/src/angola/database.py` & `angola-0.12.5/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/src/angola/dict_mutator.py` & `angola-0.12.5/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/src/angola/dict_query.py` & `angola-0.12.5/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/src/angola/lib.py` & `angola-0.12.5/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/src/angola/lib_xql.py` & `angola-0.12.5/src/angola/lib_xql.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class XQLDEFINITION:
     """
     XQL Schema Definition:
 
         :param FROM: str = the collection name
         :param ALIAS: str = alias
+        :param AS: str = alias
         :param FILTERS: dict = filters
         :param SORT: list/str = sort 
         :param OFFSET: int = the offset of the limit, default=0
         :param LIMIT: int = the limit of result, default=10
         :param PAGE: int = help calculate the skip by using a page number. 
         :param JOIN: list[XQL]
         :param RETURN_COUNT: bool =  Will return a count of all matched documents
@@ -29,14 +30,15 @@
             Can be done manually with RETURN MERGE(doc, {data})
         :param RETURN_PARTIAL_QUERY: bool 
             To return the query without final the return. By this can help with SELECT to INSERT
 
     """
     FROM: str = None
     ALIAS: str = None
+    AS: str = None
     FILTERS: dict = {}
     SORT: list = []
     OFFSET: int = 0
     LIMIT: int = 10
     PAGE: int = 1
     JOIN: list = []
     RETURN_COUNT: str = None
@@ -375,29 +377,43 @@
         return ""
     # TODO
     return ""
 
 
 def prepare_xql(xql: dict) -> dict:
     _defaults = {
+
+        "FETCH": None, # alias to FROM
+        "AS": None, # alias to ALIAS
+        "SUBQUERIES": None, # alias to JOIN
+
         "FROM": None,
         "ALIAS": "doc",
         "FILTERS": {},
         "SORT": None,
         "OFFSET": None,
         "RETURN_COUNT": False,
         "LIMIT": 10,
         "PAGE": 1,
         "JOIN": [],
         "RETURN": None,
         "RETURN_WITH": None,
         "RETURN_PARTIAL_QUERY": False,
         **xql
     }
+    
+
     r = {k.upper(): v for k, v in _defaults.items()}
+    if r.get("FETCH"):
+        r["FROM"] = r.get("FETCH")
+    if r.get("AS") :
+        r["ALIAS"] = r.get("AS")
+    if r.get("SUBQUERIES"):
+        r["JOIN"] = r.get("SUBQUERIES")
+        
     if r["RETURN"] is None:
         r["RETURN"] = r["ALIAS"]
     return r
 
 
 def xql_take_skip_page(xql: dict, max_limit=100) -> tuple:
     """
```

### Comparing `angola-0.12.3/src/angola.egg-info/PKG-INFO` & `angola-0.12.5/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.3
+Version: 0.12.5
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.3/tests/test_database.py` & `angola-0.12.5/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/tests/test_dict_mutator.py` & `angola-0.12.5/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.3/tests/test_lib.py` & `angola-0.12.5/tests/test_lib.py`

 * *Files identical despite different names*

