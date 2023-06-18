# Comparing `tmp/sppersist-1.2.1.tar.gz` & `tmp/sppersist-1.2.2.tar.gz`

## Comparing `sppersist-1.2.1.tar` & `sppersist-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/ph.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 sppersist-1.2.1/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.1/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.1/README.md
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 sppersist-1.2.2/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.2.2/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.2.2/README.md
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 sppersist-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 sppersist-1.2.2/PKG-INFO
```

### Comparing `sppersist-1.2.1/src/spPersist/DTM_filtrations.py` & `sppersist-1.2.2/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/src/spPersist/dp.py` & `sppersist-1.2.2/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/src/spPersist/hc.py` & `sppersist-1.2.2/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/src/spPersist/persistence_statistics.py` & `sppersist-1.2.2/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/src/spPersist/ph.py` & `sppersist-1.2.2/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/src/spPersist/pp.py` & `sppersist-1.2.2/src/spPersist/pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,15 @@
 def extract_mouse_brain_reference():
   '''
   extract_mouse_brain_reference returns the median gene expression by
   cluster, as a pandas dataframe, from the Yao Z et al.
   '''
 
   url = 'https://idk-etl-prod-download-bucket.s3.amazonaws.com/aibs_mouse_ctx-hpf_10x/medians.csv'
-  filename = 'medians.csv'
-  os.system('wget '+url)
-  df = pd.read_csv(filename,index_col='feature')
+  df = pd.read_csv(url,index_col='feature')
 
   return df
 
 
 def extract_reference_data(adata_ref):
   '''
   extract_reference_data takes a single-cell reference data adata_ref
```

### Comparing `sppersist-1.2.1/LICENSE` & `sppersist-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/README.md` & `sppersist-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.2.1/pyproject.toml` & `sppersist-1.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.2.1/PKG-INFO` & `sppersist-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.2.1
+Version: 1.2.2
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

