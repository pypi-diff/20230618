# Comparing `tmp/gpt_heat_routes-0.1.tar.gz` & `tmp/gpt_heat_routes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_heat_routes-0.1.tar", last modified: Sun Jun 18 12:51:19 2023, max compression
+gzip compressed data, was "gpt_heat_routes-0.1.1.tar", last modified: Sun Jun 18 13:39:10 2023, max compression
```

## Comparing `gpt_heat_routes-0.1.tar` & `gpt_heat_routes-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 12:51:19.553506 gpt_heat_routes-0.1/
--rw-r--r--   0 christostrydom   (501) staff       (20)      241 2023-06-18 12:51:19.553246 gpt_heat_routes-0.1/PKG-INFO
--rw-r--r--   0 christostrydom   (501) staff       (20)     2264 2023-06-18 12:33:36.000000 gpt_heat_routes-0.1/README.md
-drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 12:51:19.550665 gpt_heat_routes-0.1/gpt_heat_routes/
--rw-r--r--   0 christostrydom   (501) staff       (20)       32 2023-06-18 12:41:18.000000 gpt_heat_routes-0.1/gpt_heat_routes/__init__.py
--rw-r--r--   0 christostrydom   (501) staff       (20)     9885 2023-06-17 09:41:19.000000 gpt_heat_routes-0.1/gpt_heat_routes/gpt_heat_routes.py
-drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 12:51:19.552835 gpt_heat_routes-0.1/gpt_heat_routes.egg-info/
--rw-r--r--   0 christostrydom   (501) staff       (20)      241 2023-06-18 12:51:19.000000 gpt_heat_routes-0.1/gpt_heat_routes.egg-info/PKG-INFO
--rw-r--r--   0 christostrydom   (501) staff       (20)      275 2023-06-18 12:51:19.000000 gpt_heat_routes-0.1/gpt_heat_routes.egg-info/SOURCES.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)        1 2023-06-18 12:51:19.000000 gpt_heat_routes-0.1/gpt_heat_routes.egg-info/dependency_links.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)       58 2023-06-18 12:51:19.000000 gpt_heat_routes-0.1/gpt_heat_routes.egg-info/requires.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)       16 2023-06-18 12:51:19.000000 gpt_heat_routes-0.1/gpt_heat_routes.egg-info/top_level.txt
--rw-r--r--   0 christostrydom   (501) staff       (20)       38 2023-06-18 12:51:19.553571 gpt_heat_routes-0.1/setup.cfg
--rw-r--r--   0 christostrydom   (501) staff       (20)      514 2023-06-18 12:51:14.000000 gpt_heat_routes-0.1/setup.py
+drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 13:39:10.320149 gpt_heat_routes-0.1.1/
+-rw-r--r--   0 christostrydom   (501) staff       (20)      243 2023-06-18 13:39:10.319889 gpt_heat_routes-0.1.1/PKG-INFO
+-rw-r--r--   0 christostrydom   (501) staff       (20)     2264 2023-06-18 12:33:36.000000 gpt_heat_routes-0.1.1/README.md
+drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 13:39:10.316353 gpt_heat_routes-0.1.1/gpt_heat_routes/
+-rw-r--r--   0 christostrydom   (501) staff       (20)       32 2023-06-18 12:41:18.000000 gpt_heat_routes-0.1.1/gpt_heat_routes/__init__.py
+-rw-r--r--   0 christostrydom   (501) staff       (20)     9885 2023-06-17 09:41:19.000000 gpt_heat_routes-0.1.1/gpt_heat_routes/gpt_heat_routes.py
+drwxr-xr-x   0 christostrydom   (501) staff       (20)        0 2023-06-18 13:39:10.319485 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/
+-rw-r--r--   0 christostrydom   (501) staff       (20)      243 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/PKG-INFO
+-rw-r--r--   0 christostrydom   (501) staff       (20)      275 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/SOURCES.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)        1 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/dependency_links.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)       53 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/requires.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)       16 2023-06-18 13:39:10.000000 gpt_heat_routes-0.1.1/gpt_heat_routes.egg-info/top_level.txt
+-rw-r--r--   0 christostrydom   (501) staff       (20)       38 2023-06-18 13:39:10.320218 gpt_heat_routes-0.1.1/setup.cfg
+-rw-r--r--   0 christostrydom   (501) staff       (20)      500 2023-06-18 13:38:15.000000 gpt_heat_routes-0.1.1/setup.py
```

### Comparing `gpt_heat_routes-0.1/README.md` & `gpt_heat_routes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gpt_heat_routes-0.1/gpt_heat_routes/gpt_heat_routes.py` & `gpt_heat_routes-0.1.1/gpt_heat_routes/gpt_heat_routes.py`

 * *Files identical despite different names*

