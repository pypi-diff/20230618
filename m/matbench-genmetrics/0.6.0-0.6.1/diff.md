# Comparing `tmp/matbench-genmetrics-0.6.0.tar.gz` & `tmp/matbench-genmetrics-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matbench-genmetrics-0.6.0.tar", last modified: Wed Aug 10 06:58:57 2022, max compression
+gzip compressed data, was "matbench-genmetrics-0.6.1.tar", last modified: Sat Jun 17 22:25:25 2023, max compression
```

## Comparing `matbench-genmetrics-0.6.0.tar` & `matbench-genmetrics-0.6.1.tar`

### file list

```diff
@@ -1,82 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.451705 matbench-genmetrics-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     4082 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    13633 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     2219 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12844 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11849 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/configs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/data/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/data/external/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/data/external/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/data/interim/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/data/interim/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/data/processed/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/data/processed/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/data/raw/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/data/raw/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)    10379 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)     3410 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (121)    82413 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/models/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/models/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)    57800 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/notebooks/1.0-matbench-genmetrics-basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/notebooks/template.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/references/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/references/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.451705 matbench-genmetrics-0.6.0/reports/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/reports/figures/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/reports/figures/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    82413 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/reports/figures/metrics.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.455705 matbench-genmetrics-0.6.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/scripts/fingerprint_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/scripts/matbench_genmetrics_100.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/scripts/matbench_genmetrics_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/scripts/run_grayskull.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/scripts/train_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/scripts/validity_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.451705 matbench-genmetrics-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/src/matbench_genmetrics/
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24964 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/src/matbench_genmetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     5539 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics/utils/featurize.py
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics/utils/match.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12844 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-10 06:58:57.000000 matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 06:58:57.459705 matbench-genmetrics-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8055 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/tests/test_matbench_genmetrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-08-10 06:58:07.000000 matbench-genmetrics-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.629716 matbench-genmetrics-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.581715 matbench-genmetrics-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.597715 matbench-genmetrics-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13633 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-06-17 22:25:25.629716 matbench-genmetrics-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.597715 matbench-genmetrics-0.6.1/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/configs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.597715 matbench-genmetrics-0.6.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.601716 matbench-genmetrics-0.6.1/data/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/data/external/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.601716 matbench-genmetrics-0.6.1/data/interim/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/data/interim/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.601716 matbench-genmetrics-0.6.1/data/processed/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/data/processed/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.601716 matbench-genmetrics-0.6.1/data/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/data/raw/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.609716 matbench-genmetrics-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.609716 matbench-genmetrics-0.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)  2319456 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.609716 matbench-genmetrics-0.6.1/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/models/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.585715 matbench-genmetrics-0.6.1/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.609716 matbench-genmetrics-0.6.1/notebooks/core/
+-rw-r--r--   0 runner    (1001) docker     (123)   505953 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/notebooks/core/1.0-matbench-genmetrics-basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/notebooks/core/template.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.613716 matbench-genmetrics-0.6.1/notebooks/mp_time_split/
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/notebooks/mp_time_split/1.0-basic-usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1293531 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/notebooks/mp_time_split/mp-api-colab-py38.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/notebooks/mp_time_split/template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.613716 matbench-genmetrics-0.6.1/references/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/references/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.613716 matbench-genmetrics-0.6.1/reports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.617716 matbench-genmetrics-0.6.1/reports/equations/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/equations/coverage.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/equations/novelty.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/equations/uniqueness.tex
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/equations/validity.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    51270 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/equations.nb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.621716 matbench-genmetrics-0.6.1/reports/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/figures/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)  2319456 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/figures/matbench-genmetrics.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82413 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/figures/metrics.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/matbench-genmetrics.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    31055 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/reports/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.585715 matbench-genmetrics-0.6.1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.621716 matbench-genmetrics-0.6.1/scripts/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/fingerprint_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/load_imagen_pytorch_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/matbench_genmetrics_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/matbench_genmetrics_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/run_grayskull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/train_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/core/validity_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.621716 matbench-genmetrics-0.6.1/scripts/mp_time_split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/mp_time_split/data_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/mp_time_split/run_grayskull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/scripts/mp_time_split/train_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-17 22:25:25.629716 matbench-genmetrics-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.585715 matbench-genmetrics-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.585715 matbench-genmetrics-0.6.1/src/matbench_genmetrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.625716 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35505 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.625716 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/utils/featurize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/utils/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.625716 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.625716 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37847 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/mp_dummy_time_summary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/mp_dummy_time_summary.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics/mp_time_split/utils/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.625716 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 22:25:25.000000 matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 22:25:25.629716 matbench-genmetrics-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/tests/test_matbench_genmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/tests/test_mp_time_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-17 22:24:21.000000 matbench-genmetrics-0.6.1/tox.ini
```

### Comparing `matbench-genmetrics-0.6.0/.coveragerc` & `matbench-genmetrics-0.6.1/.coveragerc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # .coveragerc to control coverage.py
 [run]
 branch = True
-source = matbench_genmetrics
+source = matbench_genmetrics.core
 # omit = bad_file.py
 
 [paths]
 source =
     src/
     */site-packages/
```

### Comparing `matbench-genmetrics-0.6.0/.github/workflows/ci.yml` & `matbench-genmetrics-0.6.1/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,98 +13,112 @@
   pull_request:  # Run in every PR
   workflow_dispatch:  # Allow manually triggering the workflow
   schedule:
     # Run roughly every 15 days at 00:00 UTC
     # (useful to check if updates on dependencies break the package)
     - cron: '0 0 1,16 * *'
 
+permissions:
+  contents: read
+
 concurrency:
   group: >-
     ${{ github.workflow }}-${{ github.ref_type }}-
     ${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
 
 jobs:
   prepare:
     runs-on: ubuntu-latest
     outputs:
       wheel-distribution: ${{ steps.wheel-distribution.outputs.path }}
     steps:
       - uses: actions/checkout@v3
         with: {fetch-depth: 0}  # deep clone for setuptools-scm
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
+        id: setup-python
         with: {python-version: "3.10"}
       - name: Run static analysis and format checkers
         run: pipx run pre-commit run --all-files --show-diff-on-failure
       - name: Build package distribution files
-        run: pipx run tox -e clean,build
+        run: >-
+          pipx run --python '${{ steps.setup-python.outputs.python-path }}'
+          tox -e clean,build
       - name: Record the path of wheel distribution
         id: wheel-distribution
-        run: echo "::set-output name=path::$(ls dist/*.whl)"
+        run: echo "path=$(ls dist/*.whl)" >> $GITHUB_OUTPUT
       - name: Store the distribution files for use in other stages
         # `tests` and `publish` will use the same pre-built distributions,
         # so we make sure to release the exact same package that was tested
         uses: actions/upload-artifact@v3
         with:
           name: python-distribution-files
           path: dist/
           retention-days: 1
 
   test:
     needs: prepare
     strategy:
       matrix:
         python:
-        - "3.7"  # oldest Python supported by PSF
+        - "3.8"  # oldest Python supported by PSF
         - "3.10"  # newest Python that is stable
         platform:
         - ubuntu-latest
         # - macos-latest
         # - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
+        id: setup-python
         with:
           python-version: ${{ matrix.python }}
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
+      - name: Install mp-api
+        run: pip install mp-api
       - name: Run tests
+        env:
+          MP_API_KEY: ${{ secrets.MP_API_KEY }}
         run: >-
-          pipx run tox
-          --installpkg '${{ needs.prepare.outputs.wheel-distribution }}'
-          -- -rFEx --durations 10 --color yes
+          pipx run --python '${{ steps.setup-python.outputs.python-path }}'
+          tox --installpkg '${{ needs.prepare.outputs.wheel-distribution }}'
+          -- -rFEx --durations 10 --color yes  # pytest args
       - name: Generate coverage report
         run: pipx run coverage lcov -o coverage.lcov
       - name: Upload partial coverage report
         uses: coverallsapp/github-action@master
         with:
           path-to-lcov: coverage.lcov
           github-token: ${{ secrets.github_token }}
           flag-name: ${{ matrix.platform }} - py${{ matrix.python }}
           parallel: true
 
   finalize:
     needs: test
     runs-on: ubuntu-latest
+
     steps:
       - name: Finalize coverage report
         uses: coverallsapp/github-action@master
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           parallel-finished: true
 
   publish:
     needs: finalize
     if: ${{ github.event_name == 'push' && contains(github.ref, 'refs/tags/') }}
     runs-on: ubuntu-latest
+    permissions:
+      contents: write
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         with: {python-version: "3.10"}
       - name: Retrieve pre-built distribution files
         uses: actions/download-artifact@v3
         with: {name: python-distribution-files, path: dist/}
       - name: Publish Package
         env:
           # TODO: Set your PYPI_TOKEN as a secret using GitHub UI
```

### Comparing `matbench-genmetrics-0.6.0/.pre-commit-config.yaml` & `matbench-genmetrics-0.6.1/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
     args: ['--maxkb=10000']
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
@@ -16,47 +16,47 @@
   - id: end-of-file-fixer
   - id: requirements-txt-fixer
   - id: mixed-line-ending
     args: ['--fix=auto']  # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
 # If you want to avoid flake8 errors due to unused vars or imports:
 - repo: https://github.com/myint/autoflake
-  rev: v1.4
+  rev: v2.1.1
   hooks:
   - id: autoflake
     args: [
       --in-place,
       --remove-all-unused-imports,
       # --remove-unused-variables,
     ]
 
 - repo: https://github.com/pycqa/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 23.3.0
   hooks:
   - id: black
     language_version: python3
 
 # If like to embrace black styles even in the docs:
 - repo: https://github.com/asottile/blacken-docs
-  rev: v1.12.1
+  rev: 1.13.0
   hooks:
   - id: blacken-docs
     name: blacken-docs
     description: Run `black` on python code blocks in documentation files
     additional_dependencies: [black]
     entry: blacken-docs
     language: python
     language_version: python3
     files: '\.(rst|md|markdown|py|tex)$'
     args: ["--skip-errors"]
 
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 6.0.0
   hooks:
   - id: flake8
   ## You can add flake8 plugins via `additional_dependencies`:
   #  additional_dependencies: [flake8-bugbear]
```

### Comparing `matbench-genmetrics-0.6.0/CONTRIBUTING.md` & `matbench-genmetrics-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `matbench-genmetrics-0.6.0/Dockerfile` & `matbench-genmetrics-0.6.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `matbench-genmetrics-0.6.0/LICENSE.txt` & `matbench-genmetrics-0.6.1/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 sgbaird
+Copyright (c) 2023 sgbaird
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `matbench-genmetrics-0.6.0/PKG-INFO` & `matbench-genmetrics-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matbench-genmetrics
-Version: 0.6.0
+Version: 0.6.1
 Summary: Generative materials benchmarking metrics, inspired by CDVAE.
 Home-page: https://github.com/sparks-baird/matbench-genmetrics/
 Author: sgbaird
 Author-email: sterling.baird@utah.edu
 License: MIT
 Project-URL: Documentation, https://matbench-genmetrics.readthedocs.io
 Project-URL: Source, https://github.com/sparks-baird/matbench-genmetrics
@@ -13,14 +13,15 @@
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/matbench-genmetrics
 Project-URL: Download, https://pypi.org/project/matbench-genmetrics/#files
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: api
 Provides-Extra: dev
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![ReadTheDocs](https://readthedocs.org/projects/matbench-genmetrics/badge/?version=latest)](https://matbench-genmetrics.readthedocs.io/en/stable/)
 [![Coveralls](https://img.shields.io/coveralls/github/sparks-baird/matbench-genmetrics/main.svg)](https://coveralls.io/r/sparks-baird/matbench-genmetrics)
@@ -29,28 +30,30 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/matbench-genmetrics)
 ![Lines of code](https://img.shields.io/tokei/lines/github/sparks-baird/matbench-genmetrics)
 <!-- These are examples of badges you might also want to add to your README. Update the URLs accordingly.
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/matbench-genmetrics.svg?branch=main)](https://cirrus-ci.com/github/<USER>/matbench-genmetrics)
 [![Monthly Downloads](https://pepy.tech/badge/matbench-genmetrics/month)](https://pepy.tech/project/matbench-genmetrics)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/matbench-genmetrics)
 -->
-> **NOTE: This is a WIP repository (as of 2022-08-06) being developed in parallel with [`xtal2png`](https://github.com/sparks-baird/xtal2png) and [`mp-time-split`](https://github.com/sparks-baird/mp-time-split). Feedback and contributions welcome!**
-# matbench-genmetrics
+<!--- > **NOTE: This is a WIP repository (as of 2022-08-06) being developed in parallel with [`xtal2png`](https://github.com/sparks-baird/xtal2png) and [`mp-time-split`](https://github.com/sparks-baird/mp-time-split). Feedback and contributions welcome!** --->
+> **This is not an official repository of Matbench, but eventually, it may be [incorporated into Matbench](https://github.com/materialsproject/matbench/issues/150)**
 
+# matbench-genmetrics [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sparks-baird/matbench-genmetrics/blob/main/notebooks/1.0-matbench-genmetrics-basic.ipynb)
 > Generative materials benchmarking metrics, inspired by [guacamol](https://www.benevolent.com/guacamol) and [CDVAE](https://github.com/txie-93/cdvae).
 
 This repository provides standardized benchmarks for benchmarking generative models for
 crystal structure. Each benchmark has a fixed dataset, a predefined split, and a notion
 of best (i.e. metric) associated with it.
 
-<p align="center"><img src="https://github.com/sparks-baird/matbench-genmetrics/raw/main/reports/figures/metrics.png" width=450></p>
+<p align="center"><img src="https://github.com/sparks-baird/matbench-genmetrics/raw/main/reports/figures/matbench-genmetrics.png" width=450></p>
 
 ## Getting Started
 
 Installation, a dummy example, output metrics for the example, and descriptions of the benchmark metrics.
+
 ### Installation
 
 Create a conda environment with the `matbench-genmetrics` package installed from the
 `conda-forge` channel. Then activate the environment.
 
 > **NOTE: not available on conda-forge as of 2022-07-30, recipe under review by
 > conda-forge team. So use `pip install matbench-genmetrics` for now
@@ -74,15 +77,15 @@
 >>> from matbench_genmetrics.core import MPTSMetrics10, MPTSMetrics100, MPTSMetrics1000, MPTSMetrics10000
 >>> mptm = MPTSMetrics10(dummy=True)
 >>> for fold in mptm.folds:
 >>>     train_val_inputs = mptm.get_train_and_val_data(fold)
 >>>     dg = DummyGenerator()
 >>>     dg.fit(train_val_inputs)
 >>>     gen_structures = dg.gen(n=mptm.num_gen)
->>>     mptm.record(fold, gen_structures)
+>>>     mptm.evaluate_and_record(fold, gen_structures)
 ```
 
 ### Output
 
 ```python
 print(mptm.recorded_metrics)
 ```
@@ -120,53 +123,56 @@
         "uniqueness": 0.9111111111111111,
     },
 }
 ```
 
 ### Metrics
 
-| Metric | Description |
-|---|---|
-| Validity | One minus (Wasserstein distance between distribution of space group numbers for train and generated structures divided by distance of dummy case between train and `space_group_number == 1`). See also https://github.com/sparks-baird/matbench-genmetrics/issues/44 |
-| Coverage | Match counts between held-out test structures and generated structures divided by number of test structures ("predict the future"). |
-| Novelty | One minus (match counts between train structures and generated structures divided by number of generated structures). |
-| Uniqueness | One minus (non-self-comparing match counts within generated structures divided by total possible non-self-comparing matches). |
+| Metric     | Description                                                                                                                                                                                                                                                             |
+| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Validity   | One minus (Wasserstein distance between distribution of space group numbers for train and generated structures divided by distance of dummy case between train and `space_group_number == 1`). See also <https://github.com/sparks-baird/matbench-genmetrics/issues/44> |
+| Coverage   | Match counts between held-out test structures and generated structures divided by number of test structures ("predict the future").                                                                                                                                     |
+| Novelty    | One minus (match counts between train structures and generated structures divided by number of generated structures).                                                                                                                                                   |
+| Uniqueness | One minus (non-self-comparing match counts within generated structures divided by total possible non-self-comparing matches).                                                                                                                                           |
+
+A match is when <code><a href="https://pymatgen.org/pymatgen.analysis.structure_matcher.html#pymatgen.analysis.structure_matcher.StructureMatcher">StructureMatcher</a>(stol=0.5, ltol=0.3, angle_tol=10.0).fit(s1, s2)</code> evaluates to `True`.
+
+Detailed descriptions of the metrics are given in https://self-driving-lab-demo.readthedocs.io/en/latest/metrics.html.
+
 
-A match is when [`StructureMatcher`](https://pymatgen.org/pymatgen.analysis.structure_matcher.html#pymatgen.analysis.structure_matcher.StructureMatcher)`(stol=0.5, ltol=0.3, angle_tol=10.0).fit(s1, s2)`
-evaluates to `True`.
 
 ## Advanced Installation
 
 ### Anaconda (`conda`) installation (recommended)
 
-(2022-07-30, conda-forge installation pending, fallback to `pip install xtal2png` as separate command)
+(2022-07-30, conda-forge installation pending, fallback to `pip install matbench-genmetrics` as separate command)
 
-Create and activate a new `conda` environment named `xtal2png` (`-n`) that will search for and install the `xtal2png` package from the `conda-forge` Anaconda channel (`-c`).
+Create and activate a new `conda` environment named `matbench-genmetrics` (`-n`) that will search for and install the `matbench-genmetrics` package from the `conda-forge` Anaconda channel (`-c`).
 
 ```bash
-conda env create -n xtal2png -c conda-forge xtal2png
-conda activate xtal2png
+conda env create -n matbench-genmetrics -c conda-forge matbench-genmetrics
+conda activate matbench-genmetrics
 ```
 
 Alternatively, in an already activated environment:
 
 ```bash
-conda install -c conda-forge xtal2png
+conda install -c conda-forge matbench-genmetrics
 ```
 
-If you run into conflicts with packages you are integrating with `xtal2png`, please try installing all packages in a single line of code (or two if mixing `conda` and `pip` packages in the same environment) and installing with `mamba` ([source](https://stackoverflow.com/a/69137255/13697228)).
+If you run into conflicts with packages you are integrating with `matbench-genmetrics`, please try installing all packages in a single line of code (or two if mixing `conda` and `pip` packages in the same environment) and installing with `mamba` ([source](https://stackoverflow.com/a/69137255/13697228)).
 
 ### PyPI (`pip`) installation
 
 Create and activate a new `conda` environment named `matbench-genmetrics` (`-n`) with `python==3.9.*` or your preferred Python version, then install `matbench-genmetrics` via `pip`.
 
 ```bash
-conda create -n xtal2png python==3.9.*
-conda activate xtal2png
-pip install xtal2png
+conda create -n matbench-genmetrics python==3.9.*
+conda activate matbench-genmetrics
+pip install matbench-genmetrics
 ```
 
 ## Editable installation
 
 In order to set up the necessary environment:
 
 1. clone and enter the repository via:
@@ -216,25 +222,29 @@
 
 ## Dependency Management & Reproducibility
 
 1. Always keep your abstract (unpinned) dependencies updated in `environment.yml` and eventually
    in `setup.cfg` if you want to ship and install your package via `pip` later on.
 2. Create concrete dependencies as `environment.lock.yml` for the exact reproduction of your
    environment with:
+
    ```bash
    conda env export -n matbench-genmetrics -f environment.lock.yml
    ```
+
    For multi-OS development, consider using `--no-builds` during the export.
 3. Update your current environment with respect to a new `environment.lock.yml` using:
+
    ```bash
    conda env update -f environment.lock.yml --prune
    ```
+
 ## Project Organization
 
-```
+```txt
 ├── AUTHORS.md              <- List of developers and maintainers.
 ├── CHANGELOG.md            <- Changelog to keep track of new features and fixes.
 ├── CONTRIBUTING.md         <- Guidelines for contributing to this project.
 ├── Dockerfile              <- Build a docker container with `docker build .`.
 ├── LICENSE.txt             <- License as chosen on the command-line.
 ├── README.md               <- The top-level README for developers.
 ├── configs                 <- Directory for configurations of model & application.
```

### Comparing `matbench-genmetrics-0.6.0/README.md` & `matbench-genmetrics-0.6.1/src/matbench_genmetrics.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,59 @@
+Metadata-Version: 2.1
+Name: matbench-genmetrics
+Version: 0.6.1
+Summary: Generative materials benchmarking metrics, inspired by CDVAE.
+Home-page: https://github.com/sparks-baird/matbench-genmetrics/
+Author: sgbaird
+Author-email: sterling.baird@utah.edu
+License: MIT
+Project-URL: Documentation, https://matbench-genmetrics.readthedocs.io
+Project-URL: Source, https://github.com/sparks-baird/matbench-genmetrics
+Project-URL: Changelog, https://matbench-genmetrics.readthedocs.io/latest/changelog.html
+Project-URL: Tracker, https://github.com/sparks-baird/matbench-genmetrics/issues
+Project-URL: Conda-Forge, https://anaconda.org/conda-forge/matbench-genmetrics
+Project-URL: Download, https://pypi.org/project/matbench-genmetrics/#files
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: api
+Provides-Extra: dev
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![ReadTheDocs](https://readthedocs.org/projects/matbench-genmetrics/badge/?version=latest)](https://matbench-genmetrics.readthedocs.io/en/stable/)
 [![Coveralls](https://img.shields.io/coveralls/github/sparks-baird/matbench-genmetrics/main.svg)](https://coveralls.io/r/sparks-baird/matbench-genmetrics)
 [![PyPI-Server](https://img.shields.io/pypi/v/matbench-genmetrics.svg)](https://pypi.org/project/matbench-genmetrics/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/matbench-genmetrics.svg)](https://anaconda.org/conda-forge/matbench-genmetrics)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/matbench-genmetrics)
 ![Lines of code](https://img.shields.io/tokei/lines/github/sparks-baird/matbench-genmetrics)
 <!-- These are examples of badges you might also want to add to your README. Update the URLs accordingly.
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/matbench-genmetrics.svg?branch=main)](https://cirrus-ci.com/github/<USER>/matbench-genmetrics)
 [![Monthly Downloads](https://pepy.tech/badge/matbench-genmetrics/month)](https://pepy.tech/project/matbench-genmetrics)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/matbench-genmetrics)
 -->
-> **NOTE: This is a WIP repository (as of 2022-08-06) being developed in parallel with [`xtal2png`](https://github.com/sparks-baird/xtal2png) and [`mp-time-split`](https://github.com/sparks-baird/mp-time-split). Feedback and contributions welcome!**
-# matbench-genmetrics
+<!--- > **NOTE: This is a WIP repository (as of 2022-08-06) being developed in parallel with [`xtal2png`](https://github.com/sparks-baird/xtal2png) and [`mp-time-split`](https://github.com/sparks-baird/mp-time-split). Feedback and contributions welcome!** --->
+> **This is not an official repository of Matbench, but eventually, it may be [incorporated into Matbench](https://github.com/materialsproject/matbench/issues/150)**
 
+# matbench-genmetrics [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sparks-baird/matbench-genmetrics/blob/main/notebooks/1.0-matbench-genmetrics-basic.ipynb)
 > Generative materials benchmarking metrics, inspired by [guacamol](https://www.benevolent.com/guacamol) and [CDVAE](https://github.com/txie-93/cdvae).
 
 This repository provides standardized benchmarks for benchmarking generative models for
 crystal structure. Each benchmark has a fixed dataset, a predefined split, and a notion
 of best (i.e. metric) associated with it.
 
-<p align="center"><img src="https://github.com/sparks-baird/matbench-genmetrics/raw/main/reports/figures/metrics.png" width=450></p>
+<p align="center"><img src="https://github.com/sparks-baird/matbench-genmetrics/raw/main/reports/figures/matbench-genmetrics.png" width=450></p>
 
 ## Getting Started
 
 Installation, a dummy example, output metrics for the example, and descriptions of the benchmark metrics.
+
 ### Installation
 
 Create a conda environment with the `matbench-genmetrics` package installed from the
 `conda-forge` channel. Then activate the environment.
 
 > **NOTE: not available on conda-forge as of 2022-07-30, recipe under review by
 > conda-forge team. So use `pip install matbench-genmetrics` for now
@@ -51,15 +77,15 @@
 >>> from matbench_genmetrics.core import MPTSMetrics10, MPTSMetrics100, MPTSMetrics1000, MPTSMetrics10000
 >>> mptm = MPTSMetrics10(dummy=True)
 >>> for fold in mptm.folds:
 >>>     train_val_inputs = mptm.get_train_and_val_data(fold)
 >>>     dg = DummyGenerator()
 >>>     dg.fit(train_val_inputs)
 >>>     gen_structures = dg.gen(n=mptm.num_gen)
->>>     mptm.record(fold, gen_structures)
+>>>     mptm.evaluate_and_record(fold, gen_structures)
 ```
 
 ### Output
 
 ```python
 print(mptm.recorded_metrics)
 ```
@@ -97,53 +123,56 @@
         "uniqueness": 0.9111111111111111,
     },
 }
 ```
 
 ### Metrics
 
-| Metric | Description |
-|---|---|
-| Validity | One minus (Wasserstein distance between distribution of space group numbers for train and generated structures divided by distance of dummy case between train and `space_group_number == 1`). See also https://github.com/sparks-baird/matbench-genmetrics/issues/44 |
-| Coverage | Match counts between held-out test structures and generated structures divided by number of test structures ("predict the future"). |
-| Novelty | One minus (match counts between train structures and generated structures divided by number of generated structures). |
-| Uniqueness | One minus (non-self-comparing match counts within generated structures divided by total possible non-self-comparing matches). |
+| Metric     | Description                                                                                                                                                                                                                                                             |
+| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Validity   | One minus (Wasserstein distance between distribution of space group numbers for train and generated structures divided by distance of dummy case between train and `space_group_number == 1`). See also <https://github.com/sparks-baird/matbench-genmetrics/issues/44> |
+| Coverage   | Match counts between held-out test structures and generated structures divided by number of test structures ("predict the future").                                                                                                                                     |
+| Novelty    | One minus (match counts between train structures and generated structures divided by number of generated structures).                                                                                                                                                   |
+| Uniqueness | One minus (non-self-comparing match counts within generated structures divided by total possible non-self-comparing matches).                                                                                                                                           |
+
+A match is when <code><a href="https://pymatgen.org/pymatgen.analysis.structure_matcher.html#pymatgen.analysis.structure_matcher.StructureMatcher">StructureMatcher</a>(stol=0.5, ltol=0.3, angle_tol=10.0).fit(s1, s2)</code> evaluates to `True`.
+
+Detailed descriptions of the metrics are given in https://self-driving-lab-demo.readthedocs.io/en/latest/metrics.html.
+
 
-A match is when [`StructureMatcher`](https://pymatgen.org/pymatgen.analysis.structure_matcher.html#pymatgen.analysis.structure_matcher.StructureMatcher)`(stol=0.5, ltol=0.3, angle_tol=10.0).fit(s1, s2)`
-evaluates to `True`.
 
 ## Advanced Installation
 
 ### Anaconda (`conda`) installation (recommended)
 
-(2022-07-30, conda-forge installation pending, fallback to `pip install xtal2png` as separate command)
+(2022-07-30, conda-forge installation pending, fallback to `pip install matbench-genmetrics` as separate command)
 
-Create and activate a new `conda` environment named `xtal2png` (`-n`) that will search for and install the `xtal2png` package from the `conda-forge` Anaconda channel (`-c`).
+Create and activate a new `conda` environment named `matbench-genmetrics` (`-n`) that will search for and install the `matbench-genmetrics` package from the `conda-forge` Anaconda channel (`-c`).
 
 ```bash
-conda env create -n xtal2png -c conda-forge xtal2png
-conda activate xtal2png
+conda env create -n matbench-genmetrics -c conda-forge matbench-genmetrics
+conda activate matbench-genmetrics
 ```
 
 Alternatively, in an already activated environment:
 
 ```bash
-conda install -c conda-forge xtal2png
+conda install -c conda-forge matbench-genmetrics
 ```
 
-If you run into conflicts with packages you are integrating with `xtal2png`, please try installing all packages in a single line of code (or two if mixing `conda` and `pip` packages in the same environment) and installing with `mamba` ([source](https://stackoverflow.com/a/69137255/13697228)).
+If you run into conflicts with packages you are integrating with `matbench-genmetrics`, please try installing all packages in a single line of code (or two if mixing `conda` and `pip` packages in the same environment) and installing with `mamba` ([source](https://stackoverflow.com/a/69137255/13697228)).
 
 ### PyPI (`pip`) installation
 
 Create and activate a new `conda` environment named `matbench-genmetrics` (`-n`) with `python==3.9.*` or your preferred Python version, then install `matbench-genmetrics` via `pip`.
 
 ```bash
-conda create -n xtal2png python==3.9.*
-conda activate xtal2png
-pip install xtal2png
+conda create -n matbench-genmetrics python==3.9.*
+conda activate matbench-genmetrics
+pip install matbench-genmetrics
 ```
 
 ## Editable installation
 
 In order to set up the necessary environment:
 
 1. clone and enter the repository via:
@@ -193,25 +222,29 @@
 
 ## Dependency Management & Reproducibility
 
 1. Always keep your abstract (unpinned) dependencies updated in `environment.yml` and eventually
    in `setup.cfg` if you want to ship and install your package via `pip` later on.
 2. Create concrete dependencies as `environment.lock.yml` for the exact reproduction of your
    environment with:
+
    ```bash
    conda env export -n matbench-genmetrics -f environment.lock.yml
    ```
+
    For multi-OS development, consider using `--no-builds` during the export.
 3. Update your current environment with respect to a new `environment.lock.yml` using:
+
    ```bash
    conda env update -f environment.lock.yml --prune
    ```
+
 ## Project Organization
 
-```
+```txt
 ├── AUTHORS.md              <- List of developers and maintainers.
 ├── CHANGELOG.md            <- Changelog to keep track of new features and fixes.
 ├── CONTRIBUTING.md         <- Guidelines for contributing to this project.
 ├── Dockerfile              <- Build a docker container with `docker build .`.
 ├── LICENSE.txt             <- License as chosen on the command-line.
 ├── README.md               <- The top-level README for developers.
 ├── configs                 <- Directory for configurations of model & application.
```

### Comparing `matbench-genmetrics-0.6.0/docs/Makefile` & `matbench-genmetrics-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matbench-genmetrics-0.6.0/docs/conf.py` & `matbench-genmetrics-0.6.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,26 +106,26 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "matbench-genmetrics"
-copyright = "2022, sgbaird"
+copyright = "2023, sgbaird"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
 # If you don’t need the separation provided between version and release,
 # just set them both to the same value.
 try:
-    from matbench_genmetrics import __version__ as version
+    from matbench_genmetrics.core import __version__ as version
 except ImportError:
     version = ""
 
 if not version or version.lower() == "unknown":
     version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
 
 release = version
@@ -176,22 +176,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {"sidebar_width": "300px", "page_width": "1200px"}
-
-# html_context = {
-#     "display_github": True,
-#     "github_user": "sgbaird",
-#     "github_repo": "matbench-genmetrics",
-#     "github_version": "main/docs/",
-# }
+# html_theme_options = {"sidebar_width": "300px", "page_width": "1200px"}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
```

### Comparing `matbench-genmetrics-0.6.0/docs/index.md` & `matbench-genmetrics-0.6.1/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-# matbench-genmetrics
+# ⚛️🏋 matbench-genmetrics 🎨📐
 
-[![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+> **Mat**erials **bench**marking **gen**erative **metrics**, inspired by [guacamol](https://www.benevolent.com/guacamol) and [CDVAE](https://github.com/txie-93/cdvae).
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sparks-baird/matbench-genmetrics/blob/main/notebooks/1.0-matbench-genmetrics-basic.ipynb)
 [![ReadTheDocs](https://readthedocs.org/projects/matbench-genmetrics/badge/?version=latest)](https://matbench-genmetrics.readthedocs.io/en/stable/)
-[![Coveralls](https://img.shields.io/coveralls/github/sparks-baird/matbench-genmetrics/main.svg)](https://coveralls.io/r/sparks-baird/matbench-genmetrics)
 [![PyPI-Server](https://img.shields.io/pypi/v/matbench-genmetrics.svg)](https://pypi.org/project/matbench-genmetrics/)
-[![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/matbench-genmetrics.svg)](https://anaconda.org/conda-forge/matbench-genmetrics)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/matbench-genmetrics)
+<!---
+[![Coveralls](https://img.shields.io/coveralls/github/sparks-baird/matbench-genmetrics/main.svg)](https://coveralls.io/r/sparks-baird/matbench-genmetrics)
+[![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
+[![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/matbench-genmetrics.svg)](https://anaconda.org/conda-forge/matbench-genmetrics)
+--->
 
-Generative materials benchmarking metrics, inspired by [guacamol](https://www.benevolent.com/guacamol) and [CDVAE](https://github.com/txie-93/cdvae).
+Many generative models for crystal structure have been developed; however, few
+standardized benchmarks exist, and none exist in a format as easy-to-use as Matbench.
+Here, we introduce matbench-genmetrics, an open-source Python library for benchmarking
+generative models for crystal structures. We incorporate benchmark datasets, splits, and
+metrics inspired by [Crystal Diffusion Variational AutoEncoder (CDVAE)](https://github.com/txie-93/cdvae), which has been
+demonstrated as state-of-the-art in generative crystal structure tasks. We
+provide our own benchmarks using time-series style cross-validation splits from
+Materials Project via our [mp-time-split package](https://mp-time-split.readthedocs.io/en/latest/) and focus on four metrics: validity,
+coverage, novelty, and uniqueness.
 
 <a class="github-button" href="https://github.com/sparks-baird/matbench-genmetrics"
 data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star
 sparks-baird/matbench-genmetrics on GitHub">Star</a>
 <a class="github-button"
 href="https://github.com/sgbaird" data-size="large" data-show-count="true"
 aria-label="Follow @sgbaird on GitHub">Follow @sgbaird</a>
 <a class="github-button" href="https://github.com/sparks-baird/matbench-genmetrics/issues"
 data-icon="octicon-issue-opened" data-size="large" data-show-count="true"
 aria-label="Issue sparks-baird/matbench-genmetrics on GitHub">Issue</a>
 <a class="github-button" href="https://github.com/sparks-baird/matbench-genmetrics/discussions" data-icon="octicon-comment-discussion" data-size="large" aria-label="Discuss sparks-baird/matbench-genmetrics on GitHub">Discuss</a>
 <br><br>
 
-Many generative models for crystal structure have been developed; however, few
-standardized benchmarks exist, and none exist in a format as easy-to-use as Matbench.
-Here, we introduce  matbench-genmetrics, an open-source Python library for benchmarking
-generative models for crystal structures. We incorporate benchmark datasets, splits, and
-metrics inspired by [Crystal Diffusion Variational AutoEncoder (CDVAE)](https://github.com/txie-93/cdvae), which has been
-demonstrated as state-of-the-art in generative crystal structure tasks. We
-provide our own benchmarks using time-series style cross-validation splits from
-Materials Project via our [mp-time-split package](https://mp-time-split.readthedocs.io/en/latest/) and focus on four metrics: validity,
-coverage, novelty, and uniqueness. Finally, we provide a simple example of preparation
-and submission to the  matbench-genmetrics leaderboard using [pyxtal](https://pyxtal.readthedocs.io/en/latest/) for generation.
+<!-- Finally, we provide a simple example of preparation
+and submission to the  matbench-genmetrics leaderboard using [pyxtal](https://pyxtal.readthedocs.io/en/latest/) for generation. -->
 
 ## Contents
 
 ```{toctree}
 :maxdepth: 2
 
 Overview <readme>
+Metrics <metrics>
 Contributions & Help <contributing>
 License <license>
 Authors <authors>
 Changelog <changelog>
 Module Reference <api/modules>
 GitHub Source <https://github.com/sparks-baird/matbench-genmetrics>
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,36 +1,31 @@
-# matbench-genmetrics [![Project generated with PyScaffold](https://
-img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://
-pyscaffold.org/) [![ReadTheDocs](https://readthedocs.org/projects/matbench-
-genmetrics/badge/?version=latest)](https://matbench-genmetrics.readthedocs.io/
-en/stable/) [![Coveralls](https://img.shields.io/coveralls/github/sparks-baird/
-matbench-genmetrics/main.svg)](https://coveralls.io/r/sparks-baird/matbench-
-genmetrics) [![PyPI-Server](https://img.shields.io/pypi/v/matbench-
-genmetrics.svg)](https://pypi.org/project/matbench-genmetrics/) [![Conda-Forge]
-(https://img.shields.io/conda/vn/conda-forge/matbench-genmetrics.svg)](https://
-anaconda.org/conda-forge/matbench-genmetrics) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/matbench-genmetrics) Generative materials benchmarking
-metrics, inspired by [guacamol](https://www.benevolent.com/guacamol) and
-[CDVAE](https://github.com/txie-93/cdvae). Star Follow_@sgbaird Issue Discuss
+# âï¸ð matbench-genmetrics ð¨ð > **Mat**erials **bench**marking
+**gen**erative **metrics**, inspired by [guacamol](https://www.benevolent.com/
+guacamol) and [CDVAE](https://github.com/txie-93/cdvae). [![Open In Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/sparks-baird/matbench-genmetrics/blob/main/
+notebooks/1.0-matbench-genmetrics-basic.ipynb) [![ReadTheDocs](https://
+readthedocs.org/projects/matbench-genmetrics/badge/?version=latest)](https://
+matbench-genmetrics.readthedocs.io/en/stable/) [![PyPI-Server](https://
+img.shields.io/pypi/v/matbench-genmetrics.svg)](https://pypi.org/project/
+matbench-genmetrics/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/
+matbench-genmetrics)  Many generative models for crystal structure have been
+developed; however, few standardized benchmarks exist, and none exist in a
+format as easy-to-use as Matbench. Here, we introduce matbench-genmetrics, an
+open-source Python library for benchmarking generative models for crystal
+structures. We incorporate benchmark datasets, splits, and metrics inspired by
+[Crystal Diffusion Variational AutoEncoder (CDVAE)](https://github.com/txie-93/
+cdvae), which has been demonstrated as state-of-the-art in generative crystal
+structure tasks. We provide our own benchmarks using time-series style cross-
+validation splits from Materials Project via our [mp-time-split package](https:
+//mp-time-split.readthedocs.io/en/latest/) and focus on four metrics: validity,
+coverage, novelty, and uniqueness. Star Follow_@sgbaird Issue Discuss
 
-Many generative models for crystal structure have been developed; however, few
-standardized benchmarks exist, and none exist in a format as easy-to-use as
-Matbench. Here, we introduce matbench-genmetrics, an open-source Python library
-for benchmarking generative models for crystal structures. We incorporate
-benchmark datasets, splits, and metrics inspired by [Crystal Diffusion
-Variational AutoEncoder (CDVAE)](https://github.com/txie-93/cdvae), which has
-been demonstrated as state-of-the-art in generative crystal structure tasks. We
-provide our own benchmarks using time-series style cross-validation splits from
-Materials Project via our [mp-time-split package](https://mp-time-
-split.readthedocs.io/en/latest/) and focus on four metrics: validity, coverage,
-novelty, and uniqueness. Finally, we provide a simple example of preparation
-and submission to the matbench-genmetrics leaderboard using [pyxtal](https://
-pyxtal.readthedocs.io/en/latest/) for generation. ## Contents ```{toctree} :
-maxdepth: 2 Overview  Contributions & Help  License  Authors  Changelog  Module
-Reference
+ ## Contents ```{toctree} :maxdepth: 2 Overview  Metrics  Contributions & Help
+License  Authors  Changelog  Module Reference
 odules> GitHub Source
 github.com/sparks-baird/matbench-genmetrics> ``` ## Indices and tables *
 {ref}`genindex` * {ref}`modindex` * {ref}`search` [Sphinx]: http://www.sphinx-
 doc.org/ [Markdown]: https://daringfireball.net/projects/markdown/
 [reStructuredText]: http://www.sphinx-doc.org/en/master/usage/restructuredtext/
 basics.html [MyST]: https://myst-parser.readthedocs.io/en/latest/
```

### Comparing `matbench-genmetrics-0.6.0/docs/logo.png` & `matbench-genmetrics-0.6.1/reports/figures/metrics.png`

 * *Files identical despite different names*

### Comparing `matbench-genmetrics-0.6.0/environment.yml` & `matbench-genmetrics-0.6.1/environment.yml`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,29 @@
   - conda-forge
   - pytorch
   # - fastai
 dependencies:
   - python>=3.6
   - pip
   # BASICS
-  - numpy
-  - scipy
-  - pandas
-  - tqdm
-  - click
+  # - numpy
+  # - scipy
+  # - pandas
+  # - tqdm
+  # - click
+  # - scikit-learn
+  # - pymatgen
+  # - matminer
   - ipython
   # VISUALIZATION
   - matplotlib
-  - ipympl  # interactive matplotlib plots
-  - seaborn
+  - plotly
+  - python-kaleido
+  # - ipympl  # interactive matplotlib plots
+  # - seaborn
   # - altair
   # - yellowbrick
   # ML, STATS & DEEP LEARNING
   # - statsmodels
   # - scikit-learn
   # - sktime
   # - tslearn
@@ -35,14 +40,15 @@
   # - spacy
   # OTHER TOOLS
   # - optuna
   # - dask
   # - snakeviz
   - pip:
      - -e .  # install git checkout of matbench-genmetrics in editable mode
+     #  - element-coder
      # add here only pip-packages that are not available in conda/conda-forge! E.g.:
      # - icecream
      # - jax
      # - numpyro
      # - funsor
      # - neptune-client
      # - neptune-contrib
```

### Comparing `matbench-genmetrics-0.6.0/notebooks/template.ipynb` & `matbench-genmetrics-0.6.1/notebooks/core/template.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996875%*

 * *Differences: {"'cells'": "{1: {'source': ['from core import *']}}"}*

```diff
@@ -40,15 +40,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from matbench_genmetrics import *"
+                "from core import *"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**PLEASE** save this file right now using the following naming convention: `NUMBER_FOR_SORTING-YOUR_INITIALS-SHORT_DESCRIPTION`, e.g. `1.0-fw-initial-data-exploration`. Use the number to order the file within the directory according to its usage."
```

### Comparing `matbench-genmetrics-0.6.0/scripts/fingerprint_snapshot.py` & `matbench-genmetrics-0.6.1/scripts/core/fingerprint_snapshot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from os import path
 from pathlib import Path
 from typing import List
 
-from mp_time_split.core import MPTimeSplit
-
-from matbench_genmetrics.utils.featurize import featurize_comp_struct
+from matbench_genmetrics.core.utils.featurize import featurize_comp_struct
+from matbench_genmetrics.mp_time_split.splitter import MPTimeSplit
 
 mpt = MPTimeSplit(target="energy_above_hull")
 
 dummy = False
 mpt.load(dummy=dummy)
 material_ids: List[str] = mpt.data.material_id.tolist()
 structures = mpt.data.structure
```

### Comparing `matbench-genmetrics-0.6.0/scripts/run_grayskull.py` & `matbench-genmetrics-0.6.1/scripts/core/run_grayskull.py`

 * *Files identical despite different names*

### Comparing `matbench-genmetrics-0.6.0/scripts/train_model.py` & `matbench-genmetrics-0.6.1/scripts/core/train_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import sys
 from pathlib import Path
 
 import click
 from IPython.core import ultratb
 
-import matbench_genmetrics
+import matbench_genmetrics.core
 
 # fallback to debugger on error
 sys.excepthook = ultratb.FormattedTB(mode="Verbose", color_scheme="Linux", call_pdb=1)
 # turn UserWarning messages to errors to find the actual cause
 # import warnings
 # warnings.simplefilter("error")
 
@@ -25,21 +25,21 @@
     required=True,
     type=click.Path(exists=True),
     help="path to config file",
 )
 @click.option("--quiet", "log_level", flag_value=logging.WARNING, default=True)
 @click.option("-v", "--verbose", "log_level", flag_value=logging.INFO)
 @click.option("-vv", "--very-verbose", "log_level", flag_value=logging.DEBUG)
-@click.version_option(matbench_genmetrics.__version__)
+@click.version_option(matbench_genmetrics.core.__version__)
 def main(cfg_path: Path, log_level: int):
     logging.basicConfig(
         stream=sys.stdout,
         level=log_level,
         datefmt="%Y-%m-%d %H:%M",
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
     )
-    # YOUR CODE GOES HERE! Keep the main functionality in src/matbench_genmetrics
-    # est = matbench_genmetrics.models.Estimator()
+    # YOUR CODE GOES HERE! Keep the main functionality in src/core
+    # est = matbench_genmetrics.core.models.Estimator()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `matbench-genmetrics-0.6.0/scripts/validity_snapshot.py` & `matbench-genmetrics-0.6.1/scripts/core/validity_snapshot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import path
 from pathlib import Path
 from typing import List
 
 import pandas as pd
-from mp_time_split.core import MPTimeSplit
 
-from matbench_genmetrics.utils.featurize import mod_petti_contributions
+from matbench_genmetrics.core.utils.featurize import mod_petti_contributions
+from matbench_genmetrics.mp_time_split.splitter import MPTimeSplit
 
 mpt = MPTimeSplit(target="energy_above_hull")
 
 dummy = True
 mpt.load(dummy=dummy)
 material_ids: List[str] = mpt.data.material_id.tolist()
 structures = mpt.data.structure
```

### Comparing `matbench-genmetrics-0.6.0/setup.cfg` & `matbench-genmetrics-0.6.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -25,47 +25,61 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.6
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	pymatgen
+	numpy
+	pandas
 	scipy
-	mp-time-split[pyxtal]
+	scikit-learn
+	pymatgen
+	pyxtal
 	pystow
 	element-coder
+	pymatviz
+	matminer
+	pybtex
+	typing-extensions
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
+api = 
+	mp-api; python_version>="3.8"
 dev = 
 	conda-souschef
 	grayskull
 	pydocstyle
 	mypy
 	flake8
 	black
 	ipykernel
+	pre-commit
 testing = 
 	setuptools
 	pytest
 	pytest-cov
+	mp-api
 
 [options.entry_points]
 console_scripts = 
-	matbench-genmetrics = matbench_genmetrics.core:run
-	matbench_genmetrics = matbench_genmetrics.core:run
+	matbench-genmetrics = matbench_genmetrics.core.core:run
+	matbench_genmetrics = matbench_genmetrics.core.core:run
+	mp-time-split = matbench_genmetrics.mp_time_split.core:run
+	mp_time_split = matbench_genmetrics.mp_time_split.core:run
 
 [tool:pytest]
 addopts = 
-	--cov matbench_genmetrics --cov-report term-missing
+	--cov
+	--cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 
@@ -80,20 +94,22 @@
 	.tox
 	build
 	dist
 	.eggs
 	docs/conf.py
 
 [pyscaffold]
-version = 4.2.2.post1.dev2+ge50b5e1
-package = matbench_genmetrics
+version = 4.4.1
+package = core
 extensions = 
 	dsproject
 	github_actions
 	markdown
+	namespace
 	no_skeleton
 	pre_commit
+namespace = matbench_genmetrics
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `matbench-genmetrics-0.6.0/setup.py` & `matbench-genmetrics-0.6.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
     Setup file for matbench-genmetrics.
     Use setup.cfg to configure your project.
 
-    This file was generated with PyScaffold 4.2.2.post1.dev2+ge50b5e1.
+    This file was generated with PyScaffold 4.4.1.
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
```

### Comparing `matbench-genmetrics-0.6.0/src/matbench_genmetrics/__init__.py` & `matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Model benchmarking using validity, coverage, novelty, and uniqueness metrics"""
 import sys
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
```

### Comparing `matbench-genmetrics-0.6.0/src/matbench_genmetrics/core.py` & `matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Core functionality for matbench-genmetrics (generative materials benchmarking)"""
 import argparse
+import json
 import logging
+import pickle
 import sys
 from pathlib import Path
 from typing import List, Optional
 
 import numpy as np
-from mp_time_split.core import MPTimeSplit
 from pymatgen.core.structure import Structure
 from pystow import ensure_csv
 from scipy.stats import wasserstein_distance
 
-from matbench_genmetrics import __version__
-from matbench_genmetrics.utils.featurize import (
+from matbench_genmetrics.core import __version__
+from matbench_genmetrics.core.utils.featurize import (
     featurize_comp_struct,
     mod_petti_contributions,
 )
-from matbench_genmetrics.utils.match import (
+from matbench_genmetrics.core.utils.match import (
     ALLOWED_MATCH_TYPES,
     cdvae_cov_compstruct_match_matrix,
     get_structure_match_matrix,
 )
+from matbench_genmetrics.mp_time_split.splitter import MPTimeSplit
 
 # causes pytest to fail (tests not found, DLL load error)
 # from matbench_genmetrics.cdvae.metrics import RecEval, GenEval, OptEval
 
 
 __author__ = "sgbaird"
 __copyright__ = "sgbaird"
@@ -63,34 +65,47 @@
 FULL_STRUCT_NAME = "struct_fingerprints.csv"
 DUMMY_STRUCT_NAME = "dummy_struct_fingerprints.csv"
 FULL_SPG_NAME = "space_group_number.csv"
 DUMMY_SPG_NAME = "dummy_space_group_number.csv"
 FULL_MODPETTI_NAME = "mod_petti_contributions.csv"
 DUMMY_MODPETTI_NAME = "dummy_mod_petti_contributions.csv"
 
-# FULL_COMP_CHECKSUM_FROZEN = ""
-# DUMMY_COMP_CHECKSUM_FROZEN = ""
-# FULL_STRUCT_CHECKSUM_FROZEN = ""
-# DUMMY_STRUCT_CHECKSUM_FROZEN = ""
-# FULL_SPG_CHECKSUM_FROZEN = ""
-# DUMMY_SPG_CHECKSUM_FROZEN = ""
-
 FULL_COMP_URL = "https://figshare.com/ndownloader/files/36581838"
 DUMMY_COMP_URL = "https://figshare.com/ndownloader/files/36582174"
 FULL_STRUCT_URL = "https://figshare.com/ndownloader/files/36581841"
 DUMMY_STRUCT_URL = "https://figshare.com/ndownloader/files/36582177"
 FULL_SPG_URL = "https://figshare.com/ndownloader/files/36620538"
 DUMMY_SPG_URL = "https://figshare.com/ndownloader/files/36620544"
 FULL_MODPETTI_URL = "https://figshare.com/ndownloader/files/36620535"
 DUMMY_MODPETTI_URL = "https://figshare.com/ndownloader/files/36620541"
 
 DATA_HOME = "matbench-genmetrics"
 
 
 class GenMatcher(object):
+    """
+    A class for matching generated structures to test structures.
+
+    Parameters
+    ----------
+    test_structures : List[pymatgen.Structure]
+        A list of test structures.
+    gen_structures : List[pymatgen.Structure]
+        A list of generated structures.
+    match_type : str, optional
+        The type of matching algorithm to use. Default is "StructureMatcher".
+    match_kwargs : dict, optional
+        Additional keyword arguments to pass to the matching algorithm.
+
+    Attributes
+    ----------
+    match_matrix : numpy.ndarray
+        A matrix of match scores between test and generated structures.
+    """
+
     def __init__(
         self,
         test_structures,
         gen_structures: Optional[List[Structure]] = None,
         test_comp_fingerprints: Optional[np.ndarray] = None,
         gen_comp_fingerprints: Optional[np.ndarray] = None,
         test_struct_fingerprints: Optional[np.ndarray] = None,
@@ -141,14 +156,47 @@
         self.num_test = len(self.test_structures)
         self.num_gen = len(self.gen_structures)
 
         self._match_matrix = None
 
     @property
     def match_matrix(self):
+        """A matrix of match scores between test and generated structures.
+
+        match_matrix : numpy.ndarray
+            The element at position (i, j) represents the match score between the ith
+            test structure and the jth generated structure. The match score is
+            calculated using the specified matching algorithm and any additional keyword
+            arguments passed to the `GenMatcher` class.
+
+            Examples
+            --------
+            >>> from pymatgen.core.structure import Structure
+            >>> from pymatgen.core.lattice import Lattice
+            >>> test_structures = [
+            ...     Structure(
+            ...         Lattice.cubic(3.0), ["Si", "Si"], [[0, 0, 0], [0.5, 0.5, 0.5]]
+            ...     ),
+            ...     Structure(
+            ...         Lattice.cubic(3.0), ["Si", "Si"], [[0, 0, 0], [0.5, 0.5, 0.5]]
+            ...     ),
+            ... ]
+            >>> gen_structures = [
+            ...     Structure(
+            ...         Lattice.cubic(3.0), ["Si", "Si"], [[0, 0, 0], [0.5, 0.5, 0.5]]
+            ...     ),
+            ...     Structure(
+            ...         Lattice.cubic(3.0), ["Si", "Si"], [[0, 0, 0], [0.5, 0.5, 0.5]]
+            ...     ),
+            ... ]
+            >>> matcher = GenMatcher(test_structures, gen_structures)
+            >>> matcher.match_matrix
+            array([[1., 1.],
+                [1., 1.]])
+        """
         if self._match_matrix is not None:
             return self._match_matrix
 
         if self.match_type == "StructureMatcher":
             match_matrix = get_structure_match_matrix(
                 self.test_structures,
                 self.gen_structures,
@@ -207,19 +255,65 @@
         of unique structures, even if repeat structures exist.
         """
         num_possible = self.num_test**2 - self.num_test
         return self.duplicity_count / num_possible
 
 
 class GenMetrics(object):
+    """
+    Evaluate the performance of a generative model on a set of training and test data.
+
+    Parameters
+    ----------
+    train_structures : List[pymatgen.Structure]
+        A list of training structures.
+    test_structures : List[pymatgen.Structure]
+        A list of test structures.
+    gen_structures : List[pymatgen.Structure]
+        A list of generated structures.
+    test_pred_structures : List[pymatgen.Structure]
+        A list of test structures predicted by the machine learning model.
+    match_type : str, optional
+        The type of matching algorithm to use. Default is "StructureMatcher".
+    match_kwargs : dict, optional
+        Additional keyword arguments to pass to the matching algorithm.
+
+    Attributes
+    ----------
+    train_test_match_matrix : numpy.ndarray
+        A matrix of match scores between training and test structures. The element at
+        position (i, j) represents the match score between the ith training structure
+        and the jth test structure. The match score is calculated using the specified
+        matching algorithm and any additional keyword arguments passed to the
+        `GenMetrics` class.
+    test_pred_match_matrix : numpy.ndarray
+        A matrix of match scores between test structures and predicted test structures.
+        The element at position (i, j) represents the match score between the ith test
+        structure and the jth predicted test structure. The match score is calculated
+        using the specified matching algorithm and any additional keyword arguments
+        passed to the `GenMetrics` class.
+    train_gen_match_matrix : numpy.ndarray
+        A matrix of match scores between training structures and generated structures.
+        The element at position (i, j) represents the match score between the ith
+        training structure and the jth generated structure. The match score is
+        calculated using the specified matching algorithm and any additional keyword
+        arguments passed to the `GenMetrics` class.
+    test_gen_match_matrix : numpy.ndarray
+        A matrix of match scores between test structures and generated structures. The
+        element at position (i, j) represents the match score between the ith test
+        structure and the jth generated structure. The match score is calculated using
+        the specified matching algorithm and any additional keyword arguments passed to
+        the `GenMetrics` class.
+    """
+
     def __init__(
         self,
-        train_structures,
-        test_structures,
-        gen_structures,
+        train_structures: List[Structure],
+        test_structures: List[Structure],
+        gen_structures: List[Structure],
         train_comp_fingerprints=None,
         test_comp_fingerprints=None,
         train_struct_fingerprints=None,
         test_struct_fingerprints=None,
         train_test_spg=None,
         train_test_modpetti_df=None,
         test_pred_structures=None,
@@ -245,47 +339,34 @@
             self.gen_comp_fingerprints,
             self.gen_struct_fingerprints,
         ) = featurize_comp_struct(self.gen_structures)
 
         self._cdvae_metrics = None
         self._mpts_metrics = None
 
-    # @property
-    # def cdvae_metrics(self):
-    #     # FIXME: update with CDVAE structures and handle 3 dataset types
-    #     if self._cdvae_metrics is not None:
-    #         return self._cdvae_metrics
-
-    #     rec_eval = RecEval(self.test_pred_structures, self.test_structures)
-    #     reconstruction_metrics = rec_eval.get_metrics()
-
-    #     gen_eval = GenEval(self.gen_structures, self.test_structures)
-    #     generation_metrics = gen_eval.get_metrics()
-
-    #     opt_eval = OptEval(self.gen_structures, self.test_structures)
-    #     optimization_metrics = opt_eval.get_metrics()
-
-    #     self._cdvae_metrics = (
-    #         reconstruction_metrics,
-    #         generation_metrics,
-    #         optimization_metrics,
-    #     )
-
-    #     return self._cdvae_metrics
-
     @property
     def validity(self):
         """Scaled Wasserstein distance between real (train/test) and gen structures."""
         # TODO: implement notion of compositional validity, since this is only structure
         train_test_structures = self.train_structures + self.test_structures
+
+        def try_get_space_group_info(structure):
+            try:
+                spg_tmp = structure.get_space_group_info()
+            except TypeError as e:
+                _logger.debug(e)
+                spg_tmp = ("P", 1)
+            return spg_tmp
+
         if self.train_test_spg is None:
             self.train_test_spg = [
-                ts.get_space_group_info()[1] for ts in train_test_structures
+                try_get_space_group_info(ts)[1] for ts in train_test_structures
             ]
-        gen_spg = [ts.get_space_group_info()[1] for ts in self.gen_structures]
+
+        gen_spg = [try_get_space_group_info(ts)[1] for ts in self.gen_structures]
 
         if self.train_test_modpetti_df is None:
             self.train_test_modpetti_df = mod_petti_contributions(train_test_structures)
         gen_modpetti_df = mod_petti_contributions(self.gen_structures)
 
         dummy_spg_case = wasserstein_distance(self.train_test_spg, [1])
         spg_distance = wasserstein_distance(self.train_test_spg, gen_spg)
@@ -371,14 +452,69 @@
             "coverage": self.coverage,
             "novelty": self.novelty,
             "uniqueness": self.uniqueness,
         }
 
 
 class MPTSMetrics(object):
+    """
+    Evaluate the performance of a crystal generative model using MP Time Split (MPTS).
+
+    Parameters
+    ----------
+    dummy : bool, optional
+        Whether to use dummy data for testing purposes. Default is False.
+    verbose : bool, optional
+        Whether to print out the results of the evaluation. Default is True.
+    num_gen : int, optional
+        The number of generated structures to use for the evaluation. Default is None.
+    save_dir : str, optional
+        The directory to save the generated structures to. Default is "results".
+    match_type : str, optional
+        The type of matching algorithm to use. Default is "StructureMatcher".
+
+    Attributes
+    ----------
+    train_scores : List[Dict[str, float]]
+        A list of dictionaries containing the evaluation results for each fold of the
+        training data.
+    val_scores : List[Dict[str, float]]
+        A list of dictionaries containing the evaluation results for each fold of the
+        validation data.
+    test_scores : List[Dict[str, float]]
+        A list of dictionaries containing the evaluation results for each fold of the
+        test data.
+    gen_scores : List[Dict[str, float]]
+        A list of dictionaries containing the evaluation results for each fold of the
+        generated data.
+    test_pred_scores : List[Dict[str, float]]
+        A list of dictionaries containing the evaluation results for each fold of the
+        predicted test data.
+    **match_kwargs : Dict[str, Any]
+        Keyword arguments passed to GenMetrics.
+
+    Methods
+    -------
+    get_train_and_val_data(fold: int) -> Tuple[List[Structure], List[Structure]]:
+        Get the training and validation data for a given fold.
+    evaluate_and_record(fold: int, gen_structures: List[Structure]) -> None:
+        Evaluate the performance of the model on the generated structures and record the
+        results.
+
+    Notes
+    -----
+    This class assumes that the data is split into training, validation, and test sets
+    using the MP Time Split (MPTS) protocol. The `get_train_and_val_data` method is used
+    to retrieve the training and validation data for a given fold, and the
+    `evaluate_and_record` method is used to evaluate the performance of the model on the
+    generated structures and record the results. The evaluation results are stored in
+    the `train_scores`, `val_scores`, `test_scores`, `gen_scores`, and
+    `test_pred_scores` attributes.
+    """
+
     def __init__(
         self,
         dummy=False,
         verbose=True,
         num_gen=None,
         save_dir="results",
         match_type="cdvae_coverage",
@@ -395,15 +531,33 @@
 
         self.mpt = MPTimeSplit(target="energy_above_hull")
         self.folds = self.mpt.folds
         self.gms: List[Optional[GenMetrics]] = [None] * len(self.folds)
         self.recorded_metrics = {}
 
     def load_fingerprints(self, dummy=False):
+        """Load precalculated fingerprints from FigShare.
 
+        Parameters
+        ----------
+        dummy : bool, optional
+            Whether to load a small, dummy dataset, by default False
+
+        Returns
+        -------
+        DataFrame
+            Compositional fingerprints
+
+        Examples
+        --------
+        >>> mptm = MPTSMetrics()
+        >>> comp_fingerprints_df, struct_fingerprints_df = mptm.load_fingerprints(
+        ...     dummy=False
+        ... )
+        """
         comp_url = DUMMY_COMP_URL if dummy else FULL_COMP_URL
         struct_url = DUMMY_STRUCT_URL if dummy else FULL_STRUCT_URL
         comp_name = DUMMY_COMP_NAME if dummy else FULL_COMP_NAME
         struct_name = DUMMY_STRUCT_NAME if dummy else FULL_STRUCT_NAME
 
         read_csv_kwargs = dict(index_col="material_id", sep=",")
         self.comp_fingerprints_df = ensure_csv(
@@ -419,14 +573,33 @@
             read_csv_kwargs=read_csv_kwargs,
         )
         # REVIEW: consider doing checksum validation
 
         return self.comp_fingerprints_df, self.struct_fingerprints_df
 
     def load_space_group_and_mod_petti(self, dummy=False):
+        """Load space groups and modified pettifor encodings from FigShare.
+
+        Parameters
+        ----------
+        dummy : bool, optional
+            Whether to load a small, dummy dataset, by default False
+
+        Returns
+        -------
+        DataFrame
+            space group numbers
+        DataFrame
+            modified pettifor encodings
+
+        Examples
+        --------
+        >>> mptm = MPTSMetrics()
+        >>> spg_df, modpetti_df = mptm.load_space_group_and_mod_petti(dummy=False)
+        """
         spg_name = DUMMY_SPG_NAME if dummy else FULL_SPG_NAME
         spg_url = DUMMY_SPG_URL if dummy else FULL_SPG_URL
         modpetti_name = DUMMY_MODPETTI_NAME if dummy else FULL_MODPETTI_NAME
         modpetti_url = DUMMY_MODPETTI_URL if dummy else FULL_MODPETTI_URL
 
         self.spg_df = ensure_csv(
             DATA_HOME,
@@ -438,31 +611,52 @@
             DATA_HOME,
             name=modpetti_name,
             url=modpetti_url,
             read_csv_kwargs=dict(index_col="symbol", sep=","),
         )
         return self.spg_df, self.modpetti_df
 
-    def get_train_and_val_data(self, fold, include_val=False):
+    def get_train_and_val_data(self, fold: int, include_val=False):
+        """Get the MPTimeSplit fingerprints, sp.grp numbers, and modPetti info.
+
+
 
+        Parameters
+        ----------
+        fold : int
+            Which of the 5 folds to use for training and validation (0-4)
+        include_val : bool, optional
+            Whether to return the validation data in addition to the training data, by
+            default False
+
+        Returns
+        -------
+        DataFrame
+            Training inputs
+        DataFrame
+            Validation inputs. Only returned if `include_val` is True.
+
+
+        Examples
+        --------
+        >>> mptm = MPTSMetrics()
+        >>> train_inputs = mptm.get_train_and_val_data(fold, include_val=False)
+        """
         if self.recorded_metrics == {}:
             self.mpt.load(dummy=self.dummy)
         (
             self.train_inputs,
             self.val_inputs,
             self.train_outputs,
             self.val_outputs,
         ) = self.mpt.get_train_and_val_data(fold)
 
         spg_df, modpetti_df = self.load_space_group_and_mod_petti(dummy=self.dummy)
         self.spg = spg_df.space_group_number.values
         self.modpetti_df = modpetti_df
-        # self.train_spg, self.val_spg = [
-        #     spg.iloc[tvs].values for tvs in self.mpt.trainval_splits[fold]
-        # ]
 
         if self.match_type == "cdvae_coverage":
             comp_fps, struct_fps = self.load_fingerprints(dummy=self.dummy)
 
             self.train_comp_fingerprints, self.val_comp_fingerprints = [
                 comp_fps.iloc[tvs].values for tvs in self.mpt.trainval_splits[fold]
             ]
@@ -477,15 +671,27 @@
             self.val_struct_fingerprints = None
 
         if include_val:
             return self.train_inputs, self.val_inputs
 
         return self.train_inputs
 
-    def evaluate_and_record(self, fold, gen_structures, test_pred_structures=None):
+    def evaluate_and_record(self, fold: int, gen_structures, test_pred_structures=None):
+        """Evaluate generated structures and record metrics.
+
+        Parameters
+        ----------
+        fold : int
+            Fold number.
+        gen_structures : list of pymatgen Structure
+        List of generated structures.
+        test_pred_structures : list of pymatgen Structure, optional
+            List of predicted structures for the test set. If not provided, the
+            test set is assumed to be the same as the validation set.
+        """
         if self.num_gen is not None and self.num_gen != len(gen_structures):
             raise ValueError(
                 f"Number of generated structures ({len(gen_structures)}) does not match expected number ({self.num_gen})."  # noqa: E501
             )
         self.gms[fold] = GenMetrics(
             self.train_inputs.tolist(),
             self.val_inputs.tolist(),
@@ -504,59 +710,70 @@
 
         self.recorded_metrics[fold] = self.gms[fold].metrics
 
         # i.e. store the values for the current fold for testing purposes
         for metric, value in self.recorded_metrics[fold].items():
             setattr(self, metric, value)
 
+    def save(self, fpath_stem):
+        with open(fpath_stem + ".pkl", "wb") as f:
+            pickle.dump(self, f)
+
+        with open(fpath_stem + ".json", "w") as fp:
+            json.dump(self.recorded_metrics, fp)
+
+    def load(self, fpath):
+        with open(fpath, "rb") as f:
+            return pickle.load(f)
+
 
 class MPTSMetrics10(MPTSMetrics):
+    """Benchmark class for MPTSMetrics with 10 generated structures."""
+
     def __init__(self, dummy=False, verbose=True):
         MPTSMetrics.__init__(
             self, dummy=dummy, verbose=verbose, num_gen=10, match_type="cdvae_coverage"
         )
 
 
 class MPTSMetrics100(MPTSMetrics):
+    """Benchmark class for MPTSMetrics with 100 generated structures."""
+
     def __init__(self, dummy=False, verbose=True):
         MPTSMetrics.__init__(
             self, dummy=dummy, verbose=verbose, num_gen=100, match_type="cdvae_coverage"
         )
 
 
 class MPTSMetrics1000(MPTSMetrics):
+    """Benchmark class for MPTSMetrics with 1000 generated structures."""
+
     def __init__(self, dummy=False, verbose=True):
         MPTSMetrics.__init__(
             self,
             dummy=dummy,
             verbose=verbose,
             num_gen=1000,
             match_type="cdvae_coverage",
         )
 
 
 class MPTSMetrics10000(MPTSMetrics):
+    """Benchmark class for MPTSMetrics with 10000 generated structures."""
+
     def __init__(self, dummy=False, verbose=True):
         MPTSMetrics.__init__(
             self,
             dummy=dummy,
             verbose=verbose,
             num_gen=10000,
             match_type="cdvae_coverage",
         )
 
 
-# def get_rms_dist(gen_structures, test_structures):
-#     rms_dist = np.zeros((len(gen_structures), len(test_structures)))
-#     for i, gs in enumerate(tqdm(gen_structures)):
-#         for j, ts in enumerate(tqdm(test_structures)):
-#             rms_dist[i, j] = sm.get_rms_dist(gs, ts)[0]
-
-#     return rms_dist
-
 # ---- CLI ----
 # The functions defined in this section are wrappers around the main Python
 # API allowing them to be called directly from the terminal as a CLI
 # executable/script.
 
 
 def parse_args(args):
@@ -705,7 +922,67 @@
 #     self.symmetric = False
 
 # if dummy:
 #     self.train_test_spg = ensure_csv(DUMMY_SPG_URL, name=DUMMY_SPG_NAME).values
 # else:
 #     self.train_test_spg = ensure_csv(FULL_SPG_URL, name=FULL_SPG_NAME).values
 # return self.train_test_spg
+
+# self.train_test_spg = [
+#     ts.get_space_group_info()[1] for ts in train_test_structures
+# ]
+
+# gen_spg = [ts.get_space_group_info()[1] for ts in self.gen_structures]
+
+# self.train_test_spg = []
+# for ts in train_test_structures:
+
+# self.train_test_spg.append(spg_tmp[1] if spg_tmp is not None else 1)
+# gen_spg = []
+# for i, gs in enumerate(self.gen_structures):
+#     print(i)
+#     spg_tmp = gs.get_space_group_info()
+#     gen_spg.append(spg_tmp[1] if spg_tmp is not None else 1)
+
+
+# @property
+# def cdvae_metrics(self):
+#     # FIXME: update with CDVAE structures and handle 3 dataset types
+#     if self._cdvae_metrics is not None:
+#         return self._cdvae_metrics
+
+#     rec_eval = RecEval(self.test_pred_structures, self.test_structures)
+#     reconstruction_metrics = rec_eval.get_metrics()
+
+#     gen_eval = GenEval(self.gen_structures, self.test_structures)
+#     generation_metrics = gen_eval.get_metrics()
+
+#     opt_eval = OptEval(self.gen_structures, self.test_structures)
+#     optimization_metrics = opt_eval.get_metrics()
+
+#     self._cdvae_metrics = (
+#         reconstruction_metrics,
+#         generation_metrics,
+#         optimization_metrics,
+#     )
+
+#     return self._cdvae_metrics
+
+# def get_rms_dist(gen_structures, test_structures):
+#     rms_dist = np.zeros((len(gen_structures), len(test_structures)))
+#     for i, gs in enumerate(tqdm(gen_structures)):
+#         for j, ts in enumerate(tqdm(test_structures)):
+#             rms_dist[i, j] = sm.get_rms_dist(gs, ts)[0]
+
+#     return rms_dist
+
+# self.train_spg, self.val_spg = [
+#     spg.iloc[tvs].values for tvs in self.mpt.trainval_splits[fold]
+# ]
+
+
+# FULL_COMP_CHECKSUM_FROZEN = ""
+# DUMMY_COMP_CHECKSUM_FROZEN = ""
+# FULL_STRUCT_CHECKSUM_FROZEN = ""
+# DUMMY_STRUCT_CHECKSUM_FROZEN = ""
+# FULL_SPG_CHECKSUM_FROZEN = ""
+# DUMMY_SPG_CHECKSUM_FROZEN = ""
```

### Comparing `matbench-genmetrics-0.6.0/src/matbench_genmetrics/utils/featurize.py` & `matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/utils/featurize.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 from element_coder import encode
 from matminer.featurizers.composition.composite import ElementProperty
 from matminer.featurizers.site.fingerprint import CrystalNNFingerprint
 from matminer.featurizers.structure.sites import SiteStatsFingerprint
 from pymatgen.core.structure import Structure
 
-from matbench_genmetrics.utils.match import get_tqdm
+from matbench_genmetrics.core.utils.match import get_tqdm
 
 cnnf = CrystalNNFingerprint.from_preset("ops")
 ep = ElementProperty.from_preset("magpie")
 ssf = SiteStatsFingerprint(cnnf, stats=("mean"))
 
 
 def featurize_comp_struct(
@@ -58,21 +58,16 @@
         lambda s: s.composition.fractional_composition
     )
     # NOTE: be aware of amount_tolerance=1e-8
     summed_comp = np.sum(compositions).fractional_composition
     _data = summed_comp._data
     mod_petti = [encode(k, "mod_pettifor") for k in _data.keys()]
     mod_petti_comp = dict(zip(mod_petti, _data.values()))
-
     mod_petti_df = pd.DataFrame(
-        dict(
-            symbol=list(_data.keys()),
-            mod_petti=mod_petti_comp.keys(),
-            contribution=mod_petti_comp.values(),
-        )
+        dict(mod_petti=mod_petti_comp.keys(), contribution=mod_petti_comp.values()),
     ).sort_values("mod_petti")
     return mod_petti_df
 
 
 def cdvae_cov_comp_fingerprints(structures, verbose=False):
     my_tqdm = get_tqdm(verbose)
     CompFP = ElementProperty.from_preset("magpie")
@@ -145,7 +140,17 @@
 
     return struct_fps
 
 
 # %% Code Graveyard
 # structures = pd.DataFrame({struct_name: structures})
 # compositions = pd.DataFrame({comp_name: compositions})
+
+# pd.DataFrame(
+# dict(
+#     # symbol=list(_data.keys()), # mod_petti lacking 118 unique mappings
+#     mod_petti=mod_petti_comp.keys(),
+#     contribution=mod_petti_comp.values(),
+# )
+# )
+
+# mod_petti_df = pd.DataFrame(mod_petti_comp, index=[0]).sort_values("mod_petti")
```

### Comparing `matbench-genmetrics-0.6.0/src/matbench_genmetrics/utils/match.py` & `matbench-genmetrics-0.6.1/src/matbench_genmetrics/core/utils/match.py`

 * *Files identical despite different names*

### Comparing `matbench-genmetrics-0.6.0/src/matbench_genmetrics.egg-info/PKG-INFO` & `matbench-genmetrics-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,35 @@
-Metadata-Version: 2.1
-Name: matbench-genmetrics
-Version: 0.6.0
-Summary: Generative materials benchmarking metrics, inspired by CDVAE.
-Home-page: https://github.com/sparks-baird/matbench-genmetrics/
-Author: sgbaird
-Author-email: sterling.baird@utah.edu
-License: MIT
-Project-URL: Documentation, https://matbench-genmetrics.readthedocs.io
-Project-URL: Source, https://github.com/sparks-baird/matbench-genmetrics
-Project-URL: Changelog, https://matbench-genmetrics.readthedocs.io/latest/changelog.html
-Project-URL: Tracker, https://github.com/sparks-baird/matbench-genmetrics/issues
-Project-URL: Conda-Forge, https://anaconda.org/conda-forge/matbench-genmetrics
-Project-URL: Download, https://pypi.org/project/matbench-genmetrics/#files
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: dev
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 [![ReadTheDocs](https://readthedocs.org/projects/matbench-genmetrics/badge/?version=latest)](https://matbench-genmetrics.readthedocs.io/en/stable/)
 [![Coveralls](https://img.shields.io/coveralls/github/sparks-baird/matbench-genmetrics/main.svg)](https://coveralls.io/r/sparks-baird/matbench-genmetrics)
 [![PyPI-Server](https://img.shields.io/pypi/v/matbench-genmetrics.svg)](https://pypi.org/project/matbench-genmetrics/)
 [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/matbench-genmetrics.svg)](https://anaconda.org/conda-forge/matbench-genmetrics)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/matbench-genmetrics)
 ![Lines of code](https://img.shields.io/tokei/lines/github/sparks-baird/matbench-genmetrics)
 <!-- These are examples of badges you might also want to add to your README. Update the URLs accordingly.
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/matbench-genmetrics.svg?branch=main)](https://cirrus-ci.com/github/<USER>/matbench-genmetrics)
 [![Monthly Downloads](https://pepy.tech/badge/matbench-genmetrics/month)](https://pepy.tech/project/matbench-genmetrics)
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/matbench-genmetrics)
 -->
-> **NOTE: This is a WIP repository (as of 2022-08-06) being developed in parallel with [`xtal2png`](https://github.com/sparks-baird/xtal2png) and [`mp-time-split`](https://github.com/sparks-baird/mp-time-split). Feedback and contributions welcome!**
-# matbench-genmetrics
+<!--- > **NOTE: This is a WIP repository (as of 2022-08-06) being developed in parallel with [`xtal2png`](https://github.com/sparks-baird/xtal2png) and [`mp-time-split`](https://github.com/sparks-baird/mp-time-split). Feedback and contributions welcome!** --->
+> **This is not an official repository of Matbench, but eventually, it may be [incorporated into Matbench](https://github.com/materialsproject/matbench/issues/150)**
 
+# matbench-genmetrics [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sparks-baird/matbench-genmetrics/blob/main/notebooks/1.0-matbench-genmetrics-basic.ipynb)
 > Generative materials benchmarking metrics, inspired by [guacamol](https://www.benevolent.com/guacamol) and [CDVAE](https://github.com/txie-93/cdvae).
 
 This repository provides standardized benchmarks for benchmarking generative models for
 crystal structure. Each benchmark has a fixed dataset, a predefined split, and a notion
 of best (i.e. metric) associated with it.
 
-<p align="center"><img src="https://github.com/sparks-baird/matbench-genmetrics/raw/main/reports/figures/metrics.png" width=450></p>
+<p align="center"><img src="https://github.com/sparks-baird/matbench-genmetrics/raw/main/reports/figures/matbench-genmetrics.png" width=450></p>
 
 ## Getting Started
 
 Installation, a dummy example, output metrics for the example, and descriptions of the benchmark metrics.
+
 ### Installation
 
 Create a conda environment with the `matbench-genmetrics` package installed from the
 `conda-forge` channel. Then activate the environment.
 
 > **NOTE: not available on conda-forge as of 2022-07-30, recipe under review by
 > conda-forge team. So use `pip install matbench-genmetrics` for now
@@ -74,15 +53,15 @@
 >>> from matbench_genmetrics.core import MPTSMetrics10, MPTSMetrics100, MPTSMetrics1000, MPTSMetrics10000
 >>> mptm = MPTSMetrics10(dummy=True)
 >>> for fold in mptm.folds:
 >>>     train_val_inputs = mptm.get_train_and_val_data(fold)
 >>>     dg = DummyGenerator()
 >>>     dg.fit(train_val_inputs)
 >>>     gen_structures = dg.gen(n=mptm.num_gen)
->>>     mptm.record(fold, gen_structures)
+>>>     mptm.evaluate_and_record(fold, gen_structures)
 ```
 
 ### Output
 
 ```python
 print(mptm.recorded_metrics)
 ```
@@ -120,53 +99,56 @@
         "uniqueness": 0.9111111111111111,
     },
 }
 ```
 
 ### Metrics
 
-| Metric | Description |
-|---|---|
-| Validity | One minus (Wasserstein distance between distribution of space group numbers for train and generated structures divided by distance of dummy case between train and `space_group_number == 1`). See also https://github.com/sparks-baird/matbench-genmetrics/issues/44 |
-| Coverage | Match counts between held-out test structures and generated structures divided by number of test structures ("predict the future"). |
-| Novelty | One minus (match counts between train structures and generated structures divided by number of generated structures). |
-| Uniqueness | One minus (non-self-comparing match counts within generated structures divided by total possible non-self-comparing matches). |
+| Metric     | Description                                                                                                                                                                                                                                                             |
+| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Validity   | One minus (Wasserstein distance between distribution of space group numbers for train and generated structures divided by distance of dummy case between train and `space_group_number == 1`). See also <https://github.com/sparks-baird/matbench-genmetrics/issues/44> |
+| Coverage   | Match counts between held-out test structures and generated structures divided by number of test structures ("predict the future").                                                                                                                                     |
+| Novelty    | One minus (match counts between train structures and generated structures divided by number of generated structures).                                                                                                                                                   |
+| Uniqueness | One minus (non-self-comparing match counts within generated structures divided by total possible non-self-comparing matches).                                                                                                                                           |
+
+A match is when <code><a href="https://pymatgen.org/pymatgen.analysis.structure_matcher.html#pymatgen.analysis.structure_matcher.StructureMatcher">StructureMatcher</a>(stol=0.5, ltol=0.3, angle_tol=10.0).fit(s1, s2)</code> evaluates to `True`.
+
+Detailed descriptions of the metrics are given in https://self-driving-lab-demo.readthedocs.io/en/latest/metrics.html.
+
 
-A match is when [`StructureMatcher`](https://pymatgen.org/pymatgen.analysis.structure_matcher.html#pymatgen.analysis.structure_matcher.StructureMatcher)`(stol=0.5, ltol=0.3, angle_tol=10.0).fit(s1, s2)`
-evaluates to `True`.
 
 ## Advanced Installation
 
 ### Anaconda (`conda`) installation (recommended)
 
-(2022-07-30, conda-forge installation pending, fallback to `pip install xtal2png` as separate command)
+(2022-07-30, conda-forge installation pending, fallback to `pip install matbench-genmetrics` as separate command)
 
-Create and activate a new `conda` environment named `xtal2png` (`-n`) that will search for and install the `xtal2png` package from the `conda-forge` Anaconda channel (`-c`).
+Create and activate a new `conda` environment named `matbench-genmetrics` (`-n`) that will search for and install the `matbench-genmetrics` package from the `conda-forge` Anaconda channel (`-c`).
 
 ```bash
-conda env create -n xtal2png -c conda-forge xtal2png
-conda activate xtal2png
+conda env create -n matbench-genmetrics -c conda-forge matbench-genmetrics
+conda activate matbench-genmetrics
 ```
 
 Alternatively, in an already activated environment:
 
 ```bash
-conda install -c conda-forge xtal2png
+conda install -c conda-forge matbench-genmetrics
 ```
 
-If you run into conflicts with packages you are integrating with `xtal2png`, please try installing all packages in a single line of code (or two if mixing `conda` and `pip` packages in the same environment) and installing with `mamba` ([source](https://stackoverflow.com/a/69137255/13697228)).
+If you run into conflicts with packages you are integrating with `matbench-genmetrics`, please try installing all packages in a single line of code (or two if mixing `conda` and `pip` packages in the same environment) and installing with `mamba` ([source](https://stackoverflow.com/a/69137255/13697228)).
 
 ### PyPI (`pip`) installation
 
 Create and activate a new `conda` environment named `matbench-genmetrics` (`-n`) with `python==3.9.*` or your preferred Python version, then install `matbench-genmetrics` via `pip`.
 
 ```bash
-conda create -n xtal2png python==3.9.*
-conda activate xtal2png
-pip install xtal2png
+conda create -n matbench-genmetrics python==3.9.*
+conda activate matbench-genmetrics
+pip install matbench-genmetrics
 ```
 
 ## Editable installation
 
 In order to set up the necessary environment:
 
 1. clone and enter the repository via:
@@ -216,25 +198,29 @@
 
 ## Dependency Management & Reproducibility
 
 1. Always keep your abstract (unpinned) dependencies updated in `environment.yml` and eventually
    in `setup.cfg` if you want to ship and install your package via `pip` later on.
 2. Create concrete dependencies as `environment.lock.yml` for the exact reproduction of your
    environment with:
+
    ```bash
    conda env export -n matbench-genmetrics -f environment.lock.yml
    ```
+
    For multi-OS development, consider using `--no-builds` during the export.
 3. Update your current environment with respect to a new `environment.lock.yml` using:
+
    ```bash
    conda env update -f environment.lock.yml --prune
    ```
+
 ## Project Organization
 
-```
+```txt
 ├── AUTHORS.md              <- List of developers and maintainers.
 ├── CHANGELOG.md            <- Changelog to keep track of new features and fixes.
 ├── CONTRIBUTING.md         <- Guidelines for contributing to this project.
 ├── Dockerfile              <- Build a docker container with `docker build .`.
 ├── LICENSE.txt             <- License as chosen on the command-line.
 ├── README.md               <- The top-level README for developers.
 ├── configs                 <- Directory for configurations of model & application.
```

### Comparing `matbench-genmetrics-0.6.0/tests/test_matbench_genmetrics.py` & `matbench-genmetrics-0.6.1/tests/test_matbench_genmetrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from itertools import product
 from typing import Callable, List, Tuple
 
 import numpy as np
 import numpy.typing as npt
 import pytest
-from mp_time_split.utils.gen import DummyGenerator
 from numpy.testing import assert_array_equal
 from pymatgen.core.lattice import Lattice
 from pymatgen.core.structure import Structure
 from pymatgen.transformations.standard_transformations import (
     PerturbStructureTransformation,
 )
 
-from matbench_genmetrics.core import GenMatcher, GenMetrics, MPTSMetrics
-from matbench_genmetrics.utils.featurize import cdvae_cov_struct_fingerprints
+from matbench_genmetrics.core.metrics import GenMatcher, GenMetrics, MPTSMetrics
+from matbench_genmetrics.core.utils.featurize import cdvae_cov_struct_fingerprints
+from matbench_genmetrics.mp_time_split.utils.gen import DummyGenerator
 
 # from pytest_cases import fixture, parametrize, parametrize_with_cases
 
 np.random.seed(10)
 
 coords = [[0, 0, 0], [0.75, 0.5, 0.75]]
 lattice = Lattice.from_parameters(a=3.84, b=3.84, c=3.84, alpha=120, beta=90, gamma=60)
```

### Comparing `matbench-genmetrics-0.6.0/tox.ini` & `matbench-genmetrics-0.6.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
 passenv =
     HOME
+    SETUPTOOLS_*
+    MP_API_KEY
 extras =
     testing
 commands =
     pytest {posargs}
 
 
 # # To run `tox -e lint` you need to make sure you have a
@@ -25,38 +27,45 @@
 # [testenv:lint]
 # description = Perform static analysis and style checks
 # skip_install = True
 # deps = pre-commit
 # passenv =
 #     HOMEPATH
 #     PROGRAMDATA
+#     SETUPTOOLS_*
 # commands =
 #     pre-commit run --all-files {posargs:--show-diff-on-failure}
 
 
 [testenv:{build,clean}]
 description =
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
     clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
 # https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
 skip_install = True
 changedir = {toxinidir}
 deps =
     build: build[virtualenv]
+passenv =
+    SETUPTOOLS_*
 commands =
     clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
     clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
+# By default, both `sdist` and `wheel` are built. If your sdist is too big or you don't want
+# to make it available, consider running: `tox -e build -- --wheel`
 
 
 [testenv:{docs,doctests,linkcheck}]
 description =
     docs: Invoke sphinx-build to build the docs
     doctests: Invoke sphinx-build to run doctests
     linkcheck: Check for broken links in the documentation
+passenv =
+    SETUPTOOLS_*
 setenv =
     DOCSDIR = {toxinidir}/docs
     BUILDDIR = {toxinidir}/docs/_build
     docs: BUILD = html
     doctests: BUILD = doctest
     linkcheck: BUILD = linkcheck
 deps =
@@ -74,11 +83,12 @@
 skip_install = True
 changedir = {toxinidir}
 passenv =
     # See: https://twine.readthedocs.io/en/latest/
     TWINE_USERNAME
     TWINE_PASSWORD
     TWINE_REPOSITORY
+    TWINE_REPOSITORY_URL
 deps = twine
 commands =
     python -m twine check dist/*
     python -m twine upload {posargs:--repository {env:TWINE_REPOSITORY:testpypi}} dist/*
```

