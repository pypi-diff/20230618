# Comparing `tmp/bugbug-0.0.98.tar.gz` & `tmp/bugbug-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bugbug-0.0.98.tar", last modified: Sat Sep  7 00:01:39 2019, max compression
+gzip compressed data, was "dist/bugbug-0.0.99.tar", last modified: Wed Sep 11 19:20:24 2019, max compression
```

## Comparing `bugbug-0.0.98.tar` & `bugbug-0.0.99.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/
--rw-r--r--   0 root         (0) root         (0)      257 2019-09-07 00:01:38.000000 bugbug-0.0.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      450 2019-09-07 00:01:39.000000 bugbug-0.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5732 2019-09-07 00:01:38.000000 bugbug-0.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2019-09-07 00:01:38.000000 bugbug-0.0.98/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug/
--rw-r--r--   0 root         (0) root         (0)      191 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19764 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/bug_features.py
--rw-r--r--   0 root         (0) root         (0)    29590 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/bug_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     6751 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/bugzilla.py
--rw-r--r--   0 root         (0) root         (0)     8783 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/commit_features.py
--rw-r--r--   0 root         (0) root         (0)     5629 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/db.py
--rw-r--r--   0 root         (0) root         (0)     7055 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/feature_cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug/labels/
--rw-r--r--   0 root         (0) root         (0)     7170 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/bug_nobug.csv
--rw-r--r--   0 root         (0) root         (0)     9467 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/defect_enhancement_task.csv
--rw-r--r--   0 root         (0) root         (0)    36449 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/defect_enhancement_task_e.csv
--rw-r--r--   0 root         (0) root         (0)   173880 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/defect_enhancement_task_h.csv
--rw-r--r--   0 root         (0) root         (0)    36389 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/defect_enhancement_task_p.csv
--rw-r--r--   0 root         (0) root         (0)    12215 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/defect_enhancement_task_s.csv
--rw-r--r--   0 root         (0) root         (0)    43135 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/regression_bug_nobug.csv
--rw-r--r--   0 root         (0) root         (0)     4365 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/regressionrange.csv
--rw-r--r--   0 root         (0) root         (0)     4823 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/str.csv
--rw-r--r--   0 root         (0) root         (0)     1452 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels/tracking.csv
--rw-r--r--   0 root         (0) root         (0)     1229 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/labels.py
--rw-r--r--   0 root         (0) root         (0)    23122 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug/models/
--rw-r--r--   0 root         (0) root         (0)     2139 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3725 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/assignee.py
--rw-r--r--   0 root         (0) root         (0)     4189 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/backout.py
--rw-r--r--   0 root         (0) root         (0)     4218 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/bugtype.py
--rw-r--r--   0 root         (0) root         (0)    12193 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/component.py
--rw-r--r--   0 root         (0) root         (0)    15862 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/component_nn.py
--rw-r--r--   0 root         (0) root         (0)    11016 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/defect.py
--rw-r--r--   0 root         (0) root         (0)     1999 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/defect_enhancement_task.py
--rw-r--r--   0 root         (0) root         (0)     4424 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/devdocneeded.py
--rw-r--r--   0 root         (0) root         (0)     4703 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/duplicate.py
--rw-r--r--   0 root         (0) root         (0)     3165 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/qaneeded.py
--rw-r--r--   0 root         (0) root         (0)     1443 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/regression.py
--rw-r--r--   0 root         (0) root         (0)     3111 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/regressionrange.py
--rw-r--r--   0 root         (0) root         (0)     3991 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/regressor.py
--rw-r--r--   0 root         (0) root         (0)     3816 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/stepstoreproduce.py
--rw-r--r--   0 root         (0) root         (0)     4511 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/tracking.py
--rw-r--r--   0 root         (0) root         (0)     3314 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/models/uplift.py
--rw-r--r--   0 root         (0) root         (0)     3951 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/nlp.py
--rw-r--r--   0 root         (0) root         (0)     1699 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/nn.py
--rw-r--r--   0 root         (0) root         (0)    23755 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/repository.py
--rw-r--r--   0 root         (0) root         (0)    21986 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/similarity.py
--rw-r--r--   0 root         (0) root         (0)     4990 2019-09-07 00:01:38.000000 bugbug-0.0.98/bugbug/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/
--rw-r--r--   0 root         (0) root         (0)      450 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2205 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      684 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      444 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2019-09-07 00:01:39.000000 bugbug-0.0.98/bugbug.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       63 2019-09-07 00:01:38.000000 bugbug-0.0.98/extra-nlp-requirements.txt
--rw-r--r--   0 root         (0) root         (0)       31 2019-09-07 00:01:38.000000 bugbug-0.0.98/extra-nn-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/http_service/
--rw-r--r--   0 root         (0) root         (0)       24 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13843 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/app.py
--rw-r--r--   0 root         (0) root         (0)      984 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/check_models.py
--rw-r--r--   0 root         (0) root         (0)      457 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/download_models.py
--rw-r--r--   0 root         (0) root         (0)     4195 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/http_service/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/tests/test_app.py
--rw-r--r--   0 root         (0) root         (0)      911 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/utils.py
--rw-r--r--   0 root         (0) root         (0)     1168 2019-09-07 00:01:38.000000 bugbug-0.0.98/http_service/worker.py
--rw-r--r--   0 root         (0) root         (0)      485 2019-09-07 00:01:38.000000 bugbug-0.0.98/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-07 00:01:39.000000 bugbug-0.0.98/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5784 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/analyze_training_metrics.py
--rw-r--r--   0 root         (0) root         (0)     3080 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/bug_classifier.py
--rw-r--r--   0 root         (0) root         (0)     5127 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/bug_retriever.py
--rw-r--r--   0 root         (0) root         (0)     1443 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/check.py
--rw-r--r--   0 root         (0) root         (0)     3390 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/check_all_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2834 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/comment_level_labeler.py
--rw-r--r--   0 root         (0) root         (0)     5237 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/commit_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1439 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/commit_retriever.py
--rw-r--r--   0 root         (0) root         (0)     1529 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/evaluate_similarity.py
--rw-r--r--   0 root         (0) root         (0)     1617 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/generate_duplicate_sheet.py
--rw-r--r--   0 root         (0) root         (0)     2348 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/generate_sheet.py
--rw-r--r--   0 root         (0) root         (0)     1805 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/get_type_labels.py
--rw-r--r--   0 root         (0) root         (0)     3603 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/get_untriaged.py
--rw-r--r--   0 root         (0) root         (0)     3676 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/microannotate_generator.py
--rw-r--r--   0 root         (0) root         (0)    22978 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/regressor_finder.py
--rw-r--r--   0 root         (0) root         (0)     4053 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/retrieve_training_metrics.py
--rw-r--r--   0 root         (0) root         (0)      930 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/similarity_query.py
--rw-r--r--   0 root         (0) root         (0)     1850 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/similarity_trainer.py
--rw-r--r--   0 root         (0) root         (0)     3563 2019-09-07 00:01:38.000000 bugbug-0.0.98/scripts/trainer.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-09-07 00:01:39.000000 bugbug-0.0.98/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2270 2019-09-07 00:01:38.000000 bugbug-0.0.98/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/
+-rw-r--r--   0 root         (0) root         (0)      257 2019-09-11 19:20:24.000000 bugbug-0.0.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      450 2019-09-11 19:20:24.000000 bugbug-0.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5732 2019-09-11 19:20:24.000000 bugbug-0.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2019-09-11 19:20:24.000000 bugbug-0.0.99/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/
+-rw-r--r--   0 root         (0) root         (0)      191 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19764 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/bug_features.py
+-rw-r--r--   0 root         (0) root         (0)    29590 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/bug_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/bugzilla.py
+-rw-r--r--   0 root         (0) root         (0)     8783 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/commit_features.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/db.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/feature_cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/
+-rw-r--r--   0 root         (0) root         (0)     7170 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/bug_nobug.csv
+-rw-r--r--   0 root         (0) root         (0)     9467 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/defect_enhancement_task.csv
+-rw-r--r--   0 root         (0) root         (0)    36449 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/defect_enhancement_task_e.csv
+-rw-r--r--   0 root         (0) root         (0)   173880 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/defect_enhancement_task_h.csv
+-rw-r--r--   0 root         (0) root         (0)    36389 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/defect_enhancement_task_p.csv
+-rw-r--r--   0 root         (0) root         (0)    12215 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/defect_enhancement_task_s.csv
+-rw-r--r--   0 root         (0) root         (0)    43135 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/regression_bug_nobug.csv
+-rw-r--r--   0 root         (0) root         (0)     4365 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/regressionrange.csv
+-rw-r--r--   0 root         (0) root         (0)     4823 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/str.csv
+-rw-r--r--   0 root         (0) root         (0)     1452 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels/tracking.csv
+-rw-r--r--   0 root         (0) root         (0)     1229 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/labels.py
+-rw-r--r--   0 root         (0) root         (0)    23750 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/
+-rw-r--r--   0 root         (0) root         (0)     2139 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/assignee.py
+-rw-r--r--   0 root         (0) root         (0)     4189 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/backout.py
+-rw-r--r--   0 root         (0) root         (0)     4218 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/bugtype.py
+-rw-r--r--   0 root         (0) root         (0)    12193 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/component.py
+-rw-r--r--   0 root         (0) root         (0)    15862 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/component_nn.py
+-rw-r--r--   0 root         (0) root         (0)    11016 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/defect.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/defect_enhancement_task.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/devdocneeded.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/duplicate.py
+-rw-r--r--   0 root         (0) root         (0)     3165 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/qaneeded.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/regression.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/regressionrange.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/stepstoreproduce.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/tracking.py
+-rw-r--r--   0 root         (0) root         (0)     3314 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/models/uplift.py
+-rw-r--r--   0 root         (0) root         (0)     3951 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/nn.py
+-rw-r--r--   0 root         (0) root         (0)    23755 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/repository.py
+-rw-r--r--   0 root         (0) root         (0)    21986 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/similarity.py
+-rw-r--r--   0 root         (0) root         (0)     4990 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      450 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2250 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      769 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      444 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2019-09-11 19:20:24.000000 bugbug-0.0.99/bugbug.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2019-09-11 19:20:24.000000 bugbug-0.0.99/extra-nlp-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2019-09-11 19:20:24.000000 bugbug-0.0.99/extra-nn-requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/
+-rw-r--r--   0 root         (0) root         (0)       24 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13843 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/app.py
+-rw-r--r--   0 root         (0) root         (0)      984 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/check_models.py
+-rw-r--r--   0 root         (0) root         (0)      457 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/download_models.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/tests/test_app.py
+-rw-r--r--   0 root         (0) root         (0)      911 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2019-09-11 19:20:24.000000 bugbug-0.0.99/http_service/worker.py
+-rw-r--r--   0 root         (0) root         (0)      485 2019-09-11 19:20:24.000000 bugbug-0.0.99/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5784 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/analyze_training_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/bug_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     5167 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/bug_retriever.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/check.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/check_all_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/comment_level_labeler.py
+-rw-r--r--   0 root         (0) root         (0)     5277 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/commit_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/commit_retriever.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/evaluate_similarity.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/generate_duplicate_sheet.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/generate_sheet.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/get_type_labels.py
+-rw-r--r--   0 root         (0) root         (0)     3603 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/get_untriaged.py
+-rw-r--r--   0 root         (0) root         (0)     3716 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/microannotate_generator.py
+-rw-r--r--   0 root         (0) root         (0)    23018 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/regressor_finder.py
+-rw-r--r--   0 root         (0) root         (0)     4053 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/retrieve_training_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      930 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/similarity_query.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/similarity_trainer.py
+-rw-r--r--   0 root         (0) root         (0)     2471 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/test_scheduling_history_retriever.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2019-09-11 19:20:24.000000 bugbug-0.0.99/scripts/trainer.py
+-rw-r--r--   0 root         (0) root         (0)       38 2019-09-11 19:20:24.000000 bugbug-0.0.99/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2370 2019-09-11 19:20:24.000000 bugbug-0.0.99/setup.py
```

### Comparing `bugbug-0.0.98/README.md` & `bugbug-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/bug_features.py` & `bugbug-0.0.99/bugbug/bug_features.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/bug_snapshot.py` & `bugbug-0.0.99/bugbug/bug_snapshot.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/bugzilla.py` & `bugbug-0.0.99/bugbug/bugzilla.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/commit_features.py` & `bugbug-0.0.99/bugbug/commit_features.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/db.py` & `bugbug-0.0.99/bugbug/db.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/feature_cleanup.py` & `bugbug-0.0.99/bugbug/feature_cleanup.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/bug_nobug.csv` & `bugbug-0.0.99/bugbug/labels/bug_nobug.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/defect_enhancement_task.csv` & `bugbug-0.0.99/bugbug/labels/defect_enhancement_task.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/defect_enhancement_task_e.csv` & `bugbug-0.0.99/bugbug/labels/defect_enhancement_task_e.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/defect_enhancement_task_h.csv` & `bugbug-0.0.99/bugbug/labels/defect_enhancement_task_h.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/defect_enhancement_task_p.csv` & `bugbug-0.0.99/bugbug/labels/defect_enhancement_task_p.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/defect_enhancement_task_s.csv` & `bugbug-0.0.99/bugbug/labels/defect_enhancement_task_s.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/regression_bug_nobug.csv` & `bugbug-0.0.99/bugbug/labels/regression_bug_nobug.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/regressionrange.csv` & `bugbug-0.0.99/bugbug/labels/regressionrange.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/str.csv` & `bugbug-0.0.99/bugbug/labels/str.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels/tracking.csv` & `bugbug-0.0.99/bugbug/labels/tracking.csv`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/labels.py` & `bugbug-0.0.99/bugbug/labels.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/model.py` & `bugbug-0.0.99/bugbug/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,27 +89,36 @@
     }
 
     return result
 
 
 def print_labeled_confusion_matrix(confusion_matrix, labels, is_multilabel=False):
     confusion_matrix_table = confusion_matrix.tolist()
+
+    # Don't show the Not classified row in the table output
+    if "__NOT_CLASSIFIED__" in labels and not is_multilabel:
+        confusion_matrix_table.pop(labels.index("__NOT_CLASSIFIED__"))
+
     if not is_multilabel:
         confusion_matrix_table = [confusion_matrix_table]
 
     for num, table in enumerate(confusion_matrix_table):
         if is_multilabel:
             print(f"label: {labels[num]}")
             table_labels = [0, 1]
         else:
             table_labels = labels
 
         confusion_matrix_header = []
-        for i in range(len(table)):
-            confusion_matrix_header.append(f"{table_labels[i]} (Predicted)")
+        for i in range(len(table[0])):
+            confusion_matrix_header.append(
+                f"{table_labels[i]} (Predicted)"
+                if table_labels[i] != "__NOT_CLASSIFIED__"
+                else "Not classified"
+            )
         for i in range(len(table)):
             table[i].insert(0, f"{table_labels[i]} (Actual)")
         print(
             tabulate(table, headers=confusion_matrix_header, tablefmt="fancy_grid"),
             end="\n\n",
         )
 
@@ -424,53 +433,60 @@
         )
 
         tracking_metrics["confusion_matrix"] = confusion_matrix.tolist()
 
         # Evaluate results on the test set for some confidence thresholds.
         for confidence_threshold in [0.6, 0.7, 0.8, 0.9]:
             y_pred_probas = self.clf.predict_proba(X_test)
+            confidence_class_names = self.class_names + ["__NOT_CLASSIFIED__"]
 
-            y_test_filter = []
             y_pred_filter = []
+            classified_indices = []
             for i in range(0, len(y_test)):
                 argmax = np.argmax(y_pred_probas[i])
                 if y_pred_probas[i][argmax] < confidence_threshold:
+                    if not is_multilabel:
+                        y_pred_filter.append("__NOT_CLASSIFIED__")
                     continue
 
-                y_test_filter.append(y_test[i])
+                classified_indices.append(i)
                 if is_multilabel:
                     y_pred_filter.append(y_pred[i])
                 else:
                     y_pred_filter.append(argmax)
 
             if not is_multilabel:
-                y_pred_filter = self.le.inverse_transform(y_pred_filter)
+                y_pred_filter = np.array(y_pred_filter)
+                y_pred_filter[classified_indices] = self.le.inverse_transform(
+                    np.array(y_pred_filter[classified_indices], dtype=int)
+                )
 
             print(
-                f"\nConfidence threshold > {confidence_threshold} - {len(y_test_filter)} classified"
+                f"\nConfidence threshold > {confidence_threshold} - {len(y_test)} classified"
             )
-            if len(y_test_filter) != 0:
-                if is_multilabel:
-                    confusion_matrix = metrics.multilabel_confusion_matrix(
-                        np.asarray(y_test_filter), np.asarray(y_pred_filter)
-                    )
-                else:
-                    confusion_matrix = metrics.confusion_matrix(
-                        np.asarray(y_test_filter),
-                        np.asarray(y_pred_filter),
-                        labels=self.class_names,
-                    )
-                    print(
-                        classification_report_imbalanced(
-                            y_test_filter, y_pred_filter, labels=self.class_names
-                        )
+            if is_multilabel:
+                confusion_matrix = metrics.multilabel_confusion_matrix(
+                    y_test[classified_indices], np.asarray(y_pred_filter)
+                )
+            else:
+                confusion_matrix = metrics.confusion_matrix(
+                    y_test.astype(str),
+                    y_pred_filter.astype(str),
+                    labels=confidence_class_names,
+                )
+                print(
+                    classification_report_imbalanced(
+                        y_test.astype(str),
+                        y_pred_filter.astype(str),
+                        labels=confidence_class_names,
                     )
-                print_labeled_confusion_matrix(
-                    confusion_matrix, self.class_names, is_multilabel=is_multilabel
                 )
+            print_labeled_confusion_matrix(
+                confusion_matrix, confidence_class_names, is_multilabel=is_multilabel
+            )
 
         joblib.dump(self, self.__class__.__name__.lower())
 
         return tracking_metrics
 
     @staticmethod
     def load(model_file_name):
```

### Comparing `bugbug-0.0.98/bugbug/models/__init__.py` & `bugbug-0.0.99/bugbug/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/assignee.py` & `bugbug-0.0.99/bugbug/models/assignee.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/backout.py` & `bugbug-0.0.99/bugbug/models/backout.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/bugtype.py` & `bugbug-0.0.99/bugbug/models/bugtype.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/component.py` & `bugbug-0.0.99/bugbug/models/component.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/component_nn.py` & `bugbug-0.0.99/bugbug/models/component_nn.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/defect.py` & `bugbug-0.0.99/bugbug/models/defect.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/defect_enhancement_task.py` & `bugbug-0.0.99/bugbug/models/defect_enhancement_task.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/devdocneeded.py` & `bugbug-0.0.99/bugbug/models/devdocneeded.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/duplicate.py` & `bugbug-0.0.99/bugbug/models/duplicate.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/qaneeded.py` & `bugbug-0.0.99/bugbug/models/qaneeded.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/regression.py` & `bugbug-0.0.99/bugbug/models/regression.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/regressionrange.py` & `bugbug-0.0.99/bugbug/models/regressionrange.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/regressor.py` & `bugbug-0.0.99/bugbug/models/regressor.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/stepstoreproduce.py` & `bugbug-0.0.99/bugbug/models/stepstoreproduce.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/tracking.py` & `bugbug-0.0.99/bugbug/models/tracking.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/models/uplift.py` & `bugbug-0.0.99/bugbug/models/uplift.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/nlp.py` & `bugbug-0.0.99/bugbug/nlp.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/nn.py` & `bugbug-0.0.99/bugbug/nn.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/repository.py` & `bugbug-0.0.99/bugbug/repository.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/similarity.py` & `bugbug-0.0.99/bugbug/similarity.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug/utils.py` & `bugbug-0.0.99/bugbug/utils.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/bugbug.egg-info/SOURCES.txt` & `bugbug-0.0.99/bugbug.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -76,8 +76,9 @@
 scripts/get_type_labels.py
 scripts/get_untriaged.py
 scripts/microannotate_generator.py
 scripts/regressor_finder.py
 scripts/retrieve_training_metrics.py
 scripts/similarity_query.py
 scripts/similarity_trainer.py
+scripts/test_scheduling_history_retriever.py
 scripts/trainer.py
```

### Comparing `bugbug-0.0.98/bugbug.egg-info/entry_points.txt` & `bugbug-0.0.99/bugbug.egg-info/entry_points.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,13 +2,14 @@
 bugbug-analyze-training-metrics = scripts.analyze_training_metrics:main
 bugbug-check = scripts.check:main
 bugbug-check-all-metrics = scripts.check_all_metrics:main
 bugbug-classify-bug = scripts.bug_classifier:main
 bugbug-classify-commit = scripts.commit_classifier:main
 bugbug-data-bugzilla = scripts.bug_retriever:main
 bugbug-data-commits = scripts.commit_retriever:main
+bugbug-data-test-scheduling-history = scripts.test_scheduling_history_retriever:main
 bugbug-microannotate-generate = scripts.microannotate_generator:main
 bugbug-regressor-finder = scripts.regressor_finder:main
 bugbug-retrieve-training-metrics = scripts.retrieve_training_metrics:main
 bugbug-train = scripts.trainer:main
 bugbug-train-similarity = scripts.similarity_trainer:main
```

### Comparing `bugbug-0.0.98/http_service/app.py` & `bugbug-0.0.99/http_service/app.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/http_service/check_models.py` & `bugbug-0.0.99/http_service/check_models.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/http_service/models.py` & `bugbug-0.0.99/http_service/models.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/http_service/tests/test_app.py` & `bugbug-0.0.99/http_service/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/http_service/utils.py` & `bugbug-0.0.99/http_service/utils.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/http_service/worker.py` & `bugbug-0.0.99/http_service/worker.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/analyze_training_metrics.py` & `bugbug-0.0.99/scripts/analyze_training_metrics.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/bug_classifier.py` & `bugbug-0.0.99/scripts/bug_classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,7 +90,11 @@
         default="default",
     )
     parser.add_argument("--bug-id", help="Classify the given bug id")
 
     args = parser.parse_args()
 
     classify_bugs(args.model, args.classifier, args.bug_id)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/bug_retriever.py` & `bugbug-0.0.99/scripts/bug_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,7 +130,11 @@
     parser = argparse.ArgumentParser(description=description)
 
     # Parse args to show the help if `--help` is passed
     parser.parse_args()
 
     retriever = Retriever()
     retriever.retrieve_bugs()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/check.py` & `bugbug-0.0.99/scripts/check.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,7 +47,11 @@
 
     parser.add_argument("model", help="Which model to check.")
 
     args = parser.parse_args()
 
     checker = ModelChecker()
     checker.go(args.model)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/check_all_metrics.py` & `bugbug-0.0.99/scripts/check_all_metrics.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/comment_level_labeler.py` & `bugbug-0.0.99/scripts/comment_level_labeler.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/commit_classifier.py` & `bugbug-0.0.99/scripts/commit_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,7 +160,11 @@
     parser.add_argument("cache-root", help="Cache for repository clones.")
     parser.add_argument("diff_id", help="diff ID to analyze.", type=int)
 
     args = parser.parse_args()
 
     classifier = CommitClassifier(getattr(args, "cache-root"))
     classifier.classify(args.diff_id)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/commit_retriever.py` & `bugbug-0.0.99/scripts/commit_retriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,7 +46,11 @@
     parser.add_argument("cache-root", help="Cache for repository clones.")
 
     args = parser.parse_args()
 
     retriever = Retriever(getattr(args, "cache-root"))
 
     retriever.retrieve_commits()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/evaluate_similarity.py` & `bugbug-0.0.99/scripts/evaluate_similarity.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/generate_duplicate_sheet.py` & `bugbug-0.0.99/scripts/generate_duplicate_sheet.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/generate_sheet.py` & `bugbug-0.0.99/scripts/generate_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,7 +76,11 @@
     parser.add_argument(
         "threshold", type=float, default=0.7, help="Confidence threshold for the model"
     )
 
     args = parser.parse_args()
 
     generate_sheet(args.model, args.token, args.days, args.threshold)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/get_type_labels.py` & `bugbug-0.0.99/scripts/get_type_labels.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/get_untriaged.py` & `bugbug-0.0.99/scripts/get_untriaged.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/microannotate_generator.py` & `bugbug-0.0.99/scripts/microannotate_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,7 +118,11 @@
         getattr(args, "cache-root"),
         getattr(args, "repo-url"),
         args.tokenize,
         args.remove_comments,
     )
 
     generator.generate()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/regressor_finder.py` & `bugbug-0.0.99/scripts/regressor_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,7 +592,11 @@
     )
     evaluate(db.read(TOKENIZED_BUG_INTRODUCING_COMMITS_DB))
 
     regressor_finder.find_bug_introducing_commits(
         bug_fixing_commits, commits_to_ignore, False
     )
     evaluate(db.read(BUG_INTRODUCING_COMMITS_DB))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `bugbug-0.0.98/scripts/retrieve_training_metrics.py` & `bugbug-0.0.99/scripts/retrieve_training_metrics.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/similarity_query.py` & `bugbug-0.0.99/scripts/similarity_query.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/similarity_trainer.py` & `bugbug-0.0.99/scripts/similarity_trainer.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/scripts/trainer.py` & `bugbug-0.0.99/scripts/trainer.py`

 * *Files identical despite different names*

### Comparing `bugbug-0.0.98/setup.py` & `bugbug-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     packages=find_packages(exclude=["contrib", "docs", "tests"]),
     include_package_data=True,
     license="MPL2",
     entry_points={
         "console_scripts": [
             "bugbug-data-commits = scripts.commit_retriever:main",
             "bugbug-data-bugzilla = scripts.bug_retriever:main",
+            "bugbug-data-test-scheduling-history = scripts.test_scheduling_history_retriever:main",
             "bugbug-train = scripts.trainer:main",
             "bugbug-train-similarity = scripts.similarity_trainer:main",
             "bugbug-check = scripts.check:main",
             "bugbug-microannotate-generate = scripts.microannotate_generator:main",
             "bugbug-classify-commit = scripts.commit_classifier:main",
             "bugbug-classify-bug = scripts.bug_classifier:main",
             "bugbug-regressor-finder = scripts.regressor_finder:main",
```

