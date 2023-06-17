# Comparing `tmp/skmetpy-0.0.6.tar.gz` & `tmp/skmetpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.0.6.tar", last modified: Sat Jun 17 16:17:32 2023, max compression
+gzip compressed data, was "skmetpy-0.0.7.tar", last modified: Sat Jun 17 21:59:51 2023, max compression
```

## Comparing `skmetpy-0.0.6.tar` & `skmetpy-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:17:32.665884 skmetpy-0.0.6/
--rw-rw-rw-   0        0        0      259 2023-06-17 16:17:32.665884 skmetpy-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:17:32.659893 skmetpy-0.0.6/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.6/nunpy/__init__.py
--rw-rw-rw-   0        0        0    17657 2023-06-17 16:17:23.000000 skmetpy-0.0.6/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-17 16:17:32.665884 skmetpy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-17 16:17:30.000000 skmetpy-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:17:32.664883 skmetpy-0.0.6/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 16:17:32.000000 skmetpy-0.0.6/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 21:59:51.109706 skmetpy-0.0.7/
+-rw-rw-rw-   0        0        0      259 2023-06-17 21:59:51.109706 skmetpy-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 21:59:51.104011 skmetpy-0.0.7/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.7/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    24940 2023-06-17 21:59:38.000000 skmetpy-0.0.7/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 21:59:51.109706 skmetpy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-17 21:59:43.000000 skmetpy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:59:51.108703 skmetpy-0.0.7/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-17 21:59:50.000000 skmetpy-0.0.7/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-17 21:59:50.000000 skmetpy-0.0.7/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 21:59:50.000000 skmetpy-0.0.7/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 21:59:50.000000 skmetpy-0.0.7/skmetpy.egg-info/top_level.txt
```

