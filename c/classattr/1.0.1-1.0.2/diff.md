# Comparing `tmp/classattr-1.0.1.tar.gz` & `tmp/classattr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classattr-1.0.1.tar", last modified: Sun Jun 18 15:17:06 2023, max compression
+gzip compressed data, was "classattr-1.0.2.tar", last modified: Sun Jun 18 17:25:46 2023, max compression
```

## Comparing `classattr-1.0.1.tar` & `classattr-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 15:17:06.807811 classattr-1.0.1/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.1/LICENSE
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1221 2023-06-18 15:17:06.807811 classattr-1.0.1/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1010 2023-06-18 07:21:25.000000 classattr-1.0.1/README.md
-drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 15:17:06.807811 classattr-1.0.1/classattr.egg-info/
--rw-rw-r--   0 thierry   (1000) thierry   (1000)     1221 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/PKG-INFO
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/SOURCES.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/dependency_links.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 15:17:06.000000 classattr-1.0.1/classattr.egg-info/top_level.txt
--rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 15:17:06.807811 classattr-1.0.1/setup.cfg
--rw-rw-r--   0 thierry   (1000) thierry   (1000)      490 2023-06-18 15:16:55.000000 classattr-1.0.1/setup.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 17:25:46.885137 classattr-1.0.2/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1075 2023-05-20 07:22:28.000000 classattr-1.0.2/LICENSE
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1460 2023-06-18 17:25:46.885137 classattr-1.0.2/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1050 2023-06-18 15:26:45.000000 classattr-1.0.2/README.md
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-06-18 17:25:46.885137 classattr-1.0.2/classattr.egg-info/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1460 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      158 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-06-18 17:25:46.000000 classattr-1.0.2/classattr.egg-info/top_level.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-06-18 17:25:46.885137 classattr-1.0.2/setup.cfg
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)      539 2023-06-18 17:18:31.000000 classattr-1.0.2/setup.py
```

### Comparing `classattr-1.0.1/LICENSE` & `classattr-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `classattr-1.0.1/PKG-INFO` & `classattr-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1
-Name: classattr
-Version: 1.0.1
-Summary: classattr provides tools to manage class and object attributes
-Home-page: https://framagit.org/makeforartandscience/classattr
-Author: Thierry Dassé
-License: MIT License
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-License-File: LICENSE
+# ClassAttr package
 
+This package provides tools to manage objects attributes.
 
+It can be usefull to deal with default value attributes.
+
+# Installation
+
+> pip install classattr
+
+
+## Example
+
+```
 from classattr import ClassAttr, RAISE, FORCE
 
 class Point(ClassAttr):
 
     ## class atribute, can be default value
     x = 0
     y = 0
@@ -50,10 +51,9 @@
 print('x = {}, y = {}, r = {}'.format(d.x,d.y,d.radius))
 
 d.set(radius=1.5)
 d.color = 'blue'
 print(d.get())
 
 d.set(unknown_var = 53) # raise an error, if you want to create use mode=FORCE
-
-
+```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `classattr-1.0.1/README.md` & `classattr-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,32 @@
+Metadata-Version: 2.1
+Name: classattr
+Version: 1.0.2
+Summary: classattr provides tools to manage class and object attributes
+Home-page: https://framagit.org/makeforartandscience/classattr
+Author: Thierry Dassé
+License: MIT License
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ClassAttr package
 
 This package provides tools to manage objects attributes.
 
 It can be usefull to deal with default value attributes.
 
+# Installation
+
+> pip install classattr
+
 
-## Example:
+## Example
 
 ```
 from classattr import ClassAttr, RAISE, FORCE
 
 class Point(ClassAttr):
 
     ## class atribute, can be default value
@@ -49,7 +66,9 @@
 d.set(radius=1.5)
 d.color = 'blue'
 print(d.get())
 
 d.set(unknown_var = 53) # raise an error, if you want to create use mode=FORCE
 ```
 
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `classattr-1.0.1/classattr.egg-info/PKG-INFO` & `classattr-1.0.2/classattr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 Metadata-Version: 2.1
 Name: classattr
-Version: 1.0.1
+Version: 1.0.2
 Summary: classattr provides tools to manage class and object attributes
 Home-page: https://framagit.org/makeforartandscience/classattr
 Author: Thierry Dassé
 License: MIT License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# ClassAttr package
 
+This package provides tools to manage objects attributes.
+
+It can be usefull to deal with default value attributes.
+
+# Installation
+
+> pip install classattr
+
+
+## Example
+
+```
 from classattr import ClassAttr, RAISE, FORCE
 
 class Point(ClassAttr):
 
     ## class atribute, can be default value
     x = 0
     y = 0
@@ -50,10 +64,11 @@
 print('x = {}, y = {}, r = {}'.format(d.x,d.y,d.radius))
 
 d.set(radius=1.5)
 d.color = 'blue'
 print(d.get())
 
 d.set(unknown_var = 53) # raise an error, if you want to create use mode=FORCE
+```
```

