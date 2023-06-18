# Comparing `tmp/pdf-docx-pic-3.1.1.tar.gz` & `tmp/pdf-docx-pic-3.1.1.2023.6.18.14.43.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-3.1.1.tar", last modified: Sun Jun 18 03:11:01 2023, max compression
+gzip compressed data, was "pdf-docx-pic-3.1.1.2023.6.18.14.43.46.tar", last modified: Sun Jun 18 06:44:17 2023, max compression
```

## Comparing `pdf-docx-pic-3.1.1.tar` & `pdf-docx-pic-3.1.1.2023.6.18.14.43.46.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 03:11:01.649367 pdf-docx-pic-3.1.1/
--rw-rw-rw-   0        0        0      841 2023-06-18 03:11:01.649367 pdf-docx-pic-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-06-18 03:10:40.000000 pdf-docx-pic-3.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 03:11:01.649367 pdf-docx-pic-3.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 03:11:01.643219 pdf-docx-pic-3.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 03:11:01.643219 pdf-docx-pic-3.1.1/src/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1/src/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1/src/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:11:01.649367 pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0      841 2023-06-18 03:11:01.000000 pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-18 03:11:01.000000 pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 03:11:01.000000 pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-18 03:11:01.000000 pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-18 03:11:01.000000 pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/
+-rw-rw-rw-   0        0        0      860 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-06-18 06:43:53.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.541058 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.541058 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0      860 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/top_level.txt
```

### Comparing `pdf-docx-pic-3.1.1/PKG-INFO` & `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.1
+Version: 3.1.1.2023.6.18.14.43.46
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
```

### Comparing `pdf-docx-pic-3.1.1/pyproject.toml` & `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "pdf-docx-pic"
-version = "3.1.1"
+version = "3.1.1.2023.6.18.14.43.46"
 requires-python = ">=2.6"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Django :: 4.2",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)",
     "Operating System :: MacOS :: MacOS X",
```

### Comparing `pdf-docx-pic-3.1.1/src/pdf-docx-pic/main.py` & `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf-docx-pic-3.1.1/src/pdf_docx_pic.egg-info/PKG-INFO` & `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.1
+Version: 3.1.1.2023.6.18.14.43.46
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
```

