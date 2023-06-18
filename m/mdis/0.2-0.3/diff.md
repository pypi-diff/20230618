# Comparing `tmp/mdis-0.2.tar.gz` & `tmp/mdis-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-7z_xmyvn/mdis-0.2.tar", last modified: Fri Jun 16 20:12:32 2023, max compression
+gzip compressed data, was "/home/ghostmansd/mdis/dist/.tmp-8cr_ulv3/mdis-0.3.tar", last modified: Sun Jun 18 11:21:15 2023, max compression
```

## Comparing `mdis-0.2.tar` & `mdis-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.2/LICENSE
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4456 2023-06-16 20:12:32.000000 mdis-0.2/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3642 2023-06-14 10:36:25.000000 mdis-0.2/README.md
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      928 2023-06-16 20:05:13.000000 mdis-0.2/pyproject.toml
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-16 20:12:32.000000 mdis-0.2/setup.cfg
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/src/
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      328 2023-06-16 20:05:17.000000 mdis-0.2/src/mdis/__init__.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2430 2023-06-14 10:35:12.000000 mdis-0.2/src/mdis/dispatcher.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      322 2023-06-14 10:34:25.000000 mdis-0.2/src/mdis/visitor.py
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      624 2023-06-14 10:29:43.000000 mdis-0.2/src/mdis/walker.py
-drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4456 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/PKG-INFO
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/SOURCES.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/dependency_links.txt
--rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-16 20:12:32.000000 mdis-0.2/src/mdis.egg-info/top_level.txt
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     1272 2023-06-13 22:23:19.000000 mdis-0.3/LICENSE
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 11:21:15.000000 mdis-0.3/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     3649 2023-06-16 20:42:33.000000 mdis-0.3/README.md
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      938 2023-06-18 11:20:46.000000 mdis-0.3/pyproject.toml
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)       38 2023-06-18 11:21:15.000000 mdis-0.3/setup.cfg
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/src/
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      328 2023-06-18 11:20:50.000000 mdis-0.3/src/mdis/__init__.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     2430 2023-06-14 10:35:12.000000 mdis-0.3/src/mdis/dispatcher.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      477 2023-06-16 20:42:11.000000 mdis-0.3/src/mdis/visitor.py
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      624 2023-06-14 10:29:43.000000 mdis-0.3/src/mdis/walker.py
+drwxr-xr-x   0 ghostmansd  (1000) ghostmansd  (1000)        0 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)     4473 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/PKG-INFO
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)      243 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/SOURCES.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        1 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/dependency_links.txt
+-rw-r--r--   0 ghostmansd  (1000) ghostmansd  (1000)        5 2023-06-18 11:21:15.000000 mdis-0.3/src/mdis.egg-info/top_level.txt
```

### Comparing `mdis-0.2/LICENSE` & `mdis-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdis-0.2/PKG-INFO` & `mdis-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.2
+Version: 0.3
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
-Project-URL: Homepage, https://repo.or.cz/mdis.git
-Project-URL: Bug Tracker, https://repo.or.cz/mdis.git
+Project-URL: Homepage, https://git.libre-soc.org/?p=mdis.git
+Project-URL: Bug Tracker, https://bugs.libre-soc.org/
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -73,15 +73,15 @@
 The example below shows how to execute some arbitrary code upon visiting an object.
 
     import contextlib
 
     import mdis.dispatcher
     import mdis.visitor
 
-    class CustomVisitor(mdis.visitor.Visitor):
+    class CustomVisitor(mdis.visitor.ContextVisitor):
         @mdis.dispatcher.hook(int)
         @contextlib.contextmanager
         def dispatch_int(self, instance):
             print("entering int")
             yield (instance + 42)
             print("leaving int")
```

### Comparing `mdis-0.2/README.md` & `mdis-0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 The example below shows how to execute some arbitrary code upon visiting an object.
 
     import contextlib
 
     import mdis.dispatcher
     import mdis.visitor
 
-    class CustomVisitor(mdis.visitor.Visitor):
+    class CustomVisitor(mdis.visitor.ContextVisitor):
         @mdis.dispatcher.hook(int)
         @contextlib.contextmanager
         def dispatch_int(self, instance):
             print("entering int")
             yield (instance + 42)
             print("leaving int")
```

### Comparing `mdis-0.2/pyproject.toml` & `mdis-0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=46.4.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdis"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="Dmitry Selyutin", email="ghostmansd@gmail.com" },
 ]
 keywords = [
     "dispatch",
     "dispather",
     "map",
@@ -28,9 +28,9 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://repo.or.cz/mdis.git"
-"Bug Tracker" = "https://repo.or.cz/mdis.git"
+"Homepage" = "https://git.libre-soc.org/?p=mdis.git"
+"Bug Tracker" = "https://bugs.libre-soc.org/"
```

### Comparing `mdis-0.2/src/mdis/dispatcher.py` & `mdis-0.3/src/mdis/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mdis-0.2/src/mdis/walker.py` & `mdis-0.3/src/mdis/walker.py`

 * *Files identical despite different names*

### Comparing `mdis-0.2/src/mdis.egg-info/PKG-INFO` & `mdis-0.3/src/mdis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mdis
-Version: 0.2
+Version: 0.3
 Summary: Python dispatching library
 Author-email: Dmitry Selyutin <ghostmansd@gmail.com>
-Project-URL: Homepage, https://repo.or.cz/mdis.git
-Project-URL: Bug Tracker, https://repo.or.cz/mdis.git
+Project-URL: Homepage, https://git.libre-soc.org/?p=mdis.git
+Project-URL: Bug Tracker, https://bugs.libre-soc.org/
 Keywords: dispatch,dispather,map,iterator,iterable,visitor,walker
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -73,15 +73,15 @@
 The example below shows how to execute some arbitrary code upon visiting an object.
 
     import contextlib
 
     import mdis.dispatcher
     import mdis.visitor
 
-    class CustomVisitor(mdis.visitor.Visitor):
+    class CustomVisitor(mdis.visitor.ContextVisitor):
         @mdis.dispatcher.hook(int)
         @contextlib.contextmanager
         def dispatch_int(self, instance):
             print("entering int")
             yield (instance + 42)
             print("leaving int")
```

