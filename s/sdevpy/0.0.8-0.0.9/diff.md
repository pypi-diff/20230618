# Comparing `tmp/sdevpy-0.0.8.tar.gz` & `tmp/sdevpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.0.8.tar", last modified: Sun Jun 18 05:57:27 2023, max compression
+gzip compressed data, was "sdevpy-0.0.9.tar", last modified: Sun Jun 18 08:28:58 2023, max compression
```

## Comparing `sdevpy-0.0.8.tar` & `sdevpy-0.0.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.665924 sdevpy-0.0.8/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      854 2023-06-18 05:57:27.665924 sdevpy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-06-17 04:46:40.000000 sdevpy-0.0.8/README.md
--rw-rw-rw-   0        0        0      643 2023-06-18 05:37:58.000000 sdevpy-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 05:57:27.665924 sdevpy-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.551961 sdevpy-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.566956 sdevpy-0.0.8/src/sdevpy/
--rw-rw-rw-   0        0        0        0 2023-06-18 05:31:15.000000 sdevpy-0.0.8/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.601946 sdevpy-0.0.8/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.8/src/sdevpy/analytics/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.8/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.8/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.8/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.8/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.8/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.8/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.8/src/sdevpy/analytics/sabr.py
--rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.8/src/sdevpy/example.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.612941 sdevpy-0.0.8/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.8/src/sdevpy/machinelearning/__init__.py
--rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.8/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.8/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.8/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.8/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.8/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.620940 sdevpy-0.0.8/src/sdevpy/maths/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.8/src/sdevpy/maths/__init__.py
--rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.8/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.8/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.8/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.8/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.622938 sdevpy-0.0.8/src/sdevpy/projects/
--rw-rw-rw-   0        0        0      888 2023-06-18 05:26:29.000000 sdevpy-0.0.8/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.629935 sdevpy-0.0.8/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.8/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.8/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.8/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.636933 sdevpy-0.0.8/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0     2508 2023-06-18 05:56:21.000000 sdevpy-0.0.8/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.8/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.8/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.8/src/sdevpy/projects/stovol/xsabrfit.py
--rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.8/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.8/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.647930 sdevpy-0.0.8/src/sdevpy/tools/
--rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.8/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.8/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.8/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.8/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.8/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.8/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.662925 sdevpy-0.0.8/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     2083 2023-06-11 09:18:49.000000 sdevpy-0.0.8/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.583951 sdevpy-0.0.8/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0      854 2023-06-18 05:57:27.000000 sdevpy-0.0.8/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1753 2023-06-18 05:57:27.000000 sdevpy-0.0.8/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 05:57:27.000000 sdevpy-0.0.8/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 05:57:27.000000 sdevpy-0.0.8/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 05:57:27.000000 sdevpy-0.0.8/src/sdevpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 05:57:27.663924 sdevpy-0.0.8/tests/
--rw-rw-rw-   0        0        0      164 2023-06-18 03:57:12.000000 sdevpy-0.0.8/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.105496 sdevpy-0.0.9/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1725 2023-06-18 08:28:58.104497 sdevpy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.0.9/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-18 08:25:52.000000 sdevpy-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 08:28:58.105496 sdevpy-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:57.942550 sdevpy-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:57.956544 sdevpy-0.0.9/src/sdevpy/
+-rw-rw-rw-   0        0        0       21 2023-06-18 08:28:32.000000 sdevpy-0.0.9/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.030521 sdevpy-0.0.9/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.9/src/sdevpy/analytics/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.9/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.9/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.9/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.9/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.9/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.9/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.9/src/sdevpy/analytics/sabr.py
+-rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.9/src/sdevpy/example.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.043517 sdevpy-0.0.9/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/__init__.py
+-rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.051514 sdevpy-0.0.9/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.9/src/sdevpy/maths/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.9/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.9/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.9/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.9/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.052513 sdevpy-0.0.9/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0      888 2023-06-18 05:26:29.000000 sdevpy-0.0.9/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.064510 sdevpy-0.0.9/src/sdevpy/projects/pinns/
+-rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.9/src/sdevpy/projects/pinns/ernst_pinns.py
+-rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns.py
+-rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns_worst_of.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.081505 sdevpy-0.0.9/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0     2508 2023-06-18 05:56:21.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/xsabrfit.py
+-rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.9/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.9/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.091502 sdevpy-0.0.9/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.9/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.9/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.9/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.9/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.9/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.9/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.101498 sdevpy-0.0.9/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     2118 2023-06-18 08:25:27.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.003530 sdevpy-0.0.9/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0     1725 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1753 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.103497 sdevpy-0.0.9/tests/
+-rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.0.9/tests/test.py
```

### Comparing `sdevpy-0.0.8/LICENSE` & `sdevpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/pyproject.toml` & `sdevpy-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.0.9/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/black.py` & `sdevpy-0.0.9/src/sdevpy/analytics/black.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.0.9/src/sdevpy/analytics/fbsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.0.9/src/sdevpy/analytics/mcheston.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.0.9/src/sdevpy/analytics/mcsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.0.9/src/sdevpy/analytics/mczabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/analytics/sabr.py` & `sdevpy-0.0.9/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.0.9/src/sdevpy/machinelearning/callbacks.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/machinelearning/datasets.py` & `sdevpy-0.0.9/src/sdevpy/machinelearning/datasets.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.0.9/src/sdevpy/machinelearning/learningmodel.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.0.9/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.0.9/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/maths/interpolations.py` & `sdevpy-0.0.9/src/sdevpy/maths/interpolations.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/maths/rand.py` & `sdevpy-0.0.9/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/datafiles.py` & `sdevpy-0.0.9/src/sdevpy/projects/datafiles.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/pinns/ernst_pinns.py` & `sdevpy-0.0.9/src/sdevpy/projects/pinns/ernst_pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/pinns/pinns.py` & `sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/pinns/pinns_worst_of.py` & `sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns_worst_of.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/stovol/stovolplot.py` & `sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolplot.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.0.9/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/projects/stovol/xsabrfit.py` & `sdevpy-0.0.9/src/sdevpy/projects/stovol/xsabrfit.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/test.py` & `sdevpy-0.0.9/src/sdevpy/test.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/tools/clipboard.py` & `sdevpy-0.0.9/src/sdevpy/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/tools/filemanager.py` & `sdevpy-0.0.9/src/sdevpy/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.0.9/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/tools/timegrids.py` & `sdevpy-0.0.9/src/sdevpy/tools/timegrids.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/tools/timer.py` & `sdevpy-0.0.9/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/fbsabrgenerator.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/fbsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/mcsabrgenerator.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/mcsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/mczabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/sabrgenerator.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.8/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.0.9/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Select stovol generator based on type and other required information """
-from volsurfacegen.sabrgenerator import SabrGenerator, ShiftedSabrGenerator
-from volsurfacegen.mcsabrgenerator import McShiftedSabrGenerator
-from volsurfacegen.fbsabrgenerator import FbSabrGenerator
-from volsurfacegen.mczabrgenerator import McShiftedZabrGenerator
-from volsurfacegen.mchestongenerator import McShiftedHestonGenerator
+from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator, ShiftedSabrGenerator
+from sdevpy.volsurfacegen.mcsabrgenerator import McShiftedSabrGenerator
+from sdevpy.volsurfacegen.fbsabrgenerator import FbSabrGenerator
+from sdevpy.volsurfacegen.mczabrgenerator import McShiftedZabrGenerator
+from sdevpy.volsurfacegen.mchestongenerator import McShiftedHestonGenerator
 
 
 def set_generator(type_, num_expiries=10, surface_size=50, num_mc=100000,
                   points_per_year=25, seed=42):
     """ Select generator based on type and other information. Currently available are: SABR,
         ShiftedSABR, McShiftedSABR, FbSABR, McShiftedZABR and McShiftedHeston. All models
         except SABR and ShiftedSABR require inputs num_expiries and surface_size for sample
```

### Comparing `sdevpy-0.0.8/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.0.9/src/sdevpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

