# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.6.17-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.6.18-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,40 +1,40 @@
-Zip file size: 3194102 bytes, number of entries: 38
--rw-r--r--  2.0 unx      567 b- defN 23-Jun-17 12:57 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-Jun-17 12:57 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Jun-17 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jun-17 12:57 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10704968 b- defN 23-Jun-17 12:57 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-Jun-17 12:57 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-Jun-17 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2477 b- defN 23-Jun-17 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Jun-17 12:57 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Jun-17 12:57 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5727 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     6661 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    19751 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    61087 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    77521 b- defN 23-Jun-17 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39508 b- defN 23-Jun-17 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jun-17 12:57 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1505 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     3268 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3026 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Jun-17 12:51 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3268 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     2976 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     2551 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     3284 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3284 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     4919 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     6928 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3019 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4875 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     4164 b- defN 23-Jun-17 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     2934 b- defN 23-Jun-17 12:57 fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-17 12:57 fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-17 12:57 fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4171 b- defN 23-Jun-17 12:57 fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/RECORD
-38 files, 11023708 bytes uncompressed, 3187080 bytes compressed:  71.1%
+Zip file size: 3194103 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      567 b- defN 23-Jun-18 12:57 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-Jun-18 12:57 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Jun-18 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jun-18 12:57 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10704968 b- defN 23-Jun-18 12:57 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-Jun-18 12:57 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Jun-18 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2477 b- defN 23-Jun-18 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Jun-18 12:57 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-Jun-18 12:57 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5727 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     6661 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    19751 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    61087 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    77521 b- defN 23-Jun-18 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39508 b- defN 23-Jun-18 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Jun-18 12:57 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1505 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     3268 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3026 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-Jun-18 12:52 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3268 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     2976 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     2551 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     3284 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3284 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     4919 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     6928 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3019 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4875 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     4164 b- defN 23-Jun-18 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-Jun-18 12:57 fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-18 12:57 fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-18 12:57 fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4171 b- defN 23-Jun-18 12:57 fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/RECORD
+38 files, 11023708 bytes uncompressed, 3187081 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -96,20 +96,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.6.17
+Version: 2023.6.18
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=GkOhkl3-XKu3xyDXKzk8XPCtkA_0TdAI6hjsL0MClnU,3284
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=BDtx7iIyOR--Ws-CVpkEPxrJLd9_zBs4AfWnDeF0jAk,3284
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=8kUKUJAR19mb2wkTKwWgH7th7ZEXeCsxkH3YbvE9dN4,4919
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=YQklXzidPuOldTLpScvNm_QVkIH1Igue3YmEy_YRFtw,6928
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=BllKtG77efcD_L3Wz2oKnOfozApTfNVLkWSwZOug2cE,3019
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=Z61ddb_JEiwtoi-iphmijUYybdTN-sqIgTPVUFTBJtU,4875
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=bwnpj8egWnyC_ze2e3ZI1B9NWO_WxQDDIs1fNX5jMwM,4164
-fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/METADATA,sha256=-ofoGbs9yNWdcbmcXPLvf9UNvX_XL19ey3r7eCa-q8Q,2934
-fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
-fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.6.17.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/METADATA,sha256=e-HkeAmZFQVzePrYrDMKCkcLTYY4S2TsPmUmZWQZ9gk,2934
+fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
+fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.6.18.dist-info/RECORD,,
```

