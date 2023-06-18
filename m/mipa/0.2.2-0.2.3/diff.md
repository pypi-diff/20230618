# Comparing `tmp/mipa-0.2.2.tar.gz` & `tmp/mipa-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipa-0.2.2.tar", last modified: Tue Apr 25 08:53:03 2023, max compression
+gzip compressed data, was "mipa-0.2.3.tar", last modified: Sun Jun 18 02:35:22 2023, max compression
```

## Comparing `mipa-0.2.2.tar` & `mipa-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 08:52:51.000000 mipa-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 08:52:51.000000 mipa-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-25 08:53:03.218676 mipa-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-25 08:52:51.000000 mipa-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 08:52:51.000000 mipa-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 08:52:51.000000 mipa-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 08:53:03.218676 mipa-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 08:52:51.000000 mipa-0.2.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 08:52:51.000000 mipa-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:35:08.000000 mipa-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-18 02:35:08.000000 mipa-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-18 02:35:22.596957 mipa-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-18 02:35:08.000000 mipa-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-18 02:35:08.000000 mipa-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 02:35:08.000000 mipa-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-18 02:35:22.596957 mipa-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-18 02:35:08.000000 mipa-0.2.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-18 02:35:08.000000 mipa-0.2.3/versioneer.py
```

### Comparing `mipa-0.2.2/LICENSE` & `mipa-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/PKG-INFO` & `mipa-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipa
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/MiPA
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mipa-0.2.2/README.md` & `mipa-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/client.py` & `mipa-0.2.3/mipa/client.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/exception.py` & `mipa-0.2.3/mipa/exception.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/ext/commands/_types.py` & `mipa-0.2.3/mipa/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/ext/commands/bot.py` & `mipa-0.2.3/mipa/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/ext/commands/cog.py` & `mipa-0.2.3/mipa/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/ext/commands/context.py` & `mipa-0.2.3/mipa/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/ext/commands/core.py` & `mipa-0.2.3/mipa/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/ext/tasks/__init__.py` & `mipa-0.2.3/mipa/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/gateway.py` & `mipa-0.2.3/mipa/gateway.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/http.py` & `mipa-0.2.3/mipa/http.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/router.py` & `mipa-0.2.3/mipa/router.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/state.py` & `mipa-0.2.3/mipa/state.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa/utils.py` & `mipa-0.2.3/mipa/utils.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/mipa.egg-info/PKG-INFO` & `mipa-0.2.3/mipa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipa
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/MiPA
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mipa-0.2.2/mipa.egg-info/SOURCES.txt` & `mipa-0.2.3/mipa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/setup.py` & `mipa-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.2/versioneer.py` & `mipa-0.2.3/versioneer.py`

 * *Files identical despite different names*

