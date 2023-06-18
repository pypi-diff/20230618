# Comparing `tmp/unihan-etl-0.9.4.tar.gz` & `tmp/unihan-etl-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unihan-etl-0.9.4.tar", last modified: Mon Jun  5 05:03:55 2017, max compression
+gzip compressed data, was "dist/unihan-etl-0.9.5.tar", last modified: Mon Jun 26 17:39:43 2017, max compression
```

## Comparing `unihan-etl-0.9.4.tar` & `unihan-etl-0.9.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/
--rw-r--r--   0 me         (501) staff       (20)      722 2017-05-26 17:22:41.000000 unihan-etl-0.9.4/.tmuxp.yaml
--rw-r--r--   0 me         (501) staff       (20)     4299 2017-06-05 05:03:19.000000 unihan-etl-0.9.4/CHANGES
-drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/doc/
--rw-r--r--   0 me         (501) staff       (20)     1483 2017-05-26 18:39:59.000000 unihan-etl-0.9.4/doc/about.rst
--rw-r--r--   0 me         (501) staff       (20)      508 2017-05-28 02:00:19.000000 unihan-etl-0.9.4/doc/api.rst
--rw-r--r--   0 me         (501) staff       (20)      170 2017-05-26 18:40:25.000000 unihan-etl-0.9.4/doc/cli.rst
--rw-r--r--   0 me         (501) staff       (20)      739 2017-05-30 19:01:13.000000 unihan-etl-0.9.4/doc/FAQ.rst
--rw-r--r--   0 me         (501) staff       (20)       82 2017-05-26 15:00:23.000000 unihan-etl-0.9.4/doc/history.rst
--rw-r--r--   0 me         (501) staff       (20)      162 2017-05-30 18:58:43.000000 unihan-etl-0.9.4/doc/index.rst
--rw-r--r--   0 me         (501) staff       (20)     7670 2017-05-29 14:56:08.000000 unihan-etl-0.9.4/doc/unihan.rst
--rw-r--r--   0 me         (501) staff       (20)     1119 2017-05-26 15:00:23.000000 unihan-etl-0.9.4/LICENSE
--rw-r--r--   0 me         (501) staff       (20)      146 2017-05-26 18:38:54.000000 unihan-etl-0.9.4/MANIFEST.in
--rw-r--r--   0 me         (501) staff       (20)    11253 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)     7967 2017-05-29 11:57:01.000000 unihan-etl-0.9.4/README.rst
-drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/requirements/
--rw-r--r--   0 me         (501) staff       (20)       46 2017-05-27 18:37:44.000000 unihan-etl-0.9.4/requirements/base.txt
--rw-r--r--   0 me         (501) staff       (20)       42 2017-06-02 21:11:17.000000 unihan-etl-0.9.4/requirements/dev.txt
--rw-r--r--   0 me         (501) staff       (20)       71 2017-05-28 18:54:20.000000 unihan-etl-0.9.4/requirements/doc.txt
--rw-r--r--   0 me         (501) staff       (20)       14 2017-05-31 14:32:40.000000 unihan-etl-0.9.4/requirements/test.txt
--rw-r--r--   0 me         (501) staff       (20)       38 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/setup.cfg
--rwxr-xr-x   0 me         (501) staff       (20)     2285 2017-05-26 18:35:54.000000 unihan-etl-0.9.4/setup.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl/
--rw-r--r--   0 me         (501) staff       (20)      289 2017-06-05 05:03:04.000000 unihan-etl-0.9.4/unihan_etl/__about__.py
--rw-r--r--   0 me         (501) staff       (20)        0 2017-05-26 15:00:23.000000 unihan-etl-0.9.4/unihan_etl/__init__.py
--rw-r--r--   0 me         (501) staff       (20)      377 2017-05-26 15:00:23.000000 unihan-etl-0.9.4/unihan_etl/__main__.py
--rw-r--r--   0 me         (501) staff       (20)      696 2017-05-26 15:00:23.000000 unihan-etl-0.9.4/unihan_etl/_compat.py
--rw-r--r--   0 me         (501) staff       (20)     4338 2017-05-30 18:49:08.000000 unihan-etl-0.9.4/unihan_etl/constants.py
--rw-r--r--   0 me         (501) staff       (20)     9538 2017-06-05 05:00:42.000000 unihan-etl-0.9.4/unihan_etl/expansion.py
--rwxr-xr-x   0 me         (501) staff       (20)    16078 2017-05-26 19:22:49.000000 unihan-etl-0.9.4/unihan_etl/process.py
--rw-r--r--   0 me         (501) staff       (20)      650 2017-05-28 02:02:32.000000 unihan-etl-0.9.4/unihan_etl/test.py
--rw-r--r--   0 me         (501) staff       (20)     3215 2017-05-26 15:00:23.000000 unihan-etl-0.9.4/unihan_etl/util.py
-drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/
--rw-r--r--   0 me         (501) staff       (20)        1 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/dependency_links.txt
--rw-r--r--   0 me         (501) staff       (20)       56 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/entry_points.txt
--rw-r--r--   0 me         (501) staff       (20)        1 2017-05-26 18:34:27.000000 unihan-etl-0.9.4/unihan_etl.egg-info/not-zip-safe
--rw-r--r--   0 me         (501) staff       (20)    11253 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/PKG-INFO
--rw-r--r--   0 me         (501) staff       (20)       46 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/requires.txt
--rw-r--r--   0 me         (501) staff       (20)      679 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/SOURCES.txt
--rw-r--r--   0 me         (501) staff       (20)       11 2017-06-05 05:03:55.000000 unihan-etl-0.9.4/unihan_etl.egg-info/top_level.txt
+drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/
+-rw-r--r--   0 me         (501) staff       (20)      722 2017-05-26 17:22:41.000000 unihan-etl-0.9.5/.tmuxp.yaml
+-rw-r--r--   0 me         (501) staff       (20)     4403 2017-06-26 17:38:41.000000 unihan-etl-0.9.5/CHANGES
+drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/doc/
+-rw-r--r--   0 me         (501) staff       (20)     1483 2017-05-26 18:39:59.000000 unihan-etl-0.9.5/doc/about.rst
+-rw-r--r--   0 me         (501) staff       (20)      508 2017-05-28 02:00:19.000000 unihan-etl-0.9.5/doc/api.rst
+-rw-r--r--   0 me         (501) staff       (20)      170 2017-05-26 18:40:25.000000 unihan-etl-0.9.5/doc/cli.rst
+-rw-r--r--   0 me         (501) staff       (20)      739 2017-05-30 19:01:13.000000 unihan-etl-0.9.5/doc/FAQ.rst
+-rw-r--r--   0 me         (501) staff       (20)       82 2017-05-26 15:00:23.000000 unihan-etl-0.9.5/doc/history.rst
+-rw-r--r--   0 me         (501) staff       (20)      162 2017-05-30 18:58:43.000000 unihan-etl-0.9.5/doc/index.rst
+-rw-r--r--   0 me         (501) staff       (20)     7670 2017-05-29 14:56:08.000000 unihan-etl-0.9.5/doc/unihan.rst
+-rw-r--r--   0 me         (501) staff       (20)     1119 2017-05-26 15:00:23.000000 unihan-etl-0.9.5/LICENSE
+-rw-r--r--   0 me         (501) staff       (20)      146 2017-05-26 18:38:54.000000 unihan-etl-0.9.5/MANIFEST.in
+-rw-r--r--   0 me         (501) staff       (20)    11253 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)     7967 2017-05-29 11:57:01.000000 unihan-etl-0.9.5/README.rst
+drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/requirements/
+-rw-r--r--   0 me         (501) staff       (20)       46 2017-05-27 18:37:44.000000 unihan-etl-0.9.5/requirements/base.txt
+-rw-r--r--   0 me         (501) staff       (20)       42 2017-06-10 17:53:31.000000 unihan-etl-0.9.5/requirements/dev.txt
+-rw-r--r--   0 me         (501) staff       (20)       72 2017-06-26 15:09:27.000000 unihan-etl-0.9.5/requirements/doc.txt
+-rw-r--r--   0 me         (501) staff       (20)       14 2017-06-10 17:53:31.000000 unihan-etl-0.9.5/requirements/test.txt
+-rw-r--r--   0 me         (501) staff       (20)       38 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/setup.cfg
+-rwxr-xr-x   0 me         (501) staff       (20)     2285 2017-05-26 18:35:54.000000 unihan-etl-0.9.5/setup.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl/
+-rw-r--r--   0 me         (501) staff       (20)      289 2017-06-26 17:39:12.000000 unihan-etl-0.9.5/unihan_etl/__about__.py
+-rw-r--r--   0 me         (501) staff       (20)        0 2017-05-26 15:00:23.000000 unihan-etl-0.9.5/unihan_etl/__init__.py
+-rw-r--r--   0 me         (501) staff       (20)      377 2017-05-26 15:00:23.000000 unihan-etl-0.9.5/unihan_etl/__main__.py
+-rw-r--r--   0 me         (501) staff       (20)      696 2017-05-26 15:00:23.000000 unihan-etl-0.9.5/unihan_etl/_compat.py
+-rw-r--r--   0 me         (501) staff       (20)     4338 2017-05-30 18:49:08.000000 unihan-etl-0.9.5/unihan_etl/constants.py
+-rw-r--r--   0 me         (501) staff       (20)     9932 2017-06-26 17:35:50.000000 unihan-etl-0.9.5/unihan_etl/expansion.py
+-rwxr-xr-x   0 me         (501) staff       (20)    16078 2017-05-26 19:22:49.000000 unihan-etl-0.9.5/unihan_etl/process.py
+-rw-r--r--   0 me         (501) staff       (20)      650 2017-05-28 02:02:32.000000 unihan-etl-0.9.5/unihan_etl/test.py
+-rw-r--r--   0 me         (501) staff       (20)     3215 2017-05-26 15:00:23.000000 unihan-etl-0.9.5/unihan_etl/util.py
+drwxr-xr-x   0 me         (501) staff       (20)        0 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/
+-rw-r--r--   0 me         (501) staff       (20)        1 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 me         (501) staff       (20)       56 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/entry_points.txt
+-rw-r--r--   0 me         (501) staff       (20)        1 2017-05-26 18:34:27.000000 unihan-etl-0.9.5/unihan_etl.egg-info/not-zip-safe
+-rw-r--r--   0 me         (501) staff       (20)    11253 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/PKG-INFO
+-rw-r--r--   0 me         (501) staff       (20)       46 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/requires.txt
+-rw-r--r--   0 me         (501) staff       (20)      679 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 me         (501) staff       (20)       11 2017-06-26 17:39:43.000000 unihan-etl-0.9.5/unihan_etl.egg-info/top_level.txt
```

### Comparing `unihan-etl-0.9.4/.tmuxp.yaml` & `unihan-etl-0.9.5/.tmuxp.yaml`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/CHANGES` & `unihan-etl-0.9.5/CHANGES`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 =========
 Changelog
 =========
 
 Here you can find the recent changes to the project.
 
+- :release:`0.9.5 <2017-06-26>`
+- :support:`-` Enhance support for locations on *kHDZRadBreak* fields.
+
 - :release:`0.9.4 <2017-06-05>`
 - :bug:`-` Fix kIRG_GSource without location
 - :bug:`-` Fix kFenn output
 - :bug:`-` Fix kHanyuPinlu support output for n diacritics
 
 - :release:`0.9.3 <2017-05-31>`
 - :support:`-` Add expansion for kIRGKangXi
```

### Comparing `unihan-etl-0.9.4/doc/about.rst` & `unihan-etl-0.9.5/doc/about.rst`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/doc/FAQ.rst` & `unihan-etl-0.9.5/doc/FAQ.rst`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/doc/unihan.rst` & `unihan-etl-0.9.5/doc/unihan.rst`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/LICENSE` & `unihan-etl-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/PKG-INFO` & `unihan-etl-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unihan-etl
-Version: 0.9.4
+Version: 0.9.5
 Summary: Export UNIHAN to Python, Data Package, CSV, JSON and YAML
 Home-page: https://unihan-etl.git-pull.com
 Author: Tony Narlock
 Author-email: cihai@git-pull.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/unihan-etl
 Description: *unihan-etl* - `ETL`_ tool `UNIHAN`_. Retrieve, extract, and transform
```

### Comparing `unihan-etl-0.9.4/README.rst` & `unihan-etl-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/setup.py` & `unihan-etl-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/unihan_etl/_compat.py` & `unihan-etl-0.9.5/unihan_etl/_compat.py`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/unihan_etl/constants.py` & `unihan-etl-0.9.5/unihan_etl/constants.py`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/unihan_etl/expansion.py` & `unihan-etl-0.9.5/unihan_etl/expansion.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,24 +264,39 @@
         }
     return value
 
 
 def expand_kHDZRadBreak(value):
     rad, loc = value.split(':')
 
+    location_pattern = re.compile(r"""
+        (?P<volume>[1-8])
+        (?P<page>[0-9]{4})\.
+        (?P<character>[0-3][0-9])
+        (?P<virtual>[01])
+    """, re.X)
+
+    l = location_pattern.match(loc).groupdict()
+    location = {
+        "volume": int(l['volume']),
+        "page": int(l['page']),
+        "character": int(l['character']),
+        "virtual": int(l['virtual'])
+    }
+
     pattern = re.compile(r"""
         (?P<radical>[{}]+)
         \[(?P<ucn>U\+2F[0-9A-D][0-9A-F])\]
     """.format(zhon.hanzi.radicals), re.X)
     m = pattern.match(rad).groupdict()
 
     return {
         "radical": m['radical'],
         "ucn": m['ucn'],
-        "location": loc
+        "location": location
     }
 
 
 def expand_kSBGY(value):
     for i, v in enumerate(value):
         vals = v.split('.')
         value[i] = {
```

### Comparing `unihan-etl-0.9.4/unihan_etl/process.py` & `unihan-etl-0.9.5/unihan_etl/process.py`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/unihan_etl/test.py` & `unihan-etl-0.9.5/unihan_etl/test.py`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/unihan_etl/util.py` & `unihan-etl-0.9.5/unihan_etl/util.py`

 * *Files identical despite different names*

### Comparing `unihan-etl-0.9.4/unihan_etl.egg-info/PKG-INFO` & `unihan-etl-0.9.5/unihan_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: unihan-etl
-Version: 0.9.4
+Version: 0.9.5
 Summary: Export UNIHAN to Python, Data Package, CSV, JSON and YAML
 Home-page: https://unihan-etl.git-pull.com
 Author: Tony Narlock
 Author-email: cihai@git-pull.com
 License: MIT
 Download-URL: https://pypi.python.org/pypi/unihan-etl
 Description: *unihan-etl* - `ETL`_ tool `UNIHAN`_. Retrieve, extract, and transform
```

### Comparing `unihan-etl-0.9.4/unihan_etl.egg-info/SOURCES.txt` & `unihan-etl-0.9.5/unihan_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

