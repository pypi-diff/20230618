# Comparing `tmp/featherplot-0.0.2.tar.gz` & `tmp/featherplot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featherplot-0.0.2.tar", last modified: Fri Jun 16 19:09:07 2023, max compression
+gzip compressed data, was "featherplot-0.0.3.tar", last modified: Sun Jun 18 13:49:00 2023, max compression
```

## Comparing `featherplot-0.0.2.tar` & `featherplot-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:09:07.774103 featherplot-0.0.2/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.2/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.2/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-16 19:09:07.773965 featherplot-0.0.2/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.2/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:09:07.772621 featherplot-0.0.2/featherplot/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    17256 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1574 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/commands.py
--rw-r--r--   0 solst      (501) staff       (20)      209 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.2/featherplot/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)     4366 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/deepscatter.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      241 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     6565 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/types.py
--rw-r--r--   0 solst      (501) staff       (20)    20001 2023-06-16 19:08:53.000000 featherplot-0.0.2/featherplot/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-16 19:09:07.773766 featherplot-0.0.2/featherplot.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      572 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)      115 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.2/featherplot.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-16 19:09:07.000000 featherplot-0.0.2/featherplot.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      870 2023-06-16 19:08:48.000000 featherplot-0.0.2/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-16 19:09:07.774144 featherplot-0.0.2/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.2/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 13:49:00.494004 featherplot-0.0.3/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.3/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.3/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-18 13:49:00.493862 featherplot-0.0.3/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.3/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 13:49:00.491311 featherplot-0.0.3/featherplot/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    17489 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1574 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)      209 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.3/featherplot/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)     4366 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/deepscatter.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      241 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     6565 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    20393 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 13:49:00.493658 featherplot-0.0.3/featherplot.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      572 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)      115 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.3/featherplot.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      870 2023-06-18 13:48:49.000000 featherplot-0.0.3/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-18 13:49:00.494045 featherplot-0.0.3/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.3/setup.py
```

### Comparing `featherplot-0.0.2/LICENSE` & `featherplot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/PKG-INFO` & `featherplot-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `featherplot-0.0.2/README.md` & `featherplot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/featherplot/_modidx.py` & `featherplot-0.0.3/featherplot/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
                                                                                     'featherplot/types.py'),
                                    'featherplot.types.MissingKwargsError': ('types.html#missingkwargserror', 'featherplot/types.py'),
                                    'featherplot.types.QuadFeatherColumnTypeGuard': ( 'types.html#quadfeathercolumntypeguard',
                                                                                      'featherplot/types.py'),
                                    'featherplot.types.TransformTypeGuard': ('types.html#transformtypeguard', 'featherplot/types.py'),
                                    'featherplot.types.TypeGuardError': ('types.html#typeguarderror', 'featherplot/types.py')},
             'featherplot.utils': { 'featherplot.utils.AnnDataProcessor': ('utils.html#anndataprocessor', 'featherplot/utils.py'),
+                                   'featherplot.utils.AnnDataProcessor.emb_name': ( 'utils.html#anndataprocessor.emb_name',
+                                                                                    'featherplot/utils.py'),
                                    'featherplot.utils.AnnDataProcessor.get_embedding': ( 'utils.html#anndataprocessor.get_embedding',
                                                                                          'featherplot/utils.py'),
                                    'featherplot.utils.AnnDataProcessor.get_sidecars': ( 'utils.html#anndataprocessor.get_sidecars',
                                                                                         'featherplot/utils.py'),
                                    'featherplot.utils.DataFrameToMetadata': ('utils.html#dataframetometadata', 'featherplot/utils.py'),
                                    'featherplot.utils.DataFrameToMetadata.__post_init__': ( 'utils.html#dataframetometadata.__post_init__',
                                                                                             'featherplot/utils.py'),
```

### Comparing `featherplot-0.0.2/featherplot/commands.py` & `featherplot-0.0.3/featherplot/commands.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/featherplot/deepscatter.py` & `featherplot-0.0.3/featherplot/deepscatter.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/featherplot/paths.py` & `featherplot-0.0.3/featherplot/paths.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/featherplot/types.py` & `featherplot-0.0.3/featherplot/types.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/featherplot/utils.py` & `featherplot-0.0.3/featherplot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,26 +580,40 @@
     adata: ad.AnnData
     x_emb: str = 'X_phate'
     layer: Optional[str] = None
     
 
     def get_sidecars(self):
         layer = self.adata.layers.get(self.layer, None)
+
+
         if layer is None:
             layer = self.adata.X
 
+        if hasattr(layer, 'toarray'):
+            layer = layer.toarray()
+
+        if hasattr(layer, 'todense'):
+            layer = layer.todense()
+
         df = pd.DataFrame(
             layer,
             columns=self.adata.var.index,
             index=self.adata.obs.index
         )
-
         return df
+    
+    @property
+    def emb_name(self):
+        return self.x_emb.replace('X_', '').upper()
 
-    def get_embedding(self):
-        df = self.adata.obsm.get(self.x_emb, None)        
-        # df_points = adata.obsm.get(EMB).rename({
-        #     'fake-SNE X': 'x','fake-SNE Y': 'y', 'fake-SNE Z': 'z'
-        # }, axis=1)
-        # df.loc[:, 'conditions'] = self.adata.obs.conditions
+    def get_embedding(self, add_conditions:bool=False):
+        emb = self.adata.obsm.get(self.x_emb, None)
+        cols = [f'{self.emb_name}_{i+1}' for i in range(emb.shape[1])]
+        df = pd.DataFrame(
+            emb, columns=cols, 
+            index=self.adata.obs.index
+        )
+        if add_conditions and 'conditions' in self.adata.obs.columns:        
+            df.loc[:, 'conditions'] = self.adata.obs.conditions        
         return df
```

### Comparing `featherplot-0.0.2/featherplot.egg-info/PKG-INFO` & `featherplot-0.0.3/featherplot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.2
+Version: 0.0.3
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `featherplot-0.0.2/featherplot.egg-info/SOURCES.txt` & `featherplot-0.0.3/featherplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.2/settings.ini` & `featherplot-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = featherplot-py
 lib_name = featherplot
-version = 0.0.2
+version = 0.0.3
 min_python = 3.10
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = featherplot
 nbs_path = nbs
 recursive = True
```

### Comparing `featherplot-0.0.2/setup.py` & `featherplot-0.0.3/setup.py`

 * *Files identical despite different names*

