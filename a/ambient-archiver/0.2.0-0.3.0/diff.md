# Comparing `tmp/ambient-archiver-0.2.0.tar.gz` & `tmp/ambient-archiver-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-archiver-0.2.0.tar", last modified: Sun Nov  6 23:35:39 2022, max compression
+gzip compressed data, was "ambient-archiver-0.3.0.tar", last modified: Sun Jun 18 17:10:06 2023, max compression
```

## Comparing `ambient-archiver-0.2.0.tar` & `ambient-archiver-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 23:35:39.730988 ambient-archiver-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-11-06 23:35:39.730988 ambient-archiver-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-06 23:35:39.730988 ambient-archiver-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 23:35:39.726988 ambient-archiver-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 23:35:39.726988 ambient-archiver-0.2.0/src/ambient/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/src/ambient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/src/ambient/ambient.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/src/ambient/backfill.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-11-06 23:35:25.000000 ambient-archiver-0.2.0/src/ambient/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 23:35:39.730988 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-11-06 23:35:39.000000 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-11-06 23:35:39.000000 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 23:35:39.000000 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-06 23:35:39.000000 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-06 23:35:39.000000 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-06 23:35:39.000000 ambient-archiver-0.2.0/src/ambient_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:10:06.378931 ambient-archiver-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-18 17:10:06.378931 ambient-archiver-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-18 17:10:06.378931 ambient-archiver-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:10:06.374931 ambient-archiver-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:10:06.378931 ambient-archiver-0.3.0/src/ambient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/src/ambient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/src/ambient/ambient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/src/ambient/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-18 17:09:52.000000 ambient-archiver-0.3.0/src/ambient/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:10:06.378931 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-18 17:10:06.000000 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-18 17:10:06.000000 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:10:06.000000 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 17:10:06.000000 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 17:10:06.000000 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 17:10:06.000000 ambient-archiver-0.3.0/src/ambient_archiver.egg-info/top_level.txt
```

### Comparing `ambient-archiver-0.2.0/LICENSE` & `ambient-archiver-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ambient-archiver-0.2.0/PKG-INFO` & `ambient-archiver-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-archiver
-Version: 0.2.0
+Version: 0.3.0
 Summary: Archive your data from ambientweather.net
 Home-page: https://github.com/mikepqr/ambient-archiver
 Author: Mike Lee Williams
 Author-email: mike@mike.place
 Project-URL: Bug Reports, https://github.com/mikepqr/ambient-archiver/issues
 Project-URL: Source, https://github.com/mikepqr/ambient-archiver
 Keywords: weather
@@ -13,17 +13,19 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # ambient-archiver
 
 Download and analyse your data from ambientweather.net
 
 ## Installation
@@ -86,19 +88,19 @@
             - cron:  '*/5 * * * *'
 
         jobs:
           ambient:
             runs-on: ubuntu-latest
             steps:
             - name: Check out repo
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
             - name: Set up Python
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
-                python-version: 3.8
+                python-version: 3.10
             - name: Install Python dependencies
               run: |
                 pip install ambient-archiver
             - name: Overwrite since midnight
               env:
                 AMBIENT_MAC: ${{ secrets.AMBIENT_MAC }}
                 AMBIENT_API_KEY: ${{ secrets.AMBIENT_API_KEY }}
@@ -129,19 +131,19 @@
             - cron:  '0 1 * * *'
 
         jobs:
           daily:
             runs-on: ubuntu-latest
             steps:
             - name: Check out repo
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
             - name: Set up Python
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
-                python-version: 3.8
+                python-version: 3.10
             - name: Install Python dependencies
               run: |
                 pip install ambient-archiver
             - name: Overwrite yesterday
               env:
                 AMBIENT_MAC: ${{ secrets.AMBIENT_MAC }}
                 AMBIENT_API_KEY: ${{ secrets.AMBIENT_API_KEY }}
```

### Comparing `ambient-archiver-0.2.0/README.md` & `ambient-archiver-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,19 @@
             - cron:  '*/5 * * * *'
 
         jobs:
           ambient:
             runs-on: ubuntu-latest
             steps:
             - name: Check out repo
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
             - name: Set up Python
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
-                python-version: 3.8
+                python-version: 3.10
             - name: Install Python dependencies
               run: |
                 pip install ambient-archiver
             - name: Overwrite since midnight
               env:
                 AMBIENT_MAC: ${{ secrets.AMBIENT_MAC }}
                 AMBIENT_API_KEY: ${{ secrets.AMBIENT_API_KEY }}
@@ -105,19 +105,19 @@
             - cron:  '0 1 * * *'
 
         jobs:
           daily:
             runs-on: ubuntu-latest
             steps:
             - name: Check out repo
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
             - name: Set up Python
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
-                python-version: 3.8
+                python-version: 3.10
             - name: Install Python dependencies
               run: |
                 pip install ambient-archiver
             - name: Overwrite yesterday
               env:
                 AMBIENT_MAC: ${{ secrets.AMBIENT_MAC }}
                 AMBIENT_API_KEY: ${{ secrets.AMBIENT_API_KEY }}
```

### Comparing `ambient-archiver-0.2.0/src/ambient/ambient.py` & `ambient-archiver-0.3.0/src/ambient/ambient.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 def log_head_tail(data):
     try:
         logging.info(
             f"Got {len(data)} records from {data[-1]['date']} to {data[0]['date']}"
         )
     except IndexError:
-        raise ValueError(f"Got no records.")
+        raise ValueError("Got no records.")
     except KeyError:
         logging.info(f"{data}")
         raise ValueError("Data format invalid. Check api_key, application_key and mac.")
 
 
 def today(context=None):
     """Overwrite <today>.json.gz with all data since 00:00 UTC"""
```

### Comparing `ambient-archiver-0.2.0/src/ambient/backfill.py` & `ambient-archiver-0.3.0/src/ambient/backfill.py`

 * *Files identical despite different names*

### Comparing `ambient-archiver-0.2.0/src/ambient/cli.py` & `ambient-archiver-0.3.0/src/ambient/cli.py`

 * *Files identical despite different names*

### Comparing `ambient-archiver-0.2.0/src/ambient_archiver.egg-info/PKG-INFO` & `ambient-archiver-0.3.0/src/ambient_archiver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-archiver
-Version: 0.2.0
+Version: 0.3.0
 Summary: Archive your data from ambientweather.net
 Home-page: https://github.com/mikepqr/ambient-archiver
 Author: Mike Lee Williams
 Author-email: mike@mike.place
 Project-URL: Bug Reports, https://github.com/mikepqr/ambient-archiver/issues
 Project-URL: Source, https://github.com/mikepqr/ambient-archiver
 Keywords: weather
@@ -13,17 +13,19 @@
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # ambient-archiver
 
 Download and analyse your data from ambientweather.net
 
 ## Installation
@@ -86,19 +88,19 @@
             - cron:  '*/5 * * * *'
 
         jobs:
           ambient:
             runs-on: ubuntu-latest
             steps:
             - name: Check out repo
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
             - name: Set up Python
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
-                python-version: 3.8
+                python-version: 3.10
             - name: Install Python dependencies
               run: |
                 pip install ambient-archiver
             - name: Overwrite since midnight
               env:
                 AMBIENT_MAC: ${{ secrets.AMBIENT_MAC }}
                 AMBIENT_API_KEY: ${{ secrets.AMBIENT_API_KEY }}
@@ -129,19 +131,19 @@
             - cron:  '0 1 * * *'
 
         jobs:
           daily:
             runs-on: ubuntu-latest
             steps:
             - name: Check out repo
-              uses: actions/checkout@v2
+              uses: actions/checkout@v3
             - name: Set up Python
-              uses: actions/setup-python@v2
+              uses: actions/setup-python@v4
               with:
-                python-version: 3.8
+                python-version: 3.10
             - name: Install Python dependencies
               run: |
                 pip install ambient-archiver
             - name: Overwrite yesterday
               env:
                 AMBIENT_MAC: ${{ secrets.AMBIENT_MAC }}
                 AMBIENT_API_KEY: ${{ secrets.AMBIENT_API_KEY }}
```

