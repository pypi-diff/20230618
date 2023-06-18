# Comparing `tmp/kkyCrawler-1.0.5.tar.gz` & `tmp/kkyCrawler-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkyCrawler-1.0.5.tar", last modified: Sun Jun 18 18:13:43 2023, max compression
+gzip compressed data, was "kkyCrawler-1.0.6.tar", last modified: Sun Jun 18 18:21:21 2023, max compression
```

## Comparing `kkyCrawler-1.0.5.tar` & `kkyCrawler-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 18:13:43.562776 kkyCrawler-1.0.5/
--rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      418 2023-06-18 18:13:43.561776 kkyCrawler-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.5/README.md
--rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 18:13:43.562776 kkyCrawler-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-06-18 18:08:09.000000 kkyCrawler-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:13:43.538814 kkyCrawler-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 18:13:43.549776 kkyCrawler-1.0.5/src/kkyCrawler/
--rw-rw-rw-   0        0        0       97 2023-06-18 18:13:14.000000 kkyCrawler-1.0.5/src/kkyCrawler/__init__.py
--rw-rw-rw-   0        0        0    15892 2023-06-18 18:11:49.000000 kkyCrawler-1.0.5/src/kkyCrawler/extractor.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:13:43.559779 kkyCrawler-1.0.5/src/kkyCrawler.egg-info/
--rw-rw-rw-   0        0        0      418 2023-06-18 18:13:43.000000 kkyCrawler-1.0.5/src/kkyCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-18 18:13:43.000000 kkyCrawler-1.0.5/src/kkyCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 18:13:43.000000 kkyCrawler-1.0.5/src/kkyCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-18 18:13:43.000000 kkyCrawler-1.0.5/src/kkyCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 18:13:43.000000 kkyCrawler-1.0.5/src/kkyCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 18:21:21.986114 kkyCrawler-1.0.6/
+-rw-rw-rw-   0        0        0       26 2023-06-18 16:20:09.000000 kkyCrawler-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      418 2023-06-18 18:21:21.985118 kkyCrawler-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2023-06-18 16:19:53.000000 kkyCrawler-1.0.6/README.md
+-rw-rw-rw-   0        0        0      180 2023-06-18 16:37:26.000000 kkyCrawler-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 18:21:21.986114 kkyCrawler-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-06-18 18:20:14.000000 kkyCrawler-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:21:21.955076 kkyCrawler-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 18:21:21.969428 kkyCrawler-1.0.6/src/kkyCrawler/
+-rw-rw-rw-   0        0        0       97 2023-06-18 18:13:14.000000 kkyCrawler-1.0.6/src/kkyCrawler/__init__.py
+-rw-rw-rw-   0        0        0    15892 2023-06-18 18:11:49.000000 kkyCrawler-1.0.6/src/kkyCrawler/extractor.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:21:21.983057 kkyCrawler-1.0.6/src/kkyCrawler.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-06-18 18:21:21.000000 kkyCrawler-1.0.6/src/kkyCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-06-18 18:21:21.000000 kkyCrawler-1.0.6/src/kkyCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:21:21.000000 kkyCrawler-1.0.6/src/kkyCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-18 18:21:21.000000 kkyCrawler-1.0.6/src/kkyCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 18:21:21.000000 kkyCrawler-1.0.6/src/kkyCrawler.egg-info/top_level.txt
```

### Comparing `kkyCrawler-1.0.5/setup.py` & `kkyCrawler-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-install_requires = [
-    "PyPDF2>=3.0.1",
-    "tqdm>=4.65",
-    "beautifulsoup4>=4.12.2",
-]
-
 setuptools.setup(
     name="kkyCrawler",
-    version="1.0.5",
+    version="1.0.6",
     author="eik4862",
     author_email="lkd1962@naver.com",
     description="law case crawling lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={},
@@ -23,10 +17,13 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.10",
-    setup_requires=install_requires,
-    install_requires=install_requires,
+    install_requires=[
+        "PyPDF2>=3.0.1",
+        "tqdm>=4.65",
+        "beautifulsoup4>=4.12.2",
+    ],
 )
```

### Comparing `kkyCrawler-1.0.5/src/kkyCrawler/extractor.py` & `kkyCrawler-1.0.6/src/kkyCrawler/extractor.py`

 * *Files identical despite different names*

