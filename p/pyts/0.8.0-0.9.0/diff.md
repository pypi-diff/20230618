# Comparing `tmp/pyts-0.8.0.tar.gz` & `tmp/pyts-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyts-0.8.0.tar", last modified: Fri Mar 29 10:01:08 2019, max compression
+gzip compressed data, was "dist/pyts-0.9.0.tar", last modified: Mon Aug 26 09:36:27 2019, max compression
```

## Comparing `pyts-0.8.0.tar` & `pyts-0.9.0.tar`

### file list

```diff
@@ -1,99 +1,164 @@
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1524 2019-03-29 08:41:16.000000 pyts-0.8.0/LICENSE.txt
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       26 2019-03-29 08:41:16.000000 pyts-0.8.0/MANIFEST.in
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8468 2019-03-29 10:01:08.000000 pyts-0.8.0/PKG-INFO
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6523 2019-03-29 09:50:42.000000 pyts-0.8.0/README.md
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      601 2019-03-29 09:50:06.000000 pyts-0.8.0/pyts/__init__.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/approximation/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      524 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9101 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/dft.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8899 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/mcb.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5951 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/paa.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4388 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/sax.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6217 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/sfa.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/approximation/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-13 12:22:51.000000 pyts-0.8.0/pyts/approximation/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5775 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/tests/test_dft.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7598 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/tests/test_mcb.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5457 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/tests/test_paa.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3950 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/tests/test_sax.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1974 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/approximation/tests/test_sfa.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/bag_of_words/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      134 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/bag_of_words/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5035 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/bag_of_words/bow.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/bag_of_words/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/bag_of_words/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3871 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/bag_of_words/tests/test_bow.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/classification/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      229 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/classification/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    12272 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/classification/bossvs.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8108 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/classification/knn.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7015 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/classification/saxvsm.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/classification/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/classification/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7524 2019-03-29 08:41:16.000000 pyts-0.8.0/pyts/classification/tests/test_bossvs.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2080 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/classification/tests/test_knn.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3199 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/classification/tests/test_saxvsm.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/decomposition/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      162 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/decomposition/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7487 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/decomposition/ssa.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/decomposition/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/decomposition/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5315 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/decomposition/tests/test_ssa.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/image/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      292 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5960 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/gaf.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6373 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/mtf.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7893 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/recurrence.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/image/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/image/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5262 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/tests/test_gaf.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8364 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/tests/test_mtf.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6391 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/image/tests/test_recurrence.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/metrics/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      475 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/metrics/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1142 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/metrics/boss.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    35059 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/metrics/dtw.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/metrics/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/metrics/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1614 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/metrics/tests/test_boss.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    17791 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/metrics/tests/test_dtw.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/preprocessing/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      546 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5123 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/discretizer.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4172 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/imputer.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6016 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/scaler.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/preprocessing/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/preprocessing/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3861 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/tests/test_discretizer.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2284 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/tests/test_imputer.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4041 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/tests/test_scaler.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1463 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/tests/test_transformer.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5846 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/preprocessing/transformer.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/tests/__init__.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/transformation/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      161 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/transformation/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    12531 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/transformation/boss.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/transformation/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/transformation/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6119 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/transformation/tests/test_boss.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8338 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/transformation/tests/test_weasel.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    15485 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/transformation/weasel.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/utils/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      153 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/utils/__init__.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts/utils/tests/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.8.0/pyts/utils/tests/__init__.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4563 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/utils/tests/test_utils.py
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4444 2019-03-29 08:41:17.000000 pyts-0.8.0/pyts/utils/utils.py
-drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts.egg-info/
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8468 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts.egg-info/PKG-INFO
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2237 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts.egg-info/SOURCES.txt
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        1 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts.egg-info/dependency_links.txt
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        1 2019-02-04 10:28:45.000000 pyts-0.8.0/pyts.egg-info/not-zip-safe
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      153 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts.egg-info/requires.txt
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        5 2019-03-29 10:01:08.000000 pyts-0.8.0/pyts.egg-info/top_level.txt
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       62 2019-03-29 08:41:17.000000 pyts-0.8.0/requirements.txt
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      314 2019-03-29 10:01:08.000000 pyts-0.8.0/setup.cfg
--rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2199 2019-03-29 09:50:41.000000 pyts-0.8.0/setup.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1524 2019-03-29 08:41:16.000000 pyts-0.9.0/LICENSE.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       26 2019-08-06 12:23:59.000000 pyts-0.9.0/MANIFEST.in
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9623 2019-08-26 09:36:27.000000 pyts-0.9.0/PKG-INFO
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7578 2019-08-26 08:40:32.000000 pyts-0.9.0/README.md
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      621 2019-08-26 08:07:24.000000 pyts-0.9.0/pyts/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/approximation/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      524 2019-03-29 08:41:16.000000 pyts-0.9.0/pyts/approximation/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9504 2019-08-26 07:52:34.000000 pyts-0.9.0/pyts/approximation/dft.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8886 2019-08-26 07:52:36.000000 pyts-0.9.0/pyts/approximation/mcb.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6197 2019-08-26 07:52:33.000000 pyts-0.9.0/pyts/approximation/paa.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4324 2019-08-26 07:52:37.000000 pyts-0.9.0/pyts/approximation/sax.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6646 2019-08-26 07:52:41.000000 pyts-0.9.0/pyts/approximation/sfa.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/approximation/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-13 12:22:51.000000 pyts-0.9.0/pyts/approximation/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3292 2019-08-26 07:52:50.000000 pyts-0.9.0/pyts/approximation/tests/test_dft.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7449 2019-08-26 07:52:53.000000 pyts-0.9.0/pyts/approximation/tests/test_mcb.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3175 2019-08-26 07:52:57.000000 pyts-0.9.0/pyts/approximation/tests/test_paa.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2143 2019-08-26 07:53:01.000000 pyts-0.9.0/pyts/approximation/tests/test_sax.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2873 2019-08-26 07:53:07.000000 pyts-0.9.0/pyts/approximation/tests/test_sfa.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/bag_of_words/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      134 2019-03-29 08:41:16.000000 pyts-0.9.0/pyts/bag_of_words/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5406 2019-08-26 07:53:19.000000 pyts-0.9.0/pyts/bag_of_words/bow.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/bag_of_words/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 08:41:16.000000 pyts-0.9.0/pyts/bag_of_words/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2538 2019-08-26 07:53:28.000000 pyts-0.9.0/pyts/bag_of_words/tests/test_bow.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/classification/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      229 2019-03-29 08:41:16.000000 pyts-0.9.0/pyts/classification/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    12796 2019-08-26 07:53:37.000000 pyts-0.9.0/pyts/classification/bossvs.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8828 2019-08-26 07:53:41.000000 pyts-0.9.0/pyts/classification/knn.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7499 2019-08-26 07:53:45.000000 pyts-0.9.0/pyts/classification/saxvsm.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/classification/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/classification/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6281 2019-08-26 07:53:52.000000 pyts-0.9.0/pyts/classification/tests/test_bossvs.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1267 2019-08-26 07:53:55.000000 pyts-0.9.0/pyts/classification/tests/test_knn.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3492 2019-08-26 07:54:00.000000 pyts-0.9.0/pyts/classification/tests/test_saxvsm.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      694 2019-08-08 07:40:23.000000 pyts-0.9.0/pyts/datasets/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts/datasets/cached_datasets/
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/Coffee/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      645 2019-08-07 13:43:02.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/Coffee/Coffee.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)   128604 2019-08-07 13:43:02.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/Coffee/Coffee_TEST.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)   128604 2019-08-07 13:43:02.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/Coffee/Coffee_TRAIN.txt
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/GunPoint/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      710 2019-08-07 14:27:31.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/GunPoint/GunPoint.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)   362550 2019-08-07 14:27:31.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/GunPoint/GunPoint_TEST.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)   120850 2019-08-07 14:27:31.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/GunPoint/GunPoint_TRAIN.txt
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/PigCVP/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1419 2019-08-08 07:19:00.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/PigCVP/PigCVP.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)  6659744 2019-08-08 07:19:00.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/PigCVP/PigCVP_TEST.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)  3329872 2019-08-08 07:19:00.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UCR/PigCVP/PigCVP_TRAIN.txt
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UEA/
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UEA/BasicMotions/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      413 2019-08-07 12:58:36.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UEA/BasicMotions/BasicMotions.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)   230257 2019-08-07 12:58:36.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UEA/BasicMotions/BasicMotions_TEST.arff
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)   230378 2019-08-07 12:58:36.000000 pyts-0.9.0/pyts/datasets/cached_datasets/UEA/BasicMotions/BasicMotions_TRAIN.arff
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/info/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6993 2019-08-06 12:58:05.000000 pyts-0.9.0/pyts/datasets/info/ucr.pickle
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1555 2019-08-06 12:54:48.000000 pyts-0.9.0/pyts/datasets/info/uea.pickle
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    10877 2019-08-26 07:54:13.000000 pyts-0.9.0/pyts/datasets/load.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5141 2019-08-26 07:54:17.000000 pyts-0.9.0/pyts/datasets/make.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/datasets/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-05 10:39:41.000000 pyts-0.9.0/pyts/datasets/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1742 2019-08-26 07:54:54.000000 pyts-0.9.0/pyts/datasets/tests/test_load.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3216 2019-08-26 07:54:57.000000 pyts-0.9.0/pyts/datasets/tests/test_make.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3364 2019-08-26 07:55:01.000000 pyts-0.9.0/pyts/datasets/tests/test_ucr.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2696 2019-08-26 07:55:07.000000 pyts-0.9.0/pyts/datasets/tests/test_uea.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9842 2019-08-26 07:54:20.000000 pyts-0.9.0/pyts/datasets/ucr.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9582 2019-08-26 07:54:25.000000 pyts-0.9.0/pyts/datasets/uea.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/decomposition/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      162 2019-08-09 11:29:47.000000 pyts-0.9.0/pyts/decomposition/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7893 2019-08-26 07:55:22.000000 pyts-0.9.0/pyts/decomposition/ssa.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/decomposition/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/decomposition/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3679 2019-08-26 07:55:28.000000 pyts-0.9.0/pyts/decomposition/tests/test_ssa.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/image/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      292 2019-08-05 13:45:36.000000 pyts-0.9.0/pyts/image/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6228 2019-08-26 07:55:39.000000 pyts-0.9.0/pyts/image/gaf.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6651 2019-08-26 07:55:42.000000 pyts-0.9.0/pyts/image/mtf.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     8380 2019-08-26 07:55:46.000000 pyts-0.9.0/pyts/image/recurrence.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/image/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/image/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4264 2019-08-26 07:55:51.000000 pyts-0.9.0/pyts/image/tests/test_gaf.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6002 2019-08-26 07:55:55.000000 pyts-0.9.0/pyts/image/tests/test_mtf.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4945 2019-08-26 07:56:00.000000 pyts-0.9.0/pyts/image/tests/test_recurrence.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/metrics/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      475 2019-08-09 10:11:54.000000 pyts-0.9.0/pyts/metrics/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1399 2019-08-26 07:56:10.000000 pyts-0.9.0/pyts/metrics/boss.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    36671 2019-08-26 07:56:14.000000 pyts-0.9.0/pyts/metrics/dtw.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/metrics/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-03-29 08:41:17.000000 pyts-0.9.0/pyts/metrics/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1130 2019-08-26 07:56:18.000000 pyts-0.9.0/pyts/metrics/tests/test_boss.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    20574 2019-08-26 07:56:23.000000 pyts-0.9.0/pyts/metrics/tests/test_dtw.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      163 2019-08-05 13:46:36.000000 pyts-0.9.0/pyts/multivariate/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/classification/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       87 2019-08-02 13:23:45.000000 pyts-0.9.0/pyts/multivariate/classification/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5035 2019-08-26 07:56:35.000000 pyts-0.9.0/pyts/multivariate/classification/multivariate.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/classification/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-02 13:10:30.000000 pyts-0.9.0/pyts/multivariate/classification/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2894 2019-08-26 07:56:40.000000 pyts-0.9.0/pyts/multivariate/classification/tests/test_multivariate.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/image/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       77 2019-08-02 13:32:30.000000 pyts-0.9.0/pyts/multivariate/image/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5252 2019-08-26 07:56:49.000000 pyts-0.9.0/pyts/multivariate/image/joint_rp.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/image/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-02 13:10:36.000000 pyts-0.9.0/pyts/multivariate/image/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2983 2019-08-26 07:56:57.000000 pyts-0.9.0/pyts/multivariate/image/tests/test_joint_rp.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-07-31 13:33:23.000000 pyts-0.9.0/pyts/multivariate/tests/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/transformation/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      139 2019-08-02 14:23:24.000000 pyts-0.9.0/pyts/multivariate/transformation/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5802 2019-08-26 07:57:08.000000 pyts-0.9.0/pyts/multivariate/transformation/multivariate.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/transformation/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-02 13:10:41.000000 pyts-0.9.0/pyts/multivariate/transformation/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4925 2019-08-26 07:57:21.000000 pyts-0.9.0/pyts/multivariate/transformation/tests/test_multivariate.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1786 2019-08-26 07:57:25.000000 pyts-0.9.0/pyts/multivariate/transformation/tests/test_weasel_muse.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9210 2019-08-26 07:57:17.000000 pyts-0.9.0/pyts/multivariate/transformation/weasel_muse.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/utils/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       64 2019-08-05 09:06:59.000000 pyts-0.9.0/pyts/multivariate/utils/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/multivariate/utils/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-05 09:03:57.000000 pyts-0.9.0/pyts/multivariate/utils/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      642 2019-08-26 07:57:43.000000 pyts-0.9.0/pyts/multivariate/utils/tests/test_utils.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      517 2019-08-26 07:57:34.000000 pyts-0.9.0/pyts/multivariate/utils/utils.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/preprocessing/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      546 2019-03-29 08:41:17.000000 pyts-0.9.0/pyts/preprocessing/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5495 2019-08-26 07:58:00.000000 pyts-0.9.0/pyts/preprocessing/discretizer.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4540 2019-08-26 07:58:04.000000 pyts-0.9.0/pyts/preprocessing/imputer.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     7452 2019-08-26 07:58:07.000000 pyts-0.9.0/pyts/preprocessing/scaler.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/preprocessing/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/preprocessing/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     3905 2019-08-26 07:58:17.000000 pyts-0.9.0/pyts/preprocessing/tests/test_discretizer.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2082 2019-08-26 07:58:21.000000 pyts-0.9.0/pyts/preprocessing/tests/test_imputer.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2447 2019-08-26 07:58:24.000000 pyts-0.9.0/pyts/preprocessing/tests/test_scaler.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2348 2019-08-26 07:58:28.000000 pyts-0.9.0/pyts/preprocessing/tests/test_transformer.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6532 2019-08-26 07:58:11.000000 pyts-0.9.0/pyts/preprocessing/transformer.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/tests/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/transformation/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      161 2019-03-29 08:41:17.000000 pyts-0.9.0/pyts/transformation/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    13525 2019-08-26 07:58:42.000000 pyts-0.9.0/pyts/transformation/boss.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/transformation/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/transformation/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     6243 2019-08-26 07:58:51.000000 pyts-0.9.0/pyts/transformation/tests/test_boss.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5966 2019-08-26 07:58:55.000000 pyts-0.9.0/pyts/transformation/tests/test_weasel.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)    16109 2019-08-26 07:58:46.000000 pyts-0.9.0/pyts/transformation/weasel.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/utils/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      153 2019-03-29 08:41:17.000000 pyts-0.9.0/pyts/utils/__init__.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts/utils/tests/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-02-04 09:00:59.000000 pyts-0.9.0/pyts/utils/tests/__init__.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2158 2019-08-26 07:59:14.000000 pyts-0.9.0/pyts/utils/tests/test_segmentation.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     1578 2019-08-26 07:59:20.000000 pyts-0.9.0/pyts/utils/tests/test_windowed_view.py
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     5196 2019-08-26 07:59:08.000000 pyts-0.9.0/pyts/utils/utils.py
+drwxr-xr-x   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        0 2019-08-26 09:36:27.000000 pyts-0.9.0/pyts.egg-info/
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     9623 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts.egg-info/PKG-INFO
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     4234 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts.egg-info/SOURCES.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        1 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts.egg-info/dependency_links.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        1 2019-02-04 10:28:45.000000 pyts-0.9.0/pyts.egg-info/not-zip-safe
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      160 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts.egg-info/requires.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)        5 2019-08-26 09:36:26.000000 pyts-0.9.0/pyts.egg-info/top_level.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)       62 2019-07-31 14:48:17.000000 pyts-0.9.0/requirements.txt
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)      332 2019-08-26 09:36:27.000000 pyts-0.9.0/setup.cfg
+-rw-r--r--   0 johann.faouzi (20978) ICM-INSTITUTE\CRICM_ARAMIS (15860)     2552 2019-08-26 08:08:01.000000 pyts-0.9.0/setup.py
```

### Comparing `pyts-0.8.0/LICENSE.txt` & `pyts-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyts-0.8.0/PKG-INFO` & `pyts-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: pyts
-Version: 0.8.0
-Summary: A python package for time series transformation and classification
+Version: 0.9.0
+Summary: A python package for time series classification
 Home-page: https://github.com/johannfaouzi/pyts
 Maintainer: Johann Faouzi
 Maintainer-email: johann.faouzi@gmail.com
 License: new BSD
 Download-URL: https://github.com/johannfaouzi/pyts
 Description: [![Build Status](https://travis-ci.org/johannfaouzi/pyts.svg?branch=master)](https://travis-ci.org/johannfaouzi/pyts)
         [![Build Status](https://img.shields.io/appveyor/ci/johannfaouzi/pyts/master.svg)](https://ci.appveyor.com/project/johannfaouzi/pyts)
-        [![Build Status](https://circleci.com/gh/johannfaouzi/pyts/tree/master.svg?style=shield)](https://circleci.com/gh/johannfaouzi/pyts)
         [![Documentation Status](https://readthedocs.org/projects/pyts/badge/?version=latest)](https://pyts.readthedocs.io/en/latest/?badge=latest)
         [![Codecov](https://codecov.io/gh/johannfaouzi/pyts/branch/master/graph/badge.svg)](https://codecov.io/gh/johannfaouzi/pyts)
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyts.svg)](https://img.shields.io/pypi/pyversions/pyts.svg)
         [![PyPI version](https://badge.fury.io/py/pyts.svg)](https://badge.fury.io/py/pyts)
+        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/johannfaouzi/pyts.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/johannfaouzi/pyts/context:python)
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1244152.svg)](https://doi.org/10.5281/zenodo.1244152)
         
-        ## pyts: a Python package for time series transformation and classification
+        ## pyts: a Python package for time series classification
         
-        pyts is a Python package for time series transformation and classification. It
+        pyts is a Python package for time series classification. It
         aims to make time series classification easily accessible by providing
         preprocessing and utility tools, and implementations of
         state-of-the-art algorithms. Most of these algorithms transform time series,
         thus pyts provides several tools to perform these transformations.
         
         
         ### Installation
         
         #### Dependencies
         
         pyts requires:
         
         - Python (>= 3.5)
         - NumPy (>= 1.15.4)
-        - SciPy (>= 1.1.0)
+        - SciPy (>= 1.3.0)
         - Scikit-Learn (>=0.20.1)
-        - Numba (>0.41.0)
+        - Numba (>=0.41.0)
         
         To run the examples Matplotlib (>=2.0.0) is required.
         
         
         #### User installation
         
         If you already have a working installation of numpy, scipy, scikit-learn and
         numba, you can easily install pyts using ``pip``
         
             pip install pyts
         
+        or ``conda`` via the ``conda-forge`` channel
+        
+          conda install -c conda-forge pyts
+        
         You can also get the latest version of pyts by cloning the repository
         
             git clone https://github.com/johannfaouzi/pyts.git
             cd pyts
             pip install .
         
         
@@ -74,15 +78,15 @@
         [Development Guide](https://scikit-learn.org/stable/developers/). A slight
         difference is the use of Numba instead of Cython for optimization.
         
         ### Documentation
         
         The section below gives some information about the implemented algorithms in pyts.
         For more information, please have a look at the
-        [HTML documentation available via ReadTheDocs](https://pyts.readthedocs.io/en/latest/)
+        [HTML documentation available via ReadTheDocs](https://pyts.readthedocs.io/en/latest/).
         
         ### Implemented features
         
         pyts consists of the following modules:
         
         - `approximation`: This module provides implementations of algorithms that
         approximate time series. Implemented algorithms are
@@ -99,17 +103,21 @@
         
         - `classification`: This module provides implementations of algorithms that
         can classify time series. Implemented algorithms are
         [KNeighborsClassifier](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.KNeighborsClassifier.html#),
         [SAXVSM](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.SAXVSM.html#) and
         [BOSSVS](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.BOSSVS.html#).
         
+        - `datasets`: This module provides utilities to make or load toy datasets,
+        as well as fetching datasets from the
+        [UEA & UCR Time Series Classification Repository](http://www.timeseriesclassification.com).
+        
         - `decomposition`: This module provides implementations of algorithms that
-        decompose a time series into several time series. The only implemented algorithm
-        is
+        decompose a time series into several time series. The only implemented
+        algorithm is
         [Singular Spectrum Analysis](https://pyts.readthedocs.io/en/latest/generated/pyts.decomposition.SingularSpectrumAnalysis.html#).
         
         - `image`: This module provides implementations of algorithms that transform
         time series into images. Implemented algorithms are
         [Recurrence Plot](https://pyts.readthedocs.io/en/latest/generated/pyts.image.RecurrencePlot.html#),
         [Gramian Angular Field](https://pyts.readthedocs.io/en/latest/generated/pyts.image.GramianAngularField.html#) and
         [Markov Transition Field](https://pyts.readthedocs.io/en/latest/generated/pyts.image.MarkovTransitionField.html#).
@@ -117,20 +125,29 @@
         - `metrics`: This module provides implementations of metrics that are specific
         to time series. Implemented metrics are
         [Dynamic Time Warping](https://pyts.readthedocs.io/en/latest/generated/pyts.metrics.dtw.html#)
         with several variants and the
         [BOSS](https://pyts.readthedocs.io/en/latest/generated/pyts.metrics.boss.html#)
         metric.
         
+        - `multivariate`: This modules provides utilities to deal with multivariate
+        time series. Available tools are
+        [MultivariateTransformer](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.transformation.MultivariateTransformer.html) and
+        [MultivariateClassifier](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.classification.MultivariateClassifier.html)
+        to transform and classify multivariate time series using tools for univariate
+        time series respectively, as well as
+        [JointRecurrencePlot](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.image.JointRecurrencePlot.html) and
+        [WEASEL+MUSE](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.transformation.WEASELMUSE.html).
+        
         - `preprocessing`: This module provides most of the scikit-learn preprocessing
         tools but applied sample-wise (i.e. to each time series independently) instead
         of feature-wise, as well as an
         [imputer](https://pyts.readthedocs.io/en/latest/generated/pyts.preprocessing.InterpolationImputer.html#)
         of missing values using interpolation. More information is available at the
-        [pyts.preprocessing API documentation](https://pyts.readthedocs.io/en/latest/api.html#module-pyts.preprocessing)
+        [pyts.preprocessing API documentation](https://pyts.readthedocs.io/en/latest/api.html#module-pyts.preprocessing).
         
         - `transformation`: This module provides implementations of algorithms that
         transform a data set of time series with shape `(n_samples, n_timestamps)` into
         a data set with shape `(n_samples, n_features)`. Implemented algorithms are
         [BOSS](https://pyts.readthedocs.io/en/latest/generated/pyts.transformation.BOSS.html#) and
         [WEASEL](https://pyts.readthedocs.io/en/latest/generated/pyts.transformation.WEASEL.html#).
```

### Comparing `pyts-0.8.0/README.md` & `pyts-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 [![Build Status](https://travis-ci.org/johannfaouzi/pyts.svg?branch=master)](https://travis-ci.org/johannfaouzi/pyts)
 [![Build Status](https://img.shields.io/appveyor/ci/johannfaouzi/pyts/master.svg)](https://ci.appveyor.com/project/johannfaouzi/pyts)
-[![Build Status](https://circleci.com/gh/johannfaouzi/pyts/tree/master.svg?style=shield)](https://circleci.com/gh/johannfaouzi/pyts)
 [![Documentation Status](https://readthedocs.org/projects/pyts/badge/?version=latest)](https://pyts.readthedocs.io/en/latest/?badge=latest)
 [![Codecov](https://codecov.io/gh/johannfaouzi/pyts/branch/master/graph/badge.svg)](https://codecov.io/gh/johannfaouzi/pyts)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyts.svg)](https://img.shields.io/pypi/pyversions/pyts.svg)
 [![PyPI version](https://badge.fury.io/py/pyts.svg)](https://badge.fury.io/py/pyts)
+[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/johannfaouzi/pyts.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/johannfaouzi/pyts/context:python)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1244152.svg)](https://doi.org/10.5281/zenodo.1244152)
 
-## pyts: a Python package for time series transformation and classification
+## pyts: a Python package for time series classification
 
-pyts is a Python package for time series transformation and classification. It
+pyts is a Python package for time series classification. It
 aims to make time series classification easily accessible by providing
 preprocessing and utility tools, and implementations of
 state-of-the-art algorithms. Most of these algorithms transform time series,
 thus pyts provides several tools to perform these transformations.
 
 
 ### Installation
 
 #### Dependencies
 
 pyts requires:
 
 - Python (>= 3.5)
 - NumPy (>= 1.15.4)
-- SciPy (>= 1.1.0)
+- SciPy (>= 1.3.0)
 - Scikit-Learn (>=0.20.1)
-- Numba (>0.41.0)
+- Numba (>=0.41.0)
 
 To run the examples Matplotlib (>=2.0.0) is required.
 
 
 #### User installation
 
 If you already have a working installation of numpy, scipy, scikit-learn and
 numba, you can easily install pyts using ``pip``
 
     pip install pyts
 
+or ``conda`` via the ``conda-forge`` channel
+
+  conda install -c conda-forge pyts
+
 You can also get the latest version of pyts by cloning the repository
 
     git clone https://github.com/johannfaouzi/pyts.git
     cd pyts
     pip install .
 
 
@@ -65,15 +69,15 @@
 [Development Guide](https://scikit-learn.org/stable/developers/). A slight
 difference is the use of Numba instead of Cython for optimization.
 
 ### Documentation
 
 The section below gives some information about the implemented algorithms in pyts.
 For more information, please have a look at the
-[HTML documentation available via ReadTheDocs](https://pyts.readthedocs.io/en/latest/)
+[HTML documentation available via ReadTheDocs](https://pyts.readthedocs.io/en/latest/).
 
 ### Implemented features
 
 pyts consists of the following modules:
 
 - `approximation`: This module provides implementations of algorithms that
 approximate time series. Implemented algorithms are
@@ -90,17 +94,21 @@
 
 - `classification`: This module provides implementations of algorithms that
 can classify time series. Implemented algorithms are
 [KNeighborsClassifier](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.KNeighborsClassifier.html#),
 [SAXVSM](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.SAXVSM.html#) and
 [BOSSVS](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.BOSSVS.html#).
 
+- `datasets`: This module provides utilities to make or load toy datasets,
+as well as fetching datasets from the
+[UEA & UCR Time Series Classification Repository](http://www.timeseriesclassification.com).
+
 - `decomposition`: This module provides implementations of algorithms that
-decompose a time series into several time series. The only implemented algorithm
-is
+decompose a time series into several time series. The only implemented
+algorithm is
 [Singular Spectrum Analysis](https://pyts.readthedocs.io/en/latest/generated/pyts.decomposition.SingularSpectrumAnalysis.html#).
 
 - `image`: This module provides implementations of algorithms that transform
 time series into images. Implemented algorithms are
 [Recurrence Plot](https://pyts.readthedocs.io/en/latest/generated/pyts.image.RecurrencePlot.html#),
 [Gramian Angular Field](https://pyts.readthedocs.io/en/latest/generated/pyts.image.GramianAngularField.html#) and
 [Markov Transition Field](https://pyts.readthedocs.io/en/latest/generated/pyts.image.MarkovTransitionField.html#).
@@ -108,20 +116,29 @@
 - `metrics`: This module provides implementations of metrics that are specific
 to time series. Implemented metrics are
 [Dynamic Time Warping](https://pyts.readthedocs.io/en/latest/generated/pyts.metrics.dtw.html#)
 with several variants and the
 [BOSS](https://pyts.readthedocs.io/en/latest/generated/pyts.metrics.boss.html#)
 metric.
 
+- `multivariate`: This modules provides utilities to deal with multivariate
+time series. Available tools are
+[MultivariateTransformer](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.transformation.MultivariateTransformer.html) and
+[MultivariateClassifier](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.classification.MultivariateClassifier.html)
+to transform and classify multivariate time series using tools for univariate
+time series respectively, as well as
+[JointRecurrencePlot](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.image.JointRecurrencePlot.html) and
+[WEASEL+MUSE](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.transformation.WEASELMUSE.html).
+
 - `preprocessing`: This module provides most of the scikit-learn preprocessing
 tools but applied sample-wise (i.e. to each time series independently) instead
 of feature-wise, as well as an
 [imputer](https://pyts.readthedocs.io/en/latest/generated/pyts.preprocessing.InterpolationImputer.html#)
 of missing values using interpolation. More information is available at the
-[pyts.preprocessing API documentation](https://pyts.readthedocs.io/en/latest/api.html#module-pyts.preprocessing)
+[pyts.preprocessing API documentation](https://pyts.readthedocs.io/en/latest/api.html#module-pyts.preprocessing).
 
 - `transformation`: This module provides implementations of algorithms that
 transform a data set of time series with shape `(n_samples, n_timestamps)` into
 a data set with shape `(n_samples, n_features)`. Implemented algorithms are
 [BOSS](https://pyts.readthedocs.io/en/latest/generated/pyts.transformation.BOSS.html#) and
 [WEASEL](https://pyts.readthedocs.io/en/latest/generated/pyts.transformation.WEASEL.html#).
```

### Comparing `pyts-0.8.0/pyts/__init__.py` & `pyts-0.9.0/pyts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Time series transformation and classification module for Python.
 
-pyts is a Python package for time series transformation and classification.
+pyts is a Python package for time series classification.
 It aims to make time series classification easily accessible by providing
 preprocessing and utility tools, and implementations of state-of-the-art
 algorithms. Most of these algorithms transform time series, thus pyts provides
 several tools to perform these transformations.
 """
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
-__all__ = ['approximation', 'bag_of_words', 'classification', 'decomposition',
-           'image', 'metrics', 'preprocessing', 'transformation', 'utils']
+__all__ = ['approximation', 'bag_of_words', 'classification', 'datasets',
+           'decomposition', 'image', 'metrics', 'multivariate',
+           'preprocessing', 'transformation', 'utils']
```

### Comparing `pyts-0.8.0/pyts/approximation/__init__.py` & `pyts-0.9.0/pyts/approximation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyts-0.8.0/pyts/approximation/dft.py` & `pyts-0.9.0/pyts/approximation/dft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Code for Discrete Fourier Transform."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.feature_selection import f_classif
 from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 from math import ceil
 from warnings import warn
 from ..preprocessing import StandardScaler
 
 
 class DiscreteFourierTransform(BaseEstimator, TransformerMixin):
     """Discrete Fourier Transform.
 
     Parameters
     ----------
-    n_coefs : None, int or float (default = 1.)
+    n_coefs : None, int or float (default = None)
         The number of Fourier coefficients to keep. If None, all the Fourier
         coeeficients are kept. If an integer, the ``n_coefs`` most significant
         Fourier coefficients are returned if ``anova=True``, otherwise the
         first ``n_coefs`` Fourier coefficients are returned. If a float, it
         represents a percentage of the size of each time series and must be
         between 0 and 1. The number of coefficients will be computed as
         ``ceil(n_coefs * (n_timestamps - 1))`` if ``drop_sum=True`` and
@@ -36,24 +39,33 @@
         If True, center each time series before scaling.
 
     norm_std : bool (default = False)
         If True, scale each time series to unit variance.
 
     Attributes
     ----------
-    support_ : array, shape (n_coefs, )
+    support_ : array, shape = (n_coefs,)
         Indices of the kept Fourier coefficients.
 
     References
     ----------
     .. [1] P. Schäfer, and M. Högqvist, "SFA: A Symbolic Fourier Approximation
            and Index for Similarity Search in High Dimensional Datasets",
            International Conference on Extending Database Technology,
            15, 516-527 (2012).
 
+    Examples
+    --------
+    >>> from pyts.approximation import DiscreteFourierTransform
+    >>> from pyts.datasets import load_gunpoint
+    >>> X, _, _, _ = load_gunpoint(return_X_y=True)
+    >>> transformer = DiscreteFourierTransform(n_coefs=4)
+    >>> X_new = transformer.fit_transform(X)
+    >>> X_new.shape
+    (50, 4)
 
     """
 
     def __init__(self, n_coefs=None, drop_sum=False, anova=False,
                  norm_mean=False, norm_std=False):
         self.n_coefs = n_coefs
         self.drop_sum = drop_sum
```

### Comparing `pyts-0.8.0/pyts/approximation/mcb.py` & `pyts-0.9.0/pyts/approximation/mcb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Multiple Coefficient Binning."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from numba import njit, prange
 from scipy.stats import norm
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
 from sklearn.utils.multiclass import check_classification_targets
@@ -46,17 +49,16 @@
 
 class MultipleCoefficientBinning(BaseEstimator, TransformerMixin):
     """Bin continuous data into intervals column-wise.
 
     Parameters
     ----------
     n_bins : int (default = 4)
-        The number of bins to produce. The intervals for the bins are
-        determined by the minimum and maximum of the input data. It must
-        be greater than or equal to 2.
+        The number of bins to produce. It must be between 2 and
+        ``min(n_samples, 26)``.
 
     strategy : str (default = 'quantile')
         Strategy used to define the widths of the bins:
 
         - 'uniform': All bins in each sample have identical widths
         - 'quantile': All bins in each sample have the same number of points
         - 'normal': Bin edges are quantiles from a standard normal distribution
@@ -77,14 +79,28 @@
     References
     ----------
     .. [1] P. Schäfer, and M. Högqvist, "SFA: A Symbolic Fourier Approximation
            and Index for Similarity Search in High Dimensional Datasets",
            International Conference on Extending Database Technology,
            15, 516-527 (2012).
 
+    Examples
+    --------
+    >>> from pyts.approximation import MultipleCoefficientBinning
+    >>> X = [[0, 4],
+    ...      [2, 7],
+    ...      [1, 6],
+    ...      [3, 5]]
+    >>> transformer = MultipleCoefficientBinning(n_bins=2)
+    >>> print(transformer.fit_transform(X))
+    [['a' 'a']
+     ['b' 'b']
+     ['a' 'b']
+     ['b' 'a']]
+
     """
 
     def __init__(self, n_bins=4, strategy='quantile', alphabet=None):
         self.n_bins = n_bins
         self.strategy = strategy
         self.alphabet = alphabet
 
@@ -137,44 +153,35 @@
             return indices
         else:
             return self._alphabet[indices]
 
     def _check_params(self, n_samples):
         if not isinstance(self.n_bins, (int, np.integer)):
             raise TypeError("'n_bins' must be an integer.")
-        if not 2 <= self.n_bins <= n_samples:
+        if not 2 <= self.n_bins <= min(n_samples, 26):
             raise ValueError(
                 "'n_bins' must be greater than or equal to 2 and lower than "
-                "or equal to n_samples (got {0}).".format(self.n_bins)
+                "or equal to min(n_samples, 26) (got {0}).".format(self.n_bins)
             )
         if self.strategy not in ['uniform', 'quantile', 'normal', 'entropy']:
             raise ValueError("'strategy' must be either 'uniform', 'quantile',"
                              " 'normal' or 'entropy' (got {0})."
                              .format(self.strategy))
         if not ((self.alphabet is None)
                 or (self.alphabet == 'ordinal')
                 or (isinstance(self.alphabet, (list, tuple, np.ndarray)))):
             raise TypeError("'alphabet' must be None, 'ordinal' or array-like "
                             "with shape (n_bins,) (got {0})."
                             .format(self.alphabet))
         if self.alphabet is None:
-            if self.n_bins < 27:
-                alphabet = np.array(
-                    [chr(i) for i in range(97, 97 + self.n_bins)])
-            else:
-                try:
-                    alphabet = np.asarray([chr(i) for i in range(self.n_bins)])
-                except:
-                    raise ValueError("'n_bins' is unexpectedly high. You "
-                                     "should try with a smaller value.")
+            alphabet = np.array([chr(i) for i in range(97, 97 + self.n_bins)])
         elif self.alphabet == 'ordinal':
             alphabet = 'ordinal'
         else:
-            alphabet = check_array(self.alphabet, ensure_2d=False,
-                                   dtype=None)
+            alphabet = check_array(self.alphabet, ensure_2d=False, dtype=None)
             if alphabet.shape != (self.n_bins,):
                 raise ValueError("If 'alphabet' is array-like, its shape "
                                  "must be equal to (n_bins,).")
         return alphabet
 
     def _check_constant(self, X):
         if np.any(np.max(X, axis=0) - np.min(X, axis=0) == 0):
@@ -198,29 +205,29 @@
         elif strategy == 'quantile':
             bins_edges = np.percentile(
                 X, np.linspace(0, 100, self.n_bins + 1)[1:-1], axis=0
             ).T
             if np.any(np.diff(bins_edges, axis=0) == 0):
                 raise ValueError(
                     "At least two consecutive quantiles are equal. "
-                    "You should try with a smaller number of bins or "
-                    "remove features with low variation."
+                    "Consider trying with a smaller number of bins or "
+                    "removing timestamps with low variation."
                 )
         else:
             bins_edges = self._entropy_bins(X, y, n_timestamps, n_bins)
         return bins_edges
 
     def _entropy_bins(self, X, y, n_timestamps, n_bins):
         bins = np.empty((n_timestamps, n_bins - 1))
         clf = DecisionTreeClassifier(criterion='entropy',
                                      max_leaf_nodes=n_bins)
         for i in range(n_timestamps):
             clf.fit(X[:, i][:, None], y)
             threshold = clf.tree_.threshold[clf.tree_.children_left != -1]
             if threshold.size < (n_bins - 1):
                 raise ValueError(
-                    "The number of bins is too high for feature {0}. "
-                    "Try with a smaller number of bins or remove "
-                    "this feature.".format(i)
+                    "The number of bins is too high for timestamp {0}. "
+                    "Consider trying with a smaller number of bins or "
+                    "removing this timestamp.".format(i)
                 )
             bins[i] = threshold
         return np.sort(bins, axis=1)
```

### Comparing `pyts-0.8.0/pyts/approximation/paa.py` & `pyts-0.9.0/pyts/approximation/paa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Piecewise Aggregate Approximation."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from numba import njit, prange
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from ..utils import segmentation
 
@@ -18,15 +21,15 @@
 
 
 class PiecewiseAggregateApproximation(BaseEstimator, TransformerMixin):
     """Piecewise Aggregate Approximation.
 
     Parameters
     ----------
-    window_size : int, float or None (default = 1.)
+    window_size : int, float or None (default = 1)
         Length of the sliding window. If float, it represents
         a percentage of the size of each time series and must be
         between 0 and 1.
 
     output_size : int, float or None (default = None)
         Size of the returned time series. If float, it represents
         a percentage of the size of each time series and must be
@@ -43,17 +46,27 @@
     References
     ----------
     .. [1] E. Keogh, K. Chakrabarti, M. Pazzani, and S. Mehrotra,
            "Dimensionality reduction for fast similarity search in large
            time series databases". Knowledge and information Systems,
            3(3), 263-286 (2001).
 
+    Examples
+    --------
+    >>> from pyts.approximation import PiecewiseAggregateApproximation
+    >>> X = [[0, 4, 2, 1, 7, 6, 3, 5],
+    ...      [2, 5, 4, 5, 3, 4, 2, 3]]
+    >>> transformer = PiecewiseAggregateApproximation(window_size=2)
+    >>> transformer.transform(X)
+    array([[2. , 1.5, 6.5, 4. ],
+           [3.5, 4.5, 3.5, 2.5]])
+
     """
 
-    def __init__(self, window_size=1., output_size=None, overlapping=True):
+    def __init__(self, window_size=1, output_size=None, overlapping=True):
         self.window_size = window_size
         self.output_size = output_size
         self.overlapping = overlapping
 
     def fit(self, X=None, y=None):
         """Pass.
 
@@ -107,17 +120,16 @@
                               (int, np.integer, float, np.floating)):
                 raise TypeError("If specified, 'window_size' must be an "
                                 "integer or a float.")
             if isinstance(self.window_size, (int, np.integer)):
                 if not 1 <= self.window_size <= n_timestamps:
                     raise ValueError(
                         "If 'window_size' is an integer, it must be greater "
-                        "than or equal to 1 and lower than or equal to the "
-                        "size of each time series (i.e. the size of the last "
-                        "dimension of X) (got {0}).".format(self.window_size)
+                        "than or equal to 1 and lower than or equal to "
+                        "n_timestamps (got {0}).".format(self.window_size)
                     )
                 window_size = self.window_size
             else:
                 if not 0 < self.window_size <= 1:
                     raise ValueError(
                         "If 'window_size' is a float, it must be greater "
                         "than 0 and lower than or equal to 1 "
@@ -130,17 +142,16 @@
                               (int, np.integer, float, np.floating)):
                 raise TypeError("If specified, 'output_size' must be an "
                                 "integer or a float.")
             if isinstance(self.output_size, (int, np.integer)):
                 if not 1 <= self.output_size <= n_timestamps:
                     raise ValueError(
                         "If 'output_size' is an integer, it must be greater "
-                        "than or equal to 1 and lower than or equal to the "
-                        "size of each time series (i.e. the size of the last "
-                        "dimension of X) (got {0}).".format(self.output_size)
+                        "than or equal to 1 and lower than or equal to "
+                        "n_timestamps (got {0}).".format(self.output_size)
                     )
                 output_size = self.output_size
             else:
                 if not 0 < self.output_size <= 1.:
                     raise ValueError(
                         "If 'output_size' is a float, it must be greater "
                         "than 0 and lower than or equal to 1 "
```

### Comparing `pyts-0.8.0/pyts/approximation/sax.py` & `pyts-0.9.0/pyts/approximation/sax.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 """Code for Symbolic Aggregate approXimation."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from ..preprocessing import KBinsDiscretizer
 
 
 class SymbolicAggregateApproximation(BaseEstimator, TransformerMixin):
     """Symbolic Aggregate approXimation.
 
     Parameters
     ----------
     n_bins : int (default = 4)
-        The number of bins to produce. The intervals for the bins are
-        determined by the minimum and maximum of the input data. It must
-        be greater than or equal to 2.
+        The number of bins to produce. It must be between 2 and
+        ``min(n_timestamps, 26)``.
 
     strategy : 'uniform', 'quantile' or 'normal' (default = 'quantile')
         Strategy used to define the widths of the bins:
 
         - 'uniform': All bins in each sample have identical widths
         - 'quantile': All bins in each sample have the same number of points
         - 'normal': Bin edges are quantiles from a standard normal distribution
 
     alphabet : None or array-like, shape = (n_bins,)
         Alphabet to use. If None, the first `n_bins` letters of the Latin
-        alphabet are used if `n_bins` is lower than 27, otherwise the alphabet
-        will be defined to [chr(i) for i in range(n_bins)]. If 'ordinal',
-        integers are used.
+        alphabet are used. If 'ordinal', integers are used.
 
     References
     ----------
     .. [1] J. Lin, E. Keogh, L. Wei, and S. Lonardi, "Experiencing SAX: a
            novel symbolic representation of time series". Data Mining and
            Knowledge Discovery, 15(2), 107-144 (2007).
 
+    Examples
+    --------
+    >>> from pyts.approximation import SymbolicAggregateApproximation
+    >>> X = [[0, 4, 2, 1, 7, 6, 3, 5],
+    ...      [2, 5, 4, 5, 3, 4, 2, 3]]
+    >>> transformer = SymbolicAggregateApproximation()
+    >>> print(transformer.transform(X))
+    [['a' 'c' 'b' 'a' 'd' 'd' 'b' 'c']
+     ['a' 'd' 'c' 'd' 'b' 'c' 'a' 'b']]
+
     """
 
     def __init__(self, n_bins=4, strategy='quantile', alphabet=None):
         self.n_bins = n_bins
         self.strategy = strategy
         self.alphabet = alphabet
 
@@ -82,39 +92,32 @@
             return indices
         else:
             return alphabet[indices]
 
     def _check_params(self, n_timestamps):
         if not isinstance(self.n_bins, (int, np.integer)):
             raise TypeError("'n_bins' must be an integer.")
-        if not 2 <= self.n_bins <= n_timestamps:
+        if not 2 <= self.n_bins <= min(n_timestamps, 26):
             raise ValueError(
                 "'n_bins' must be greater than or equal to 2 and lower than "
-                "or equal to n_timestamps (got {0}).".format(self.n_bins)
+                "or equal to min(n_timestamps, 26) (got {0})."
+                .format(self.n_bins)
             )
         if self.strategy not in ['uniform', 'quantile', 'normal']:
             raise ValueError("'strategy' must be either 'uniform', 'quantile' "
                              "or 'normal' (got {0})".format(self.strategy))
         if not ((self.alphabet is None)
                 or (self.alphabet == 'ordinal')
                 or (isinstance(self.alphabet, (list, tuple, np.ndarray)))):
             raise TypeError("'alphabet' must be None, 'ordinal' or array-like "
                             "with shape (n_bins,) (got {0})"
                             .format(self.alphabet))
         if self.alphabet is None:
-            if self.n_bins < 27:
-                alphabet = np.array(
-                    [chr(i) for i in range(97, 97 + self.n_bins)])
-            else:
-                try:
-                    alphabet = np.asarray([chr(i) for i in range(self.n_bins)])
-                except:
-                    raise ValueError("'n_bins' is unexpectedly high. You "
-                                     "should try with a smaller value.")
+            alphabet = np.array([chr(i) for i in range(97, 97 + self.n_bins)])
         elif self.alphabet == 'ordinal':
             alphabet = 'ordinal'
         else:
-            alphabet = np.asarray(self.alphabet)
-            if alphabet.shape != (self.n_bins, ):
+            alphabet = check_array(self.alphabet, ensure_2d=False, dtype=None)
+            if alphabet.shape != (self.n_bins,):
                 raise ValueError("If 'alphabet' is array-like, its shape "
                                  "must be equal to (n_bins,).")
         return alphabet
```

### Comparing `pyts-0.8.0/pyts/approximation/sfa.py` & `pyts-0.9.0/pyts/approximation/sfa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 """Code for Symbolic Fourier Approximation."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.pipeline import Pipeline
 from sklearn.utils.validation import check_is_fitted
 from .dft import DiscreteFourierTransform
 from .mcb import MultipleCoefficientBinning
 
 
 class SymbolicFourierApproximation(BaseEstimator, TransformerMixin):
     """Symbolic Fourier Approximation.
 
     Parameters
     ----------
-    n_coefs : None, int or float (default = 1.)
+    n_coefs : None, int or float (default = None)
         The number of Fourier coefficients to keep. If None, all the Fourier
         coeeficients are kept. If an integer, the ``n_coefs`` most significant
         Fourier coefficients are returned if ``anova=True``, otherwise the
         first ``n_coefs`` Fourier coefficients are returned. If a float, it
         represents a percentage of the size of each time series and must be
         between 0 and 1. The number of coefficients will be computed as
         ``ceil(n_coefs * (n_timestamps - 1))`` if ``drop_sum=True`` and
         ``ceil(n_coefs * n_timestamps)`` if ``drop_sum=False``.
 
+    n_bins : int (default = 4)
+        The number of bins to produce. The intervals for the bins are
+        determined by the minimum and maximum of the input data. It must
+        be between 2 and 26.
+
+    strategy : str (default = 'quantile')
+        Strategy used to define the widths of the bins:
+
+        - 'uniform': All bins in each sample have identical widths
+        - 'quantile': All bins in each sample have the same number of points
+        - 'normal': Bin edges are quantiles from a standard normal distribution
+        - 'entropy': Bin edges are computed using information gain
+
     drop_sum : bool (default = False)
         If True, the first Fourier coefficient (i.e. the sum of the time
         series) is dropped. If False, the real part of the first Fourier
         coefficient is kept.
 
     anova : bool (default = False)
         If True, the Fourier coefficient selection is done via a one-way
@@ -34,54 +50,51 @@
     norm_mean : bool (default = False)
         If True, center the data before scaling. If ``norm_mean=True`` and
         ``anova=False``, the first Fourier coefficient will be dropped.
 
     norm_std : bool (default = False)
         If True, scale the data to unit variance.
 
-    n_bins : int (default = 5)
-        The number of bins to produce. The intervals for the bins are
-        determined by the minimum and maximum of the input data. It must
-        be between 2 and 26.
-
-    strategy : str (default = 'quantile')
-        Strategy used to define the widths of the bins:
-
-        - 'uniform': All bins in each sample have identical widths
-        - 'quantile': All bins in each sample have the same number of points
-        - 'normal': Bin edges are quantiles from a standard normal distribution
-        - 'entropy': Bin edges are computed using information gain
-
     alphabet : None, 'ordinal' or array-like, shape = (n_bins,)
         Alphabet to use. If None, the first `n_bins` letters of the Latin
         alphabet are used if `n_bins` is lower than 27, otherwise the alphabet
         will be defined to [chr(i) for i in range(n_bins)]. If 'ordinal',
         integers are used.
 
     Attributes
     ----------
-    support_ : array, shape (n_coefs, )
-        Indices of the kept Fourier coefficients.
-
     bin_edges_ : array, shape = (n_bins - 1,) or (n_timestamps, n_bins - 1)
         Bin edges with shape = (n_bins - 1,) if ``strategy='normal'`` or
         (n_timestamps, n_bins - 1) otherwise.
 
+    support_ : array, shape = (n_coefs,)
+        Indices of the kept Fourier coefficients.
+
     References
     ----------
     .. [1] P. Schäfer, and M. Högqvist, "SFA: A Symbolic Fourier Approximation
            and Index for Similarity Search in High Dimensional Datasets",
            International Conference on Extending Database Technology,
            15, 516-527 (2012).
 
+    Examples
+    --------
+    >>> from pyts.approximation import SymbolicFourierApproximation
+    >>> from pyts.datasets import load_gunpoint
+    >>> X, _, _, _ = load_gunpoint(return_X_y=True)
+    >>> transformer = SymbolicFourierApproximation(n_coefs=4)
+    >>> X_new = transformer.fit_transform(X)
+    >>> X_new.shape
+    (50, 4)
+
     """
 
-    def __init__(self, n_coefs=None, drop_sum=False, anova=False,
-                 norm_mean=False, norm_std=False, n_bins=4,
-                 strategy='quantile', alphabet=None):
+    def __init__(self, n_coefs=None, n_bins=4, strategy='quantile',
+                 drop_sum=False, anova=False, norm_mean=False, norm_std=False,
+                 alphabet=None):
         self.n_coefs = n_coefs
         self.drop_sum = drop_sum
         self.anova = anova
         self.norm_mean = norm_mean
         self.norm_std = norm_std
         self.n_bins = n_bins
         self.strategy = strategy
@@ -91,15 +104,15 @@
         """Select Fourier coefficients and compute bin edges for each feature.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
             Data to transform.
 
-        y : None or array-like, shape = (n_samples,)
+        y : None or array-like, shape = (n_samples,) (default = None)
             Class labels for each sample. Only used if ``anova=True`` or
             ``strategy='entropy'.``
 
         """
         dft = DiscreteFourierTransform(
             n_coefs=self.n_coefs, drop_sum=self.drop_sum, anova=self.anova,
             norm_mean=self.norm_mean, norm_std=self.norm_std
```

### Comparing `pyts-0.8.0/pyts/bag_of_words/bow.py` & `pyts-0.9.0/pyts/bag_of_words/bow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,51 @@
 """Code for Bag-of-Words."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from ..utils import windowed_view
 
 
 class BagOfWords(BaseEstimator, TransformerMixin):
-    """Transform time series into bag of words.
+    r"""Transform time series into bag of words.
 
     Parameters
     ----------
     window_size : int or float (default = 0.1)
         Size of the sliding window (i.e. the size of each word). If float, it
         represents the percentage of the size of each time series and must be
         between 0 and 1. The window size will be computed as
         ``ceil(window_size * n_timestamps)``.
 
     window_step : int or float (default = 1)
-        Step of the sliding window. If float, it
-        represents the percentage of the size of each time series and must be
-        between 0 and 1. The window size will be computed as
-        ``ceil(window_step * n_timestamps)``.
+        Step of the sliding window. If float, it represents the percentage of
+        the size of each time series and must be between 0 and 1. The window
+        size will be computed as ``ceil(window_step * n_timestamps)``.
 
     numerosity_reduction : bool (default = True)
         If True, delete sample-wise all but one occurence of back to back
         identical occurences of the same words.
 
+    Examples
+    --------
+    >>> from pyts.bag_of_words import BagOfWords
+    >>> X = [['a', 'a', 'b', 'a', 'b', 'b', 'b', 'b', 'a'],
+    ...      ['a', 'b', 'c', 'c', 'c', 'c', 'a', 'a', 'c']]
+    >>> bow = BagOfWords(window_size=2)
+    >>> print(bow.transform(X))
+    ['aa ab ba ab bb ba' 'ab bc cc ca aa ac']
+    >>> bow = BagOfWords(window_size=2, numerosity_reduction=False)
+    >>> print(bow.transform(X))
+    ['aa ab ba ab bb bb bb ba' 'ab bc cc cc cc ca aa ac']
+
     """
 
     def __init__(self, window_size=0.1, window_step=1,
                  numerosity_reduction=True):
         self.window_size = window_size
         self.window_step = window_step
         self.numerosity_reduction = numerosity_reduction
@@ -59,15 +73,15 @@
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
 
         Returns
         -------
-        X_new : array, shape = (n_samples, )
+        X_new : array, shape = (n_samples,)
             Transformed data. Each row is a string consisting of words
             separated by a whitespace.
 
         """
         X = check_array(X, dtype=None)
         n_samples, n_timestamps = X.shape
         window_size, window_step = self._check_params(n_timestamps)
@@ -91,41 +105,39 @@
         if not isinstance(self.window_size,
                           (int, np.integer, float, np.floating)):
             raise TypeError("'window_size' must be an integer or a float.")
         if isinstance(self.window_size, (int, np.integer)):
             if not 1 <= self.window_size <= n_timestamps:
                 raise ValueError(
                     "If 'window_size' is an integer, it must be greater "
-                    "than or equal to 1 and lower than or equal to the "
-                    "size of each time series (i.e. the size of the last "
-                    "dimension of X) (got {0}).".format(self.window_size)
+                    "than or equal to 1 and lower than or equal to "
+                    "n_timestamps (got {0}).".format(self.window_size)
                 )
             window_size = self.window_size
         else:
             if not 0 < self.window_size <= 1:
                 raise ValueError(
                     "If 'window_size' is a float, it must be greater "
-                    "than 0 and lower than or equal to 1 "
-                    "(got {0}).".format(self.window_size)
+                    "than 0 and lower than or equal to 1 (got {0})."
+                    .format(self.window_size)
                 )
             window_size = ceil(self.window_size * n_timestamps)
         if not isinstance(self.window_step,
                           (int, np.integer, float, np.floating)):
             raise TypeError("'window_step' must be an integer or a float.")
         if isinstance(self.window_step, (int, np.integer)):
             if not 1 <= self.window_step <= n_timestamps:
                 raise ValueError(
                     "If 'window_step' is an integer, it must be greater "
-                    "than or equal to 1 and lower than or equal to the "
-                    "size of each time series (i.e. the size of the last "
-                    "dimension of X) (got {0}).".format(self.window_step)
+                    "than or equal to 1 and lower than or equal to "
+                    "n_timestamps (got {0}).".format(self.window_step)
                 )
             window_step = self.window_step
         else:
             if not 0 < self.window_step <= 1:
                 raise ValueError(
                     "If 'window_step' is a float, it must be greater "
-                    "than 0 and lower than or equal to 1 "
-                    "(got {0}).".format(self.window_step)
+                    "than 0 and lower than or equal to 1 (got {0})."
+                    .format(self.window_step)
                 )
             window_step = ceil(self.window_step * n_timestamps)
         return window_size, window_step
```

### Comparing `pyts-0.8.0/pyts/classification/bossvs.py` & `pyts-0.9.0/pyts/classification/bossvs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Bag-of-SFA Symbols in Vector Space."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from sklearn.utils.validation import check_array, check_X_y, check_is_fitted
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.metrics.pairwise import cosine_similarity
 from sklearn.preprocessing import LabelEncoder
@@ -78,29 +81,43 @@
         exactly once. Prevents zero divisions.
 
     sublinear_tf : bool (default = True)
         Apply sublinear tf scaling, i.e. replace tf with 1 + log(tf).
 
     Attributes
     ----------
-    vocabulary_ : dict
-        A mapping of feature indices to terms.
-
-    tfidf_ : array, shape = (n_classes, n_words)
-        Term-document matrix.
+    classes_ : array, shape = (n_classes,)
+        An array of class labels known to the classifier.
 
     idf_ : array, shape = (n_features,) , or None
         The learned idf vector (global term weights) when ``use_idf=True``,
         None otherwise.
 
+    tfidf_ : array, shape = (n_classes, n_words)
+        Term-document matrix.
+
+    vocabulary_ : dict
+        A mapping of feature indices to terms.
+
     References
     ----------
     .. [1] P. Schäfer, "Scalable Time Series Classification". Data Mining and
            Knowledge Discovery, 30(5), 1273-1298 (2016).
 
+    Examples
+    --------
+    >>> from pyts.classification import BOSSVS
+    >>> from pyts.datasets import load_gunpoint
+    >>> X_train, X_test, y_train, y_test = load_gunpoint(return_X_y=True)
+    >>> clf = BOSSVS(window_size=28)
+    >>> clf.fit(X_train, y_train) # doctest: +ELLIPSIS
+    BOSSVS(...)
+    >>> clf.score(X_test, y_test)
+    0.98
+
     """
 
     def __init__(self, word_size=4, n_bins=4, window_size=10, window_step=1,
                  anova=False, drop_sum=False, norm_mean=False, norm_std=False,
                  strategy='quantile', alphabet=None, numerosity_reduction=True,
                  use_idf=True, smooth_idf=False, sublinear_tf=True):
         self.word_size = word_size
```

### Comparing `pyts-0.8.0/pyts/classification/knn.py` & `pyts-0.9.0/pyts/classification/knn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """Code for k-nearest-neighbors."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.neighbors import KNeighborsClassifier as SklearnKNN
+from sklearn.preprocessing import LabelEncoder
 from sklearn.utils.validation import check_X_y, check_is_fitted
 from ..metrics import (boss, dtw, dtw_classic, dtw_region, dtw_fast,
                        dtw_multiscale, sakoe_chiba_band, itakura_parallelogram)
 
 
 class KNeighborsClassifier(BaseEstimator, ClassifierMixin):
     """k nearest neighbors classifier.
@@ -38,15 +42,15 @@
     leaf_size : int, optional (default = 30)
         Leaf size passed to BallTree or KDTree.  This can affect the
         speed of the construction and query, as well as the memory
         required to store the tree.  The optimal value depends on the
         nature of the problem.
 
     metric : string or DistanceMetric object (default = 'minkowski')
-        the distance metric to use for the tree.  The default metric is
+        The distance metric to use for the tree.  The default metric is
         minkowski, and with p=2 is equivalent to the standard Euclidean
         metric. See the documentation of the DistanceMetric class from
         scikit-learn for a list of available metrics. For Dynamic Time
         Warping, the available metrics are 'dtw', 'dtw_sakoechiba',
         'dtw_itakura', 'dtw_multiscale', 'dtw_fast' and 'boss'.
 
     p : integer, optional (default = 2)
@@ -58,14 +62,30 @@
         Additional keyword arguments for the metric function.
 
     n_jobs : int, optional (default = 1)
         The number of parallel jobs to run for neighbors search.
         If ``n_jobs=-1``, then the number of jobs is set to the number of CPU
         cores. Doesn't affect :meth:`fit` method.
 
+    Attributes
+    ----------
+    classes_ : array, shape = (n_classes,)
+        An array of class labels known to the classifier.
+
+    Examples
+    --------
+    >>> from pyts.classification import KNeighborsClassifier
+    >>> from pyts.datasets import load_gunpoint
+    >>> X_train, X_test, y_train, y_test = load_gunpoint(return_X_y=True)
+    >>> clf = KNeighborsClassifier()
+    >>> clf.fit(X_train, y_train) # doctest: +ELLIPSIS
+    KNeighborsClassifier(...)
+    >>> clf.score(X_test, y_test)
+    0.91...
+
     """
 
     def __init__(self, n_neighbors=1, weights='uniform', algorithm='auto',
                  leaf_size=30, p=2, metric='minkowski', metric_params=None,
                  n_jobs=1, **kwargs):
         self.n_neighbors = n_neighbors
         self.weights = weights
@@ -90,14 +110,16 @@
 
         Returns
         -------
         self : object
 
         """
         X, y = check_X_y(X, y)
+        self._le = LabelEncoder().fit(y)
+        self.classes_ = self._le.classes_
 
         if self.metric == 'dtw':
             self._clf = SklearnKNN(
                 n_neighbors=self.n_neighbors, weights=self.weights,
                 algorithm='brute', metric=dtw,
                 metric_params=self.metric_params,
                 n_jobs=self.n_jobs, **self.kwargs
@@ -203,13 +225,13 @@
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
             Test samples.
 
         Returns
         -------
-        y : array-like, shape = (n_samples,)
+        y_pred : array-like, shape = (n_samples,)
             Class labels for each data sample.
 
         """
         check_is_fitted(self, '_clf')
         return self._clf.predict(X)
```

### Comparing `pyts-0.8.0/pyts/classification/saxvsm.py` & `pyts-0.9.0/pyts/classification/saxvsm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for SAX-VSM."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from sklearn.utils.validation import check_X_y, check_is_fitted
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.metrics.pairwise import cosine_similarity
 from sklearn.preprocessing import LabelEncoder
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
@@ -19,29 +22,24 @@
     model. Then the classes are transformed into a Vector Space Model
     (VSM) using term frequencies (tf) and inverse document frequencies
     (idf).
 
     Parameters
     ----------
     n_bins : int (default = 4)
-        The number of bins to produce. The intervals for the bins are
-        determined by the minimum and maximum of the input data. It must
-        be between 2 and 26.
+        The number of bins to produce. It must be between 2 and
+        ``min(n_timestamps, 26)``.
 
     strategy : 'uniform', 'quantile' or 'normal' (default = 'quantile')
         Strategy used to define the widths of the bins:
 
         - 'uniform': All bins in each sample have identical widths
         - 'quantile': All bins in each sample have the same number of points
         - 'normal': Bin edges are quantiles from a standard normal distribution
 
-    alphabet : None or array-like, shape = (n_bins,)
-        Alphabet to use. If None, the first `n_bins` letters of the Latin
-        alphabet are used.
-
     window_size : int or float (default = 4)
         Size of the sliding window (i.e. the size of each word). If float, it
         represents the percentage of the size of each time series and must be
         between 0 and 1. The window size will be computed as
         ``ceil(window_size * n_timestamps)``.
 
     window_step : int or float (default = 1)
@@ -60,46 +58,64 @@
         Smooth idf weights by adding one to document frequencies, as if an
         extra document was seen containing every term in the collection
         exactly once. Prevents zero divisions.
 
     sublinear_tf : bool (default = True)
         Apply sublinear tf scaling, i.e. replace tf with 1 + log(tf).
 
+    alphabet : None or array-like, shape = (n_bins,)
+        Alphabet to use. If None, the first `n_bins` letters of the Latin
+        alphabet are used.
+
     Attributes
     ----------
-    vocabulary_ : dict
-        A mapping of feature indices to terms.
-
-    tfidf_ : array, shape = (n_classes, n_words)
-        Term-document matrix.
+    classes_ : array, shape = (n_classes,)
+        An array of class labels known to the classifier.
 
     idf_ : array, shape = (n_features,) , or None
         The learned idf vector (global term weights) when ``use_idf=True``,
         None otherwise.
 
+    tfidf_ : array, shape = (n_classes, n_words)
+        Term-document matrix.
+
+    vocabulary_ : dict
+        A mapping of feature indices to terms.
+
     References
     ----------
     .. [1] P. Senin, and S. Malinchik, "SAX-VSM: Interpretable Time Series
            Classification Using SAX and Vector Space Model". International
            Conference on Data Mining, 13, 1175-1180 (2013).
 
+    Examples
+    --------
+    >>> from pyts.classification import SAXVSM
+    >>> from pyts.datasets import load_gunpoint
+    >>> X_train, X_test, y_train, y_test = load_gunpoint(return_X_y=True)
+    >>> clf = SAXVSM(window_size=34, sublinear_tf=False, use_idf=False)
+    >>> clf.fit(X_train, y_train) # doctest: +ELLIPSIS
+    SAXVSM(...)
+    >>> clf.score(X_test, y_test)
+    0.76
+
     """
 
-    def __init__(self, n_bins=4, strategy='quantile', alphabet=None,
-                 window_size=4, window_step=1, numerosity_reduction=True,
-                 use_idf=True, smooth_idf=False, sublinear_tf=True):
+    def __init__(self, n_bins=4, strategy='quantile', window_size=4,
+                 window_step=1, numerosity_reduction=True, use_idf=True,
+                 smooth_idf=False, sublinear_tf=True, alphabet=None):
         self.n_bins = n_bins
         self.strategy = strategy
-        self.alphabet = alphabet
         self.window_size = window_size
         self.window_step = window_step
         self.numerosity_reduction = numerosity_reduction
         self.use_idf = use_idf
         self.smooth_idf = smooth_idf
         self.sublinear_tf = sublinear_tf
+        self.alphabet = alphabet
 
     def fit(self, X, y):
         """Fit the model according to the given training data.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
@@ -149,15 +165,15 @@
 
     def decision_function(self, X):
         """Evaluate the cosine similarity between document-term matrix and X.
 
         Parameters
         ----------
         X : array-like, shape (n_samples, n_timestamps)
-            Testing vector.
+            Test samples.
 
         Returns
         -------
         X : array-like, shape (n_samples, n_classes)
             osine similarity between the document-term matrix and X.
 
         """
```

### Comparing `pyts-0.8.0/pyts/classification/tests/test_saxvsm.py` & `pyts-0.9.0/pyts/classification/tests/test_saxvsm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,93 @@
 """Testing for SAX-VSM."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 import pytest
+import re
 from math import log
 from sklearn.metrics.pairwise import cosine_similarity
-from ..saxvsm import SAXVSM
-
+from pyts.classification import SAXVSM
 
-def test_SAXVSM():
-    """Test 'SAXVSM' class."""
-    # Parameter check
-    msg_error = "'n_bins' must be an integer."
-    with pytest.raises(TypeError, match=msg_error):
-        clf = SAXVSM(n_bins="3", strategy='uniform', window_size=2,
-                     numerosity_reduction=False, sublinear_tf=False)
-        clf.fit(np.c_[np.ones((4, 5)), np.zeros((4, 6))], [0, 0, 1, 1])
-
-    msg_error = "'n_bins' must be between 2 and 26."
-    with pytest.raises(ValueError, match=msg_error):
-        clf = SAXVSM(n_bins=30, strategy='uniform', window_size=2,
-                     numerosity_reduction=False, sublinear_tf=False)
-        clf.fit(np.c_[np.ones((4, 5)), np.zeros((4, 6))], [0, 0, 1, 1])
 
-    # Test 1
+X = [[0, 0, 0, 1, 0, 0, 1, 1, 1],
+     [0, 1, 1, 1, 0, 0, 1, 1, 1],
+     [0, 0, 0, 1, 0, 0, 0, 1, 0]]
+y = [0, 0, 1]
+
+
+@pytest.mark.parametrize(
+    'params, error, err_msg',
+    [({'n_bins': '3'}, TypeError, "'n_bins' must be an integer."),
+     ({'n_bins': 1}, ValueError, "'n_bins' must be between 2 and 26.")]
+)
+def test_parameter_check(params, error, err_msg):
+    """Test parameter validation."""
+    clf = SAXVSM(**params)
+    with pytest.raises(error, match=re.escape(err_msg)):
+        clf.fit(X, y)
+
+
+def test_actual_results_strategy_uniform():
+    """Test that the actual results are the expected ones."""
+    # Data
     X = [[0, 0, 0, 1, 0, 0, 1, 1, 1],
          [0, 1, 1, 1, 0, 0, 1, 1, 1],
          [0, 0, 0, 1, 0, 0, 0, 1, 0]]
     y = [0, 0, 1]
 
     clf = SAXVSM(n_bins=2, strategy='uniform', window_size=2,
                  numerosity_reduction=False, sublinear_tf=False)
-    arr_actual = clf.fit(X, y).decision_function(X)
+    decision_function_actual = clf.fit(X, y).decision_function(X)
 
     # X_sax = np.array(['a', 'b'])[np.asarray(X)]
     # X_bow = ["aa aa ab ba aa ab bb bb",
     #          "ab bb bb ba aa ab bb bb",
     #          "aa aa ab ba aa aa ab ba"]
     freq = np.asarray([[3, 2, 1, 2],
                        [1, 2, 1, 4],
                        [4, 2, 2, 0]])
     tf = np.asarray([[4, 4, 2, 6],
                      [4, 2, 2, 0]])
     idf = np.asarray([1, 1, 1, log(2) + 1])
-    arr_desired = cosine_similarity(freq, tf * idf[None, :])
-    np.testing.assert_allclose(arr_actual, arr_desired, atol=1e-5, rtol=0.)
+    decision_function_desired = cosine_similarity(freq, tf * idf[None, :])
+    np.testing.assert_allclose(decision_function_actual,
+                               decision_function_desired, atol=1e-5, rtol=0.)
+
+    pred_actual = clf.predict(X)
+    pred_desired = cosine_similarity(freq, tf * idf[None, :]).argmax(axis=1)
+    np.testing.assert_array_equal(pred_actual, pred_desired)
 
-    arr_actual = clf.fit(X, y).predict(X)
-    arr_desired = cosine_similarity(freq, tf * idf[None, :]).argmax(axis=1)
-    np.testing.assert_array_equal(arr_actual, arr_desired)
 
-    # Test 2
+def test_actual_results_strategy_quantile():
+    """Test that the actual results are the expected ones."""
+    # Data
     X = [[0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9],
          [0.0, 0.3, 0.2, 0.4, 0.1, 0.5, 0.6, 0.7, 0.8, 0.9],
          [0.0, 0.9, 0.1, 0.8, 0.2, 0.7, 0.3, 0.6, 0.4, 0.5]]
     y = [0, 0, 1]
+
     clf = SAXVSM(n_bins=2, strategy='quantile', window_size=2,
                  numerosity_reduction=False, sublinear_tf=False)
-    arr_actual = clf.fit(X, y).decision_function(X)
+    decision_function_actual = clf.fit(X, y).decision_function(X)
 
     # X_sax = [['a', 'a', 'a', 'a', 'a', 'b', 'b', 'b', 'b', 'b'],
     #          ['a', 'a', 'a', 'a', 'a', 'b', 'b', 'b', 'b', 'b'],
     #          ['a', 'b', 'a', 'b', 'a', 'b', 'a', 'b', 'a', 'b']]
     # X_bow = ["aa aa aa aa ab bb bb bb bb",
     #          "aa aa aa aa ab bb bb bb bb",
     #          "ab ba ab ba ab ba ab ba ab"]
     freq = np.asarray([[4, 1, 0, 4],
                        [4, 1, 0, 4],
                        [0, 5, 4, 0]])
     tf = np.asarray([[8, 2, 0, 8],
                      [0, 5, 4, 0]])
     idf = np.asarray([log(2) + 1, 1, log(2) + 1, log(2) + 1])
-    arr_desired = cosine_similarity(freq, tf * idf[None, :])
-    np.testing.assert_allclose(arr_actual, arr_desired, atol=1e-5, rtol=0.)
-
-    arr_actual = clf.fit(X, y).predict(X)
-    arr_desired = cosine_similarity(freq, tf * idf[None, :]).argmax(axis=1)
-    np.testing.assert_array_equal(arr_actual, arr_desired)
+    decision_function_desired = cosine_similarity(freq, tf * idf[None, :])
+    np.testing.assert_allclose(decision_function_actual,
+                               decision_function_desired, atol=1e-5, rtol=0.)
+
+    pred_actual = clf.fit(X, y).predict(X)
+    pred_desired = cosine_similarity(freq, tf * idf[None, :]).argmax(axis=1)
+    np.testing.assert_array_equal(pred_actual, pred_desired)
```

### Comparing `pyts-0.8.0/pyts/decomposition/ssa.py` & `pyts-0.9.0/pyts/decomposition/ssa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Singular Spectrum Analysis."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from numba import njit, prange
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from ..utils import windowed_view
 
@@ -53,14 +56,24 @@
         for each group.
 
     References
     ----------
     .. [1] N. Golyandina, and A. Zhigljavsky, "Singular Spectrum Analysis for
            Time Series". Springer-Verlag Berlin Heidelberg (2013).
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.decomposition import SingularSpectrumAnalysis
+    >>> X, _, _, _ = load_gunpoint(return_X_y=True)
+    >>> transformer = SingularSpectrumAnalysis(window_size=5)
+    >>> X_new = transformer.transform(X)
+    >>> X_new.shape
+    (50, 5, 150)
+
     """
 
     def __init__(self, window_size=4, groups=None):
         self.window_size = window_size
         self.groups = groups
 
     def fit(self, X=None, y=None):
```

### Comparing `pyts-0.8.0/pyts/image/gaf.py` & `pyts-0.9.0/pyts/image/gaf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Gramian Angular Field."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from numba import njit, prange
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from ..approximation import PiecewiseAggregateApproximation
 from ..preprocessing import MinMaxScaler
@@ -51,14 +54,24 @@
 
     References
     ----------
     .. [1] Z. Wang and T. Oates, "Encoding Time Series as Images for Visual
            Inspection and Classification Using Tiled Convolutional Neural
            Networks." AAAI Workshop (2015).
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.image import GramianAngularField
+    >>> X, _, _, _ = load_gunpoint(return_X_y=True)
+    >>> transformer = GramianAngularField()
+    >>> X_new = transformer.transform(X)
+    >>> X_new.shape
+    (50, 150, 150)
+
     """
 
     def __init__(self, image_size=1., sample_range=(-1, 1),
                  method='summation', overlapping=False):
         self.image_size = image_size
         self.sample_range = sample_range
         self.method = method
@@ -122,25 +135,24 @@
         if not isinstance(self.image_size,
                           (int, np.integer, float, np.floating)):
             raise TypeError("'image_size' must be an integer or a float.")
         if isinstance(self.image_size, (int, np.integer)):
             if self.image_size < 1 or self.image_size > n_timestamps:
                 raise ValueError(
                     "If 'image_size' is an integer, it must be greater "
-                    "than or equal to 1 and lower than or equal to the size "
-                    "of each time series (i.e. the size of the last dimension "
-                    "of X) (got {0}).".format(self.image_size)
+                    "than or equal to 1 and lower than or equal to "
+                    "n_timestamps (got {0}).".format(self.image_size)
                 )
             image_size = self.image_size
         else:
-            if self.image_size < 0. or self.image_size > 1.:
+            if not (0 < self.image_size <= 1.):
                 raise ValueError(
                     "If 'image_size' is a float, it must be greater "
-                    "than or equal to 0 and lower than or equal to 1 "
-                    "(got {0}).".format(self.image_size)
+                    "than 0 and lower than or equal to 1 (got {0})."
+                    .format(self.image_size)
                 )
             image_size = ceil(self.image_size * n_timestamps)
         if not ((self.sample_range is None)
                 or (isinstance(self.sample_range, tuple))):
             raise TypeError("'sample_range' must be None or a tuple.")
         if isinstance(self.sample_range, tuple):
             if len(self.sample_range) != 2:
```

### Comparing `pyts-0.8.0/pyts/image/mtf.py` & `pyts-0.9.0/pyts/image/mtf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Markov Transition Field."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from numba import njit, prange
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from ..preprocessing import KBinsDiscretizer
 from ..utils import segmentation
@@ -71,14 +74,24 @@
 
     References
     ----------
     .. [1] Z. Wang and T. Oates, "Encoding Time Series as Images for Visual
            Inspection and Classification Using Tiled Convolutional Neural
            Networks." AAAI Workshop (2015).
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.image import MarkovTransitionField
+    >>> X, _, _, _ = load_gunpoint(return_X_y=True)
+    >>> transformer = MarkovTransitionField()
+    >>> X_new = transformer.transform(X)
+    >>> X_new.shape
+    (50, 150, 150)
+
     """
 
     def __init__(self, image_size=1., n_bins=8,
                  strategy='quantile', overlapping=False):
         self.image_size = image_size
         self.n_bins = n_bins
         self.strategy = strategy
@@ -123,15 +136,15 @@
                                        strategy=self.strategy)
         X_binned = discretizer.fit_transform(X)
 
         X_mtm = _markov_transition_matrix(X_binned, n_samples,
                                           n_timestamps, self.n_bins)
         sum_mtm = X_mtm.sum(axis=2)
         np.place(sum_mtm, sum_mtm == 0, 1)
-        X_mtm = X_mtm / sum_mtm[:, :, None]
+        X_mtm /= sum_mtm[:, :, None]
 
         X_mtf = _markov_transition_field(
             X_binned, X_mtm, n_samples, n_timestamps, self.n_bins
         )
 
         window_size, remainder = divmod(n_timestamps, image_size)
         if remainder == 0:
@@ -153,25 +166,24 @@
         if not isinstance(self.image_size,
                           (int, np.integer, float, np.floating)):
             raise TypeError("'image_size' must be an integer or a float.")
         if isinstance(self.image_size, (int, np.integer)):
             if self.image_size < 1 or self.image_size > n_timestamps:
                 raise ValueError(
                     "If 'image_size' is an integer, it must be greater "
-                    "than or equal to 1 and lower than or equal to the size "
-                    "of each time series (i.e. the size of the last dimension "
-                    "of X) (got {0}).".format(self.image_size)
+                    "than or equal to 1 and lower than or equal to "
+                    "n_timestamps (got {0}).".format(self.image_size)
                 )
             image_size = self.image_size
         else:
             if self.image_size < 0. or self.image_size > 1.:
                 raise ValueError(
                     "If 'image_size' is a float, it must be greater "
-                    "than or equal to 0 and lower than or equal to 1 "
-                    "(got {0}).".format(self.image_size)
+                    "than 0 and lower than or equal to 1 (got {0})."
+                    .format(self.image_size)
                 )
             image_size = ceil(self.image_size * n_timestamps)
         if not isinstance(self.n_bins, (int, np.integer)):
             raise TypeError("'n_bins' must be an integer.")
         if not self.n_bins >= 2:
             raise ValueError("'n_bins' must be greater than or equal to 2.")
         if self.strategy not in ['uniform', 'quantile', 'normal']:
```

### Comparing `pyts-0.8.0/pyts/image/recurrence.py` & `pyts-0.9.0/pyts/image/recurrence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for Reccurence Plot."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
 from numpy.lib.stride_tricks import as_strided
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 
 
@@ -13,15 +16,15 @@
                  n_timestamps - (dimension - 1) * time_delay,
                  dimension)
     s0, s1 = X.strides
     strides_new = (s0, s1, time_delay * s1)
     return as_strided(X, shape=shape_new, strides=strides_new)
 
 
-class RecurrencePlot(BaseEstimator, TransformerMixin):
+class RecurrencePlot(BaseEstimator, TransformerMixin):  # noqa: D207
     r"""Recurrence Plot.
 
     A recurrence plot is an image representing the distances between
     trajectories extracted from the original time series.
 
     Parameters
     ----------
@@ -31,51 +34,63 @@
         0 and 1.
 
     time_delay : int or float (default = 1)
         Time gap between two back-to-back points of the trajectory. If
         float, If float, it represents a percentage of the size of each
         time series and must be between 0 and 1.
 
-    threshold : float, 'percentage_points', 'percentage_distance' or None
-    (default = None)
-        Threshold for the minimum distance. If None, the recurrence plot
-        is not binarized.
+    threshold : float, 'point', 'distance' or None (default = None)
+        Threshold for the minimum distance. If None, the recurrence plots
+        are not binarized. If 'point', the threshold is computed such as
+        `percentage` percents of the points are smaller than the threshold.
+        If 'distance', the threshold is computed as the `percentage` of the
+        maximum distance.
 
     percentage : int or float (default = 10)
-        Percentage of black points if ``threshold='percentage_points'``
-        or percentage of maximum distance for threshold if
-        ``threshold='percentage_distance'``. Ignored if ``threshold``
-        is a float or None.
+        Percentage of black points if ``threshold='point'`` or percentage of
+        maximum distance for threshold if ``threshold='distance'``.
+        Ignored if ``threshold`` is a float or None.
 
     Notes
     -----
     Given a time series :math:`(x_1, \ldots, x_n)`, the extracted
     trajectories are
 
     .. math::
 
-        \vec(x)_i = (x_i, x_{i + \tau}, \ldots, x_{i + (m - 1)\tau}), \quad
+        \vec{x}_i = (x_i, x_{i + \tau}, \ldots, x_{i + (m - 1)\tau}), \quad
         \forall i \in \{1, \ldots, n - (m - 1)\tau \}
 
     where `m` is the `dimension` of the trajectories and :math:`\tau` is the
     `time_delay`. The recurrence plot, denoted :math:`R`, is the
     pairwise distance between the trajectories
 
     .. math::
 
-        R_{i, j} = \Theta(\varepsilon - \| \vec(x)_i - \vec(x)_j \|)
+        R_{i, j} = \Theta(\varepsilon - \| \vec{x}_i - \vec{x}_j \|), \quad
+        \forall i,j \in \{1, \ldots, n - (m - 1)\tau \}
 
     where :math:`\Theta` is the Heaviside function and :math:`\varepsilon`
     is the `threshold`.
 
     References
     ----------
     .. [1] J.-P Eckmann and S. Oliffson Kamphorst and D Ruelle, "Recurrence
            Plots of Dynamical Systems". Europhysics Letters (1987).
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.image import RecurrencePlot
+    >>> X, _, _, _ = load_gunpoint(return_X_y=True)
+    >>> transformer = RecurrencePlot()
+    >>> X_new = transformer.transform(X)
+    >>> X_new.shape
+    (50, 150, 150)
+
     """
 
     def __init__(self, dimension=1, time_delay=1,
                  threshold=None, percentage=10):
         self.dimension = dimension
         self.time_delay = time_delay
         self.threshold = threshold
@@ -123,22 +138,22 @@
             X_traj = _trajectories(X, dimension, time_delay)
             X_dist = np.sqrt(
                 np.sum((X_traj[:, None, :, :] - X_traj[:, :, None, :]) ** 2,
                        axis=3)
             )
         if self.threshold is None:
             X_rp = X_dist
-        elif self.threshold == 'percentage_points':
+        elif self.threshold == 'point':
             image_size = n_timestamps - (dimension - 1) * time_delay
             percents = np.percentile(
                 np.reshape(X_dist, (n_samples, image_size * image_size)),
                 self.percentage, axis=1
             )
             X_rp = X_dist < percents[:, None, None]
-        elif self.threshold == 'percentage_distance':
+        elif self.threshold == 'distance':
             percents = self.percentage / 100 * np.max(X_dist, axis=(1, 2))
             X_rp = X_dist < percents[:, None, None]
         else:
             X_rp = X_dist < self.threshold
         return X_rp.astype('float64')
 
     def _check_params(self, n_timestamps):
@@ -180,28 +195,26 @@
                     "than 0 and lower than or equal to 1 "
                     "(got {0}).".format(self.time_delay)
                 )
             time_delay = ceil(self.time_delay * n_timestamps)
 
         if n_timestamps - (dimension - 1) * time_delay < 1:
             raise ValueError("The number of trajectories must be positive. "
-                             "Try with smaller values for 'dimension' and "
-                             "'time_delay'.")
+                             "Consider trying with smaller values for "
+                             "'dimension' and 'time_delay'.")
 
         if (self.threshold is not None
-            and self.threshold not in ['percentage_points',
-                                       'percentage_distance']
+            and self.threshold not in ['point', 'distance']
             and not isinstance(self.threshold,
                                (int, np.integer, float, np.floating))):
-            raise TypeError("'threshold' must be either None, "
-                            "'percentage_points', 'percentage_distance', "
-                            "a float or an integer.")
+            raise TypeError("'threshold' must be either None, 'point', "
+                            "'distance', a float or an integer.")
         if ((isinstance(self.threshold, (int, np.integer, float, np.floating)))
-            and (self.threshold < 0)):
-            raise ValueError("If 'threshold' is a float or an integer,"
+            and (self.threshold <= 0)):
+            raise ValueError("If 'threshold' is a float or an integer, "
                              "it must be greater than or equal to 0.")
 
         if not isinstance(self.percentage,
                           (int, np.integer, float, np.floating)):
             raise TypeError("'percentage' must be a float or an integer.")
         if not 0 <= self.percentage <= 100:
             raise ValueError("'percentage' must be between 0 and 100.")
```

### Comparing `pyts-0.8.0/pyts/metrics/boss.py` & `pyts-0.9.0/pyts/metrics/boss.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for BOSS metric."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import sqrt
 from sklearn.utils import check_array
 
 
 def boss(x, y):
     """Return the BOSS distance between two arrays.
@@ -21,14 +24,24 @@
 
     References
     ----------
     .. [1] P. Schäfer, "The BOSS is concerned with time series classification
            in the presence of noise". Data Mining and Knowledge Discovery,
            29(6), 1505-1530 (2015).
 
+    Examples
+    --------
+    >>> from pyts.metrics import boss
+    >>> x = [0, 5, 5, 3, 4, 5]
+    >>> y = [3, 0, 0, 0, 8, 0]
+    >>> boss(x, y)
+    10.0
+    >>> boss(y, x)
+    5.0
+
     """
     x = check_array(x, ensure_2d=False, dtype='float64')
     y = check_array(y, ensure_2d=False, dtype='float64')
     if x.ndim != 1:
         raise ValueError("'x' must a one-dimensional array.")
     if y.ndim != 1:
         raise ValueError("'y' must a one-dimensional array.")
```

### Comparing `pyts-0.8.0/pyts/metrics/dtw.py` & `pyts-0.9.0/pyts/metrics/dtw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Code for Dynamic Time Warping and its variants."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
-from math import ceil, log2
+from math import ceil, log2, sqrt
 from numba import njit, prange
 from sklearn.utils import check_array
 
 
 @njit()
 def _square(x, y):
     return (x - y) ** 2
@@ -32,14 +35,26 @@
     cost_mat = np.empty((n_timestamps, n_timestamps))
     for j in prange(n_timestamps):
         for i in prange(n_timestamps):
             cost_mat[i, j] = dist(x[i], y[j])
     return cost_mat
 
 
+def _check_input_dtw(x, y):
+    x = check_array(x, ensure_2d=False, dtype='float64')
+    y = check_array(y, ensure_2d=False, dtype='float64')
+    if x.ndim != 1:
+        raise ValueError("'x' must be a one-dimensional array.")
+    if y.ndim != 1:
+        raise ValueError("'y' must be a one-dimensional array.")
+    if x.shape != y.shape:
+        raise ValueError("'x' and 'y' must have the same shape.")
+    return x, y, x.size
+
+
 def cost_matrix(x, y, dist='square', region=None):
     """Compute the cost matrix between two samples.
 
     Parameters
     ----------
     x : array-like, shape = (n_timestamps,)
         First sample.
@@ -83,17 +98,18 @@
                 raise ValueError("Calling dist(1, 1) did not return a float "
                                  "or an integer.")
         dist_ = dist
     if region is not None:
         region = check_array(region)
         region_shape = region.shape
         if region_shape != (2, x.size):
-            raise ValueError("The shape of 'region' must be equal to "
-                             "(2, n_timestamps) (got {0})".format(region_shape)
-                             )
+            raise ValueError(
+                "The shape of 'region' must be equal to (2, n_timestamps) "
+                "(got {0}).".format(region_shape)
+            )
     if region is None:
         cost_mat = _cost_matrix_no_region(x, y, dist_)
     else:
         cost_mat = _cost_matrix_region(x, y, dist_, region)
     return cost_mat
 
 
@@ -193,24 +209,30 @@
             elif argmin == 1:
                 path.append((i - 1, j))
             else:
                 path.append((i, j - 1))
     return np.transpose(np.array(path)[::-1])
 
 
-def _check_input_dtw(x, y):
-    x = check_array(x, ensure_2d=False, dtype='float64')
-    y = check_array(y, ensure_2d=False, dtype='float64')
-    if x.ndim != 1:
-        raise ValueError("'x' must a one-dimensional array.")
-    if y.ndim != 1:
-        raise ValueError("'y' must a one-dimensional array.")
-    if x.shape != y.shape:
-        raise ValueError("'x' and 'y' must have the same shape.")
-    return x, y, x.size
+def _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                    return_cost=False, return_accumulated=False,
+                    return_path=False):
+    """Return the results according to the parameters."""
+    res = (dtw_dist, )
+    if return_cost:
+        res += (cost_mat, )
+    if return_accumulated:
+        res += (acc_cost_mat, )
+    if return_path:
+        path = _return_path(acc_cost_mat)
+        res += (path, )
+    if len(res) == 1:
+        return res[0]
+    else:
+        return res
 
 
 def dtw_classic(x, y, dist='square', return_cost=False,
                 return_accumulated=False, return_path=False):
     """Classic Dynamic Time Warping (DTW) distance between two samples.
 
     Parameters
@@ -249,33 +271,34 @@
 
     path : array, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw_classic
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> dtw_classic(x, y)
+    2.0
+
     """
     x, y, n_timestamps = _check_input_dtw(x, y)
 
     cost_mat = cost_matrix(x, y, dist=dist, region=None)
     acc_cost_mat = accumulated_cost_matrix(cost_mat)
     dtw_dist = acc_cost_mat[-1, -1]
+    if dist == 'square':
+        dtw_dist = sqrt(dtw_dist)
 
-    res = (dtw_dist, )
-    if return_cost:
-        res += (cost_mat, )
-    if return_accumulated:
-        res += (acc_cost_mat, )
-    if return_path:
-        path = _return_path(acc_cost_mat)
-        res += (path, )
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
+    res = _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                          return_cost, return_accumulated, return_path)
+    return res
 
 
 def dtw_region(x, y, dist='square', region=None, return_cost=False,
                return_accumulated=False, return_path=False):
     """Dynamic Time Warping (DTW) distance with a constraint region.
 
     Parameters
@@ -320,69 +343,72 @@
 
     path : array, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw_region
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> region = [[0, 1, 1], [2, 2, 3]]
+    >>> dtw_region(x, y, region=region)
+    2.23...
+
     """
     x, y, n_timestamps = _check_input_dtw(x, y)
 
-    if region is None:
-        region_ = None
-    else:
-        try:
-            region_ = check_array(region, dtype='int64', ensure_2d=True)
-        except:
-            raise ValueError("If 'region' is not None, it must be array-like "
-                             "with shape (2, n_timestamps).")
-        if region_.shape != (2, n_timestamps):
+    if region is not None:
+        region = check_array(region, dtype='int64')
+        if region.shape != (2, n_timestamps):
             raise ValueError("If 'region' is not None, it must be array-like "
                              "with shape (2, n_timestamps).")
 
-    cost_mat = cost_matrix(x, y, dist=dist, region=region_)
+    cost_mat = cost_matrix(x, y, dist=dist, region=region)
     acc_cost_mat = accumulated_cost_matrix(cost_mat)
     dtw_dist = acc_cost_mat[-1, -1]
+    if dist == 'square':
+        dtw_dist = sqrt(dtw_dist)
 
-    res = (dtw_dist, )
-    if return_cost:
-        res += (cost_mat, )
-    if return_accumulated:
-        res += (acc_cost_mat, )
-    if return_path:
-        path = _return_path(acc_cost_mat)
-        res += (path, )
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
+    res = _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                          return_cost, return_accumulated, return_path)
+    return res
 
 
 def sakoe_chiba_band(n_timestamps, window_size=0.1):
     """Compute the Sakoe-Chiba band.
 
     Parameters
     ----------
     n_timestamps : int
         The size of both time series.
 
-    window_size : int or float
+    window_size : int or float (default = 0.1)
         The window above and below the diagonale. If float, it must be between
         0 and 1, and the actual window size will be computed as
         ``ceil(window_size * (n_timestamps - 1))``. Each cell whose distance
         with the diagonale is lower than or equal to 'window_size' becomes a
         valid cell for the path.
 
     Returns
     -------
     region : array, shape = (2, n_timestamps)
         Constraint region. The first row consists of the starting indices
         (included) and the second row consists of the ending indices (excluded)
         of the valid rows for each column.
 
+    Examples
+    --------
+    >>> from pyts.metrics import sakoe_chiba_band
+    >>> print(sakoe_chiba_band(5, window_size=2))
+    [[0 0 0 1 2]
+     [3 4 5 5 5]]
+
     """
     if not isinstance(n_timestamps, (int, np.integer)):
         raise TypeError("'n_timestamps' must be an intger.")
     else:
         if not n_timestamps >= 2:
             raise ValueError("'n_timestamps' must be an integer greater than "
                              "or equal to 2.")
@@ -421,15 +447,15 @@
 
     dist : 'square', 'absolute' or callable (default = 'square')
         Distance used. If 'square', the squared difference is used.
         If 'absolute', the absolute difference is used. If callable,
         it must be a function with a numba.njit() decorator that takes
         as input two numbers (two arguments) and returns a number.
 
-    window_size : int or float
+    window_size : int or float (default = 0.1)
         The window above and below the diagonale. If float, it must be between
         0 and 1, and the actual window size will be computed as
         ``int(window_size * (n_timestamps - 1))``. Each cell whose distance
         with the diagonale is lower than or equal to 'window_size' becomes a
         valid cell for the path.
 
     return_cost : bool (default = False)
@@ -454,54 +480,62 @@
 
     path : array, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw_sakoechiba
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> dtw_sakoechiba(x, y, window_size=1)
+    2.0
+
     """
     x, y, n_timestamps = _check_input_dtw(x, y)
 
     region = sakoe_chiba_band(n_timestamps, window_size)
     cost_mat = cost_matrix(x, y, dist=dist, region=region)
     acc_cost_mat = accumulated_cost_matrix(cost_mat)
     dtw_dist = acc_cost_mat[-1, -1]
+    if dist == 'square':
+        dtw_dist = sqrt(dtw_dist)
 
-    res = (dtw_dist, )
-    if return_cost:
-        res += (cost_mat, )
-    if return_accumulated:
-        res += (acc_cost_mat, )
-    if return_path:
-        path = _return_path(acc_cost_mat)
-        res += (path, )
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
+    res = _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                          return_cost, return_accumulated, return_path)
+    return res
 
 
 def itakura_parallelogram(n_timestamps, max_slope=2.):
     """Compute the Itakura parallelogram.
 
     Parameters
     ----------
     n_timestamps : int
         The size of both time series.
 
-    max_slope : float
+    max_slope : float (default = 2.)
         Maximum slope for the parallelogram.
 
     Returns
     -------
     region : array, shape = (2, n_timestamps)
         Constraint region. The first row consists of the starting indices
         (included) and the second row consists of the ending indices (excluded)
         of the valid rows for each column.
 
+    Examples
+    --------
+    >>> from pyts.metrics import itakura_parallelogram
+    >>> print(itakura_parallelogram(5))
+    [[0 1 1 2 4]
+     [1 3 4 4 5]]
+
     """
     if not isinstance(n_timestamps, (int, np.integer)):
         raise TypeError("'n_timestamps' must be an intger.")
     else:
         if not n_timestamps >= 2:
             raise ValueError("'n_timestamps' must be an integer greater than "
                              "or equal to 2.")
@@ -546,15 +580,15 @@
 
     dist : 'square', 'absolute' or callable (default = 'square')
         Distance used. If 'square', the squared difference is used.
         If 'absolute', the absolute difference is used. If callable,
         it must be a function with a numba.njit() decorator that takes
         as input two numbers (two arguments) and returns a number.
 
-    max_slope : float
+    max_slope : float (default = 2.)
         Maximum slope for the parallelogram.
 
     return_cost : bool (default = False)
         If True, the cost matrix is returned.
 
     return_accumulated : bool (default = False)
         If True, the accumulated cost matrix is returned.
@@ -575,34 +609,35 @@
 
     path : array, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw_itakura
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> dtw_itakura(x, y, max_slope=1.5)
+    2.23...
+
     """
     x, y, n_timestamps = _check_input_dtw(x, y)
 
     region = itakura_parallelogram(n_timestamps, max_slope)
     cost_mat = cost_matrix(x, y, dist=dist, region=region)
     acc_cost_mat = accumulated_cost_matrix(cost_mat)
     dtw_dist = acc_cost_mat[-1, -1]
+    if dist == 'square':
+        dtw_dist = sqrt(dtw_dist)
 
-    res = (dtw_dist, )
-    if return_cost:
-        res += (cost_mat, )
-    if return_accumulated:
-        res += (acc_cost_mat, )
-    if return_path:
-        path = _return_path(acc_cost_mat)
-        res += (path, )
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
+    res = _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                          return_cost, return_accumulated, return_path)
+    return res
 
 
 def _multiscale_region(n_timestamps, resolution_level, n_timestamps_reduced,
                        path, radius):
     path_length = path.shape[1]
     path_up = np.repeat(path, radius, axis=1)
     path_down = path_up.copy()
@@ -685,14 +720,22 @@
 
     path : array, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw_multiscale
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> dtw_multiscale(x, y, resolution=2)
+    2.23...
+
     """
     x, y, n_timestamps = _check_input_dtw(x, y)
     if not isinstance(resolution, (int, np.integer)):
         raise TypeError("'resolution' must be an integer.")
     if resolution < 1:
         raise ValueError("'resolution' must be a positive integer.")
     if not isinstance(radius, (int, np.integer)):
@@ -718,27 +761,20 @@
         path_res = _return_path(acc_cost_mat_res)
         region = _multiscale_region(n_timestamps, resolution,
                                     x_padded.size, path_res, radius)
 
     cost_mat = cost_matrix(x, y, dist=dist, region=region)
     acc_cost_mat = accumulated_cost_matrix(cost_mat)
     dtw_dist = acc_cost_mat[-1, -1]
+    if dist == 'square':
+        dtw_dist = sqrt(dtw_dist)
 
-    res = (dtw_dist, )
-    if return_cost:
-        res += (cost_mat, )
-    if return_accumulated:
-        res += (acc_cost_mat, )
-    if return_path:
-        path = _return_path(acc_cost_mat)
-        res += (path, )
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
+    res = _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                          return_cost, return_accumulated, return_path)
+    return res
 
 
 def dtw_fast(x, y, dist='square', radius=0, return_cost=False,
              return_accumulated=False, return_path=False):
     """Fast Dynamic Time Warping distance.
 
     Parameters
@@ -783,14 +819,22 @@
 
     path : ndarray, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw_fast
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> dtw_multiscale(x, y, resolution=2, radius=1)
+    2.0
+
     """
     x, y, n_timestamps = _check_input_dtw(x, y)
     if not isinstance(radius, (int, np.integer)):
         raise TypeError("'radius' must be an integer.")
     if radius < 0:
         raise ValueError("'radius' must be a non-negative integer.")
 
@@ -821,27 +865,20 @@
             n_timestamps_next = ceil((2 * n_timestamps) / resolution)
             region = _multiscale_region(n_timestamps_next, 2, x_padded.size,
                                         path_res, radius)
 
     cost_mat = cost_matrix(x, y, dist=dist, region=region)
     acc_cost_mat = accumulated_cost_matrix(cost_mat)
     dtw_dist = acc_cost_mat[-1, -1]
+    if dist == 'square':
+        dtw_dist = sqrt(dtw_dist)
 
-    res = (dtw_dist, )
-    if return_cost:
-        res += (cost_mat, )
-    if return_accumulated:
-        res += (acc_cost_mat, )
-    if return_path:
-        path = _return_path(acc_cost_mat)
-        res += (path, )
-    if len(res) == 1:
-        return res[0]
-    else:
-        return res
+    res = _return_results(dtw_dist, cost_mat, acc_cost_mat,
+                          return_cost, return_accumulated, return_path)
+    return res
 
 
 def dtw(x, y, dist='square', method='classic', options=None, return_cost=False,
         return_accumulated=False, return_path=False):
     """Dynamic Time Warping (DTW) distance between two samples.
 
     Parameters
@@ -868,14 +905,17 @@
             - 'fast': FastDTW
 
     options : None or dict (default = None)
         Dictionary of method options
 
             - 'classic': None
             - 'sakoechiba': window_size (int or float)
+            - 'itakura': max_slope (float)
+            - 'multiscale': resolution (int) and radius (int)
+            - 'fast': radius (int)
 
     return_cost : bool (default = False)
         If True, the cost matrix is returned.
 
     return_accumulated : bool (default = False)
         If True, the accumulated cost matrix is returned.
 
@@ -895,14 +935,22 @@
 
     path : ndarray, shape = (2, path_length)
         The optimal path along the cost matrix. The first row consists
         of the indices of the optimal path for x while the second row
         consists of the indices of the optimal path for y. Only returned
         if ``return_path=True``.
 
+    Examples
+    --------
+    >>> from pyts.metrics import dtw
+    >>> x = [0, 1, 1]
+    >>> y = [2, 0, 1]
+    >>> dtw(x, y, method='sakoechiba', options={'window_size': 2})
+    2.0
+
     """
     if options is None:
         options = dict()
 
     if method == 'classic':
         return dtw_classic(x, y, dist=dist, return_cost=return_cost,
                            return_accumulated=return_accumulated,
```

### Comparing `pyts-0.8.0/pyts/preprocessing/__init__.py` & `pyts-0.9.0/pyts/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyts-0.8.0/pyts/preprocessing/discretizer.py` & `pyts-0.9.0/pyts/preprocessing/discretizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for discretizers."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from numba import njit, prange
 from scipy.stats import norm
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_array
 from warnings import warn
 
@@ -58,14 +61,24 @@
     strategy : 'uniform', 'quantile' or 'normal' (default = 'quantile')
         Strategy used to define the widths of the bins:
 
         - 'uniform': All bins in each sample have identical widths
         - 'quantile': All bins in each sample have the same number of points
         - 'normal': Bin edges are quantiles from a standard normal distribution
 
+    Examples
+    --------
+    >>> from pyts.preprocessing import KBinsDiscretizer
+    >>> X = [[0, 1, 0, 2, 3, 3, 2, 1],
+    ...      [7, 0, 6, 1, 5, 3, 4, 2]]
+    >>> discretizer = KBinsDiscretizer(n_bins=2)
+    >>> print(discretizer.transform(X))
+    [[0 0 0 1 1 1 1 0]
+     [1 0 1 0 1 0 1 0]]
+
     """
 
     def __init__(self, n_bins=5, strategy='quantile'):
         self.n_bins = n_bins
         self.strategy = strategy
 
     def fit(self, X=None, y=None):
```

### Comparing `pyts-0.8.0/pyts/preprocessing/imputer.py` & `pyts-0.9.0/pyts/preprocessing/imputer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for imputers."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from scipy.interpolate import interp1d
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.impute import MissingIndicator
 from sklearn.utils.validation import check_array
 
 
@@ -22,14 +25,24 @@
         ('linear', 'nearest', 'zero', 'slinear', 'quadratic', 'cubic',
         'previous', 'next', where 'zero', 'slinear', 'quadratic' and 'cubic'
         refer to a spline interpolation of zeroth, first, second or third
         order; 'previous' and 'next' simply return the previous or next value
         of the point) or as an integer specifying the order of the spline
         interpolator to use. Default is 'linear'.
 
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from pyts.preprocessing import InterpolationImputer
+    >>> X = [[1, None, 3, 4], [8, None, 4, None]]
+    >>> imputer = InterpolationImputer()
+    >>> imputer.transform(X)
+    array([[1., 2., 3., 4.],
+           [8., 6., 4., 2.]])
+
     """
 
     def __init__(self, missing_values=np.nan, strategy='linear'):
         self.missing_values = missing_values
         self.strategy = strategy
 
     def fit(self, X=None, y=None):
```

### Comparing `pyts-0.8.0/pyts/preprocessing/scaler.py` & `pyts-0.9.0/pyts/preprocessing/scaler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for scalers."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import StandardScaler as SklearnStandardScaler
 from sklearn.preprocessing import MinMaxScaler as SklearnMinMaxScaler
 from sklearn.preprocessing import MaxAbsScaler as SklearnMaxAbsScaler
 from sklearn.preprocessing import RobustScaler as SklearnRobustScaler
 from sklearn.utils.validation import check_array
 
@@ -15,14 +18,24 @@
     ----------
     with_mean : bool (default = True)
         If True, center the data before scaling.
 
     with_std : bool (default = True)
         If True, scale the data to unit variance.
 
+    Examples
+    --------
+    >>> from pyts.preprocessing import StandardScaler
+    >>> X = [[0, 2, 0, 4, 4, 6, 4, 4],
+    ...      [1, 0, 3, 2, 2, 2, 0, 2]]
+    >>> scaler = StandardScaler()
+    >>> scaler.transform(X)
+    array([[-1.5, -0.5, -1.5,  0.5,  0.5,  1.5,  0.5,  0.5],
+           [-0.5, -1.5,  1.5,  0.5,  0.5,  0.5, -1.5,  0.5]])
+
     """
 
     def __init__(self, with_mean=True, with_std=True):
         self.with_mean = with_mean
         self.with_std = with_std
 
     def fit(self, X=None, y=None):
@@ -68,14 +81,24 @@
     """Transforms samples by scaling each sample to a given range.
 
     Parameters
     ----------
     sample_range : tuple (min, max) (default = (0, 1))
         Desired range of transformed data.
 
+    Examples
+    --------
+    >>> from pyts.preprocessing import MinMaxScaler
+    >>> X = [[1, 5, 3, 2, 9, 6, 4, 7],
+    ...      [1, -2, 3, 2, 2, 1, 0, 2]]
+    >>> scaler = MinMaxScaler()
+    >>> scaler.transform(X)
+    array([[0.   , 0.5  , 0.25 , 0.125, 1.   , 0.625, 0.375, 0.75 ],
+           [0.6  , 0.   , 1.   , 0.8  , 0.8  , 0.6  , 0.4  , 0.8  ]])
+
     """
 
     def __init__(self, sample_range=(0, 1)):
         self.sample_range = sample_range
 
     def fit(self, X=None, y=None):
         """Pass.
@@ -112,15 +135,27 @@
         X = check_array(X, dtype='float64')
         scaler = SklearnMinMaxScaler(feature_range=self.sample_range)
         X_new = scaler.fit_transform(X.T).T
         return X_new
 
 
 class MaxAbsScaler(BaseEstimator, TransformerMixin):
-    """Scale each sample by its maximum absolute value."""
+    """Scale each sample by its maximum absolute value.
+
+    Examples
+    --------
+    >>> from pyts.preprocessing import MaxAbsScaler
+    >>> X = [[1, 5, 3, 2, 10, 6, 4, 7],
+    ...      [1, -5, 3, 2, 2, 1, 0, 2]]
+    >>> scaler = MaxAbsScaler()
+    >>> scaler.transform(X)
+    array([[ 0.1,  0.5,  0.3,  0.2,  1. ,  0.6,  0.4,  0.7],
+           [ 0.2, -1. ,  0.6,  0.4,  0.4,  0.2,  0. ,  0.4]])
+
+    """
 
     def __init__(self):
         pass
 
     def fit(self, X=None, y=None):
         """Pass.
 
@@ -184,14 +219,26 @@
 
     with_scaling : bool (default = True)
         If True, scale the data to interquartile range.
 
     quantile_range : tuple (q_min, q_max), 0.0 < q_min < q_max < 100.0
         Default: (25.0, 75.0) = (1st quantile, 3rd quantile) = IQR
 
+    Examples
+    --------
+    >>> from pyts.preprocessing import RobustScaler
+    >>> X = [[1, -2,  4],
+    ...      [-2,  1,  1],
+    ...      [2,  3, -2]]
+    >>> scaler = RobustScaler()
+    >>> scaler.transform(X)
+    array([[ 0. , -1. ,  1. ],
+           [-2. ,  0. ,  0. ],
+           [ 0. ,  0.4, -1.6]])
+
     """
 
     def __init__(self, with_centering=True, with_scaling=True,
                  quantile_range=(25.0, 75.0)):
         self.with_centering = with_centering
         self.with_scaling = with_scaling
         self.quantile_range = quantile_range
```

### Comparing `pyts-0.8.0/pyts/preprocessing/tests/test_transformer.py` & `pyts-0.9.0/pyts/multivariate/transformation/tests/test_weasel_muse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,57 @@
-"""Testing for transformers."""
+"""Testing for WEASELMUSE class."""
+
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
 
 import numpy as np
-from itertools import product
-from scipy.stats import norm
-from ..transformer import PowerTransformer, QuantileTransformer
-
-
-def test_PowerTransformer():
-    """Test 'PowerTransformer' class."""
-    X = np.arange(30).reshape(3, 10)
-    method_list = ['yeo-johnson', 'box-cox']
-    standardize_list = [True, False]
-    for (method, standardize) in product(
-        method_list, standardize_list
-    ):
-        PowerTransformer().fit_transform(X)
-
-
-def test_QuantileTransformer():
-    """Test 'QuantileTransformer' class."""
-    # Test 1: uniform distribution
-    X = np.arange(33).reshape(3, 11)
-    arr_actual = QuantileTransformer(
-        n_quantiles=10, output_distribution='uniform'
-    ).fit_transform(X)
-    arr_desired = (X - X.min(axis=1)[:, None])
-    arr_desired = arr_desired / (X.max(axis=1) - X.min(axis=1))[:, None]
-    np.testing.assert_allclose(arr_actual, arr_desired, atol=1e-5, rtol=0.)
-
-    # Test 2: normal distribution
-    X_ppf = norm.ppf(np.linspace(0, 1, 1000)[1:-1])
-    weights = np.round(norm.pdf(X_ppf) * 1000).astype('int64')
-    X = []
-    for value, weight in zip(X_ppf, weights):
-        X += [value] * weight
-    X = np.asarray(X).reshape(1, -1)
-    arr_actual = QuantileTransformer(
-        n_quantiles=100, output_distribution='normal'
-    ).fit_transform(X)
-    arr_desired = X
-    atol = 0.01 * X.shape[1]
-    np.testing.assert_allclose(arr_actual, arr_desired, atol=atol)
+import pytest
+from scipy.sparse import csr_matrix
+
+from pyts.multivariate.transformation import WEASELMUSE
+
+n_samples, n_features, n_timestamps, n_classes = 40, 3, 100, 2
+rng = np.random.RandomState(42)
+X = rng.randn(n_samples, n_features, n_timestamps)
+y = rng.randint(n_classes, size=n_samples)
+
+
+@pytest.mark.parametrize(
+    'params, type_desired',
+    [({'sparse': True}, csr_matrix), ({'sparse': False}, np.ndarray)]
+)
+def test_output_dtype(params, type_desired):
+    """Check that the output dtype is the expected one."""
+    transformer = WEASELMUSE(**params)
+    output = transformer.fit_transform(X, y)
+    assert isinstance(output, type_desired)
+
+
+@pytest.mark.parametrize(
+    'params', [{'sparse': True}, {'sparse': False}]
+)
+def test_output_ndim(params):
+    """Check that the number of dimensions is always 2."""
+    transformer = WEASELMUSE(**params)
+    ndim_actual = transformer.fit_transform(X, y).ndim
+    assert ndim_actual == 2
+
+
+def test_n_estimators():
+    """Check that the number of estimators is the number of features."""
+    transformer = WEASELMUSE().fit(X, y)
+    assert len(transformer._estimators) == n_features
+    assert len(transformer._estimators_diff) == n_features
+
+
+@pytest.mark.parametrize(
+    'params', [{'sparse': True}, {'sparse': False}]
+)
+def test_fit_transform(params):
+    """Check that fit and transform and fit_transform yield same results."""
+    transformer = WEASELMUSE(**params)
+    arr_1 = transformer.fit(X, y).transform(X)
+    arr_2 = transformer.fit_transform(X, y)
+    if transformer.sparse:
+        assert (arr_1 != arr_2).nnz == 0
+    else:
+        np.testing.assert_array_equal(arr_1, arr_2)
```

### Comparing `pyts-0.8.0/pyts/preprocessing/transformer.py` & `pyts-0.9.0/pyts/preprocessing/transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Code for transformers."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.preprocessing import PowerTransformer as SklearnPowerTransformer
 from sklearn.preprocessing import (QuantileTransformer as
                                    SklearnQuantileTransformer)
 from sklearn.utils.validation import check_array
 
 
@@ -46,14 +49,24 @@
     ----------
     .. [1] I.K. Yeo and R.A. Johnson, "A new family of power transformations to
            improve normality or symmetry." Biometrika, 87(4), pp.954-959,
            (2000).
     .. [2] G.E.P. Box and D.R. Cox, "An Analysis of Transformations", Journal
            of the Royal Statistical Society B, 26, 211-252 (1964).
 
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from pyts.preprocessing import PowerTransformer
+    >>> X = [[1, 3, 4], [2, 2, 5]]
+    >>> pt = PowerTransformer()
+    >>> print(pt.transform(X))
+    [[-1.316...  0.209...  1.106...]
+     [-0.707... -0.707...  1.414...]]
+
     """
 
     def __init__(self, method='yeo-johnson', standardize=True):
         self.method = method
         self.standardize = standardize
 
     def fit(self, X=None, y=None):
@@ -84,15 +97,15 @@
 
         Returns
         -------
         X_new : array-like, shape = (n_samples, n_timestamps)
             Transformed data.
 
         """
-        X = check_array(X, dtype='float64')
+        X = check_array(X, dtype='float64', force_all_finite='allow-nan')
         transformer = SklearnPowerTransformer(
             method=self.method, standardize=self.standardize
         )
         X_new = transformer.fit_transform(X.T).T
         return X_new
 
 
@@ -125,14 +138,23 @@
     random_state : int, RandomState instance or None, optional (default=None)
         If int, random_state is the seed used by the random number generator;
         If RandomState instance, random_state is the random number generator;
         If None, the random number generator is the RandomState instance used
         by np.random. Note that this is used by subsampling and smoothing
         noise.
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.preprocessing import QuantileTransformer
+    >>> X, _, _, _  = load_gunpoint(return_X_y=True)
+    >>> qt = QuantileTransformer(n_quantiles=10)
+    >>> qt.transform(X) # doctest: +ELLIPSIS
+    array([...])
+
     """
 
     def __init__(self, n_quantiles=1000, output_distribution='uniform',
                  subsample=int(1e5), random_state=None):
         self.n_quantiles = n_quantiles
         self.output_distribution = output_distribution
         self.subsample = subsample
```

### Comparing `pyts-0.8.0/pyts/transformation/boss.py` & `pyts-0.9.0/pyts/transformation/boss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 """Code for Bag-of-SFA Symbols."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from math import ceil
+from scipy.sparse import csr_matrix
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.utils.validation import check_array, check_is_fitted
 from sklearn.utils.multiclass import check_classification_targets
 from ..approximation import SymbolicFourierApproximation
 from ..utils import windowed_view
 
@@ -23,14 +27,22 @@
     ----------
     word_size : int (default = 4)
         Size of each word.
 
     n_bins : int (default = 4)
         The number of bins to produce. It must be between 2 and 26.
 
+    strategy : str (default = 'quantile')
+        Strategy used to define the widths of the bins:
+
+        - 'uniform': All bins in each sample have identical widths
+        - 'quantile': All bins in each sample have the same number of points
+        - 'normal': Bin edges are quantiles from a standard normal distribution
+        - 'entropy': Bin edges are computed using information gain
+
     window_size : int or float (default = 10)
         Size of the sliding window. If float, it represents the percentage of
         the size of each time series and must be between 0 and 1. The window
         size will be computed as ``ceil(window_size * n_timestamps)``.
 
     window_step : int or float (default = 1)
         Step of the sliding window. If float, it represents the percentage of
@@ -47,58 +59,67 @@
 
     norm_mean : bool (default = False)
         If True, center each subseries before scaling.
 
     norm_std : bool (default = False)
         If True, scale each subseries to unit variance.
 
-    strategy : str (default = 'quantile')
-        Strategy used to define the widths of the bins:
+    numerosity_reduction : bool (default = True)
+        If True, delete sample-wise all but one occurence of back to back
+        identical occurences of the same words.
 
-        - 'uniform': All bins in each sample have identical widths
-        - 'quantile': All bins in each sample have the same number of points
-        - 'normal': Bin edges are quantiles from a standard normal distribution
-        - 'entropy': Bin edges are computed using information gain
+    sparse : bool (default = True)
+        Return a sparse matrix if True, else return an array.
 
     alphabet : None, 'ordinal' or array-like, shape = (n_bins,)
         Alphabet to use. If None, the first `n_bins` letters of the Latin
         alphabet are used.
 
-    numerosity_reduction : bool (default = True)
-        If True, delete sample-wise all but one occurence of back to back
-        identical occurences of the same words.
-
     Attributes
     ----------
     vocabulary_ : dict
         A mapping of feature indices to terms.
 
     References
     ----------
     .. [1] P. Schäfer, "The BOSS is concerned with time series classification
            in the presence of noise". Data Mining and Knowledge Discovery,
            29(6), 1505-1530 (2015).
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.transformation import BOSS
+    >>> X_train, X_test, _, _ = load_gunpoint(return_X_y=True)
+    >>> boss = BOSS(word_size=2, n_bins=2, sparse=False)
+    >>> boss.fit(X_train) # doctest: +ELLIPSIS
+    BOSS(...)
+    >>> sorted(boss.vocabulary_.values())
+    ['aa', 'ab', 'ba', 'bb']
+    >>> boss.transform(X_test) # doctest: +ELLIPSIS
+    array(...)
+
     """
 
-    def __init__(self, word_size=4, n_bins=4, window_size=10, window_step=1,
-                 anova=False, drop_sum=False, norm_mean=False,
-                 norm_std=False, strategy='quantile', alphabet=None,
-                 numerosity_reduction=True):
+    def __init__(self, word_size=4, n_bins=4, strategy='quantile',
+                 window_size=10, window_step=1, anova=False, drop_sum=False,
+                 norm_mean=False, norm_std=False, numerosity_reduction=True,
+                 sparse=True, alphabet=None):
         self.word_size = word_size
         self.n_bins = n_bins
+        self.strategy = strategy
         self.window_size = window_size
         self.window_step = window_step
         self.anova = anova
         self.drop_sum = drop_sum
         self.norm_mean = norm_mean
         self.norm_std = norm_std
-        self.strategy = strategy
-        self.alphabet = alphabet
         self.numerosity_reduction = numerosity_reduction
+        self.sparse = sparse
+        self.alphabet = alphabet
 
     def fit(self, X, y=None):
         """Fit the model according to the given training data.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
@@ -126,15 +147,18 @@
         X_windowed = X_windowed.reshape(n_samples * n_windows, window_size)
 
         sfa = SymbolicFourierApproximation(
             n_coefs=self.word_size, drop_sum=self.drop_sum, anova=self.anova,
             norm_mean=self.norm_mean, norm_std=self.norm_std,
             n_bins=self.n_bins, strategy=self.strategy, alphabet=self.alphabet
         )
-        y_repeated = np.repeat(y, n_windows)
+        if y is None:
+            y_repeated = None
+        else:
+            y_repeated = np.repeat(y, n_windows)
         X_sfa = sfa.fit_transform(X_windowed, y_repeated)
 
         X_word = np.asarray([''.join(X_sfa[i])
                              for i in range(n_samples * n_windows)])
         X_word = X_word.reshape(n_samples, n_windows)
 
         if self.numerosity_reduction:
@@ -158,14 +182,15 @@
 
     def transform(self, X):
         """Transform the provided data.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
+            Test samples.
 
         Returns
         -------
         X_new : sparse matrix, shape = (n_samples, n_words)
             Document-term matrix.
 
         """
@@ -187,23 +212,25 @@
                               np.full(n_samples, True)]
             X_bow = np.asarray([' '.join(X_word[i, not_equal[i]])
                                 for i in range(n_samples)])
         else:
             X_bow = np.asarray([' '.join(X_word[i]) for i in range(n_samples)])
 
         X_boss = self._vectorizer.transform(X_bow)
-        return X_boss
+        if not self.sparse:
+            return X_boss.A
+        return csr_matrix(X_boss)
 
     def fit_transform(self, X, y=None):
         """Fit the data then transform it.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
-            Train samples.
+            Training vector.
 
         y : None or array-like, shape = (n_samples,)
             Class labels for each data sample.
 
         Returns
         -------
         X_new : sparse matrix, shape = (n_samples, n_words)
@@ -224,15 +251,18 @@
         X_windowed = X_windowed.reshape(n_samples * n_windows, window_size)
 
         sfa = SymbolicFourierApproximation(
             n_coefs=self.word_size, drop_sum=self.drop_sum, anova=self.anova,
             norm_mean=self.norm_mean, norm_std=self.norm_std,
             n_bins=self.n_bins, strategy=self.strategy, alphabet=self.alphabet
         )
-        y_repeated = np.repeat(y, n_windows)
+        if y is None:
+            y_repeated = None
+        else:
+            y_repeated = np.repeat(y, n_windows)
         X_sfa = sfa.fit_transform(X_windowed, y_repeated)
 
         X_word = np.asarray([''.join(X_sfa[i])
                              for i in range(n_samples * n_windows)])
         X_word = X_word.reshape(n_samples, n_windows)
 
         if self.numerosity_reduction:
@@ -248,15 +278,17 @@
         self.vocabulary_ = {value: key for key, value in
                             vectorizer.vocabulary_.items()}
         self._window_size = window_size
         self._window_step = window_step
         self._n_windows = n_windows
         self._sfa = sfa
         self._vectorizer = vectorizer
-        return X_boss
+        if not self.sparse:
+            return X_boss.A
+        return csr_matrix(X_boss)
 
     def _check_params(self, n_timestamps):
         if not isinstance(self.word_size, (int, np.integer)):
             raise TypeError("'word_size' must be an integer.")
         if not self.word_size >= 1:
             raise ValueError("'word_size' must be a positive integer.")
```

### Comparing `pyts-0.8.0/pyts/transformation/weasel.py` & `pyts-0.9.0/pyts/transformation/weasel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Code for Word ExtrAction for time SEries cLassification."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
-from scipy.sparse import csc_matrix, hstack
+from scipy.sparse import coo_matrix, csr_matrix, hstack
 from sklearn.utils.validation import check_array, check_X_y, check_is_fitted
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.feature_selection import chi2
 from ..approximation import SymbolicFourierApproximation
 from ..utils import windowed_view
@@ -59,14 +62,17 @@
         - 'normal': Bin edges are quantiles from a standard normal distribution
         - 'entropy': Bin edges are computed using information gain
 
     chi2_threshold : int or float (default = 2)
         The threshold used to perform feature selection. Only the words with
         a chi2 statistic above this threshold will be kept.
 
+    sparse : bool (default = True)
+        Return a sparse matrix if True, else return an array.
+
     alphabet : None, 'ordinal' or array-like, shape = (n_bins,)
         Alphabet to use. If None, the first `n_bins` letters of the Latin
         alphabet are used.
 
     Attributes
     ----------
     vocabulary_ : dict
@@ -74,41 +80,52 @@
 
     References
     ----------
     .. [1] P. Schäfer, and U. Leser, "Fast and Accurate Time Series
            Classification with WEASEL". Conference on Information and Knowledge
            Management, 637-646 (2017).
 
+    Examples
+    --------
+    >>> from pyts.datasets import load_gunpoint
+    >>> from pyts.transformation import WEASEL
+    >>> X_train, _, y_train, _ = load_gunpoint(return_X_y=True)
+    >>> weasel = WEASEL(sparse=False)
+    >>> weasel.fit(X_train, y_train) # doctest: +ELLIPSIS
+    WEASEL(...)
+    >>> weasel.transform(X_train) # doctest: +ELLIPSIS
+    array(...)
+
     """
 
     def __init__(self, word_size=4, n_bins=4,
                  window_sizes=[0.1, 0.3, 0.5, 0.7, 0.9], window_steps=None,
                  anova=True, drop_sum=True, norm_mean=True, norm_std=True,
-                 strategy='entropy', chi2_threshold=2, alphabet=None):
+                 strategy='entropy', chi2_threshold=2, sparse=True,
+                 alphabet=None):
         self.word_size = word_size
         self.n_bins = n_bins
         self.window_sizes = window_sizes
         self.window_steps = window_steps
         self.anova = anova
         self.drop_sum = drop_sum
         self.norm_mean = norm_mean
         self.norm_std = norm_std
-        self.n_bins = n_bins
         self.strategy = strategy
         self.chi2_threshold = chi2_threshold
+        self.sparse = sparse
         self.alphabet = alphabet
 
     def fit(self, X, y):
         """Fit the model according to the given training data.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
-            Training vector, where n_samples in the number of samples and
-            n_features is the number of features.
+            Training vector.
 
         y : array-like, shape = (n_samples,)
             Class labels for each data sample.
 
         Returns
         -------
         self : object
@@ -183,15 +200,15 @@
         """
         check_is_fitted(self, ['_relevant_features_list', '_sfa_list',
                                '_vectorizer_list', 'vocabulary_'])
 
         X = check_array(X)
         n_samples, n_timestamps = X.shape
 
-        X_features = csc_matrix((n_samples, 0), dtype=np.int64)
+        X_features = coo_matrix((n_samples, 0), dtype=np.int64)
 
         for (window_size, window_step, sfa,
              vectorizer, relevant_features) in zip(
                  self._window_sizes, self._window_steps, self._sfa_list,
                  self._vectorizer_list, self._relevant_features_list):
 
             n_windows = ((n_timestamps - window_size + window_step)
@@ -205,25 +222,27 @@
             X_word = np.asarray([''.join(X_sfa[i])
                                  for i in range(n_samples * n_windows)])
             X_word = X_word.reshape(n_samples, n_windows)
             X_bow = np.asarray([' '.join(X_word[i]) for i in range(n_samples)])
             X_counts = vectorizer.transform(X_bow)[:, relevant_features]
             X_features = hstack([X_features, X_counts])
 
-        return X_features
+        if not self.sparse:
+            return X_features.A
+        return csr_matrix(X_features)
 
     def fit_transform(self, X, y):
         """Fit the data then transform it.
 
         Parameters
         ----------
         X : array-like, shape = (n_samples, n_timestamps)
             Train samples.
 
-        y : None or array-like, shape = (n_samples,)
+        y : array-like, shape = (n_samples,)
             Class labels for each data sample.
 
         Returns
         -------
         X_new : array, shape (n_samples, n_words)
             Document-term matrix.
 
@@ -236,15 +255,15 @@
         self._window_steps = window_steps
 
         self._sfa_list = []
         self._vectorizer_list = []
         self._relevant_features_list = []
         self.vocabulary_ = {}
 
-        X_features = csc_matrix((n_samples, 0), dtype=np.int64)
+        X_features = coo_matrix((n_samples, 0), dtype=np.int64)
 
         for (window_size, window_step) in zip(window_sizes, window_steps):
             n_windows = ((n_timestamps - window_size + window_step)
                          // window_step)
             X_windowed = windowed_view(
                 X, window_size=window_size, window_step=window_step
             )
@@ -278,15 +297,17 @@
                 self.vocabulary_[i + old_length_vocab] = \
                     str(window_size) + " " + vocabulary[idx]
 
             self._relevant_features_list.append(relevant_features)
             self._sfa_list.append(sfa)
             self._vectorizer_list.append(vectorizer)
 
-        return X_features
+        if not self.sparse:
+            return X_features.A
+        return csr_matrix(X_features)
 
     def _check_params(self, n_timestamps):
         if not isinstance(self.word_size, (int, np.integer)):
             raise TypeError("'word_size' must be an integer.")
         if not self.word_size >= 1:
             raise ValueError("'word_size' must be a positive integer.")
```

### Comparing `pyts-0.8.0/pyts/utils/utils.py` & `pyts-0.9.0/pyts/utils/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Code for utility tools."""
 
+# Author: Johann Faouzi <johann.faouzi@gmail.com>
+# License: BSD-3-Clause
+
 import numpy as np
 from numpy.lib.stride_tricks import as_strided
 from sklearn.utils import check_array
 
 
-def segmentation(ts_size, window_size, overlapping, n_segments=None):
+def segmentation(ts_size, window_size, overlapping=False, n_segments=None):
     """Compute the indices for Piecewise Agrgegate Approximation.
 
     Parameters
     ----------
     ts_size : int
         The size of the time series.
 
     window_size : int
         The size of the window.
 
-    overlapping : bool
+    overlapping : bool (default = False)
         If True, overlapping windows may be used. If False, non-overlapping
         are used.
 
     n_segments : int or None (default = None)
         The number of windows. If None, the number is automatically
         computed using ``window_size``.
 
@@ -31,14 +34,25 @@
 
     end : array
         The upper bound for each window.
 
     size : int
         The size of ``start``.
 
+    Examples
+    --------
+    >>> from pyts.utils import segmentation
+    >>> start, end, size = segmentation(ts_size=12, window_size=3)
+    >>> print(start)
+    [0 3 6 9]
+    >>> print(end)
+    [ 3  6  9 12]
+    >>> size
+    4
+
     """
     if not isinstance(ts_size, (int, np.integer)):
         raise TypeError("'ts_size' must be an integer.")
     if not ts_size >= 2:
         raise ValueError("'ts_size' must be an integer greater than or equal "
                          "to 2 (got {0}).".format(ts_size))
     if not isinstance(window_size, (int, np.integer)):
@@ -48,19 +62,23 @@
                          "equal to 1 (got {0}).".format(window_size))
     if not window_size <= ts_size:
         raise ValueError("'window_size' must be lower than or equal to "
                          "'ts_size' ({0} > {1}).".format(window_size, ts_size))
     if not (n_segments is None or isinstance(n_segments, (int, np.integer))):
         raise TypeError("'n_segments' must be None or an integer.")
     if isinstance(n_segments, (int, np.integer)):
-        if not 2 <= n_segments <= ts_size:
+        if not n_segments >= 2:
             raise ValueError(
                 "If 'n_segments' is an integer, it must be greater than or "
-                "equal to 2 and lower than or equal to 'ts_size' "
-                "({0} > {1}).".format(n_segments, ts_size)
+                "equal to 2 (got {0}).".format(n_segments)
+            )
+        if not n_segments <= ts_size:
+            raise ValueError(
+                "If 'n_segments' is an integer, it must be lower than or "
+                "equal to 'ts_size' ({0} > {1}).".format(n_segments, ts_size)
             )
 
     if n_segments is None:
         quotient, remainder = divmod(ts_size, window_size)
         n_segments = quotient if remainder == 0 else quotient + 1
 
     if not overlapping:
@@ -97,14 +115,25 @@
 
     Returns
     -------
     X_new : array, shape = (n_samples, n_windows, window_size)
         Windowed view of the input data. ``n_windows`` is computed as
         ``(n_timestamps - window_size + window_step) // window_step``.
 
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from pyts.utils import windowed_view
+    >>> windowed_view(np.arange(6).reshape(1, -1), window_size=2)
+    array([[[0, 1],
+            [1, 2],
+            [2, 3],
+            [3, 4],
+            [4, 5]]])
+
     """
     X = check_array(X, dtype=None)
     n_samples, n_timestamps = X.shape
 
     if not isinstance(window_size, (int, np.integer)):
         raise TypeError("'window_size' must be an integer.")
     if not 1 <= window_size <= n_timestamps:
```

### Comparing `pyts-0.8.0/pyts.egg-info/PKG-INFO` & `pyts-0.9.0/pyts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: pyts
-Version: 0.8.0
-Summary: A python package for time series transformation and classification
+Version: 0.9.0
+Summary: A python package for time series classification
 Home-page: https://github.com/johannfaouzi/pyts
 Maintainer: Johann Faouzi
 Maintainer-email: johann.faouzi@gmail.com
 License: new BSD
 Download-URL: https://github.com/johannfaouzi/pyts
 Description: [![Build Status](https://travis-ci.org/johannfaouzi/pyts.svg?branch=master)](https://travis-ci.org/johannfaouzi/pyts)
         [![Build Status](https://img.shields.io/appveyor/ci/johannfaouzi/pyts/master.svg)](https://ci.appveyor.com/project/johannfaouzi/pyts)
-        [![Build Status](https://circleci.com/gh/johannfaouzi/pyts/tree/master.svg?style=shield)](https://circleci.com/gh/johannfaouzi/pyts)
         [![Documentation Status](https://readthedocs.org/projects/pyts/badge/?version=latest)](https://pyts.readthedocs.io/en/latest/?badge=latest)
         [![Codecov](https://codecov.io/gh/johannfaouzi/pyts/branch/master/graph/badge.svg)](https://codecov.io/gh/johannfaouzi/pyts)
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyts.svg)](https://img.shields.io/pypi/pyversions/pyts.svg)
         [![PyPI version](https://badge.fury.io/py/pyts.svg)](https://badge.fury.io/py/pyts)
+        [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/johannfaouzi/pyts.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/johannfaouzi/pyts/context:python)
         [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1244152.svg)](https://doi.org/10.5281/zenodo.1244152)
         
-        ## pyts: a Python package for time series transformation and classification
+        ## pyts: a Python package for time series classification
         
-        pyts is a Python package for time series transformation and classification. It
+        pyts is a Python package for time series classification. It
         aims to make time series classification easily accessible by providing
         preprocessing and utility tools, and implementations of
         state-of-the-art algorithms. Most of these algorithms transform time series,
         thus pyts provides several tools to perform these transformations.
         
         
         ### Installation
         
         #### Dependencies
         
         pyts requires:
         
         - Python (>= 3.5)
         - NumPy (>= 1.15.4)
-        - SciPy (>= 1.1.0)
+        - SciPy (>= 1.3.0)
         - Scikit-Learn (>=0.20.1)
-        - Numba (>0.41.0)
+        - Numba (>=0.41.0)
         
         To run the examples Matplotlib (>=2.0.0) is required.
         
         
         #### User installation
         
         If you already have a working installation of numpy, scipy, scikit-learn and
         numba, you can easily install pyts using ``pip``
         
             pip install pyts
         
+        or ``conda`` via the ``conda-forge`` channel
+        
+          conda install -c conda-forge pyts
+        
         You can also get the latest version of pyts by cloning the repository
         
             git clone https://github.com/johannfaouzi/pyts.git
             cd pyts
             pip install .
         
         
@@ -74,15 +78,15 @@
         [Development Guide](https://scikit-learn.org/stable/developers/). A slight
         difference is the use of Numba instead of Cython for optimization.
         
         ### Documentation
         
         The section below gives some information about the implemented algorithms in pyts.
         For more information, please have a look at the
-        [HTML documentation available via ReadTheDocs](https://pyts.readthedocs.io/en/latest/)
+        [HTML documentation available via ReadTheDocs](https://pyts.readthedocs.io/en/latest/).
         
         ### Implemented features
         
         pyts consists of the following modules:
         
         - `approximation`: This module provides implementations of algorithms that
         approximate time series. Implemented algorithms are
@@ -99,17 +103,21 @@
         
         - `classification`: This module provides implementations of algorithms that
         can classify time series. Implemented algorithms are
         [KNeighborsClassifier](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.KNeighborsClassifier.html#),
         [SAXVSM](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.SAXVSM.html#) and
         [BOSSVS](https://pyts.readthedocs.io/en/latest/generated/pyts.classification.BOSSVS.html#).
         
+        - `datasets`: This module provides utilities to make or load toy datasets,
+        as well as fetching datasets from the
+        [UEA & UCR Time Series Classification Repository](http://www.timeseriesclassification.com).
+        
         - `decomposition`: This module provides implementations of algorithms that
-        decompose a time series into several time series. The only implemented algorithm
-        is
+        decompose a time series into several time series. The only implemented
+        algorithm is
         [Singular Spectrum Analysis](https://pyts.readthedocs.io/en/latest/generated/pyts.decomposition.SingularSpectrumAnalysis.html#).
         
         - `image`: This module provides implementations of algorithms that transform
         time series into images. Implemented algorithms are
         [Recurrence Plot](https://pyts.readthedocs.io/en/latest/generated/pyts.image.RecurrencePlot.html#),
         [Gramian Angular Field](https://pyts.readthedocs.io/en/latest/generated/pyts.image.GramianAngularField.html#) and
         [Markov Transition Field](https://pyts.readthedocs.io/en/latest/generated/pyts.image.MarkovTransitionField.html#).
@@ -117,20 +125,29 @@
         - `metrics`: This module provides implementations of metrics that are specific
         to time series. Implemented metrics are
         [Dynamic Time Warping](https://pyts.readthedocs.io/en/latest/generated/pyts.metrics.dtw.html#)
         with several variants and the
         [BOSS](https://pyts.readthedocs.io/en/latest/generated/pyts.metrics.boss.html#)
         metric.
         
+        - `multivariate`: This modules provides utilities to deal with multivariate
+        time series. Available tools are
+        [MultivariateTransformer](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.transformation.MultivariateTransformer.html) and
+        [MultivariateClassifier](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.classification.MultivariateClassifier.html)
+        to transform and classify multivariate time series using tools for univariate
+        time series respectively, as well as
+        [JointRecurrencePlot](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.image.JointRecurrencePlot.html) and
+        [WEASEL+MUSE](https://pyts.readthedocs.io/en/latest/generated/pyts.multivariate.transformation.WEASELMUSE.html).
+        
         - `preprocessing`: This module provides most of the scikit-learn preprocessing
         tools but applied sample-wise (i.e. to each time series independently) instead
         of feature-wise, as well as an
         [imputer](https://pyts.readthedocs.io/en/latest/generated/pyts.preprocessing.InterpolationImputer.html#)
         of missing values using interpolation. More information is available at the
-        [pyts.preprocessing API documentation](https://pyts.readthedocs.io/en/latest/api.html#module-pyts.preprocessing)
+        [pyts.preprocessing API documentation](https://pyts.readthedocs.io/en/latest/api.html#module-pyts.preprocessing).
         
         - `transformation`: This module provides implementations of algorithms that
         transform a data set of time series with shape `(n_samples, n_timestamps)` into
         a data set with shape `(n_samples, n_features)`. Implemented algorithms are
         [BOSS](https://pyts.readthedocs.io/en/latest/generated/pyts.transformation.BOSS.html#) and
         [WEASEL](https://pyts.readthedocs.io/en/latest/generated/pyts.transformation.WEASEL.html#).
```

### Comparing `pyts-0.8.0/setup.py` & `pyts-0.9.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-"""A python package for time series transformation and classification."""
+"""A python package for time series classification."""
 
 import pyts
 from setuptools import find_packages, setup
 
 
 DISTNAME = 'pyts'
-DESCRIPTION = ('A python package for time series transformation '
-               'and classification')
+DESCRIPTION = 'A python package for time series classification'
 with open('README.md') as f:
     LONG_DESCRIPTION = f.read()
 LONG_DESCRIPTION_CONTENT_TYPE = 'text/markdown'
 MAINTAINER = 'Johann Faouzi'
 MAINTAINER_EMAIL = 'johann.faouzi@gmail.com'
 URL = 'https://github.com/johannfaouzi/pyts'
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/johannfaouzi/pyts'
 VERSION = pyts.__version__
 INSTALL_REQUIRES = ['numpy>=1.15.4'
-                    'scipy>=1.1.0'
+                    'scipy>=1.3.0'
                     'scikit-learn>=0.20.1'
                     'numba>=0.41.0']
 CLASSIFIERS = ['Development Status :: 3 - Alpha',
                'Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
                'License :: OSI Approved',
                'Programming Language :: Python',
@@ -35,30 +34,39 @@
                'Programming Language :: Python :: 3.6',
                'Programming Language :: Python :: 3.7']
 EXTRAS_REQUIRE = {
     'tests': [
         'pytest',
         'pytest-cov'],
     'docs': [
-        'sphinx',
+        'sphinx==1.8.2',
         'sphinx-gallery',
         'sphinx_rtd_theme',
         'numpydoc',
         'matplotlib'
     ]
 }
+PACKAGE_DATA = {
+    'pyts': ['datasets/cached_datasets/UCR/Coffee/*.txt',
+             'datasets/cached_datasets/UCR/GunPoint/*.txt',
+             'datasets/cached_datasets/UCR/PigCVP/*.txt',
+             'datasets/cached_datasets/UEA/BasicMotions/*.arff',
+             'datasets/cached_datasets/UEA/BasicMotions/*.txt',
+             'datasets/info/*.pickle']
+}
 
 setup(name=DISTNAME,
       maintainer=MAINTAINER,
       maintainer_email=MAINTAINER_EMAIL,
       description=DESCRIPTION,
       license=LICENSE,
       url=URL,
       version=VERSION,
       download_url=DOWNLOAD_URL,
       long_description=LONG_DESCRIPTION,
       long_description_content_type=LONG_DESCRIPTION_CONTENT_TYPE,
       zip_safe=False,
       classifiers=CLASSIFIERS,
       packages=find_packages(),
+      package_data=PACKAGE_DATA,
       install_requires=INSTALL_REQUIRES,
       extras_require=EXTRAS_REQUIRE)
```

