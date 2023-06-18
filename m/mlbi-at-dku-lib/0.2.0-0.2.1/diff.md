# Comparing `tmp/mlbi_at_dku_lib-0.2.0.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.0.tar", last modified: Sun Jun 18 09:51:40 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.1.tar", last modified: Sun Jun 18 14:43:56 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.0.tar` & `mlbi_at_dku_lib-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.0/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.0/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.0/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36537 2023-06-18 09:51:04.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-18 09:51:32.000000 mlbi_at_dku_lib-0.2.0/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.0/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.528264 mlbi_at_dku_lib-0.2.1/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.1/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.1/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 14:43:56.528264 mlbi_at_dku_lib-0.2.1/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.1/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.508265 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36565 2023-06-18 14:40:16.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.520265 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-18 14:43:56.532264 mlbi_at_dku_lib-0.2.1/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-18 14:43:13.000000 mlbi_at_dku_lib-0.2.1/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.520265 mlbi_at_dku_lib-0.2.1/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.1/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.2.0/LICENSE` & `mlbi_at_dku_lib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.0/PKG-INFO` & `mlbi_at_dku_lib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/icnv.py`

 * *Files 1% similar despite different names*

```diff
@@ -788,15 +788,15 @@
     
     return cm[odr[0]]
 
 
 def compute_cnv_scores(adata, ref_ind, use_cnv_score = False,
                        cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                       cmd_cutoff = 0.01, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
+                       dec_margin = 0.05, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
                        plot_stat = False, use_cnv_cluster = True, use_ref = True, suffix = '', Data = None):
     
     score_key = score_key + suffix
     ## Get X_pca for ref_type cells
 
     X_pca = adata.obsm['X_cnv_pca']
     
@@ -884,20 +884,20 @@
     for c in cnv_clust_lst:
         b = adata.obs[cluster_key] == c
         adata.obs.loc[b, score_key] = adata.obs.loc[b, score_key].mean()
     '''
     if use_ref:
         df, params = get_cnv_threshold_useref( adata.obs, ref_ind, 
                                        score_key = score_key, cluster_key = cluster_key,
-                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = cmd_cutoff,
+                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
     else:
         df, params = get_cnv_threshold_bimodal( adata.obs, ref_ind, 
                                         score_key = score_key, cluster_key = cluster_key, 
-                                        th_min = th_min, refp_min = refp_min, ucr = cmd_cutoff,
+                                        th_min = th_min, refp_min = refp_min, ucr = dec_margin,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
     
     etime = round(time.time() - start_time) 
     print(' .. done (%i) ' % etime) #, end = '', flush = True)
     
     return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
                       'tumor_prob'+suffix, 'tumor_cluster'+ suffix]], params
@@ -997,15 +997,15 @@
         return cluster_label, km
     '''
 
 def detect_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
                        clust = None, Clustering_resolution = 1, N_clusters = 30,
                        # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                       cmd_cutoff = 0.01, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
+                       dec_margin = 0.05, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
                        plot_stat = False, use_cnv_cluster = True, use_ref = True, 
                        suffix = '', Data = None):
     
     score_key = 'tumor_score' + suffix
     cluster_key = 'cnv_cluster' 
     ## Get X_pca for ref_type cells
 
@@ -1020,15 +1020,15 @@
     
     N_components_pca = 15
     pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
 
     if not pca: 
         X_pca = pca_obj.fit_transform(X_cnv)
     else: 
-        X_pca = X_cnv #.copy(deep = True)
+        X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
     if clust:      
         y_clust = list(clust)
     else:
         y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
                                 resolution = Clustering_resolution)
         
@@ -1088,20 +1088,20 @@
     etime = round(time.time() - start_time) 
     print('G(%i)' % etime, end = '', flush = True)
     
     ## Replace GMM scores with their cluster mean
     if ref_ind is not None:
         dft, params = get_cnv_threshold_useref( df, ref_ind, 
                                        score_key = score_key, cluster_key = cluster_key,
-                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = cmd_cutoff,
+                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = dec_margin,
                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
     else:
         dft, params = get_cnv_threshold_bimodal( df, ref_ind, 
                                         score_key = score_key, cluster_key = cluster_key, 
-                                        th_min = th_min, refp_min = refp_min, ucr = cmd_cutoff,
+                                        th_min = th_min, refp_min = refp_min, ucr = dec_margin,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
     
     etime = round(time.time() - start_time) 
     print(' .. done (%i) ' % etime) #, end = '', flush = True)
     
     return df, params
```

### Comparing `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.2.0/setup.py` & `mlbi_at_dku_lib-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.2.0',
+    version             = '0.2.1',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

