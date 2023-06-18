# Comparing `tmp/kkyCrawler-1.0.3.tar.gz` & `tmp/kkyCrawler-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyCrawler-1.0.3.tar", last modified: Sun Jun 18 17:49:10 2023, max compression
+gzip compressed data, was "kkyCrawler-1.0.4.tar", last modified: Sun Jun 18 17:57:19 2023, max compression
```

## Comparing `kkyCrawler-1.0.3.tar` & `kkyCrawler-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 17:49:10.437754 kkyCrawler-1.0.3/
--rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      418 2023-06-18 17:49:10.437754 kkyCrawler-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.3/README.md
--rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 17:49:10.437754 kkyCrawler-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-06-18 17:48:57.000000 kkyCrawler-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:49:10.419888 kkyCrawler-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 17:49:10.437754 kkyCrawler-1.0.3/src/kkyCrawler/
--rw-rw-rw-   0        0        0        0 2023-06-18 16:13:06.000000 kkyCrawler-1.0.3/src/kkyCrawler/__init__.py
--rw-rw-rw-   0        0        0    15799 2023-06-18 16:19:00.000000 kkyCrawler-1.0.3/src/kkyCrawler/kkycrawler.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:49:10.437754 kkyCrawler-1.0.3/src/kkyCrawler.egg-info/
--rw-rw-rw-   0        0        0      418 2023-06-18 17:49:10.000000 kkyCrawler-1.0.3/src/kkyCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-18 17:49:10.000000 kkyCrawler-1.0.3/src/kkyCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 17:49:10.000000 kkyCrawler-1.0.3/src/kkyCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 17:49:10.000000 kkyCrawler-1.0.3/src/kkyCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 17:57:19.228912 kkyCrawler-1.0.4/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      418 2023-06-18 17:57:19.228912 kkyCrawler-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.4/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:57:19.229945 kkyCrawler-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-06-18 17:57:06.000000 kkyCrawler-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:57:19.198969 kkyCrawler-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 17:57:19.216480 kkyCrawler-1.0.4/src/kkyCrawler/
+-rw-rw-rw-   0        0        0       53 2023-06-18 17:56:51.000000 kkyCrawler-1.0.4/src/kkyCrawler/__init__.py
+-rw-rw-rw-   0        0        0    15799 2023-06-18 16:19:00.000000 kkyCrawler-1.0.4/src/kkyCrawler/kkycrawler.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:57:19.226915 kkyCrawler-1.0.4/src/kkyCrawler.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-18 17:57:19.000000 kkyCrawler-1.0.4/src/kkyCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-18 17:57:19.000000 kkyCrawler-1.0.4/src/kkyCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:57:19.000000 kkyCrawler-1.0.4/src/kkyCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 17:57:19.000000 kkyCrawler-1.0.4/src/kkyCrawler.egg-info/top_level.txt
```

### Comparing `kkyCrawler-1.0.3/setup.py` & `kkyCrawler-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "PyPDF2>=3.0.1",
     "tqdm>=4.65",
     "beautifulsoup4>=4.12.2",
 ]
 
 setuptools.setup(
     name="kkyCrawler",
-    version="1.0.3",
+    version="1.0.4",
     author="eik4862",
     author_email="lkd1962@naver.com",
     description="law case crawling lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={},
```

### Comparing `kkyCrawler-1.0.3/src/kkyCrawler/kkycrawler.py` & `kkyCrawler-1.0.4/src/kkyCrawler/kkycrawler.py`

 * *Files identical despite different names*

