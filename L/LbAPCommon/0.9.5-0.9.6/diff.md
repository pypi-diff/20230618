# Comparing `tmp/LbAPCommon-0.9.5.tar.gz` & `tmp/LbAPCommon-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbAPCommon-0.9.5.tar", last modified: Sun Jun 18 20:27:31 2023, max compression
+gzip compressed data, was "LbAPCommon-0.9.6.tar", last modified: Sun Jun 18 20:46:23 2023, max compression
```

## Comparing `LbAPCommon-0.9.5.tar` & `LbAPCommon-0.9.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.052000 LbAPCommon-0.9.5/
--rw-r--r--   0 root         (0) root         (0)     2039 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1562 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1144 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-18 20:27:31.052000 LbAPCommon-0.9.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      856 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/README.md
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/environment.yaml
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-18 20:27:31.052000 LbAPCommon-0.9.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2536 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.040000 LbAPCommon-0.9.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.040000 LbAPCommon-0.9.5/src/LbAPCommon/
--rw-r--r--   0 root         (0) root         (0)     2108 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/cern_sso.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon/checks/
--rw-r--r--   0 root         (0) root         (0)     4881 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4835 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/checks/common.py
--rw-r--r--   0 root         (0) root         (0)     7357 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/checks/num_entries.py
--rw-r--r--   0 root         (0) root         (0)    39009 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/checks/range.py
--rw-r--r--   0 root         (0) root         (0)    20997 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     9344 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/checks/validations.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/config.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/hacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon/linting/
--rw-r--r--   0 root         (0) root         (0)      999 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/linting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6047 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/linting/bk_paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon/options_parsing/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/options_parsing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
--rw-r--r--   0 root         (0) root         (0)    26734 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/parsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon/validators/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/validators/bookkeeping_xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon/validators/logs/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/validators/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon/validators/logs/data/
--rw-r--r--   0 root         (0) root         (0)     3535 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/src/LbAPCommon/validators/logs/data/known_messages.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-18 20:27:30.000000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1786 2023-06-18 20:27:31.000000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 20:27:30.000000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 20:27:30.000000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-18 20:27:30.000000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-18 20:27:30.000000 LbAPCommon-0.9.5/src/LbAPCommon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.044000 LbAPCommon-0.9.5/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.048000 LbAPCommon-0.9.5/tests/checks/
--rw-r--r--   0 root         (0) root         (0)   471631 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/checks/example_tuple_with_lumi.root
--rw-r--r--   0 root         (0) root         (0)    47368 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/checks/test_advanced.py
--rw-r--r--   0 root         (0) root         (0)    64427 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/checks/test_simple.py
--rw-r--r--   0 root         (0) root         (0)    90340 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/checks/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.048000 LbAPCommon-0.9.5/tests/example-logs/
--rw-r--r--   0 root         (0) root         (0)   516613 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/error-failed-to-read-file.log
--rw-r--r--   0 root         (0) root         (0)   344567 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/error-illegal-instruction.log
--rw-r--r--   0 root         (0) root         (0)     3373 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/error-missing-shared-library.log
--rw-r--r--   0 root         (0) root         (0)     2723 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/error-platform-unsupported.log
--rw-r--r--   0 root         (0) root         (0)   584650 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/error-related-info-missing.log
--rw-r--r--   0 root         (0) root         (0)   135940 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/good-DaVinci_00110296_00000038_1.log
--rw-r--r--   0 root         (0) root         (0)   139869 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/good-DaVinci_00110296_00000194_1.log
--rw-r--r--   0 root         (0) root         (0)   751141 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/example-logs/good-Gauss_00104988_00000011_1.log
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.052000 LbAPCommon-0.9.5/tests/linting/
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/linting/test_bk_paths.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/linting/test_processing_pass.py
--rw-r--r--   0 root         (0) root         (0)    40668 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/test_good_parsing.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/test_hacks.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/test_log_parsing.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/test_log_splitting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:27:31.052000 LbAPCommon-0.9.5/tests/test_performance/
--rw-r--r--   0 root         (0) root         (0)    44540 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/test_performance/example1.yaml
--rw-r--r--   0 root         (0) root         (0)     1113 2023-06-18 20:27:16.000000 LbAPCommon-0.9.5/tests/test_performance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.280000 LbAPCommon-0.9.6/
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-18 20:46:23.280000 LbAPCommon-0.9.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/README.md
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/environment.yaml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-18 20:46:23.280000 LbAPCommon-0.9.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.264000 LbAPCommon-0.9.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.268000 LbAPCommon-0.9.6/src/LbAPCommon/
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/cern_sso.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.272000 LbAPCommon-0.9.6/src/LbAPCommon/checks/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/checks/common.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/checks/num_entries.py
+-rw-r--r--   0 root         (0) root         (0)    39009 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/checks/range.py
+-rw-r--r--   0 root         (0) root         (0)    20997 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9381 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/checks/validations.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/config.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/hacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.272000 LbAPCommon-0.9.6/src/LbAPCommon/linting/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/linting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6047 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/linting/bk_paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.272000 LbAPCommon-0.9.6/src/LbAPCommon/options_parsing/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/options_parsing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
+-rw-r--r--   0 root         (0) root         (0)    26734 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/parsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.272000 LbAPCommon-0.9.6/src/LbAPCommon/validators/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/validators/bookkeeping_xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.272000 LbAPCommon-0.9.6/src/LbAPCommon/validators/logs/
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/validators/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.272000 LbAPCommon-0.9.6/src/LbAPCommon/validators/logs/data/
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/src/LbAPCommon/validators/logs/data/known_messages.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.268000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-18 20:46:23.000000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-06-18 20:46:23.000000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 20:46:23.000000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 20:46:23.000000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-18 20:46:23.000000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-18 20:46:23.000000 LbAPCommon-0.9.6/src/LbAPCommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.276000 LbAPCommon-0.9.6/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.276000 LbAPCommon-0.9.6/tests/checks/
+-rw-r--r--   0 root         (0) root         (0)   471631 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/checks/example_tuple_with_lumi.root
+-rw-r--r--   0 root         (0) root         (0)    47368 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/checks/test_advanced.py
+-rw-r--r--   0 root         (0) root         (0)    64427 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/checks/test_simple.py
+-rw-r--r--   0 root         (0) root         (0)    90340 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/checks/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.280000 LbAPCommon-0.9.6/tests/example-logs/
+-rw-r--r--   0 root         (0) root         (0)   516613 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/error-failed-to-read-file.log
+-rw-r--r--   0 root         (0) root         (0)   344567 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/error-illegal-instruction.log
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/error-missing-shared-library.log
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/error-platform-unsupported.log
+-rw-r--r--   0 root         (0) root         (0)   584650 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/error-related-info-missing.log
+-rw-r--r--   0 root         (0) root         (0)   135940 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/good-DaVinci_00110296_00000038_1.log
+-rw-r--r--   0 root         (0) root         (0)   139869 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/good-DaVinci_00110296_00000194_1.log
+-rw-r--r--   0 root         (0) root         (0)   751141 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/example-logs/good-Gauss_00104988_00000011_1.log
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.280000 LbAPCommon-0.9.6/tests/linting/
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/linting/test_bk_paths.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/linting/test_processing_pass.py
+-rw-r--r--   0 root         (0) root         (0)    40668 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/test_good_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/test_hacks.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/test_log_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/test_log_splitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:46:23.280000 LbAPCommon-0.9.6/tests/test_performance/
+-rw-r--r--   0 root         (0) root         (0)    44540 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/test_performance/example1.yaml
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-18 20:46:08.000000 LbAPCommon-0.9.6/tests/test_performance.py
```

### Comparing `LbAPCommon-0.9.5/.gitignore` & `LbAPCommon-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/.gitlab-ci.yml` & `LbAPCommon-0.9.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/.pre-commit-config.yaml` & `LbAPCommon-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/LICENSE` & `LbAPCommon-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/PKG-INFO` & `LbAPCommon-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPCommon
-Version: 0.9.5
+Version: 0.9.6
 Summary: Common utilities used by LHCb DPA WP2 related software
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Keywords: LHCb HEP CERN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LbAPCommon-0.9.5/README.md` & `LbAPCommon-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/setup.py` & `LbAPCommon-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/__init__.py` & `LbAPCommon-0.9.6/src/LbAPCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/cern_sso.py` & `LbAPCommon-0.9.6/src/LbAPCommon/cern_sso.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/checks/__init__.py` & `LbAPCommon-0.9.6/src/LbAPCommon/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/checks/common.py` & `LbAPCommon-0.9.6/src/LbAPCommon/checks/common.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/checks/num_entries.py` & `LbAPCommon-0.9.6/src/LbAPCommon/checks/num_entries.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/checks/range.py` & `LbAPCommon-0.9.6/src/LbAPCommon/checks/range.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/checks/utils.py` & `LbAPCommon-0.9.6/src/LbAPCommon/checks/utils.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/checks/validations.py` & `LbAPCommon-0.9.6/src/LbAPCommon/checks/validations.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     if "bk_query" in job_data["input"]:
         input_type = "bk_query"
         job_input = job_data["input"]["bk_query"].lower()
     elif "job_name" in job_data["input"]:
         input_type = "job_name"
         job_input = job_data["input"]["job_name"].lower()
     elif "transform_ids" in job_data["input"]:
+        input_type = "transform_ids"
         job_input = tuple(job_data["input"]["transform_ids"])
     else:
         result.error(
             f"Job input for {job_name} must either be a bk_query, job_name or transform_ids!"
         )
 
     job_names = input_to_job[job_input]
```

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/config.py` & `LbAPCommon-0.9.6/src/LbAPCommon/config.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/hacks.py` & `LbAPCommon-0.9.6/src/LbAPCommon/hacks.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/linting/__init__.py` & `LbAPCommon-0.9.6/src/LbAPCommon/linting/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/linting/bk_paths.py` & `LbAPCommon-0.9.6/src/LbAPCommon/linting/bk_paths.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/options_parsing/__init__.py` & `LbAPCommon-0.9.6/src/LbAPCommon/options_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py` & `LbAPCommon-0.9.6/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/parsing.py` & `LbAPCommon-0.9.6/src/LbAPCommon/parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/validators/__init__.py` & `LbAPCommon-0.9.6/src/LbAPCommon/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/validators/bookkeeping_xml.py` & `LbAPCommon-0.9.6/src/LbAPCommon/validators/bookkeeping_xml.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/validators/logs/__init__.py` & `LbAPCommon-0.9.6/src/LbAPCommon/validators/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon/validators/logs/data/known_messages.yaml` & `LbAPCommon-0.9.6/src/LbAPCommon/validators/logs/data/known_messages.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon.egg-info/PKG-INFO` & `LbAPCommon-0.9.6/src/LbAPCommon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPCommon
-Version: 0.9.5
+Version: 0.9.6
 Summary: Common utilities used by LHCb DPA WP2 related software
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Keywords: LHCb HEP CERN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LbAPCommon-0.9.5/src/LbAPCommon.egg-info/SOURCES.txt` & `LbAPCommon-0.9.6/src/LbAPCommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/checks/example_tuple_with_lumi.root` & `LbAPCommon-0.9.6/tests/checks/example_tuple_with_lumi.root`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/checks/test_advanced.py` & `LbAPCommon-0.9.6/tests/checks/test_advanced.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/checks/test_simple.py` & `LbAPCommon-0.9.6/tests/checks/test_simple.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/checks/test_utils.py` & `LbAPCommon-0.9.6/tests/checks/test_utils.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/error-failed-to-read-file.log` & `LbAPCommon-0.9.6/tests/example-logs/error-failed-to-read-file.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/error-illegal-instruction.log` & `LbAPCommon-0.9.6/tests/example-logs/error-illegal-instruction.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/error-missing-shared-library.log` & `LbAPCommon-0.9.6/tests/example-logs/error-missing-shared-library.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/error-platform-unsupported.log` & `LbAPCommon-0.9.6/tests/example-logs/error-platform-unsupported.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/error-related-info-missing.log` & `LbAPCommon-0.9.6/tests/example-logs/error-related-info-missing.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/good-DaVinci_00110296_00000038_1.log` & `LbAPCommon-0.9.6/tests/example-logs/good-DaVinci_00110296_00000038_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/good-DaVinci_00110296_00000194_1.log` & `LbAPCommon-0.9.6/tests/example-logs/good-DaVinci_00110296_00000194_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/example-logs/good-Gauss_00104988_00000011_1.log` & `LbAPCommon-0.9.6/tests/example-logs/good-Gauss_00104988_00000011_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/linting/test_bk_paths.py` & `LbAPCommon-0.9.6/tests/linting/test_bk_paths.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/linting/test_processing_pass.py` & `LbAPCommon-0.9.6/tests/linting/test_processing_pass.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/test_good_parsing.py` & `LbAPCommon-0.9.6/tests/test_good_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/test_hacks.py` & `LbAPCommon-0.9.6/tests/test_hacks.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/test_log_parsing.py` & `LbAPCommon-0.9.6/tests/test_log_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/test_log_splitting.py` & `LbAPCommon-0.9.6/tests/test_log_splitting.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/test_performance/example1.yaml` & `LbAPCommon-0.9.6/tests/test_performance/example1.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.5/tests/test_performance.py` & `LbAPCommon-0.9.6/tests/test_performance.py`

 * *Files identical despite different names*

