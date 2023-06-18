# Comparing `tmp/hurricaneapi-0.1.3.tar.gz` & `tmp/hurricaneapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurricaneapi-0.1.3.tar", last modified: Sun Jun 18 13:13:13 2023, max compression
+gzip compressed data, was "hurricaneapi-0.1.4.tar", last modified: Sun Jun 18 13:23:13 2023, max compression
```

## Comparing `hurricaneapi-0.1.3.tar` & `hurricaneapi-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 13:13:13.643011 hurricaneapi-0.1.3/
--rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      282 2023-06-18 13:13:13.643011 hurricaneapi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 13:13:13.639013 hurricaneapi-0.1.3/hurricaneapi/
--rw-rw-rw-   0        0        0       78 2023-06-18 13:12:10.000000 hurricaneapi-0.1.3/hurricaneapi/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1.3/hurricaneapi/application.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:13:13.643011 hurricaneapi-0.1.3/hurricaneapi.egg-info/
--rw-rw-rw-   0        0        0      282 2023-06-18 13:13:13.000000 hurricaneapi-0.1.3/hurricaneapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-18 13:13:13.000000 hurricaneapi-0.1.3/hurricaneapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 13:13:13.000000 hurricaneapi-0.1.3/hurricaneapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 13:13:13.000000 hurricaneapi-0.1.3/hurricaneapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-18 13:13:13.000000 hurricaneapi-0.1.3/hurricaneapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      455 2023-06-18 13:11:47.000000 hurricaneapi-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 13:13:13.644014 hurricaneapi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-06-18 13:13:05.000000 hurricaneapi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:23:13.523260 hurricaneapi-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      282 2023-06-18 13:23:13.523260 hurricaneapi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 13:23:13.518262 hurricaneapi-0.1.4/hurricaneapi/
+-rw-rw-rw-   0        0        0      170 2023-06-18 13:20:54.000000 hurricaneapi-0.1.4/hurricaneapi/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1.4/hurricaneapi/application.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:23:13.522261 hurricaneapi-0.1.4/hurricaneapi.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      455 2023-06-18 13:11:47.000000 hurricaneapi-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:23:13.524260 hurricaneapi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      398 2023-06-18 13:20:54.000000 hurricaneapi-0.1.4/setup.py
```

### Comparing `hurricaneapi-0.1.3/LICENSE` & `hurricaneapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hurricaneapi-0.1.3/hurricaneapi/application.py` & `hurricaneapi-0.1.4/hurricaneapi/application.py`

 * *Files identical despite different names*

