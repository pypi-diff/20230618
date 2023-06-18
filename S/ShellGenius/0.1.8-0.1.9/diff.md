# Comparing `tmp/shellgenius-0.1.8.tar.gz` & `tmp/shellgenius-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellgenius-0.1.8.tar", last modified: Tue Jun 13 20:36:09 2023, max compression
+gzip compressed data, was "shellgenius-0.1.9.tar", last modified: Sat Jun 17 18:55:15 2023, max compression
```

## Comparing `shellgenius-0.1.8.tar` & `shellgenius-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 20:36:09.957960 shellgenius-0.1.8/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.8/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 20:36:09.947960 shellgenius-0.1.8/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3488 2023-06-07 23:47:27.000000 shellgenius-0.1.8/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-13 20:36:09.957960 shellgenius-0.1.8/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-06-13 20:36:01.000000 shellgenius-0.1.8/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 20:36:09.947960 shellgenius-0.1.8/shellgenius/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.8/shellgenius/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-05-09 15:21:52.000000 shellgenius-0.1.8/shellgenius/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5452 2023-06-13 20:35:31.000000 shellgenius-0.1.8/shellgenius/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 20:36:09.947960 shellgenius-0.1.8/shellgenius.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      338 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-13 20:36:09.000000 shellgenius-0.1.8/shellgenius.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-17 18:55:15.483546 shellgenius-0.1.9/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-16 17:57:38.000000 shellgenius-0.1.9/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8098 2023-06-17 18:55:15.483546 shellgenius-0.1.9/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7965 2023-06-16 22:56:28.000000 shellgenius-0.1.9/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-17 18:55:15.483546 shellgenius-0.1.9/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-06-17 18:54:10.000000 shellgenius-0.1.9/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-17 18:55:15.483546 shellgenius-0.1.9/shellgenius/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.9/shellgenius/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-06-15 11:00:25.000000 shellgenius-0.1.9/shellgenius/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5452 2023-06-13 20:35:31.000000 shellgenius-0.1.9/shellgenius/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-17 18:55:15.483546 shellgenius-0.1.9/shellgenius.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8098 2023-06-17 18:55:15.000000 shellgenius-0.1.9/shellgenius.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-06-17 18:55:15.000000 shellgenius-0.1.9/shellgenius.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-17 18:55:15.000000 shellgenius-0.1.9/shellgenius.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-06-17 18:55:15.000000 shellgenius-0.1.9/shellgenius.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      338 2023-06-17 18:55:15.000000 shellgenius-0.1.9/shellgenius.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-17 18:55:15.000000 shellgenius-0.1.9/shellgenius.egg-info/top_level.txt
```

### Comparing `shellgenius-0.1.8/setup.py` & `shellgenius-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="shellgenius",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "shellgenius = shellgenius.cli:shellgenius",
         ]
     },
```

### Comparing `shellgenius-0.1.8/shellgenius/cli.py` & `shellgenius-0.1.9/shellgenius/cli.py`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.8/shellgenius/gpt_integration.py` & `shellgenius-0.1.9/shellgenius/gpt_integration.py`

 * *Files identical despite different names*

