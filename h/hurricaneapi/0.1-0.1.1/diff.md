# Comparing `tmp/hurricaneapi-0.1.tar.gz` & `tmp/hurricaneapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurricaneapi-0.1.tar", last modified: Sun Jun 18 12:42:27 2023, max compression
+gzip compressed data, was "hurricaneapi-0.1.1.tar", last modified: Sun Jun 18 12:55:10 2023, max compression
```

## Comparing `hurricaneapi-0.1.tar` & `hurricaneapi-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 12:42:27.829409 hurricaneapi-0.1/
--rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1/LICENSE
--rw-rw-rw-   0        0        0      216 2023-06-18 12:42:27.829409 hurricaneapi-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 12:42:27.824410 hurricaneapi-0.1/hurricaneapi/
--rw-rw-rw-   0        0        0       51 2023-03-01 18:36:49.000000 hurricaneapi-0.1/hurricaneapi/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1/hurricaneapi/application.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:42:27.828409 hurricaneapi-0.1/hurricaneapi.egg-info/
--rw-rw-rw-   0        0        0      216 2023-06-18 12:42:27.000000 hurricaneapi-0.1/hurricaneapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-18 12:42:27.000000 hurricaneapi-0.1/hurricaneapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 12:42:27.000000 hurricaneapi-0.1/hurricaneapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 12:42:27.000000 hurricaneapi-0.1/hurricaneapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-18 12:42:27.000000 hurricaneapi-0.1/hurricaneapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      375 2023-06-18 12:34:08.000000 hurricaneapi-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 12:42:27.830408 hurricaneapi-0.1/setup.cfg
--rw-rw-rw-   0        0        0      233 2023-06-18 12:40:49.000000 hurricaneapi-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:55:10.861177 hurricaneapi-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      282 2023-06-18 12:55:10.861177 hurricaneapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 12:55:10.856177 hurricaneapi-0.1.1/hurricaneapi/
+-rw-rw-rw-   0        0        0       51 2023-03-01 18:36:49.000000 hurricaneapi-0.1.1/hurricaneapi/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1.1/hurricaneapi/application.py
+drwxrwxrwx   0        0        0        0 2023-06-18 12:55:10.860177 hurricaneapi-0.1.1/hurricaneapi.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-06-18 12:55:10.000000 hurricaneapi-0.1.1/hurricaneapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-18 12:55:10.000000 hurricaneapi-0.1.1/hurricaneapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 12:55:10.000000 hurricaneapi-0.1.1/hurricaneapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 12:55:10.000000 hurricaneapi-0.1.1/hurricaneapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-18 12:55:10.000000 hurricaneapi-0.1.1/hurricaneapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      375 2023-06-18 12:34:08.000000 hurricaneapi-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 12:55:10.861177 hurricaneapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-06-18 12:54:07.000000 hurricaneapi-0.1.1/setup.py
```

### Comparing `hurricaneapi-0.1/LICENSE` & `hurricaneapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hurricaneapi-0.1/hurricaneapi/application.py` & `hurricaneapi-0.1.1/hurricaneapi/application.py`

 * *Files identical despite different names*

