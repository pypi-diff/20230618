# Comparing `tmp/lmqg-0.1.0.tar.gz` & `tmp/lmqg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmqg-0.1.0.tar", last modified: Fri May 12 17:50:07 2023, max compression
+gzip compressed data, was "lmqg-0.1.1.tar", last modified: Sun Jun 18 21:20:41 2023, max compression
```

## Comparing `lmqg-0.1.0.tar` & `lmqg-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.623651 lmqg-0.1.0/
--rw-r--r--   0 asahi      (501) staff       (20)    19917 2021-10-29 09:59:07.000000 lmqg-0.1.0/LICENSE
--rw-r--r--   0 asahi      (501) staff       (20)    16475 2023-05-12 17:50:07.623802 lmqg-0.1.0/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)    15679 2023-05-12 17:49:30.000000 lmqg-0.1.0/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.589243 lmqg-0.1.0/lmqg/
--rw-r--r--   0 asahi      (501) staff       (20)      382 2023-02-22 13:09:46.000000 lmqg-0.1.0/lmqg/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    12897 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/automatic_evaluation.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.600200 lmqg-0.1.0/lmqg/automatic_evaluation_tool/
--rw-r--r--   0 asahi      (501) staff       (20)      256 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/__init__.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.605095 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/
--rw-r--r--   0 asahi      (501) staff       (20)       66 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    11181 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/score.py
--rw-r--r--   0 asahi      (501) staff       (20)    11657 2022-09-03 23:52:23.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/scorer.py
--rw-r--r--   0 asahi      (501) staff       (20)    29393 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/utils.py
--rw-r--r--   0 asahi      (501) staff       (20)      732 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bertscore.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.608409 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/
--rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2155 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu.py
--rwxr-xr-x   0 asahi      (501) staff       (20)     8721 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.610530 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/
--rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/__init__.py
--rwxr-xr-x   0 asahi      (501) staff       (20)     7124 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/meteor.py
--rw-r--r--   0 asahi      (501) staff       (20)      840 2023-02-26 10:57:31.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor.py
--rw-r--r--   0 asahi      (501) staff       (20)     6909 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/moverscore.py
--rw-r--r--   0 asahi      (501) staff       (20)     3748 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py
--rwxr-xr-x   0 asahi      (501) staff       (20)     4510 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/rouge.py
--rw-r--r--   0 asahi      (501) staff       (20)      884 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/text_normalization.py
--rw-r--r--   0 asahi      (501) staff       (20)     2747 2022-12-05 11:07:21.000000 lmqg-0.1.0/lmqg/data.py
--rw-r--r--   0 asahi      (501) staff       (20)     1018 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/exceptions.py
--rw-r--r--   0 asahi      (501) staff       (20)    16244 2023-02-22 13:09:46.000000 lmqg-0.1.0/lmqg/grid_searcher.py
--rw-r--r--   0 asahi      (501) staff       (20)     7082 2023-02-22 13:09:46.000000 lmqg-0.1.0/lmqg/inference_api.py
--rw-r--r--   0 asahi      (501) staff       (20)    35965 2023-03-15 21:59:59.000000 lmqg-0.1.0/lmqg/language_model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.616950 lmqg-0.1.0/lmqg/lmqg_cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-09-03 23:52:23.000000 lmqg-0.1.0/lmqg/lmqg_cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     3645 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation.py
--rw-r--r--   0 asahi      (501) staff       (20)     5582 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)     4648 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py
--rw-r--r--   0 asahi      (501) staff       (20)     9719 2023-03-06 13:07:50.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qag.py
--rw-r--r--   0 asahi      (501) staff       (20)     7295 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_finetuning.py
--rw-r--r--   0 asahi      (501) staff       (20)     1913 2023-03-06 12:09:53.000000 lmqg-0.1.0/lmqg/lmqg_cl/push_to_hf.py
--rw-r--r--   0 asahi      (501) staff       (20)    61040 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/lmqg_cl/readme_template.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.622685 lmqg-0.1.0/lmqg/qa_evaluation_tool/
--rw-r--r--   0 asahi      (501) staff       (20)       93 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     3999 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py
--rwxr-xr-x   0 asahi      (501) staff       (20)    22361 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/run_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)     4741 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/trainer_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)    22310 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/utils_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)     3102 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/spacy_module.py
--rw-r--r--   0 asahi      (501) staff       (20)    12421 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/trainer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.592882 lmqg-0.1.0/lmqg.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)    16475 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     1624 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)      516 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/entry_points.txt
--rw-r--r--   0 asahi      (501) staff       (20)      279 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        5 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-12 17:50:07.624288 lmqg-0.1.0/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     2900 2023-05-12 17:50:04.000000 lmqg-0.1.0/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.048549 lmqg-0.1.1/
+-rw-r--r--   0 asahi      (501) staff       (20)    19917 2021-10-29 09:59:07.000000 lmqg-0.1.1/LICENSE
+-rw-r--r--   0 asahi      (501) staff       (20)    16528 2023-06-18 21:20:41.048861 lmqg-0.1.1/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)    15732 2023-06-01 12:11:24.000000 lmqg-0.1.1/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.018870 lmqg-0.1.1/lmqg/
+-rw-r--r--   0 asahi      (501) staff       (20)      382 2023-02-22 13:09:46.000000 lmqg-0.1.1/lmqg/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    12897 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/automatic_evaluation.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.026954 lmqg-0.1.1/lmqg/automatic_evaluation_tool/
+-rw-r--r--   0 asahi      (501) staff       (20)      256 2022-12-04 12:31:54.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/__init__.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.030758 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/
+-rw-r--r--   0 asahi      (501) staff       (20)       66 2022-05-20 15:17:04.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    11181 2022-05-20 15:17:04.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/score.py
+-rw-r--r--   0 asahi      (501) staff       (20)    11657 2022-09-03 23:52:23.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/scorer.py
+-rw-r--r--   0 asahi      (501) staff       (20)    29393 2022-05-20 15:17:04.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/utils.py
+-rw-r--r--   0 asahi      (501) staff       (20)      732 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bertscore.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.033488 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bleu/
+-rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bleu/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2155 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bleu/bleu.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)     8721 2022-02-18 17:28:54.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.035481 lmqg-0.1.1/lmqg/automatic_evaluation_tool/meteor/
+-rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/meteor/__init__.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)     7124 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/meteor/meteor.py
+-rw-r--r--   0 asahi      (501) staff       (20)      840 2023-02-26 10:57:31.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/meteor.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6909 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/moverscore.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3748 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)     4510 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/rouge.py
+-rw-r--r--   0 asahi      (501) staff       (20)      884 2022-02-18 17:28:54.000000 lmqg-0.1.1/lmqg/automatic_evaluation_tool/text_normalization.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2747 2022-12-05 11:07:21.000000 lmqg-0.1.1/lmqg/data.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1018 2022-05-20 15:17:04.000000 lmqg-0.1.1/lmqg/exceptions.py
+-rw-r--r--   0 asahi      (501) staff       (20)    16244 2023-02-22 13:09:46.000000 lmqg-0.1.1/lmqg/grid_searcher.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7082 2023-02-22 13:09:46.000000 lmqg-0.1.1/lmqg/inference_api.py
+-rw-r--r--   0 asahi      (501) staff       (20)    35965 2023-03-15 21:59:59.000000 lmqg-0.1.1/lmqg/language_model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.041426 lmqg-0.1.1/lmqg/lmqg_cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-09-03 23:52:23.000000 lmqg-0.1.1/lmqg/lmqg_cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3645 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5582 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4648 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py
+-rw-r--r--   0 asahi      (501) staff       (20)     9719 2023-03-06 13:07:50.000000 lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation_qag.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7295 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/lmqg_cl/model_finetuning.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1913 2023-03-06 12:09:53.000000 lmqg-0.1.1/lmqg/lmqg_cl/push_to_hf.py
+-rw-r--r--   0 asahi      (501) staff       (20)    61040 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/lmqg_cl/readme_template.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.047224 lmqg-0.1.1/lmqg/qa_evaluation_tool/
+-rw-r--r--   0 asahi      (501) staff       (20)       93 2022-12-04 12:31:54.000000 lmqg-0.1.1/lmqg/qa_evaluation_tool/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3999 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)    22361 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/qa_evaluation_tool/run_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4741 2022-12-04 12:31:54.000000 lmqg-0.1.1/lmqg/qa_evaluation_tool/trainer_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)    22310 2022-12-04 12:31:54.000000 lmqg-0.1.1/lmqg/qa_evaluation_tool/utils_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3102 2023-02-04 14:23:33.000000 lmqg-0.1.1/lmqg/spacy_module.py
+-rw-r--r--   0 asahi      (501) staff       (20)    12421 2023-02-12 10:54:29.000000 lmqg-0.1.1/lmqg/trainer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-18 21:20:41.021517 lmqg-0.1.1/lmqg.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)    16528 2023-06-18 21:20:40.000000 lmqg-0.1.1/lmqg.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     1624 2023-06-18 21:20:40.000000 lmqg-0.1.1/lmqg.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-06-18 21:20:40.000000 lmqg-0.1.1/lmqg.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)      516 2023-06-18 21:20:40.000000 lmqg-0.1.1/lmqg.egg-info/entry_points.txt
+-rw-r--r--   0 asahi      (501) staff       (20)      279 2023-06-18 21:20:40.000000 lmqg-0.1.1/lmqg.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        5 2023-06-18 21:20:40.000000 lmqg-0.1.1/lmqg.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-06-18 21:20:41.049826 lmqg-0.1.1/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     2917 2023-06-18 21:20:28.000000 lmqg-0.1.1/setup.py
```

### Comparing `lmqg-0.1.0/LICENSE` & `lmqg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/PKG-INFO` & `lmqg-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmqg
-Version: 0.1.0
+Version: 0.1.1
 Summary: Language Model for Question Generation.
 Home-page: https://github.com/asahi417/lm-question-generation
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.1.0.tar.gz
+Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.1.1.tar.gz
 Keywords: language model,question-answering,question-generation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -36,27 +36,27 @@
 paragraph-level QAG, where user will provide a context (paragraph or document), and the model will generate a list of 
 question and answer pairs on the context. With `lmqg`, you can do following things:
 - [***Generation in One Line of Code:***](https://github.com/asahi417/lm-question-generation#generate-question--answer) Generate questions and answers in *8* languages (en/fr/ja/ko/ru/it/es/de).
 - [***Model Training/Evaluation:***](https://github.com/asahi417/lm-question-generation#model-development) Train & evaluate your own QG/QAG models.
 - [***QAG & QG Model Hosting:***](https://github.com/asahi417/lm-question-generation#rest-api-with-huggingface-inference-api) Host your QAG models on a web application or a restAPI server.
 - [***AutoQG:***](https://github.com/asahi417/lm-question-generation/tree/master#autoqg) Online web service to generate questions and answers with our models.
  
-***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://asahiushio.com/files/paper_2023_acl_qag.pdf), [LMQG at system demonstration](https://asahiushio.com/files/paper_2023_acl_demo.pdf)). \
+***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://arxiv.org/abs/2305.17002), [LMQG at system demonstration](https://arxiv.org/abs/2305.17416)). \
 ***Update Oct 2022:*** Our [QG paper](https://aclanthology.org/2022.emnlp-main.42/) got accepted by EMNLP main 2022.
 
 ### A bit more about QAG models 📝
 Our QAG models can be grouped into three types: **Pipeline**, **Multitask**, 
 and **End2end** (see Figure 1). The **Pipeline** consists of question generation (QG) and answer extraction (AE) models independently,
 where AE will parse all the sentences in the context to extract answers, and QG will generate questions on the answers.
 The **Multitask** follows same architecture as the **Pipeline**, but the QG and AE models are shared model fine-tuned jointly.
 Finally, **End2end** model will generate a list of question and answer pairs in an end-to-end manner.
 In practice, **Pipeline** and **Multitask** generate more question and answer pairs, while **End2end** generates less but a few times faster, 
 and the quality of the generated question and answer pairs depend on language.
 All types are available in the *8* diverse languages (en/fr/ja/ko/ru/it/es/de) via `lmqg`, and the models are all shared on HuggingFace (see the [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md)).
-To know more about QAG, please check [our ACL 2023 paper](https://asahiushio.com/files/paper_2023_acl_qag.pdf) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
+To know more about QAG, please check [our ACL 2023 paper](https://arxiv.org/abs/2305.17002) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
 
 ### Is QAG different from Question Generation (QG)? 🤔
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/example.png" width="700">
   <br><em> Figure 2: An example of QAG (a) and QG (b). </em>
 </p>
@@ -87,15 +87,18 @@
 ```python
 from pprint import pprint
 from lmqg import TransformersQG
 
 # initialize model
 model = TransformersQG('lmqg/t5-base-squad-qag') # or TransformersQG(model='lmqg/t5-base-squad-qg-ae') 
 # paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known " \
+          "as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, " \
+          "J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his " \
+          "best known pictures is a view of the city of Oxford from Hinksey Hill."
 # model prediction
 question_answer = model.generate_qa(context)
 # the output is a list of tuple (question, answer)
 pprint(question_answer)
 [
     ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
     ('What is William Turner often known as?', 'William Turner of Oxford or just Turner of Oxford'),
@@ -111,15 +114,18 @@
 ```python
 from pprint import pprint
 from lmqg import TransformersQG
 
 # initialize model
 model = TransformersQG(model='lmqg/t5-base-squad-qg', model_ae='lmqg/t5-base-squad-ae')  
 # paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known " \
+          "as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, " \
+          "J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his " \
+          "best known pictures is a view of the city of Oxford from Hinksey Hill."
 # model prediction
 question_answer = model.generate_qa(context)
 # the output is a list of tuple (question, answer)
 pprint(question_answer)
 [
     ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
     ('What is another name for William Turner?', 'William Turner of Oxford'),
@@ -287,34 +293,34 @@
     month = dec,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
 
-- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2022 Finding***](https://asahiushio.com/files/paper_2023_acl_qag.pdf): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2023, Finding***](https://arxiv.org/abs/2305.17002): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
 ```
-@inproceedings{ushio-etal-2023-tba,
-    title = "TBA",
+@inproceedings{ushio-etal-2023-an-empirical,
+    title = "An Empirical Comparison of LM-based Question and Answer Generation Methods",
     author = "Ushio, Asahi  and
         Alva-Manchego, Fernando  and
         Camacho-Collados, Jose",
-    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: Findings",
     month = Jul,
     year = "2023",
     address = "Toronto, Canada",
     publisher = "Association for Computational Linguistics",
 }
 ```
 
-- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration***](https://asahiushio.com/files/paper_2023_acl_demo.pdf): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2023, System Demonstration***](https://arxiv.org/abs/2305.17416): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
 
 ```
-@inproceedings{ushio-etal-2023-a-practical-toolkit
-    title = "A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration",
+@inproceedings{ushio-etal-2023-a-practical-toolkit,
+    title = "A Practical Toolkit for Multilingual Question and Answer Generation",
     author = "Ushio, Asahi  and
         Alva-Manchego, Fernando  and
         Camacho-Collados, Jose",
     booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
     month = Jul,
     year = "2023",
     address = "Toronto, Canada",
```

### Comparing `lmqg-0.1.0/README.md` & `lmqg-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 paragraph-level QAG, where user will provide a context (paragraph or document), and the model will generate a list of 
 question and answer pairs on the context. With `lmqg`, you can do following things:
 - [***Generation in One Line of Code:***](https://github.com/asahi417/lm-question-generation#generate-question--answer) Generate questions and answers in *8* languages (en/fr/ja/ko/ru/it/es/de).
 - [***Model Training/Evaluation:***](https://github.com/asahi417/lm-question-generation#model-development) Train & evaluate your own QG/QAG models.
 - [***QAG & QG Model Hosting:***](https://github.com/asahi417/lm-question-generation#rest-api-with-huggingface-inference-api) Host your QAG models on a web application or a restAPI server.
 - [***AutoQG:***](https://github.com/asahi417/lm-question-generation/tree/master#autoqg) Online web service to generate questions and answers with our models.
  
-***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://asahiushio.com/files/paper_2023_acl_qag.pdf), [LMQG at system demonstration](https://asahiushio.com/files/paper_2023_acl_demo.pdf)). \
+***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://arxiv.org/abs/2305.17002), [LMQG at system demonstration](https://arxiv.org/abs/2305.17416)). \
 ***Update Oct 2022:*** Our [QG paper](https://aclanthology.org/2022.emnlp-main.42/) got accepted by EMNLP main 2022.
 
 ### A bit more about QAG models 📝
 Our QAG models can be grouped into three types: **Pipeline**, **Multitask**, 
 and **End2end** (see Figure 1). The **Pipeline** consists of question generation (QG) and answer extraction (AE) models independently,
 where AE will parse all the sentences in the context to extract answers, and QG will generate questions on the answers.
 The **Multitask** follows same architecture as the **Pipeline**, but the QG and AE models are shared model fine-tuned jointly.
 Finally, **End2end** model will generate a list of question and answer pairs in an end-to-end manner.
 In practice, **Pipeline** and **Multitask** generate more question and answer pairs, while **End2end** generates less but a few times faster, 
 and the quality of the generated question and answer pairs depend on language.
 All types are available in the *8* diverse languages (en/fr/ja/ko/ru/it/es/de) via `lmqg`, and the models are all shared on HuggingFace (see the [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md)).
-To know more about QAG, please check [our ACL 2023 paper](https://asahiushio.com/files/paper_2023_acl_qag.pdf) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
+To know more about QAG, please check [our ACL 2023 paper](https://arxiv.org/abs/2305.17002) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
 
 ### Is QAG different from Question Generation (QG)? 🤔
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/example.png" width="700">
   <br><em> Figure 2: An example of QAG (a) and QG (b). </em>
 </p>
@@ -65,15 +65,18 @@
 ```python
 from pprint import pprint
 from lmqg import TransformersQG
 
 # initialize model
 model = TransformersQG('lmqg/t5-base-squad-qag') # or TransformersQG(model='lmqg/t5-base-squad-qg-ae') 
 # paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known " \
+          "as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, " \
+          "J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his " \
+          "best known pictures is a view of the city of Oxford from Hinksey Hill."
 # model prediction
 question_answer = model.generate_qa(context)
 # the output is a list of tuple (question, answer)
 pprint(question_answer)
 [
     ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
     ('What is William Turner often known as?', 'William Turner of Oxford or just Turner of Oxford'),
@@ -89,15 +92,18 @@
 ```python
 from pprint import pprint
 from lmqg import TransformersQG
 
 # initialize model
 model = TransformersQG(model='lmqg/t5-base-squad-qg', model_ae='lmqg/t5-base-squad-ae')  
 # paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known " \
+          "as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, " \
+          "J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his " \
+          "best known pictures is a view of the city of Oxford from Hinksey Hill."
 # model prediction
 question_answer = model.generate_qa(context)
 # the output is a list of tuple (question, answer)
 pprint(question_answer)
 [
     ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
     ('What is another name for William Turner?', 'William Turner of Oxford'),
@@ -265,34 +271,34 @@
     month = dec,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
 
-- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2022 Finding***](https://asahiushio.com/files/paper_2023_acl_qag.pdf): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2023, Finding***](https://arxiv.org/abs/2305.17002): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
 ```
-@inproceedings{ushio-etal-2023-tba,
-    title = "TBA",
+@inproceedings{ushio-etal-2023-an-empirical,
+    title = "An Empirical Comparison of LM-based Question and Answer Generation Methods",
     author = "Ushio, Asahi  and
         Alva-Manchego, Fernando  and
         Camacho-Collados, Jose",
-    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: Findings",
     month = Jul,
     year = "2023",
     address = "Toronto, Canada",
     publisher = "Association for Computational Linguistics",
 }
 ```
 
-- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration***](https://asahiushio.com/files/paper_2023_acl_demo.pdf): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2023, System Demonstration***](https://arxiv.org/abs/2305.17416): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
 
 ```
-@inproceedings{ushio-etal-2023-a-practical-toolkit
-    title = "A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration",
+@inproceedings{ushio-etal-2023-a-practical-toolkit,
+    title = "A Practical Toolkit for Multilingual Question and Answer Generation",
     author = "Ushio, Asahi  and
         Alva-Manchego, Fernando  and
         Camacho-Collados, Jose",
     booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
     month = Jul,
     year = "2023",
     address = "Toronto, Canada",
```

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation.py` & `lmqg-0.1.1/lmqg/automatic_evaluation.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/score.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/score.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/scorer.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/scorer.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/utils.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/bert_score/utils.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bertscore.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/bertscore.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/meteor.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/meteor.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/moverscore.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/moverscore.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/rouge.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/rouge.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/automatic_evaluation_tool/text_normalization.py` & `lmqg-0.1.1/lmqg/automatic_evaluation_tool/text_normalization.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/data.py` & `lmqg-0.1.1/lmqg/data.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/exceptions.py` & `lmqg-0.1.1/lmqg/exceptions.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/grid_searcher.py` & `lmqg-0.1.1/lmqg/grid_searcher.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/inference_api.py` & `lmqg-0.1.1/lmqg/inference_api.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/language_model.py` & `lmqg-0.1.1/lmqg/language_model.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation.py` & `lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa.py` & `lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py` & `lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qag.py` & `lmqg-0.1.1/lmqg/lmqg_cl/model_evaluation_qag.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/model_finetuning.py` & `lmqg-0.1.1/lmqg/lmqg_cl/model_finetuning.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/push_to_hf.py` & `lmqg-0.1.1/lmqg/lmqg_cl/push_to_hf.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/lmqg_cl/readme_template.py` & `lmqg-0.1.1/lmqg/lmqg_cl/readme_template.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py` & `lmqg-0.1.1/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/qa_evaluation_tool/run_qa.py` & `lmqg-0.1.1/lmqg/qa_evaluation_tool/run_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/qa_evaluation_tool/trainer_qa.py` & `lmqg-0.1.1/lmqg/qa_evaluation_tool/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/qa_evaluation_tool/utils_qa.py` & `lmqg-0.1.1/lmqg/qa_evaluation_tool/utils_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/spacy_module.py` & `lmqg-0.1.1/lmqg/spacy_module.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg/trainer.py` & `lmqg-0.1.1/lmqg/trainer.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg.egg-info/PKG-INFO` & `lmqg-0.1.1/lmqg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmqg
-Version: 0.1.0
+Version: 0.1.1
 Summary: Language Model for Question Generation.
 Home-page: https://github.com/asahi417/lm-question-generation
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.1.0.tar.gz
+Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.1.1.tar.gz
 Keywords: language model,question-answering,question-generation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -36,27 +36,27 @@
 paragraph-level QAG, where user will provide a context (paragraph or document), and the model will generate a list of 
 question and answer pairs on the context. With `lmqg`, you can do following things:
 - [***Generation in One Line of Code:***](https://github.com/asahi417/lm-question-generation#generate-question--answer) Generate questions and answers in *8* languages (en/fr/ja/ko/ru/it/es/de).
 - [***Model Training/Evaluation:***](https://github.com/asahi417/lm-question-generation#model-development) Train & evaluate your own QG/QAG models.
 - [***QAG & QG Model Hosting:***](https://github.com/asahi417/lm-question-generation#rest-api-with-huggingface-inference-api) Host your QAG models on a web application or a restAPI server.
 - [***AutoQG:***](https://github.com/asahi417/lm-question-generation/tree/master#autoqg) Online web service to generate questions and answers with our models.
  
-***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://asahiushio.com/files/paper_2023_acl_qag.pdf), [LMQG at system demonstration](https://asahiushio.com/files/paper_2023_acl_demo.pdf)). \
+***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://arxiv.org/abs/2305.17002), [LMQG at system demonstration](https://arxiv.org/abs/2305.17416)). \
 ***Update Oct 2022:*** Our [QG paper](https://aclanthology.org/2022.emnlp-main.42/) got accepted by EMNLP main 2022.
 
 ### A bit more about QAG models 📝
 Our QAG models can be grouped into three types: **Pipeline**, **Multitask**, 
 and **End2end** (see Figure 1). The **Pipeline** consists of question generation (QG) and answer extraction (AE) models independently,
 where AE will parse all the sentences in the context to extract answers, and QG will generate questions on the answers.
 The **Multitask** follows same architecture as the **Pipeline**, but the QG and AE models are shared model fine-tuned jointly.
 Finally, **End2end** model will generate a list of question and answer pairs in an end-to-end manner.
 In practice, **Pipeline** and **Multitask** generate more question and answer pairs, while **End2end** generates less but a few times faster, 
 and the quality of the generated question and answer pairs depend on language.
 All types are available in the *8* diverse languages (en/fr/ja/ko/ru/it/es/de) via `lmqg`, and the models are all shared on HuggingFace (see the [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md)).
-To know more about QAG, please check [our ACL 2023 paper](https://asahiushio.com/files/paper_2023_acl_qag.pdf) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
+To know more about QAG, please check [our ACL 2023 paper](https://arxiv.org/abs/2305.17002) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
 
 ### Is QAG different from Question Generation (QG)? 🤔
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/example.png" width="700">
   <br><em> Figure 2: An example of QAG (a) and QG (b). </em>
 </p>
@@ -87,15 +87,18 @@
 ```python
 from pprint import pprint
 from lmqg import TransformersQG
 
 # initialize model
 model = TransformersQG('lmqg/t5-base-squad-qag') # or TransformersQG(model='lmqg/t5-base-squad-qg-ae') 
 # paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known " \
+          "as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, " \
+          "J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his " \
+          "best known pictures is a view of the city of Oxford from Hinksey Hill."
 # model prediction
 question_answer = model.generate_qa(context)
 # the output is a list of tuple (question, answer)
 pprint(question_answer)
 [
     ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
     ('What is William Turner often known as?', 'William Turner of Oxford or just Turner of Oxford'),
@@ -111,15 +114,18 @@
 ```python
 from pprint import pprint
 from lmqg import TransformersQG
 
 # initialize model
 model = TransformersQG(model='lmqg/t5-base-squad-qg', model_ae='lmqg/t5-base-squad-ae')  
 # paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known " \
+          "as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, " \
+          "J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his " \
+          "best known pictures is a view of the city of Oxford from Hinksey Hill."
 # model prediction
 question_answer = model.generate_qa(context)
 # the output is a list of tuple (question, answer)
 pprint(question_answer)
 [
     ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
     ('What is another name for William Turner?', 'William Turner of Oxford'),
@@ -287,34 +293,34 @@
     month = dec,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
 
-- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2022 Finding***](https://asahiushio.com/files/paper_2023_acl_qag.pdf): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2023, Finding***](https://arxiv.org/abs/2305.17002): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
 ```
-@inproceedings{ushio-etal-2023-tba,
-    title = "TBA",
+@inproceedings{ushio-etal-2023-an-empirical,
+    title = "An Empirical Comparison of LM-based Question and Answer Generation Methods",
     author = "Ushio, Asahi  and
         Alva-Manchego, Fernando  and
         Camacho-Collados, Jose",
-    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: Findings",
     month = Jul,
     year = "2023",
     address = "Toronto, Canada",
     publisher = "Association for Computational Linguistics",
 }
 ```
 
-- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration***](https://asahiushio.com/files/paper_2023_acl_demo.pdf): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2023, System Demonstration***](https://arxiv.org/abs/2305.17416): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
 
 ```
-@inproceedings{ushio-etal-2023-a-practical-toolkit
-    title = "A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration",
+@inproceedings{ushio-etal-2023-a-practical-toolkit,
+    title = "A Practical Toolkit for Multilingual Question and Answer Generation",
     author = "Ushio, Asahi  and
         Alva-Manchego, Fernando  and
         Camacho-Collados, Jose",
     booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
     month = Jul,
     year = "2023",
     address = "Toronto, Canada",
```

### Comparing `lmqg-0.1.0/lmqg.egg-info/SOURCES.txt` & `lmqg-0.1.1/lmqg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/lmqg.egg-info/entry_points.txt` & `lmqg-0.1.1/lmqg.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lmqg-0.1.0/setup.py` & `lmqg-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r') as f:
-    readme = f.read()
-VERSION = '0.1.0'
+with open('README.md', 'rb') as f:
+    readme = f.read().decode("UTF-8")
+VERSION = '0.1.1'
 NAME = 'lmqg'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
     packages=find_packages(exclude=['tests', 'misc', 'asset']),
     version=VERSION,
     license=LICENSE,
```

