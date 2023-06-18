# Comparing `tmp/CKAstroTools-0.0.1.tar.gz` & `tmp/CKAstroTools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/koenig/PycharmProjects/ckastrotools/dist/.tmp-7rkqnlxr/CKAstroTools-0.0.1.tar", last modified: Sun Jun 18 09:31:54 2023, max compression
+gzip compressed data, was "/home/koenig/PycharmProjects/ckastrotools/dist/.tmp-sby0dqam/CKAstroTools-0.0.2.tar", last modified: Sun Jun 18 09:39:16 2023, max compression
```

## Comparing `CKAstroTools-0.0.1.tar` & `CKAstroTools-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/CKAstroTools.egg-info/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/CKAstroTools.egg-info/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      393 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/CKAstroTools.egg-info/SOURCES.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/CKAstroTools.egg-info/dependency_links.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/CKAstroTools.egg-info/requires.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       11 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/CKAstroTools.egg-info/top_level.txt
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.1/LICENSE
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/PKG-INFO
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      750 2023-06-18 09:30:05.000000 CKAstroTools-0.0.1/README.md
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/ckastrokit/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.1/ckastrokit/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.1/ckastrokit/__main__.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/ckastrokit/io/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.1/ckastrokit/io/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.1/ckastrokit/io/subcube.py
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/ckastrokit/milkyway/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.1/ckastrokit/milkyway/__init__.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)    16547 2023-06-16 04:26:53.000000 CKAstroTools-0.0.1/ckastrokit/milkyway/spiralarms.py
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-18 09:30:45.000000 CKAstroTools-0.0.1/pyproject.toml
--rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/setup.cfg
-drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:31:54.000000 CKAstroTools-0.0.1/tests/
--rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.1/tests/test_main.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      405 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       14 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/requires.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       13 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/CKAstroTools.egg-info/top_level.txt
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1071 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/LICENSE
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1352 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/PKG-INFO
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      750 2023-06-18 09:30:05.000000 CKAstroTools-0.0.2/README.md
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/ckastrotools/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        1 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/ckastrotools/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       78 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/ckastrotools/__main__.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/ckastrotools/io/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       31 2022-12-19 10:11:43.000000 CKAstroTools-0.0.2/ckastrotools/io/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)     1270 2022-12-19 10:33:57.000000 CKAstroTools-0.0.2/ckastrotools/io/subcube.py
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/ckastrotools/milkyway/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)        0 2023-06-10 14:05:04.000000 CKAstroTools-0.0.2/ckastrotools/milkyway/__init__.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)    16547 2023-06-16 04:26:53.000000 CKAstroTools-0.0.2/ckastrotools/milkyway/spiralarms.py
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      826 2023-06-18 09:37:37.000000 CKAstroTools-0.0.2/pyproject.toml
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)       38 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/setup.cfg
+drwxrwxr-x   0 koenig    (1000) koenig    (1000)        0 2023-06-18 09:39:16.000000 CKAstroTools-0.0.2/tests/
+-rw-rw-r--   0 koenig    (1000) koenig    (1000)      146 2022-12-19 09:28:13.000000 CKAstroTools-0.0.2/tests/test_main.py
```

### Comparing `CKAstroTools-0.0.1/CKAstroTools.egg-info/PKG-INFO` & `CKAstroTools-0.0.2/CKAstroTools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.1
+Version: 0.0.2
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CKAstroTools-0.0.1/LICENSE` & `CKAstroTools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.1/PKG-INFO` & `CKAstroTools-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CKAstroTools
-Version: 0.0.1
+Version: 0.0.2
 Summary: General toolks for astronomy I personally use regularly for data analysis.
 Author: Carsten König
 License: MIT License
 Project-URL: Homepage, https://gitlab.com/ck2go/ckastrotools
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CKAstroTools-0.0.1/README.md` & `CKAstroTools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.1/ckastrokit/io/subcube.py` & `CKAstroTools-0.0.2/ckastrotools/io/subcube.py`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.1/ckastrokit/milkyway/spiralarms.py` & `CKAstroTools-0.0.2/ckastrotools/milkyway/spiralarms.py`

 * *Files identical despite different names*

### Comparing `CKAstroTools-0.0.1/pyproject.toml` & `CKAstroTools-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             "pytest",
             "pytest-mock"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "CKAstroTools"
 description = "General toolks for astronomy I personally use regularly for data analysis."
-version = "0.0.1"
+version = "0.0.2"
 requires-python = ">=3.7"
 dependencies = ["spectral-cube"]
 keywords = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

