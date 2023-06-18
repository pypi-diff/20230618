# Comparing `tmp/hurricaneapi-0.1.4.tar.gz` & `tmp/hurricaneapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hurricaneapi-0.1.4.tar", last modified: Sun Jun 18 13:23:13 2023, max compression
+gzip compressed data, was "hurricaneapi-0.1.5.tar", last modified: Sun Jun 18 13:41:13 2023, max compression
```

## Comparing `hurricaneapi-0.1.4.tar` & `hurricaneapi-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 13:23:13.523260 hurricaneapi-0.1.4/
--rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      282 2023-06-18 13:23:13.523260 hurricaneapi-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 13:23:13.518262 hurricaneapi-0.1.4/hurricaneapi/
--rw-rw-rw-   0        0        0      170 2023-06-18 13:20:54.000000 hurricaneapi-0.1.4/hurricaneapi/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1.4/hurricaneapi/application.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:23:13.522261 hurricaneapi-0.1.4/hurricaneapi.egg-info/
--rw-rw-rw-   0        0        0      282 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-18 13:23:13.000000 hurricaneapi-0.1.4/hurricaneapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      455 2023-06-18 13:11:47.000000 hurricaneapi-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 13:23:13.524260 hurricaneapi-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-06-18 13:20:54.000000 hurricaneapi-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.458942 hurricaneapi-0.1.5/
+-rw-rw-rw-   0        0        0     1093 2023-02-25 18:34:13.000000 hurricaneapi-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      282 2023-06-18 13:41:13.458942 hurricaneapi-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-02-25 18:34:13.000000 hurricaneapi-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.444942 hurricaneapi-0.1.5/hurricaneapi/
+-rw-rw-rw-   0        0        0      107 2023-06-18 13:41:04.000000 hurricaneapi-0.1.5/hurricaneapi/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-03-01 18:38:34.000000 hurricaneapi-0.1.5/hurricaneapi/application.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.455942 hurricaneapi-0.1.5/hurricaneapi/responses/
+-rw-rw-rw-   0        0        0      254 2023-03-01 18:51:02.000000 hurricaneapi-0.1.5/hurricaneapi/responses/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 18:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/responses/file_response.py
+-rw-rw-rw-   0        0        0      365 2023-03-01 18:43:47.000000 hurricaneapi-0.1.5/hurricaneapi/responses/html_response.py
+-rw-rw-rw-   0        0        0      507 2023-03-01 18:48:19.000000 hurricaneapi-0.1.5/hurricaneapi/responses/json_response.py
+-rw-rw-rw-   0        0        0      371 2023-03-01 18:50:37.000000 hurricaneapi-0.1.5/hurricaneapi/responses/plain_text_response.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 18:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/responses/redirect_response.py
+-rw-rw-rw-   0        0        0     2332 2023-03-01 18:36:49.000000 hurricaneapi-0.1.5/hurricaneapi/responses/response.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 18:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/responses/streaming_response.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.457941 hurricaneapi-0.1.5/hurricaneapi/routing/
+-rw-rw-rw-   0        0        0        0 2023-06-18 13:38:35.000000 hurricaneapi-0.1.5/hurricaneapi/routing/__init__.py
+-rw-rw-rw-   0        0        0      351 2023-03-01 18:36:49.000000 hurricaneapi-0.1.5/hurricaneapi/routing/route.py
+-rw-rw-rw-   0        0        0     1143 2023-03-01 18:36:49.000000 hurricaneapi-0.1.5/hurricaneapi/routing/router.py
+drwxrwxrwx   0        0        0        0 2023-06-18 13:41:13.448943 hurricaneapi-0.1.5/hurricaneapi.egg-info/
+-rw-rw-rw-   0        0        0      282 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      702 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-06-18 13:41:13.000000 hurricaneapi-0.1.5/hurricaneapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      455 2023-06-18 13:11:47.000000 hurricaneapi-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 13:41:13.458942 hurricaneapi-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      448 2023-06-18 13:41:04.000000 hurricaneapi-0.1.5/setup.py
```

### Comparing `hurricaneapi-0.1.4/LICENSE` & `hurricaneapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hurricaneapi-0.1.4/hurricaneapi/application.py` & `hurricaneapi-0.1.5/hurricaneapi/application.py`

 * *Files identical despite different names*

