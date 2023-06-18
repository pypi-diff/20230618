# Comparing `tmp/sppersist-1.1.9.tar.gz` & `tmp/sppersist-1.2.0.tar.gz`

## Comparing `sppersist-1.1.9.tar` & `sppersist-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/ph.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 sppersist-1.1.9/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.9/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.9/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 sppersist-1.2.0/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.0/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.2.0/PKG-INFO
```

### Comparing `sppersist-1.1.9/src/spPersist/DTM_filtrations.py` & `sppersist-1.2.0/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/src/spPersist/dp.py` & `sppersist-1.2.0/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/src/spPersist/hc.py` & `sppersist-1.2.0/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/src/spPersist/persistence_statistics.py` & `sppersist-1.2.0/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/src/spPersist/ph.py` & `sppersist-1.2.0/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/src/spPersist/pp.py` & `sppersist-1.2.0/src/spPersist/pp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import cell2location
 import scanpy as sc
+import pandas as pd
+import os
 
 def quality_control_metrics(adata):
   '''
   quality_control_metrics takes an annotated data object adata
   produced in the data processing module and performs 
   quality control calculation as recommended in Scanpy
   preprocessing tutorials.
@@ -122,14 +124,27 @@
     print('Empty entry or the parameter is invalid.')
   else:
     p = int(p)
     adata = adata[adata.obs["pct_counts_mt"] < p]
     print(f"#cells after MT filter: {adata.n_obs}")
 
 
+def extract_mouse_brain_reference():
+  '''
+  extract_mouse_brain_reference returns the median gene expression by
+  cluster, as a pandas dataframe, from the Yao Z et al.
+  '''
+
+  url = 'https://idk-etl-prod-download-bucket.s3.amazonaws.com/aibs_mouse_ctx-hpf_10x/medians.csv'
+  filename = 'medians.csv'
+  os.system('wget '+url)
+  df = pd.read_csv(filename,index_col='feature')
+
+  return df
+
 
 def extract_reference_data(adata_ref):
   '''
   extract_reference_data takes a single-cell reference data adata_ref
   as annotated data object, and returns the estimated reference expression
   as a pandas dataframe.
   '''
@@ -155,25 +170,24 @@
                                       for i in adata_ref.uns['mod']['factor_names']]].copy()
   inf_aver.columns = adata_ref.uns['mod']['factor_names']
   inf_aver.iloc[0:5, 0:5]
 
   return inf_aver
 
 
-def deconvolute(ad, ref):
+def deconvolute(adata, ref):
   '''
-  deconvolute takes an annotated data object ad produced
+  deconvolute takes an annotated data object adata produced
   in the data processing module and a single-cell reference 
   data ref as a pandas dataframe, and performs deconvolution 
   methods as demonstrated in the cell2location tutorial with 
-  human lymph node. It returns the spatially resolved 
-  annotated data.
+  human lymph node. The cell abundance is stored in obsm and
+  the deconvolution model is stored in uns['mod']. 
   '''
 
-  adata = ad.copy()
   cell2location.models.Cell2location.setup_anndata(adata=adata)
 
   # create and train the model
   mod = cell2location.models.Cell2location(
       adata, cell_state_df=ref, 
       # the expected average cell abundance: tissue-dependent 
       # hyper-prior which can be estimated from paired histology:
@@ -202,16 +216,14 @@
       mod.samples["post_sample_q05"], mod.adata_manager
   )
 
   # Add to anndata layers
   for i, n in enumerate(mod.factor_names_):
       adata.layers[n] = expected_dict['mu'][i]
 
-  return adata
-
 
 def cell_type_identification(adata):
   '''
   cell_type_identification takes an annotated data object adata, and
   identifies cell types in adata via KNN and Leiden clustering, as 
   recommended in the cell2location tutorial.
   '''
```

### Comparing `sppersist-1.1.9/LICENSE` & `sppersist-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/README.md` & `sppersist-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.9/pyproject.toml` & `sppersist-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.1.9/PKG-INFO` & `sppersist-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.1.9
+Version: 1.2.0
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

