# Comparing `tmp/sppersist-1.2.2.tar.gz` & `tmp/sppersist-1.2.3.tar.gz`

## Comparing `sppersist-1.2.2.tar` & `sppersist-1.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/ph.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.2/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.2/README.md
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 sppersist-1.2.3/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.3/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.3/README.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.3/PKG-INFO
```

### Comparing `sppersist-1.2.2/src/spPersist/DTM_filtrations.py` & `sppersist-1.2.3/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/src/spPersist/dp.py` & `sppersist-1.2.3/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/src/spPersist/hc.py` & `sppersist-1.2.3/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/src/spPersist/persistence_statistics.py` & `sppersist-1.2.3/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/src/spPersist/ph.py` & `sppersist-1.2.3/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/src/spPersist/pp.py` & `sppersist-1.2.3/src/spPersist/pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,17 +168,17 @@
                                       for i in adata_ref.uns['mod']['factor_names']]].copy()
   inf_aver.columns = adata_ref.uns['mod']['factor_names']
   inf_aver.iloc[0:5, 0:5]
 
   return inf_aver
 
 
-def deconvolute(adata, ref):
+def cell_type_deconvolution(adata, ref):
   '''
-  deconvolute takes an annotated data object adata produced
+  cell_type_deconvolution takes an annotated data object adata produced
   in the data processing module and a single-cell reference 
   data ref as a pandas dataframe, and performs deconvolution 
   methods as demonstrated in the cell2location tutorial with 
   human lymph node. The cell abundance is stored in obsm and
   the deconvolution model is stored in uns['mod']. 
   '''
```

### Comparing `sppersist-1.2.2/LICENSE` & `sppersist-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/README.md` & `sppersist-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.2/pyproject.toml` & `sppersist-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.2.2/PKG-INFO` & `sppersist-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.2.2
+Version: 1.2.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

