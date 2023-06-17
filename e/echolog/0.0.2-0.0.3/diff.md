# Comparing `tmp/echolog-0.0.2.tar.gz` & `tmp/echolog-0.0.3.tar.gz`

## Comparing `echolog-0.0.2.tar` & `echolog-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 echolog-0.0.2/src/echolog/__init__.py
--rw-r--r--   0        0        0    11837 2020-02-02 00:00:00.000000 echolog-0.0.2/src/echolog/echolog.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 echolog-0.0.2/LICENSE
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 echolog-0.0.2/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 echolog-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5863 2020-02-02 00:00:00.000000 echolog-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 echolog-0.0.3/src/echolog/__init__.py
+-rw-r--r--   0        0        0    11837 2020-02-02 00:00:00.000000 echolog-0.0.3/src/echolog/echolog.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 echolog-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 echolog-0.0.3/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 echolog-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 echolog-0.0.3/PKG-INFO
```

### Comparing `echolog-0.0.2/src/echolog/echolog.py` & `echolog-0.0.3/src/echolog/echolog.py`

 * *Files identical despite different names*

### Comparing `echolog-0.0.2/LICENSE` & `echolog-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `echolog-0.0.2/README.md` & `echolog-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `echolog-0.0.2/pyproject.toml` & `echolog-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "echolog"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="nerdpersonthing" },
 ]
 description = "A logging package that adds an echo() function to return both the input expression/variable and its results. Also sets up nicely-formatted logging."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "os",
-  "re",
-  "inspect",
-  "logging",
   "datetime",
   "dotmap",
   "ansicon; os_name == 'nt'",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/nerdpersonthing/echolog"
```

### Comparing `echolog-0.0.2/PKG-INFO` & `echolog-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: echolog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A logging package that adds an echo() function to return both the input expression/variable and its results. Also sets up nicely-formatted logging.
 Project-URL: Homepage, https://github.com/nerdpersonthing/echolog
 Author: nerdpersonthing
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: ansicon; os_name == 'nt'
 Requires-Dist: datetime
 Requires-Dist: dotmap
-Requires-Dist: inspect
-Requires-Dist: logging
-Requires-Dist: os
-Requires-Dist: re
 Description-Content-Type: text/markdown
 
 # echolog
 A logging package that adds an "echo" function to return both the input expression/variable and its results. Also sets up nicely-formatted logging.
 
 ## Utilities
```

