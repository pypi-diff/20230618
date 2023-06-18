# Comparing `tmp/sengo-0.0.1.tar.gz` & `tmp/sengo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vanangamudi/agam/projects/code/tamilnlp/sengo/dist/.tmp-3eqqv770/sengo-0.0.1.tar", last modified: Sun Jun 18 19:21:39 2023, max compression
+gzip compressed data, was "/home/vanangamudi/agam/projects/code/tamilnlp/sengo/dist/.tmp-bd06hjsh/sengo-0.0.2.tar", last modified: Sun Jun 18 20:30:09 2023, max compression
```

## Comparing `sengo-0.0.1.tar` & `sengo-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.884815 sengo-0.0.1/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    35149 2023-06-18 18:51:40.000000 sengo-0.0.1/LICENSE
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    43082 2023-06-18 19:21:39.884815 sengo-0.0.1/PKG-INFO
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     2051 2023-06-18 18:51:40.000000 sengo-0.0.1/YENNAI_PADI.txt
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.628810 sengo-0.0.1/mlm/
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.628810 sengo-0.0.1/mlm/padalam/
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.628810 sengo-0.0.1/mlm/padalam/01/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      902 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/01/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.632810 sengo-0.0.1/mlm/padalam/02/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1094 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/02/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.632810 sengo-0.0.1/mlm/padalam/03/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     2704 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/03/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.648810 sengo-0.0.1/mlm/padalam/04/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     3980 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/04/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.660811 sengo-0.0.1/mlm/padalam/05/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     4141 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/05/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.700812 sengo-0.0.1/mlm/padalam/06/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5925 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/06/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.700812 sengo-0.0.1/mlm/padalam/07/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     6515 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/07/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.752813 sengo-0.0.1/mlm/padalam/08/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     6653 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/08/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.816814 sengo-0.0.1/mlm/padalam/09/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     7090 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/09/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.852815 sengo-0.0.1/mlm/padalam/10/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     7322 2023-06-18 18:51:40.000000 sengo-0.0.1/mlm/padalam/10/sengo.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.884815 sengo-0.0.1/mlm/sengo/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5920 2023-06-18 19:07:48.000000 sengo-0.0.1/mlm/sengo/sengo.py
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1450 2023-06-18 19:07:54.000000 sengo-0.0.1/mlm/sengo/vaayil.py
-drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 19:21:39.884815 sengo-0.0.1/mlm/sengo.egg-info/
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    43082 2023-06-18 19:21:39.000000 sengo-0.0.1/mlm/sengo.egg-info/PKG-INFO
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      449 2023-06-18 19:21:39.000000 sengo-0.0.1/mlm/sengo.egg-info/SOURCES.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)        1 2023-06-18 19:21:39.000000 sengo-0.0.1/mlm/sengo.egg-info/dependency_links.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       14 2023-06-18 19:21:39.000000 sengo-0.0.1/mlm/sengo.egg-info/top_level.txt
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      841 2023-06-18 19:21:08.000000 sengo-0.0.1/pyproject.toml
--rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       38 2023-06-18 19:21:39.884815 sengo-0.0.1/setup.cfg
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    35149 2023-06-18 18:51:40.000000 sengo-0.0.2/LICENSE
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    43082 2023-06-18 20:30:09.790579 sengo-0.0.2/PKG-INFO
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     2051 2023-06-18 18:51:40.000000 sengo-0.0.2/YENNAI_PADI.txt
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.786579 sengo-0.0.2/mlm/
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.786579 sengo-0.0.2/mlm/padalam/
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.786579 sengo-0.0.2/mlm/padalam/01/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      902 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/01/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/02/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1094 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/02/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/03/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     2704 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/03/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/04/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     3980 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/04/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/05/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     4141 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/05/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/06/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5925 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/06/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/07/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     6515 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/07/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/08/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     6653 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/08/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/09/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     7090 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/09/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/padalam/10/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     7322 2023-06-18 18:51:40.000000 sengo-0.0.2/mlm/padalam/10/sengo.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/sengo/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       21 2023-06-18 19:23:46.000000 sengo-0.0.2/mlm/sengo/__init__.py
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     5920 2023-06-18 19:07:48.000000 sengo-0.0.2/mlm/sengo/sengo.py
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)     1037 2023-06-18 20:21:39.000000 sengo-0.0.2/mlm/sengo/vaayil.py
+drwxrwxr-x   0 vanangamudi  (1000) vanangamudi  (1000)        0 2023-06-18 20:30:09.790579 sengo-0.0.2/mlm/sengo.egg-info/
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)    43082 2023-06-18 20:30:09.000000 sengo-0.0.2/mlm/sengo.egg-info/PKG-INFO
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      539 2023-06-18 20:30:09.000000 sengo-0.0.2/mlm/sengo.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)        1 2023-06-18 20:30:09.000000 sengo-0.0.2/mlm/sengo.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       46 2023-06-18 20:30:09.000000 sengo-0.0.2/mlm/sengo.egg-info/entry_points.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       18 2023-06-18 20:30:09.000000 sengo-0.0.2/mlm/sengo.egg-info/requires.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       14 2023-06-18 20:30:09.000000 sengo-0.0.2/mlm/sengo.egg-info/top_level.txt
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)      937 2023-06-18 20:29:55.000000 sengo-0.0.2/pyproject.toml
+-rw-rw-r--   0 vanangamudi  (1000) vanangamudi  (1000)       38 2023-06-18 20:30:09.790579 sengo-0.0.2/setup.cfg
```

### Comparing `sengo-0.0.1/LICENSE` & `sengo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/PKG-INFO` & `sengo-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sengo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sengo regular expression engine from scratch for Tamil Text
 Author-email: vanangamudi <selva.developer@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sengo-0.0.1/YENNAI_PADI.txt` & `sengo-0.0.2/YENNAI_PADI.txt`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/01/sengo.py` & `sengo-0.0.2/mlm/padalam/01/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/02/sengo.py` & `sengo-0.0.2/mlm/padalam/02/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/03/sengo.py` & `sengo-0.0.2/mlm/padalam/03/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/04/sengo.py` & `sengo-0.0.2/mlm/padalam/04/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/05/sengo.py` & `sengo-0.0.2/mlm/padalam/05/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/06/sengo.py` & `sengo-0.0.2/mlm/padalam/06/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/07/sengo.py` & `sengo-0.0.2/mlm/padalam/07/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/08/sengo.py` & `sengo-0.0.2/mlm/padalam/08/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/09/sengo.py` & `sengo-0.0.2/mlm/padalam/09/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/padalam/10/sengo.py` & `sengo-0.0.2/mlm/padalam/10/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/sengo/sengo.py` & `sengo-0.0.2/mlm/sengo/sengo.py`

 * *Files identical despite different names*

### Comparing `sengo-0.0.1/mlm/sengo.egg-info/PKG-INFO` & `sengo-0.0.2/mlm/sengo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sengo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sengo regular expression engine from scratch for Tamil Text
 Author-email: vanangamudi <selva.developer@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `sengo-0.0.1/pyproject.toml` & `sengo-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sengo"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="vanangamudi", email="selva.developer@gmail.com" },
 ]
 description = "Sengo regular expression engine from scratch for Tamil Text"
 readme = "YENNAI_PADI.txt"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "arichuvadi >= 0.0.4",
+]
+
+[project.scripts]
+sengo = "sengo.vaayil:vaayil"
+
 [project.urls]
 "Homepage" = "https://github.com/vanangamudi/sengo"
 "Bug Tracker" = "https://github.com/vanangamudi/sengo/issues"
 
 [tool.setuptools]
 #package-dir = {"" = "mlm"}
 include-package-data = true
```

