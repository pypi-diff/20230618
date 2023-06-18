# Comparing `tmp/kkyCrawler-1.0.1.tar.gz` & `tmp/kkyCrawler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyCrawler-1.0.1.tar", last modified: Sun Jun 18 16:39:16 2023, max compression
+gzip compressed data, was "kkyCrawler-1.0.2.tar", last modified: Sun Jun 18 17:40:38 2023, max compression
```

## Comparing `kkyCrawler-1.0.1.tar` & `kkyCrawler-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.134730 kkyCrawler-1.0.1/
--rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      418 2023-06-18 16:39:16.133731 kkyCrawler-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.1/README.md
--rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 16:39:16.134730 kkyCrawler-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-06-18 16:37:58.000000 kkyCrawler-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.101603 kkyCrawler-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.120397 kkyCrawler-1.0.1/src/kkyCrawler/
--rw-rw-rw-   0        0        0        0 2023-06-18 16:13:06.000000 kkyCrawler-1.0.1/src/kkyCrawler/__init__.py
--rw-rw-rw-   0        0        0    15799 2023-06-18 16:19:00.000000 kkyCrawler-1.0.1/src/kkyCrawler/kkycrawler.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.132748 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/
--rw-rw-rw-   0        0        0      418 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:38.931676 kkyCrawler-1.0.2/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      418 2023-06-18 17:40:38.930675 kkyCrawler-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.2/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:40:38.931676 kkyCrawler-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-06-18 17:40:20.000000 kkyCrawler-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:38.890948 kkyCrawler-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:38.913067 kkyCrawler-1.0.2/src/kkyCrawler/
+-rw-rw-rw-   0        0        0        0 2023-06-18 16:13:06.000000 kkyCrawler-1.0.2/src/kkyCrawler/__init__.py
+-rw-rw-rw-   0        0        0    15799 2023-06-18 16:19:00.000000 kkyCrawler-1.0.2/src/kkyCrawler/kkycrawler.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:40:38.928686 kkyCrawler-1.0.2/src/kkyCrawler.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-18 17:40:38.000000 kkyCrawler-1.0.2/src/kkyCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-18 17:40:38.000000 kkyCrawler-1.0.2/src/kkyCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:40:38.000000 kkyCrawler-1.0.2/src/kkyCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-18 17:40:38.000000 kkyCrawler-1.0.2/src/kkyCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 17:40:38.000000 kkyCrawler-1.0.2/src/kkyCrawler.egg-info/top_level.txt
```

### Comparing `kkyCrawler-1.0.1/src/kkyCrawler/kkycrawler.py` & `kkyCrawler-1.0.2/src/kkyCrawler/kkycrawler.py`

 * *Files identical despite different names*

