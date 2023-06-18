# Comparing `tmp/pystorz-0.3.4.tar.gz` & `tmp/pystorz-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorz-0.3.4.tar", last modified: Sat Jun 10 16:54:26 2023, max compression
+gzip compressed data, was "dist/pystorz-0.3.5.tar", last modified: Sun Jun 18 01:32:12 2023, max compression
```

## Comparing `pystorz-0.3.4.tar` & `pystorz-0.3.5.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.490068 pystorz-0.3.4/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.4/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-10 16:54:26.489895 pystorz-0.3.4/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.4/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.481989 pystorz-0.3.4/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.4/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.482869 pystorz-0.3.4/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.4/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.483231 pystorz-0.3.4/pystorz/meta/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.3.4/pystorz/meta/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.4/pystorz/meta/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.484578 pystorz-0.3.4/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.4/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.4/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.4/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.486153 pystorz-0.3.4/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.4/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.4/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.4/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.4/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.4/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.4/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.487190 pystorz-0.3.4/pystorz/rest/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.3.4/pystorz/rest/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/rest/client.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.4/pystorz/rest/headers.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/rest/internals.py
--rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.4/pystorz/rest/server.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.487536 pystorz-0.3.4/pystorz/router/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.3.4/pystorz/router/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2344 2023-06-06 17:21:47.000000 pystorz-0.3.4/pystorz/router/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.488422 pystorz-0.3.4/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.4/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2734 2023-06-10 16:53:04.000000 pystorz-0.3.4/pystorz/sql/mysql.py
--rw-r--r--   0 wazofski   (501) staff       (20)      192 2023-06-04 16:07:46.000000 pystorz-0.3.4/pystorz/sql/sqlite.py
--rw-r--r--   0 wazofski   (501) staff       (20)    15493 2023-06-09 19:44:00.000000 pystorz-0.3.4/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.489631 pystorz-0.3.4/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.4/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.4/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.4/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.4/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-10 16:54:26.482648 pystorz-0.3.4/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     1081 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-10 16:54:26.000000 pystorz-0.3.4/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-10 16:54:26.490149 pystorz-0.3.4/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-10 16:53:46.000000 pystorz-0.3.4/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.353195 pystorz-0.3.5/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.5/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     3506 2023-06-18 01:32:12.352971 pystorz-0.3.5/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.5/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.342860 pystorz-0.3.5/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.5/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.344077 pystorz-0.3.5/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.5/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.344532 pystorz-0.3.5/pystorz/meta/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:40.000000 pystorz-0.3.5/pystorz/meta/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2580 2023-06-06 17:22:59.000000 pystorz-0.3.5/pystorz/meta/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.346067 pystorz-0.3.5/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.5/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4164 2023-06-05 18:53:35.000000 pystorz-0.3.5/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.5/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.347985 pystorz-0.3.5/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.5/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.5/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.5/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.5/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.5/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.5/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.349151 pystorz-0.3.5/pystorz/rest/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:44.000000 pystorz-0.3.5/pystorz/rest/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/rest/client.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.5/pystorz/rest/headers.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/rest/internals.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.5/pystorz/rest/server.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.349608 pystorz-0.3.5/pystorz/router/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-06-09 19:44:42.000000 pystorz-0.3.5/pystorz/router/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2336 2023-06-18 00:52:08.000000 pystorz-0.3.5/pystorz/router/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.351100 pystorz-0.3.5/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.5/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2544 2023-06-18 01:30:20.000000 pystorz-0.3.5/pystorz/sql/adapter.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      876 2023-06-18 01:24:36.000000 pystorz-0.3.5/pystorz/sql/mysql.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      470 2023-06-18 01:24:50.000000 pystorz-0.3.5/pystorz/sql/sqlite.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    15152 2023-06-18 01:17:02.000000 pystorz-0.3.5/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.352399 pystorz-0.3.5/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.5/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.5/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.5/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.5/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-18 01:32:12.343752 pystorz-0.3.5/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     3506 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     1104 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)      128 2023-06-18 01:32:12.000000 pystorz-0.3.5/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-18 01:32:12.353261 pystorz-0.3.5/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)     1316 2023-06-18 00:43:38.000000 pystorz-0.3.5/setup.py
```

### Comparing `pystorz-0.3.4/LICENSE` & `pystorz-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/PKG-INFO` & `pystorz-0.3.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pystorz
-Version: 0.3.4
-Summary: Python package for the Storz object store framework.
-Home-page: https://github.com/wazofski/pystorz
-Author: wazofski
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
 <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
 </p>
 
 **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
 
 **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
```

### Comparing `pystorz-0.3.4/README.md` & `pystorz-0.3.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,75 @@
-<p align="center">
-<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
-</p>
-
-**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
-
-**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
-
-Original storz was written in go. You can check it out here:
-[https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
-
-This is a python port of the original storz.
-Still in development.
-
-## Quick Start Guide
-
-### Installation
-```
-pip install pystorz
-```
-
-## Model example
-
-You can find a saomple model in the tests folder.
-[https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
-
-You can define simple structures and reference them as fields in other structures.
-
-You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
-
-Only a SQLite store is implemented at the moment.
-
-More to come.
-Check out the go version (link above) for more information.
-
-## Usage
-```
-    from pystorz.mgen import builder
-
-    # run the code gen to 
-    builder.Generate("path/to/model.yml")
-    # this will make a generated folder in the project home directory
-
-    # you can then import the generated model
-    from generated import model
-
-    # initialize a store
-    stor = SqliteStore(
-        Schema(),
-        SqliteConnector("path/to/your/sqlite3.db"))
-
-    world = model.WorldFactory()
-    world.External().SetName("hello")
-
-    created_world = stor.Create(world)
-    world.External().SetDescription("hello world")
-    updated_world = stor.Update(world.Metadata().Identity(), world)
-    
-    # ...
-
-```
+Metadata-Version: 2.1
+Name: pystorz
+Version: 0.3.5
+Summary: Python package for the Storz object store framework.
+Home-page: https://github.com/wazofski/pystorz
+Author: wazofski
+License: UNKNOWN
+Description: <p align="center">
+        <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
+        </p>
+        
+        **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+        
+        **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
+        
+        Original storz was written in go. You can check it out here:
+        [https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
+        
+        This is a python port of the original storz.
+        Still in development.
+        
+        ## Quick Start Guide
+        
+        ### Installation
+        ```
+        pip install pystorz
+        ```
+        
+        ## Model example
+        
+        You can find a saomple model in the tests folder.
+        [https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
+        
+        You can define simple structures and reference them as fields in other structures.
+        
+        You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
+        
+        Only a SQLite store is implemented at the moment.
+        
+        More to come.
+        Check out the go version (link above) for more information.
+        
+        ## Usage
+        ```
+            from pystorz.mgen import builder
+        
+            # run the code gen to 
+            builder.Generate("path/to/model.yml")
+            # this will make a generated folder in the project home directory
+        
+            # you can then import the generated model
+            from generated import model
+        
+            # initialize a store
+            stor = SqliteStore(
+                Schema(),
+                SqliteConnector("path/to/your/sqlite3.db"))
+        
+            world = model.WorldFactory()
+            world.External().SetName("hello")
+        
+            created_world = stor.Create(world)
+            world.External().SetDescription("hello world")
+            updated_world = stor.Update(world.Metadata().Identity(), world)
+            
+            # ...
+        
+        ```
+        
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `pystorz-0.3.4/pystorz/meta/store.py` & `pystorz-0.3.5/pystorz/meta/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/mgen/builder.py` & `pystorz-0.3.5/pystorz/mgen/builder.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/mgen/loader.py` & `pystorz-0.3.5/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/mgen/templates/structure.py` & `pystorz-0.3.5/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.3.5/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/mgen/test.py` & `pystorz-0.3.5/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/mgen/utils.py` & `pystorz-0.3.5/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/rest/client.py` & `pystorz-0.3.5/pystorz/rest/client.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/rest/headers.py` & `pystorz-0.3.5/pystorz/rest/headers.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/rest/internals.py` & `pystorz-0.3.5/pystorz/rest/internals.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/rest/server.py` & `pystorz-0.3.5/pystorz/rest/server.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/router/store.py` & `pystorz-0.3.5/pystorz/router/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pystorz.store import options
 from pystorz.internal import constants
 
 log = logging.getLogger(__name__)
 
 
 class RouteStore(store.Store):
-    def __init__(self, default: store.Store, mapping: dict):
+    def __init__(self, mapping: dict, default=None):
         self.Default = default
         self.Mapping = {}
 
         for k, v in mapping.items():
             self.Mapping[k.lower().replace("/", "")] = v
 
     def Create(self, obj: store.Object, *opt: options.CreateOption) -> store.Object:
```

### Comparing `pystorz-0.3.4/pystorz/sql/mysql.py` & `pystorz-0.3.5/pystorz/sql/adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,102 @@
 import logging
-import mysql.connector
-from pystorz.sql.store import SqlStore
-
 log = logging.getLogger(__name__)
 
-class _MySQLAdapter:
-    def __init__(self, host, port, username, password, database):
-        self.host = host
-        self.port = port
-        self.username = username
-        self.password = password
-        self.database = database
-        self.connection = None
+
+class SQLAdapter:
+    def __init__(self):
+        self._connection = None
         self._cursor = None
 
     def connect(self):
-        try:
+        raise NotImplementedError()
+
+    def connection(self):
+        if not self._connection:
+            self._connection = self.connect()
             self._cursor = None
-            self.connection = mysql.connector.connect(
-                host=self.host,
-                port=self.port,
-                user=self.username,
-                password=self.password,
-                database=self.database
-            )
-            return self.connection
-        except Exception as err:
-            log.error("connect", err)
-            raise err
-
-    def cursor(self):
-        try:
-            if self.connection is None:
-                self.connect()
-            
-            if self._cursor is None:
-                self._cursor = self.connection.cursor()
+        
+        return self._connection
+
+    def cursor(self, retry=True):
+        try:
+            if not self._cursor:
+                connection = self.connection()
+                self._cursor = connection.cursor()
 
             return self._cursor
         except Exception as err:
-            log.error("cursor", err)
-            if self.connection is None:
+            if not retry:
                 raise err
-            self.connection = None
-        
-        return self.cursor()
+
+        self._connection = None
+        self._cursor = None
+        return self.cursor(False)
 
     def close(self):
         try:
             if self._cursor:
                 self._cursor.close()
-            if self.connection:
-                self.connection.close()
+
+            if self._connection:
+                self._connection.close()
         except Exception as err:
             log.error("close", err)
-            raise err
+
+        self._connection = None
         self._cursor = None
 
-    def execute(self, query, params=None):
+    def execute(self, query, params=None, retry=True):
         try:
-            if self._cursor is None:
-                self.cursor()
-            
+            cursor = self.cursor()
             if params:
-                self._cursor.execute(query, params)
+                return cursor.execute(query, params)
             else:
-                self._cursor.execute(query)
+                return cursor.execute(query)
         except Exception as err:
-            log.error("execute", err)
-            raise err
+            if not retry:
+                raise err
+
+        self._connection = None
+        return self.execute(query, params, False)
 
-    def fetchall(self):
+    def fetchall(self, retry=True):
         try:
-            return self._cursor.fetchall()
+            return self.cursor().fetchall()
         except Exception as err:
-            log.error("fetch all", err)
-            raise err
+            if not retry:
+                raise err
 
-    def commit(self):
+        self._connection = None
+        return self.fetchall(False)
+    
+
+    def fetchone(self, retry=True):
         try:
-            self.connection.commit()
+            return self.cursor().fetchone()
         except Exception as err:
-            log.error("commit", err)
-            raise err
-        self._cursor = None
+            if not retry:
+                raise err
 
-    def rollback(self):
+        self._connection = None
+        return self.fetchone(False)
+
+    def commit(self, retry=True):
         try:
-            self.connection.rollback()
+            return self.connection().commit()
         except Exception as err:
-            log.error("rollback", err)
-            raise err
-        self._cursor = None
+            log.info(f"exception: {retry}")
+            if not retry:
+                raise err
 
+        self._connection = None
+        return self.commit(False)
 
-def MySqlStoreFactory(schema, host, port, user, password, database):
-    def connector():
-        return _MySQLAdapter(host, port, user, password, database)
+    def rollback(self, retry=True):
+        try:
+            return self.connection().rollback()
+        except Exception as err:
+            if not retry:
+                raise err
 
-    return SqlStore(schema, connector)
+        self._connection = None
+        return self.rollback(False)
```

### Comparing `pystorz-0.3.4/pystorz/sql/store.py` & `pystorz-0.3.5/pystorz/sql/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,24 +46,23 @@
             raise Exception(constants.ErrObjectExists)
 
         db = self._connection()
 
         try:
             # Start a transaction
             db.execute("BEGIN")
-            cursor = db.cursor()
 
             self._setIdentity(
-                cursor,
+                db,
                 obj.Metadata().Identity().Path(),
                 obj.PrimaryKey(),
                 obj.Metadata().Kind(),
             )
 
-            self._setObject(cursor, obj.PrimaryKey(), obj.Metadata().Kind(), obj)
+            self._setObject(db, obj.PrimaryKey(), obj.Metadata().Kind(), obj)
 
             # Commit the transaction
             db.commit()
             return obj.Clone()
         except Exception as e:
             db.rollback()
             raise e
@@ -111,32 +110,31 @@
                 raise Exception(constants.ErrObjectExists)
 
         db = self._connection()
 
         try:
             # Start a transaction
             db.execute("BEGIN")
-            cursor = db.cursor()
-
-            self._removeIdentity(cursor, existing.Metadata().Identity().Path())
+            
+            self._removeIdentity(db, existing.Metadata().Identity().Path())
 
             obj.Metadata().SetIdentity(existing.Metadata().Identity())
 
             self._setIdentity(
-                cursor,
+                db,
                 obj.Metadata().Identity().Path(),
                 obj.PrimaryKey(),
                 obj.Metadata().Kind(),
             )
 
             self._removeObject(
-                cursor, existing.PrimaryKey(), existing.Metadata().Kind()
+                db, existing.PrimaryKey(), existing.Metadata().Kind()
             )
 
-            self._setObject(cursor, obj.PrimaryKey(), obj.Metadata().Kind(), obj)
+            self._setObject(db, obj.PrimaryKey(), obj.Metadata().Kind(), obj)
 
             db.commit()
             return obj.Clone()
         except Exception as e:
             db.rollback()
             raise e
 
@@ -154,27 +152,26 @@
             existing = self.Get(identity)
 
         db = self._connection()
 
         # try:
         # Start a transaction
         db.execute("BEGIN")
-        cursor = db.cursor()
-
+        
         if copt.filter is None:
-            self._removeIdentity(cursor, existing.Metadata().Identity().Path())
+            self._removeIdentity(db, existing.Metadata().Identity().Path())
             self._removeObject(
-                cursor, existing.PrimaryKey(), existing.Metadata().Kind()
+                db, existing.PrimaryKey(), existing.Metadata().Kind()
             )
         else:
             clause = self._buildFilterClause(copt, identity)
-            keys = self._getObjectKeys(cursor, identity.Type(), clause)
+            keys = self._getObjectKeys(db, identity.Type(), clause)
 
-            self._removeObjects(cursor, identity.Type(), clause)
-            self._removeIdentities(cursor, identity.Type(), keys)
+            self._removeObjects(db, identity.Type(), clause)
+            self._removeIdentities(db, identity.Type(), keys)
 
         db.commit()
         # except Exception as e:
         #     db.rollback()
         #     raise e
 
     def Get(self, identity, *opt):
@@ -184,22 +181,21 @@
         log.info("get {}".format(identity.Path()))
 
         copt = options.CommonOptionHolderFactory()
         for o in opt:
             o.ApplyFunction()(copt)
 
         db = self._connection()
-        cursor = db.cursor()
 
         res = None
         if identity.IsId():
-            pkey, typ = self._getIdentity(cursor, identity.Path())
-            res = self._getObject(cursor, pkey, typ)
+            pkey, typ = self._getIdentity(db, identity.Path())
+            res = self._getObject(db, pkey, typ)
         else:
-            res = self._getObject(cursor, identity.Key(), identity.Type())
+            res = self._getObject(db, identity.Key(), identity.Type())
         
         db.commit()
         return res
 
     def List(self, identity, *opt: list[options.ListOption]):
         if identity is None:
             raise Exception(constants.ErrInvalidPath)
@@ -211,16 +207,15 @@
 
         copt = options.CommonOptionHolderFactory()
 
         for o in opt:
             o.ApplyFunction()(copt)
 
         db = self._connection()
-        cursor = db.cursor()
-
+        
         query = """SELECT Object FROM Objects 
         WHERE Type = '{}'""".format(
             identity.Type()
         )
 
         query += self._buildFilterClause(copt, identity)
 
@@ -236,65 +231,63 @@
 
         if copt.page_size is not None and copt.page_size > 0:
             query = query + " LIMIT {}".format(copt.page_size)
 
         if copt.page_offset is not None and copt.page_offset > 0:
             query = query + " OFFSET {}".format(copt.page_offset)
 
-        self._do_query(cursor, query)
-        rows = cursor.fetchall()
+        self._do_query(db, query)
+        rows = db.fetchall()
 
         res = self._parseObjectRows(rows, identity.Type())
         db.commit()
         return res
 
     def _prepareTables(self, db):
         create = """
         CREATE TABLE IF NOT EXISTS IdIndex (
             Path VARCHAR(75) NOT NULL PRIMARY KEY,
             Pkey NVARCHAR(50) NOT NULL,
             Type VARCHAR(25) NOT NULL);
         """
 
-        cursor = db.cursor()
-        self._do_query(cursor, create)
+        self._do_query(db, create)
 
         create = """
         CREATE TABLE IF NOT EXISTS Objects (
             Pkey NVARCHAR(50) NOT NULL,
             Type VARCHAR(25) NOT NULL,
             Object JSON,
             PRIMARY KEY (Pkey,Type));
         """
 
-        cursor.execute(create)
-        cursor.close()
-
+        db.execute(create)
+        
         db.commit()
 
-    def _getIdentity(self, cursor, path):
+    def _getIdentity(self, db, path):
         query = """SELECT Pkey, Type FROM IdIndex 
         WHERE Path='{}'""".format(
             path
         )
 
-        self._do_query(cursor, query)
-        result = cursor.fetchone()
+        self._do_query(db, query)
+        result = db.fetchone()
 
         if result is not None:
             pkey, typ = result
             return pkey, typ
         else:
             raise Exception(constants.ErrNoSuchObject)
 
-    def _setIdentity(self, cursor, path, pkey, typ):
+    def _setIdentity(self, db, path, pkey, typ):
         # existing_pkey, existing_typ = None, None
 
         # try:
-        #     existing_pkey, existing_typ = self._getIdentity(cursor, path)
+        #     existing_pkey, existing_typ = self._getIdentity(db, path)
         # except Exception as e:
         #     log.debug("identity get failed: {}".format(e))
 
         # query = ""
         # if existing_pkey is not None and existing_typ is not None:
         #     query = """UPDATE IdIndex SET Pkey='{}', Type='{}'
         #     WHERE Path='{}'""".format(
@@ -302,46 +295,46 @@
         #     )
         # else:
         query = """INSERT INTO IdIndex (Pkey, Type, Path)
         VALUES ('{}', '{}', '{}')""".format(
             pkey, typ.lower(), path
         )
 
-        self._do_query(cursor, query)
+        self._do_query(db, query)
 
-    def _removeIdentity(self, cursor, path):
+    def _removeIdentity(self, db, path):
         query = """DELETE FROM IdIndex
         WHERE Path = '{}'""".format(
             path
         )
 
-        self._do_query(cursor, query)
+        self._do_query(db, query)
 
-    def _getObject(self, cursor, pkey, typ):
+    def _getObject(self, db, pkey, typ):
         query = """SELECT Object FROM Objects
         WHERE Pkey='{}' AND Type='{}'""".format(
             pkey, typ.lower()
         )
 
-        self._do_query(cursor, query)
-        result = cursor.fetchone()
+        self._do_query(db, query)
+        result = db.fetchone()
 
         if result is not None:
             data = result[0]
             data = utils.decode_string(data)
             return self._parseObjectRow(data, typ)
         else:
             raise Exception(constants.ErrNoSuchObject)
 
-    def _setObject(self, cursor, pkey, typ, obj):
+    def _setObject(self, db, pkey, typ, obj):
         query = ""
         # existing_obj = None
 
         # try:
-        #     existing_obj = self._getObject(cursor, pkey, typ)
+        #     existing_obj = self._getObject(db, pkey, typ)
         # except Exception as e:
         #     log.debug("object get failed: {}".format(e))
 
         data = obj.ToJson()
         # encode the data so it doesn't contain any SQL unfriendly characters
         data = utils.encode_string(data)
 
@@ -352,79 +345,79 @@
         #     )
         # else:
         query = """INSERT INTO Objects (Object, Pkey, Type)
         VALUES ('{}', '{}', '{}')""".format(
             data, pkey, typ.lower()
         )
 
-        self._do_query(cursor, query)
+        self._do_query(db, query)
 
-    def _removeObject(self, cursor, pkey, typ):
+    def _removeObject(self, db, pkey, typ):
         query = """DELETE FROM Objects
         WHERE Pkey = '{}' AND Type = '{}'""".format(
             pkey, typ.lower()
         )
 
-        self._do_query(cursor, query)
+        self._do_query(db, query)
 
-    def _getObjectKeys(self, cursor, typ, clause):
+    def _getObjectKeys(self, db, typ, clause):
         query = """SELECT Pkey FROM Objects
         WHERE Type = '{}' {}""".format(
             typ.lower(),
             clause,
         )
 
-        self._do_query(cursor, query)
-        rows = cursor.fetchall()
+        self._do_query(db, query)
+        rows = db.fetchall()
         res = []
         for row in rows:
             res.append(row[0])
         return res
 
-    def _removeIdentities(self, cursor, typ, keys):
+    def _removeIdentities(self, db, typ, keys):
         batch_size = 100
         for i in range(0, len(keys), batch_size):
             batch = keys[i : i + batch_size]
             clause = "Pkey IN ({})".format(",".join(["'{}'".format(k) for k in batch]))
 
             query = """DELETE FROM IdIndex
                 WHERE Type = '{}' AND {}""".format(
                 typ.lower(),
                 clause,
             )
 
-            self._do_query(cursor, query)
+            self._do_query(db, query)
 
-    def _removeObjects(self, cursor, typ, clause):
+    def _removeObjects(self, db, typ, clause):
         query = """DELETE FROM Objects
         WHERE Type = '{}' {}""".format(
             typ.lower(),
             clause,
         )
 
-        self._do_query(cursor, query)
+        self._do_query(db, query)
 
     def _parseObjectRow(self, data, typ):
         return utils.unmarshal_object(data, self._schema, typ)
 
     def _parseObjectRows(self, rows, typ):
         res = []
         for row in rows:
             data = utils.decode_string(row[0])
             res.append(self._parseObjectRow(data, typ))
         return res
 
-    def _do_query(self, cursor, query):
+    def _do_query(self, db, query):
         log.debug("running query: {}".format(query))
 
         statements = sqlparse.parse(query)
         if len(statements) > 1:
             raise Exception(constants.ErrInvalidRequest)
 
-        cursor.execute(query)
+        db.execute(query)
 
     def _buildFilterClause(self, copt, identity):
         if copt.filter is None:
             return ""
 
         sample = self._schema.ObjectForKind(identity.Type())
         # if sample is None:
```

### Comparing `pystorz-0.3.4/pystorz/store/meta.py` & `pystorz-0.3.5/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/store/options.py` & `pystorz-0.3.5/pystorz/store/options.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/store/store.py` & `pystorz-0.3.5/pystorz/store/store.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz/store/utils.py` & `pystorz-0.3.5/pystorz/store/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.3.4/pystorz.egg-info/PKG-INFO` & `pystorz-0.3.5/pystorz.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
+License: UNKNOWN
+Description: <p align="center">
+        <img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
+        </p>
+        
+        **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
+        
+        **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
+        
+        Original storz was written in go. You can check it out here:
+        [https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
+        
+        This is a python port of the original storz.
+        Still in development.
+        
+        ## Quick Start Guide
+        
+        ### Installation
+        ```
+        pip install pystorz
+        ```
+        
+        ## Model example
+        
+        You can find a saomple model in the tests folder.
+        [https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
+        
+        You can define simple structures and reference them as fields in other structures.
+        
+        You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
+        
+        Only a SQLite store is implemented at the moment.
+        
+        More to come.
+        Check out the go version (link above) for more information.
+        
+        ## Usage
+        ```
+            from pystorz.mgen import builder
+        
+            # run the code gen to 
+            builder.Generate("path/to/model.yml")
+            # this will make a generated folder in the project home directory
+        
+            # you can then import the generated model
+            from generated import model
+        
+            # initialize a store
+            stor = SqliteStore(
+                Schema(),
+                SqliteConnector("path/to/your/sqlite3.db"))
+        
+            world = model.WorldFactory()
+            world.External().SetName("hello")
+        
+            created_world = stor.Create(world)
+            world.External().SetDescription("hello world")
+            updated_world = stor.Update(world.Metadata().Identity(), world)
+            
+            # ...
+        
+        ```
+        
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-License-File: LICENSE
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
-</p>
-
-**pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
-
-**pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
-
-Original storz was written in go. You can check it out here:
-[https://github.com/wazofski/gostorz](https://github.com/wazofski/gostorz)
-
-This is a python port of the original storz.
-Still in development.
-
-## Quick Start Guide
-
-### Installation
-```
-pip install pystorz
-```
-
-## Model example
-
-You can find a saomple model in the tests folder.
-[https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml](https://github.com/wazofski/pystorz/blob/master/tests/model/sample.yml)
-
-You can define simple structures and reference them as fields in other structures.
-
-You need to define Objects that will become your root level modeled objects. You can then create, update, delete and retrieve these from using a store.
-
-Only a SQLite store is implemented at the moment.
-
-More to come.
-Check out the go version (link above) for more information.
-
-## Usage
-```
-    from pystorz.mgen import builder
-
-    # run the code gen to 
-    builder.Generate("path/to/model.yml")
-    # this will make a generated folder in the project home directory
-
-    # you can then import the generated model
-    from generated import model
-
-    # initialize a store
-    stor = SqliteStore(
-        Schema(),
-        SqliteConnector("path/to/your/sqlite3.db"))
-
-    world = model.WorldFactory()
-    world.External().SetName("hello")
-
-    created_world = stor.Create(world)
-    world.External().SetDescription("hello world")
-    updated_world = stor.Update(world.Metadata().Identity(), world)
-    
-    # ...
-
-```
```

### Comparing `pystorz-0.3.4/pystorz.egg-info/SOURCES.txt` & `pystorz-0.3.5/pystorz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 pystorz/rest/client.py
 pystorz/rest/headers.py
 pystorz/rest/internals.py
 pystorz/rest/server.py
 pystorz/router/__init__.py
 pystorz/router/store.py
 pystorz/sql/__init__.py
+pystorz/sql/adapter.py
 pystorz/sql/mysql.py
 pystorz/sql/sqlite.py
 pystorz/sql/store.py
 pystorz/store/__init__.py
 pystorz/store/meta.py
 pystorz/store/options.py
 pystorz/store/store.py
```

### Comparing `pystorz-0.3.4/setup.py` & `pystorz-0.3.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pystorz',
-    version='0.3.4',
+    version='0.3.5',
     author='wazofski',
     description='Python package for the Storz object store framework.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/wazofski/pystorz',
     packages=[
         "pystorz",
```

