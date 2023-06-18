# Comparing `tmp/LbAPCommon-0.9.3.tar.gz` & `tmp/LbAPCommon-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbAPCommon-0.9.3.tar", last modified: Mon Apr 17 09:45:24 2023, max compression
+gzip compressed data, was "LbAPCommon-0.9.4.tar", last modified: Sun Jun 18 20:05:08 2023, max compression
```

## Comparing `LbAPCommon-0.9.3.tar` & `LbAPCommon-0.9.4.tar`

### file list

```diff
@@ -1,64 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.908000 LbAPCommon-0.9.3/
--rw-r--r--   0 root         (0) root         (0)     2039 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1144 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    32472 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-17 09:45:24.908000 LbAPCommon-0.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      856 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/README.md
--rw-r--r--   0 root         (0) root         (0)      409 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/environment.yaml
--rw-r--r--   0 root         (0) root         (0)      301 2023-04-17 09:45:24.908000 LbAPCommon-0.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2536 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.892000 LbAPCommon-0.9.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.896000 LbAPCommon-0.9.3/src/LbAPCommon/
--rw-r--r--   0 root         (0) root         (0)     2108 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5011 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/cern_sso.py
--rw-r--r--   0 root         (0) root         (0)    68549 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/checks.py
--rw-r--r--   0 root         (0) root         (0)    19904 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/checks_utils.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/config.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/hacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.896000 LbAPCommon-0.9.3/src/LbAPCommon/linting/
--rw-r--r--   0 root         (0) root         (0)      999 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/linting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6047 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/linting/bk_paths.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.900000 LbAPCommon-0.9.3/src/LbAPCommon/options_parsing/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/options_parsing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
--rw-r--r--   0 root         (0) root         (0)    26704 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/parsing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.900000 LbAPCommon-0.9.3/src/LbAPCommon/validators/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/validators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/validators/bookkeeping_xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.900000 LbAPCommon-0.9.3/src/LbAPCommon/validators/logs/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/validators/logs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.900000 LbAPCommon-0.9.3/src/LbAPCommon/validators/logs/data/
--rw-r--r--   0 root         (0) root         (0)     3535 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/src/LbAPCommon/validators/logs/data/known_messages.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.896000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-17 09:45:24.000000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1640 2023-04-17 09:45:24.000000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 09:45:24.000000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 09:45:24.000000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-17 09:45:24.000000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-17 09:45:24.000000 LbAPCommon-0.9.3/src/LbAPCommon.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.900000 LbAPCommon-0.9.3/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.900000 LbAPCommon-0.9.3/tests/checks/
--rw-r--r--   0 root         (0) root         (0)   471631 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/checks/example_tuple_with_lumi.root
--rw-r--r--   0 root         (0) root         (0)    47226 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/checks/test_advanced.py
--rw-r--r--   0 root         (0) root         (0)    65451 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/checks/test_simple.py
--rw-r--r--   0 root         (0) root         (0)    90324 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/checks/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.904000 LbAPCommon-0.9.3/tests/example-logs/
--rw-r--r--   0 root         (0) root         (0)   516613 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/error-failed-to-read-file.log
--rw-r--r--   0 root         (0) root         (0)   344567 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/error-illegal-instruction.log
--rw-r--r--   0 root         (0) root         (0)     3373 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/error-missing-shared-library.log
--rw-r--r--   0 root         (0) root         (0)     2723 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/error-platform-unsupported.log
--rw-r--r--   0 root         (0) root         (0)   584650 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/error-related-info-missing.log
--rw-r--r--   0 root         (0) root         (0)   135940 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/good-DaVinci_00110296_00000038_1.log
--rw-r--r--   0 root         (0) root         (0)   139869 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/good-DaVinci_00110296_00000194_1.log
--rw-r--r--   0 root         (0) root         (0)   751141 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/example-logs/good-Gauss_00104988_00000011_1.log
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.908000 LbAPCommon-0.9.3/tests/linting/
--rw-r--r--   0 root         (0) root         (0)     1839 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/linting/test_bk_paths.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/linting/test_processing_pass.py
--rw-r--r--   0 root         (0) root         (0)    40723 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/test_good_parsing.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/test_hacks.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/test_log_parsing.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/test_log_splitting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:45:24.908000 LbAPCommon-0.9.3/tests/test_performance/
--rw-r--r--   0 root         (0) root         (0)    44540 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/test_performance/example1.yaml
--rw-r--r--   0 root         (0) root         (0)     1113 2023-04-17 09:45:05.000000 LbAPCommon-0.9.3/tests/test_performance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.336000 LbAPCommon-0.9.4/
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-18 20:05:08.336000 LbAPCommon-0.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/environment.yaml
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-18 20:05:08.336000 LbAPCommon-0.9.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.320000 LbAPCommon-0.9.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.324000 LbAPCommon-0.9.4/src/LbAPCommon/
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/cern_sso.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/src/LbAPCommon/checks/
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4835 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/checks/common.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/checks/num_entries.py
+-rw-r--r--   0 root         (0) root         (0)    39009 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/checks/range.py
+-rw-r--r--   0 root         (0) root         (0)    20808 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9344 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/checks/validations.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/config.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/hacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/src/LbAPCommon/linting/
+-rw-r--r--   0 root         (0) root         (0)      999 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/linting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6047 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/linting/bk_paths.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/src/LbAPCommon/options_parsing/
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/options_parsing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
+-rw-r--r--   0 root         (0) root         (0)    26734 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/parsing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/src/LbAPCommon/validators/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/validators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/validators/bookkeeping_xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/src/LbAPCommon/validators/logs/
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/validators/logs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/src/LbAPCommon/validators/logs/data/
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/src/LbAPCommon/validators/logs/data/known_messages.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.324000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-18 20:05:08.000000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-06-18 20:05:08.000000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 20:05:08.000000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 20:05:08.000000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-18 20:05:08.000000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-18 20:05:08.000000 LbAPCommon-0.9.4/src/LbAPCommon.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.328000 LbAPCommon-0.9.4/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.332000 LbAPCommon-0.9.4/tests/checks/
+-rw-r--r--   0 root         (0) root         (0)   471631 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/checks/example_tuple_with_lumi.root
+-rw-r--r--   0 root         (0) root         (0)    47368 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/checks/test_advanced.py
+-rw-r--r--   0 root         (0) root         (0)    64427 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/checks/test_simple.py
+-rw-r--r--   0 root         (0) root         (0)    90340 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/checks/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.336000 LbAPCommon-0.9.4/tests/example-logs/
+-rw-r--r--   0 root         (0) root         (0)   516613 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/error-failed-to-read-file.log
+-rw-r--r--   0 root         (0) root         (0)   344567 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/error-illegal-instruction.log
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/error-missing-shared-library.log
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/error-platform-unsupported.log
+-rw-r--r--   0 root         (0) root         (0)   584650 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/error-related-info-missing.log
+-rw-r--r--   0 root         (0) root         (0)   135940 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/good-DaVinci_00110296_00000038_1.log
+-rw-r--r--   0 root         (0) root         (0)   139869 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/good-DaVinci_00110296_00000194_1.log
+-rw-r--r--   0 root         (0) root         (0)   751141 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/example-logs/good-Gauss_00104988_00000011_1.log
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.336000 LbAPCommon-0.9.4/tests/linting/
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/linting/test_bk_paths.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/linting/test_processing_pass.py
+-rw-r--r--   0 root         (0) root         (0)    40668 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/test_good_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/test_hacks.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/test_log_parsing.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/test_log_splitting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 20:05:08.336000 LbAPCommon-0.9.4/tests/test_performance/
+-rw-r--r--   0 root         (0) root         (0)    44540 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/test_performance/example1.yaml
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-06-18 20:04:52.000000 LbAPCommon-0.9.4/tests/test_performance.py
```

### Comparing `LbAPCommon-0.9.3/.gitignore` & `LbAPCommon-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/.gitlab-ci.yml` & `LbAPCommon-0.9.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/.pre-commit-config.yaml` & `LbAPCommon-0.9.4/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
```

### Comparing `LbAPCommon-0.9.3/LICENSE` & `LbAPCommon-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/PKG-INFO` & `LbAPCommon-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPCommon
-Version: 0.9.3
+Version: 0.9.4
 Summary: Common utilities used by LHCb DPA WP2 related software
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Keywords: LHCb HEP CERN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LbAPCommon-0.9.3/README.md` & `LbAPCommon-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/setup.py` & `LbAPCommon-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/__init__.py` & `LbAPCommon-0.9.4/src/LbAPCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/cern_sso.py` & `LbAPCommon-0.9.4/src/LbAPCommon/cern_sso.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/checks_utils.py` & `LbAPCommon-0.9.4/src/LbAPCommon/checks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,46 @@
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 """Contains utility functions used to display and save the output of the checks.
 """
 import copy
 import json
 import warnings
+from collections import defaultdict
 
 import hist
 import numpy as np
 import uproot
 from hist import Hist
 
-from LbAPCommon.checks import CheckResult
+from .common import CheckResult
+
+
+def map_input_to_jobs(jobs_data: dict, bk_queries_only=False):
+    """Map each input used in the production to the job name(s) that use it as input.
+
+    Args:
+        jobs_data (dict): Configuration for all of the jobs.
+
+    Returns:
+        dict: A mapping from each input to a list of each job in the production that uses it.
+    """
+    input_to_job = defaultdict(set)
+    for job_name, job_data in jobs_data.items():
+        if "bk_query" in job_data["input"]:
+            input_to_job[job_data["input"]["bk_query"].lower()].add(job_name)
+        elif "job_name" in job_data["input"]:
+            if not bk_queries_only:
+                input_to_job[job_data["input"]["job_name"].lower()].add(job_name)
+        else:
+            raise ValueError(
+                f"Job input for {job_name} must either be a bk_query or a job_name!"
+            )
+
+    return input_to_job
 
 
 def hist_to_root(job_name, check_results, output_path):
     """Save histograms to a root file.
 
     Creates a .root file at the provided output location, containing any
     histograms stored in the check results.
```

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/config.py` & `LbAPCommon-0.9.4/src/LbAPCommon/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,8 +42,8 @@
     "duplicate_inputs",
     "job_name_matches_polarity",
     "both_polarities_used",
 ]
 validation_types = [
     *simple_validations,
 ]
-validation_modes = ["Strict", "Lenient", "None"]
+validation_modes = ["Strict", "Lenient", "Ignore"]
```

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/hacks.py` & `LbAPCommon-0.9.4/src/LbAPCommon/hacks.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/linting/__init__.py` & `LbAPCommon-0.9.4/src/LbAPCommon/linting/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/linting/bk_paths.py` & `LbAPCommon-0.9.4/src/LbAPCommon/linting/bk_paths.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/options_parsing/__init__.py` & `LbAPCommon-0.9.4/src/LbAPCommon/options_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py` & `LbAPCommon-0.9.4/src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/parsing.py` & `LbAPCommon-0.9.4/src/LbAPCommon/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,17 +565,17 @@
         repo_root (str): Repository location.
         prod_name (str): Production name.
 
     Raises:
         ValueError: Raised if there are showstopper issues in the parsed job configuration.
     """
     # Ensure all values that can be either a list or a string are lists of strings
-    for job_name, job_data in jobs_data.items():
+    for job_name, _ in jobs_data.items():
         try:
-            _validate_job_data(repo_root, prod_name, job_name, job_data, checks_data)
+            _validate_job_data(repo_root, prod_name, job_name, jobs_data, checks_data)
         except Exception as e:
             raise ValueError(f"Failed to validate {job_name!r} with error {e!r}") from e
 
     # Ensure job name inputs are unambiguous
     for job_name, job_data in jobs_data.items():
         if "job_name" in job_data["input"]:
             if job_data["input"]["job_name"] not in jobs_data:
@@ -604,15 +604,16 @@
     # Validate checks
     try:
         _validate_checks_data(checks_data, jobs_data)
     except Exception as e:
         raise ValueError(f"Failed to validate checks with error {e!r}") from e
 
 
-def _validate_job_data(repo_root, prod_name, job_name, job_data, checks_data):
+def _validate_job_data(repo_root, prod_name, job_name, jobs_data, checks_data):
+    job_data = jobs_data[job_name]
     # Normalise list/str fields to always be lists
     for prop in ["output", "options", "inform", "checks", "extra_checks"]:
         if not isinstance(job_data.get(prop, []), (list, dict)):
             job_data[prop] = [job_data[prop]]
 
     # Validate the input data
     if "bk_query" in job_data["input"]:
```

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/validators/__init__.py` & `LbAPCommon-0.9.4/src/LbAPCommon/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/validators/bookkeeping_xml.py` & `LbAPCommon-0.9.4/src/LbAPCommon/validators/bookkeeping_xml.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/validators/logs/__init__.py` & `LbAPCommon-0.9.4/src/LbAPCommon/validators/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon/validators/logs/data/known_messages.yaml` & `LbAPCommon-0.9.4/src/LbAPCommon/validators/logs/data/known_messages.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon.egg-info/PKG-INFO` & `LbAPCommon-0.9.4/src/LbAPCommon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPCommon
-Version: 0.9.3
+Version: 0.9.4
 Summary: Common utilities used by LHCb DPA WP2 related software
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/LbAPCommon
 Keywords: LHCb HEP CERN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `LbAPCommon-0.9.3/src/LbAPCommon.egg-info/SOURCES.txt` & `LbAPCommon-0.9.4/src/LbAPCommon.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 LICENSE
 README.md
 environment.yaml
 setup.cfg
 setup.py
 src/LbAPCommon/__init__.py
 src/LbAPCommon/cern_sso.py
-src/LbAPCommon/checks.py
-src/LbAPCommon/checks_utils.py
 src/LbAPCommon/config.py
 src/LbAPCommon/hacks.py
 src/LbAPCommon/parsing.py
 src/LbAPCommon.egg-info/PKG-INFO
 src/LbAPCommon.egg-info/SOURCES.txt
 src/LbAPCommon.egg-info/dependency_links.txt
 src/LbAPCommon.egg-info/not-zip-safe
 src/LbAPCommon.egg-info/requires.txt
 src/LbAPCommon.egg-info/top_level.txt
+src/LbAPCommon/checks/__init__.py
+src/LbAPCommon/checks/common.py
+src/LbAPCommon/checks/num_entries.py
+src/LbAPCommon/checks/range.py
+src/LbAPCommon/checks/utils.py
+src/LbAPCommon/checks/validations.py
 src/LbAPCommon/linting/__init__.py
 src/LbAPCommon/linting/bk_paths.py
 src/LbAPCommon/options_parsing/__init__.py
 src/LbAPCommon/options_parsing/gaudi_pickle_to_json.py
 src/LbAPCommon/validators/__init__.py
 src/LbAPCommon/validators/bookkeeping_xml.py
 src/LbAPCommon/validators/logs/__init__.py
```

### Comparing `LbAPCommon-0.9.3/tests/checks/example_tuple_with_lumi.root` & `LbAPCommon-0.9.4/tests/checks/example_tuple_with_lumi.root`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/checks/test_advanced.py` & `LbAPCommon-0.9.4/tests/checks/test_advanced.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,30 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
+import json
 from textwrap import dedent
 
 import pytest
 
 import LbAPCommon
 from LbAPCommon import checks
-from LbAPCommon.checks_utils import checks_to_JSON
+from LbAPCommon.checks.utils import checks_to_JSON
 
 pytest.importorskip("XRootD")  # tests here will not run on CI
 
 
+def _regularise_json(s):
+    return dedent(json.dumps(json.loads(s), indent="  "))
+
+
 def test_num_entries_parsing_to_JSON():
     rendered_yaml = dedent(
         """\
     checks:
         check_num_entries:
             type: num_entries
             count: 1000
@@ -61,22 +66,22 @@
         job_name: {
             check_name: result,
         }
     }
 
     checks_json = checks_to_JSON(checks_data, check_results_with_job)
 
-    json_expected = dedent(
+    json_expected = _regularise_json(
         """\
     {
       "job_1": {
         "check_num_entries": {
           "passed": true,
           "messages": [
-            "Found 5135823 in DecayTree (1000 required)"
+            [0, "Found 5135823 in DecayTree (1000 required)"]
           ],
           "can_combine": true,
           "input": {
             "type": "num_entries",
             "count": 1000,
             "tree_pattern": "DecayTree"
           },
@@ -145,22 +150,22 @@
         job_name: {
             check_name: result,
         }
     }
 
     checks_json = checks_to_JSON(checks_data, check_results_with_job)
 
-    json_expected = dedent(
+    json_expected = _regularise_json(
         """\
 {
   "job_1": {
     "check_range": {
       "passed": true,
       "messages": [
-        "Histogram of H1_PZ successfully filled from TTree DecayTree (contains 4776546.0 events)"
+        [0, "Histogram of H1_PZ successfully filled from TTree DecayTree (contains 4776546.0 events)"]
       ],
       "can_combine": true,
       "input": {
         "type": "range",
         "expression": "H1_PZ",
         "limits": {
           "min": 0.0,
@@ -372,22 +377,22 @@
         job_name: {
             check_name: result,
         }
     }
 
     checks_json = checks_to_JSON(checks_data, check_results_with_job)
 
-    json_expected = dedent(
+    json_expected = _regularise_json(
         """\
 {
   "job_1": {
     "check_range_nd": {
       "passed": true,
       "messages": [
-        "Histogram of H1_PZ, H2_PZ successfully filled from TTree DecayTree (contains 5134453.0 events)"
+        [0, "Histogram of H1_PZ, H2_PZ successfully filled from TTree DecayTree (contains 5134453.0 events)"]
       ],
       "can_combine": true,
       "input": {
         "type": "range_nd",
         "expressions": {
           "x": "H1_PZ",
           "y": "H2_PZ"
```

### Comparing `LbAPCommon-0.9.3/tests/checks/test_simple.py` & `LbAPCommon-0.9.4/tests/checks/test_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         ["check_num_entries"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check_num_entries"]
     assert result.passed
-    assert result.messages == ["Found 5135823 in DecayTree (1000 required)"]
+    assert result.has_all_messages("Found 5135823 in DecayTree (1000 required)")
     assert result.tree_data["DecayTree"]["num_entries"] == 5135823
 
 
 def test_num_entries_passing_multiple_files():
     rendered_yaml = dedent(
         """\
     checks:
@@ -89,15 +89,15 @@
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root",
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetUp.root",
         ],
     )["check_num_entries"]
     assert result.passed
-    assert result.messages == ["Found 8556118 in DecayTree (1000 required)"]
+    assert result.has_all_messages("Found 8556118 in DecayTree (1000 required)")
     assert result.tree_data["DecayTree"]["num_entries"] == 8556118
 
 
 def test_num_entries_failing():
     rendered_yaml = dedent(
         """\
     checks:
@@ -127,15 +127,17 @@
         ["check_num_entries"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check_num_entries"]
     assert not result.passed
-    assert result.messages == ["Found 5135823 in DecayTree (1000000000 required)"]
+    assert result.has_all_messages(
+        "Found too little entries 5135823 in DecayTree (1000000000 required)"
+    )
     assert result.tree_data["DecayTree"]["num_entries"] == 5135823
 
 
 def test_lenient_num_entries_failing():
     rendered_yaml = dedent(
         """\
     checks:
@@ -166,30 +168,29 @@
         ["check_num_entries"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check_num_entries"]
     assert result.passed
-    assert result.messages == [
-        "Found 5135823 in DecayTree (1000000000 required)",
-        "Passed despite failure due to mode being set to Lenient.",
-    ]
+    assert result.has_all_messages(
+        "Found too little entries 5135823 in DecayTree (1000000000 required)",
+    )
     assert result.tree_data["DecayTree"]["num_entries"] == 5135823
 
 
 def test_none_num_entries_failing():
     rendered_yaml = dedent(
         """\
     checks:
         check_num_entries:
             type: num_entries
             count: 1000000000
             tree_pattern: DecayTree
-            mode: None
+            mode: Ignore
 
     job_1:
         application: DaVinci/v45r8
         input:
             bk_query: /bookkeeping/path/ALLSTREAMS.DST
         output: FILETYPE.ROOT
         options:
@@ -208,15 +209,15 @@
         ["check_num_entries"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check_num_entries"]
     assert result.passed
-    assert result.messages == ["Automatically passed as the mode (None) was requested!"]
+    assert result.has_all_messages("Check ignored due to user configuration")
 
 
 def test_num_entries_failing_tree_name():
     rendered_yaml = dedent(
         """\
     checks:
         check_num_entries:
@@ -245,15 +246,15 @@
         ["check_num_entries"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check_num_entries"]
     assert not result.passed
-    assert result.messages == ["No TTree objects found that match RandomName"]
+    assert result.has_all_messages("No TTree objects found that match RandomName")
     for _key, data in result.tree_data.items():
         assert data["histograms"] == []
 
 
 def test_num_entries_per_invpb_passing():
     rendered_yaml = dedent(
         """\
@@ -284,17 +285,17 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Found 11513.1 entries per unit luminosity (pb-1) in DecayTree (10000.0 required)"
-    ]
+    )
     assert result.tree_data["DecayTree"]["num_entries_per_invpb"] == 11513.1
 
 
 def test_num_entries_per_invpb_failing():
     rendered_yaml = dedent(
         """\
     checks:
@@ -324,17 +325,17 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert not result.passed
-    assert result.messages == [
-        "Found 11513.1 entries per unit luminosity (pb-1) in DecayTree (10000000.0 required)"
-    ]
+    assert result.has_all_messages(
+        "Found too little 11513.1 entries per unit luminosity (pb-1) in DecayTree (10000000.0 required)"
+    )
     assert result.tree_data["DecayTree"]["num_entries_per_invpb"] == 11513.1
 
 
 def test_num_entries_per_invpb_failing_MC():
     rendered_yaml = dedent(
         """\
     checks:
@@ -365,17 +366,17 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Failed to get luminosity information (total luminosity = 0)"
-    ]
+    )
 
 
 def test_num_entries_per_invpb_failing_MC_nameTTree():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -404,17 +405,17 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "No TTree objects found that match RandomName",
-    ]
+    )
 
 
 def test_range_check_passing():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -447,17 +448,17 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Histogram of H1_PZ successfully filled from TTree DecayTree (contains 5134459.0 events)"
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 5134459
 
 
 def test_range_check_passing_multiple_files():
     rendered_yaml = dedent(
@@ -494,29 +495,29 @@
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root",
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetUp.root",
         ],
     )["check"]
     assert result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Histogram of H1_PZ successfully filled from TTree DecayTree (contains 8553802.0 events)"
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 8553802
 
 
 def test_range_check_DTF_passing():
     rendered_yaml = dedent(
         """\
     checks:
         check:
             type: range
-            expression: Dst_D0Fit_M
+            expression: Dst_D0Fit_M[:, 0]
             limits:
                 min: 2000.0
                 max: 2080.0
             n_bins: 50
             tree_pattern: DecayTree
 
     job_1:
@@ -539,19 +540,17 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert result.passed
-    assert result.messages == [
-        "Expression 'Dst_D0Fit_M' evaluated to a variable-length array with shape '37685 * var * float32' in 'DecayTree'."
-        " Selecting by default Dst_D0Fit_M[:,0]. If this is not intended, please update the expression value accordingly.",
-        "Histogram of Dst_D0Fit_M successfully filled from TTree DecayTree (contains 37515.0 events)",
-    ]
+    assert result.has_all_messages(
+        "Histogram of Dst_D0Fit_M[:, 0] successfully filled from TTree DecayTree (contains 37515.0 events)",
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 37515
 
 
 def test_range_check_DTF_diff_passing():
     rendered_yaml = dedent(
@@ -586,17 +585,17 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Histogram of Dst_D0Fit_M[:,0]-Dst_D0Fit_D0_M[:,0] successfully filled from TTree DecayTree (contains 28310.0 events)"
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 28310
 
 
 def test_range_check_DTF_diff_failing():
     rendered_yaml = dedent(
@@ -631,22 +630,22 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert not result.passed
-    assert result.messages == [
-        "Expression 'Dst_D0Fit_M-Dst_D0Fit_D0_M' evaluated to a variable-length array with "
-        "shape '37685 * var * float32' in 'DecayTree'."
+    assert result.has_all_messages(
+        "Expression 'Dst_D0Fit_M-Dst_D0Fit_D0_M' evaluated to a variable-length array"
+        " with shape '37685 * var * float32' in 'DecayTree'."
         " Selecting by default Dst_D0Fit_M-Dst_D0Fit_D0_M[:,0]. If this is not intended,"
         " please update the expression value accordingly.",
         "Expression 'Dst_D0Fit_M-Dst_D0Fit_D0_M' evaluated to non 1-D array with type "
         "'37685 * var * float32' in 'DecayTree'",
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     for h in result.tree_data["DecayTree"]["histograms"]:
         assert h.sum() == 0
 
 
 def test_range_check_failing_range():
     rendered_yaml = dedent(
@@ -682,81 +681,80 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == ["No events found in range for Tree DecayTree"]
+    assert result.has_all_messages("No events found in range for Tree DecayTree")
     assert list(result.tree_data.keys()) == ["DecayTree"]
     for h in result.tree_data["DecayTree"]["histograms"]:
         assert h.sum() == 0
 
 
-def test_lenient_range_check_failing_range():
-    rendered_yaml = dedent(
-        """\
-    checks:
-        check:
-            type: range
-            expression: H1_PZ
-            limits:
-                min: -100000.0
-                max: -99999.0
-            n_bins: 50
-            tree_pattern: DecayTree
-            mode: Lenient
-
-    job_1:
-        application: DaVinci/v45r8
-        input:
-            bk_query: /bookkeeping/path/ALLSTREAMS.DST
-        output: FILETYPE.ROOT
-        options:
-            - options.py
-            - $VAR/a.py
-        wg: Charm
-        inform: a.b@c.d
-        checks:
-            - check
-    """
-    )
-    jobs_data, checks_data = LbAPCommon.parse_yaml(rendered_yaml)
-    result = checks.run_job_checks(
-        jobs_data,
-        "job_1",
-        ["check"],
-        checks_data,
-        [
-            "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
-        ],
-    )["check"]
-    assert result.passed
-    assert result.messages == [
-        "No events found in range for Tree DecayTree",
-        "Passed despite failure due to mode being set to Lenient.",
-    ]
-    assert list(result.tree_data.keys()) == ["DecayTree"]
-    for h in result.tree_data["DecayTree"]["histograms"]:
-        assert h.sum() == 0
+# def test_lenient_range_check_failing_range():
+#     rendered_yaml = dedent(
+#         """\
+#     checks:
+#         check:
+#             type: range
+#             expression: H1_PZ
+#             limits:
+#                 min: -100000.0
+#                 max: -99999.0
+#             n_bins: 50
+#             tree_pattern: DecayTree
+#             mode: Lenient
+
+#     job_1:
+#         application: DaVinci/v45r8
+#         input:
+#             bk_query: /bookkeeping/path/ALLSTREAMS.DST
+#         output: FILETYPE.ROOT
+#         options:
+#             - options.py
+#             - $VAR/a.py
+#         wg: Charm
+#         inform: a.b@c.d
+#         checks:
+#             - check
+#     """
+#     )
+#     jobs_data, checks_data = LbAPCommon.parse_yaml(rendered_yaml)
+#     result = checks.run_job_checks(
+#         jobs_data,
+#         "job_1",
+#         ["check"],
+#         checks_data,
+#         [
+#             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
+#         ],
+#     )["check"]
+#     assert result.passed
+#     assert result.has_all_messages(
+#         "No events found in range for Tree DecayTree",
+#     )
+#     assert list(result.tree_data.keys()) == ["DecayTree"]
+#     for h in result.tree_data["DecayTree"]["histograms"]:
+#         assert h.sum() == 0
 
 
 def test_none_range_check_failing_range():
     rendered_yaml = dedent(
         """\
     checks:
         check:
             type: range
             expression: H1_PZ
             limits:
                 min: -100000.0
                 max: -99999.0
             n_bins: 50
             tree_pattern: DecayTree
-            mode: None
+            mode: Ignore
 
     job_1:
         application: DaVinci/v45r8
         input:
             bk_query: /bookkeeping/path/ALLSTREAMS.DST
         output: FILETYPE.ROOT
         options:
@@ -775,15 +773,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert result.passed
-    assert result.messages == ["Automatically passed as the mode (None) was requested!"]
+    assert result.has_all_messages("Check ignored due to user configuration")
 
 
 def test_range_check_failing_missing_branch():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -815,15 +813,15 @@
         "job_1",
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
-    message = result.messages[0]
+    message = result.messages[0][1]
     pattern = r"Missing branch in "
     matched = False
     if re.match(pattern, message):
         matched = True
     assert not result.passed
     assert matched
     assert list(result.tree_data.keys()) == ["DecayTree"]
@@ -865,15 +863,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == ["No TTree objects found that match RandomName"]
+    assert result.has_all_messages("No TTree objects found that match RandomName")
     assert list(result.tree_data.keys()) == []
 
 
 def test_range_check_failing_bad_mean():
     rendered_yaml = dedent(
         """\
     checks:
@@ -909,17 +907,17 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "The observed mean (49110.65313794501) differs from the expected value by 450889.346862055 (<=1.0 required)"
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 5134459
 
 
 def test_range_check_failing_bad_stddev():
     rendered_yaml = dedent(
@@ -957,17 +955,17 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "The observed standard deviation (53099.76473607609) differs from the expected value by 446900.2352639239 (<=1.0 required)"
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 5134459
 
 
 def test_range_check_nd_passing():
     rendered_yaml = dedent(
@@ -1016,33 +1014,33 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Histogram of H1_PZ, H2_PZ successfully filled from TTree DecayTree (contains 2525189.0 events)",
         "Histogram of H1_PZ, H2_PX successfully filled from TTree DecayTree (contains 2525189.0 events)",
         "Histogram of H2_PZ, H2_PX successfully filled from TTree DecayTree (contains 2525189.0 events)",
         "Histogram of H1_PZ, H2_PZ, H2_PX successfully filled from TTree DecayTree (contains 2525189.0 events)",
-    ]
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
 
 
 def test_range_check_nd_DTF_passing():
     rendered_yaml = dedent(
         """\
     checks:
         check:
             type: range_nd
             expressions:
-                x: Dst_D0Fit_M
-                y: Dst_D0Fit_D0_M
+                x: Dst_D0Fit_M[:, 0]
+                y: Dst_D0Fit_D0_M[:, 0]
             limits:
                 x:
                     min: 2000.0
                     max: 2080.0
                 y:
                     min: 1850.0
                     max: 1920.0
@@ -1071,21 +1069,17 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert result.passed
-    assert result.messages == [
-        "Expression 'Dst_D0Fit_M' evaluated to a variable-length array with shape '37685 * var * float32' in 'DecayTree'."
-        " Selecting by default Dst_D0Fit_M[:,0]. If this is not intended, please update the expression value accordingly.",
-        "Expression 'Dst_D0Fit_D0_M' evaluated to a variable-length array with shape '37685 * var * float32' in 'DecayTree'."
-        " Selecting by default Dst_D0Fit_D0_M[:,0]. If this is not intended, please update the expression value accordingly.",
-        "Histogram of Dst_D0Fit_M, Dst_D0Fit_D0_M successfully filled from TTree DecayTree (contains 37515.0 events)",
-    ]
+    assert result.has_all_messages(
+        "Histogram of Dst_D0Fit_M[:, 0], Dst_D0Fit_D0_M[:, 0] successfully filled from TTree DecayTree (contains 37515.0 events)",
+    )
     assert list(result.tree_data.keys()) == ["DecayTree"]
     assert not result.tree_data["DecayTree"]["histograms"] == []
     assert result.tree_data["DecayTree"]["num_entries"] == 37515
 
 
 def test_range_check_nd_failing_missing_limit():
     rendered_yaml = dedent(
@@ -1131,17 +1125,17 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "For each variable, a corresponding range should be defined."
-    ]
+    )
     assert list(result.tree_data.keys()) == []
 
 
 def test_range_check_nd_failing_missing_branch():
     rendered_yaml = dedent(
         """\
     checks:
@@ -1182,15 +1176,15 @@
         "job_1",
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
-    message = result.messages[0]
+    message = result.messages[0][1]
     pattern = r"Missing branch in "
     matched = False
     if re.match(pattern, message):
         matched = True
     assert not result.passed
     assert matched
     assert list(result.tree_data.keys()) == ["DecayTree"]
@@ -1240,15 +1234,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == ["No events found in range for Tree DecayTree"]
+    assert result.has_all_messages("No events found in range for Tree DecayTree")
     assert list(result.tree_data.keys()) == ["DecayTree"]
     for h in result.tree_data["DecayTree"]["histograms"]:
         assert h.sum() == 0
 
 
 def test_range_check_nd_failing_tree_name():
     rendered_yaml = dedent(
@@ -1297,15 +1291,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == ["No TTree objects found that match RandomName"]
+    assert result.has_all_messages("No TTree objects found that match RandomName")
     assert list(result.tree_data.keys()) == []
 
 
 def test_range_check_bkg_subtracted_passing():
     rendered_yaml = dedent(
         """\
     checks:
@@ -1347,17 +1341,16 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/MasterclassDatasets/D0lifetime/2014/MasterclassData.root"
         ],
     )["check"]
     assert result.passed
-    assert (
-        result.messages[0]
-        == "Background subtraction performed successfully for Tree DecayTree"
+    assert result.has_all_messages(
+        "Background subtraction performed successfully for Tree DecayTree"
     )
     assert list(result.tree_data.keys())[0] == "DecayTree"
     assert not result.tree_data["DecayTree"]["histograms"] == []
 
 
 def test_range_check_bkg_subtracted_DTF_passing():
     rendered_yaml = dedent(
@@ -1366,15 +1359,15 @@
         check:
             type: range_bkg_subtracted
             expression: Dst_PX
             limits:
                 min: 0.0
                 max: 500000.0
             n_bins: 50
-            expr_for_subtraction: Dst_D0Fit_M
+            expr_for_subtraction: Dst_D0Fit_M[:, 0]
             mean_sig: 2010.3
             background_shift: 15.0
             background_window: 10.0
             signal_window: 10.0
             blind_ranges:
                 min: 10000.0
                 max: 30000.0
@@ -1400,17 +1393,16 @@
         jobs_data,
         "job_1",
         ["check"],
         checks_data,
         file_list,
     )["check"]
     assert result.passed
-    assert (
-        result.messages[1]
-        == "Background subtraction performed successfully for Tree DecayTree"
+    assert result.has_all_messages(
+        "Background subtraction performed successfully for Tree DecayTree"
     )
     assert list(result.tree_data.keys())[0] == "DecayTree"
     assert not result.tree_data["DecayTree"]["histograms"] == []
 
 
 def test_range_check_bkg_subtracted_failing_range():
     rendered_yaml = dedent(
@@ -1454,17 +1446,16 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/MasterclassDatasets/D0lifetime/2014/MasterclassData.root"
         ],
     )["check"]
     assert not result.passed
-    assert (
-        result.messages[0]
-        == "Not enough events for background subtraction found in range for Tree DecayTree"
+    assert result.has_all_messages(
+        "Not enough events for background subtraction found in range for Tree DecayTree"
     )
     assert list(result.tree_data.keys())[0] == "DecayTree"
 
 
 def test_range_check_bkg_subtracted_failing_missing_branch():
     rendered_yaml = dedent(
         """\
@@ -1506,15 +1497,15 @@
         "job_1",
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/MasterclassDatasets/D0lifetime/2014/MasterclassData.root"
         ],
     )["check"]
-    message = result.messages[0]
+    message = result.messages[0][1]
     print(message)
     pattern = r"Missing branch in "
     matched = False
     if re.match(pattern, message):
         matched = True
     assert not result.passed
     assert matched
@@ -1563,15 +1554,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/MasterclassDatasets/D0lifetime/2014/MasterclassData.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == ["No TTree objects found that match RandomName"]
+    assert result.has_all_messages("No TTree objects found that match RandomName")
     assert list(result.tree_data.keys()) == []
 
 
 def test_branches_exist_passing():
     rendered_yaml = dedent(
         """\
     checks:
@@ -1603,15 +1594,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert result.passed
-    assert result.messages == ["All required branches were found in Tree DecayTree"]
+    assert result.has_all_messages("All required branches were found in Tree DecayTree")
 
 
 def test_branches_exist_failing_missing_branches():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -1643,17 +1634,17 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Required branches not found in Tree DecayTree: ['RandomName']"
-    ]
+    )
 
 
 def test_lenient_branches_exist_failing_missing_branches():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -1686,32 +1677,31 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert result.passed
-    assert result.messages == [
-        "Required branches not found in Tree DecayTree: ['RandomName']",
-        "Passed despite failure due to mode being set to Lenient.",
-    ]
+    assert result.has_all_messages(
+        "Required branches not found in Tree DecayTree: ['RandomName']"
+    )
 
 
 def test_none_branches_exist_failing_missing_branches():
     rendered_yaml = dedent(
         """\
     checks:
         check:
             type: branches_exist
             branches:
                 - H1_PZ
                 - H2_PZ
                 - RandomName
             tree_pattern: DecayTree
-            mode: None
+            mode: Ignore
 
     job_1:
         application: DaVinci/v45r8
         input:
             bk_query: /bookkeeping/path/ALLSTREAMS.DST
         output: FILETYPE.ROOT
         options:
@@ -1730,15 +1720,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert result.passed
-    assert result.messages == ["Automatically passed as the mode (None) was requested!"]
+    assert result.has_all_messages("Check ignored due to user configuration")
 
 
 def test_branches_exist_failing_tree_name():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -1769,15 +1759,15 @@
         ["check"],
         checks_data,
         [
             "root://eospublic.cern.ch//eos/opendata/lhcb/AntimatterMatters2017/data/B2HHH_MagnetDown.root"
         ],
     )["check"]
     assert not result.passed
-    assert result.messages == ["No TTree objects found that match RandomName"]
+    assert result.has_all_messages("No TTree objects found that match RandomName")
 
 
 # default checks
 
 
 def test_wrong_polarity():
     rendered_yaml = dedent(
@@ -1809,19 +1799,19 @@
         "job_MagUp",
         [],
         checks_data,
         [],
     )["job_name_matches_polarity"]
 
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Found 'magup' in job name 'job_magup' with'magdown' input "
         "('/mc/2017/beam6500gev-2018-magdown/sim09g/trig0x617d18a4/reco18/24142001/allstreams.dst'). "
         "Has the wrong magnet polarity been used?"
-    ]
+    )
 
 
 def test_wrong_polarity_acronym():
     rendered_yaml = dedent(
         """\
     job_MD:
         application: DaVinci/v45r3
@@ -1850,19 +1840,19 @@
         "job_MU",
         [],
         checks_data,
         [],
     )["job_name_matches_polarity"]
 
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "Found 'mu' in job name 'job_mu' with'magdown' input "
         "('/mc/2017/beam6500gev-2018-magdown/sim09g/trig0x617d18a4/reco18/24142001/allstreams.dst'). "
         "Has the wrong magnet polarity been used?"
-    ]
+    )
 
 
 def test_tuple_in_job_name():
     rendered_yaml = dedent(
         """\
     job_MagDown_tuple:
         application: DaVinci/v45r3
@@ -1890,25 +1880,23 @@
         jobs_data,
         "job_MagDown_tuple",
         [],
         checks_data,
         [],
     )["job_name_matches_polarity"]
     assert result.passed
-    assert result.messages == []
 
     result = checks.run_job_checks(
         jobs_data,
         "job_MagUp_tuple",
         [],
         checks_data,
         [],
     )["job_name_matches_polarity"]
     assert result.passed
-    assert result.messages == []
 
 
 def test_polarity_acronym():
     rendered_yaml = dedent(
         """\
     job_MagDown_2018:
         application: DaVinci/v45r3
@@ -1962,15 +1950,14 @@
             jobs_data,
             job_name,
             [],
             checks_data,
             [],
         )["job_name_matches_polarity"]
         assert result.passed
-        assert result.messages == []
 
 
 def test_missing_polarity():
     rendered_yaml = dedent(
         """\
     job_MagDown:
         application: DaVinci/v45r3
@@ -1988,20 +1975,20 @@
         jobs_data,
         "job_MagDown",
         [],
         checks_data,
         [],
     )["both_polarities_used"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         "/mc/2018/beam6500gev-2018-magdown/sim09g/trig0x617d18a4/reco18/24142001/allstreams.dst"
         " has been requested as input for 1 job(s)"
         " but its opposite polarity counterpart has not been requested for any jobs."
         " Are you sure you do not want the other polarity?"
-    ]
+    )
 
 
 def test_duplicate_bk_query():
     rendered_yaml = dedent(
         """\
     job_1:
         application: DaVinci/v45r3
@@ -2031,19 +2018,19 @@
             jobs_data,
             job_name,
             [],
             checks_data,
             [],
         )["duplicate_inputs"]
         assert not result.passed
-        assert result.messages == [
-            f"{job_name} shares an input "
-            "(/mc/2018/beam6500gev-2018-magdown/sim09g/trig0x617d18a4/reco18/24142001/allstreams.dst) "
+        assert result.has_all_messages(
+            f"{job_name!r} shares an input "
+            "(/MC/2018/Beam6500GeV-2018-MagDown/Sim09g/Trig0x617d18a4/Reco18/24142001/ALLSTREAMS.DST) "
             f"with the following jobs [{other_job_name!r}]"
-        ]
+        )
 
 
 def test_lenient_duplicate_bk_query():
     rendered_yaml = dedent(
         """\
     checks:
         duplicate_bk_query:
@@ -2081,30 +2068,29 @@
         result = checks.run_job_checks(
             jobs_data,
             job_name,
             ["duplicate_bk_query"],
             checks_data,
             [],
         )["duplicate_bk_query"]
-        # assert result.passed
-        assert result.messages == [
-            f"{job_name} shares an input "
-            "(/mc/2018/beam6500gev-2018-magdown/sim09g/trig0x617d18a4/reco18/24142001/allstreams.dst) "
-            f"with the following jobs [{other_job_name!r}]",
-            "Passed despite failure due to mode being set to Lenient.",
-        ]
+        assert result.passed
+        assert result.has_all_messages(
+            f"{job_name!r} shares an input "
+            "(/MC/2018/Beam6500GeV-2018-MagDown/Sim09g/Trig0x617d18a4/Reco18/24142001/ALLSTREAMS.DST) "
+            f"with the following jobs [{other_job_name!r}]"
+        )
 
 
 def test_none_duplicate_bk_query():
     rendered_yaml = dedent(
         """\
     checks:
         duplicate_bk_query:
             type: duplicate_inputs
-            mode: None
+            mode: Ignore
 
     job_1:
         application: DaVinci/v45r3
         input:
             bk_query: /MC/2018/Beam6500GeV-2018-MagDown/Sim09g/Trig0x617d18a4/Reco18/24142001/ALLSTREAMS.DST
         output: FILETYPE.ROOT
         options:
@@ -2133,17 +2119,15 @@
             jobs_data,
             job_name,
             ["duplicate_bk_query"],
             checks_data,
             [],
         )["duplicate_bk_query"]
         assert result.passed
-        assert result.messages == [
-            f"Automatically passed for {job_name} as the mode (None) was requested!"
-        ]
+        assert result.has_all_messages("Check ignored due to user configuration")
 
 
 def test_good_job_chain_polarity():
     rendered_yaml = dedent(
         """\
     job_1_MagDown:
         application: DaVinci/v45r3
@@ -2181,15 +2165,14 @@
         jobs_data,
         "job_2_MagDown",
         [],
         checks_data,
         [],
     )["job_name_matches_polarity"]
     assert result.passed
-    assert result.messages == []
 
 
 def test_bad_job_chain_polarity():
     rendered_yaml = dedent(
         """\
     job_1_MagDown:
         application: DaVinci/v45r3
@@ -2229,19 +2212,19 @@
         jobs_data,
         job_name,
         [],
         checks_data,
         [],
     )["job_name_matches_polarity"]
     assert not result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         f"Found 'magdown' in job name {job_name.lower()!r} with"
         f"'magup' input ({target.lower()!r}). "
         "Has the wrong magnet polarity been used?"
-    ]
+    )
 
 
 def test_lenient_bad_job_chain_polarity():
     rendered_yaml = dedent(
         """\
     checks:
         check:
@@ -2292,29 +2275,28 @@
         jobs_data,
         job_name,
         ["check"],
         checks_data,
         [],
     )["check"]
     assert result.passed
-    assert result.messages == [
+    assert result.has_all_messages(
         f"Found 'magdown' in job name {job_name.lower()!r} with"
         f"'magup' input ({target.lower()!r}). "
-        "Has the wrong magnet polarity been used?",
-        "Passed despite failure due to mode being set to Lenient.",
-    ]
+        "Has the wrong magnet polarity been used?"
+    )
 
 
 def test_none_bad_job_chain_polarity():
     rendered_yaml = dedent(
         """\
     checks:
         check:
             type: job_name_matches_polarity
-            mode: None
+            mode: Ignore
 
     job_1_MagDown:
         application: DaVinci/v45r3
         input:
             bk_query: /MC/2018/Beam6500GeV-2018-MagDown/Sim09g/Trig0x617d18a4/Reco18/24142001/ALLSTREAMS.DST
         output: FILETYPE.DST
         options:
@@ -2355,10 +2337,8 @@
         jobs_data,
         job_name,
         ["check"],
         checks_data,
         [],
     )["check"]
     assert result.passed
-    assert result.messages == [
-        f"Automatically passed for {job_name.lower()} as the mode (None) was requested!"
-    ]
+    assert result.has_all_messages("Check ignored due to user configuration")
```

### Comparing `LbAPCommon-0.9.3/tests/checks/test_utils.py` & `LbAPCommon-0.9.4/tests/checks/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from textwrap import dedent
 
 import hist
 import numpy as np
 import pytest
 from hist import Hist
 
-from LbAPCommon import checks_utils
+from LbAPCommon.checks import utils as checks_utils
 
 
 def test_1D_hist_serialise_then_deserialise():
     axis0 = hist.axis.Regular(10, -5.0, 5.0, name="x-axis name")
     h = Hist(axis0, name="demo hist 1D")
 
     x = np.array(
```

### Comparing `LbAPCommon-0.9.3/tests/example-logs/error-failed-to-read-file.log` & `LbAPCommon-0.9.4/tests/example-logs/error-failed-to-read-file.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/error-illegal-instruction.log` & `LbAPCommon-0.9.4/tests/example-logs/error-illegal-instruction.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/error-missing-shared-library.log` & `LbAPCommon-0.9.4/tests/example-logs/error-missing-shared-library.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/error-platform-unsupported.log` & `LbAPCommon-0.9.4/tests/example-logs/error-platform-unsupported.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/error-related-info-missing.log` & `LbAPCommon-0.9.4/tests/example-logs/error-related-info-missing.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/good-DaVinci_00110296_00000038_1.log` & `LbAPCommon-0.9.4/tests/example-logs/good-DaVinci_00110296_00000038_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/good-DaVinci_00110296_00000194_1.log` & `LbAPCommon-0.9.4/tests/example-logs/good-DaVinci_00110296_00000194_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/example-logs/good-Gauss_00104988_00000011_1.log` & `LbAPCommon-0.9.4/tests/example-logs/good-Gauss_00104988_00000011_1.log`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/linting/test_bk_paths.py` & `LbAPCommon-0.9.4/tests/linting/test_bk_paths.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/linting/test_processing_pass.py` & `LbAPCommon-0.9.4/tests/linting/test_processing_pass.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/test_good_parsing.py` & `LbAPCommon-0.9.4/tests/test_good_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1039,16 +1039,15 @@
             "wg": "Charm",
             "inform": "a.b@c.d",
         }
     }
     data["job_1"][key] = value
     rendered_yaml = yaml.safe_dump(data)
     with pytest.raises((ValueError, strictyaml.StrictYAMLError)):
-        jobs_data, checks_data = LbAPCommon.parse_yaml(rendered_yaml)
-        LbAPCommon.validate_yaml(jobs_data, checks_data, "a", "b")
+        LbAPCommon.validate_yaml(*LbAPCommon.parse_yaml(rendered_yaml), "a", "b")
 
 
 def test_completion_percentage_not_in_defaults():
     job_template = {
         "application": "DaVinci/v45r3",
         "input": {
             "bk_query": "/MC/2018/Beam6500GeV-2018-MagDown/Sim09g/Trig0x617d18a4/Reco18/24142001/ALLSTREAMS.DST"
```

### Comparing `LbAPCommon-0.9.3/tests/test_hacks.py` & `LbAPCommon-0.9.4/tests/test_hacks.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/test_log_parsing.py` & `LbAPCommon-0.9.4/tests/test_log_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/test_log_splitting.py` & `LbAPCommon-0.9.4/tests/test_log_splitting.py`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/test_performance/example1.yaml` & `LbAPCommon-0.9.4/tests/test_performance/example1.yaml`

 * *Files identical despite different names*

### Comparing `LbAPCommon-0.9.3/tests/test_performance.py` & `LbAPCommon-0.9.4/tests/test_performance.py`

 * *Files identical despite different names*

