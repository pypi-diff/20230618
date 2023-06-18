# Comparing `tmp/next-bus-bot-1.2.1.tar.gz` & `tmp/next-bus-bot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next-bus-bot-1.2.1.tar", last modified: Sun Jun 18 10:19:07 2023, max compression
+gzip compressed data, was "next-bus-bot-1.3.0.tar", last modified: Sun Jun 18 13:23:04 2023, max compression
```

## Comparing `next-bus-bot-1.2.1.tar` & `next-bus-bot-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.561010 next-bus-bot-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/.github/workflows/linters.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 10:19:07.561010 next-bus-bot-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/src/nbb/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/nbb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/api_call.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/idfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 10:18:44.000000 next-bus-bot-1.2.1/src/nbb/nbb_conf.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 10:19:07.557009 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 10:19:07.000000 next-bus-bot-1.2.1/src/next_bus_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.526615 next-bus-bot-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.530615 next-bus-bot-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/.github/workflows/linters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.526615 next-bus-bot-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.530615 next-bus-bot-1.3.0/src/nbb/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/nbb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/bot_discord.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1053 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/idfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-18 13:22:48.000000 next-bus-bot-1.3.0/src/nbb/nbb_conf.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 13:23:04.534615 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-18 13:23:04.000000 next-bus-bot-1.3.0/src/next_bus_bot.egg-info/top_level.txt
```

### Comparing `next-bus-bot-1.2.1/.github/workflows/linters.yml` & `next-bus-bot-1.3.0/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/.github/workflows/python-publish.yml` & `next-bus-bot-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/LICENSE.txt` & `next-bus-bot-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/PKG-INFO` & `next-bus-bot-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.2.1
+Version: 1.3.0
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2022 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: discord
 License-File: LICENSE.txt
 
 ===============
 Next Bus Bot
 ===============
 
 A bot/ cli tool that simply gives you the waiting times for next buses at your favorite bus stop.
```

### Comparing `next-bus-bot-1.2.1/README.rst` & `next-bus-bot-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/pyproject.toml` & `next-bus-bot-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 [project.scripts]
 nbb = "nbb.cli:main"
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "pytest-xdist", "pytest-sugar"]
 dev = ["black", "isort"]
+discord = ["discord.py"]
 
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "setuptools_scm[toml]>=6.2", "wheel"]
 build-backend = "setuptools.build_meta"
```

### Comparing `next-bus-bot-1.2.1/src/nbb/api_call.py` & `next-bus-bot-1.3.0/src/nbb/api_call.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/src/nbb/config.py` & `next-bus-bot-1.3.0/src/nbb/config.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/src/nbb/idfm.py` & `next-bus-bot-1.3.0/src/nbb/idfm.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/src/nbb/nbb_conf.toml` & `next-bus-bot-1.3.0/src/nbb/nbb_conf.toml`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.2.1/src/next_bus_bot.egg-info/PKG-INFO` & `next-bus-bot-1.3.0/src/next_bus_bot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.2.1
+Version: 1.3.0
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2022 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: discord
 License-File: LICENSE.txt
 
 ===============
 Next Bus Bot
 ===============
 
 A bot/ cli tool that simply gives you the waiting times for next buses at your favorite bus stop.
```

