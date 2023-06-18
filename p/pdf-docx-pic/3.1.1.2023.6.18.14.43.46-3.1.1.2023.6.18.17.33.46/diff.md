# Comparing `tmp/pdf-docx-pic-3.1.1.2023.6.18.14.43.46.tar.gz` & `tmp/pdf-docx-pic-3.1.1.2023.6.18.17.33.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf-docx-pic-3.1.1.2023.6.18.14.43.46.tar", last modified: Sun Jun 18 06:44:17 2023, max compression
+gzip compressed data, was "pdf-docx-pic-3.1.1.2023.6.18.17.33.46.tar", last modified: Sun Jun 18 09:36:29 2023, max compression
```

## Comparing `pdf-docx-pic-3.1.1.2023.6.18.14.43.46.tar` & `pdf-docx-pic-3.1.1.2023.6.18.17.33.46.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/
--rw-rw-rw-   0        0        0      860 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-06-18 06:43:53.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.541058 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.541058 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/
--rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/__init__.py
--rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/main.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:44:17.556696 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/
--rw-rw-rw-   0        0        0      860 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-18 06:44:17.000000 pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/
+-rw-rw-rw-   0        0        0     1300 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/PKG-INFO
+-rw-rw-rw-   0        0        0     1463 2023-06-18 09:36:04.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.108216 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.123841 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/
+-rw-rw-rw-   0        0        0        0 2023-06-17 02:49:27.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/__init__.py
+-rw-rw-rw-   0        0        0     6432 2023-06-17 02:22:45.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/main.py
+drwxrwxrwx   0        0        0        0 2023-06-18 09:36:29.128905 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/
+-rw-rw-rw-   0        0        0     1300 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 09:36:29.000000 pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/top_level.txt
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/PKG-INFO` & `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.1.2023.6.18.14.43.46
+Version: 3.1.1.2023.6.18.17.33.46
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: GPU
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=2.6
```

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf-docx-pic/main.py` & `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf-docx-pic/main.py`

 * *Files identical despite different names*

### Comparing `pdf-docx-pic-3.1.1.2023.6.18.14.43.46/src/pdf_docx_pic.egg-info/PKG-INFO` & `pdf-docx-pic-3.1.1.2023.6.18.17.33.46/src/pdf_docx_pic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: pdf-docx-pic
-Version: 3.1.1.2023.6.18.14.43.46
+Version: 3.1.1.2023.6.18.17.33.46
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: GPU
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows :: Windows 7
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8
+Classifier: Operating System :: Microsoft :: Windows :: Windows 8.1
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=2.6
```

