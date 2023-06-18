# Comparing `tmp/CToolKit-1.1.tar.gz` & `tmp/CToolKit-1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CToolKit-1.1.tar", last modified: Sun Jun 18 21:34:02 2023, max compression
+gzip compressed data, was "CToolKit-1.11.tar", last modified: Sun Jun 18 21:36:13 2023, max compression
```

## Comparing `CToolKit-1.1.tar` & `CToolKit-1.11.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:34:02.252960 CToolKit-1.1/
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:34:02.244960 CToolKit-1.1/CToolKit/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-06-18 19:59:56.000000 CToolKit-1.1/CToolKit/ComandLineExecution.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:34:02.252960 CToolKit-1.1/CToolKit/Errors/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-06-17 06:47:02.000000 CToolKit-1.1/CToolKit/Errors/ComandLineError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-06-17 06:58:51.000000 CToolKit-1.1/CToolKit/Errors/ComandLineWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-06-17 06:48:41.000000 CToolKit-1.1/CToolKit/Errors/CopilationError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-06-17 06:49:33.000000 CToolKit-1.1/CToolKit/Errors/CopilationWarning.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-06-17 06:47:14.000000 CToolKit-1.1/CToolKit/Errors/ExecutionError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      116 2023-06-17 06:57:42.000000 CToolKit-1.1/CToolKit/Errors/ValgrindError.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      115 2023-06-17 07:04:59.000000 CToolKit-1.1/CToolKit/Errors/ValgrindLeak.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-06-17 04:59:48.000000 CToolKit-1.1/CToolKit/Errors/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      811 2023-06-18 18:20:38.000000 CToolKit-1.1/CToolKit/__init__.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1459 2023-06-18 20:23:25.000000 CToolKit-1.1/CToolKit/amalgamation.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     4637 2023-06-18 19:58:16.000000 CToolKit-1.1/CToolKit/comand_line_functions.py
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2967 2023-06-18 20:01:08.000000 CToolKit-1.1/CToolKit/readme_converter.py
-drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:34:02.248960 CToolKit-1.1/CToolKit.egg-info/
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3274 2023-06-18 21:34:02.000000 CToolKit-1.1/CToolKit.egg-info/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      566 2023-06-18 21:34:02.000000 CToolKit-1.1/CToolKit.egg-info/SOURCES.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-06-18 21:34:02.000000 CToolKit-1.1/CToolKit.egg-info/dependency_links.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-06-18 21:34:02.000000 CToolKit-1.1/CToolKit.egg-info/top_level.txt
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.1/LICENSE
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3274 2023-06-18 21:34:02.252960 CToolKit-1.1/PKG-INFO
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2866 2023-06-18 21:03:52.000000 CToolKit-1.1/README.md
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-06-18 21:34:02.252960 CToolKit-1.1/setup.cfg
--rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      663 2023-06-18 21:33:24.000000 CToolKit-1.1/setup.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.485931 CToolKit-1.11/
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.457931 CToolKit-1.11/CToolKit/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      504 2023-06-18 19:59:56.000000 CToolKit-1.11/CToolKit/ComandLineExecution.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.485931 CToolKit-1.11/CToolKit/Errors/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      306 2023-06-17 06:47:02.000000 CToolKit-1.11/CToolKit/Errors/ComandLineError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      226 2023-06-17 06:58:51.000000 CToolKit-1.11/CToolKit/Errors/ComandLineWarning.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      110 2023-06-17 06:48:41.000000 CToolKit-1.11/CToolKit/Errors/CopilationError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      118 2023-06-17 06:49:33.000000 CToolKit-1.11/CToolKit/Errors/CopilationWarning.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      108 2023-06-17 06:47:14.000000 CToolKit-1.11/CToolKit/Errors/ExecutionError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      116 2023-06-17 06:57:42.000000 CToolKit-1.11/CToolKit/Errors/ValgrindError.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      115 2023-06-17 07:04:59.000000 CToolKit-1.11/CToolKit/Errors/ValgrindLeak.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        0 2023-06-17 04:59:48.000000 CToolKit-1.11/CToolKit/Errors/__init__.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      811 2023-06-18 18:20:38.000000 CToolKit-1.11/CToolKit/__init__.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1459 2023-06-18 20:23:25.000000 CToolKit-1.11/CToolKit/amalgamation.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     4637 2023-06-18 19:58:16.000000 CToolKit-1.11/CToolKit/comand_line_functions.py
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2967 2023-06-18 20:01:08.000000 CToolKit-1.11/CToolKit/readme_converter.py
+drwxrwxr-x   0 jurandi   (1000) jurandi   (1000)        0 2023-06-18 21:36:13.465931 CToolKit-1.11/CToolKit.egg-info/
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3370 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/PKG-INFO
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      566 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        1 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)        9 2023-06-18 21:36:13.000000 CToolKit-1.11/CToolKit.egg-info/top_level.txt
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     1060 2023-06-17 02:11:11.000000 CToolKit-1.11/LICENSE
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     3370 2023-06-18 21:36:13.485931 CToolKit-1.11/PKG-INFO
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)     2961 2023-06-18 21:35:32.000000 CToolKit-1.11/README.md
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)       38 2023-06-18 21:36:13.485931 CToolKit-1.11/setup.cfg
+-rw-rw-r--   0 jurandi   (1000) jurandi   (1000)      664 2023-06-18 21:36:08.000000 CToolKit-1.11/setup.py
```

### Comparing `CToolKit-1.1/CToolKit/__init__.py` & `CToolKit-1.11/CToolKit/__init__.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.1/CToolKit/amalgamation.py` & `CToolKit-1.11/CToolKit/amalgamation.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.1/CToolKit/comand_line_functions.py` & `CToolKit-1.11/CToolKit/comand_line_functions.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.1/CToolKit/readme_converter.py` & `CToolKit-1.11/CToolKit/readme_converter.py`

 * *Files identical despite different names*

### Comparing `CToolKit-1.1/CToolKit.egg-info/PKG-INFO` & `CToolKit-1.11/CToolKit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.1
+Version: 1.11
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 License-File: LICENSE
 
 # CToolkit
  is An Python Package to manipulate C/C++ buildings and  PipeLines
  providing easy automation tools to increase your code pipelines 
  with amalgamations, black box testing, and readme replacment
 
+### Instalation from Pip
+for install the lib from pip call 
+
+~~~shell
+pip install CToolKit
+~~~
 ### Installation from scratch
 
 clone the repo into your machine with:
 
 ~~~shell
 git clone https://github.com/OUIsolutions/CTolkitBuild.git
 ~~~
```

### Comparing `CToolKit-1.1/CToolKit.egg-info/SOURCES.txt` & `CToolKit-1.11/CToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CToolKit-1.1/LICENSE` & `CToolKit-1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `CToolKit-1.1/PKG-INFO` & `CToolKit-1.11/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CToolKit
-Version: 1.1
+Version: 1.11
 Summary: CToolKit to manipulate CPipeLines and Repos
 Home-page: https://oui.tec.br/
 Author: Mateus Moutinho
 Author-email: mateusmoutinho01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,20 @@
 License-File: LICENSE
 
 # CToolkit
  is An Python Package to manipulate C/C++ buildings and  PipeLines
  providing easy automation tools to increase your code pipelines 
  with amalgamations, black box testing, and readme replacment
 
+### Instalation from Pip
+for install the lib from pip call 
+
+~~~shell
+pip install CToolKit
+~~~
 ### Installation from scratch
 
 clone the repo into your machine with:
 
 ~~~shell
 git clone https://github.com/OUIsolutions/CTolkitBuild.git
 ~~~
```

### Comparing `CToolKit-1.1/README.md` & `CToolKit-1.11/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # CToolkit
  is An Python Package to manipulate C/C++ buildings and  PipeLines
  providing easy automation tools to increase your code pipelines 
  with amalgamations, black box testing, and readme replacment
 
+### Instalation from Pip
+for install the lib from pip call 
+
+~~~shell
+pip install CToolKit
+~~~
 ### Installation from scratch
 
 clone the repo into your machine with:
 
 ~~~shell
 git clone https://github.com/OUIsolutions/CTolkitBuild.git
 ~~~
```

### Comparing `CToolKit-1.1/setup.py` & `CToolKit-1.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='CToolKit',
-    version='1.1',
+    version='1.11',
     description='CToolKit to manipulate CPipeLines and Repos',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mateus Moutinho',
     author_email='mateusmoutinho01@gmail.com',
     url='https://oui.tec.br/',
     packages=find_packages(),
```

