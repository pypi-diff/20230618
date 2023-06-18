# Comparing `tmp/mlbi_at_dku_lib-0.1.8.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.8.tar", last modified: Sat Jun 17 08:47:21 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.9.tar", last modified: Sun Jun 18 06:32:59 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.8.tar` & `mlbi_at_dku_lib-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.485413 mlbi_at_dku_lib-0.1.8/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.8/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.8/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-17 08:47:21.485413 mlbi_at_dku_lib-0.1.8/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.8/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.453413 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.473413 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-17 08:47:21.485413 mlbi_at_dku_lib-0.1.8/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-17 08:47:14.000000 mlbi_at_dku_lib-0.1.8/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.473413 mlbi_at_dku_lib-0.1.8/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.8/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.9/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.9/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.9/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30639 2023-06-18 06:25:48.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-18 06:32:59.000000 mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-18 06:32:51.000000 mlbi_at_dku_lib-0.1.9/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 06:32:59.788079 mlbi_at_dku_lib-0.1.9/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.9/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.8/LICENSE` & `mlbi_at_dku_lib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.8/PKG-INFO` & `mlbi_at_dku_lib-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/icnv.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     pr[b] = MIN_ABS_VALUE
     
     return pr
 
 
 def get_cnv_threshold_bimodal( obs, ref_key, ref_types, score_key = 'cnv_score', 
                                cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
-                               plot_stat = True, suffix = '', Data = None ):
+                               ucr = 0.1, plot_stat = True, suffix = '', Data = None ):
     
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
     
     df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
     idx_lst = list(df.index.values)
     
     ps = bimodal_fit( df['cmean'] )
@@ -124,45 +124,31 @@
     tpr = get_malignancy_prob( s, list(ps) )
     obs['tumor_score'+ suffix] = tpr
     
     # print('threshold: ', th )
     th = max(th, th_min)
     
     dec = pd.Series(['Normal']*len(s), index = obs.index)
-    '''
-    b = s >= th
-    dec[b] = 'Tumor'
-    dec[~b] = 'Normal'
-    '''
     
-    # br = (obs[ref_key].isin(ref_types))
+    lt = th - (th - m0)*ucr # p_exc 
+    ut = th + (m1 - th)*ucr #p_exc
+    
     bs = (s > th)
+    df['dec'] = 'Normal'
     for idx in idx_lst:
-        if df.loc[idx, 'cmean'] > th:
-            b1 = obs[cluster_key] == idx
+        b1 = obs[cluster_key] == idx
+        if df.loc[idx, 'cmean'] > ut:            
             dec[b1] = 'Tumor'
-    
-#     br = (obs[ref_key].isin(ref_types))
-#     bs = (s > th)
-#     for idx in idx_lst:
-#         if df.loc[idx, 'cmean'] > th:
-#             b1 = obs[cluster_key] == idx
-#             if np.sum(b1&br) == 0:
-#                 dec[b1] = 'Tumor'
-#             elif np.sum(b1&br)/np.sum(b1) >= refp_min:
-#                 pass
-#             else:
-#                 dec[b1&bs&(~br)] = 'Tumor'
+            df.loc[idx, 'dec'] = 'Tumor'
+        elif df.loc[idx, 'cmean'] < lt:
+            pass
+        else:
+            dec[b1] = 'unclear'
+            df.loc[idx, 'dec'] = 'unclear'
                 
-#                 # if np.sum(b1&(~br)&bs)/np.sum(b1) < 0.4:
-#                 if np.sum(b1&bs&(~br)/np.sum(b1) < 0.3:
-#                     pass
-#                 else:
-#                     # dec[b1&(~br)&bs] = 'Tumor'
-#                     dec[b1&bs&(~br)] = 'Tumor'
     
     # b = (obs[ref_key].isin(ref_types)) | (s <= th)
     # dec[b] = 'Normal'    
     obs['tumor_dec'+ suffix] = dec
     
     tclust = dec.copy(deep = True)
     tclust[:] = None
@@ -172,41 +158,35 @@
         b1 = dec == 'Tumor'
         if np.sum(b&b1) > 0:
             tclust[b&b1] = 'Tumor_c%i' % cnt
             cnt += 1        
     obs['tumor_cluster'+ suffix] = tclust
 
     ss_div_dm = (np.sqrt(v1)+np.sqrt(v0))/(m1-m0)
-    print('Std_sum/Mean_diff: %f' % (ss_div_dm))
+    if ss_div_dm > 1:
+        print('INFO: Std_sum/Mean_diff: %f > 1' % (ss_div_dm))
+        print('INFO: indicating that no tumor cells might be present in this sample.' % (ss_div_dm))
+    
+    params = {}
+    params['th'] = th
+    params['m0'] = m0
+    params['v0'] = v0
+    params['w0'] = w0
+    params['m1'] = m1
+    params['v1'] = v1
+    params['w1'] = w1
+    params['df'] = df
     
     if plot_stat:
-        nn = len(df['cmean'])
-        pdf0 = pdf0*(w0*nn*(200/n_bins)/pdf0.sum())
-        pdf1 = pdf1*(w1*nn*(200/n_bins)/pdf1.sum())
-
-        pr = get_malignancy_prob( xs0, [w0, m0, v0, w1, m1, v1] )
-
-        plt.figure(figsize = (4,3))
-        df['cmean'].hist(bins = n_bins)
-        plt.plot(xs0, pdf0)
-        plt.plot(xs1, pdf1)
-        plt.plot([th, th], [0, max(pdf0.max(), pdf1.max())])
-        plt.plot(xs0, pr)
-
-        # plt.title('Unsupervised Bimodal Fit')
-        if Data is None: plt.title('Unsupervised Bimodal Fit')
-        else: plt.title('Unsupervised Bimodal Fit (%s)' % Data)
-        plt.xlabel('CNV_score')
-        plt.ylabel('Number of clusters') 
-        plt.legend(['Normal', 'Tumor', 'Threshold','Score hist.', 'Tumor Prob.'], 
-                   loc = 'upper left', bbox_to_anchor = (1, 1))
-        plt.yscale('log')
-        plt.show()
+        plot_stats( params, n_bins = 30, title = None, title_fs = 14,
+                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
+                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
+                    figsize = (4,3), log = False, alpha = 0.8 )
         
-    return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix]]
+    return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix]], params
 
 
 def get_cnv_threshold_useref( obs, ref_key, ref_types, score_key = 'tumor_score', 
                               cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
                               p_exc = 0.1, ucr = 0.1, plot_stat = True, 
                               suffix = '', Data = None ):
     
@@ -420,67 +400,31 @@
             tclust[b&b1] = 'Tumor_c%i' % cnt
             cnt += 1        
     obs['tumor_cluster'+ suffix] = tclust
     
     etime = round(time.time() - start_time) 
     # print('CNVth(%i) ' % etime, end = '', flush = True)
     
+    params = {}
+    params['th'] = th
+    params['m0'] = m0
+    params['v0'] = v0
+    params['w0'] = w0
+    params['m1'] = m1
+    params['v1'] = v1
+    params['w1'] = w1
+    params['df'] = df
+    
     if plot_stat:
-        pr = pdf1/(pdf1 + pdf0) # get_malignancy_prob( xs0, [w0, m0, v0, w1, m1, v1] )
-        b = (xs0 < m0)
-        pr[b] = MIN_ABS_VALUE
-
-        nn = len(df['cmean'])
-        pdf0 = pdf0*(w0*nn*(200/n_bins)/pdf0.sum())
-        pdf1 = pdf1*(w1*nn*(200/n_bins)/(pdf1.sum() + MIN_ABS_VALUE))
-
-        plt.figure(figsize = (4,3))
-        
-#         legend_labels = []
-#         rstep = 0.1
-#         b = df['dec'] == 'Normal'
-#         if np.sum(b) > 0:
-#             legend_labels.append('Normal')
-#             n_bins = round((df.loc[b, 'cmean'].max() - df.loc[b, 'cmean'].min())/rstep)
-#             if n_bins < 10: n_bins = 10
-#             df.loc[b, 'cmean'].hist(bins = n_bins, alpha = 0.6)
-#         b = df['dec'] == 'Tumor'
-#         if np.sum(b) > 0:
-#             legend_labels.append('Tumor')
-#             n_bins = round((df.loc[b, 'cmean'].max() - df.loc[b, 'cmean'].min())/rstep)
-#             if n_bins < 10: n_bins = 10
-#             df.loc[b, 'cmean'].hist(bins = n_bins, alpha = 0.6)
-#         b = df['dec'] == 'unclear'
-#         if np.sum(b) > 0:
-#             legend_labels.append('unclear')
-#             n_bins = round((df.loc[b, 'cmean'].max() - df.loc[b, 'cmean'].min())/rstep)
-#             if n_bins < 10: n_bins = 10
-#             df.loc[b, 'cmean'].hist(bins = n_bins, alpha = 0.6)
-#         plt.legend(legend_labels, #, 'Score hist.'], 
-#                    loc = 'upper left', bbox_to_anchor = (1, 1))
-
-        df['cmean'].hist(bins = n_bins)
-        plt.plot(xs0, pdf0)
-        plt.plot(xs1, pdf1)
-        plt.plot([th, th], [0, max(pdf0.max(), pdf1.max())])
-        plt.plot([lt, lt], [0, max(pdf0.max(), pdf1.max())])
-        plt.plot([ut, ut], [0, max(pdf0.max(), pdf1.max())])
-        plt.plot(xs0, pr)
-        plt.legend(['Normal', 'Tumor', 'Threshold', 'Tumor Prob.'], #, 'Score hist.'], 
-                   loc = 'upper left', bbox_to_anchor = (1, 1))
-        plt.yscale('log')
-        
-        # plt.title('Bimodal Fit using Reference')
-        if Data is None: plt.title('Bimodal Fit using Reference')
-        else: plt.title('Bimodal Fit using Ref (%s)' % Data)
-        plt.xlabel('CNV_score')
-        plt.ylabel('Number of clusters')
-        plt.show()
+        plot_stats( params, n_bins = 30, title = None, title_fs = 14,
+                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
+                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
+                    figsize = (4,3), log = False, alpha = 0.8 )
         
-    return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix, 'tumor_cluster'+ suffix]]
+    return obs[['tumor_dec'+ suffix, 'tumor_prob'+ suffix, 'tumor_cluster'+ suffix]], params
 
 
 def get_cnv_threshold( obs, cluster_sel, score_key = 'cnv_score', 
                        cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
                        p_exc = 0.1, plot_stat = True, suffix = '', Data = None ):
     
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
@@ -644,41 +588,109 @@
             tclust[b&b1] = 'Tumor_c%i' % cnt
             cnt += 1        
     obs['tumor_cluster'+ suffix] = tclust
     
     etime = round(time.time() - start_time) 
     # print('CNVth(%i) ' % etime, end = '', flush = True)
     
+    params = {}
+    params['th'] = th
+    params['m0'] = m0
+    params['v0'] = v0
+    params['w0'] = w0
+    params['m1'] = m1
+    params['v1'] = v1
+    params['w1'] = w1
+    params['df'] = df
+    
     if plot_stat:
-        pr = pdf1/(pdf1 + pdf0) # get_malignancy_prob( xs0, [w0, m0, v0, w1, m1, v1] )
-        b = (xs0 < m0)
-        pr[b] = MIN_ABS_VALUE
-
-        nn = len(df['cmean'])
-        pdf0 = pdf0*(w0*nn*(200/n_bins)/pdf0.sum())
-        pdf1 = pdf1*(w1*nn*(200/n_bins)/(pdf1.sum() + MIN_ABS_VALUE))
-
-        plt.figure(figsize = (4,3))
-        df['cmean'].hist(bins = n_bins)
-        plt.plot(xs0, pdf0)
-        plt.plot(xs1, pdf1)
-        plt.plot([th, th], [0, max(pdf0.max(), pdf1.max())])
-        plt.plot(xs0, pr)
-
-        if Data is None: plt.title('Unsupervised Bimodal Fit')
-        else: plt.title('Unsupervised Bimodal Fit (%s)' % Data)
-        plt.xlabel('CNV_score')
-        plt.ylabel('Number of clusters')
-        plt.legend(['Normal', 'Tumor', 'Threshold', 'Tumor Prob.'], #, 'Score hist.'], 
-                   loc = 'upper left', bbox_to_anchor = (1, 1))
-        plt.yscale('log')
-        plt.show()
+        plot_stats( params, n_bins = 30, title = None, title_fs = 14,
+                    label_fs = 12, tick_fs = 11, legend_fs = 11, 
+                    legend_loc = 'upper left', bbox_to_anchor = (1, 1),
+                    figsize = (4,3), log = False, alpha = 0.8 )
+
+    return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix, 'tumor_cluster'+ suffix]], params
+
+
+def plot_stats( params, n_bins = 30, title = None, title_fs = 14,
+                label_fs = 12, tick_fs = 11, legend_fs = 11, 
+                legend_loc = 'upper left', bbox_to_anchor = (1, 1),
+                figsize = (4,3), log = True, alpha = 0.8 ):
+    
+    th = params['th']
+    m0 = params['m0']
+    v0 = params['v0']
+    w0 = params['w0']
+    m1 = params['m1']
+    v1 = params['v1']
+    w1 = params['w1']
+    df = params['df']
         
-    return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix, 'tumor_cluster'+ suffix]]
+    mxv = df['cmean'].max()
+    mnv = df['cmean'].min()
+    Dv = mxv - mnv
+    dv = Dv/200
+
+    x = np.arange(mnv,mxv,dv)
+    pdf0, xs0 = get_normal_pdf( x, m0, v0, 100)
+    pdf1, xs1 = get_normal_pdf( x, m1, v1, 100)
+    
+    pr = pdf1/(pdf1 + pdf0) # get_malignancy_prob( xs0, [w0, m0, v0, w1, m1, v1] )
+    bx = (xs0 >= m0) & ((xs1 <= m1))
 
+    nn = len(df['cmean'])
+    pdf0 = pdf0*(w0*nn*(200/n_bins)/pdf0.sum())
+    pdf1 = pdf1*(w1*nn*(200/n_bins)/(pdf1.sum())) 
+
+    max_pdf = max(pdf0.max(), pdf1.max())
+    
+    plt.figure(figsize = figsize)
+    ax = plt.gca()
+    
+    counts, bins = np.histogram(df['cmean'], bins = n_bins)
+    # max_cnt = np.max(counts)
+
+    legend_labels = []
+    
+    max_cnt = 0
+    b = df['dec'] == 'Normal'
+    if np.sum(b) > 0:
+        legend_labels.append('Normal')
+        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
+        max_cnt = max(max_cnt, np.max(counts))
+    b = df['dec'] == 'Tumor'
+    if np.sum(b) > 0:
+        legend_labels.append('Tumor')
+        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
+        max_cnt = max(max_cnt, np.max(counts))
+    b = df['dec'] == 'unclear'
+    if np.sum(b) > 0:
+        legend_labels.append('unclear')
+        counts, bins_t, bar_t = plt.hist(df.loc[b, 'cmean'], bins = bins, alpha = alpha)
+        max_cnt = max(max_cnt, np.max(counts))
+    
+    sf = 0.9*max_cnt/max_pdf
+    plt.plot(xs0, pdf0*sf)
+    plt.plot(xs1, pdf1*sf)
+    plt.plot([th, th], [0, max_cnt]) # max(pdf0.max()*sf, pdf1.max()*sf)])
+    plt.plot(xs0[bx], pr[bx]*max_cnt)
+
+    if title is not None: plt.title(title, fontsize = title_fs)
+    plt.xlabel('CNV_score', fontsize = label_fs)
+    plt.ylabel('Number of clusters', fontsize = label_fs)
+    plt.legend(['Normal distr.', 'Tumor distr.', 'Threshold', 'Tumor Prob.'], #, 'Score hist.'], 
+               loc = legend_loc, bbox_to_anchor = bbox_to_anchor, fontsize = legend_fs)
+    if log: plt.yscale('log')
+    ax.tick_params(axis='x', labelsize=tick_fs)
+    ax.tick_params(axis='y', labelsize=tick_fs)
+    plt.grid()
+    plt.show()
+        
+    return 
+    
 
 def get_cnv_dec(adata, ref_key, ref_types, cluster_key = 'cnv_leiden', 
                        score_key = 'cnv_score', th_min = 0, use_ref = True, suffix = ''):
     
     if use_ref:
         df = get_cnv_threshold_useref( adata.obs, ref_key, ref_types, 
                                        score_key = score_key, cluster_key = cluster_key, th_min = th_min,
@@ -835,22 +847,22 @@
                 print('ERROR: No reference cell types found.')
                 adata.obs[score_key] = 0
                 adata.obs['tumor_prob'+ suffix] = 0
                 adata.obs['tumor_dec'+ suffix] = 'NA'
                 adata.obs['tumor_cluster'+ suffix] = ''
                 return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
                           'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+            X_pca_sel = X_pca[b,:]
+        else:
+            X_pca_sel = X_pca
 
 
         etime = round(time.time() - start_time) 
         # print('C(%i).' % etime, end = '', flush = True)
 
-        #'''
-        X_pca_sel = X_pca[b,:]
-
         ## Get GMM model parameters
         gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
         gmm.fit(X_pca_sel)
         y_conf_gmm = -gmm.score_samples(X_pca)
         #'''
         X_cnv = pd.DataFrame(adata.obsm['X_cnv'].todense(), index = adata.obs.index.values)
         y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
@@ -871,29 +883,29 @@
     '''
     cnv_clust_lst = list(set(adata.obs[cluster_key]))
     for c in cnv_clust_lst:
         b = adata.obs[cluster_key] == c
         adata.obs.loc[b, score_key] = adata.obs.loc[b, score_key].mean()
     '''
     if use_ref:
-        df = get_cnv_threshold_useref( adata.obs, ref_key, ref_types, 
+        df, params = get_cnv_threshold_useref( adata.obs, ref_key, ref_types, 
                                        score_key = score_key, cluster_key = cluster_key,
                                        th_min = th_min, refp_min = refp_min, p_exc = p_exc, ucr = cmd_cutoff,
                                        plot_stat = plot_stat, suffix = suffix, Data = Data )
     else:
-        df = get_cnv_threshold_bimodal( adata.obs, ref_key, ref_types, 
+        df, params = get_cnv_threshold_bimodal( adata.obs, ref_key, ref_types, 
                                         score_key = score_key, cluster_key = cluster_key, 
-                                        th_min = th_min, refp_min = refp_min, # p_exc = 0.1, 
+                                        th_min = th_min, refp_min = refp_min, ucr = cmd_cutoff,
                                         plot_stat = plot_stat, suffix = suffix, Data = Data )
     
     etime = round(time.time() - start_time) 
     print(' .. done (%i) ' % etime) #, end = '', flush = True)
     
     return adata.obs[[cluster_key, score_key, 'tumor_dec'+suffix, 
-                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]]
+                      'tumor_prob'+suffix, 'tumor_cluster'+ suffix]], params
 
 
 import warnings
 
 def run_icnv(adata, ref_key, ref_types, gtf_file, cluster_key = 'cnv_leiden', 
              resolution = 2, N_pca = 15, n_neighbors = 10, pca_umap = True ):
```

### Comparing `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.9/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.8/setup.py` & `mlbi_at_dku_lib-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.8',
+    version             = '0.1.9',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

