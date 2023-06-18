# Comparing `tmp/kkyCrawler-0.0.1.tar.gz` & `tmp/kkyCrawler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyCrawler-0.0.1.tar", last modified: Sun Jun 18 16:29:21 2023, max compression
+gzip compressed data, was "kkyCrawler-1.0.1.tar", last modified: Sun Jun 18 16:39:16 2023, max compression
```

## Comparing `kkyCrawler-0.0.1.tar` & `kkyCrawler-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:21.668026 kkyCrawler-0.0.1/
--rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      418 2023-06-18 16:29:21.666953 kkyCrawler-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-18 16:18:39.000000 kkyCrawler-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 16:29:21.668026 kkyCrawler-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-06-18 16:19:33.000000 kkyCrawler-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:21.644282 kkyCrawler-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:21.653386 kkyCrawler-0.0.1/src/kkyCrawler/
--rw-rw-rw-   0        0        0        0 2023-06-18 16:13:06.000000 kkyCrawler-0.0.1/src/kkyCrawler/__init__.py
--rw-rw-rw-   0        0        0    15799 2023-06-18 16:19:00.000000 kkyCrawler-0.0.1/src/kkyCrawler/kkycrawler.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:29:21.665393 kkyCrawler-0.0.1/src/kkyCrawler.egg-info/
--rw-rw-rw-   0        0        0      418 2023-06-18 16:29:21.000000 kkyCrawler-0.0.1/src/kkyCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-18 16:29:21.000000 kkyCrawler-0.0.1/src/kkyCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:29:21.000000 kkyCrawler-0.0.1/src/kkyCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 16:29:21.000000 kkyCrawler-0.0.1/src/kkyCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.134730 kkyCrawler-1.0.1/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      418 2023-06-18 16:39:16.133731 kkyCrawler-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.1/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:39:16.134730 kkyCrawler-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      697 2023-06-18 16:37:58.000000 kkyCrawler-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.101603 kkyCrawler-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.120397 kkyCrawler-1.0.1/src/kkyCrawler/
+-rw-rw-rw-   0        0        0        0 2023-06-18 16:13:06.000000 kkyCrawler-1.0.1/src/kkyCrawler/__init__.py
+-rw-rw-rw-   0        0        0    15799 2023-06-18 16:19:00.000000 kkyCrawler-1.0.1/src/kkyCrawler/kkycrawler.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:39:16.132748 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 16:39:16.000000 kkyCrawler-1.0.1/src/kkyCrawler.egg-info/top_level.txt
```

### Comparing `kkyCrawler-0.0.1/setup.py` & `kkyCrawler-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kkyCrawler",
-    version="0.0.1",
+    version="1.0.1",
     author="eik4862",
     author_email="lkd1962@naver.com",
     description="law case crawling lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={},
```

### Comparing `kkyCrawler-0.0.1/src/kkyCrawler/kkycrawler.py` & `kkyCrawler-1.0.1/src/kkyCrawler/kkycrawler.py`

 * *Files identical despite different names*

