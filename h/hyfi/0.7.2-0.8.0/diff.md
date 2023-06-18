# Comparing `tmp/hyfi-0.7.2.tar.gz` & `tmp/hyfi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.7.2.tar", max compression
+gzip compressed data, was "hyfi-0.8.0.tar", max compression
```

## Comparing `hyfi-0.7.2.tar` & `hyfi-0.8.0.tar`

### file list

```diff
@@ -1,83 +1,85 @@
--rw-r--r--   0        0        0     1071 2023-06-17 11:43:48.311136 hyfi-0.7.2/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-17 11:43:48.311136 hyfi-0.7.2/README.md
--rw-r--r--   0        0        0     4592 2023-06-17 11:44:20.783312 hyfi-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3804 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2544 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__click__.py
--rw-r--r--   0        0        0      647 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9856 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      735 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-17 11:44:20.683312 hyfi-0.7.2/src/hyfi/_version.py
--rw-r--r--   0        0        0      777 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3182 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/cached_path/_cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-17 11:44:20.683312 hyfi-0.7.2/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      407 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-17 11:43:48.315136 hyfi-0.7.2/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      948 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0      120 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      609 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      121 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      130 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6369 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     3045 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8363 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4535 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     6610 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0    21338 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0     7618 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3487 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16589 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2579 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    30754 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      217 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     2903 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     5743 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     5564 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/py.typed
--rw-r--r--   0        0        0     4907 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     5239 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     5667 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    12630 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/file.py
--rw-r--r--   0        0        0     9920 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1114 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3699 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     4162 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1986 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0     9766 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     5476 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      232 2023-06-17 11:43:48.319136 hyfi-0.7.2/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-18 12:24:27.497927 hyfi-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-18 12:24:27.497927 hyfi-0.8.0/README.md
+-rw-r--r--   0        0        0     4592 2023-06-18 12:24:55.180192 hyfi-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3804 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2544 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      647 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9858 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      735 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-18 12:24:55.096186 hyfi-0.8.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0      777 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3182 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/cached_path/_cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:24:27.501927 hyfi-0.8.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-18 12:24:55.096186 hyfi-0.8.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      407 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      948 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      396 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      132 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      195 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6369 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     3045 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8363 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4535 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     6610 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0    22023 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0     7618 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3487 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16589 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2636 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    30789 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      219 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     3220 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     1897 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     4649 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5874 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4544 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     5234 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     6948 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/dataframe.py
+-rw-r--r--   0        0        0     5667 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0     6215 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/file.py
+-rw-r--r--   0        0        0    10015 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1114 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3766 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     4162 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     2002 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0     9981 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     5584 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      232 2023-06-18 12:24:27.505928 hyfi-0.8.0/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 hyfi-0.8.0/PKG-INFO
```

### Comparing `hyfi-0.7.2/LICENSE` & `hyfi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/README.md` & `hyfi-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/pyproject.toml` & `hyfi-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.7.2"
+version = "0.8.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.7.2/src/hyfi/__cli__.py` & `hyfi-0.8.0/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/__click__.py` & `hyfi-0.8.0/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/__global__/__init__.py` & `hyfi-0.8.0/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/__global__/config.py` & `hyfi-0.8.0/src/hyfi/__global__/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             logger.debug("Using default config.")
 
         # Skip project config initialization.
         if "project" not in config:
             logger.info("No project config found, skip project config initialization.")
             return
         self.project = ProjectConfig(**config["project"])
-        self.project.init_project()
+        # self.project.init_project()
         # Initialize joblib backend if joblib is not set.
         if self.project.joblib:
             self.project.joblib.init_backend()
 
         self.__initilized__ = True
 
     def terminate(self):
```

### Comparing `hyfi-0.7.2/src/hyfi/__init__.py` & `hyfi-0.8.0/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/about/__init__.py` & `hyfi-0.8.0/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/batch/__init__.py` & `hyfi-0.8.0/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/__init__.py` & `hyfi-0.8.0/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/__init__.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/_cached_path.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/cache_file.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/common.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/file_lock.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/meta.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/progress.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/__init__.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/beaker.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/hf.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/http.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/testing.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/cached_path/_cached_path/util.py` & `hyfi-0.8.0/src/hyfi/cached_path/_cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.8.0/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.8.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.8.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.8.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.8.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.8.0/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/copier/__init__.py` & `hyfi-0.8.0/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/dotenv/__init__.py` & `hyfi-0.8.0/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/graphics/collage.py` & `hyfi-0.8.0/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/graphics/motion.py` & `hyfi-0.8.0/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/graphics/utils.py` & `hyfi-0.8.0/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/hydra/__init__.py` & `hyfi-0.8.0/src/hyfi/hydra/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,57 +70,57 @@
         super().__init__(**args)
         self.__cfg__ = self.compose(
             config_group=self.config_group,
             overrides=self.overrides,
             config_data=self.config_data,
             throw_on_resolution_failure=self.throw_on_resolution_failure,
             throw_on_missing=self.throw_on_missing,
-            config_name=self.config_name,
+            root_config_name=self.config_name,
             config_module=self.config_module,
             global_package=self.global_package,
             verbose=self.verbose,
         )
 
     def compose(
         self,
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        config_name: Union[str, None] = None,
+        root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
         """
         Compose a configuration by applying overrides
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
             overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
             config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group.key=value`)
             return_as_dict: Return the result as a dict
             throw_on_resolution_failure: If True throw an exception if resolution fails
             throw_on_missing: If True throw an exception if config_group doesn't exist
-            config_name: Name of the root config to be used (e.g. `hconf`)
+            root_config_name: Name of the root config to be used (e.g. `hconf`)
             config_module: Module of the config to be used (e.g. `hyfi.conf`)
             global_package: If True, the config assumed to be a global package
             verbose: If True print configuration to stdout
 
         Returns:
             A config object or a dictionary with the composed config
         """
         self.__cfg__ = Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
-            config_name=config_name,
+            root_config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
         return self.__cfg__
 
     @property
@@ -134,26 +134,26 @@
     def __call__(
         self,
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        config_name: Union[str, None] = None,
+        root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> DictConfig:
         return self.compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
-            config_name=config_name,
+            root_config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
 
     def __getitem__(self, key):
         return self.__cfg__[key]
@@ -258,37 +258,37 @@
         Returns:
             A Config object that corresponds to the given config.
         """
         return OmegaConf.create(cfg)
 
     @staticmethod
     def hydra_compose(
-        config_name: Union[str, None] = None,
+        root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
     ):
         is_initialized = hydra.core.global_hydra.GlobalHydra.instance().is_initialized()  # type: ignore
         config_module = config_module or __hydra_config__.hyfi_config_module
         logger.debug("config_module: %s", config_module)
         if is_initialized:
             # Hydra is already initialized.
             logger.debug("Hydra is already initialized")
-            cfg = hydra.compose(config_name=config_name, overrides=overrides)
+            cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         else:
             with hydra.initialize_config_module(
                 config_module=config_module, version_base=__hydra_version_base__
             ):
-                cfg = hydra.compose(config_name=config_name, overrides=overrides)
+                cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         if is_initialized:
-            cfg = hydra.compose(config_name=config_name, overrides=overrides)
+            cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         else:
             with hydra.initialize_config_module(
                 config_module=config_module, version_base=__hydra_version_base__
             ):
-                cfg = hydra.compose(config_name=config_name, overrides=overrides)
+                cfg = hydra.compose(config_name=root_config_name, overrides=overrides)
         return cfg
 
     @staticmethod
     def split_config_group(
         config_group: Union[str, None] = None,
     ) -> Tuple[str, str, str]:
         if config_group:
@@ -309,15 +309,15 @@
     @staticmethod
     def _compose(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        config_name: Union[str, None] = None,
+        root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         **kwargs,
     ) -> DictConfig:
         if isinstance(config_data, DictConfig):
             logger.debug("returning config_group_kwargs without composing")
             return config_data
@@ -326,15 +326,15 @@
             overrides = []
         # Set the group key and value of the config group.
         config_group, group_key, group_value = Composer.split_config_group(config_group)
         # If group_key and group_value are specified in the configuration file.
         if group_key and group_value:
             # Initialize hydra configuration module.
             cfg = Composer.hydra_compose(
-                config_name=config_name,
+                root_config_name=root_config_name,
                 config_module=config_module,
                 overrides=overrides,
             )
             cfg = _select(
                 cfg,
                 key=group_key,
                 default=None,
@@ -344,25 +344,45 @@
             override = config_group if cfg is not None else f"+{config_group}"
             # Add override to overrides list.
             if isinstance(override, str):
                 if overrides:
                     overrides.append(override)
                 else:
                     overrides = [override]
-        # Add config group overrides to overrides list.
-        if group_key and config_data:
-            for k, v in config_data.items():
-                if isinstance(v, (str, int)):
-                    overrides.append(f"{group_key}.{k}={v}")
         # if verbose:
         logger.debug(f"compose config with overrides: {overrides}")
         # Initialize hydra and return the configuration.
         cfg = Composer.hydra_compose(
-            config_name=config_name, config_module=config_module, overrides=overrides
+            root_config_name=root_config_name,
+            config_module=config_module,
+            overrides=overrides,
+        )
+        # Add config group overrides to overrides list.
+        group_overrides = []
+        group_cfg = Composer.select(
+            cfg,
+            key=group_key,
+            default=None,
+            throw_on_missing=False,
+            throw_on_resolution_failure=False,
         )
+        if config_data and group_cfg:
+            group_overrides.extend(
+                f"{group_key}.{k}={v}"
+                for k, v in config_data.items()
+                if isinstance(v, (str, int, float, bool)) and k in group_cfg
+            )
+        if group_overrides:
+            overrides.extend(group_overrides)
+            cfg = Composer.hydra_compose(
+                root_config_name=root_config_name,
+                config_module=config_module,
+                overrides=overrides,
+            )
+
         # Select the group_key from the configuration.
         if group_key and not global_package:
             cfg = Composer.select(
                 cfg,
                 key=group_key,
                 default=None,
                 throw_on_missing=throw_on_missing,
@@ -568,44 +588,44 @@
 def _compose(
     config_group: Union[str, None] = None,
     overrides: Union[List[str], None] = None,
     config_data: Union[Dict[str, Any], DictConfig, None] = None,
     return_as_dict: bool = True,
     throw_on_resolution_failure: bool = True,
     throw_on_missing: bool = False,
-    config_name: Union[str, None] = None,
+    root_config_name: Union[str, None] = None,
     config_module: Union[str, None] = None,
     global_package: bool = False,
     verbose: bool = False,
 ) -> Union[DictConfig, Dict]:  # sourcery skip: low-code-quality
     """
     Compose a configuration by applying overrides
 
     Args:
         config_group: Name of the config group to compose (`config_group=name`)
         overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
         config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
         return_as_dict: Return the result as a dict
         throw_on_resolution_failure: If True throw an exception if resolution fails
         throw_on_missing: If True throw an exception if config_group doesn't exist
-        config_name: Name of the root config to be used (e.g. `hconf`)
+        root_config_name: Name of the root config to be used (e.g. `hconf`)
         config_module: Module of the config to be used (e.g. `hyfi.conf`)
         global_package: If True, the config assumed to be a global package
         verbose: If True print configuration to stdout
 
     Returns:
         A config object or a dictionary with the composed config
     """
     cmpsr = Composer(
         config_group=config_group,
         overrides=overrides,
         config_data=config_data,
         throw_on_resolution_failure=throw_on_resolution_failure,
         throw_on_missing=throw_on_missing,
-        config_name=config_name,
+        config_name=root_config_name,
         config_module=config_module,
         global_package=global_package,
         verbose=verbose,
     )
     return cmpsr.config_as_dict if return_as_dict else cmpsr.config
```

### Comparing `hyfi-0.7.2/src/hyfi/hydra/main.py` & `hyfi-0.8.0/src/hyfi/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/joblib/__init__.py` & `hyfi-0.8.0/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/joblib/batch/apply.py` & `hyfi-0.8.0/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.8.0/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.8.0/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/joblib/pipe.py` & `hyfi-0.8.0/src/hyfi/joblib/pipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,17 @@
                 batcher_instance.minibatch_size = min(
                     int(len(series) / batcher_instance.procs) + 1, minibatch_size
                 )
                 logger.info(
                     f"Using batcher with minibatch size: {batcher_instance.minibatch_size}"
                 )
                 results = decorator_apply(
-                    func, batcher_instance, description=description
+                    func,
+                    batcher_instance,
+                    description=description,  # type: ignore
                 )(series)
                 if batcher_instance is not None:
                     batcher_instance.minibatch_size = batcher_minibatch_size
                 return results
 
         if batcher_instance is None:
             logger.info("Warning: batcher not initialized")
```

### Comparing `hyfi-0.7.2/src/hyfi/main/__init__.py` & `hyfi-0.8.0/src/hyfi/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,45 +135,45 @@
     def compose(
         config_group: Union[str, None] = None,
         overrides: Union[List[str], None] = None,
         config_data: Union[Dict[str, Any], DictConfig, None] = None,
         return_as_dict: bool = True,
         throw_on_resolution_failure: bool = True,
         throw_on_missing: bool = False,
-        config_name: Union[str, None] = None,
+        root_config_name: Union[str, None] = None,
         config_module: Union[str, None] = None,
         global_package: bool = False,
         verbose: bool = False,
     ) -> Union[DictConfig, Dict]:
         """
         Compose a configuration by applying overrides
 
         Args:
             config_group: Name of the config group to compose (`config_group=name`)
             overrides: List of config groups to apply overrides to (`overrides=["override_name"]`)
             config_data: Keyword arguments to override config group values (will be converted to overrides of the form `config_group_name.key=value`)
             return_as_dict: Return the result as a dict
             throw_on_resolution_failure: If True throw an exception if resolution fails
             throw_on_missing: If True throw an exception if config_group doesn't exist
-            config_name: Name of the root config to be used (e.g. `hconf`)
+            root_config_name: Name of the root config to be used (e.g. `hconf`)
             config_module: Module of the config to be used (e.g. `hyfi.conf`)
             global_package: If True, the config assumed to be a global package
             verbose: If True print configuration to stdout
 
         Returns:
             A config object or a dictionary with the composed config
         """
         return Composer._compose(
             config_group=config_group,
             overrides=overrides,
             config_data=config_data,
             return_as_dict=return_as_dict,
             throw_on_resolution_failure=throw_on_resolution_failure,
             throw_on_missing=throw_on_missing,
-            config_name=config_name,
+            config_name=root_config_name,
             config_module=config_module,
             global_package=global_package,
             verbose=verbose,
         )
 
     @staticmethod
     def select(
@@ -435,15 +435,15 @@
         columns=None,
         index: bool = False,
         filetype="parquet",
         suffix: str = "",
         verbose: bool = False,
         **kwargs,
     ):
-        from hyfi.utils.file import save_data
+        from hyfi.utils.dataframe import save_data
 
         save_data(
             data,
             filename,
             base_dir=base_dir,
             columns=columns,
             index=index,
@@ -451,15 +451,15 @@
             suffix=suffix,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def load_data(filename=None, base_dir=None, filetype=None, verbose=False, **kwargs):
-        from hyfi.utils.file import load_data
+        from hyfi.utils.dataframe import load_data
 
         if filename is not None:
             filename = str(filename)
         if SpecialKeys.TARGET in kwargs:
             return XC.instantiate(
                 kwargs,
                 filename=filename,
@@ -501,29 +501,29 @@
         columns=None,
         add_key_as_name=False,
         name_column="_name_",
         ignore_index=True,
         verbose=False,
         **kwargs,
     ):
-        from hyfi.utils.file import concat_data
+        from hyfi.utils.dataframe import concat_data
 
         return concat_data(
             data,
             columns=columns,
             add_key_as_name=add_key_as_name,
             name_column=name_column,
             ignore_index=ignore_index,
             verbose=verbose,
             **kwargs,
         )
 
     @staticmethod
     def is_dataframe(data):
-        from hyfi.utils.file import is_dataframe
+        from hyfi.utils.dataframe import is_dataframe
 
         return is_dataframe(data)
 
     @staticmethod
     def is_colab():
         return is_colab()
```

### Comparing `hyfi-0.7.2/src/hyfi/path/__init__.py` & `hyfi-0.8.0/src/hyfi/path/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from typing import Any
 
 from pydantic import BaseModel
 
 from hyfi.__global__ import __about__
-from hyfi.hydra import _compose
+from hyfi.hydra import Composer
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 class PathConfig(BaseModel):
     config_name: str = "__init__"
@@ -45,30 +45,43 @@
     class Config:
         extra = "allow"
         arbitrary_types_allowed = True
 
     def __init__(
         self,
         config_name: str = "__init__",
+        config_group: str = "path",
         **data: Any,
     ):
         """
         Initialize the config. This is the base implementation of __init__. You can override this in your own subclass if you want to customize the initilization of a config by passing a keyword argument ` data `.
 
         Args:
                 config_name: The name of the config to initialize
                 data: The data to initialize
         """
-        # Initialize the config module.
-        data = _compose(
-            f"path={config_name}",
+        super().__init__(**data)
+        self.initialize_configs(
+            config_name=config_name,
+            config_group=config_group,
+            **data,
+        )
+
+    def initialize_configs(
+        self,
+        config_name: str = "__init__",
+        config_group: str = "path",
+        **data,
+    ):
+        # Initialize the config with the given config_name.
+        data = Composer(
+            config_group=f"{config_group}={config_name}",
             config_data=data,
-            config_module=__about__.config_module,
-        )  # type: ignore
-        super().__init__(config_name=config_name, **data)
+        ).config_as_dict
+        self.__dict__.update(data)
 
     @property
     def log_dir(self):
         """
         Create and return the path to the log directory. This is a convenience method for use in unit tests that want to ensure that the log directory exists and is accessible to the user.
```

### Comparing `hyfi-0.7.2/src/hyfi/path/batch.py` & `hyfi-0.8.0/src/hyfi/path/task.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 from pathlib import Path
 from typing import Any
 
 from pydantic import BaseModel
 
-from hyfi.hydra import _compose
+from hyfi.hydra import Composer
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
-class BatchPathConfig(BaseModel):
-    config_name: str = "__batch__"
+class TaskPathConfig(BaseModel):
+    config_name: str = "__task__"
 
-    project_workspace_root = ""
-    batch_name: str = "demo"
-    batch_output: str = ""
-    task_name: str = "default-task"
-    task_root: str = ""
+    task_root: str = "tmp/task"
     task_outputs: str = ""
     task_datasets: str = ""
     task_library: str = ""
     task_models: str = ""
     task_cache: str = ""
     task_tmp: str = ""
     task_log: str = ""
 
     class Config:
         extra = "ignore"
 
-    def __init__(self, config_name: str = "__batch__", **data: Any):
+    def __init__(
+        self,
+        config_name: str = "__task__",
+        config_group: str = "path",
+        **data: Any,
+    ):
         """
         Initialize the batch. This is the method you call when you want to initialize the batch from a config
 
         Args:
                 config_name: The name of the config you want to use
                 data: The data you want to initilize the
         """
-        # Initialize the config with the given config_name.
-        if not data:
-            logger.debug(
-                "There are no arguments to initilize a config, using default config %s",
-                config_name,
-            )
-            data = _compose(f"path={config_name}")
         super().__init__(**data)
+        self.initialize_configs(
+            config_name=config_name,
+            config_group=config_group,
+            **data,
+        )
 
-    @property
-    def project_workspace_dir(self) -> Path:
-        """
-        Get the path to the project workspace directory.
-
-
-        Returns:
-                absolute path to the project workspace directory or None if not set by the user ( in which case a default is used )
-        """
-        self.project_workspace_root = self.project_workspace_root or "./workspace"
-        return Path(self.project_workspace_root).absolute()
+    def initialize_configs(
+        self,
+        config_name: str = "__task__",
+        config_group: str = "path",
+        **data,
+    ):
+        # Initialize the config with the given config_name.
+        data = Composer(
+            config_group=f"{config_group}={config_name}",
+            config_data=data,
+        ).config_as_dict
+        self.__dict__.update(data)
 
     @property
     def root_dir(self) -> Path:
         """
-        Returns the absolute path to the task root directory. If the task_root attribute is set it is used as the path to the task's data directory. Otherwise the task name is used as the path to the project's data directory.
-
+        Returns the absolute path to the task root directory.
 
         Returns:
                 an absolute path to the task root directory or None if it doesn't exist or cannot be converted to a path object
         """
-        self.task_root = (
-            self.task_root or (self.project_workspace_dir / self.task_name).as_posix()
-        )
         # return as an absolute path
         return Path(self.task_root).absolute()
 
     @property
     def output_dir(self) -> Path:
         """
         Returns the directory where the task outputs are stored. It is used to determine where the output files will be stored when running the task.
@@ -81,28 +77,14 @@
         Returns:
                 absolute path to the output directory of the task ( relative to the task root directory ) or None if not
         """
         self.task_outputs = self.task_outputs or (self.root_dir / "outputs").as_posix()
         return Path(self.task_outputs).absolute()
 
     @property
-    def batch_dir(self) -> Path:
-        """
-        The directory where the batch is stored. It is used to determine where the results are stored for a batch of data to be processed.
-
-
-        Returns:
-                The directory where the batch output is stored for a batch of data to be processed ( relative to the task output directory )
-        """
-        self.batch_output = (
-            self.batch_output or (self.output_dir / self.batch_name).as_posix()
-        )
-        return Path(self.batch_output).absolute()
-
-    @property
     def library_dir(self) -> Path:
         """
         The path to the library.
 
 
         Returns:
                 absolute path to the library directory ( relative to the task root directory ).
```

### Comparing `hyfi-0.7.2/src/hyfi/project/__init__.py` & `hyfi-0.8.0/src/hyfi/project/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Any, Union
 
 from pydantic import BaseModel, validator
 
 from hyfi.__global__ import __about__
 from hyfi.dotenv import DotEnvConfig
-from hyfi.hydra import _compose
+from hyfi.hydra import Composer
 from hyfi.joblib import JobLibConfig
 from hyfi.path import PathConfig
 from hyfi.utils.logging import getLogger
 from hyfi.utils.notebook import is_notebook
 
 logger = getLogger(__name__)
 
@@ -55,29 +55,40 @@
             else:
                 raise ValueError("verbose must be a boolean or a string of 0 or 1")
         return v
 
     def __init__(
         self,
         config_name: str = "__init__",
+        config_group: str = "project",
         **data: Any,
     ):
-        data = _compose(
-            f"project={config_name}",
+        super().__init__(**data)
+        self.initialize_configs(
+            config_name=config_name,
+            config_group=config_group,
+            **data,
+        )
+
+    def initialize_configs(
+        self,
+        config_name: str = "__init__",
+        config_group: str = "project",
+        **data,
+    ):
+        # Initialize the config with the given config_name.
+        data = Composer(
+            config_group=f"{config_group}={config_name}",
             config_data=data,
-            config_module=__about__.config_module,
-        )  # type: ignore
-        super().__init__(config_name=config_name, **data)
+        ).config_as_dict
+        self.__dict__.update(data)
 
-    def init_project(self):
         self.dotenv = DotEnvConfig()
-        if self.path is None:
-            self.path = PathConfig()
-        if self.joblib is None:
-            self.joblib = JobLibConfig()
+        self.path = PathConfig(**self.__dict__["path"])
+        self.joblib = JobLibConfig(**self.__dict__["joblib"])
 
         self.dotenv.HYFI_PROJECT_NAME = self.project_name
         self.dotenv.HYFI_TASK_NAME = self.task_name
         self.dotenv.HYFI_PROJECT_DESC = self.project_description
         self.dotenv.HYFI_PROJECT_ROOT = self.project_root
         self.dotenv.HYFI_PROJECT_WORKSPACE_NAME = self.project_workspace_name
         self.dotenv.HYFI_GLOBAL_ROOT = self.global_hyfi_root
```

### Comparing `hyfi-0.7.2/src/hyfi/task/__init__.py` & `hyfi-0.8.0/src/hyfi/task/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import contextlib
 from pathlib import Path
 from typing import Union
 
-from omegaconf import DictConfig
 from pydantic import BaseModel
 
 from hyfi.hydra import Composer
 from hyfi.module import ModuleConfig
 from hyfi.path.batch import BatchPathConfig
 from hyfi.project import ProjectConfig
 from hyfi.utils.lib import ensure_import_module
@@ -14,158 +12,150 @@
 
 logger = getLogger(__name__)
 
 
 class TaskConfig(BaseModel):
     config_name: str = "__init__"
     config_group: str = "task"
-    task_name: str
-    path: BatchPathConfig = None  # type: ignore
-    project: ProjectConfig = None  # type: ignore
-    module: ModuleConfig = None  # type: ignore
+    task_name: str = "demo-task"
+    task_root: str = "tmp/task"
     autoload: bool = False
     version: str = "0.0.0"
-    _config_: DictConfig = None  # type: ignore
-    _initial_config_: DictConfig = None  # type: ignore
+    module: ModuleConfig = None  # type: ignore
+    path: BatchPathConfig = None  # type: ignore
+    project: ProjectConfig = None  # type: ignore
 
     class Config:
         arbitrary_types_allowed = True
         extra = "allow"
         validate_assignment = False
         exclude = {
-            "_config_",
-            "_initial_config_",
             "__data__",
             "path",
             "module",
             "project",
         }
         include = {}
         underscore_attrs_are_private = True
         property_set_methods = {
-            "name": "set_name",
-            "root_dir": "set_root_dir",
+            "task_name": "set_task_name",
+            "task_root": "set_task_root",
         }
 
     def __init__(
         self,
-        config_name: str = "",
-        config_group: str = "",
-        root_dir: str = "",
-        **args,
+        config_name: str = "__init__",
+        config_group: str = "task",
+        **data,
     ):
-        if config_group:
-            args = Composer.merge(Composer._compose(config_group), args)
-        else:
-            args = Composer.to_config(args)
-        super().__init__(config_name=config_name, config_group=config_group, **args)
-
-        object.__setattr__(self, "_config_", args)
-        object.__setattr__(self, "_initial_config_", args.copy())
-        self.initialize_configs(root_dir=root_dir)
+        super().__init__(**data)
+        self.initialize_configs(
+            config_name=config_name,
+            config_group=config_group,
+            **data,
+        )
 
     def __setattr__(self, key, val):
         super().__setattr__(key, val)
-        method = self.__config__.property_set_methods.get(key)
-        if method is not None:
+        if method := self.__config__.property_set_methods.get(key):  # type: ignore
             getattr(self, method)(val)
 
-    def set_root_dir(self, root_dir: Union[str, Path]):
-        path = self.config.path
-        if path is None:
-            path = Composer._compose("path=_batch_")
-            logger.info(
-                f"There is no path in the config, using default path: {path.root}"
-            )
-            self._config_.path = path
-        if root_dir is not None:
-            path.root = str(root_dir)
-        self.path = BatchPathConfig(**path)
-
-    def set_name(self, val):
-        self._config_.name = val
-        if self.task_name is None or self.task_name != val:
-            self.task_name = val
+    def set_task_root(self, val: Union[str, Path]):
+        if not self.task_root or self.task_root != val:
+            self.initialize_configs(task_root=val)
+
+    def set_task_name(self, val):
+        if not self.task_name or self.task_name != val:
+            self.initialize_configs(task_name=val)
 
-    def initialize_configs(self, root_dir=None, **kwargs):
-        self.root_dir = root_dir
+    def initialize_configs(
+        self,
+        config_name: str = "__init__",
+        config_group: str = "task",
+        **data,
+    ):
+        # Initialize the config with the given config_name.
+        data = Composer(
+            config_group=f"{config_group}={config_name}",
+            config_data=data,
+        ).config_as_dict
+        self.__dict__.update(data)
+        if "module" in data:
+            self.module = ModuleConfig(**data["module"])
+        if "path" in data:
+            self.path = BatchPathConfig(**data["path"])
+        if "project" in data:
+            self.project = ProjectConfig(**data["project"])
 
     @property
     def config(self):
-        return self._config_
+        return self.dict()
 
     @property
     def root_dir(self) -> Path:
-        return Path(self.path.root)
+        return self.path.root_dir
 
     @property
-    def output_dir(self):
+    def output_dir(self) -> Path:
         return self.path.output_dir
 
     @property
     def project_name(self):
         return self.project.project_name
 
     @property
-    def project_dir(self):
-        return Path(self.project.project_dir)
+    def project_dir(self) -> Path:
+        return Path(self.project.project_root)
 
     @property
-    def workspace_dir(self):
+    def workspace_dir(self) -> Path:
         return Path(self.project.project_workspace_dir)
 
     @property
-    def model_dir(self):
+    def model_dir(self) -> Path:
         return self.path.model_dir
 
     @property
-    def log_dir(self):
+    def log_dir(self) -> Path:
         return self.project.path.log_dir
 
     @property
-    def cache_dir(self):
-        cache_dir = Path(self.project.path.global_cache)
-        if cache_dir is None:
-            cache_dir = self.output_dir / ".cache"
-            cache_dir.mkdir(parents=True, exist_ok=True)
-        return Path(cache_dir)
+    def cache_dir(self) -> Path:
+        return self.project.path.cache_dir
 
     @property
-    def library_dir(self):
+    def library_dir(self) -> Path:
         return self.path.library_dir
 
     @property
-    def verbose(self):
-        return self.project.verbose
-
-    def autorun(self):
-        return Composer.methods(self.auto, self)
+    def verbose(self) -> bool:
+        return bool(self.project.verbose)
 
-    def show_config(self):
-        Composer.print(self.dict())
+    def print_config(self):
+        Composer.print(self.config)
 
     def load_modules(self):
         """Load the modules"""
-        if self.module.get("modules") is None:
+        if not self.module.modules:
             logger.info("No modules to load")
             return
         library_dir = self.library_dir
         for module in self.module.modules:
             name = module.name
             libname = module.libname
             liburi = module.liburi
             specname = module.specname
             libpath = library_dir / libname
             syspath = module.get("syspath")
             if syspath is not None:
                 syspath = library_dir / syspath
             ensure_import_module(name, libpath, liburi, specname, syspath)
 
-    def reset(self, objects=None):
+    def reset(self, objects=None, release_gpu_memory=True):
         """Reset the memory cache"""
         if isinstance(objects, list):
             for obj in objects:
                 del obj
-        with contextlib.suppress(ImportError):
+        if release_gpu_memory:
             from hyfi.utils.gpu import GPUMon
 
             GPUMon.release_gpu_memory()
```

### Comparing `hyfi-0.7.2/src/hyfi/task/batch.py` & `hyfi-0.8.0/src/hyfi/task/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from hyfi.task import TaskConfig
 from hyfi.utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 class BatchTaskConfig(TaskConfig):
+    batch_name: str = "demo"
     batch: BatchConfig = None  # type: ignore
 
     class Config:
         arbitrary_types_allowed = True
         extra = "allow"
         validate_assignment = False
         exclude = {
@@ -33,43 +34,42 @@
             "batch_num": "set_batch_num",
             "root_dir": "set_root_dir",
         }
 
     def __init__(self, **args):
         super().__init__(**args)
 
-    def set_name(self, val):
-        super().set_name(val)
+    def set_batch_name(self, val):
+        super().set_task_name(val)
         self._config_.batch.batch_name = val
         self.batch.batch_name = val
         self.initialize_configs(name=val)
 
     def set_batch_num(self, val):
         self._config_.batch.batch_num = val
         self.batch.batch_num = val
 
     def initialize_configs(
-        self, root_dir=None, batch_config_class=BatchConfig, **kwargs
+        self,
+        task_root: str = "",
+        batch_config_class=BatchConfig,
+        **kwargs,
     ):
-        super().initialize_configs(root_dir=root_dir, **kwargs)
+        super().initialize_configs(task_root=task_root, **kwargs)
 
         self.batch = batch_config_class(**self.config.batch)
         self.batch_num = self.batch.batch_num
         # if self.project.use_huggingface_hub:
         #     self.secrets.init_huggingface_hub()
         if self.verbose:
             logger.info(
                 f"Initalized batch: {self.batch_name}({self.batch_num}) in {self.root_dir}"
             )
 
     @property
-    def batch_name(self):
-        return self.batch.batch_name
-
-    @property
     def batch_num(self):
         return self.batch.batch_num
 
     @property
     def seed(self):
         return self.batch.seed
```

### Comparing `hyfi-0.7.2/src/hyfi/utils/env.py` & `hyfi-0.8.0/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/utils/func.py` & `hyfi-0.8.0/src/hyfi/utils/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,28 +270,34 @@
             for _col in _columns:
                 data[_col] = pd.to_datetime(data[_col], format=_format, **kwargs)
         return data
     else:
         return data
 
 
-def to_numeric(data, _columns=None, errors="coerce", downcast=None, **kwargs):
+def to_numeric(
+    data,
+    _columns=None,
+    errors="coerce",
+    downcast=None,
+    **kwargs,
+):
     """Convert a string, int, or float object to a float object"""
     import pandas as pd
 
     if isinstance(data, str):
         return float(data)
     elif isinstance(data, (int, float)) or not isinstance(data, pd.DataFrame):
         return data
     else:
         if _columns:
             if isinstance(_columns, str):
                 _columns = [_columns]
             for _col in _columns:
-                data[_col] = pd.to_numeric(data[_col], errors=errors, downcast=downcast)
+                data[_col] = pd.to_numeric(data[_col], errors=errors, downcast=downcast)  # type: ignore
         return data
 
 
 def human_readable_type_name(t: Type) -> str:
     """
     Generates a useful-for-humans label for a type.
     For builtin types, it's just the class name (eg "str" or "int").
@@ -321,23 +327,33 @@
      {'character': 'a', 'number': 2},
      {'character': 'b', 'number': 1},
      {'character': 'b', 'number': 2}]
     """
     return (dict(zip(dicts, x)) for x in itertools.product(*dicts.values()))
 
 
-def dict_to_dataframe(data, orient="columns", dtype=None, columns=None):
+def dict_to_dataframe(
+    data,
+    orient="columns",
+    dtype=None,
+    columns=None,
+):
     """Convert a dictionary to a pandas dataframe"""
     import pandas as pd
 
-    return pd.DataFrame.from_dict(data, orient=orient, dtype=dtype, columns=columns)
+    return pd.DataFrame.from_dict(data, orient=orient, dtype=dtype, columns=columns)  # type: ignore
 
 
 def records_to_dataframe(
-    data, index=None, exclude=None, columns=None, coerce_float=False, nrows=None
+    data,
+    index=None,
+    exclude=None,
+    columns=None,
+    coerce_float=False,
+    nrows=None,
 ):
     """Convert a list of records to a pandas dataframe"""
     import pandas as pd
 
     return pd.DataFrame.from_records(
         data,
         index=index,
```

### Comparing `hyfi-0.7.2/src/hyfi/utils/google.py` & `hyfi-0.8.0/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/utils/gpu.py` & `hyfi-0.8.0/src/hyfi/utils/gpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,14 +111,18 @@
         import torch  # type: ignore
 
         return torch.cuda.is_available()
     except ImportError:
         return False
 
 
+class CudaDeviceNotFoundError(Exception):
+    pass
+
+
 def set_cuda(device=0):
     """Set cuda device to use"""
     try:
         import torch  # type: ignore
 
         _names = []
         if isinstance(device, str):
@@ -131,8 +135,8 @@
             _names.append(f"{_device_name} (id:{id})")
         logger.info(f"Setting cuda device to {_names}")
         device = ", ".join(ids)
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = device
     except ImportError as e:
         os.environ["CUDA_VISIBLE_DEVICES"] = ""
-        raise Exception("Cuda device not found") from e
+        raise CudaDeviceNotFoundError("Cuda device not found") from e
```

### Comparing `hyfi-0.7.2/src/hyfi/utils/lib.py` & `hyfi-0.8.0/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.7.2/src/hyfi/utils/logging.py` & `hyfi-0.8.0/src/hyfi/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         The logger that was
     """
     level = level or os.environ.get("HYFI_LOG_LEVEL") or "INFO"
     level = level.upper()
     os.environ["HYFI_LOG_LEVEL"] = level
     # Filter warnings by applying filterwarnings_action to the warnings.
     if filterwarnings_action is not None:
-        warnings.filterwarnings(filterwarnings_action)
+        warnings.filterwarnings(filterwarnings_action)  # type: ignore
     # Return the logging level.
     if isinstance(level, str):
         level = getattr(logging, level.upper(), logging.INFO)
     # Configure logging level level and force logging.
     if sys.version_info >= (3, 8):
         logging.basicConfig(level=level, force=force, **kwargs)
     else:
```

### Comparing `hyfi-0.7.2/src/hyfi/utils/notebook.py` & `hyfi-0.8.0/src/hyfi/utils/notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Utilities for working with notebooks.""" ""
+import contextlib
 import logging
 import os
 import sys
 
 from hyfi.utils.file import read
 
 logger = logging.getLogger(__name__)
 
 
 def is_notebook():
     """Check if the code is running in a notebook."""
     try:
-        get_ipython
+        get_ipython  # type: ignore
     except NameError:
         return False
     # pylint: disable=undefined-variable
-    shell_type = get_ipython().__class__.__name__  # noqa
+    shell_type = get_ipython().__class__.__name__  # type: ignore # noqa
     # logger.info(f"shell type: {shell_type}")
     return shell_type in ["ZMQInteractiveShell", "Shell"]
 
 
 def is_colab():
     """Check if the code is running in Google Colab."""
     is_colab = "google.colab" in sys.modules
@@ -177,27 +178,28 @@
 def colored_str(s, color="black"):
     """Colored string."""
     # return "<text style=color:{}>{}</text>".format(color, s)
     return "<text style=color:{}>{}</text>".format(color, s.replace("\n", "<br>"))
 
 
 def cprint(str_tuples):
-    from IPython.display import HTML as html_print
+    from IPython.core.display import HTML as html_print
     from IPython.display import display
 
     display(html_print(" ".join([colored_str(ti, color=ci) for ti, ci in str_tuples])))
 
 
 def create_dropdown(
     options, value, description, disabled=False, style=None, layout=None, **kwargs
 ):
     """Create a dropdown widget."""
+    import ipywidgets as widgets
+
     if style is None:
         style = {"description_width": "initial"}
-    import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
     return widgets.Dropdown(
         options=options,
         value=value,
@@ -215,17 +217,18 @@
     placeholder="",
     disabled=False,
     style=None,
     layout=None,
     **kwargs,
 ):
     """Create a textarea widget."""
+    import ipywidgets as widgets
+
     if style is None:
         style = {"description_width": "initial"}
-    import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
     return widgets.Textarea(
         value=value,
         placeholder=placeholder,
@@ -253,17 +256,18 @@
     )
 
 
 def create_radiobutton(
     options, description, value=None, disabled=False, style=None, layout=None, **kwargs
 ):
     """Create a radiobutton widget."""
+    import ipywidgets as widgets
+
     if style is None:
         style = {"description_width": "initial"}
-    import ipywidgets as widgets
 
     layout = (
         widgets.Layout(width="auto") if layout is None else widgets.Layout(**layout)
     )
     return widgets.RadioButtons(
         options=options,
         value=value,
@@ -346,29 +350,32 @@
 
 def load_extentions(exts=None):
     """Load extentions."""
     if exts is None:
         exts = ["autotime"]
     if not is_notebook():
         return
-    from IPython import get_ipython
+    with contextlib.suppress(ImportError):
+        from IPython.core.getipython import get_ipython
 
-    ip = get_ipython()
-    try:
-        loaded = ip.extension_manager.loaded
-        for ext in exts:
-            if ext not in loaded:
-                ip.extentension_manager.load_extension(ext)
-    except AttributeError:
-        for ext in exts:
-            try:
-                ip.magic(f"load_ext {ext}")
-            except ModuleNotFoundError:
-                logger.info("Extension %s not found. Install it first.", ext)
+        ip = get_ipython()
+        if ip is None:
+            return
+        try:
+            loaded = ip.extension_manager.loaded
+            for ext in exts:
+                if ext not in loaded:
+                    ip.extentension_manager.load_extension(ext)
+        except AttributeError:
+            for ext in exts:
+                try:
+                    ip.magic(f"load_ext {ext}")
+                except ModuleNotFoundError:
+                    logger.info("Extension %s not found. Install it first.", ext)
 
 
 def set_matplotlib_formats(*formats, **kwargs):
     """Set matplotlib formats."""
     if is_notebook():
-        from IPython.display import set_matplotlib_formats
+        from IPython.core.display import set_matplotlib_formats
 
         set_matplotlib_formats(*formats, **kwargs)
```

### Comparing `hyfi-0.7.2/src/hyfi/utils/tools.py` & `hyfi-0.8.0/src/hyfi/utils/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 colorama.init()
 
 
 class Style:
     """Common color styles."""
 
-    OK: IntSeq = [colorama.Fore.GREEN, colorama.Style.BRIGHT]
-    WARNING: IntSeq = [colorama.Fore.YELLOW, colorama.Style.BRIGHT]
-    IGNORE: IntSeq = [colorama.Fore.CYAN]
-    DANGER: IntSeq = [colorama.Fore.RED, colorama.Style.BRIGHT]
-    RESET: IntSeq = [colorama.Fore.RESET, colorama.Style.RESET_ALL]
+    OK: IntSeq = [colorama.Fore.GREEN, colorama.Style.BRIGHT]  # type: ignore
+    WARNING: IntSeq = [colorama.Fore.YELLOW, colorama.Style.BRIGHT]  # type: ignore
+    IGNORE: IntSeq = [colorama.Fore.CYAN]  # type: ignore
+    DANGER: IntSeq = [colorama.Fore.RED, colorama.Style.BRIGHT]  # type: ignore
+    RESET: IntSeq = [colorama.Fore.RESET, colorama.Style.RESET_ALL]  # type: ignore
 
 
 INDENT = " " * 2
 HLINE = "-" * 42
 
 NO_VALUE: object = object()
 
@@ -48,15 +48,15 @@
     if not verbose:
         return None  # HACK: Satisfy MyPy
     _msg = str(msg)
     action = action.rjust(indent, " ")
     if not style:
         return action + _msg
 
-    out = style + [action] + Style.RESET + [INDENT, _msg]
+    out = style + [action] + Style.RESET + [INDENT, _msg]  # type: ignore
     print(*out, sep="", file=file_)
     return None  # HACK: Satisfy MyPy
 
 
 def printf_exception(
     e: Exception, action: str, msg: str = "", indent: int = 0, quiet: bool = False
 ) -> None:
@@ -104,15 +104,15 @@
 def force_str_end(original_str: str, end: str = "\n") -> str:
     """Make sure a `original_str` ends with `end`.
 
     Params:
         original_str: String that you want to ensure ending.
         end: String that must exist at the end of `original_str`
     """
-    return original_str + end if not original_str.endswith(end) else original_str
+    return original_str if original_str.endswith(end) else original_str + end
 
 
 def handle_remove_readonly(
     func: Callable, path: str, exc: Tuple[BaseException, OSError, TracebackType]
 ) -> None:
     """Handle errors when trying to remove read-only files through `shutil.rmtree`.
 
@@ -145,15 +145,15 @@
     @classmethod
     def _cleanup(cls, name, warn_message):
         cls._robust_cleanup(name)
         warnings.warn(warn_message, ResourceWarning)
 
     def cleanup(self):
         """Remove directory safely."""
-        if self._finalizer.detach():
+        if self._finalizer.detach():  # type: ignore
             self._robust_cleanup(self.name)
 
     @staticmethod
     def _robust_cleanup(name):
         shutil.rmtree(name, ignore_errors=False, onerror=handle_remove_readonly)
```

### Comparing `hyfi-0.7.2/PKG-INFO` & `hyfi-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.7.2
+Version: 0.8.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

