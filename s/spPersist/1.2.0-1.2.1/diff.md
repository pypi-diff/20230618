# Comparing `tmp/sppersist-1.2.0.tar.gz` & `tmp/sppersist-1.2.1.tar.gz`

## Comparing `sppersist-1.2.0.tar` & `sppersist-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/ph.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.0/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.0/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.1/README.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.1/PKG-INFO
```

### Comparing `sppersist-1.2.0/src/spPersist/DTM_filtrations.py` & `sppersist-1.2.1/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/src/spPersist/dp.py` & `sppersist-1.2.1/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/src/spPersist/hc.py` & `sppersist-1.2.1/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/src/spPersist/persistence_statistics.py` & `sppersist-1.2.1/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/src/spPersist/ph.py` & `sppersist-1.2.1/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/src/spPersist/pp.py` & `sppersist-1.2.1/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/LICENSE` & `sppersist-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/README.md` & `sppersist-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.0/pyproject.toml` & `sppersist-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,8 +18,9 @@
 ]
 
 dependencies = [
   "gudhi",
   "scanpy",
   "cell2location",
   "gcsfs",
+  "leidenalg",
 ]
```

### Comparing `sppersist-1.2.0/PKG-INFO` & `sppersist-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.2.0
+Version: 1.2.1
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: cell2location
 Requires-Dist: gcsfs
 Requires-Dist: gudhi
+Requires-Dist: leidenalg
 Requires-Dist: scanpy
 Description-Content-Type: text/markdown
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
```

