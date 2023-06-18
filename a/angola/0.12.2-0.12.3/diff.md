# Comparing `tmp/angola-0.12.2.tar.gz` & `tmp/angola-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.12.2.tar", last modified: Sat Jun 17 18:39:25 2023, max compression
+gzip compressed data, was "angola-0.12.3.tar", last modified: Sun Jun 18 07:13:00 2023, max compression
```

## Comparing `angola-0.12.2.tar` & `angola-0.12.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.698866 angola-0.12.2/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.2/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.2/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-17 18:39:25.698929 angola-0.12.2/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.2/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-17 18:39:25.699155 angola-0.12.2/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-17 18:39:15.000000 angola-0.12.2/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.692696 angola-0.12.2/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.696280 angola-0.12.2/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.2/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-11 22:47:22.000000 angola-0.12.2/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.2/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.2/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.2/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    19447 2023-06-09 03:27:14.000000 angola-0.12.2/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.697226 angola-0.12.2/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-17 18:39:25.000000 angola-0.12.2/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-17 18:39:25.698772 angola-0.12.2/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.2/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.2/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.2/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.2/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.2/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.972939 angola-0.12.3/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.12.3/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.12.3/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:13:00.973035 angola-0.12.3/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      938 2023-06-09 03:27:48.000000 angola-0.12.3/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-06-18 07:13:00.973378 angola-0.12.3/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-06-18 07:12:54.000000 angola-0.12.3/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.965994 angola-0.12.3/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.969958 angola-0.12.3/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      428 2023-06-09 03:27:14.000000 angola-0.12.3/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    50794 2023-06-11 22:47:22.000000 angola-0.12.3/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    12956 2023-06-03 04:28:39.000000 angola-0.12.3/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.12.3/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    17470 2023-06-03 04:30:01.000000 angola-0.12.3/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    19679 2023-06-18 07:12:48.000000 angola-0.12.3/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.971285 angola-0.12.3/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1318 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-06-18 07:13:00.000000 angola-0.12.3/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-06-18 07:13:00.972836 angola-0.12.3/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.12.3/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.12.3/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.12.3/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.12.3/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.12.3/tests/test_query.py
```

### Comparing `angola-0.12.2/LICENSE` & `angola-0.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/PKG-INFO` & `angola-0.12.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.2
+Version: 0.12.3
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.2/README.md` & `angola-0.12.3/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/setup.py` & `angola-0.12.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.12.2"
+VERSION = "0.12.3"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.12.2/src/angola/database.py` & `angola-0.12.3/src/angola/database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/src/angola/dict_mutator.py` & `angola-0.12.3/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/src/angola/dict_query.py` & `angola-0.12.3/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/src/angola/lib.py` & `angola-0.12.3/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/src/angola/lib_xql.py` & `angola-0.12.3/src/angola/lib_xql.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,37 +249,46 @@
     return aql, params
 
 
 def _parse_filter_row(k, value, propkey) -> tuple:
     operator = "$EQ"  # default operator
     # extract the key and the operator
     # ie -> "name:$eq" or "city:$in"
+
+    # "x:$in": "@policy._key"
+
     # link#, especially in join: "'name': '#parent.key'"
 
     if ":" in k:
         k, operator = k.split(":", 2)
         operator = operator.upper()
 
     # literal values starts with `#`
     # it indicates the value should not be converted, but rather return as is without `#`
     # ie:
-    # - {k: "#parent.key"} -> k == parent.key
-    # - {k: '#@params_value'} -> k == @params_value
+    # - {k: "@parent.key"} -> k == parent.key
+    # - {k: '$@params_value'} -> k == @params_value
     #
     dlit = isinstance(value, str) and value.startswith("#")
 
     # gen a unique number to make sure values generated are unique
     num_ = lib.gen_number(6)
     ukey = slugify("%s_%s" % (k, num_), separator="_")
     stmt = ""
     params = {}
     value = eval_macros(value=value)
 
     if dlit:
-        value = value.replace("#", "")
+        if value.startswith("@"):
+            value = value.replace("@", "")
+        elif value.startswith("#@"):
+            value = value.replace("#@", "@")
+        elif value.startswith("#"):
+            value = value.replace("#", "")
+
         if operator in _rev_ops_order:  # reverse order
             stmt = " {value} {operator} {propkey}.{key}"
         else:
             stmt = " {propkey}.{key} {operator} {value}"
     
     # between -> $gte and $lte
     elif operator == "$BETWEEN":
```

### Comparing `angola-0.12.2/src/angola.egg-info/PKG-INFO` & `angola-0.12.3/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.12.2
+Version: 0.12.3
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.12.2/tests/test_database.py` & `angola-0.12.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/tests/test_dict_mutator.py` & `angola-0.12.3/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.12.2/tests/test_lib.py` & `angola-0.12.3/tests/test_lib.py`

 * *Files identical despite different names*

