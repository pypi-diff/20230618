# Comparing `tmp/mrfix-1.0.6.tar.gz` & `tmp/mrfix-2.0.3.tar.gz`

## Comparing `mrfix-1.0.6.tar` & `mrfix-2.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-1.0.6/LICENZE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-1.0.6/src/mrfix/__init__.py
--rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 mrfix-1.0.6/src/mrfix/mrfix.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-1.0.6/.gitignore
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 mrfix-1.0.6/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    10352 2020-02-02 00:00:00.000000 mrfix-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 mrfix-2.0.3/LICENZE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mrfix-2.0.3/src/mrfix/__init__.py
+-rw-r--r--   0        0        0    28450 2020-02-02 00:00:00.000000 mrfix-2.0.3/src/mrfix/mrfix.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 mrfix-2.0.3/.gitignore
+-rw-r--r--   0        0        0    75915 2020-02-02 00:00:00.000000 mrfix-2.0.3/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 mrfix-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    76423 2020-02-02 00:00:00.000000 mrfix-2.0.3/PKG-INFO
```

### Comparing `mrfix-1.0.6/LICENZE` & `mrfix-2.0.3/LICENZE`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.6/.gitignore` & `mrfix-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mrfix-1.0.6/pyproject.toml` & `mrfix-2.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system] 
 requires = ["hatchling"] 
 build-backend = "hatchling.build"
 
 [project] 
 name = "mrfix"
-version = "1.0.6"
+version = "2.0.3"
 authors = [   
   { name="Valerii Zhuravlev", email="valerzhurav2011@gmail.com" },
 ] 
 description = "A package with a set of decorator-methods for automatic testing of the user interface using Python + Selenium"
 readme = "README.md" 
 requires-python = ">=3.9"
 classifiers = [
```

