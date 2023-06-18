# Comparing `tmp/pdf-docx-pic-3.1.1.2023.6.18.17.33.46.tar.gz` & `tmp/pdf-docx-pic-3.1.1.2023.6.18.17.53.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-3.1.1.2023.6.18.17.33.46.tar", last modified: Sun Jun 18 09:36:29 2023, max compression
+gzip compressed data, was "pdf-docx-pic-3.1.1.2023.6.18.17.53.22.tar", last modified: Sun Jun 18 09:53:51 2023, max compression
```

## Comparing `pdf-docx-pic-3.1.1.2023.6.18.17.33.46.tar` & `pdf-docx-pic-3.1.1.2023.6.18.17.53.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/
--rw-rw-rw-   0        0        0     1300 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/PKG-INFO
--rw-rw-rw-   0        0        0     1463 2023-06-18 09:36:04.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.108216 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.123841 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0     1300 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 09:53:51.080583 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/
+-rw-rw-rw-   0        0        0     1354 2023-06-18 09:53:51.080583 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/PKG-INFO
+-rw-rw-rw-   0        0        0     1512 2023-06-18 09:53:32.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 09:53:51.080583 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 09:53:51.057622 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 09:53:51.057622 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:53:51.080583 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1354 2023-06-18 09:53:51.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-18 09:53:51.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 09:53:51.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-18 09:53:51.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 09:53:51.000000 pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/top_level.txt
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/PKG-INFO` & `pdf-docx-pic-3.1.1.2023.6.18.17.53.22/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.1.2023.6.18.17.33.46
+Version: 3.1.1.2023.6.18.17.53.22
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 7
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
+Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/pyproject.toml` & `pdf-docx-pic-3.1.1.2023.6.18.17.53.22/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "pdf-docx-pic"
-version = "3.1.1.2023.6.18.17.33.46"
+version = "3.1.1.2023.6.18.17.53.22"
 requires-python = ">=2.6"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: GPU",
     "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Django :: 4.2",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
@@ -15,14 +15,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows :: Windows 7",
     "Operating System :: Microsoft :: Windows :: Windows 8",
     "Operating System :: Microsoft :: Windows :: Windows 8.1",
     "Operating System :: Microsoft :: Windows :: Windows 10",
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Operating System :: POSIX",
+    "Natural Language :: Chinese (Simplified)",
     "Programming Language :: Python :: 2.6",
     "Programming Language :: Python :: 2.7",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/main.py` & `pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/PKG-INFO` & `pdf-docx-pic-3.1.1.2023.6.18.17.53.22/src/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.1.2023.6.18.17.33.46
+Version: 3.1.1.2023.6.18.17.53.22
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU
 Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 7
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
+Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

