# Comparing `tmp/gpteasy-1.1.tar.gz` & `tmp/gpteasy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-1.1.tar", last modified: Sat Jun 17 22:17:59 2023, max compression
+gzip compressed data, was "gpteasy-1.1.1.tar", last modified: Sat Jun 17 22:20:34 2023, max compression
```

## Comparing `gpteasy-1.1.tar` & `gpteasy-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:17:59.816780 gpteasy-1.1/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5186 2023-06-17 22:17:59.816355 gpteasy-1.1/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 14:20:31.000000 gpteasy-1.1/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:17:59.813550 gpteasy-1.1/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.1/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    13176 2023-06-17 22:16:40.000000 gpteasy-1.1/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1/gpteasy/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:17:59.815839 gpteasy-1.1/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5186 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      276 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 22:17:59.000000 gpteasy-1.1/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1144 2023-06-17 22:17:06.000000 gpteasy-1.1/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 22:17:59.816904 gpteasy-1.1/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:20:34.810096 gpteasy-1.1.1/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.1.1/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:20:34.809817 gpteasy-1.1.1/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 22:20:27.000000 gpteasy-1.1.1/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:20:34.807372 gpteasy-1.1.1/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.1.1/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.1.1/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.1.1/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    13176 2023-06-17 22:16:40.000000 gpteasy-1.1.1/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.1.1/gpteasy/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 22:20:34.809457 gpteasy-1.1.1/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      276 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 22:20:34.000000 gpteasy-1.1.1/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1146 2023-06-17 22:20:27.000000 gpteasy-1.1.1/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 22:20:34.810176 gpteasy-1.1.1/setup.cfg
```

### Comparing `gpteasy-1.1/LICENSE` & `gpteasy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1/PKG-INFO` & `gpteasy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1
+Version: 1.1.1
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.0.3
+Current version: 1.1.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1/README.md` & `gpteasy-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.0.3
+Current version: 1.1.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1/gpteasy/commands.py` & `gpteasy-1.1.1/gpteasy/commands.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1/gpteasy/display.py` & `gpteasy-1.1.1/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1/gpteasy/gpt.py` & `gpteasy-1.1.1/gpteasy/gpt.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1/gpteasy/repl.py` & `gpteasy-1.1.1/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.1/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.1.1/gpteasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.1
+Version: 1.1.1
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.0.3
+Current version: 1.1.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.1/pyproject.toml` & `gpteasy-1.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "1.1"
+version = "1.1.1"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

