# Comparing `tmp/lib-dzne-auto-interface-0.2.3.tar.gz` & `tmp/lib-dzne-auto-interface-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-auto-interface-0.2.3.tar", last modified: Sun Jun 11 16:27:00 2023, max compression
+gzip compressed data, was "lib-dzne-auto-interface-0.3.0.tar", last modified: Sun Jun 18 15:26:25 2023, max compression
```

## Comparing `lib-dzne-auto-interface-0.2.3.tar` & `lib-dzne-auto-interface-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.3/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.2.3/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      547 2023-06-11 16:25:51.000000 lib-dzne-auto-interface-0.2.3/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface/
--rw-r--r--   0 base      (1001) base      (1001)    10524 2023-06-11 09:31:19.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-11 16:27:00.001679 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      286 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       24 2023-06-11 16:26:59.000000 lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.3.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.3.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      553 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/
+-rw-r--r--   0 base      (1001) base      (1001)     2297 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/Information.py
+-rw-rw-r--   0 base      (1001) base      (1001)    15234 2023-06-18 10:18:44.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/
+-rw-r--r--   0 base      (1001) base      (1001)      886 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/HelpButton.py
+-rw-r--r--   0 base      (1001) base      (1001)      654 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/Stack.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/
+-rw-r--r--   0 base      (1001) base      (1001)     7764 2023-06-18 15:26:20.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     2265 2023-06-17 21:16:13.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface/gui/inputs/_parsing_nargs.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-18 15:26:25.183829 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      524 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       24 2023-06-18 15:26:25.000000 lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/top_level.txt
```

### Comparing `lib-dzne-auto-interface-0.2.3/LICENSE` & `lib-dzne-auto-interface-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.2.3/PKG-INFO` & `lib-dzne-auto-interface-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.3
+Version: 0.3.0
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-auto-interface-0.2.3/pyproject.toml` & `lib-dzne-auto-interface-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-auto-interface"
-version = "0.2.3"
+version = "0.3.0"
 description = "Libary for automatically created interfaces. "
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
-dependencies = []
+dependencies = [
+    
+]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-auto-interface-0.2.3/src/lib_dzne_auto_interface.egg-info/PKG-INFO` & `lib-dzne-auto-interface-0.3.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.3
+Version: 0.3.0
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

