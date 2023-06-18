# Comparing `tmp/stql-1.0.tar.gz` & `tmp/stql-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stql-1.0.tar", last modified: Sun Jun 18 11:24:51 2023, max compression
+gzip compressed data, was "stql-2.0.tar", last modified: Sun Jun 18 16:19:41 2023, max compression
```

## Comparing `stql-1.0.tar` & `stql-2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 11:24:51.707588 stql-1.0/
--rw-rw-rw-   0        0        0      101 2023-06-18 11:24:51.707588 stql-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-18 11:24:51.708589 stql-1.0/setup.cfg
--rw-rw-rw-   0        0        0      210 2023-06-18 11:14:05.000000 stql-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 11:24:51.700456 stql-1.0/stql/
--rw-rw-rw-   0        0        0     6256 2023-06-18 11:24:01.000000 stql-1.0/stql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 11:24:51.706587 stql-1.0/stql.egg-info/
--rw-rw-rw-   0        0        0      101 2023-06-18 11:24:51.000000 stql-1.0/stql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-18 11:24:51.000000 stql-1.0/stql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 11:24:51.000000 stql-1.0/stql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-18 11:24:51.000000 stql-1.0/stql.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        5 2023-06-18 11:24:51.000000 stql-1.0/stql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 16:19:41.923390 stql-2.0/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:19:41.923390 stql-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:19:41.923390 stql-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      210 2023-06-18 16:19:20.000000 stql-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:19:41.907147 stql-2.0/stql/
+-rw-rw-rw-   0        0        0     9924 2023-06-18 16:18:39.000000 stql-2.0/stql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:19:41.923390 stql-2.0/stql.egg-info/
+-rw-rw-rw-   0        0        0      101 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        5 2023-06-18 16:19:41.000000 stql-2.0/stql.egg-info/top_level.txt
```

