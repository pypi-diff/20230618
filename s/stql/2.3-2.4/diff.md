# Comparing `tmp/stql-2.3.tar.gz` & `tmp/stql-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stql-2.3.tar", last modified: Sun Jun 18 16:29:07 2023, max compression
+gzip compressed data, was "stql-2.4.tar", last modified: Sun Jun 18 16:43:14 2023, max compression
```

## Comparing `stql-2.3.tar` & `stql-2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:07.257373 stql-2.3/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:29:07.257373 stql-2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-18 16:29:07.257373 stql-2.3/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-06-18 16:28:41.000000 stql-2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:07.232899 stql-2.3/stql/
--rw-rw-rw-   0        0        0     9919 2023-06-18 16:28:33.000000 stql-2.3/stql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:07.254226 stql-2.3/stql.egg-info/
--rw-rw-rw-   0        0        0      101 2023-06-18 16:29:07.000000 stql-2.3/stql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-18 16:29:07.000000 stql-2.3/stql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:29:07.000000 stql-2.3/stql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 16:29:07.000000 stql-2.3/stql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-06-18 16:29:07.000000 stql-2.3/stql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 16:43:14.283736 stql-2.4/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:43:14.283736 stql-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:43:14.299374 stql-2.4/setup.cfg
+-rw-rw-rw-   0        0        0      210 2023-06-18 16:42:54.000000 stql-2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:43:14.275224 stql-2.4/stql/
+-rw-rw-rw-   0        0        0    18549 2023-06-18 16:42:42.000000 stql-2.4/stql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:43:14.283736 stql-2.4/stql.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2023-06-18 16:43:14.000000 stql-2.4/stql.egg-info/top_level.txt
```

