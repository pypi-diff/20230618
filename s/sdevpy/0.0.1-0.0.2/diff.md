# Comparing `tmp/sdevpy-0.0.1.tar.gz` & `tmp/sdevpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.0.1.tar", last modified: Sun Jun 18 01:36:42 2023, max compression
+gzip compressed data, was "sdevpy-0.0.2.tar", last modified: Sun Jun 18 02:46:00 2023, max compression
```

## Comparing `sdevpy-0.0.1.tar` & `sdevpy-0.0.2.tar`

### file list

```diff
@@ -1,63 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:42.215469 sdevpy-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      854 2023-06-18 01:36:42.214469 sdevpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-17 04:46:40.000000 sdevpy-0.0.1/README.md
--rw-rw-rw-   0        0        0      632 2023-06-18 01:32:31.000000 sdevpy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 01:36:42.215469 sdevpy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.416729 sdevpy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.485708 sdevpy-0.0.1/src/sdevpy/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.1/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.742624 sdevpy-0.0.1/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.1/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.1/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.1/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.1/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.1/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.1/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.1/src/sdevpy/analytics/sabr.py
--rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.1/src/sdevpy/example.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.791609 sdevpy-0.0.1/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.1/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.1/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.1/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.1/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.1/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.896575 sdevpy-0.0.1/src/sdevpy/maths/
--rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.1/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.1/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.1/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.1/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.933560 sdevpy-0.0.1/src/sdevpy/projects/
--rw-rw-rw-   0        0        0      874 2023-06-16 04:17:05.000000 sdevpy-0.0.1/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.966553 sdevpy-0.0.1/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.1/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.1/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.1/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:42.022533 sdevpy-0.0.1/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0     2480 2023-06-16 13:01:52.000000 sdevpy-0.0.1/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.1/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.1/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.1/src/sdevpy/projects/stovol/xsabrfit.py
--rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.1/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.1/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:42.080513 sdevpy-0.0.1/src/sdevpy/tools/
--rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.1/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.1/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.1/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.1/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.1/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.1/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:42.212470 sdevpy-0.0.1/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     2083 2023-06-11 09:18:49.000000 sdevpy-0.0.1/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:36:41.537694 sdevpy-0.0.1/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0      854 2023-06-18 01:36:41.000000 sdevpy-0.0.1/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2023-06-18 01:36:41.000000 sdevpy-0.0.1/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 01:36:41.000000 sdevpy-0.0.1/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 01:36:41.000000 sdevpy-0.0.1/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 01:36:41.000000 sdevpy-0.0.1/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.849967 sdevpy-0.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      854 2023-06-18 02:46:00.848970 sdevpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-17 04:46:40.000000 sdevpy-0.0.2/README.md
+-rw-rw-rw-   0        0        0      632 2023-06-18 02:45:30.000000 sdevpy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 02:46:00.849967 sdevpy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.544067 sdevpy-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.565060 sdevpy-0.0.2/src/sdevpy/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.684021 sdevpy-0.0.2/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/analytics/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.2/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.2/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.2/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.2/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.2/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.2/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.2/src/sdevpy/analytics/sabr.py
+-rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.2/src/sdevpy/example.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.736005 sdevpy-0.0.2/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/machinelearning/__init__.py
+-rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.2/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.2/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.2/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.2/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.2/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.772995 sdevpy-0.0.2/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/maths/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.2/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.2/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.2/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.2/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.775992 sdevpy-0.0.2/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/projects/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-06-16 04:17:05.000000 sdevpy-0.0.2/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.794986 sdevpy-0.0.2/src/sdevpy/projects/pinns/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/projects/pinns/__init__.py
+-rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.2/src/sdevpy/projects/pinns/ernst_pinns.py
+-rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.2/src/sdevpy/projects/pinns/pinns.py
+-rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.2/src/sdevpy/projects/pinns/pinns_worst_of.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.809981 sdevpy-0.0.2/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/projects/stovol/__init__.py
+-rw-rw-rw-   0        0        0     2480 2023-06-16 13:01:52.000000 sdevpy-0.0.2/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.2/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.2/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.2/src/sdevpy/projects/stovol/xsabrfit.py
+-rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.2/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.2/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.820978 sdevpy-0.0.2/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/tools/__init__.py
+-rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.2/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.2/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.2/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.2/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.2/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.2/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.847969 sdevpy-0.0.2/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/__init__.py
+-rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     2083 2023-06-11 09:18:49.000000 sdevpy-0.0.2/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:46:00.670026 sdevpy-0.0.2/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0      854 2023-06-18 02:46:00.000000 sdevpy-0.0.2/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1914 2023-06-18 02:46:00.000000 sdevpy-0.0.2/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 02:46:00.000000 sdevpy-0.0.2/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 02:46:00.000000 sdevpy-0.0.2/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 02:46:00.000000 sdevpy-0.0.2/src/sdevpy.egg-info/top_level.txt
```

### Comparing `sdevpy-0.0.1/LICENSE` & `sdevpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/PKG-INFO` & `sdevpy-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.0.1/pyproject.toml` & `sdevpy-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.0.2/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/black.py` & `sdevpy-0.0.2/src/sdevpy/analytics/black.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.0.2/src/sdevpy/analytics/fbsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.0.2/src/sdevpy/analytics/mcheston.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.0.2/src/sdevpy/analytics/mcsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.0.2/src/sdevpy/analytics/mczabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/analytics/sabr.py` & `sdevpy-0.0.2/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.0.2/src/sdevpy/machinelearning/callbacks.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/machinelearning/datasets.py` & `sdevpy-0.0.2/src/sdevpy/machinelearning/datasets.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.0.2/src/sdevpy/machinelearning/learningmodel.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.0.2/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.0.2/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/maths/interpolations.py` & `sdevpy-0.0.2/src/sdevpy/maths/interpolations.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/maths/rand.py` & `sdevpy-0.0.2/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/datafiles.py` & `sdevpy-0.0.2/src/sdevpy/projects/datafiles.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/pinns/ernst_pinns.py` & `sdevpy-0.0.2/src/sdevpy/projects/pinns/ernst_pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/pinns/pinns.py` & `sdevpy-0.0.2/src/sdevpy/projects/pinns/pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/pinns/pinns_worst_of.py` & `sdevpy-0.0.2/src/sdevpy/projects/pinns/pinns_worst_of.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.0.2/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/stovol/stovolplot.py` & `sdevpy-0.0.2/src/sdevpy/projects/stovol/stovolplot.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.0.2/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/projects/stovol/xsabrfit.py` & `sdevpy-0.0.2/src/sdevpy/projects/stovol/xsabrfit.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/test.py` & `sdevpy-0.0.2/src/sdevpy/test.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/tools/clipboard.py` & `sdevpy-0.0.2/src/sdevpy/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/tools/filemanager.py` & `sdevpy-0.0.2/src/sdevpy/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.0.2/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/tools/timegrids.py` & `sdevpy-0.0.2/src/sdevpy/tools/timegrids.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/tools/timer.py` & `sdevpy-0.0.2/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/fbsabrgenerator.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/fbsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/mcsabrgenerator.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/mcsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/mczabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/sabrgenerator.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.0.2/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.1/src/sdevpy.egg-info/PKG-INFO` & `sdevpy-0.0.2/src/sdevpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.0.1/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.0.2/src/sdevpy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,52 @@
 src/sdevpy/settings.py
 src/sdevpy/test.py
 src/sdevpy.egg-info/PKG-INFO
 src/sdevpy.egg-info/SOURCES.txt
 src/sdevpy.egg-info/dependency_links.txt
 src/sdevpy.egg-info/requires.txt
 src/sdevpy.egg-info/top_level.txt
+src/sdevpy/analytics/__init__.py
 src/sdevpy/analytics/bachelier.py
 src/sdevpy/analytics/black.py
 src/sdevpy/analytics/fbsabr.py
 src/sdevpy/analytics/mcheston.py
 src/sdevpy/analytics/mcsabr.py
 src/sdevpy/analytics/mczabr.py
 src/sdevpy/analytics/sabr.py
+src/sdevpy/machinelearning/__init__.py
 src/sdevpy/machinelearning/callbacks.py
 src/sdevpy/machinelearning/datasets.py
 src/sdevpy/machinelearning/learningmodel.py
 src/sdevpy/machinelearning/learningschedules.py
 src/sdevpy/machinelearning/topology.py
+src/sdevpy/maths/__init__.py
 src/sdevpy/maths/interpolations.py
 src/sdevpy/maths/metrics.py
 src/sdevpy/maths/optimization.py
 src/sdevpy/maths/rand.py
+src/sdevpy/projects/__init__.py
 src/sdevpy/projects/datafiles.py
+src/sdevpy/projects/pinns/__init__.py
 src/sdevpy/projects/pinns/ernst_pinns.py
 src/sdevpy/projects/pinns/pinns.py
 src/sdevpy/projects/pinns/pinns_worst_of.py
+src/sdevpy/projects/stovol/__init__.py
 src/sdevpy/projects/stovol/stovolgen.py
 src/sdevpy/projects/stovol/stovolplot.py
 src/sdevpy/projects/stovol/stovoltrain.py
 src/sdevpy/projects/stovol/xsabrfit.py
+src/sdevpy/tools/__init__.py
 src/sdevpy/tools/clipboard.py
 src/sdevpy/tools/constants.py
 src/sdevpy/tools/filemanager.py
 src/sdevpy/tools/jsonmanager.py
 src/sdevpy/tools/timegrids.py
 src/sdevpy/tools/timer.py
+src/sdevpy/volsurfacegen/__init__.py
 src/sdevpy/volsurfacegen/fbsabrgenerator.py
 src/sdevpy/volsurfacegen/mchestongenerator.py
 src/sdevpy/volsurfacegen/mcsabrgenerator.py
 src/sdevpy/volsurfacegen/mczabrgenerator.py
 src/sdevpy/volsurfacegen/sabrgenerator.py
 src/sdevpy/volsurfacegen/smilegenerator.py
 src/sdevpy/volsurfacegen/stovolfactory.py
```

