# Comparing `tmp/pyleoclim-0.9.0.tar.gz` & `tmp/pyleoclim-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleoclim-0.9.0.tar", last modified: Wed Aug 17 02:34:08 2022, max compression
+gzip compressed data, was "pyleoclim-0.9.1.tar", last modified: Sat Sep 17 20:29:40 2022, max compression
```

## Comparing `pyleoclim-0.9.0.tar` & `pyleoclim-0.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-08-17 02:34:08.825043 pyleoclim-0.9.0/
--rw-r--r--   0 deborahkhider   (501) staff       (20)     6471 2022-08-17 02:34:08.825309 pyleoclim-0.9.0/PKG-INFO
--rw-r--r--   0 deborahkhider   (501) staff       (20)     5907 2022-06-06 18:54:34.000000 pyleoclim-0.9.0/README.md
-drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-08-17 02:34:08.805948 pyleoclim-0.9.0/pyleoclim/
--rw-r--r--   0 deborahkhider   (501) staff       (20)      456 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/__init__.py
-drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-08-17 02:34:08.813866 pyleoclim-0.9.0/pyleoclim/core/
--rw-r--r--   0 deborahkhider   (501) staff       (20)      675 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/__init__.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    36739 2022-06-27 20:52:17.000000 pyleoclim-0.9.0/pyleoclim/core/coherence.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     2304 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/corr.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     7507 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/correns.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    32709 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/ensembleseries.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    16333 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/lipd.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    56833 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/lipdseries.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    64683 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/multipleseries.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    46099 2022-08-16 22:40:39.000000 pyleoclim-0.9.0/pyleoclim/core/psds.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    23669 2022-08-16 22:40:39.000000 pyleoclim-0.9.0/pyleoclim/core/scalograms.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)   119233 2022-08-17 01:59:06.000000 pyleoclim-0.9.0/pyleoclim/core/series.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     8520 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/spatialdecomp.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    10919 2022-08-12 19:34:36.000000 pyleoclim-0.9.0/pyleoclim/core/ssares.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)      678 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/core/surrogateseries.py
-drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-08-17 02:34:08.818087 pyleoclim-0.9.0/pyleoclim/tests/
--rw-r--r--   0 deborahkhider   (501) staff       (20)      163 2020-09-18 05:05:42.000000 pyleoclim-0.9.0/pyleoclim/tests/__init__.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)      290 2020-09-18 05:05:42.000000 pyleoclim-0.9.0/pyleoclim/tests/examples.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     3494 2022-06-27 20:52:17.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_Coherence.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     2111 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_CorrEns.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     6291 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_EnsembleSeries.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     2598 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_Lipd.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     3877 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_LipdSeries.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     3119 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_MultiplePSD.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    14048 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_MultipleSeries.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     2034 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_PSD.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     2750 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_SSARes.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     2001 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_Scalogram.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    32708 2022-08-12 22:49:37.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_Series.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     3235 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/tests/test_core_SpatialDecomp.py
-drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-08-17 02:34:08.824274 pyleoclim-0.9.0/pyleoclim/utils/
--rw-r--r--   0 deborahkhider   (501) staff       (20)      527 2021-10-25 22:02:49.000000 pyleoclim-0.9.0/pyleoclim/utils/__init__.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    16885 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/causality.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    27176 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/correlation.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    14946 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/decomposition.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    15335 2022-06-27 20:52:17.000000 pyleoclim-0.9.0/pyleoclim/utils/filter.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     8356 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/jsonutils.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    49377 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/lipdutils.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    17759 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/mapping.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    14208 2022-08-16 22:13:59.000000 pyleoclim-0.9.0/pyleoclim/utils/plotting.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    44040 2022-08-12 21:23:17.000000 pyleoclim-0.9.0/pyleoclim/utils/spectral.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)     4971 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/tsbase.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    13916 2022-06-06 18:54:35.000000 pyleoclim-0.9.0/pyleoclim/utils/tsmodel.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)    37316 2022-08-12 22:09:59.000000 pyleoclim-0.9.0/pyleoclim/utils/tsutils.py
--rw-r--r--   0 deborahkhider   (501) staff       (20)   114742 2022-08-12 19:47:18.000000 pyleoclim-0.9.0/pyleoclim/utils/wavelet.py
-drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-08-17 02:34:08.807719 pyleoclim-0.9.0/pyleoclim.egg-info/
--rw-r--r--   0 deborahkhider   (501) staff       (20)     6471 2022-08-17 02:34:08.000000 pyleoclim-0.9.0/pyleoclim.egg-info/PKG-INFO
--rw-r--r--   0 deborahkhider   (501) staff       (20)     1553 2022-08-17 02:34:08.000000 pyleoclim-0.9.0/pyleoclim.egg-info/SOURCES.txt
--rw-r--r--   0 deborahkhider   (501) staff       (20)        1 2022-08-17 02:34:08.000000 pyleoclim-0.9.0/pyleoclim.egg-info/dependency_links.txt
--rw-r--r--   0 deborahkhider   (501) staff       (20)        1 2019-09-06 00:42:29.000000 pyleoclim-0.9.0/pyleoclim.egg-info/not-zip-safe
--rw-r--r--   0 deborahkhider   (501) staff       (20)      251 2022-08-17 02:34:08.000000 pyleoclim-0.9.0/pyleoclim.egg-info/requires.txt
--rw-r--r--   0 deborahkhider   (501) staff       (20)       10 2022-08-17 02:34:08.000000 pyleoclim-0.9.0/pyleoclim.egg-info/top_level.txt
--rw-r--r--   0 deborahkhider   (501) staff       (20)       79 2022-08-17 02:34:08.826122 pyleoclim-0.9.0/setup.cfg
--rw-r--r--   0 deborahkhider   (501) staff       (20)     1446 2022-08-17 02:29:23.000000 pyleoclim-0.9.0/setup.py
+drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-09-17 20:29:40.759530 pyleoclim-0.9.1/
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     6489 2022-09-17 20:29:40.759683 pyleoclim-0.9.1/PKG-INFO
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     5945 2022-09-17 20:27:17.000000 pyleoclim-0.9.1/README.md
+drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-09-17 20:29:40.723934 pyleoclim-0.9.1/pyleoclim/
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      456 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/__init__.py
+drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-09-17 20:29:40.740432 pyleoclim-0.9.1/pyleoclim/core/
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      675 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/core/__init__.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    36739 2022-06-27 20:52:17.000000 pyleoclim-0.9.1/pyleoclim/core/coherence.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     2424 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/core/corr.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     8527 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/core/correns.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    32709 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/core/ensembleseries.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    16333 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/core/lipd.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    56906 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/core/lipdseries.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    64683 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/core/multipleseries.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    46087 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/core/psds.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    23669 2022-08-16 22:40:39.000000 pyleoclim-0.9.1/pyleoclim/core/scalograms.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)   120216 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/core/series.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     8520 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/core/spatialdecomp.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    10919 2022-08-12 19:34:36.000000 pyleoclim-0.9.1/pyleoclim/core/ssares.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      678 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/core/surrogateseries.py
+drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-09-17 20:29:40.747164 pyleoclim-0.9.1/pyleoclim/tests/
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      163 2020-09-18 05:05:42.000000 pyleoclim-0.9.1/pyleoclim/tests/__init__.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      290 2020-09-18 05:05:42.000000 pyleoclim-0.9.1/pyleoclim/tests/examples.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     3494 2022-06-27 20:52:17.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_Coherence.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     2111 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_CorrEns.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     6291 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_EnsembleSeries.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     2598 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_Lipd.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     3877 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_LipdSeries.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     3119 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_MultiplePSD.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    14048 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_MultipleSeries.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     2034 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_PSD.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     2750 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_SSARes.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     2001 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_Scalogram.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    32708 2022-08-12 22:49:37.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_Series.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     3235 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/tests/test_core_SpatialDecomp.py
+drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-09-17 20:29:40.758238 pyleoclim-0.9.1/pyleoclim/utils/
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      527 2021-10-25 22:02:49.000000 pyleoclim-0.9.1/pyleoclim/utils/__init__.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    16885 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/causality.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    27176 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/correlation.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    14946 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/decomposition.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    15335 2022-06-27 20:52:17.000000 pyleoclim-0.9.1/pyleoclim/utils/filter.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     8356 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/jsonutils.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    49377 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/lipdutils.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    17759 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/mapping.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    14547 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/utils/plotting.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    44026 2022-09-17 20:17:31.000000 pyleoclim-0.9.1/pyleoclim/utils/spectral.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     4971 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/tsbase.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    13916 2022-06-06 18:54:35.000000 pyleoclim-0.9.1/pyleoclim/utils/tsmodel.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)    37316 2022-08-12 22:09:59.000000 pyleoclim-0.9.1/pyleoclim/utils/tsutils.py
+-rw-r--r--   0 deborahkhider   (501) staff       (20)   114742 2022-08-12 19:47:18.000000 pyleoclim-0.9.1/pyleoclim/utils/wavelet.py
+drwxr-xr-x   0 deborahkhider   (501) staff       (20)        0 2022-09-17 20:29:40.728157 pyleoclim-0.9.1/pyleoclim.egg-info/
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     6489 2022-09-17 20:29:40.000000 pyleoclim-0.9.1/pyleoclim.egg-info/PKG-INFO
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     1553 2022-09-17 20:29:40.000000 pyleoclim-0.9.1/pyleoclim.egg-info/SOURCES.txt
+-rw-r--r--   0 deborahkhider   (501) staff       (20)        1 2022-09-17 20:29:40.000000 pyleoclim-0.9.1/pyleoclim.egg-info/dependency_links.txt
+-rw-r--r--   0 deborahkhider   (501) staff       (20)        1 2019-09-06 00:42:29.000000 pyleoclim-0.9.1/pyleoclim.egg-info/not-zip-safe
+-rw-r--r--   0 deborahkhider   (501) staff       (20)      249 2022-09-17 20:29:40.000000 pyleoclim-0.9.1/pyleoclim.egg-info/requires.txt
+-rw-r--r--   0 deborahkhider   (501) staff       (20)       10 2022-09-17 20:29:40.000000 pyleoclim-0.9.1/pyleoclim.egg-info/top_level.txt
+-rw-r--r--   0 deborahkhider   (501) staff       (20)       79 2022-09-17 20:29:40.760161 pyleoclim-0.9.1/setup.cfg
+-rw-r--r--   0 deborahkhider   (501) staff       (20)     1444 2022-09-17 20:19:23.000000 pyleoclim-0.9.1/setup.py
```

### Comparing `pyleoclim-0.9.0/PKG-INFO` & `pyleoclim-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: pyleoclim
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python package for paleoclimate data analysis
 Home-page: https://github.com/LinkedEarth/Pyleoclim_util/pyleoclim
+Download-URL: https://github.com/LinkedEarth/Pyleoclim_util/tarball/0.9.1
 Author: Deborah Khider, Feng Zhu, Julien Emile-Geay, Jun Hu, Myron Kwan, Pratheek Athreya, Alexander James, Daniel Garijo
 Author-email: linkedearth@gmail.com
 License: GPL-3.0 License
-Download-URL: https://github.com/LinkedEarth/Pyleoclim_util/tarball/0.9.0
 Keywords: Paleoclimate, Data Analysis, LiPD
-Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 <!---[![PyPI](https://img.shields.io/pypi/dm/pyleoclim.svg)](https://pypi.python.org/pypi/Pyleoclim)-->
 [![PyPI version](https://badge.fury.io/py/pyleoclim.svg)](https://badge.fury.io/py/pyleoclim)
 [![PyPI](https://img.shields.io/badge/python-3.9-yellow.svg)]()
 [![license](https://img.shields.io/github/license/linkedearth/Pyleoclim_util.svg)]()
-[![DOI](https://zenodo.org/badge/59611213.svg)](https://zenodo.org/badge/latestdoi/59611213)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6999279.svg)](https://doi.org/10.5281/zenodo.6999279)
 [![NSF-1541029](https://img.shields.io/badge/NSF-1541029-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1541029)
 [![Build Status](https://travis-ci.org/LinkedEarth/Pyleoclim_util.svg?branch=master)](https://travis-ci.org/LinkedEarth/Pyleoclim_util)
 
 ![](https://github.com/LinkedEarth/Logos/raw/master/pyleoclim_logo_full_white.png)
 
 **Python Package for the Analysis of Paleoclimate Data**
 
-Paleoclimate data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.
+[Paleoclimate](https://www.ncdc.noaa.gov/news/what-paleoclimatology) data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.
 Pyleoclim is a Python package primarily geared towards the analysis and visualization of such timeseries. The package includes several low-level methods to deal with these issues under the hood, leaving paleoscientists to interact with intuitive, high-level analysis and plotting methods that support publication-quality scientific workflows.
 
 There are many entry points to Pyleoclim, thanks to its underlying [data structures](https://pyleoclim-util.readthedocs.io/en/master/core/ui.html). The package leverages the Linked Paleo Data ([LiPD](http://www.clim-past.net/12/1093/2016/)) standard container and its associated [utilities](http://nickmckay.github.io/LiPD-utilities/). The package is aware of age ensembles stored via LiPD and uses them for time-uncertain analyses, very much like its R sidekick, [GeoChronR](https://doi.org/10.5194/gchron-2020-25).
 
 LiPD is not an obligatory entry point to Pyleoclim. Low-level modules work on [NumPy](http://www.numpy.org) arrays or [Pandas](https://pandas.pydata.org) dataframes, so most Pyleoclim timeseries analysis functionalities can apply to these more common types as well, including those generated by numerical models (via [xarray](http://xarray.pydata.org)). This makes the package suitable for rigorous and efficient model-data comparisons, like [this one](https://www.pnas.org/content/116/18/8728.short).
 
-We've worked very hard to make Pyleoclim accessible to a wide variety of users, from establisher researchers to high-school students, and from seasoned Pythonistas to first-time programmers. A growing collection of workflows that use Pyleoclim are available as Jupyter notebooks on [paleoBooks](https://github.com/LinkedEarth/PaleoBooks/tree/master/notebooks), with video tutorials on the LinkedEarth [YouTube channel](https://www.youtube.com/watch?v=LJaQBFMK2-Q&list=PL93NbaRnKAuF4WpIQf-4y_U4lo-GqcrcW). Python novices are encouraged to follow these [self-paced tutorials](http://linked.earth/ec_workshops_py/) before trying Pyleoclim.
+We've worked very hard to make Pyleoclim accessible to a wide variety of users, from establisher researchers to high-school students, and from seasoned Pythonistas to first-time programmers. A progressive introduction to the package is available at [PyleoTutorials](http://linked.earth/PyleoTutorials/) A growing collection of research-grade workflows using Pyleoclim and the LinkedEarth research ecosystem are available as Jupyter notebooks on [paleoBooks](https://github.com/LinkedEarth/PaleoBooks/tree/master/notebooks), with video tutorials on the LinkedEarth [YouTube channel](https://www.youtube.com/watch?v=LJaQBFMK2-Q&list=PL93NbaRnKAuF4WpIQf-4y_U4lo-GqcrcW). Python novices are encouraged to follow these [self-paced tutorials](http://linked.earth/ec_workshops_py/) before trying Pyleoclim.
 
 Science-based training materials are also available from the [paleoHackathon repository](https://github.com/LinkedEarth/paleoHackathon). You can run these training notebooks at any time in a myBinder environment. We also run live training workshops several times a year. Follow us on [Twitter](https://twitter.com/Linked_Earth), or join our [Discourse Forum](https://discourse.linked.earth) for more information.
 
 ### Versions
 
 See our [releases page](https://github.com/LinkedEarth/Pyleoclim_util/releases) for details on what's included in each version.
 
@@ -60,19 +59,15 @@
 
 Please submit any reproducible bugs you encounter to the [issue tracker](https://github.com/LinkedEarth/Pyleoclim_util/issues). For usage questions, please use [Discourse](https://discourse.linked.earth).
 
 
 ### License
 
 The project is licensed under the GNU Public License. Please refer to the file call license.
-If you use the code in publications, please credit the work using this citation:
-
-_Deborah Khider, Feng Zhu, Julien Emile-Geay, Jun Hu, Alexander James, Pratheek Athreya, Myron Kwan, Daniel Garijo. (xxxx). Pyleoclim: vx.x.x Release. Zenodo. http://doi.org/10.5281/zenodo.1212692_
+If you use the code in publications, please credit the work using the citation file. 
 
 
 ### Disclaimer
 
 This material is based upon work supported by the National Science Foundation under Grant Number ICER-1541029. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the investigators and do not necessarily reflect the views of the National Science Foundation.
 
 This research is funded in part by JP Morgan Chase & Co. Any views or opinions expressed herein are solely those of the authors listed, and may differ from the views and opinions expressed by JP Morgan Chase & Co. or its affilitates. This material is not a product of the Research Department of J.P. Morgan Securities LLC. This material should not be construed as an individual recommendation of for any particular client and is not intended as a recommendation of particular securities, financial instruments or strategies for a particular client. This material does not constitute a solicitation or offer in any jurisdiction.
-
-
```

### Comparing `pyleoclim-0.9.0/README.md` & `pyleoclim-0.9.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!---[![PyPI](https://img.shields.io/pypi/dm/pyleoclim.svg)](https://pypi.python.org/pypi/Pyleoclim)-->
 [![PyPI version](https://badge.fury.io/py/pyleoclim.svg)](https://badge.fury.io/py/pyleoclim)
 [![PyPI](https://img.shields.io/badge/python-3.9-yellow.svg)]()
 [![license](https://img.shields.io/github/license/linkedearth/Pyleoclim_util.svg)]()
-[![DOI](https://zenodo.org/badge/59611213.svg)](https://zenodo.org/badge/latestdoi/59611213)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6999279.svg)](https://doi.org/10.5281/zenodo.6999279)
 [![NSF-1541029](https://img.shields.io/badge/NSF-1541029-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1541029)
 [![Build Status](https://travis-ci.org/LinkedEarth/Pyleoclim_util.svg?branch=master)](https://travis-ci.org/LinkedEarth/Pyleoclim_util)
 
 ![](https://github.com/LinkedEarth/Logos/raw/master/pyleoclim_logo_full_white.png)
 
 **Python Package for the Analysis of Paleoclimate Data**
 
-Paleoclimate data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.
+[Paleoclimate](https://www.ncdc.noaa.gov/news/what-paleoclimatology) data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.
 Pyleoclim is a Python package primarily geared towards the analysis and visualization of such timeseries. The package includes several low-level methods to deal with these issues under the hood, leaving paleoscientists to interact with intuitive, high-level analysis and plotting methods that support publication-quality scientific workflows.
 
 There are many entry points to Pyleoclim, thanks to its underlying [data structures](https://pyleoclim-util.readthedocs.io/en/master/core/ui.html). The package leverages the Linked Paleo Data ([LiPD](http://www.clim-past.net/12/1093/2016/)) standard container and its associated [utilities](http://nickmckay.github.io/LiPD-utilities/). The package is aware of age ensembles stored via LiPD and uses them for time-uncertain analyses, very much like its R sidekick, [GeoChronR](https://doi.org/10.5194/gchron-2020-25).
 
 LiPD is not an obligatory entry point to Pyleoclim. Low-level modules work on [NumPy](http://www.numpy.org) arrays or [Pandas](https://pandas.pydata.org) dataframes, so most Pyleoclim timeseries analysis functionalities can apply to these more common types as well, including those generated by numerical models (via [xarray](http://xarray.pydata.org)). This makes the package suitable for rigorous and efficient model-data comparisons, like [this one](https://www.pnas.org/content/116/18/8728.short).
 
-We've worked very hard to make Pyleoclim accessible to a wide variety of users, from establisher researchers to high-school students, and from seasoned Pythonistas to first-time programmers. A growing collection of workflows that use Pyleoclim are available as Jupyter notebooks on [paleoBooks](https://github.com/LinkedEarth/PaleoBooks/tree/master/notebooks), with video tutorials on the LinkedEarth [YouTube channel](https://www.youtube.com/watch?v=LJaQBFMK2-Q&list=PL93NbaRnKAuF4WpIQf-4y_U4lo-GqcrcW). Python novices are encouraged to follow these [self-paced tutorials](http://linked.earth/ec_workshops_py/) before trying Pyleoclim.
+We've worked very hard to make Pyleoclim accessible to a wide variety of users, from establisher researchers to high-school students, and from seasoned Pythonistas to first-time programmers. A progressive introduction to the package is available at [PyleoTutorials](http://linked.earth/PyleoTutorials/) A growing collection of research-grade workflows using Pyleoclim and the LinkedEarth research ecosystem are available as Jupyter notebooks on [paleoBooks](https://github.com/LinkedEarth/PaleoBooks/tree/master/notebooks), with video tutorials on the LinkedEarth [YouTube channel](https://www.youtube.com/watch?v=LJaQBFMK2-Q&list=PL93NbaRnKAuF4WpIQf-4y_U4lo-GqcrcW). Python novices are encouraged to follow these [self-paced tutorials](http://linked.earth/ec_workshops_py/) before trying Pyleoclim.
 
 Science-based training materials are also available from the [paleoHackathon repository](https://github.com/LinkedEarth/paleoHackathon). You can run these training notebooks at any time in a myBinder environment. We also run live training workshops several times a year. Follow us on [Twitter](https://twitter.com/Linked_Earth), or join our [Discourse Forum](https://discourse.linked.earth) for more information.
 
 ### Versions
 
 See our [releases page](https://github.com/LinkedEarth/Pyleoclim_util/releases) for details on what's included in each version.
 
@@ -46,17 +46,15 @@
 
 Please submit any reproducible bugs you encounter to the [issue tracker](https://github.com/LinkedEarth/Pyleoclim_util/issues). For usage questions, please use [Discourse](https://discourse.linked.earth).
 
 
 ### License
 
 The project is licensed under the GNU Public License. Please refer to the file call license.
-If you use the code in publications, please credit the work using this citation:
-
-_Deborah Khider, Feng Zhu, Julien Emile-Geay, Jun Hu, Alexander James, Pratheek Athreya, Myron Kwan, Daniel Garijo. (xxxx). Pyleoclim: vx.x.x Release. Zenodo. http://doi.org/10.5281/zenodo.1212692_
+If you use the code in publications, please credit the work using the citation file. 
 
 
 ### Disclaimer
 
 This material is based upon work supported by the National Science Foundation under Grant Number ICER-1541029. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the investigators and do not necessarily reflect the views of the National Science Foundation.
 
 This research is funded in part by JP Morgan Chase & Co. Any views or opinions expressed herein are solely those of the authors listed, and may differ from the views and opinions expressed by JP Morgan Chase & Co. or its affilitates. This material is not a product of the Research Department of J.P. Morgan Securities LLC. This material should not be construed as an individual recommendation of for any particular client and is not intended as a recommendation of particular securities, financial instruments or strategies for a particular client. This material does not constitute a solicitation or offer in any jurisdiction.
```

### Comparing `pyleoclim-0.9.0/pyleoclim/core/__init__.py` & `pyleoclim-0.9.1/pyleoclim/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/coherence.py` & `pyleoclim-0.9.1/pyleoclim/core/coherence.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/corr.py` & `pyleoclim-0.9.1/pyleoclim/core/corr.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Corr objects are used to store the results of the correlation method between Series
 and/or MultipleSeries. Its main purpose is to allow a print function to display the output.
 """
 
 import numpy as np
 from tabulate import tabulate
+from copy import deepcopy
 
 def pval_format(p, threshold=0.01, style='exp'):
     ''' Print p-value with proper format when p is close to 0
     '''
     if p < threshold:
         if p == 0:
             if style == 'float':
@@ -66,14 +67,19 @@
     def __init__(self, r, p, signif, alpha, p_fmt_td=0.01, p_fmt_style='exp'):
         self.r = r
         self.p = p
         self.p_fmt_td = p_fmt_td
         self.p_fmt_style = p_fmt_style
         self.signif = signif
         self.alpha = alpha
+        
+    def copy(self):
+        '''Copy object
+        '''
+        return deepcopy(self)
 
     def __str__(self):
         '''
         Prints out the correlation results
         '''
         formatted_p = pval_format(self.p, threshold=self.p_fmt_td, style=self.p_fmt_style)
```

### Comparing `pyleoclim-0.9.0/pyleoclim/core/correns.py` & `pyleoclim-0.9.1/pyleoclim/core/correns.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 """
 CorrEns objects store the result of an ensemble correlation calculation between timeseries and/or ensemble of timeseries.
 The class enables a print and plot function to easily visualize the result. 
 """
 
 import numpy as np
 import seaborn as sns
+import pandas as pd
 from matplotlib import pyplot as plt, transforms as transforms
 from matplotlib.ticker import MaxNLocator
 from tabulate import tabulate
+from copy import deepcopy
 
 from ..utils import plotting
 
 def pval_format(p, threshold=0.01, style='exp'):
     ''' Print p-value with proper format when p is close to 0
     '''
     if p < threshold:
@@ -89,14 +91,19 @@
         self.r = r
         self.p = p
         self.p_fmt_td = p_fmt_td
         self.p_fmt_style = p_fmt_style
         self.signif = signif
         self.signif_fdr = signif_fdr
         self.alpha = alpha
+        
+    def copy(self):
+        '''Copy object
+        '''
+        return deepcopy(self)
 
     def __str__(self):
         '''
         Prints out the correlation results
         '''
 
         pi_list = []
@@ -110,44 +117,52 @@
             f'signif. w/ FDR (α: {self.alpha})': self.signif_fdr,
         }
 
         msg = print(tabulate(table, headers='keys'))
 
         return f'Ensemble size: {len(self.r)}'
 
-    def plot(self, figsize=[4, 4], title=None, ax=None, savefig_settings=None, hist_kwargs=None, title_kwargs=None,
-             xlim=None,
-             clr_insignif=sns.xkcd_rgb['grey'], clr_signif=sns.xkcd_rgb['teal'],
-             clr_signif_fdr=sns.xkcd_rgb['pale orange'],
-             clr_percentile=sns.xkcd_rgb['salmon'], rwidth=0.8, bins=None, vrange=None):
+    def plot(self, figsize=[4, 4], title=None, ax=None, savefig_settings=None, hist_kwargs=None,
+             title_kwargs=None, xlim=None, alpha = 0.8, multiple = 'layer',
+             clr_insignif='silver', clr_signif=sns.xkcd_rgb['teal'],
+             clr_signif_fdr='darkorange', clr_percentile=sns.xkcd_rgb['salmon']):
         ''' Plot the distribution of correlation values as a histogram
+       
+        Uses seaborn's `histplot <https://seaborn.pydata.org/generated/seaborn.histplot.html>`_
         
         Color-coding is used to indicate significance, with or without applying 
         the False Discovery Rate (FDR) method. 
 
         Parameters
         ----------
         figsize : list, optional
         
             The figure size. The default is [4, 4].
 
         title : str, optional
         
             Plot title. The default is None.
+            
+        multiple: str, optional 
+            Approach to organizing the 3 different histrograms on the plot. 
+            possible values: “layer”[default], “dodge”, “stack”, “fill”
+            
+        alpha : float in [0, 1]
+            transparency parameter for histrogram bars. Default: 0.8
 
         savefig_settings : dict
         
             the dictionary of arguments for plt.savefig(); some notes below:
             - "path" must be specified; it can be any existing or new path,
               with or without a suffix; if the suffix is not given in "path", it will follow "format"
             - "format" can be one of {"pdf", "eps", "png", "ps"}
 
         hist_kwargs : dict
         
-            the keyword arguments for ax.hist()
+            additional keyword arguments for sns.histplot() [experimental]
 
         title_kwargs : dict
         
             the keyword arguments for ax.set_title()
 
         ax : matplotlib.axis, optional
         
@@ -161,44 +176,53 @@
         See also
         --------
         
         pyleoclim.core.series.Series.correlation: correlation with significance
         
         pyleoclim.utils.correlation.fdr: False Discovery Rate
 
-        matplotlib.pyplot.hist: https://matplotlib.org/3.3.3/api/_as_gen/matplotlib.pyplot.hist.html
+        seaborn.histplot: https://seaborn.pydata.org/generated/seaborn.histplot.html
         
         pyleoclim.utils.plotting.savefig : save figures in Pyleoclim
         '''
         savefig_settings = {} if savefig_settings is None else savefig_settings.copy()
         hist_kwargs = {} if hist_kwargs is None else hist_kwargs.copy()
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
 
-        if vrange is None:
-            vrange = [np.min(self.r), np.max(self.r)]
-
-        clr_list = [clr_insignif, clr_signif, clr_signif_fdr]
-        args = {'rwidth': rwidth, 'bins': bins, 'range': vrange, 'color': clr_list}
+        clr_list = [clr_signif_fdr, clr_signif, clr_insignif]
+        args = {'multiple': multiple, 'alpha': alpha, 'ax': ax}
         args.update(hist_kwargs)
-        # insignif_args.update(hist_kwargs)
-
+        
         r_insignif = np.array(self.r)[~np.array(self.signif)]
         r_signif = np.array(self.r)[self.signif]
         r_signif_fdr = np.array(self.r)[self.signif_fdr]
-        r_stack = [r_insignif, r_signif, r_signif_fdr]
-        ax.hist(r_stack, stacked=True, **args)
-        ax.legend([f'p ≥ {self.alpha}', f'p < {self.alpha} (w/o FDR)', f'p < {self.alpha} (w/ FDR)'], loc='upper left',
-                  bbox_to_anchor=(1.1, 1), ncol=1)
+        #r_stack = [r_insignif, r_signif, r_signif_fdr]
+        #ax.hist(r_stack, stacked=True, **args)
+
+        # put everything into a dataframe to be able to use seaborn
+            
+        data = np.empty((len(self.r),3)); data[:] = np.NaN
+        col  = [f'p < {self.alpha} (w/ FDR)',f'p < {self.alpha} (w/o FDR)', f'p ≥ {self.alpha}']
+        data[self.signif_fdr,0] = r_signif_fdr        
+        data[self.signif, 1] = r_signif
+        data[~np.array(self.signif),2] = r_insignif
+
+        df = pd.DataFrame(data,columns=col) # place data into a dataframe for seaborn to chew on
+        sns.set_palette(sns.color_palette(clr_list)) # update color palette
+        ax = sns.histplot(data=df, **args) # draw histogram
+        sns.move_legend(ax, "upper left", bbox_to_anchor=(1.08, 1)) # move legend to the right
+    
+        #ax.legend(loc='upper right', bbox_to_anchor=(1.1, 1), ncol=1)
 
         frac_signif = np.size(r_signif) / np.size(self.r)
         frac_signif_fdr = np.size(r_signif_fdr) / np.size(self.r)
-        ax.text(x=1.1, y=0.5, s=f'Fraction significant: {frac_signif * 100:.1f}%', transform=ax.transAxes, fontsize=10,
+        ax.text(x=1.1, y=0.4, s=f'Fraction significant: {frac_signif * 100:.1f}%', transform=ax.transAxes, fontsize=10,
                 color=clr_signif)
-        ax.text(x=1.1, y=0.4, s=f'Fraction significant: {frac_signif_fdr * 100:.1f}%', transform=ax.transAxes,
+        ax.text(x=1.1, y=0.5, s=f'Fraction significant: {frac_signif_fdr * 100:.1f}%', transform=ax.transAxes,
                 fontsize=10, color=clr_signif_fdr)
 
         r_pcts = np.percentile(self.r, [2.5, 25, 50, 75, 97.5])
         trans = transforms.blended_transform_factory(ax.transData, ax.transAxes)
         for r_pct, pt, ls in zip(r_pcts, np.array([2.5, 25, 50, 75, 97.5]) / 100, [':', '--', '-', '--', ':']):
             ax.axvline(x=r_pct, linestyle=ls, color=clr_percentile)
             ax.text(x=r_pct, y=1.02, s=pt, color=clr_percentile, transform=trans, ha='center', fontsize=10)
```

### Comparing `pyleoclim-0.9.0/pyleoclim/core/ensembleseries.py` & `pyleoclim-0.9.1/pyleoclim/core/ensembleseries.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/lipd.py` & `pyleoclim-0.9.1/pyleoclim/core/lipd.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/lipdseries.py` & `pyleoclim-0.9.1/pyleoclim/core/lipdseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,25 +732,25 @@
         if ensemble == True:
             warnings.warn('Some of the computation in ensemble mode can require a few minutes to complete.')
 
         savefig_settings = {} if savefig_settings is None else savefig_settings.copy()
         res = self.getMetadata()
         # start plotting
         fig = plt.figure(figsize=figsize)
-        gs = gridspec.GridSpec(2, 5)
+        gs = gridspec.GridSpec(2, 6, wspace=0)
         gs.update(left=0, right=1.1)
 
         if ensemble == True:
             ens = self.chronEnsembleToPaleo(D)
             ensc = ens.common_time()
 
         ax = {}
         # Plot the timeseries
         plt_kwargs = {} if plt_kwargs is None else plt_kwargs.copy()
-        ax['ts'] = plt.subplot(gs[0, :-3])
+        ax['ts'] = fig.add_subplot(gs[0, :-1])
         plt_kwargs.update({'ax': ax['ts']})
         # use the defaults if color/markers not specified
         if ensemble == False:
             if 'marker' not in plt_kwargs.keys():
                 archiveType = lipdutils.LipdToOntology(res['archiveType']).lower().replace(" ", "")
                 plt_kwargs.update({'marker': self.plot_default[archiveType][1]})
             if 'color' not in plt_kwargs.keys():
@@ -768,17 +768,17 @@
             ax['ts'] = ensc.plot_envelope(**plt_kwargs)
         else:
             raise ValueError("Invalid argument value for ensemble")
         ymin, ymax = ax['ts'].get_ylim()
 
         # plot the distplot
         distplt_kwargs = {} if distplt_kwargs is None else distplt_kwargs.copy()
-        ax['dts'] = plt.subplot(gs[0, 2])
+        ax['dts'] = fig.add_subplot(gs[0, -1:])
         distplt_kwargs.update({'ax': ax['dts']})
-        distplt_kwargs.update({'ylabel': 'PDF'})
+        distplt_kwargs.update({'ylabel': 'Counts'})
         distplt_kwargs.update({'vertical': True})
         if 'color' not in distplt_kwargs.keys():
             archiveType = lipdutils.LipdToOntology(res['archiveType']).lower().replace(" ", "")
             distplt_kwargs.update({'color': self.plot_default[archiveType][0]})
         if ensemble == False:
             ax['dts'] = self.distplot(**distplt_kwargs)
         elif ensemble == True:
@@ -852,15 +852,15 @@
         if 'legend' in map_kwargs.keys():
             legend = map_kwargs['legend']
         else:
             legend = False
         # make the plot map
 
         data_crs = ccrs.PlateCarree()
-        ax['map'] = plt.subplot(gs[1, 0], projection=proj)
+        ax['map'] = fig.add_subplot(gs[1, 0:2], projection=proj)
         ax['map'].coastlines()
         if background is True:
             ax['map'].stock_img()
         # Other extra information
         if borders is True:
             ax['map'].add_feature(cfeature.BORDERS)
         if lakes is True:
@@ -881,15 +881,15 @@
             pass
         else:
             if ensemble == False:
                 spectral_kwargs.update({'freq_method': 'lomb_scargle'})
             elif ensemble == True:
                 pass
 
-        ax['spec'] = plt.subplot(gs[1, 1:3])
+        ax['spec'] = fig.add_subplot(gs[1, -3:])
         spectralfig_kwargs = {} if spectralfig_kwargs is None else spectralfig_kwargs.copy()
         spectralfig_kwargs.update({'ax': ax['spec']})
 
         if ensemble == False:
             ts_preprocess = self.detrend().standardize()
             psd = ts_preprocess.spectral(**spectral_kwargs)
 
@@ -929,15 +929,17 @@
                       "    Climate Variable: " + res["Climate_Variable"] + "\n" + \
                       "    Detail: " + res["Detail"] + "\n" + \
                       "    Seasonality: " + res["Seasonality"] + "\n" + \
                       "    Direction: " + res["Interpretation_Direction"] + "\n \n" + \
                       "Calibration: \n" + \
                       "    Equation: " + res["Calibration_equation"] + "\n" + \
                       "    Notes: " + res["Calibration_notes"]
-            plt.figtext(0.7, 0.4, textstr, fontsize=12)
+            plt.figtext(1.15, 0.4, textstr, fontsize=12)
+        
+        #gs.tight_layout(fig)
 
         if 'path' in savefig_settings:
             plotting.savefig(fig, settings=savefig_settings)
 
         return fig, ax
 
     def mapNearRecord(self, D, n=5, radius=None, sameArchive=False,
```

### Comparing `pyleoclim-0.9.0/pyleoclim/core/multipleseries.py` & `pyleoclim-0.9.1/pyleoclim/core/multipleseries.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/psds.py` & `pyleoclim-0.9.1/pyleoclim/core/psds.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,15 +945,15 @@
 
         new = self.copy()
         new.beta_est_res = res_dict
         new.psd_list = psd_beta_list
         return new
 
 
-    def plot(self, figsize=[10, 4], in_loglog=True, in_period=True, xlabel=None, ylabel='Amplitude', title=None,
+    def plot(self, figsize=[10, 4], in_loglog=True, in_period=True, xlabel=None, ylabel='PSD', title=None,
              xlim=None, ylim=None, savefig_settings=None, ax=None, xticks=None, yticks=None, legend=True,
              colors=None, cmap=None, norm=None, plot_kwargs=None, lgd_kwargs=None):
         '''Plot multiple PSDs on the same plot
 
         Parameters
         ----------
         
@@ -1115,15 +1115,15 @@
             if 'path' in savefig_settings:
                 plotting.savefig(fig, settings=savefig_settings)
             return fig, ax
         else:
             return ax
 
     def plot_envelope(self, figsize=[10, 4], qs=[0.025, 0.5, 0.975],
-             in_loglog=True, in_period=True, xlabel=None, ylabel='Amplitude', title=None,
+             in_loglog=True, in_period=True, xlabel=None, ylabel='PSD', title=None,
              xlim=None, ylim=None, savefig_settings=None, ax=None, xticks=None, yticks=None, plot_legend=True,
              curve_clr=sns.xkcd_rgb['pale red'], curve_lw=3, shade_clr=sns.xkcd_rgb['pale red'], shade_alpha=0.3, shade_label=None,
              lgd_kwargs=None, members_plot_num=10, members_alpha=0.3, members_lw=1, seed=None):
 
         '''Plot an envelope statistics for mulitple PSD
         
         This function plots an envelope statistics from multiple PSD. This is especially useful when the PSD are coming from an ensemble of possible solutions (e.g., age ensembles)
```

### Comparing `pyleoclim-0.9.0/pyleoclim/core/scalograms.py` & `pyleoclim-0.9.1/pyleoclim/core/scalograms.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/series.py` & `pyleoclim-0.9.1/pyleoclim/core/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         return res
 
     def plot(self, figsize=[10, 4],
               marker=None, markersize=None, color=None,
               linestyle=None, linewidth=None, xlim=None, ylim=None,
               label=None, xlabel=None, ylabel=None, title=None, zorder=None,
               legend=True, plot_kwargs=None, lgd_kwargs=None, alpha=None,
-              savefig_settings=None, ax=None, invert_xaxis=False):
+              savefig_settings=None, ax=None, invert_xaxis=False, invert_yaxis=False):
         ''' Plot the timeseries
 
         Parameters
         ----------
 
         figsize : list
             a list of two integers indicating the figure size
@@ -418,14 +418,17 @@
             The default drawing order for all lines on the plot
 
         legend : {True, False}
             plot legend or not
 
         invert_xaxis : bool, optional
             if True, the x-axis of the plot will be inverted
+        
+        invert_yaxis : bool, optional
+            same for the y-axis
 
         plot_kwargs : dict
             the dictionary of keyword arguments for ax.plot()
             See [matplotlib.pyplot.plot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html) for details
 
         lgd_kwargs : dict
             the dictionary of keyword arguments for ax.legend()
@@ -546,15 +549,15 @@
 
         res = plotting.plot_xy(
             self.time, self.value,
             figsize=figsize, xlabel=xlabel, ylabel=ylabel,
             title=title, savefig_settings=savefig_settings,
             ax=ax, legend=legend, xlim=xlim, ylim=ylim,
             plot_kwargs=plot_kwargs, lgd_kwargs=lgd_kwargs,
-            invert_xaxis=invert_xaxis,
+            invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis
         )
 
         return res
 
     def ssa(self, M=None, nMC=0, f=0.3, trunc = None, var_thresh=80):
         ''' Singular Spectrum Analysis
 
@@ -1189,19 +1192,19 @@
         ts_plot_kwargs = {} if ts_plot_kwargs is None else ts_plot_kwargs.copy()
         gridspec_kwargs = {} if gridspec_kwargs is None else gridspec_kwargs.copy()
 
         # spacing
         if (type(psd_label) == str and '\n' in psd_label) or (psd_label is None):
             gridspec_kwargs_default = {'width_ratios': [6, 1],
                                        'height_ratios': [8, 1, .35],
-                                       'hspace': .05, 'wspace': 0.1}
+                                       'hspace': 0.05, 'wspace': 0}
         else:
             gridspec_kwargs_default = {'width_ratios': [6, 1],
                                        'height_ratios': [8, 1, .35],
-                                       'hspace': 0, 'wspace': 0.1}
+                                       'hspace': 0, 'wspace': 0}
 
         for key in gridspec_kwargs_default:
             if key not in gridspec_kwargs.keys():
                 gridspec_kwargs[key] = gridspec_kwargs_default[key]
 
         fig = plt.figure(constrained_layout=False, figsize=figsize)
         gs = fig.add_gridspec(3, 2, **gridspec_kwargs)
@@ -1210,17 +1213,22 @@
         # gs = gridspec.GridSpec(6, 12)
         # gs.update(wspace=0, hspace=0)
         #
         # gs0 = fig.add_gridspec(3, 2, width_ratios=[6, 1], height_ratios=[8, 1, .35],
         #                        hspace=0, wspace=0.1)
 
         # Subgridspecs
+        
+        #Let's use the same hspace/wspace if given to a user
+        
         gs_d = {}
-        gs_d['ts_scal'] = gs[0].subgridspec(2, 1, height_ratios=[1, 4], hspace=.10)
-        gs_d['psd'] = gs[1].subgridspec(2, 1, height_ratios=[1, 4], hspace=.10)
+        gs_d['ts_scal'] = gs[0].subgridspec(2, 1, height_ratios=[1, 4], hspace=gridspec_kwargs['hspace'])
+        gs_d['psd'] = gs[1].subgridspec(2, 1, height_ratios=[1, 4], hspace=gridspec_kwargs['hspace'])
+        #gs_d['ts_scal'] = gs[0].subgridspec(2, 1, height_ratios=[1, 4], hspace=.10)
+        #gs_d['psd'] = gs[1].subgridspec(2, 1, height_ratios=[1, 4], hspace=.10)
         gs_d['cb'] = gs[4].subgridspec(1, 1)
 
         ax = {}
         ### Time series
         ax['ts'] = fig.add_subplot(gs_d['ts_scal'][0, 0])
         ax['ts'] = self.plot(ax=ax['ts'], **ts_plot_kwargs)
 
@@ -1276,15 +1284,15 @@
             wavelet_plot_kwargs.update({'variable': 'amplitude'})
 
         if 'title' not in wavelet_plot_kwargs:
             wavelet_plot_kwargs.update({'title': None})
 
         if 'cbar_style' not in wavelet_plot_kwargs:
             wavelet_plot_kwargs.update({'cbar_style': {'orientation': 'horizontal', 'pad': 0.12,
-                                                       'label': wavelet_plot_kwargs['variable'].capitalize() + ' from ' + scalogram.wave_method}})
+                                                       'label': scalogram.wave_method + ' '+ wavelet_plot_kwargs['variable'].capitalize()}})
         else:
             orient = 'horizontal'
             # I think padding is now the hspace
             if 'pad' in wavelet_plot_kwargs['cbar_style']:
                 pad = wavelet_plot_kwargs['cbar_style']['pad']
             else:
                 pad = 0.12
@@ -1298,18 +1306,22 @@
         # Moving the colorbar to its own axis without leaving white space
         wavelet_plot_kwargs['cbar_style']['inset'] = True
         wavelet_plot_kwargs['cbar_style']['drawedges'] = True
 
         ax['scal'] = scalogram.plot(ax=ax['scal'], **wavelet_plot_kwargs)
 
         # pull colorbar specifications from scalogram plot
-        cbar_data = ax['scal'].figure._localaxes.__dict__['_elements'][2][1].__dict__['_colorbar'].__dict__
-
+        #cbar_data = ax['scal'].figure._localaxes.__dict__['_elements'][2][1].__dict__['_colorbar'].__dict__
+        
+        cbar_data = ax['scal'].figure._localaxes[-1]._colorbar
+        
         # remove inset colorbar (moved to its own axis below)
-        ax['scal'].figure._localaxes.__dict__['_elements'][2][1].__dict__['_colorbar'].__dict__['ax'].remove()  # clear()#remove()#.set_visible(False)
+        #ax['scal'].figure._localaxes.__dict__['_elements'][2][1].__dict__['_colorbar'].__dict__['ax'].remove()  # clear()#remove()#.set_visible(False)
+        ax['scal'].figure._localaxes[-1].remove()
+        
         if y_label_loc is not None:
             ax['scal'].get_yaxis().set_label_coords(y_label_loc, 0.5)
 
         if period_lim is not None:
             ax['scal'].set_ylim(period_lim)
             if 'ylim' in wavelet_plot_kwargs.keys():
                 print(
@@ -1382,15 +1394,15 @@
         #     ax['scal'].set_ylim(period_lim)
         #     if 'ylim' in wavelet_plot_kwargs:
         #         print('Ylim passed to psd plot through exposed argument and key word argument. The exposed argument takes precedence and will overwrite relevant key word argument.')
         # ax['scal'].invert_yaxis()
 
         ### PSD
         ax['psd'] = fig.add_subplot(gs_d['psd'][1, 0], sharey=ax['scal'])
-        ax['psd'] = psd.plot(ax=ax['psd'], transpose=True, ylabel='PSD from \n' + str(psd.spec_method),
+        ax['psd'] = psd.plot(ax=ax['psd'], transpose=True, ylabel=str(psd.spec_method) + ' PSD',
                              **psd_plot_kwargs)
 
         if period_lim is not None:
             ax['psd'].set_ylim(period_lim)
             if 'ylim' in psd_plot_kwargs:
                 print(
                     'Ylim passed to psd plot through exposed argument and key word argument. The exposed argument takes precedence and will overwrite relevant key word argument.')
@@ -1463,21 +1475,29 @@
         #
         # if psd_label is not None:
         #     ax['psd'].set_xlabel(psd_label)
         #     if 'xlabel' in psd_plot_kwargs:
         #         print('Xlabel passed to psd plot through exposed argument and key word argument. The exposed argument takes precedence and will overwrite relevant key word argument.')
 
         ax['cb'] = fig.add_subplot(gs_d['cb'][0, 0])
-        cb = mpl.colorbar.ColorbarBase(ax['cb'], orientation='horizontal',
-                                       cmap=cbar_data['cmap'],
-                                       norm=cbar_data['norm'],  # vmax and vmin
-                                       extend=cbar_data['extend'],
-                                       boundaries=cbar_data['boundaries'],  # ,
-                                       label=wavelet_plot_kwargs['cbar_style']['label'],
-                                       drawedges=cbar_data['drawedges'])  # True)
+       # cb = mpl.colorbar.ColorbarBase(ax['cb'], orientation='horizontal',
+       #                                cmap=cbar_data['cmap'],
+       #                                norm=cbar_data['norm'],  # vmax and vmin
+       #                                extend=cbar_data['extend'],
+       #                                boundaries=cbar_data['boundaries'],  # ,
+       #                                label=wavelet_plot_kwargs['cbar_style']['label'],
+       #                                drawedges=cbar_data['drawedges'])  # True)
+        
+        cb = mpl.colorbar.Colorbar(ax['cb'], mappable = cbar_data.mappable,
+                                   orientation='horizontal', 
+                                   extend=cbar_data.extend,
+                                   boundaries=cbar_data.boundaries,  # ,
+                                   label=wavelet_plot_kwargs['cbar_style']['label'],
+                                   drawedges=cbar_data.drawedges)  # True)
+        
         # ticks=[0, 3, 6, 9])
         if 'path' in savefig_settings:
             plotting.savefig(fig, settings=savefig_settings)
         return fig, ax
 
     def copy(self):
         '''Make a copy of the Series object
@@ -1542,23 +1562,22 @@
         '''
         new = self.copy()
         v_mod = tsutils.gaussianize(self.value)
         new.value = v_mod
         return new
 
     def standardize(self):
-        '''Standardizes the series ((i.e. renove its estimated mean and divides
-            by its estimated standard deviation)
+        """Standardizes the series ((i.e. remove its estimated mean and divides by its estimated standard deviation)
 
         Returns
         -------
         new : pyleoclim.Series
             The standardized series object
 
-        '''
+        """
         new = self.copy()
         v_mod = tsutils.standardize(self.value)[0]
         new.value = v_mod
         return new
 
     def center(self, timespan=None):
         ''' Centers the series (i.e. renove its estimated mean)
```

### Comparing `pyleoclim-0.9.0/pyleoclim/core/spatialdecomp.py` & `pyleoclim-0.9.1/pyleoclim/core/spatialdecomp.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/ssares.py` & `pyleoclim-0.9.1/pyleoclim/core/ssares.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/core/surrogateseries.py` & `pyleoclim-0.9.1/pyleoclim/core/surrogateseries.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_Coherence.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_Coherence.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_CorrEns.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_CorrEns.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_EnsembleSeries.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_EnsembleSeries.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_Lipd.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_Lipd.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_LipdSeries.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_LipdSeries.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_MultiplePSD.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_MultiplePSD.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_MultipleSeries.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_MultipleSeries.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_PSD.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_PSD.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_SSARes.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_SSARes.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_Scalogram.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_Scalogram.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_Series.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_Series.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/tests/test_core_SpatialDecomp.py` & `pyleoclim-0.9.1/pyleoclim/tests/test_core_SpatialDecomp.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/__init__.py` & `pyleoclim-0.9.1/pyleoclim/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/causality.py` & `pyleoclim-0.9.1/pyleoclim/utils/causality.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/correlation.py` & `pyleoclim-0.9.1/pyleoclim/utils/correlation.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/decomposition.py` & `pyleoclim-0.9.1/pyleoclim/utils/decomposition.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/filter.py` & `pyleoclim-0.9.1/pyleoclim/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/jsonutils.py` & `pyleoclim-0.9.1/pyleoclim/utils/jsonutils.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/lipdutils.py` & `pyleoclim-0.9.1/pyleoclim/utils/lipdutils.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/mapping.py` & `pyleoclim-0.9.1/pyleoclim/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/plotting.py` & `pyleoclim-0.9.1/pyleoclim/utils/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     else:
         return ax
 
 
 def plot_xy(x, y, figsize=None, xlabel=None, ylabel=None, title=None, 
             xlim=None, ylim=None,savefig_settings=None, ax=None,
             legend=True, plot_kwargs=None, lgd_kwargs=None,
-            invert_xaxis=False):
+            invert_xaxis=False, invert_yaxis=False):
     ''' Plot a timeseries
     
     Parameters
     ----------
     x : array
         The time axis for the timeseries
     y : array
@@ -229,14 +229,16 @@
     savefig_settings : dict
         the dictionary of arguments for plt.savefig(); some notes below:
         - "path" must be specified; it can be any existed or non-existed path,
           with or without a suffix; if the suffix is not given in "path", it will follow "format"
         - "format" can be one of {"pdf", "eps", "png", "ps"}
     invert_xaxis : bool, optional
         if True, the x-axis of the plot will be inverted
+    invert_yaxis : bool, optional
+        if True, the y-axis of the plot will be inverted
         
     Returns
     -------
 
     ax : the pyplot.axis object
 
     See Also
@@ -274,14 +276,17 @@
     if legend:
         ax.legend(**lgd_kwargs)
     else:
         ax.legend().remove()
 
     if invert_xaxis:
         ax.invert_xaxis()
+        
+    if invert_yaxis:
+        ax.invert_yaxis()
 
     if 'fig' in locals():
         if 'path' in savefig_settings:
             savefig(fig, settings=savefig_settings)
         return fig, ax
     else:
         return ax
@@ -297,37 +302,39 @@
 
     '''
     if fig is not None:
         plt.close(fig)
     else:
         plt.close()
 
-def savefig(fig, path=None, settings={}, verbose=True):
+def savefig(fig, path=None, dpi=300, settings={}, verbose=True):
     ''' Save a figure to a path
 
     Parameters
     ----------
     fig : matplotlib.pyplot.figure
         the figure to save
     path : str
         the path to save the figure, can be ignored and specify in "settings" instead
+    dpi : int
+        resolution in dot (pixels) per inch. Default: 300. 
     settings : dict
         the dictionary of arguments for plt.savefig(); some notes below:
         - "path" must be specified in settings if not assigned with the keyword argument;
           it can be any existed or non-existed path, with or without a suffix;
           if the suffix is not given in "path", it will follow "format"
         - "format" can be one of {"pdf", "eps", "png", "ps"}
     verbose : bool, {True,False}
         If True, print the path of the saved file.
         
     '''
     if path is None and 'path' not in settings:
         raise ValueError('"path" must be specified, either with the keyword argument or be specified in `settings`!')
 
-    savefig_args = {'bbox_inches': 'tight', 'path': path}
+    savefig_args = {'bbox_inches': 'tight', 'path': path, 'dpi': dpi}
     savefig_args.update(settings)
 
     path = pathlib.Path(savefig_args['path'])
     savefig_args.pop('path')
 
     dirpath = path.parent
     if not dirpath.exists():
@@ -342,15 +349,15 @@
     fig.savefig(path_str, **savefig_args)
     plt.close(fig)
 
     if verbose:
         print(f'Figure saved at: "{str(path)}"')
 
 
-def set_style(style='journal', font_scale=1.0):
+def set_style(style='journal', font_scale=1.0, dpi=300):
     ''' Modify the visualization style
     
     This function is inspired by [Seaborn](https://github.com/mwaskom/seaborn).
    
     
     Parameters
     ----------
@@ -469,18 +476,22 @@
             'axes.grid': True,
         })
     elif '_nogrid' in style:
         style_dict.update({
             'axes.grid': False,
         })
 
+    figure_dict = {
+        'savefig.dpi': dpi,
+    }
+
     # modify font size based on font scale
     font_dict.update({k: v * font_scale for k, v in font_dict.items()})
 
-    for d in [style_dict, font_dict]:
+    for d in [style_dict, font_dict, figure_dict]:
         mpl.rcParams.update(d)
```

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/spectral.py` & `pyleoclim-0.9.1/pyleoclim/utils/spectral.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
                  detrend = None, sg_kwargs=None,
                  gaussianize=False,
                  standardize=True,
                  average='mean'):
     """ Lomb-scargle priodogram
 
     Appropriate for unevenly-spaced arrays.
-    Uses the lomb-scargle implementation from scipy.signal: https://scipy.github.io/devdocs/generated/scipy.signal.lombscargle.html#scipy.signal.lombscargle
+    Uses the lomb-scargle implementation from scipy.signal: https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.lombscargle.html
 
     Parameters
     ----------
 
     ys : array
         a time series
     ts : array
```

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/tsbase.py` & `pyleoclim-0.9.1/pyleoclim/utils/tsbase.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/tsmodel.py` & `pyleoclim-0.9.1/pyleoclim/utils/tsmodel.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/tsutils.py` & `pyleoclim-0.9.1/pyleoclim/utils/tsutils.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim/utils/wavelet.py` & `pyleoclim-0.9.1/pyleoclim/utils/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/pyleoclim.egg-info/PKG-INFO` & `pyleoclim-0.9.1/pyleoclim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: pyleoclim
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Python package for paleoclimate data analysis
 Home-page: https://github.com/LinkedEarth/Pyleoclim_util/pyleoclim
+Download-URL: https://github.com/LinkedEarth/Pyleoclim_util/tarball/0.9.1
 Author: Deborah Khider, Feng Zhu, Julien Emile-Geay, Jun Hu, Myron Kwan, Pratheek Athreya, Alexander James, Daniel Garijo
 Author-email: linkedearth@gmail.com
 License: GPL-3.0 License
-Download-URL: https://github.com/LinkedEarth/Pyleoclim_util/tarball/0.9.0
 Keywords: Paleoclimate, Data Analysis, LiPD
-Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 
 <!---[![PyPI](https://img.shields.io/pypi/dm/pyleoclim.svg)](https://pypi.python.org/pypi/Pyleoclim)-->
 [![PyPI version](https://badge.fury.io/py/pyleoclim.svg)](https://badge.fury.io/py/pyleoclim)
 [![PyPI](https://img.shields.io/badge/python-3.9-yellow.svg)]()
 [![license](https://img.shields.io/github/license/linkedearth/Pyleoclim_util.svg)]()
-[![DOI](https://zenodo.org/badge/59611213.svg)](https://zenodo.org/badge/latestdoi/59611213)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6999279.svg)](https://doi.org/10.5281/zenodo.6999279)
 [![NSF-1541029](https://img.shields.io/badge/NSF-1541029-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1541029)
 [![Build Status](https://travis-ci.org/LinkedEarth/Pyleoclim_util.svg?branch=master)](https://travis-ci.org/LinkedEarth/Pyleoclim_util)
 
 ![](https://github.com/LinkedEarth/Logos/raw/master/pyleoclim_logo_full_white.png)
 
 **Python Package for the Analysis of Paleoclimate Data**
 
-Paleoclimate data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.
+[Paleoclimate](https://www.ncdc.noaa.gov/news/what-paleoclimatology) data, whether from observations or model simulations, offer unique challenges to the analyst, as they usually come in the form of timeseries with missing values and age uncertainties, which trip up off-the-shelf methods.
 Pyleoclim is a Python package primarily geared towards the analysis and visualization of such timeseries. The package includes several low-level methods to deal with these issues under the hood, leaving paleoscientists to interact with intuitive, high-level analysis and plotting methods that support publication-quality scientific workflows.
 
 There are many entry points to Pyleoclim, thanks to its underlying [data structures](https://pyleoclim-util.readthedocs.io/en/master/core/ui.html). The package leverages the Linked Paleo Data ([LiPD](http://www.clim-past.net/12/1093/2016/)) standard container and its associated [utilities](http://nickmckay.github.io/LiPD-utilities/). The package is aware of age ensembles stored via LiPD and uses them for time-uncertain analyses, very much like its R sidekick, [GeoChronR](https://doi.org/10.5194/gchron-2020-25).
 
 LiPD is not an obligatory entry point to Pyleoclim. Low-level modules work on [NumPy](http://www.numpy.org) arrays or [Pandas](https://pandas.pydata.org) dataframes, so most Pyleoclim timeseries analysis functionalities can apply to these more common types as well, including those generated by numerical models (via [xarray](http://xarray.pydata.org)). This makes the package suitable for rigorous and efficient model-data comparisons, like [this one](https://www.pnas.org/content/116/18/8728.short).
 
-We've worked very hard to make Pyleoclim accessible to a wide variety of users, from establisher researchers to high-school students, and from seasoned Pythonistas to first-time programmers. A growing collection of workflows that use Pyleoclim are available as Jupyter notebooks on [paleoBooks](https://github.com/LinkedEarth/PaleoBooks/tree/master/notebooks), with video tutorials on the LinkedEarth [YouTube channel](https://www.youtube.com/watch?v=LJaQBFMK2-Q&list=PL93NbaRnKAuF4WpIQf-4y_U4lo-GqcrcW). Python novices are encouraged to follow these [self-paced tutorials](http://linked.earth/ec_workshops_py/) before trying Pyleoclim.
+We've worked very hard to make Pyleoclim accessible to a wide variety of users, from establisher researchers to high-school students, and from seasoned Pythonistas to first-time programmers. A progressive introduction to the package is available at [PyleoTutorials](http://linked.earth/PyleoTutorials/) A growing collection of research-grade workflows using Pyleoclim and the LinkedEarth research ecosystem are available as Jupyter notebooks on [paleoBooks](https://github.com/LinkedEarth/PaleoBooks/tree/master/notebooks), with video tutorials on the LinkedEarth [YouTube channel](https://www.youtube.com/watch?v=LJaQBFMK2-Q&list=PL93NbaRnKAuF4WpIQf-4y_U4lo-GqcrcW). Python novices are encouraged to follow these [self-paced tutorials](http://linked.earth/ec_workshops_py/) before trying Pyleoclim.
 
 Science-based training materials are also available from the [paleoHackathon repository](https://github.com/LinkedEarth/paleoHackathon). You can run these training notebooks at any time in a myBinder environment. We also run live training workshops several times a year. Follow us on [Twitter](https://twitter.com/Linked_Earth), or join our [Discourse Forum](https://discourse.linked.earth) for more information.
 
 ### Versions
 
 See our [releases page](https://github.com/LinkedEarth/Pyleoclim_util/releases) for details on what's included in each version.
 
@@ -60,19 +59,15 @@
 
 Please submit any reproducible bugs you encounter to the [issue tracker](https://github.com/LinkedEarth/Pyleoclim_util/issues). For usage questions, please use [Discourse](https://discourse.linked.earth).
 
 
 ### License
 
 The project is licensed under the GNU Public License. Please refer to the file call license.
-If you use the code in publications, please credit the work using this citation:
-
-_Deborah Khider, Feng Zhu, Julien Emile-Geay, Jun Hu, Alexander James, Pratheek Athreya, Myron Kwan, Daniel Garijo. (xxxx). Pyleoclim: vx.x.x Release. Zenodo. http://doi.org/10.5281/zenodo.1212692_
+If you use the code in publications, please credit the work using the citation file. 
 
 
 ### Disclaimer
 
 This material is based upon work supported by the National Science Foundation under Grant Number ICER-1541029. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the investigators and do not necessarily reflect the views of the National Science Foundation.
 
 This research is funded in part by JP Morgan Chase & Co. Any views or opinions expressed herein are solely those of the authors listed, and may differ from the views and opinions expressed by JP Morgan Chase & Co. or its affilitates. This material is not a product of the Research Department of J.P. Morgan Securities LLC. This material should not be construed as an individual recommendation of for any particular client and is not intended as a recommendation of particular securities, financial instruments or strategies for a particular client. This material does not constitute a solicitation or offer in any jurisdiction.
-
-
```

### Comparing `pyleoclim-0.9.0/pyleoclim.egg-info/SOURCES.txt` & `pyleoclim-0.9.1/pyleoclim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyleoclim-0.9.0/setup.py` & `pyleoclim-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import io
 
 from setuptools import setup, find_packages
 
 
-version = '0.9.0'
+version = '0.9.1'
 
 # Read the readme file contents into variable
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='pyleoclim',
@@ -26,25 +26,25 @@
     url='https://github.com/LinkedEarth/Pyleoclim_util/pyleoclim',
     download_url='https://github.com/LinkedEarth/Pyleoclim_util/tarball/'+version,
     keywords=['Paleoclimate, Data Analysis, LiPD'],
     classifiers=[],
     install_requires=[
         "LiPD==0.2.8.8",
         "pandas>=1.3.0",
-        "numpy==1.22.0",
-        "matplotlib>=3.5.1",
-        "scipy>=1.7.0",
-        "statsmodels>=0.11.1",
-        "seaborn>=0.11",
+        "numpy<=1.24.0",
+        "matplotlib>=3.6.0",
+        "scipy>=1.9.1",
+        "statsmodels>=0.13.2",
+        "seaborn>=0.12.0",
         "scikit-learn>=0.24.2",
-        "pathos>=0.2.6",
-        "tqdm>=4.47.0",
-        "tftb>=0.1.1",
+        "pathos>=0.2.8",
+        "tqdm>=4.61.2",
+        "tftb>=0.1.3",
         "pyhht>=0.1.0",
         "wget>=3.2",
-        "numba>=0.50.1",
-        "nitime>=0.8.1",
-        "tabulate>=0.8.7",
+        "numba>=0.56",
+        "nitime>=0.9",
+        "tabulate>=0.8.9",
         "Unidecode>=1.1.1",
     ],
     python_requires=">=3.8.0"
 )
```

