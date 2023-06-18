# Comparing `tmp/sdevpy-0.0.6.tar.gz` & `tmp/sdevpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.0.6.tar", last modified: Sun Jun 18 03:45:37 2023, max compression
+gzip compressed data, was "sdevpy-0.0.7.tar", last modified: Sun Jun 18 05:27:41 2023, max compression
```

## Comparing `sdevpy-0.0.6.tar` & `sdevpy-0.0.7.tar`

### file list

```diff
@@ -1,71 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.285594 sdevpy-0.0.6/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      854 2023-06-18 03:45:37.284594 sdevpy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-17 04:46:40.000000 sdevpy-0.0.6/README.md
--rw-rw-rw-   0        0        0      643 2023-06-18 03:45:14.000000 sdevpy-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 03:45:37.285594 sdevpy-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.159635 sdevpy-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.177628 sdevpy-0.0.6/src/sdevpy/
--rw-rw-rw-   0        0        0       14 2023-06-18 03:29:43.000000 sdevpy-0.0.6/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.210618 sdevpy-0.0.6/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/analytics/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.6/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.6/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.6/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.6/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.6/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.6/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.6/src/sdevpy/analytics/sabr.py
--rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.6/src/sdevpy/example.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.219615 sdevpy-0.0.6/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/machinelearning/__init__.py
--rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.6/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.6/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.6/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.6/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.6/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.234611 sdevpy-0.0.6/src/sdevpy/maths/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/maths/__init__.py
--rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.6/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.6/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.6/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.6/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.237611 sdevpy-0.0.6/src/sdevpy/projects/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/projects/__init__.py
--rw-rw-rw-   0        0        0      874 2023-06-16 04:17:05.000000 sdevpy-0.0.6/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.245608 sdevpy-0.0.6/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/projects/pinns/__init__.py
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.6/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.6/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.6/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.254604 sdevpy-0.0.6/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/projects/stovol/__init__.py
--rw-rw-rw-   0        0        0     2480 2023-06-16 13:01:52.000000 sdevpy-0.0.6/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.6/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.6/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.6/src/sdevpy/projects/stovol/xsabrfit.py
--rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.6/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.6/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.266599 sdevpy-0.0.6/src/sdevpy/tools/
--rw-rw-rw-   0        0        0      210 2023-06-18 03:08:12.000000 sdevpy-0.0.6/src/sdevpy/tools/__init__.py
--rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.6/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.6/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.6/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.6/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.6/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.6/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.282594 sdevpy-0.0.6/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/__init__.py
--rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     2083 2023-06-11 09:18:49.000000 sdevpy-0.0.6/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-18 03:45:37.195624 sdevpy-0.0.6/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0      854 2023-06-18 03:45:37.000000 sdevpy-0.0.6/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1914 2023-06-18 03:45:37.000000 sdevpy-0.0.6/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 03:45:37.000000 sdevpy-0.0.6/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 03:45:37.000000 sdevpy-0.0.6/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 03:45:37.000000 sdevpy-0.0.6/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.821164 sdevpy-0.0.7/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      854 2023-06-18 05:27:41.821164 sdevpy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-17 04:46:40.000000 sdevpy-0.0.7/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-18 05:26:58.000000 sdevpy-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 05:27:41.821164 sdevpy-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.321326 sdevpy-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.366312 sdevpy-0.0.7/src/sdevpy/
+-rw-rw-rw-   0        0        0       35 2023-06-18 03:49:31.000000 sdevpy-0.0.7/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.444286 sdevpy-0.0.7/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.7/src/sdevpy/analytics/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.7/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.7/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.7/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.7/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.7/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.7/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.7/src/sdevpy/analytics/sabr.py
+-rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.7/src/sdevpy/example.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.487272 sdevpy-0.0.7/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.7/src/sdevpy/machinelearning/__init__.py
+-rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.7/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.7/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.7/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.7/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.7/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.552252 sdevpy-0.0.7/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.7/src/sdevpy/maths/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.7/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.7/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.7/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.7/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.557249 sdevpy-0.0.7/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0      888 2023-06-18 05:26:29.000000 sdevpy-0.0.7/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.627228 sdevpy-0.0.7/src/sdevpy/projects/pinns/
+-rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.7/src/sdevpy/projects/pinns/ernst_pinns.py
+-rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.7/src/sdevpy/projects/pinns/pinns.py
+-rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.7/src/sdevpy/projects/pinns/pinns_worst_of.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.678210 sdevpy-0.0.7/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0     2480 2023-06-16 13:01:52.000000 sdevpy-0.0.7/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.7/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.7/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.7/src/sdevpy/projects/stovol/xsabrfit.py
+-rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.7/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.7/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.746188 sdevpy-0.0.7/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.7/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.7/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.7/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.7/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.7/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.7/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.817166 sdevpy-0.0.7/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/__init__.py
+-rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     2083 2023-06-11 09:18:49.000000 sdevpy-0.0.7/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.394302 sdevpy-0.0.7/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0      854 2023-06-18 05:27:41.000000 sdevpy-0.0.7/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1790 2023-06-18 05:27:41.000000 sdevpy-0.0.7/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 05:27:41.000000 sdevpy-0.0.7/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-18 05:27:41.000000 sdevpy-0.0.7/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 05:27:41.000000 sdevpy-0.0.7/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 05:27:41.819166 sdevpy-0.0.7/tests/
+-rw-rw-rw-   0        0        0      164 2023-06-18 03:57:12.000000 sdevpy-0.0.7/tests/test.py
```

### Comparing `sdevpy-0.0.6/LICENSE` & `sdevpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/PKG-INFO` & `sdevpy-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.0.6/pyproject.toml` & `sdevpy-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.0.7/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/black.py` & `sdevpy-0.0.7/src/sdevpy/analytics/black.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.0.7/src/sdevpy/analytics/fbsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.0.7/src/sdevpy/analytics/mcheston.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.0.7/src/sdevpy/analytics/mcsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.0.7/src/sdevpy/analytics/mczabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/analytics/sabr.py` & `sdevpy-0.0.7/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.0.7/src/sdevpy/machinelearning/callbacks.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/machinelearning/datasets.py` & `sdevpy-0.0.7/src/sdevpy/machinelearning/datasets.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.0.7/src/sdevpy/machinelearning/learningmodel.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.0.7/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.0.7/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/maths/interpolations.py` & `sdevpy-0.0.7/src/sdevpy/maths/interpolations.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/maths/rand.py` & `sdevpy-0.0.7/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/datafiles.py` & `sdevpy-0.0.7/src/sdevpy/projects/datafiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Operations on data files e.g. merging, etc. """
 import os
 import pandas as pd
-from tools import filemanager
-import settings
+from sdevpy.tools import filemanager
+import sdevpy.settings
 
 
 def merge_tsv(path, shuffle=False):
     """ Merge all .tsv files into one, assuming they all have the same structure """
     merged_file = os.path.join(path, "merged.tsv")
     if os.path.exists(merged_file):
         print("removing file: " + merged_file)
```

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/pinns/ernst_pinns.py` & `sdevpy-0.0.7/src/sdevpy/projects/pinns/ernst_pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/pinns/pinns.py` & `sdevpy-0.0.7/src/sdevpy/projects/pinns/pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/pinns/pinns_worst_of.py` & `sdevpy-0.0.7/src/sdevpy/projects/pinns/pinns_worst_of.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.0.7/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/stovol/stovolplot.py` & `sdevpy-0.0.7/src/sdevpy/projects/stovol/stovolplot.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.0.7/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/projects/stovol/xsabrfit.py` & `sdevpy-0.0.7/src/sdevpy/projects/stovol/xsabrfit.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/test.py` & `sdevpy-0.0.7/src/sdevpy/test.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/tools/clipboard.py` & `sdevpy-0.0.7/src/sdevpy/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/tools/filemanager.py` & `sdevpy-0.0.7/src/sdevpy/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.0.7/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/tools/timegrids.py` & `sdevpy-0.0.7/src/sdevpy/tools/timegrids.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/tools/timer.py` & `sdevpy-0.0.7/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/fbsabrgenerator.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/fbsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/mcsabrgenerator.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/mcsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/mczabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/sabrgenerator.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.0.7/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.6/src/sdevpy.egg-info/PKG-INFO` & `sdevpy-0.0.7/src/sdevpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.0.6/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.0.7/src/sdevpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,33 +25,30 @@
 src/sdevpy/machinelearning/learningschedules.py
 src/sdevpy/machinelearning/topology.py
 src/sdevpy/maths/__init__.py
 src/sdevpy/maths/interpolations.py
 src/sdevpy/maths/metrics.py
 src/sdevpy/maths/optimization.py
 src/sdevpy/maths/rand.py
-src/sdevpy/projects/__init__.py
 src/sdevpy/projects/datafiles.py
-src/sdevpy/projects/pinns/__init__.py
 src/sdevpy/projects/pinns/ernst_pinns.py
 src/sdevpy/projects/pinns/pinns.py
 src/sdevpy/projects/pinns/pinns_worst_of.py
-src/sdevpy/projects/stovol/__init__.py
 src/sdevpy/projects/stovol/stovolgen.py
 src/sdevpy/projects/stovol/stovolplot.py
 src/sdevpy/projects/stovol/stovoltrain.py
 src/sdevpy/projects/stovol/xsabrfit.py
-src/sdevpy/tools/__init__.py
 src/sdevpy/tools/clipboard.py
 src/sdevpy/tools/constants.py
 src/sdevpy/tools/filemanager.py
 src/sdevpy/tools/jsonmanager.py
 src/sdevpy/tools/timegrids.py
 src/sdevpy/tools/timer.py
 src/sdevpy/volsurfacegen/__init__.py
 src/sdevpy/volsurfacegen/fbsabrgenerator.py
 src/sdevpy/volsurfacegen/mchestongenerator.py
 src/sdevpy/volsurfacegen/mcsabrgenerator.py
 src/sdevpy/volsurfacegen/mczabrgenerator.py
 src/sdevpy/volsurfacegen/sabrgenerator.py
 src/sdevpy/volsurfacegen/smilegenerator.py
-src/sdevpy/volsurfacegen/stovolfactory.py
+src/sdevpy/volsurfacegen/stovolfactory.py
+tests/test.py
```

