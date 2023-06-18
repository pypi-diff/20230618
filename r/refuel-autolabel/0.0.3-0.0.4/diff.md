# Comparing `tmp/refuel-autolabel-0.0.3.tar.gz` & `tmp/refuel-autolabel-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-autolabel-0.0.3.tar", last modified: Thu Jun 15 15:35:31 2023, max compression
+gzip compressed data, was "refuel-autolabel-0.0.4.tar", last modified: Sun Jun 18 19:49:40 2023, max compression
```

## Comparing `refuel-autolabel-0.0.3.tar` & `refuel-autolabel-0.0.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.643343 refuel-autolabel-0.0.3/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/LICENSE
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-15 15:35:31.642916 refuel-autolabel-0.0.3/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9005 2023-06-15 15:29:16.000000 refuel-autolabel-0.0.3/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-15 15:35:08.000000 refuel-autolabel-0.0.3/pyproject.toml
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-15 15:35:31.643404 refuel-autolabel-0.0.3/setup.cfg
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.628712 refuel-autolabel-0.0.3/src/
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.631361 refuel-autolabel-0.0.3/src/autolabel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/__init__.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.632207 refuel-autolabel-0.0.3/src/autolabel/cache/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/cache/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/cache/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/cache/sqlalchemy_cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.3/src/autolabel/confidence.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.633089 refuel-autolabel-0.0.3/src/autolabel/configs/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/configs/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/configs/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5880 2023-06-15 01:06:20.000000 refuel-autolabel-0.0.3/src/autolabel/configs/config.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.635318 refuel-autolabel-0.0.3/src/autolabel/data_models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/annotation.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/cache.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/dataset.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/task.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/data_models/task_run.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.635951 refuel-autolabel-0.0.3/src/autolabel/database/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/database/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/database/engine.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/database/state_manager.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/dataset_loader.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.636626 refuel-autolabel-0.0.3/src/autolabel/few_shot/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/few_shot/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/few_shot/fixed_example_selector.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/few_shot/vector_store.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19394 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/labeler.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.638070 refuel-autolabel-0.0.3/src/autolabel/models/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/models/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/anthropic.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/hf_pipeline.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3768 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.3/src/autolabel/models/openai.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3599 2023-06-15 01:29:24.000000 refuel-autolabel-0.0.3/src/autolabel/models/palm.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/models/refuel.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/schema.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.641755 refuel-autolabel-0.0.3/src/autolabel/tasks/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3509 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/base.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7060 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/classification.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7071 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/entity_matching.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/named_entity_recognition.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7160 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/question_answering.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.3/src/autolabel/tasks/utils.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.3/src/autolabel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-15 15:35:31.642679 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-15 15:35:31.000000 refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/top_level.txt
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.071488 refuel-autolabel-0.0.4/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1066 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/LICENSE
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-18 19:49:40.071267 refuel-autolabel-0.0.4/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9005 2023-06-15 15:29:16.000000 refuel-autolabel-0.0.4/README.md
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1922 2023-06-18 19:45:44.000000 refuel-autolabel-0.0.4/pyproject.toml
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       38 2023-06-18 19:49:40.071532 refuel-autolabel-0.0.4/setup.cfg
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.058118 refuel-autolabel-0.0.4/src/
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.062657 refuel-autolabel-0.0.4/src/autolabel/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       63 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/__init__.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.063613 refuel-autolabel-0.0.4/src/autolabel/cache/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       74 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/cache/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      924 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/cache/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1817 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/cache/sqlalchemy_cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     9137 2023-06-15 00:37:32.000000 refuel-autolabel-0.0.4/src/autolabel/confidence.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.064262 refuel-autolabel-0.0.4/src/autolabel/configs/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       65 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/configs/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1515 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/configs/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     5880 2023-06-15 01:06:20.000000 refuel-autolabel-0.0.4/src/autolabel/configs/config.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.065966 refuel-autolabel-0.0.4/src/autolabel/data_models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      195 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2001 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/annotation.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       71 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2036 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/cache.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1071 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/dataset.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      928 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/task.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2625 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/data_models/task_run.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.066545 refuel-autolabel-0.0.4/src/autolabel/database/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       77 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/database/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      410 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/database/engine.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2788 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/database/state_manager.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6592 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/dataset_loader.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.067208 refuel-autolabel-0.0.4/src/autolabel/few_shot/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2429 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/few_shot/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1295 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/few_shot/fixed_example_selector.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11031 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/few_shot/vector_store.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    19407 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/labeler.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.068816 refuel-autolabel-0.0.4/src/autolabel/models/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1965 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/models/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     2496 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/models/anthropic.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4150 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/models/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3037 2023-06-06 04:22:02.000000 refuel-autolabel-0.0.4/src/autolabel/models/hf_pipeline.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4026 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/models/openai.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3599 2023-06-15 01:29:24.000000 refuel-autolabel-0.0.4/src/autolabel/models/palm.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3569 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/models/refuel.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4625 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.4/src/autolabel/schema.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.070229 refuel-autolabel-0.0.4/src/autolabel/tasks/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1160 2023-06-14 00:54:29.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/__init__.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     3889 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/base.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7299 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/classification.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7309 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/entity_matching.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    12517 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/named_entity_recognition.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     7398 2023-06-17 06:35:55.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/question_answering.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1574 2023-06-12 01:38:44.000000 refuel-autolabel-0.0.4/src/autolabel/tasks/utils.py
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     8888 2023-06-14 20:56:12.000000 refuel-autolabel-0.0.4/src/autolabel/utils.py
+drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-06-18 19:49:40.071054 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)    11014 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1571 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)      641 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/requires.txt
+-rw-r--r--   0 rishabhbhargava   (501) staff       (20)       10 2023-06-18 19:49:40.000000 refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/top_level.txt
```

### Comparing `refuel-autolabel-0.0.3/LICENSE` & `refuel-autolabel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/PKG-INFO` & `refuel-autolabel-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for LLM powered labeling
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.3 Summary: Library
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.4 Summary: Library
 for LLM powered labeling Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `refuel-autolabel-0.0.3/README.md` & `refuel-autolabel-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/pyproject.toml` & `refuel-autolabel-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "wheel >= 0.38"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "refuel-autolabel"
-version = "0.0.3"
+version = "0.0.4"
 description = "Library for LLM powered labeling"
 readme = "README.md"
 authors = [{ name = "Refuel.ai", email = "support@refuel.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/cache/base.py` & `refuel-autolabel-0.0.4/src/autolabel/cache/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/cache/sqlalchemy_cache.py` & `refuel-autolabel-0.0.4/src/autolabel/cache/sqlalchemy_cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/confidence.py` & `refuel-autolabel-0.0.4/src/autolabel/confidence.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/configs/base.py` & `refuel-autolabel-0.0.4/src/autolabel/configs/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/configs/config.py` & `refuel-autolabel-0.0.4/src/autolabel/configs/config.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/data_models/annotation.py` & `refuel-autolabel-0.0.4/src/autolabel/data_models/annotation.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/data_models/cache.py` & `refuel-autolabel-0.0.4/src/autolabel/data_models/cache.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/data_models/dataset.py` & `refuel-autolabel-0.0.4/src/autolabel/data_models/dataset.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/data_models/task.py` & `refuel-autolabel-0.0.4/src/autolabel/data_models/task.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/data_models/task_run.py` & `refuel-autolabel-0.0.4/src/autolabel/data_models/task_run.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/database/state_manager.py` & `refuel-autolabel-0.0.4/src/autolabel/database/state_manager.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/dataset_loader.py` & `refuel-autolabel-0.0.4/src/autolabel/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/few_shot/__init__.py` & `refuel-autolabel-0.0.4/src/autolabel/few_shot/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/few_shot/fixed_example_selector.py` & `refuel-autolabel-0.0.4/src/autolabel/few_shot/fixed_example_selector.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/few_shot/vector_store.py` & `refuel-autolabel-0.0.4/src/autolabel/few_shot/vector_store.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/labeler.py` & `refuel-autolabel-0.0.4/src/autolabel/labeler.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         cost = 0.0
         postfix_dict = {}
 
         indices = range(current_index, len(inputs), self.CHUNK_SIZE)
         for current_index in track_with_stats(
             indices,
             postfix_dict,
-            total=len(inputs),
+            total=len(inputs) - current_index,
             advance=self.CHUNK_SIZE,
             console=console,
         ):
             chunk = inputs[current_index : current_index + self.CHUNK_SIZE]
             final_prompts = []
             for i, input_i in enumerate(chunk):
                 # Fetch few-shot seed examples
@@ -384,15 +384,15 @@
             table = {}
             for m in eval_result:
                 if isinstance(m.value, list) and len(m.value) > 0:
                     table[m.name] = m.value
                 else:
                     print(f"Metric: {m.name}: {m.value}")
             print_table(table, console=console, default_style=METRIC_TABLE_STYLE)
-        pprint(f"{len(llm_labels)} examples have been labeled so far.")
+        pprint(f"{task_run.current_index} examples labeled so far.")
         if len(llm_labels) > 0:
             console.rule("Last Annotated Example")
             pprint("[bold blue]Prompt[/bold blue]: ", end="")
             print(llm_labels[-1].prompt)
             pprint("[bold blue]Annotation[/bold blue]: ", end="")
             print(llm_labels[-1].label)
             console.rule()
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/__init__.py` & `refuel-autolabel-0.0.4/src/autolabel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/anthropic.py` & `refuel-autolabel-0.0.4/src/autolabel/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/base.py` & `refuel-autolabel-0.0.4/src/autolabel/models/base.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/hf_pipeline.py` & `refuel-autolabel-0.0.4/src/autolabel/models/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/openai.py` & `refuel-autolabel-0.0.4/src/autolabel/models/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 
 from autolabel.models import BaseModel
 from autolabel.configs import AutolabelConfig
 from autolabel.cache import BaseCache
 
 
 class OpenAILLM(BaseModel):
-    CHAT_ENGINE_MODELS = ["gpt-3.5-turbo", "gpt-4"]
+    CHAT_ENGINE_MODELS = [
+        "gpt-3.5-turbo",
+        "gpt-3.5-turbo-0613",
+        "gpt-3.5-turbo-16k",
+        "gpt-4",
+    ]
     MODELS_WITH_TOKEN_PROBS = ["text-curie-001", "text-davinci-003"]
 
     # Default parameters for OpenAILLM
     DEFAULT_MODEL = "gpt-3.5-turbo"
     DEFAULT_PARAMS_COMPLETION_ENGINE = {
         "max_tokens": 1000,
         "temperature": 0.0,
@@ -27,21 +32,25 @@
         "temperature": 0.0,
     }
 
     # Reference: https://openai.com/pricing
     COST_PER_PROMPT_TOKEN = {
         "text-davinci-003": 0.02 / 1000,
         "text-curie-001": 0.002 / 1000,
-        "gpt-3.5-turbo": 0.002 / 1000,
+        "gpt-3.5-turbo": 0.0015 / 1000,
+        "gpt-3.5-turbo-0613": 0.0015 / 1000,
+        "gpt-3.5-turbo-16k": 0.003 / 1000,
         "gpt-4": 0.03 / 1000,
     }
     COST_PER_COMPLETION_TOKEN = {
         "text-davinci-003": 0.02 / 1000,
         "text-curie-001": 0.002 / 1000,
         "gpt-3.5-turbo": 0.002 / 1000,
+        "gpt-3.5-turbo-0613": 0.002 / 1000,
+        "gpt-3.5-turbo-16k": 0.004 / 1000,
         "gpt-4": 0.06 / 1000,  # $0.06 per 1000 tokens in response
     }
 
     @cached_property
     def _engine(self) -> str:
         if self.model_name is not None and self.model_name in self.CHAT_ENGINE_MODELS:
             return "chat"
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/palm.py` & `refuel-autolabel-0.0.4/src/autolabel/models/palm.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/models/refuel.py` & `refuel-autolabel-0.0.4/src/autolabel/models/refuel.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/schema.py` & `refuel-autolabel-0.0.4/src/autolabel/schema.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/__init__.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/base.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import json
 
 from langchain.prompts.prompt import PromptTemplate
 from langchain.schema import Generation
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import LLMAnnotation, MetricResult, FewShotAlgorithm
-from autolabel.utils import get_format_variables
+from autolabel.utils import get_format_variables, extract_valid_json_substring
 
 logger = logging.getLogger(__name__)
 
 
 class BaseTask(ABC):
     ZERO_SHOT_TEMPLATE = "{task_guidelines}\n\n{output_guidelines}\n\nNow I want you to label the following example:\n{current_example}"
     FEW_SHOT_TEMPLATE = "{task_guidelines}\n\n{output_guidelines}\n\nSome examples with their output answers are provided below:\n\n{seed_examples}\n\nNow I want you to label the following example:\n{current_example}"
@@ -63,20 +63,29 @@
         )
 
     def parse_llm_response(
         self, response: Generation, curr_sample: Dict, prompt: str
     ) -> LLMAnnotation:
         # The last line of the response is the label
         # This is done to handle the case where the model generates an explanation before generating the label
-        completion_text = response.text.strip().split("\n")[-1].strip()
+        if self.config.chain_of_thought():
+            try:
+                completion_text = extract_valid_json_substring(
+                    response.text.strip().split("\n")[-1].strip()
+                )
+                completion_text = json.loads(completion_text)["label"]
+            except:
+                completion_text = None
+        else:
+            completion_text = response.text.strip().split("\n")[-1].strip()
         if len(response.text.strip()) == 0:
             successfully_labeled = False
             llm_label = self.NULL_LABEL_TOKEN
             logger.warning(f"LLM response is empty")
-        elif len(completion_text) == 0:
+        elif not completion_text:
             successfully_labeled = False
             llm_label = self.NULL_LABEL_TOKEN
             logger.error(f"Error parsing LLM response: {response.text}")
         else:
             successfully_labeled = True
             llm_label = completion_text.strip()
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/classification.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from autolabel.confidence import ConfidenceCalculator
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import LLMAnnotation, Metric, MetricResult
 from autolabel.tasks import BaseTask
 from autolabel.utils import get_format_variables
 
+import json
+
 
 class ClassificationTask(BaseTask):
     DEFAULT_OUTPUT_GUIDELINES = (
         'You will return the answer with just one element: "the correct label"'
     )
     DEFAULT_TASK_GUIDELINES = "Your job is to correctly label the provided input example into one of the following {num_labels} categories.\nCategories:\n{labels}\n"
 
@@ -31,20 +33,24 @@
         num_labels = len(labels_list)
         fmt_task_guidelines = self.task_guidelines.format(
             num_labels=num_labels, labels="\n".join(labels_list)
         )
 
         # prepare seed examples
         example_template = self.config.example_template()
+        label_column = self.config.label_column()
         fmt_examples = []
         for eg in examples:
-            fmt_examples.append(example_template.format_map(defaultdict(str, eg)))
+            eg_copy = eg.copy()
+            # If chain of thought is enabled
+            if label_column and self.config.chain_of_thought():
+                eg_copy[label_column] = json.dumps({"label": eg[label_column]})
+            fmt_examples.append(example_template.format_map(defaultdict(str, eg_copy)))
 
         # populate the current example in the prompt
-        label_column = self.config.label_column()
         if label_column:
             input[label_column] = ""
 
         # populate the explanation column with empty string for current example
         explanation_column = self.config.explanation_column()
         if explanation_column:
             input[explanation_column] = ""
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/entity_matching.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/entity_matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from typing import List, Dict, Tuple
+import json
 
 from langchain.prompts.prompt import PromptTemplate
 from sklearn.metrics import accuracy_score
 
 from autolabel.confidence import ConfidenceCalculator
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import LLMAnnotation, Metric, MetricResult
@@ -31,20 +32,24 @@
         num_labels = len(labels_list)
         fmt_task_guidelines = self.task_guidelines.format(
             num_labels=num_labels, labels="\n".join(labels_list)
         )
 
         # prepare seed examples
         example_template = self.config.example_template()
+        label_column = self.config.label_column()
         fmt_examples = []
         for eg in examples:
-            fmt_examples.append(example_template.format_map(defaultdict(str, eg)))
+            eg_copy = eg.copy()
+            # If chain of thought is enabled
+            if label_column and self.config.chain_of_thought():
+                eg_copy[label_column] = json.dumps({"label": eg[label_column]})
+            fmt_examples.append(example_template.format_map(defaultdict(str, eg_copy)))
 
         # populate the current example in the prompt
-        label_column = self.config.label_column()
         if label_column:
             input[label_column] = ""
 
         # populate the explanation column with empty string for current example
         explanation_column = self.config.explanation_column()
         if explanation_column:
             input[explanation_column] = ""
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/named_entity_recognition.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/question_answering.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/question_answering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from typing import List, Dict, Tuple
+import json
 
 from langchain.prompts.prompt import PromptTemplate
 from sklearn.metrics import accuracy_score
 
 from autolabel.confidence import ConfidenceCalculator
 from autolabel.configs import AutolabelConfig
 from autolabel.schema import LLMAnnotation, Metric, MetricResult
@@ -26,20 +27,24 @@
 
     def construct_prompt(self, input: Dict, examples: List[Dict]) -> str:
         # Copy over the input so that we can modify it
         input = input.copy()
 
         # prepare seed examples
         example_template = self.config.example_template()
+        label_column = self.config.label_column()
         fmt_examples = []
         for eg in examples:
-            fmt_examples.append(example_template.format_map(defaultdict(str, eg)))
+            eg_copy = eg.copy()
+            # If chain of thought is enabled
+            if label_column and self.config.chain_of_thought():
+                eg_copy[label_column] = json.dumps({"label": eg[label_column]})
+            fmt_examples.append(example_template.format_map(defaultdict(str, eg_copy)))
 
         # populate the current example in the prompt
-        label_column = self.config.label_column()
         if label_column:
             input[label_column] = ""
 
         # populate the explanation column with empty string for current example
         explanation_column = self.config.explanation_column()
         if explanation_column:
             input[explanation_column] = ""
```

### Comparing `refuel-autolabel-0.0.3/src/autolabel/tasks/utils.py` & `refuel-autolabel-0.0.4/src/autolabel/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/autolabel/utils.py` & `refuel-autolabel-0.0.4/src/autolabel/utils.py`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/PKG-INFO` & `refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refuel-autolabel
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for LLM powered labeling
 Author-email: "Refuel.ai" <support@refuel.ai>
 License: MIT License
         
         Copyright (c) 2023 refuel-ai
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.3 Summary: Library
+Metadata-Version: 2.1 Name: refuel-autolabel Version: 0.0.4 Summary: Library
 for LLM powered labeling Author-email: "Refuel.ai"
 refuel.ai> License: MIT License Copyright (c) 2023 refuel-ai Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/SOURCES.txt` & `refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refuel-autolabel-0.0.3/src/refuel_autolabel.egg-info/requires.txt` & `refuel-autolabel-0.0.4/src/refuel_autolabel.egg-info/requires.txt`

 * *Files identical despite different names*

