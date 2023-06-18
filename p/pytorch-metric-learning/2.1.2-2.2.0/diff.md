# Comparing `tmp/pytorch-metric-learning-2.1.2.tar.gz` & `tmp/pytorch-metric-learning-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-metric-learning-2.1.2.tar", last modified: Sat May 27 21:20:23 2023, max compression
+gzip compressed data, was "pytorch-metric-learning-2.2.0.tar", last modified: Sun Jun 18 18:02:42 2023, max compression
```

## Comparing `pytorch-metric-learning-2.1.2.tar` & `pytorch-metric-learning-2.2.0.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1090 2019-10-24 20:18:14.000000 pytorch-metric-learning-2.1.2/LICENSE
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15724 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/PKG-INFO
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15069 2023-05-26 16:32:49.000000 pytorch-metric-learning-2.1.2/README.md
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       38 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/setup.cfg
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1507 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.2/setup.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.352563 pytorch-metric-learning-2.1.2/src/
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.376563 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       23 2023-05-26 17:54:49.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/__init__.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.424564 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      265 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3508 2023-05-03 11:30:19.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/base_distance.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      755 2023-01-29 03:05:20.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/batched_distance.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      274 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/cosine_similarity.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      424 2021-02-11 13:46:54.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/dot_product_similarity.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1042 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/lp_distance.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      714 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/snr_distance.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.576566 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1617 2023-04-05 22:50:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/__init__.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3061 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/angular_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1386 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/arcface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      391 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/base_loss_wrapper.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2456 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/base_metric_loss_function.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2832 2021-02-11 13:46:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/circle_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2005 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/contrastive_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      939 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cosface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5333 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cross_batch_memory.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2833 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/fast_ap_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1492 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/generic_pair_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1689 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/instance_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2047 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5674 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3034 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/lifted_structure_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3288 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2863 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/mixins.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1558 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multi_similarity_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2351 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multiple_losses.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1463 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/n_pairs_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1957 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/nca_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2173 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1778 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/ntxent_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3506 2023-04-05 22:50:12.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/pnp_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3469 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1376 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_losses.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2021 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/self_supervised_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      373 2021-02-11 13:46:56.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3230 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/soft_triple_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      360 2021-02-11 13:46:57.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/sphereface_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2600 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1715 2021-05-08 22:57:02.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/supcon_loss.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2290 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/triplet_margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2049 2022-06-29 19:51:55.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3374 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/vicreg_loss.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.640566 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      569 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2874 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/angular_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2201 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/base_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     8131 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      404 2021-02-11 13:46:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/batch_hard_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2066 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/distance_weighted_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      493 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2192 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/hdc_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2315 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/multi_similarity_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1742 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/pair_margin_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2461 2023-05-26 16:17:34.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/triplet_margin_miner.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2303 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.692567 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      459 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      169 2021-02-11 13:46:59.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3816 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/base_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1130 2021-02-11 14:13:23.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1551 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/divisor_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      156 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      473 2021-02-11 13:47:00.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/mean_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1214 2021-02-11 14:13:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/multiple_reducers.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2149 2021-05-08 22:57:04.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)      182 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/sum_reducer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2211 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/threshold_reducer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.716567 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      338 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      499 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/base_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      871 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      723 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/lp_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1229 2021-02-11 14:20:16.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2697 2021-05-08 22:57:05.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      432 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.744568 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      220 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2132 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3846 2023-05-26 17:52:27.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2555 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1696 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.772568 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      243 2021-02-11 13:47:01.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    12495 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/base_tester.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1371 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_embedding_space.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2820 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2791 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/with_same_parent_label.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.796568 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      321 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11599 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/base_trainer.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     3002 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6807 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      625 2021-02-11 13:47:02.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/metric_loss_only.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1224 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/train_with_classifier.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     2295 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.880570 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2020-05-18 23:01:59.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/__init__.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    18488 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/accuracy_calculator.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15447 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/common_functions.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     6399 2023-01-29 22:17:17.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/distributed.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    11776 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/inference.py
--rw-r--r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1801 2023-01-29 03:05:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/key_checker.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15836 2023-02-21 17:27:25.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/logging_presets.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     9444 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1078 2023-01-29 21:12:58.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_tracker.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      661 2022-03-01 01:50:13.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records.py
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     1624 2021-11-28 18:40:10.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
-drwxrwxr-x   0 tkm45    (1100984) pug-tkm45 (1126026)        0 2023-05-27 21:20:23.384563 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)    15724 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/PKG-INFO
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)     5985 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/SOURCES.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)        1 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/dependency_links.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)      226 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/requires.txt
--rw-rw-r--   0 tkm45    (1100984) pug-tkm45 (1126026)       24 2023-05-27 21:20:21.000000 pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/top_level.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.458103 pytorch-metric-learning-2.2.0/
+-rw-r--r--   0 kevin      (501) staff       (20)     1090 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/LICENSE
+-rw-r--r--   0 kevin      (501) staff       (20)    15727 2023-06-18 18:02:42.457936 pytorch-metric-learning-2.2.0/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)    15109 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/README.md
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-06-18 18:02:42.458140 pytorch-metric-learning-2.2.0/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     1507 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.442916 pytorch-metric-learning-2.2.0/src/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.443979 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/
+-rw-r--r--   0 kevin      (501) staff       (20)       22 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.445503 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/
+-rw-r--r--   0 kevin      (501) staff       (20)      265 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3508 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/base_distance.py
+-rw-r--r--   0 kevin      (501) staff       (20)      755 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/batched_distance.py
+-rw-r--r--   0 kevin      (501) staff       (20)      274 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/cosine_similarity.py
+-rw-r--r--   0 kevin      (501) staff       (20)      424 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/dot_product_similarity.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1042 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/lp_distance.py
+-rw-r--r--   0 kevin      (501) staff       (20)      714 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/snr_distance.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.450231 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/
+-rw-r--r--   0 kevin      (501) staff       (20)     1696 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3061 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/angular_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1386 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/arcface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      391 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/base_loss_wrapper.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2456 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2832 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/circle_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2005 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/contrastive_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      939 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cosface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5333 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cross_batch_memory.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2833 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/fast_ap_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1492 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/generic_pair_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1689 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/instance_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2047 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5674 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3034 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4731 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/manifold_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3288 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/margin_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2863 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/mixins.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1558 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2351 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multiple_losses.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1463 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/n_pairs_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1957 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/nca_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2173 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1778 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/ntxent_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2635 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/p2s_grad_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3506 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/pnp_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3469 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1376 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_losses.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2269 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/self_supervised_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      373 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3230 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/soft_triple_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)      360 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/sphereface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2600 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1715 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/supcon_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2290 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2049 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3374 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/vicreg_loss.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.451826 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/
+-rw-r--r--   0 kevin      (501) staff       (20)      569 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2874 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/angular_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2201 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/base_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     8131 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)      404 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/batch_hard_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2066 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)      493 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/embeddings_already_packaged_as_triplets.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2192 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/hdc_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2315 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1742 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/pair_margin_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2461 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2303 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.453175 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/
+-rw-r--r--   0 kevin      (501) staff       (20)      459 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      169 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/avg_non_zero_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3816 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/base_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1130 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1551 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/divisor_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      156 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/do_nothing_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      473 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/mean_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/multiple_reducers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2149 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      182 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/sum_reducer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2211 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/threshold_reducer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.453962 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/
+-rw-r--r--   0 kevin      (501) staff       (20)      338 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      499 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/base_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      871 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      723 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1229 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2697 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      432 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/zero_mean_regularizer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.454567 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/
+-rw-r--r--   0 kevin      (501) staff       (20)      220 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2132 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3843 2023-06-18 18:02:05.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2555 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1696 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.455483 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/
+-rw-r--r--   0 kevin      (501) staff       (20)      243 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12495 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/base_tester.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1371 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_embedding_space.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2820 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2791 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/with_same_parent_label.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.456350 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/
+-rw-r--r--   0 kevin      (501) staff       (20)      321 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11599 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/base_trainer.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3002 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6807 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py
+-rw-r--r--   0 kevin      (501) staff       (20)      625 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/metric_loss_only.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1224 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/train_with_classifier.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2295 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.457752 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    18488 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/accuracy_calculator.py
+-rw-r--r--   0 kevin      (501) staff       (20)    15447 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/common_functions.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6399 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/distributed.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11776 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/inference.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1801 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/key_checker.py
+-rw-r--r--   0 kevin      (501) staff       (20)    15836 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/logging_presets.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9444 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1078 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_tracker.py
+-rw-r--r--   0 kevin      (501) staff       (20)      661 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1624 2023-06-18 00:46:47.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-06-18 18:02:42.444579 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)    15727 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     6089 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)      226 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       24 2023-06-18 18:02:42.000000 pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/top_level.txt
```

### Comparing `pytorch-metric-learning-2.1.2/LICENSE` & `pytorch-metric-learning-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/PKG-INFO` & `pytorch-metric-learning-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pytorch-metric-learning
-Version: 2.1.2
+Version: 2.2.0
 Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
 Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
 Author: Kevin Musgrave
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: with-hooks
 Provides-Extra: with-hooks-cpu
@@ -270,14 +268,15 @@
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
 | [yutanakamura-tky](https://github.com/yutanakamura-tky) | |
 | [KinglittleQ](https://github.com/KinglittleQ) | |
 | [martin0258](https://github.com/martin0258) | |
 | [michaeldeyzel](https://github.com/michaeldeyzel) | |
 | [HSinger04](https://github.com/HSinger04) | |
+| [rheum](https://github.com/rheum) | |
 
 
 
 ### Facebook AI
 Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This project began during my internship at Facebook AI where I received valuable feedback from Ser-Nam, and his team of computer vision and machine learning engineers and research scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its early stages of development.
 
 ### Open-source repos
@@ -302,9 +301,7 @@
   title={PyTorch Metric Learning},
   author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
   journal={ArXiv},
   year={2020},
   volume={abs/2008.09164}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.2 Summary: The
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.2.0 Summary: The
 easiest way to use deep metric learning in your application. Modular, flexible,
 and extensible. Written in PyTorch. Home-page: https://github.com/
-KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
-Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
-Provides-Extra: dev License-File: LICENSE
+KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.0
+Description-Content-Type: text/markdown Provides-Extra: with-hooks Provides-
+Extra: with-hooks-cpu Provides-Extra: docs Provides-Extra: dev License-File:
+LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
 ## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
 pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
 [interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
 Added SelfSupervisedLoss, plus various API improvements. See the [release
 notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
@@ -179,29 +179,30 @@
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
 [michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
-github.com/HSinger04) | | ### Facebook AI Thank you to [Ser-Nam Lim](https://
-research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/
-), and my research advisor, [Professor Serge Belongie](https://
-vision.cornell.edu/se3/people/serge-belongie/). This project began during my
-internship at Facebook AI where I received valuable feedback from Ser-Nam, and
-his team of computer vision and machine learning engineers and research
-scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/
-ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-
-3962aa7/) for reviewing my code during its early stages of development. ###
-Open-source repos This library contains code that has been adapted and modified
-from the following great open-source repos: - https://github.com/bnu-wangxun/
-Deep_Metric - https://github.com/chaoyuaw/incubator-mxnet/blob/master/example/
-gluon/embedding_learning - https://github.com/facebookresearch/deepcluster -
-https://github.com/geonm/proxy-anchor-loss - https://github.com/idstcv/
-SoftTriple - https://github.com/kunhe/FastAP-metric-learning - https://
-github.com/ronekko/deep_metric_learning - https://github.com/tjddus9597/Proxy-
-Anchor-CVPR2020 - http://kaizhao.net/regularface ### Logo Thanks to [Jeff
-Musgrave](https://www.designgenius.ca/) for designing the logo. ## Citing this
-library If you'd like to cite pytorch-metric-learning in your paper, you can
-use this bibtex: ```latex @article{Musgrave2020PyTorchML, title={PyTorch Metric
-Learning}, author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
-journal={ArXiv}, year={2020}, volume={abs/2008.09164} } ```
+github.com/HSinger04) | | | [rheum](https://github.com/rheum) | | ### Facebook
+AI Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at
+[Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor
+Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This
+project began during my internship at Facebook AI where I received valuable
+feedback from Ser-Nam, and his team of computer vision and machine learning
+engineers and research scientists. In particular, thanks to [Ashish Shah]
+(https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://
+www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its
+early stages of development. ### Open-source repos This library contains code
+that has been adapted and modified from the following great open-source repos:
+- https://github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/
+incubator-mxnet/blob/master/example/gluon/embedding_learning - https://
+github.com/facebookresearch/deepcluster - https://github.com/geonm/proxy-
+anchor-loss - https://github.com/idstcv/SoftTriple - https://github.com/kunhe/
+FastAP-metric-learning - https://github.com/ronekko/deep_metric_learning -
+https://github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/
+regularface ### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/
+) for designing the logo. ## Citing this library If you'd like to cite pytorch-
+metric-learning in your paper, you can use this bibtex: ```latex @article
+{Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
+and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
+{abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.1.2/README.md` & `pytorch-metric-learning-2.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
 | [yutanakamura-tky](https://github.com/yutanakamura-tky) | |
 | [KinglittleQ](https://github.com/KinglittleQ) | |
 | [martin0258](https://github.com/martin0258) | |
 | [michaeldeyzel](https://github.com/michaeldeyzel) | |
 | [HSinger04](https://github.com/HSinger04) | |
+| [rheum](https://github.com/rheum) | |
 
 
 
 ### Facebook AI
 Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This project began during my internship at Facebook AI where I received valuable feedback from Ser-Nam, and his team of computer vision and machine learning engineers and research scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its early stages of development.
 
 ### Open-source repos
```

#### html2text {}

```diff
@@ -170,29 +170,30 @@
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
 [michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
-github.com/HSinger04) | | ### Facebook AI Thank you to [Ser-Nam Lim](https://
-research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/
-), and my research advisor, [Professor Serge Belongie](https://
-vision.cornell.edu/se3/people/serge-belongie/). This project began during my
-internship at Facebook AI where I received valuable feedback from Ser-Nam, and
-his team of computer vision and machine learning engineers and research
-scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/
-ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-
-3962aa7/) for reviewing my code during its early stages of development. ###
-Open-source repos This library contains code that has been adapted and modified
-from the following great open-source repos: - https://github.com/bnu-wangxun/
-Deep_Metric - https://github.com/chaoyuaw/incubator-mxnet/blob/master/example/
-gluon/embedding_learning - https://github.com/facebookresearch/deepcluster -
-https://github.com/geonm/proxy-anchor-loss - https://github.com/idstcv/
-SoftTriple - https://github.com/kunhe/FastAP-metric-learning - https://
-github.com/ronekko/deep_metric_learning - https://github.com/tjddus9597/Proxy-
-Anchor-CVPR2020 - http://kaizhao.net/regularface ### Logo Thanks to [Jeff
-Musgrave](https://www.designgenius.ca/) for designing the logo. ## Citing this
-library If you'd like to cite pytorch-metric-learning in your paper, you can
-use this bibtex: ```latex @article{Musgrave2020PyTorchML, title={PyTorch Metric
-Learning}, author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
-journal={ArXiv}, year={2020}, volume={abs/2008.09164} } ```
+github.com/HSinger04) | | | [rheum](https://github.com/rheum) | | ### Facebook
+AI Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at
+[Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor
+Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This
+project began during my internship at Facebook AI where I received valuable
+feedback from Ser-Nam, and his team of computer vision and machine learning
+engineers and research scientists. In particular, thanks to [Ashish Shah]
+(https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://
+www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its
+early stages of development. ### Open-source repos This library contains code
+that has been adapted and modified from the following great open-source repos:
+- https://github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/
+incubator-mxnet/blob/master/example/gluon/embedding_learning - https://
+github.com/facebookresearch/deepcluster - https://github.com/geonm/proxy-
+anchor-loss - https://github.com/idstcv/SoftTriple - https://github.com/kunhe/
+FastAP-metric-learning - https://github.com/ronekko/deep_metric_learning -
+https://github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/
+regularface ### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/
+) for designing the logo. ## Citing this library If you'd like to cite pytorch-
+metric-learning in your paper, you can use this bibtex: ```latex @article
+{Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
+and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
+{abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.1.2/setup.py` & `pytorch-metric-learning-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/base_distance.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/base_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/batched_distance.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/batched_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/lp_distance.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/lp_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/distances/snr_distance.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/distances/snr_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/__init__.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from .cross_batch_memory import CrossBatchMemory
 from .fast_ap_loss import FastAPLoss
 from .generic_pair_loss import GenericPairLoss
 from .instance_loss import InstanceLoss
 from .intra_pair_variance_loss import IntraPairVarianceLoss
 from .large_margin_softmax_loss import LargeMarginSoftmaxLoss
 from .lifted_structure_loss import GeneralizedLiftedStructureLoss, LiftedStructureLoss
+from .manifold_loss import ManifoldLoss
 from .margin_loss import MarginLoss
 from .mixins import EmbeddingRegularizerMixin, WeightRegularizerMixin
 from .multi_similarity_loss import MultiSimilarityLoss
 from .multiple_losses import MultipleLosses
 from .n_pairs_loss import NPairsLoss
 from .nca_loss import NCALoss
 from .normalized_softmax_loss import NormalizedSoftmaxLoss
 from .ntxent_loss import NTXentLoss
+from .p2s_grad_loss import P2SGradLoss
 from .pnp_loss import PNPLoss
 from .proxy_anchor_loss import ProxyAnchorLoss
 from .proxy_losses import ProxyNCALoss
 from .self_supervised_loss import SelfSupervisedLoss
 from .signal_to_noise_ratio_losses import SignalToNoiseRatioContrastiveLoss
 from .soft_triple_loss import SoftTripleLoss
 from .sphereface_loss import SphereFaceLoss
```

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/angular_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/angular_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/arcface_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/base_metric_loss_function.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/base_metric_loss_function.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/circle_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/circle_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/contrastive_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cosface_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cosface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/cross_batch_memory.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/cross_batch_memory.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/fast_ap_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/fast_ap_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/generic_pair_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/generic_pair_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/instance_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/instance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/intra_pair_variance_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/large_margin_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/lifted_structure_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/lifted_structure_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/margin_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/mixins.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multi_similarity_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multi_similarity_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/multiple_losses.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/multiple_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/n_pairs_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/n_pairs_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/nca_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/nca_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/normalized_softmax_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/normalized_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/ntxent_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/ntxent_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/pnp_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/pnp_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_anchor_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_anchor_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/proxy_losses.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/proxy_losses.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/self_supervised_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/self_supervised_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
         loss_fn = SelfSupervisedLoss(TripletMarginLoss())
         loss = loss_fn(embeddings, ref_emb1, ref_emb2, ...)
 
     where ref_embk = kth augmentation of embeddings.
     """
 
-    def __init__(self, loss, **kwargs):
+    def __init__(self, loss, symmetric=True, **kwargs):
         super().__init__(loss=loss, **kwargs)
         self.loss = loss
+        self.symmetric = symmetric
 
     @staticmethod
     def supported_losses():
         return [
             "AngularLoss",
             "CircleLoss",
             "ContrastiveLoss",
@@ -50,13 +51,17 @@
         embeddings: representations of the original set of inputs
         ref_emb:    representations of an augmentation of the inputs.
         *args:      variable length argument list, where each argument
                     is an additional representation of an augmented version of the input.
                     i.e. ref_emb2, ref_emb3, ...
         """
         labels = torch.arange(embeddings.shape[0])
+        if self.symmetric:
+            embeddings = torch.cat([embeddings, ref_emb], dim=0)
+            labels = torch.cat([labels, labels], dim=0)
+            return self.loss(embeddings, labels)
         return self.loss(
             embeddings=embeddings,
             labels=labels,
             ref_emb=ref_emb,
             ref_labels=labels.clone(),
         )
```

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/soft_triple_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/soft_triple_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/subcenter_arcface_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/supcon_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/supcon_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/triplet_margin_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/triplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/tuplet_margin_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/tuplet_margin_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/losses/vicreg_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/losses/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/__init__.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/angular_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/angular_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/base_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/base_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/batch_easy_hard_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/distance_weighted_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/distance_weighted_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/hdc_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/hdc_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/multi_similarity_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/multi_similarity_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/pair_margin_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/pair_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/triplet_margin_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/triplet_margin_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/miners/uniform_histogram_miner.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/miners/uniform_histogram_miner.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/base_reducer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/base_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/class_weighted_reducer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/class_weighted_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/divisor_reducer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/divisor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/multiple_reducers.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/multiple_reducers.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/per_anchor_reducer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/per_anchor_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/reducers/threshold_reducer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/reducers/threshold_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/center_invariant_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/lp_regularizer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/lp_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/regular_face_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/regularizers/sparse_centers_regularizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/fixed_set_of_triplets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/hierarchical_sampler.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/hierarchical_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,17 @@
         self,
     ):
         return len(self.batches)
 
     def reshuffle(self):
         batches = []
         for combinations in self.super_pairs:
-
             for b in range(self.batches_per_super_tuple):
-
                 batch = []
                 for slb in combinations:
-
                     sub_batch = []
                     all_classes = list(self.super_image_lists[slb].keys())
                     c_f.NUMPY_RANDOM.shuffle(all_classes)
                     for cl in all_classes:
                         if len(sub_batch) >= self.sub_batch_len:
                             break
                         instances = self.super_image_lists[slb][cl]
```

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/m_per_class_sampler.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/m_per_class_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/samplers/tuples_to_weights_sampler.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/base_tester.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/base_tester.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_embedding_space.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/global_twostream_embedding_space.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/testers/with_same_parent_label.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/testers/with_same_parent_label.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/base_trainer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/base_trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/cascaded_embeddings.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/cascaded_embeddings.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/deep_adversarial_metric_learning.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/metric_loss_only.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/metric_loss_only.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/train_with_classifier.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/train_with_classifier.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/trainers/twostream_metric_loss.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/trainers/twostream_metric_loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/accuracy_calculator.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/accuracy_calculator.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/common_functions.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/distributed.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/inference.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/inference.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/key_checker.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/key_checker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/logging_presets.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/logging_presets.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_and_miner_utils.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_and_miner_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/loss_tracker.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/loss_tracker.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning/utils/module_with_records_and_reducer.py`

 * *Files identical despite different names*

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/PKG-INFO` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pytorch-metric-learning
-Version: 2.1.2
+Version: 2.2.0
 Summary: The easiest way to use deep metric learning in your application. Modular, flexible, and extensible. Written in PyTorch.
 Home-page: https://github.com/KevinMusgrave/pytorch-metric-learning
 Author: Kevin Musgrave
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: with-hooks
 Provides-Extra: with-hooks-cpu
@@ -270,14 +268,15 @@
 | [JoOkuma](https://github.com/JoOkuma) | |
 | [gkouros](https://github.com/gkouros) | |
 | [yutanakamura-tky](https://github.com/yutanakamura-tky) | |
 | [KinglittleQ](https://github.com/KinglittleQ) | |
 | [martin0258](https://github.com/martin0258) | |
 | [michaeldeyzel](https://github.com/michaeldeyzel) | |
 | [HSinger04](https://github.com/HSinger04) | |
+| [rheum](https://github.com/rheum) | |
 
 
 
 ### Facebook AI
 Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This project began during my internship at Facebook AI where I received valuable feedback from Ser-Nam, and his team of computer vision and machine learning engineers and research scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its early stages of development.
 
 ### Open-source repos
@@ -302,9 +301,7 @@
   title={PyTorch Metric Learning},
   author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
   journal={ArXiv},
   year={2020},
   volume={abs/2008.09164}
 }
 ```
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.1.2 Summary: The
+Metadata-Version: 2.1 Name: pytorch-metric-learning Version: 2.2.0 Summary: The
 easiest way to use deep metric learning in your application. Modular, flexible,
 and extensible. Written in PyTorch. Home-page: https://github.com/
-KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave License: UNKNOWN
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.0 Description-Content-Type: text/markdown
-Provides-Extra: with-hooks Provides-Extra: with-hooks-cpu Provides-Extra: docs
-Provides-Extra: dev License-File: LICENSE
+KevinMusgrave/pytorch-metric-learning Author: Kevin Musgrave Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.0
+Description-Content-Type: text/markdown Provides-Extra: with-hooks Provides-
+Extra: with-hooks-cpu Provides-Extra: docs Provides-Extra: dev License-File:
+LICENSE
 ****** [PyTorch_Metric_Learning] ******
                        [PyPi_version] [Anaconda_version]
 ## News **April 5**: v2.1.0 - Added [PNPLoss](https://kevinmusgrave.github.io/
 pytorch-metric-learning/losses/#pnploss) - Thanks to contributor
 [interestingzhuo](https://github.com/interestingzhuo). **January 29**: v2.0.0 -
 Added SelfSupervisedLoss, plus various API improvements. See the [release
 notes](https://github.com/KevinMusgrave/pytorch-metric-learning/releases/tag/
@@ -179,29 +179,30 @@
 github.com/z1w) | | | [thinline72](https://github.com/thinline72) | | |
 [tpanum](https://github.com/tpanum) | | | [fralik](https://github.com/fralik) |
 | | [joaqo](https://github.com/joaqo) | | | [JoOkuma](https://github.com/
 JoOkuma) | | | [gkouros](https://github.com/gkouros) | | | [yutanakamura-tky]
 (https://github.com/yutanakamura-tky) | | | [KinglittleQ](https://github.com/
 KinglittleQ) | | | [martin0258](https://github.com/martin0258) | | |
 [michaeldeyzel](https://github.com/michaeldeyzel) | | | [HSinger04](https://
-github.com/HSinger04) | | ### Facebook AI Thank you to [Ser-Nam Lim](https://
-research.fb.com/people/lim-ser-nam/) at [Facebook AI](https://ai.facebook.com/
-), and my research advisor, [Professor Serge Belongie](https://
-vision.cornell.edu/se3/people/serge-belongie/). This project began during my
-internship at Facebook AI where I received valuable feedback from Ser-Nam, and
-his team of computer vision and machine learning engineers and research
-scientists. In particular, thanks to [Ashish Shah](https://www.linkedin.com/in/
-ashish217/) and [Austin Reiter](https://www.linkedin.com/in/austin-reiter-
-3962aa7/) for reviewing my code during its early stages of development. ###
-Open-source repos This library contains code that has been adapted and modified
-from the following great open-source repos: - https://github.com/bnu-wangxun/
-Deep_Metric - https://github.com/chaoyuaw/incubator-mxnet/blob/master/example/
-gluon/embedding_learning - https://github.com/facebookresearch/deepcluster -
-https://github.com/geonm/proxy-anchor-loss - https://github.com/idstcv/
-SoftTriple - https://github.com/kunhe/FastAP-metric-learning - https://
-github.com/ronekko/deep_metric_learning - https://github.com/tjddus9597/Proxy-
-Anchor-CVPR2020 - http://kaizhao.net/regularface ### Logo Thanks to [Jeff
-Musgrave](https://www.designgenius.ca/) for designing the logo. ## Citing this
-library If you'd like to cite pytorch-metric-learning in your paper, you can
-use this bibtex: ```latex @article{Musgrave2020PyTorchML, title={PyTorch Metric
-Learning}, author={Kevin Musgrave and Serge J. Belongie and Ser-Nam Lim},
-journal={ArXiv}, year={2020}, volume={abs/2008.09164} } ```
+github.com/HSinger04) | | | [rheum](https://github.com/rheum) | | ### Facebook
+AI Thank you to [Ser-Nam Lim](https://research.fb.com/people/lim-ser-nam/) at
+[Facebook AI](https://ai.facebook.com/), and my research advisor, [Professor
+Serge Belongie](https://vision.cornell.edu/se3/people/serge-belongie/). This
+project began during my internship at Facebook AI where I received valuable
+feedback from Ser-Nam, and his team of computer vision and machine learning
+engineers and research scientists. In particular, thanks to [Ashish Shah]
+(https://www.linkedin.com/in/ashish217/) and [Austin Reiter](https://
+www.linkedin.com/in/austin-reiter-3962aa7/) for reviewing my code during its
+early stages of development. ### Open-source repos This library contains code
+that has been adapted and modified from the following great open-source repos:
+- https://github.com/bnu-wangxun/Deep_Metric - https://github.com/chaoyuaw/
+incubator-mxnet/blob/master/example/gluon/embedding_learning - https://
+github.com/facebookresearch/deepcluster - https://github.com/geonm/proxy-
+anchor-loss - https://github.com/idstcv/SoftTriple - https://github.com/kunhe/
+FastAP-metric-learning - https://github.com/ronekko/deep_metric_learning -
+https://github.com/tjddus9597/Proxy-Anchor-CVPR2020 - http://kaizhao.net/
+regularface ### Logo Thanks to [Jeff Musgrave](https://www.designgenius.ca/
+) for designing the logo. ## Citing this library If you'd like to cite pytorch-
+metric-learning in your paper, you can use this bibtex: ```latex @article
+{Musgrave2020PyTorchML, title={PyTorch Metric Learning}, author={Kevin Musgrave
+and Serge J. Belongie and Ser-Nam Lim}, journal={ArXiv}, year={2020}, volume=
+{abs/2008.09164} } ```
```

### Comparing `pytorch-metric-learning-2.1.2/src/pytorch_metric_learning.egg-info/SOURCES.txt` & `pytorch-metric-learning-2.2.0/src/pytorch_metric_learning.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,24 @@
 src/pytorch_metric_learning/losses/cross_batch_memory.py
 src/pytorch_metric_learning/losses/fast_ap_loss.py
 src/pytorch_metric_learning/losses/generic_pair_loss.py
 src/pytorch_metric_learning/losses/instance_loss.py
 src/pytorch_metric_learning/losses/intra_pair_variance_loss.py
 src/pytorch_metric_learning/losses/large_margin_softmax_loss.py
 src/pytorch_metric_learning/losses/lifted_structure_loss.py
+src/pytorch_metric_learning/losses/manifold_loss.py
 src/pytorch_metric_learning/losses/margin_loss.py
 src/pytorch_metric_learning/losses/mixins.py
 src/pytorch_metric_learning/losses/multi_similarity_loss.py
 src/pytorch_metric_learning/losses/multiple_losses.py
 src/pytorch_metric_learning/losses/n_pairs_loss.py
 src/pytorch_metric_learning/losses/nca_loss.py
 src/pytorch_metric_learning/losses/normalized_softmax_loss.py
 src/pytorch_metric_learning/losses/ntxent_loss.py
+src/pytorch_metric_learning/losses/p2s_grad_loss.py
 src/pytorch_metric_learning/losses/pnp_loss.py
 src/pytorch_metric_learning/losses/proxy_anchor_loss.py
 src/pytorch_metric_learning/losses/proxy_losses.py
 src/pytorch_metric_learning/losses/self_supervised_loss.py
 src/pytorch_metric_learning/losses/signal_to_noise_ratio_losses.py
 src/pytorch_metric_learning/losses/soft_triple_loss.py
 src/pytorch_metric_learning/losses/sphereface_loss.py
```

