# Comparing `tmp/scify-file-reader-0.0.1.tar.gz` & `tmp/scify-file-reader-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scify-file-reader-0.0.1.tar", last modified: Sun Jun 18 16:19:21 2023, max compression
+gzip compressed data, was "scify-file-reader-0.0.2.tar", last modified: Sun Jun 18 16:38:37 2023, max compression
```

## Comparing `scify-file-reader-0.0.1.tar` & `scify-file-reader-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 16:19:21.430221 scify-file-reader-0.0.1/
--rw-rw-rw-   0        0        0     6264 2023-06-18 16:19:21.428224 scify-file-reader-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5355 2023-06-18 14:42:03.000000 scify-file-reader-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 16:19:21.003747 scify-file-reader-0.0.1/scify_file_reader/
--rw-rw-rw-   0        0        0       58 2023-06-18 02:24:11.000000 scify-file-reader-0.0.1/scify_file_reader/__init__.py
--rw-rw-rw-   0        0        0     5033 2023-06-18 15:58:50.000000 scify-file-reader-0.0.1/scify_file_reader/file_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-18 16:19:21.348105 scify-file-reader-0.0.1/scify_file_reader.egg-info/
--rw-rw-rw-   0        0        0     6264 2023-06-18 16:19:20.000000 scify-file-reader-0.0.1/scify_file_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-18 16:19:20.000000 scify-file-reader-0.0.1/scify_file_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 16:19:20.000000 scify-file-reader-0.0.1/scify_file_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-18 16:19:20.000000 scify-file-reader-0.0.1/scify_file_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-18 16:19:20.000000 scify-file-reader-0.0.1/scify_file_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 16:19:21.431225 scify-file-reader-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1265 2023-06-18 14:35:14.000000 scify-file-reader-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:38:37.369794 scify-file-reader-0.0.2/
+-rw-rw-rw-   0        0        0     6264 2023-06-18 16:38:37.367797 scify-file-reader-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5355 2023-06-18 14:42:03.000000 scify-file-reader-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 16:38:37.019124 scify-file-reader-0.0.2/scify_file_reader/
+-rw-rw-rw-   0        0        0       58 2023-06-18 16:35:05.000000 scify-file-reader-0.0.2/scify_file_reader/__init__.py
+-rw-rw-rw-   0        0        0     8069 2023-06-18 16:33:32.000000 scify-file-reader-0.0.2/scify_file_reader/file_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-18 16:38:37.290309 scify-file-reader-0.0.2/scify_file_reader.egg-info/
+-rw-rw-rw-   0        0        0     6264 2023-06-18 16:38:36.000000 scify-file-reader-0.0.2/scify_file_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-06-18 16:38:36.000000 scify-file-reader-0.0.2/scify_file_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 16:38:36.000000 scify-file-reader-0.0.2/scify_file_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-18 16:38:36.000000 scify-file-reader-0.0.2/scify_file_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-18 16:38:36.000000 scify-file-reader-0.0.2/scify_file_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 16:38:37.370899 scify-file-reader-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1265 2023-06-18 14:35:14.000000 scify-file-reader-0.0.2/setup.py
```

### Comparing `scify-file-reader-0.0.1/PKG-INFO` & `scify-file-reader-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scify-file-reader
-Version: 0.0.1
+Version: 0.0.2
 Summary: A class to handle and process multiple files with identical structures within a directory.
 Home-page: https://github.com/Jeferson-Peter/scify-file-reader
 Author: Jeferson-Peter (Jeferson Peter)
 Author-email: jeferson.peter@pm.me
 Keywords: Python,File Reading,Multiple File Handler
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `scify-file-reader-0.0.1/README.md` & `scify-file-reader-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scify-file-reader-0.0.1/scify_file_reader.egg-info/PKG-INFO` & `scify-file-reader-0.0.2/scify_file_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scify-file-reader
-Version: 0.0.1
+Version: 0.0.2
 Summary: A class to handle and process multiple files with identical structures within a directory.
 Home-page: https://github.com/Jeferson-Peter/scify-file-reader
 Author: Jeferson-Peter (Jeferson Peter)
 Author-email: jeferson.peter@pm.me
 Keywords: Python,File Reading,Multiple File Handler
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `scify-file-reader-0.0.1/setup.py` & `scify-file-reader-0.0.2/setup.py`

 * *Files identical despite different names*

