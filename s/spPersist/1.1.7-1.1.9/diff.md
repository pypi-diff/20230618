# Comparing `tmp/sppersist-1.1.7.tar.gz` & `tmp/sppersist-1.1.9.tar.gz`

## Comparing `sppersist-1.1.7.tar` & `sppersist-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/ph.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.7/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.7/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.9/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.9/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.9/PKG-INFO
```

### Comparing `sppersist-1.1.7/src/spPersist/DTM_filtrations.py` & `sppersist-1.1.9/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/src/spPersist/dp.py` & `sppersist-1.1.9/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/src/spPersist/hc.py` & `sppersist-1.1.9/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/src/spPersist/persistence_statistics.py` & `sppersist-1.1.9/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/src/spPersist/ph.py` & `sppersist-1.1.9/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/src/spPersist/pp.py` & `sppersist-1.1.9/src/spPersist/pp.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,26 +166,26 @@
   data ref as a pandas dataframe, and performs deconvolution 
   methods as demonstrated in the cell2location tutorial with 
   human lymph node. It returns the spatially resolved 
   annotated data.
   '''
 
   adata = ad.copy()
+  cell2location.models.Cell2location.setup_anndata(adata=adata)
 
   # create and train the model
   mod = cell2location.models.Cell2location(
       adata, cell_state_df=ref, 
       # the expected average cell abundance: tissue-dependent 
       # hyper-prior which can be estimated from paired histology:
       N_cells_per_location=30,
       # hyperparameter controlling normalisation of
       # within-experiment variation in RNA detection:
       detection_alpha=20
   ) 
-  mod.view_anndata_setup()
 
   mod.train(max_epochs=30000, 
             # train using full data (batch_size=None)
             batch_size=None, 
             # use all data points in training because 
             # we need to estimate cell abundance at all locations
             train_size=1,
```

### Comparing `sppersist-1.1.7/LICENSE` & `sppersist-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/README.md` & `sppersist-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.7/pyproject.toml` & `sppersist-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.1.7"
+version = "1.1.9"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.1.7/PKG-INFO` & `sppersist-1.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.1.7
+Version: 1.1.9
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

