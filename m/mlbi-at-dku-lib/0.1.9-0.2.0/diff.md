# Comparing `tmp/mlbi_at_dku_lib-0.1.9.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.9.tar", last modified: Sun Jun 18 06:32:59 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.0.tar", last modified: Sun Jun 18 09:51:40 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.9.tar` & `mlbi_at_dku_lib-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.9/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.9/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.9/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30639 2023-06-18 06:25:48.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-18 06:32:51.000000 mlbi_at_dku_lib-0.1.9/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.9/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.0/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.0/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.0/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36537 2023-06-18 09:51:04.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-18 09:51:40.000000 mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-18 09:51:32.000000 mlbi_at_dku_lib-0.2.0/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 09:51:40.207347 mlbi_at_dku_lib-0.2.0/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.0/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.9/LICENSE` & `mlbi_at_dku_lib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.9/PKG-INFO` & `mlbi_at_dku_lib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/icnv.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     
     b = (xs < mu0)
     pr[b] = MIN_ABS_VALUE
     
     return pr
 
 
-def get_cnv_threshold_bimodal( obs, ref_key, ref_types, score_key = 'cnv_score', 
+def get_cnv_threshold_bimodal( obs, ref_ind, score_key = 'cnv_score', 
                                cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
                                ucr = 0.1, plot_stat = True, suffix = '', Data = None ):
     
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
     
     df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
     idx_lst = list(df.index.values)
@@ -181,15 +181,15 @@
                     label_fs = 12, tick_fs = 11, legend_fs = 11, 
                     legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                     figsize = (4,3), log = False, alpha = 0.8 )
         
     return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix]], params
 
 
-def get_cnv_threshold_useref( obs, ref_key, ref_types, score_key = 'tumor_score', 
+def get_cnv_threshold_useref( obs, ref_ind, score_key = 'tumor_score', 
                               cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
                               p_exc = 0.1, ucr = 0.1, plot_stat = True, 
                               suffix = '', Data = None ):
     
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
     start_time = time.time()
     
@@ -200,23 +200,23 @@
     ns = 0
     # while(ns == 0):
         
     b_inc = []
     df['Ref_percent'] = 0
     for idx in idx_lst:
         b = obs[cluster_key] == idx
-        cts = obs.loc[b, ref_key]
+        # cts = obs.loc[b, ref_key]
         '''
         ct_vc = cts.value_counts()
         cnt = 0
         for ct in list(ct_vc.index.values):
             if ct in ref_types:
                 cnt += ct_vc[ct]
         '''
-        cnt = np.sum(cts.isin(ref_types))
+        cnt = np.sum(np.array(ref_ind)[b])
         ref_percent = cnt/np.sum(b)
         df.loc[idx, 'Ref_percent'] = ref_percent
         if (ref_percent >= refp_min):
             b_inc.append(True)
         else:
             b_inc.append(False)
 
@@ -332,15 +332,15 @@
     
     dec = pd.Series(['Normal']*len(s), index = obs.index)
     '''
     b = s >= th
     dec[b] = 'Tumor'
     dec[~b] = 'Normal'
     '''
-    br = (obs[ref_key].isin(ref_types))
+    br = np.array(ref_ind)
     bs = (s > th)
     
     #'''
     lt = th - (th - m0)*ucr # p_exc 
     ut = th + (m1 - th)*ucr #p_exc
 #     b = (s > lt) & (s < ut) & (~br)
 #     print(lt, ut, np.sum(~br), np.sum(b))
@@ -785,15 +785,15 @@
     
     ss = np.array(ss)
     odr = ss.argsort()
     
     return cm[odr[0]]
 
 
-def compute_cnv_scores(adata, ref_key, ref_types, use_cnv_score = False,
+def compute_cnv_scores(adata, ref_ind, use_cnv_score = False,
                        cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
                        cmd_cutoff = 0.01, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
                        plot_stat = False, use_cnv_cluster = True, use_ref = True, suffix = '', Data = None):
     
     score_key = score_key + suffix
     ## Get X_pca for ref_type cells
@@ -825,17 +825,16 @@
         adata.obs[score_key] = adata.obs['cnv_score']
     else:
         if use_ref:
             cnv_clust_lst.sort()
             b_inc = []
             for idx in cnv_clust_lst:
                 b = y_clust == idx
-                cts = adata.obs.loc[b, ref_key]
-                bt = cts.isin(ref_types)
-                cnt = np.sum(bt)
+                bt = ref_ind
+                cnt = np.sum(b&bt)
 
                 if (cnt >= refp_min*np.sum(b)):
                     b_inc.append(True)
                 else:
                     b_inc.append(False)
 
             if np.sum(b_inc) > 0:
@@ -883,20 +882,20 @@
     '''
     cnv_clust_lst = list(set(adata.obs[cluster_key]))
     for c in cnv_clust_lst:
         b = adata.obs[cluster_key] == c
         adata.obs.loc[b, score_key] = adata.obs.loc[b, score_key].mean()
     '''
     if use_ref:
-        df, params = get_cnv_threshold_useref( adata.obs, ref_key, ref_types, 
+        df, params = get_cnv_threshold_useref( adata.obs, ref_ind, 
                                        score_key = score_key, cluster_key = cluster_key,
                                        th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = cmd_cutoff,
                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
     else:
-        df, params = get_cnv_threshold_bimodal( adata.obs, ref_key, ref_types, 
+        df, params = get_cnv_threshold_bimodal( adata.obs, ref_ind, 
                                         score_key = score_key, cluster_key = cluster_key, 
                                         th_min = th_min, refp_min = refp_min, ucr = cmd_cutoff,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
     
     etime = round(time.time() - start_time) 
     print(' .. done (%i) ' % etime) #, end = '', flush = True)
     
@@ -933,7 +932,176 @@
             cnv.tl.umap(adata)
             
         print('Scoring .. ', end = '')
         cnv.tl.cnv_score(adata, groupby = cluster_key, key_added = 'cnv_score')
         print('done.')
 
     return adata
+
+
+
+from sklearn.decomposition import PCA
+from sklearn import cluster, mixture
+from sklearn.neighbors import KNeighborsRegressor
+from sklearn.neighbors import kneighbors_graph
+from sklearn.neighbors import NearestNeighbors
+
+CLUSTERING_AGO = 'lv'
+SKNETWORK = True
+try:
+    from sknetwork.clustering import Louvain
+except ImportError:
+    print('WARNING: sknetwork not installed. Will used GMM for clustering.')
+    CLUSTERING_AGO = 'gmm'
+    SKNETWORK = False
+
+from sklearn.decomposition import PCA
+from sklearn import cluster, mixture
+from sklearn.neighbors import KNeighborsRegressor
+from sklearn.neighbors import kneighbors_graph
+from sklearn.neighbors import NearestNeighbors
+
+CLUSTERING_AGO = 'lv'
+SKNETWORK = True
+try:
+    from sknetwork.clustering import Louvain
+except ImportError:
+    print('WARNING: sknetwork not installed. Will used GMM for clustering.')
+    CLUSTERING_AGO = 'gmm'
+    SKNETWORK = False
+
+    
+def clustering_alg(X_pca, clust_algo = 'lv', N_clusters = 25, resolution = 1, N_neighbors = 10):
+    
+    if clust_algo[:2] == 'gm':
+        gmm = mixture.GaussianMixture(n_components = int(N_clusters), random_state = 0)
+        cluster_label = gmm.fit_predict(np.array(X_pca))
+        return cluster_label, gmm
+    elif clust_algo[:2] == 'km':
+        km = cluster.KMeans(n_clusters = int(N_clusters), random_state = 0)
+        km.fit(X_pca)
+        cluster_label = km.labels_
+        return cluster_label, km
+    else:
+        adj = kneighbors_graph(X_pca, int(N_neighbors), mode='connectivity', include_self=True)
+        louvain = Louvain(resolution = resolution)
+        if hasattr(louvain, 'fit_predict'):
+            cluster_label = louvain.fit_predict(adj)        
+        else:
+            cluster_label = louvain.fit_transform(adj)        
+        return cluster_label, louvain
+    '''
+    elif clust_algo[:2] == 'ld':
+        leiden = LeidenClustering()
+        leiden.fit(X)
+        cluster_label = leiden.labels_
+        return cluster_label, km
+    '''
+
+def detect_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
+                       clust = None, Clustering_resolution = 1, N_clusters = 30,
+                       # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
+                       gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
+                       cmd_cutoff = 0.01, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
+                       plot_stat = False, use_cnv_cluster = True, use_ref = True, 
+                       suffix = '', Data = None):
+    
+    score_key = 'tumor_score' + suffix
+    cluster_key = 'cnv_cluster' 
+    ## Get X_pca for ref_type cells
+
+    start_time = time.time()
+    print('Running iCNV addon .. ', end = '', flush = True)
+    
+    if isinstance(X_cnv, pd.DataFrame):
+        df = pd.DataFrame(index = X_cnv.index.values)
+    else:
+        df = pd.DataFrame()
+        X_cnv = pd.DataFrame(X_cnv)
+    
+    N_components_pca = 15
+    pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
+
+    if not pca: 
+        X_pca = pca_obj.fit_transform(X_cnv)
+    else: 
+        X_pca = X_cnv #.copy(deep = True)
+            
+    if clust:      
+        y_clust = list(clust)
+    else:
+        y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
+                                resolution = Clustering_resolution)
+        
+    cnv_clust_lst = list(set(y_clust))
+    df[cluster_key] = y_clust
+        
+    if use_ref:
+        cnv_clust_lst.sort()
+        b_inc = []
+        for idx in cnv_clust_lst:
+            b = y_clust == idx
+            bt = b & ref_ind
+            cnt = np.sum(bt)
+
+            if (cnt >= refp_min*np.sum(b)):
+                b_inc.append(True)
+            else:
+                b_inc.append(False)
+
+        if np.sum(b_inc) > 0:
+            cluster_sel = list(np.array(cnv_clust_lst)[b_inc]) 
+            b = y_clust == cluster_sel[0]
+            for c in cluster_sel[1:]:
+                b = b | (y_clust == c)
+        else:
+            print('ERROR: No reference cell types found.')
+            df[score_key] = 0
+            df['tumor_prob'+ suffix] = 0
+            df['tumor_dec'+ suffix] = 'NA'
+            df['tumor_cluster'+ suffix] = ''
+            return df[[cluster_key, score_key, 'tumor_dec'+suffix, 
+                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+        X_pca_sel = X_pca[b,:]
+    else:
+        X_pca_sel = X_pca
+
+
+    etime = round(time.time() - start_time) 
+    # print('C(%i).' % etime, end = '', flush = True)
+
+    ## Get GMM model parameters
+    gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
+    gmm.fit(X_pca_sel)
+    y_conf_gmm = -gmm.score_samples(X_pca)
+    #'''
+    y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
+
+    yc = np.array(y_conf)
+    odr = yc.argsort()
+    n = int(len(yc)*0.975)
+    ymax = yc[odr[n]]
+    b = y_conf > ymax
+    y_conf[b] = ymax
+
+    df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm*gcm)))
+
+    etime = round(time.time() - start_time) 
+    print('G(%i)' % etime, end = '', flush = True)
+    
+    ## Replace GMM scores with their cluster mean
+    if ref_ind is not None:
+        dft, params = get_cnv_threshold_useref( df, ref_ind, 
+                                       score_key = score_key, cluster_key = cluster_key,
+                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = cmd_cutoff,
+                                       plot_stat = plot_stat, suffix = suffix, Data = Data )
+    else:
+        dft, params = get_cnv_threshold_bimodal( df, ref_ind, 
+                                        score_key = score_key, cluster_key = cluster_key, 
+                                        th_min = th_min, refp_min = refp_min, ucr = cmd_cutoff,
+                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
+    
+    etime = round(time.time() - start_time) 
+    print(' .. done (%i) ' % etime) #, end = '', flush = True)
+    
+    return df, params
+
```

### Comparing `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.2.0/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.9
+Version: 0.2.0
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.9/setup.py` & `mlbi_at_dku_lib-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.9',
+    version             = '0.2.0',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

