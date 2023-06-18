# Comparing `tmp/dataflows-airtable-0.1.0.tar.gz` & `tmp/dataflows-airtable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataflows-airtable-0.1.0.tar", last modified: Wed Mar 15 13:13:03 2023, max compression
+gzip compressed data, was "dataflows-airtable-0.1.1.tar", last modified: Sun Jun 18 14:34:59 2023, max compression
```

## Comparing `dataflows-airtable-0.1.0.tar` & `dataflows-airtable-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-03-15 13:13:03.490424 dataflows-airtable-0.1.0/
--rw-r--r--   0 adam       (501) staff       (20)      154 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.0/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)      473 2021-05-14 13:36:59.000000 dataflows-airtable-0.1.0/Makefile
--rw-r--r--   0 adam       (501) staff       (20)      948 2023-03-15 13:13:03.490564 dataflows-airtable-0.1.0/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)       77 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.0/README.md
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-03-15 13:13:03.487971 dataflows-airtable-0.1.0/dataflows_airtable/
--rw-r--r--   0 adam       (501) staff       (20)        5 2023-03-15 11:12:13.000000 dataflows-airtable-0.1.0/dataflows_airtable/VERSION
--rw-r--r--   0 adam       (501) staff       (20)      136 2021-05-14 17:39:08.000000 dataflows-airtable-0.1.0/dataflows_airtable/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)       36 2021-05-14 17:40:48.000000 dataflows-airtable-0.1.0/dataflows_airtable/consts.py
--rw-r--r--   0 adam       (501) staff       (20)     3049 2023-03-15 11:12:35.000000 dataflows-airtable-0.1.0/dataflows_airtable/dump_to_airtable.py
--rw-r--r--   0 adam       (501) staff       (20)     3705 2023-03-15 13:10:53.000000 dataflows-airtable-0.1.0/dataflows_airtable/load_from_airtable.py
--rw-r--r--   0 adam       (501) staff       (20)      752 2022-11-20 17:11:38.000000 dataflows-airtable-0.1.0/dataflows_airtable/utilities.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-03-15 13:13:03.490172 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/
--rw-r--r--   0 adam       (501) staff       (20)      948 2023-03-15 13:13:03.000000 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)      528 2023-03-15 13:13:03.000000 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2023-03-15 13:13:03.000000 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 adam       (501) staff       (20)        1 2021-05-14 15:56:11.000000 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/not-zip-safe
--rw-r--r--   0 adam       (501) staff       (20)       72 2023-03-15 13:13:03.000000 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/requires.txt
--rw-r--r--   0 adam       (501) staff       (20)       19 2023-03-15 13:13:03.000000 dataflows-airtable-0.1.0/dataflows_airtable.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)      221 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.0/pylama.ini
--rw-r--r--   0 adam       (501) staff       (20)       27 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.0/pytest.ini
--rw-r--r--   0 adam       (501) staff       (20)       67 2023-03-15 13:13:03.490992 dataflows-airtable-0.1.0/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1946 2021-05-14 10:46:25.000000 dataflows-airtable-0.1.0/setup.py
--rw-r--r--   0 adam       (501) staff       (20)      318 2021-05-14 10:46:39.000000 dataflows-airtable-0.1.0/tox.ini
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-18 14:34:59.635222 dataflows-airtable-0.1.1/
+-rw-r--r--   0 adam       (501) staff       (20)      154 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.1/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)      473 2021-05-14 13:36:59.000000 dataflows-airtable-0.1.1/Makefile
+-rw-r--r--   0 adam       (501) staff       (20)      948 2023-06-18 14:34:59.635401 dataflows-airtable-0.1.1/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)       77 2021-05-14 10:24:07.000000 dataflows-airtable-0.1.1/README.md
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-18 14:34:59.631721 dataflows-airtable-0.1.1/dataflows_airtable/
+-rw-r--r--   0 adam       (501) staff       (20)        5 2023-06-18 14:17:13.000000 dataflows-airtable-0.1.1/dataflows_airtable/VERSION
+-rw-r--r--   0 adam       (501) staff       (20)      136 2021-05-14 17:39:08.000000 dataflows-airtable-0.1.1/dataflows_airtable/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)       36 2021-05-14 17:40:48.000000 dataflows-airtable-0.1.1/dataflows_airtable/consts.py
+-rw-r--r--   0 adam       (501) staff       (20)     3049 2023-03-15 11:12:35.000000 dataflows-airtable-0.1.1/dataflows_airtable/dump_to_airtable.py
+-rw-r--r--   0 adam       (501) staff       (20)     3705 2023-06-18 14:17:08.000000 dataflows-airtable-0.1.1/dataflows_airtable/load_from_airtable.py
+-rw-r--r--   0 adam       (501) staff       (20)      752 2023-06-14 12:00:00.000000 dataflows-airtable-0.1.1/dataflows_airtable/utilities.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-18 14:34:59.634908 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)      948 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)      528 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2021-05-14 15:56:11.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/not-zip-safe
+-rw-r--r--   0 adam       (501) staff       (20)       72 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       19 2023-06-18 14:34:59.000000 dataflows-airtable-0.1.1/dataflows_airtable.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)      221 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.1/pylama.ini
+-rw-r--r--   0 adam       (501) staff       (20)       27 2021-05-14 10:24:56.000000 dataflows-airtable-0.1.1/pytest.ini
+-rw-r--r--   0 adam       (501) staff       (20)       67 2023-06-18 14:34:59.635968 dataflows-airtable-0.1.1/setup.cfg
+-rw-r--r--   0 adam       (501) staff       (20)     1946 2021-05-14 10:46:25.000000 dataflows-airtable-0.1.1/setup.py
+-rw-r--r--   0 adam       (501) staff       (20)      318 2021-05-14 10:46:39.000000 dataflows-airtable-0.1.1/tox.ini
```

### Comparing `dataflows-airtable-0.1.0/PKG-INFO` & `dataflows-airtable-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows-airtable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for adding AirTable support to dataflows
 Home-page: https://github.com/dataspot/dataflows-airtable
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # dataflows-airtable
         Python library for adding AirTable support to dataflows
```

### Comparing `dataflows-airtable-0.1.0/dataflows_airtable/dump_to_airtable.py` & `dataflows-airtable-0.1.1/dataflows_airtable/dump_to_airtable.py`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.0/dataflows_airtable/load_from_airtable.py` & `dataflows-airtable-0.1.1/dataflows_airtable/load_from_airtable.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             while True:
                 try:
                     resp = rate_limiter.execute(lambda: session.get(url, params=params, timeout=10).json())
                     break
                 except Exception as e:
                     retries -= 1
                     if retries == 0:
-                        throw(e)
+                        raise(e)
                     time.sleep(5)
                     continue
             yield from map(
                 lambda r: dict(**{AIRTABLE_ID_FIELD: r['id']}, **r['fields']),
                 resp.get('records', [])
             )
             count += len(resp.get('records', []))
```

### Comparing `dataflows-airtable-0.1.0/dataflows_airtable/utilities.py` & `dataflows-airtable-0.1.1/dataflows_airtable/utilities.py`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.0/dataflows_airtable.egg-info/PKG-INFO` & `dataflows-airtable-0.1.1/dataflows_airtable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataflows-airtable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for adding AirTable support to dataflows
 Home-page: https://github.com/dataspot/dataflows-airtable
 Author: Adam Kariv
 Author-email: adam.kariv@gmail.com
 License: MIT
 Description: # dataflows-airtable
         Python library for adding AirTable support to dataflows
```

### Comparing `dataflows-airtable-0.1.0/dataflows_airtable.egg-info/SOURCES.txt` & `dataflows-airtable-0.1.1/dataflows_airtable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataflows-airtable-0.1.0/setup.py` & `dataflows-airtable-0.1.1/setup.py`

 * *Files identical despite different names*

