# Comparing `tmp/pwkit-0.8.9.tar.gz` & `tmp/pwkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pwkit-0.8.9.tar", last modified: Fri Sep 22 17:45:43 2017, max compression
+gzip compressed data, was "dist/pwkit-1.0.0.tar", last modified: Thu Dec 19 18:45:00 2019, max compression
```

## Comparing `pwkit-0.8.9.tar` & `pwkit-1.0.0.tar`

### file list

```diff
@@ -1,124 +1,222 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/
--rw-r--r--   0 peter     (1000) peter     (1000)       46 2016-06-27 13:06:38.000000 pwkit-0.8.9/MANIFEST.in
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)        6 2017-09-22 17:45:42.000000 pwkit-0.8.9/pwkit.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) peter     (1000)     3249 2017-09-22 17:45:42.000000 pwkit-0.8.9/pwkit.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       20 2017-09-22 17:45:42.000000 pwkit-0.8.9/pwkit.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2017-09-22 17:45:42.000000 pwkit-0.8.9/pwkit.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2015-06-02 22:17:54.000000 pwkit-0.8.9/pwkit.egg-info/not-zip-safe
--rw-r--r--   0 peter     (1000) peter     (1000)       47 2016-04-01 02:39:29.000000 pwkit-0.8.9/pwkit.egg-info/pbr.json
--rw-r--r--   0 peter     (1000) peter     (1000)      346 2017-09-22 17:45:42.000000 pwkit-0.8.9/pwkit.egg-info/entry_points.txt
--rw-r--r--   0 peter     (1000) peter     (1000)      923 2017-09-22 17:45:42.000000 pwkit-0.8.9/pwkit.egg-info/PKG-INFO
--rwxr-xr-x   0 peter     (1000) peter     (1000)      794 2014-05-17 20:02:06.000000 pwkit-0.8.9/devconfig.sh
--rwxr-xr-x   0 peter     (1000) peter     (1000)     3062 2017-09-22 17:45:16.000000 pwkit-0.8.9/setup.py
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2017-09-22 17:45:43.000000 pwkit-0.8.9/setup.cfg
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/
--rw-r--r--   0 peter     (1000) peter     (1000)    11357 2015-10-07 12:56:43.000000 pwkit-0.8.9/pwkit/ucd_physics.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4169 2015-10-09 03:11:17.000000 pwkit-0.8.9/pwkit/kbn_conf.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4312 2015-10-07 13:36:21.000000 pwkit-0.8.9/pwkit/tinifile.py
--rw-r--r--   0 peter     (1000) peter     (1000)    23454 2017-07-26 13:21:34.000000 pwkit-0.8.9/pwkit/latex.py
--rw-r--r--   0 peter     (1000) peter     (1000)    68709 2015-12-29 19:48:11.000000 pwkit-0.8.9/pwkit/v1msmt.py
--rw-r--r--   0 peter     (1000) peter     (1000)    33967 2017-06-20 19:40:25.000000 pwkit-0.8.9/pwkit/lsqmdl.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3033 2015-10-07 12:55:55.000000 pwkit-0.8.9/pwkit/simpleenum.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6757 2015-10-09 03:12:55.000000 pwkit-0.8.9/pwkit/pdm.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7694 2015-10-07 13:35:28.000000 pwkit-0.8.9/pwkit/radio_cal_models.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8123 2015-10-07 12:51:15.000000 pwkit-0.8.9/pwkit/contours.py
--rw-r--r--   0 peter     (1000) peter     (1000)    16546 2017-04-26 03:38:04.000000 pwkit-0.8.9/pwkit/bblocks.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10248 2015-10-09 03:11:09.000000 pwkit-0.8.9/pwkit/inifile.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8629 2016-07-08 12:31:07.000000 pwkit-0.8.9/pwkit/method_decorator.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3877 2015-10-07 12:49:44.000000 pwkit-0.8.9/pwkit/cgs.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9398 2017-08-28 19:03:01.000000 pwkit-0.8.9/pwkit/data_gui_helpers.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6464 2016-06-27 13:06:38.000000 pwkit-0.8.9/pwkit/slurp.py
--rw-r--r--   0 peter     (1000) peter     (1000)    19565 2017-04-10 15:32:51.000000 pwkit-0.8.9/pwkit/colormaps.py
--rw-r--r--   0 peter     (1000) peter     (1000)    50045 2017-04-10 19:41:46.000000 pwkit-0.8.9/pwkit/astutil.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9163 2015-10-09 03:05:50.000000 pwkit-0.8.9/pwkit/tabfile.py
--rw-r--r--   0 peter     (1000) peter     (1000)    15799 2015-10-09 03:13:19.000000 pwkit-0.8.9/pwkit/kwargv.py
--rw-r--r--   0 peter     (1000) peter     (1000)    30688 2017-09-22 17:42:59.000000 pwkit-0.8.9/pwkit/ndshow_gtk3.py
--rw-r--r--   0 peter     (1000) peter     (1000)    35107 2017-08-15 21:28:31.000000 pwkit-0.8.9/pwkit/synphot.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/cli/
--rw-r--r--   0 peter     (1000) peter     (1000)    13022 2016-08-23 14:23:18.000000 pwkit-0.8.9/pwkit/cli/multitool.py
--rw-r--r--   0 peter     (1000) peter     (1000)    18847 2015-10-13 18:22:23.000000 pwkit-0.8.9/pwkit/cli/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)    16064 2017-04-02 03:33:40.000000 pwkit-0.8.9/pwkit/cli/astrotool.py
--rw-r--r--   0 peter     (1000) peter     (1000)    10371 2017-04-13 01:24:42.000000 pwkit-0.8.9/pwkit/cli/wrapout.py
--rw-r--r--   0 peter     (1000) peter     (1000)    20430 2017-04-12 14:18:47.000000 pwkit-0.8.9/pwkit/cli/imtool.py
--rw-r--r--   0 peter     (1000) peter     (1000)    16698 2017-04-13 01:30:21.000000 pwkit-0.8.9/pwkit/cli/latexdriver.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8368 2016-06-27 13:06:38.000000 pwkit-0.8.9/pwkit/dulk_models.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6059 2017-04-15 14:30:13.000000 pwkit-0.8.9/pwkit/ninja_syntax.py
--rw-r--r--   0 peter     (1000) peter     (1000)     8317 2017-09-22 17:45:01.000000 pwkit-0.8.9/pwkit/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3667 2017-08-09 18:53:15.000000 pwkit-0.8.9/pwkit/phoenix.py
--rw-r--r--   0 peter     (1000) peter     (1000)    30224 2016-07-08 12:31:07.000000 pwkit-0.8.9/pwkit/numutil.py
--rw-r--r--   0 peter     (1000) peter     (1000)    69048 2016-07-14 14:39:40.000000 pwkit-0.8.9/pwkit/msmt.py
--rw-r--r--   0 peter     (1000) peter     (1000)    92658 2017-08-08 15:51:40.000000 pwkit-0.8.9/pwkit/lmmin.py
--rw-r--r--   0 peter     (1000) peter     (1000)    17764 2016-08-23 14:23:18.000000 pwkit-0.8.9/pwkit/immodel.py
--rw-r--r--   0 peter     (1000) peter     (1000)    16299 2016-08-12 13:07:25.000000 pwkit-0.8.9/pwkit/ellipses.py
--rw-r--r--   0 peter     (1000) peter     (1000)    25877 2017-04-28 19:24:55.000000 pwkit-0.8.9/pwkit/sherpa.py
--rw-r--r--   0 peter     (1000) peter     (1000)    37248 2017-04-14 20:35:38.000000 pwkit-0.8.9/pwkit/io.py
--rw-r--r--   0 peter     (1000) peter     (1000)    80936 2015-10-07 13:16:04.000000 pwkit-0.8.9/pwkit/unicode_to_latex.py
--rw-r--r--   0 peter     (1000) peter     (1000)    43363 2017-06-30 14:53:07.000000 pwkit-0.8.9/pwkit/astimage.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/environments/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/environments/sas/
--rw-r--r--   0 peter     (1000) peter     (1000)    15123 2015-10-09 03:10:47.000000 pwkit-0.8.9/pwkit/environments/sas/data.py
--rw-r--r--   0 peter     (1000) peter     (1000)    21016 2016-06-27 13:06:38.000000 pwkit-0.8.9/pwkit/environments/sas/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     3294 2017-04-10 15:32:51.000000 pwkit-0.8.9/pwkit/environments/heasoft.py
--rw-r--r--   0 peter     (1000) peter     (1000)     7747 2017-04-06 15:25:22.000000 pwkit-0.8.9/pwkit/environments/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/environments/jupyter/
--rw-r--r--   0 peter     (1000) peter     (1000)     5805 2015-10-17 16:29:48.000000 pwkit-0.8.9/pwkit/environments/jupyter/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/environments/ciao/
--rw-r--r--   0 peter     (1000) peter     (1000)    16793 2017-05-02 22:49:43.000000 pwkit-0.8.9/pwkit/environments/ciao/data.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5615 2017-04-06 15:42:16.000000 pwkit-0.8.9/pwkit/environments/ciao/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6635 2017-05-02 21:19:57.000000 pwkit-0.8.9/pwkit/environments/ciao/analysis.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/environments/casa/
--rw-r--r--   0 peter     (1000) peter     (1000)    21427 2017-04-10 15:32:51.000000 pwkit-0.8.9/pwkit/environments/casa/spwglue.py
--rw-r--r--   0 peter     (1000) peter     (1000)      733 2015-05-19 17:56:26.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_plotants.py
--rw-r--r--   0 peter     (1000) peter     (1000)    29577 2017-06-06 02:47:46.000000 pwkit-0.8.9/pwkit/environments/casa/closures.py
--rw-r--r--   0 peter     (1000) peter     (1000)    13276 2017-07-17 19:57:27.000000 pwkit-0.8.9/pwkit/environments/casa/dftphotom.py
--rw-r--r--   0 peter     (1000) peter     (1000)      985 2016-08-15 17:09:37.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_importalma.py
--rw-r--r--   0 peter     (1000) peter     (1000)      876 2016-08-30 12:16:26.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_setjy.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5781 2016-06-27 13:06:38.000000 pwkit-0.8.9/pwkit/environments/casa/polmodel.py
--rw-r--r--   0 peter     (1000) peter     (1000)    21077 2016-06-27 13:06:38.000000 pwkit-0.8.9/pwkit/environments/casa/gpdiagnostics.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1017 2015-05-19 17:56:26.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_importevla.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12061 2017-06-06 02:47:46.000000 pwkit-0.8.9/pwkit/environments/casa/dftspect.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1047 2015-05-19 17:56:26.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_genantpos.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6873 2017-06-15 23:29:33.000000 pwkit-0.8.9/pwkit/environments/casa/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)   116336 2017-09-22 17:42:59.000000 pwkit-0.8.9/pwkit/environments/casa/tasks.py
--rw-r--r--   0 peter     (1000) peter     (1000)      651 2016-08-15 17:09:37.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_flagcmd.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4663 2015-10-06 21:49:31.000000 pwkit-0.8.9/pwkit/environments/casa/scripting_driver.py
--rw-r--r--   0 peter     (1000) peter     (1000)     9076 2016-06-27 13:06:38.000000 pwkit-0.8.9/pwkit/environments/casa/scripting.py
--rw-r--r--   0 peter     (1000) peter     (1000)    13834 2017-07-17 20:01:16.000000 pwkit-0.8.9/pwkit/environments/casa/dftdynspec.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1084 2015-05-19 17:56:26.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_plotcal.py
--rw-r--r--   0 peter     (1000) peter     (1000)      957 2016-07-08 12:31:07.000000 pwkit-0.8.9/pwkit/environments/casa/cscript_getopacities.py
--rw-r--r--   0 peter     (1000) peter     (1000)    12615 2017-05-03 19:11:06.000000 pwkit-0.8.9/pwkit/environments/casa/util.py
--rw-r--r--   0 peter     (1000) peter     (1000)    17234 2015-12-29 19:06:11.000000 pwkit-0.8.9/pwkit/parallel.py
--rw-r--r--   0 peter     (1000) peter     (1000)     6326 2016-02-16 05:32:14.000000 pwkit-0.8.9/pwkit/tabfile2.py
--rw-r--r--   0 peter     (1000) peter     (1000)    28541 2017-04-10 15:32:51.000000 pwkit-0.8.9/pwkit/ndshow_gtk2.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/data/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2017-09-22 17:45:43.000000 pwkit-0.8.9/pwkit/data/bandpasses/
--rw-r--r--   0 peter     (1000) peter     (1000)    34560 2014-07-24 16:34:56.000000 pwkit-0.8.9/pwkit/data/bandpasses/sdss3_filter_responses.fits
--rw-r--r--   0 peter     (1000) peter     (1000)     2180 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_2mass_J.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    21901 2017-08-10 14:59:39.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_h.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    66658 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_4.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    14615 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_Mp.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      698 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_galex_fuv.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      628 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_bessell_UX.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    11273 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      417 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_bessell_V.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    21935 2000-04-26 23:12:07.000000 pwkit-0.8.9/pwkit/data/bandpasses/nsfcam_hmk_trans.dat~
--rw-r--r--   0 peter     (1000) peter     (1000)    23040 2014-07-29 22:52:49.000000 pwkit-0.8.9/pwkit/data/bandpasses/swuw1_20041120v106.arf
--rw-r--r--   0 peter     (1000) peter     (1000)      406 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_bessell_I.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      826 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_galex_nuv.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      914 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_mearth_ccd715.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      393 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_bessell_R.dat
--rw-r--r--   0 peter     (1000) peter     (1000)     1275 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_2mass_H.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    40347 2000-04-26 23:12:07.000000 pwkit-0.8.9/pwkit/data/bandpasses/nsfcam_jmk_trans.dat~
--rw-r--r--   0 peter     (1000) peter     (1000)    25811 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_Ks.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    14372 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_2.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    10472 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_1.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    66658 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_3.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      482 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_bessell_B.dat
--rw-r--r--   0 peter     (1000) peter     (1000)     1614 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_2mass_Ks.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    33727 2014-07-24 16:34:41.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_Lp.dat
--rw-r--r--   0 peter     (1000) peter     (1000)    40313 2017-08-10 14:59:13.000000 pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_J.dat
--rw-r--r--   0 peter     (1000) peter     (1000)      647 2015-06-03 13:37:40.000000 pwkit-0.8.9/Makefile.in
--rw-r--r--   0 peter     (1000) peter     (1000)     2337 2017-04-19 12:35:26.000000 pwkit-0.8.9/README.rst
--rw-r--r--   0 peter     (1000) peter     (1000)      923 2017-09-22 17:45:43.000000 pwkit-0.8.9/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      306 2017-09-22 17:42:59.000000 pwkit-0.8.9/DEVNOTES.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)      278 2019-12-19 18:41:18.000000 pwkit-1.0.0/CHANGES.md
+-rw-r--r--   0 peter     (1000) peter     (1000)     1072 2014-05-17 20:00:30.000000 pwkit-1.0.0/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)      227 2019-12-19 18:39:19.000000 pwkit-1.0.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)      923 2019-12-19 18:45:00.000000 pwkit-1.0.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     2337 2017-04-19 12:35:26.000000 pwkit-1.0.0/README.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1479 2019-12-19 18:36:43.000000 pwkit-1.0.0/RELEASE_PROCESS.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7414 2015-05-12 21:47:27.000000 pwkit-1.0.0/docs/Makefile
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/_static/
+-rw-r--r--   0 peter     (1000) peter     (1000)      422 2015-12-29 19:06:16.000000 pwkit-1.0.0/docs/source/_static/pwkit.css
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/_templates/
+-rw-r--r--   0 peter     (1000) peter     (1000)       85 2015-05-29 22:16:21.000000 pwkit-1.0.0/docs/source/_templates/layout.html
+-rw-r--r--   0 peter     (1000) peter     (1000)       83 2015-05-29 22:48:30.000000 pwkit-1.0.0/docs/source/_templates/page.html
+-rw-r--r--   0 peter     (1000) peter     (1000)     3921 2017-04-19 12:35:29.000000 pwkit-1.0.0/docs/source/about.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/cli-tools/
+-rw-r--r--   0 peter     (1000) peter     (1000)      448 2015-08-12 04:09:17.000000 pwkit-1.0.0/docs/source/cli-tools/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      374 2015-05-24 19:40:42.000000 pwkit-1.0.0/docs/source/cli-tools/pwkit-cli-multitool.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      350 2015-05-29 21:31:11.000000 pwkit-1.0.0/docs/source/cli-tools/pwkit-cli-toplevel.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      429 2015-07-24 19:26:58.000000 pwkit-1.0.0/docs/source/cli-tools/pwkit-kwargv.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     2635 2019-12-19 18:42:40.000000 pwkit-1.0.0/docs/source/conf.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/environments/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/environments/casa/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1678 2017-07-17 20:02:29.000000 pwkit-1.0.0/docs/source/environments/casa/dftdynspec.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     2862 2018-09-10 13:12:44.000000 pwkit-1.0.0/docs/source/environments/casa/dftphotom.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     2276 2018-09-10 12:46:50.000000 pwkit-1.0.0/docs/source/environments/casa/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     7886 2017-12-13 17:25:45.000000 pwkit-1.0.0/docs/source/environments/casa/tasks.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     3806 2017-04-06 14:02:59.000000 pwkit-1.0.0/docs/source/environments/casa/utilities.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/environments/heasoft/
+-rw-r--r--   0 peter     (1000) peter     (1000)     2506 2017-04-10 15:32:51.000000 pwkit-1.0.0/docs/source/environments/heasoft/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      467 2017-04-10 20:56:31.000000 pwkit-1.0.0/docs/source/environments/index.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/environments/sas/
+-rw-r--r--   0 peter     (1000) peter     (1000)      707 2017-04-10 15:40:17.000000 pwkit-1.0.0/docs/source/environments/sas/data.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      532 2017-04-10 15:36:44.000000 pwkit-1.0.0/docs/source/environments/sas/index.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/foundations/
+-rw-r--r--   0 peter     (1000) peter     (1000)     3264 2016-06-27 13:06:38.000000 pwkit-1.0.0/docs/source/foundations/core.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      426 2016-07-08 12:31:07.000000 pwkit-1.0.0/docs/source/foundations/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)    13160 2017-04-14 20:35:49.000000 pwkit-1.0.0/docs/source/foundations/io.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     5980 2019-07-10 20:53:48.000000 pwkit-1.0.0/docs/source/foundations/numerical.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1463 2015-12-29 19:06:11.000000 pwkit-1.0.0/docs/source/foundations/parallel.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      428 2015-08-11 14:12:23.000000 pwkit-1.0.0/docs/source/foundations/pwkit-simpleenum.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      556 2017-01-18 16:28:29.000000 pwkit-1.0.0/docs/source/index.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/infrastructure/
+-rw-r--r--   0 peter     (1000) peter     (1000)      433 2016-07-08 12:31:07.000000 pwkit-1.0.0/docs/source/infrastructure/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      377 2015-05-29 21:31:11.000000 pwkit-1.0.0/docs/source/infrastructure/pwkit-environments-toplevel.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      379 2016-07-08 12:31:07.000000 pwkit-1.0.0/docs/source/infrastructure/pwkit-method_decorator.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/io/
+-rw-r--r--   0 peter     (1000) peter     (1000)      483 2015-07-24 03:07:47.000000 pwkit-1.0.0/docs/source/io/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      353 2015-05-24 19:17:18.000000 pwkit-1.0.0/docs/source/io/pwkit-inifile.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      350 2015-05-24 19:19:09.000000 pwkit-1.0.0/docs/source/io/pwkit-latex.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      425 2015-08-12 03:16:39.000000 pwkit-1.0.0/docs/source/io/pwkit-tabfile.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      382 2015-05-24 19:26:54.000000 pwkit-1.0.0/docs/source/io/pwkit-tinifile.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      383 2015-05-24 19:27:58.000000 pwkit-1.0.0/docs/source/io/pwkit-unicode_to_latex.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     8981 2015-06-04 02:19:08.000000 pwkit-1.0.0/docs/source/io/slurp.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/pwkit/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/pwkit/cli/
+-rw-r--r--   0 peter     (1000) peter     (1000)      424 2015-08-12 03:29:08.000000 pwkit-1.0.0/docs/source/pwkit/cli/astrotool.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      440 2015-08-12 03:29:31.000000 pwkit-1.0.0/docs/source/pwkit/cli/imtool.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      414 2015-08-12 03:29:46.000000 pwkit-1.0.0/docs/source/pwkit/cli/latexdriver.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      376 2015-05-24 19:35:13.000000 pwkit-1.0.0/docs/source/pwkit/cli/wrapout.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      371 2015-05-24 19:15:07.000000 pwkit-1.0.0/docs/source/pwkit/colormaps.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      347 2015-05-24 19:15:01.000000 pwkit-1.0.0/docs/source/pwkit/contours.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      379 2015-05-24 19:14:53.000000 pwkit-1.0.0/docs/source/pwkit/data_gui_helpers.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/pwkit/environments/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/pwkit/environments/casa/
+-rw-r--r--   0 peter     (1000) peter     (1000)      407 2015-08-12 02:59:06.000000 pwkit-1.0.0/docs/source/pwkit/environments/casa/scripting.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      411 2015-08-12 02:58:59.000000 pwkit-1.0.0/docs/source/pwkit/environments/casa/spwglue.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/pwkit/environments/ciao/
+-rw-r--r--   0 peter     (1000) peter     (1000)      394 2016-06-27 13:06:38.000000 pwkit-1.0.0/docs/source/pwkit/environments/ciao/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      442 2015-08-12 03:31:15.000000 pwkit-1.0.0/docs/source/pwkit/ndshow_gtk2.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      442 2015-08-12 03:31:25.000000 pwkit-1.0.0/docs/source/pwkit/ndshow_gtk3.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)       52 2017-03-03 20:40:09.000000 pwkit-1.0.0/docs/source/requirements.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/docs/source/science/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6197 2017-04-10 19:42:36.000000 pwkit-1.0.0/docs/source/science/basic-astro.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1614 2018-04-03 02:12:40.000000 pwkit-1.0.0/docs/source/science/dulk-models.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1593 2018-08-09 03:21:08.000000 pwkit-1.0.0/docs/source/science/fk10-code.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      731 2018-08-08 21:31:51.000000 pwkit-1.0.0/docs/source/science/index.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1835 2018-05-10 19:57:10.000000 pwkit-1.0.0/docs/source/science/least-squares-modeling.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      448 2015-08-12 03:32:03.000000 pwkit-1.0.0/docs/source/science/pwkit-astimage.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      358 2015-05-24 19:15:22.000000 pwkit-1.0.0/docs/source/science/pwkit-bblocks.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      380 2015-08-12 03:35:24.000000 pwkit-1.0.0/docs/source/science/pwkit-cgs.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      444 2015-08-12 03:40:02.000000 pwkit-1.0.0/docs/source/science/pwkit-ellipses.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      390 2015-08-12 03:35:57.000000 pwkit-1.0.0/docs/source/science/pwkit-immodel.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      430 2015-08-12 03:36:43.000000 pwkit-1.0.0/docs/source/science/pwkit-kbn_conf.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      450 2015-08-12 03:20:02.000000 pwkit-1.0.0/docs/source/science/pwkit-lmmin.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      368 2015-05-24 19:22:28.000000 pwkit-1.0.0/docs/source/science/pwkit-msmt.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      370 2015-05-24 19:24:25.000000 pwkit-1.0.0/docs/source/science/pwkit-pdm.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      378 2015-05-24 19:24:52.000000 pwkit-1.0.0/docs/source/science/pwkit-phoenix.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      442 2015-08-12 03:37:57.000000 pwkit-1.0.0/docs/source/science/pwkit-radio_cal_models.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      481 2015-08-12 03:22:19.000000 pwkit-1.0.0/docs/source/science/pwkit-ucd_physics.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     1692 2017-04-28 19:25:24.000000 pwkit-1.0.0/docs/source/science/sherpa.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)     2859 2018-04-25 21:12:45.000000 pwkit-1.0.0/docs/source/science/synphot.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      459 2015-08-12 04:03:51.000000 pwkit-1.0.0/docs/source/section-cli.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      479 2015-07-24 03:08:17.000000 pwkit-1.0.0/docs/source/section-viz.rst
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/lmmin_reference/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      609 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/dataf
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3340 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/fdjac2.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)    15443 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/lmder.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)    49879 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/lmder1.all.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)    15544 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/lmdif.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)    52113 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/lmdif1.all.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8243 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/lmpar.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)   142529 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/mpfit.pro
+-rwxrwxr-x   0 peter     (1000) peter     (1000)    91069 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/mpfit.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    96774 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/nmpfit.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6178 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/qrsolv.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)    28363 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/test.lmder.f
+-rw-rw-r--   0 peter     (1000) peter     (1000)    19200 2012-10-01 21:27:57.000000 pwkit-1.0.0/lmmin_reference/test.lmdif.f
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7871 2019-12-19 18:42:30.000000 pwkit-1.0.0/pwkit/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    43363 2019-07-10 20:07:05.000000 pwkit-1.0.0/pwkit/astimage.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    51506 2018-03-28 16:21:16.000000 pwkit-1.0.0/pwkit/astutil.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16546 2017-04-26 03:38:04.000000 pwkit-1.0.0/pwkit/bblocks.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3877 2015-10-07 12:49:44.000000 pwkit-1.0.0/pwkit/cgs.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/cli/
+-rw-r--r--   0 peter     (1000) peter     (1000)    18847 2015-10-13 18:22:23.000000 pwkit-1.0.0/pwkit/cli/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16143 2018-06-18 21:00:59.000000 pwkit-1.0.0/pwkit/cli/astrotool.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    20430 2017-12-16 20:15:25.000000 pwkit-1.0.0/pwkit/cli/imtool.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16802 2018-09-06 13:50:11.000000 pwkit-1.0.0/pwkit/cli/latexdriver.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    13022 2016-08-23 14:23:18.000000 pwkit-1.0.0/pwkit/cli/multitool.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10356 2017-11-09 02:12:39.000000 pwkit-1.0.0/pwkit/cli/wrapout.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    19565 2017-04-10 15:32:51.000000 pwkit-1.0.0/pwkit/colormaps.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8123 2015-10-07 12:51:15.000000 pwkit-1.0.0/pwkit/contours.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/data/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/data/bandpasses/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1275 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_2mass_H.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)     2180 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_2mass_J.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)     1614 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_2mass_Ks.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      482 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_bessell_B.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      406 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_bessell_I.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      393 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_bessell_R.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      628 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_bessell_UX.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      417 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_bessell_V.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      698 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_galex_fuv.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      826 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_galex_nuv.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    11273 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)      914 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_mearth_ccd715.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    40313 2017-08-10 14:59:13.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_J.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    25811 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_Ks.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    33727 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_Lp.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    14615 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_Mp.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    21901 2017-08-10 14:59:39.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_h.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    10472 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_1.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    14372 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_2.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    66658 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_3.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    66658 2014-07-24 16:34:41.000000 pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_4.dat
+-rw-r--r--   0 peter     (1000) peter     (1000)    34560 2014-07-24 16:34:56.000000 pwkit-1.0.0/pwkit/data/bandpasses/sdss3_filter_responses.fits
+-rw-r--r--   0 peter     (1000) peter     (1000)    23040 2014-07-29 22:52:49.000000 pwkit-1.0.0/pwkit/data/bandpasses/swuw1_20041120v106.arf
+-rw-r--r--   0 peter     (1000) peter     (1000)     9871 2019-07-10 20:08:36.000000 pwkit-1.0.0/pwkit/data_gui_helpers.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    15020 2018-04-03 02:07:05.000000 pwkit-1.0.0/pwkit/dulk_models.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16299 2016-08-12 13:07:25.000000 pwkit-1.0.0/pwkit/ellipses.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/environments/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7764 2018-03-15 14:47:22.000000 pwkit-1.0.0/pwkit/environments/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/environments/casa/
+-rw-r--r--   0 peter     (1000) peter     (1000)     6776 2017-11-03 18:32:59.000000 pwkit-1.0.0/pwkit/environments/casa/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    29520 2017-11-05 15:34:16.000000 pwkit-1.0.0/pwkit/environments/casa/closures.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      651 2016-08-15 17:09:37.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_flagcmd.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1031 2017-11-02 20:44:37.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_genantpos.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      926 2017-11-02 20:16:36.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_getopacities.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      985 2016-08-15 17:09:37.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_importalma.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1017 2015-05-19 17:56:26.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_importevla.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      733 2015-05-19 17:56:26.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_plotants.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1084 2015-05-19 17:56:26.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_plotcal.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      876 2016-08-30 12:16:26.000000 pwkit-1.0.0/pwkit/environments/casa/cscript_setjy.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    13770 2018-10-09 13:29:12.000000 pwkit-1.0.0/pwkit/environments/casa/dftdynspec.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    14832 2018-09-10 13:10:08.000000 pwkit-1.0.0/pwkit/environments/casa/dftphotom.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11976 2018-10-09 13:34:29.000000 pwkit-1.0.0/pwkit/environments/casa/dftspect.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    21077 2017-11-05 15:33:32.000000 pwkit-1.0.0/pwkit/environments/casa/gpdiagnostics.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5781 2017-11-05 15:33:32.000000 pwkit-1.0.0/pwkit/environments/casa/polmodel.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9001 2017-11-05 15:33:32.000000 pwkit-1.0.0/pwkit/environments/casa/scripting.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4663 2015-10-06 21:49:31.000000 pwkit-1.0.0/pwkit/environments/casa/scripting_driver.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    21281 2017-11-05 15:33:32.000000 pwkit-1.0.0/pwkit/environments/casa/spwglue.py
+-rw-r--r--   0 peter     (1000) peter     (1000)   126821 2019-12-19 18:35:13.000000 pwkit-1.0.0/pwkit/environments/casa/tasks.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12495 2017-11-05 15:33:32.000000 pwkit-1.0.0/pwkit/environments/casa/util.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/environments/ciao/
+-rw-r--r--   0 peter     (1000) peter     (1000)     5615 2017-04-06 15:42:16.000000 pwkit-1.0.0/pwkit/environments/ciao/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6635 2017-05-02 21:19:57.000000 pwkit-1.0.0/pwkit/environments/ciao/analysis.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16793 2017-05-02 22:49:43.000000 pwkit-1.0.0/pwkit/environments/ciao/data.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3294 2017-04-10 15:32:51.000000 pwkit-1.0.0/pwkit/environments/heasoft.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/environments/jupyter/
+-rw-r--r--   0 peter     (1000) peter     (1000)     5805 2015-10-17 16:29:48.000000 pwkit-1.0.0/pwkit/environments/jupyter/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit/environments/sas/
+-rw-r--r--   0 peter     (1000) peter     (1000)    21130 2018-03-14 16:47:16.000000 pwkit-1.0.0/pwkit/environments/sas/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17394 2018-03-15 18:56:35.000000 pwkit-1.0.0/pwkit/environments/sas/data.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)    28406 2018-08-09 03:22:59.000000 pwkit-1.0.0/pwkit/fk10.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17764 2016-08-23 14:23:18.000000 pwkit-1.0.0/pwkit/immodel.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10248 2015-10-09 03:11:09.000000 pwkit-1.0.0/pwkit/inifile.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    37391 2017-11-02 20:09:47.000000 pwkit-1.0.0/pwkit/io.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4169 2015-10-09 03:11:17.000000 pwkit-1.0.0/pwkit/kbn_conf.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    16112 2018-10-09 13:43:25.000000 pwkit-1.0.0/pwkit/kwargv.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    22936 2018-03-12 19:21:28.000000 pwkit-1.0.0/pwkit/latex.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    92658 2017-08-08 15:51:40.000000 pwkit-1.0.0/pwkit/lmmin.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    35401 2019-07-19 18:50:47.000000 pwkit-1.0.0/pwkit/lsqmdl.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8629 2016-07-08 12:31:07.000000 pwkit-1.0.0/pwkit/method_decorator.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    68361 2017-09-30 21:03:03.000000 pwkit-1.0.0/pwkit/msmt.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    28541 2017-04-10 15:32:51.000000 pwkit-1.0.0/pwkit/ndshow_gtk2.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    32212 2018-02-20 23:45:02.000000 pwkit-1.0.0/pwkit/ndshow_gtk3.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6059 2017-04-15 14:30:13.000000 pwkit-1.0.0/pwkit/ninja_syntax.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    31663 2019-07-10 20:52:53.000000 pwkit-1.0.0/pwkit/numutil.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17148 2017-09-30 20:53:53.000000 pwkit-1.0.0/pwkit/parallel.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6757 2015-10-09 03:12:55.000000 pwkit-1.0.0/pwkit/pdm.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3667 2017-08-09 18:53:15.000000 pwkit-1.0.0/pwkit/phoenix.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7694 2015-10-07 13:35:28.000000 pwkit-1.0.0/pwkit/radio_cal_models.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    25877 2017-04-28 19:24:55.000000 pwkit-1.0.0/pwkit/sherpa.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3033 2015-10-07 12:55:55.000000 pwkit-1.0.0/pwkit/simpleenum.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6464 2016-06-27 13:06:38.000000 pwkit-1.0.0/pwkit/slurp.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    34053 2018-04-25 21:19:45.000000 pwkit-1.0.0/pwkit/synphot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9163 2015-10-09 03:05:50.000000 pwkit-1.0.0/pwkit/tabfile.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4312 2015-10-07 13:36:21.000000 pwkit-1.0.0/pwkit/tinifile.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11357 2015-10-07 12:56:43.000000 pwkit-1.0.0/pwkit/ucd_physics.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    81062 2018-03-12 19:21:28.000000 pwkit-1.0.0/pwkit/unicode_to_latex.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)      923 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     5996 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      346 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/not-zip-safe
+-rw-r--r--   0 peter     (1000) peter     (1000)       20 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        6 2019-12-19 18:45:00.000000 pwkit-1.0.0/pwkit.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2019-12-19 18:45:00.000000 pwkit-1.0.0/setup.cfg
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     3060 2019-12-19 18:42:21.000000 pwkit-1.0.0/setup.py
```

### Comparing `pwkit-0.8.9/pwkit.egg-info/PKG-INFO` & `pwkit-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pwkit
-Version: 0.8.9
+Version: 1.0.0
 Summary: Miscellaneous scientific and astronomical tools
 Home-page: https://github.com/pkgw/pwkit/
 Author: Peter Williams
 Author-email: peter@newton.cx
 License: MIT
 Description: This is a collection of Peter Williams' miscellaneous Python tools. I'm
             packaging them so that other people can install them off of PyPI and run
```

### Comparing `pwkit-0.8.9/setup.py` & `pwkit-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #! /usr/bin/env python
-# Copyright 2014-2016 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2014-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 # I don't use the ez_setup module because it causes us to automatically build
 # and install a new setuptools module, which I'm not interested in doing.
 
 from setuptools import setup
 
 dynamic_requires = []
 import sys
 if sys.version_info[0] < 3:
-    dynamic_requires.append ('pathlib >= 1.0')
+    dynamic_requires.append('pathlib >= 1.0')
 
-setup (
+setup(
     name = 'pwkit',
-    version = '0.8.9', # also edit pwkit/__init__.py, docs/source/conf.py!
+    version = '1.0.0', # also edit pwkit/__init__.py, docs/source/conf.py!
 
     # This package actually *is* zip-safe, but I've run into issues with
     # installing it as a Zip: in particular, the install sometimes fails with
     # "bad local file header", and reloading a module after a reinstall in
     # IPython gives an ImportError with the same message. These are annoying
     # enough and I don't really care so we just install it as flat files.
     zip_safe = False,
```

### Comparing `pwkit-0.8.9/pwkit/ucd_physics.py` & `pwkit-1.0.0/pwkit/ucd_physics.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/kbn_conf.py` & `pwkit-1.0.0/pwkit/kbn_conf.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/tinifile.py` & `pwkit-1.0.0/pwkit/tinifile.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/latex.py` & `pwkit-1.0.0/pwkit/latex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2013-2014 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2013-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """pwkit.latex - various helpers for the LaTeX typesetting system.
 
 Classes
 -------
 
@@ -43,235 +43,243 @@
 WideHeader
   Helper for multi-column headers.
 
 
 XXX: Barely tested!
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('''AlignedNumberFormatter BasicFormatter BoolFormatter LimitFormatter
-                  MaybeNumberFormatter Referencer TableBuilder UncertFormatter
-                  WideHeader latexify_l3col latexify_n2col latexify_u3col
-                  latexify''').split ()
+__all__ = '''
+AlignedNumberFormatter
+BasicFormatter
+BoolFormatter
+LimitFormatter
+MaybeNumberFormatter
+Referencer
+TableBuilder
+UncertFormatter
+WideHeader
+latexify_l3col
+latexify_n2col
+latexify_u3col
+latexify'''.split()
 
 import string
 import six
 from six.moves import range
 from . import Holder, PKError, binary_type, msmt, reraise_context, text_type
 
 
-def _reftext (key):
+def _reftext(key):
     if key[0] == '*':
-        return key[1:].encode ('ascii')
-    return b'\\citet{%s}' % key.encode ('ascii')
+        return key[1:]
+    return '\\citet{%s}' % key
 
 
-class Referencer (object):
+class Referencer(object):
     """Accumulate a numbered list of bibtex references. Methods:
 
-    refkey (bibkey)
+    refkey(bibkey)
       Return a string that should be used to give
       a numbered reference to the given bibtex
       key. "thiswork" is handled specially.
-    dump ()
+    dump()
       Return a string with \citet{} commands identifing
       all of the numbered references.
 
     Attributes:
 
     thisworktext
       text referring to "this work"; defaults to that.
     thisworkmarker
       special symbol used to denote "this work"; defaults to star.
 
     Bibtex keys beginning with asterisks have the rest of their value used for
     the citation text, rather than "\citet{<key>}".
 
     """
-    thisworktext = b'this work'
-    thisworkmarker = b'$\\star$'
+    thisworktext = 'this work'
+    thisworkmarker = '$\\star$'
 
-    def __init__ (self):
+    def __init__(self):
         self.bibkeys = []
         self.seenthiswork = False
 
 
-    def refkey (self, bibkey):
+    def refkey(self, bibkey):
         if bibkey is None:
             return ''
 
         if bibkey == 'thiswork':
             self.seenthiswork = True
             return self.thisworkmarker
 
         try:
-            idx = self.bibkeys.index (bibkey)
+            idx = self.bibkeys.index(bibkey)
         except ValueError:
-            idx = len (self.bibkeys)
-            self.bibkeys.append (bibkey)
+            idx = len(self.bibkeys)
+            self.bibkeys.append(bibkey)
 
-        return text_type (idx + 1).encode ('ascii')
+        return text_type(idx + 1)
 
 
-    def dump (self):
-        s = b', '.join (b'[%d] %s' % (i + 1, _reftext (self.bibkeys[i]))
-                       for i in range (len (self.bibkeys)))
+    def dump(self):
+        s = ', '.join('[%d] %s' % (i + 1, _reftext(self.bibkeys[i]))
+                       for i in range(len(self.bibkeys)))
 
         if self.seenthiswork:
-            s = (b'[%s]: %s, ' % (self.thisworkmarker, self.thisworktext)) + s
+            s = ('[%s]: %s, ' % (self.thisworkmarker, self.thisworktext)) + s
 
         return s
 
 
 # Generic infrastructure for converting Python objects to LaTeX.
 #
 # Note that it's important that these functions all accept miscellaneous
 # kwargs arguments, so that TableBuilder invocations can pass along special
 # control keywords that are only specific to certain cells, without causing
 # crashes elsewhere.
 
-
 _printable_ascii = frozenset(string.printable.encode('ascii'))
 
-
-def latexify (obj, **kwargs):
+def latexify(obj, **kwargs):
     """Render an object in LaTeX appropriately.
 
     """
-    if hasattr (obj, '__pk_latex__'):
-        return obj.__pk_latex__ (**kwargs)
+    if hasattr(obj, '__pk_latex__'):
+        return obj.__pk_latex__(**kwargs)
 
-    if isinstance (obj, text_type):
+    if isinstance(obj, text_type):
         from .unicode_to_latex import unicode_to_latex
-        return unicode_to_latex (obj)
+        return unicode_to_latex(obj)
 
-    if isinstance (obj, bool):
-        # isinstance (True, int) = True, so gotta handle this first.
-        raise ValueError ('no well-defined LaTeXification of bool %r' % obj)
+    if isinstance(obj, bool):
+        # isinstance(True, int) = True, so gotta handle this first.
+        raise ValueError('no well-defined LaTeXification of bool %r' % obj)
 
-    if isinstance (obj, float):
-        nplaces = kwargs.get ('nplaces')
+    if isinstance(obj, float):
+        nplaces = kwargs.get('nplaces')
         if nplaces is None:
-            return b'$%f$' % obj
-        return b'$%.*f$' % (nplaces, obj)
+            return '$%f$' % obj
+        return '$%.*f$' % (nplaces, obj)
 
-    if isinstance (obj, int):
-        return b'$%d$' % obj
+    if isinstance(obj, int):
+        return '$%d$' % obj
 
-    if isinstance (obj, binary_type):
+    if isinstance(obj, binary_type):
         if all(c in _printable_ascii for c in obj):
-            return obj
-        raise ValueError ('no safe LaTeXification of binary string %r' % obj)
+            return obj.decode('ascii')
+        raise ValueError('no safe LaTeXification of binary string %r' % obj)
 
-    raise ValueError ('can\'t LaTeXify %r' % obj)
+    raise ValueError('can\'t LaTeXify %r' % obj)
 
 
-def latexify_n2col (x, nplaces=None, **kwargs):
+def latexify_n2col(x, nplaces=None, **kwargs):
     """Render a number into LaTeX in a 2-column format, where the columns split
     immediately to the left of the decimal point. This gives nice alignment of
     numbers in a table.
 
     """
     if nplaces is not None:
-        t = b'%.*f' % (nplaces, x)
+        t = '%.*f' % (nplaces, x)
     else:
-        t = b'%f' % x
+        t = '%f' % x
 
-    if b'.' not in t:
-        return b'$%s$ &' % t
+    if '.' not in t:
+        return '$%s$ &' % t
 
-    left, right = t.split (b'.')
-    return b'$%s$ & $.%s$' % (left, right)
+    left, right = t.split('.')
+    return '$%s$ & $.%s$' % (left, right)
 
 
-def latexify_u3col (obj, **kwargs):
+def latexify_u3col(obj, **kwargs):
     """Convert an object to special LaTeX for uncertainty tables.
 
     This conversion is meant for uncertain values in a table. The return value
     should span three columns. The first column ends just before the decimal
     point in the main number value, if it has one. It has no separation from
     the second column. The second column goes from the decimal point until
     just before the "plus-or-minus" indicator. The third column goes from the
     "plus-or-minus" until the end. If the item being formatted does not fit this
     schema, it can be wrapped in something like '\multicolumn{3}{c}{...}'.
 
     """
-    if hasattr (obj, '__pk_latex_u3col__'):
-        return obj.__pk_latex_u3col__ (**kwargs)
+    if hasattr(obj, '__pk_latex_u3col__'):
+        return obj.__pk_latex_u3col__(**kwargs)
 
     # TODO: there are reasonable ways to format many basic types, but I'm not
     # going to implement them until I need to.
 
-    raise ValueError ('can\'t LaTeXify %r in 3-column uncertain format' % obj)
+    raise ValueError('can\'t LaTeXify %r in 3-column uncertain format' % obj)
 
 
-def latexify_l3col (obj, **kwargs):
+def latexify_l3col(obj, **kwargs):
     """Convert an object to special LaTeX for limit tables.
 
     This conversion is meant for limit values in a table. The return value
     should span three columns. The first column is the limit indicator: <, >,
     ~, etc. The second column is the whole part of the value, up until just
     before the decimal point. The third column is the decimal point and the
     fractional part of the value, if present. If the item being formatted does
     not fit this schema, it can be wrapped in something like
     '\multicolumn{3}{c}{...}'.
 
     """
-    if hasattr (obj, '__pk_latex_l3col__'):
-        return obj.__pk_latex_l3col__ (**kwargs)
+    if hasattr(obj, '__pk_latex_l3col__'):
+        return obj.__pk_latex_l3col__(**kwargs)
 
-    if isinstance (obj, bool):
-        # isinstance (True, int) = True, so gotta handle this first.
-        raise ValueError ('no well-defined l3col LaTeXification of bool %r' % obj)
+    if isinstance(obj, bool):
+        # isinstance(True, int) = True, so gotta handle this first.
+        raise ValueError('no well-defined l3col LaTeXification of bool %r' % obj)
 
-    if isinstance (obj, float):
-        return b'&' + latexify_n2col (obj, **kwargs)
+    if isinstance(obj, float):
+        return '&' + latexify_n2col(obj, **kwargs)
 
-    if isinstance (obj, int):
-        return b'& $%d$ &' % obj
+    if isinstance(obj, int):
+        return '& $%d$ &' % obj
 
-    raise ValueError ('can\'t LaTeXify %r in 3-column limit format' % obj)
+    raise ValueError('can\'t LaTeXify %r in 3-column limit format' % obj)
 
 
 
 # Building nice deluxetables.
 
-class WideHeader (object):
+class WideHeader(object):
     """Information needed for constructing wide table headers.
 
     nlogcols - Number of logical columns consumed by this header.
     content  - The LaTeX to insert for this header's content.
     align    - The alignment of this header; default 'c'.
 
     Rendered as \multicolumn{nlatex}{align}{content}, where `nlatex` is the
     number of LaTeX columns spanned by this header -- which may be larger than
     `nlogcols` if certain logical columns span multiple LaTeX columns.
 
     """
-    def __init__ (self, nlogcols, content, align=b'c'):
+    def __init__(self, nlogcols, content, align='c'):
         self.nlogcols = nlogcols
         self.align = align
         self.content = content
 
 
-class TableBuilder (object):
+class TableBuilder(object):
     """Build and then emit a nice deluxetable.
 
     Methods:
 
-    addcol (headings, datafunc, formatter=None, colspec=None, numbering='(%d)')
+    addcol(headings, datafunc, formatter=None, colspec=None, numbering='(%d)')
        Define a logical column.
-    addnote (key, text)
+    addnote(key, text)
        Define a table note that can appear in cells.
-    addhcline (headerrowix, logcolidx, latexdeltastart, latexdeltaend)
+    addhcline(headerrowix, logcolidx, latexdeltastart, latexdeltaend)
        Add a horizontal line between columns.
-    notemark (key)
+    notemark(key)
        Return a \\tablenotemark{} command for the specified note key.
-    emit (stream, items)
+    emit(stream, items)
        Write the table, with one row for each thing in `items`, to the stream.
 
     If an item has an attribute `tb_row_preamble`, that text is written verbatim
     before that corresponding row is output.
 
     Attributes:
 
@@ -310,33 +318,33 @@
     are handled specially.
 
     If \\tablewidth{} is not provided, the table is set at full width, not its
     natural width, which is a lame default. The default `widthspec` lets us
     auto-widen while providing a clear avenue to customizing the width.
 
     """
-    environment = b'deluxetable'
+    environment = 'deluxetable'
     label = None
-    note = b''
-    preamble = b''
-    refs = b''
-    title = b'Untitled table'
-    widthspec = b'0em'
+    note = ''
+    preamble = ''
+    refs = ''
+    title = 'Untitled table'
+    widthspec = '0em'
     numbercols = True
     final_double_backslash = False
 
-    def __init__ (self, label):
+    def __init__(self, label):
         self._colinfo = []
         self._hclines = []
         self._notes = {}
         self._notecounter = 0
         self.label = latexify(label)
 
 
-    def addcol (self, headings, datafunc, formatter=None, colspec=None, numbering=b'(%d)'):
+    def addcol(self, headings, datafunc, formatter=None, colspec=None, numbering='(%d)'):
         """Define a logical column. Arguments:
 
         headings
           A string, or list of strings and WideHeaders. The headings are stacked
           vertically in the table header section.
         datafunc
           Return LaTeX for this cell. Call spec should be
@@ -347,52 +355,52 @@
           The LaTeX column specification letters to use; defaults to 'c's.
         numbering
           If non-False, a format for writing this column's number; if False,
           no number is written.
 
         """
         if formatter is None:
-            formatter = BasicFormatter ()
+            formatter = BasicFormatter()
 
-        if isinstance (headings, six.string_types):
+        if isinstance(headings, six.string_types):
             headings = (headings, )
 
         try:
             code = six.get_function_code(datafunc)
             nargs = code.co_argcount
         except AttributeError:
-            if hasattr (datafunc, '__call__'):
+            if hasattr(datafunc, '__call__'):
                 # This is pretty hacky ...
                 nargs = six.get_function_code(datafunc.__call__).co_argcount - 1
             else:
-                raise ValueError ('cannot find code object for datafunc')
+                raise ValueError('cannot find code object for datafunc')
 
         if nargs == 3:
             wrapped = datafunc # (item, formatter, builder)
         elif nargs == 2:
-            wrapped = lambda i, f, b: datafunc (i, f)
+            wrapped = lambda i, f, b: datafunc(i, f)
         elif nargs == 1:
-            wrapped = lambda i, f, b: datafunc (i)
+            wrapped = lambda i, f, b: datafunc(i)
         elif nargs == 0: # why not
-            wrapped = lambda i, f, b: datafunc ()
+            wrapped = lambda i, f, b: datafunc()
         else:
-            raise ValueError ('datafunc must accept between 0 and 3 args; it takes %d' % nargs)
+            raise ValueError('datafunc must accept between 0 and 3 args; it takes %d' % nargs)
 
-        ci = Holder (headings=[latexify(h) for h in headings], formatter=formatter,
-                     wdatafunc=wrapped, colspec=colspec, numbering=numbering)
-        self._colinfo.append (ci)
+        ci = Holder(headings=[latexify(h) for h in headings], formatter=formatter,
+                    wdatafunc=wrapped, colspec=colspec, numbering=numbering)
+        self._colinfo.append(ci)
         return self
 
 
-    def addnote (self, key, text):
+    def addnote(self, key, text):
         self._notes[key] = [None, text]
         return self
 
 
-    def addhcline (self, headerrowidx, logcolidx, latexdeltastart, latexdeltaend):
+    def addhcline(self, headerrowidx, logcolidx, latexdeltastart, latexdeltaend):
         """Adds a horizontal line below a limited range of columns in the header section.
         Arguments:
 
         headerrowidx    - The 0-based row number *below* which the line will be
                           drawn; i.e. 0 means that the line will be drawn below
                           the first row of header cells.
         logcolidx       - The 0-based 'logical' column number relative to which
@@ -404,318 +412,318 @@
                           columns; typically going to be zero.
         latexdeltaend   - The relative position at which to finish drawing the
                           line, in the standard Python noninclusive sense. I.e.,
                           if you want to underline two LaTeX columns,
                           latexdeltaend = latexdeltastart + 2.
 
         """
-        self._hclines.append ((headerrowidx, logcolidx, latexdeltastart, latexdeltaend))
+        self._hclines.append((headerrowidx, logcolidx, latexdeltastart, latexdeltaend))
         return self
 
 
-    def notemark (self, key):
-        noteinfo = self._notes.get (key)
+    def notemark(self, key):
+        noteinfo = self._notes.get(key)
         if noteinfo is None:
-            raise ValueError ('unrecognized note key "%s"' % key)
+            raise ValueError('unrecognized note key "%s"' % key)
 
         if noteinfo[0] is None:
             if self._notecounter > 25:
-                raise PKError ('maximum number of table notes exceeded')
+                raise PKError('maximum number of table notes exceeded')
 
             noteinfo[0] = self._notecounter
             self._notecounter += 1
 
-        return b'\\tablenotemark{%c}' % chr (ord (b'a') + noteinfo[0]).encode ('ascii')
+        return '\\tablenotemark{%c}' % chr(ord('a') + noteinfo[0])
 
 
-    def emit (self, stream, items):
+    def emit(self, stream, items):
         from six import itervalues
         write = stream.write
         colinfo = self._colinfo
 
-        colspec = b''
+        colspec = ''
         ncols = 0
         nheadrows = 0
         curlatexcol = 1
 
         for ci in colinfo:
-            ci.nlcol, colspecpart, ci.headprefix = ci.formatter.colinfo (self)
+            ci.nlcol, colspecpart, ci.headprefix = ci.formatter.colinfo(self)
             ci.latexcol = curlatexcol
 
             if ci.colspec is not None:
                 # This is more about convenience for columns that don't have
                 # fancy alignment requirements, rather than about allowing
                 # overriding.
                 colspecpart = latexify(ci.colspec)
 
             if colspecpart is None:
-                colspecpart = b'c' * ci.nlcol
+                colspecpart = 'c' * ci.nlcol
 
             ncols += ci.nlcol
             colspec += colspecpart
-            nheadrows = max (nheadrows, len (ci.headings))
+            nheadrows = max(nheadrows, len(ci.headings))
             curlatexcol += ci.nlcol
 
-        write (b'% TableBuilder table\n')
-        write (br'\begin{')
-        write (self.environment)
-        write (b'}{')
-        write (colspec)
-        write (b'}\n%custom preamble\n')
-        write (self.preamble)
-        write (b'\n%hardcoded preamble\n\\tablecolumns{')
-        write (text_type (ncols).encode ('ascii'))
-        write (b'}\n\\tablewidth{')
-        write (self.widthspec)
-        write (b'}\n\\tablecaption{')
-        write (self.title)
-        write (b'\\label{')
-        write (self.label)
-        write (b'}}\n\\tablehead{\n')
+        write('% TableBuilder table\n')
+        write('\\begin{')
+        write(self.environment)
+        write('}{')
+        write(colspec)
+        write('}\n%custom preamble\n')
+        write(self.preamble)
+        write('\n%hardcoded preamble\n\\tablecolumns{')
+        write(text_type(ncols))
+        write('}\n\\tablewidth{')
+        write(self.widthspec)
+        write('}\n\\tablecaption{')
+        write(self.title)
+        write('\\label{')
+        write(self.label)
+        write('}}\n\\tablehead{\n')
 
-        cr = b''
+        cr = ''
 
-        for i in range (nheadrows):
-            write (cr)
+        for i in range(nheadrows):
+            write(cr)
 
             for hidx, cidx, lds, lde in self._hclines:
                 # Note super inefficiency. Who cares?
                 if hidx == i - 1:
                     latexcolbase = colinfo[cidx].latexcol
-                    write (b' \\cline{')
-                    write (text_type (latexcolbase + lds).encode ('ascii'))
-                    write (b'-')
-                    write (text_type (latexcolbase + lde - 1).encode ('ascii'))
-                    write (b'} ')
+                    write(' \\cline{')
+                    write(text_type(latexcolbase + lds))
+                    write('-')
+                    write(text_type(latexcolbase + lde - 1))
+                    write('} ')
 
-            sep = b''
+            sep = ''
             nlefttoskip = 0
 
-            for cidx, ci in enumerate (colinfo):
-                write (sep)
+            for cidx, ci in enumerate(colinfo):
+                write(sep)
 
                 if nlefttoskip < 1:
-                    if len (ci.headings) <= i:
-                        write (b' & ' * (ci.nlcol - 1))
+                    if len(ci.headings) <= i:
+                        write(' & ' * (ci.nlcol - 1))
                     else:
                         h = ci.headings[i]
 
-                        if isinstance (h, WideHeader):
+                        if isinstance(h, WideHeader):
                             nlefttoskip = h.nlogcols
 
                             nlatex = 0
-                            for j in range (h.nlogcols):
+                            for j in range(h.nlogcols):
                                 nlatex += colinfo[cidx + j].nlcol
 
-                            write (b'\\multicolumn{')
-                            write (text_type (nlatex).encode ('ascii'))
-                            write (b'}{')
-                            write (h.align)
-                            write (b'}{')
-                            write (h.content)
-                            write (b'}')
+                            write('\\multicolumn{')
+                            write(text_type(nlatex))
+                            write('}{')
+                            write(h.align)
+                            write('}{')
+                            write(h.content)
+                            write('}')
                         else:
-                            write (ci.headprefix)
-                            write (b'{')
-                            write (h)
-                            write (b'}')
+                            write(ci.headprefix)
+                            write('{')
+                            write(h)
+                            write('}')
 
                 nlefttoskip -= 1
 
                 if nlefttoskip > 0:
-                    sep = b' '
+                    sep = ' '
                 else:
-                    sep = b' & '
+                    sep = ' & '
 
-            cr = b' \\\\\n'
+            cr = ' \\\\\n'
 
         if self.numbercols:
             colnum = 1
-            sep = b''
-            write (b' \\\\ \\\\\n')
+            sep = ''
+            write(' \\\\ \\\\\n')
 
             for ci in colinfo:
-                write (sep)
-                write (b'\\multicolumn{')
-                write (text_type (ci.nlcol).encode ('ascii'))
-                write (b'}{c}{')
+                write(sep)
+                write('\\multicolumn{')
+                write(text_type(ci.nlcol))
+                write('}{c}{')
                 if ci.numbering is False:
                     pass
-                elif b'%d' in ci.numbering:
-                    write (ci.numbering % colnum)
+                elif '%d' in ci.numbering:
+                    write(ci.numbering % colnum)
                     colnum += 1
                 else:
-                    write (ci.numbering)
-                write (b'}')
-                sep = b' & '
+                    write(ci.numbering)
+                write('}')
+                sep = ' & '
 
-        write (b'\n}\n\\startdata\n')
+        write('\n}\n\\startdata\n')
 
-        cr = b''
+        cr = ''
 
         for item in items:
-            write (cr)
-            sep = b''
+            write(cr)
+            sep = ''
 
-            rp = getattr (item, 'tb_row_preamble', None)
+            rp = getattr(item, 'tb_row_preamble', None)
             if rp is not None:
-                write (rp)
+                write(rp)
 
             for ci in colinfo:
-                write (sep)
-                formatted = ci.wdatafunc (item, ci.formatter, self)
+                write(sep)
+                formatted = ci.wdatafunc(item, ci.formatter, self)
                 try:
-                    write (formatted)
+                    write(formatted)
                 except Exception:
-                    reraise_context ('while writing %r (from %r with %r)',
-                                     formatted, item, ci.formatter)
-                sep = b' & '
+                    reraise_context('while writing %r (from %r with %r)',
+                                    formatted, item, ci.formatter)
+                sep = ' & '
 
-            cr = b' \\\\\n'
+            cr = ' \\\\\n'
 
         if self.final_double_backslash:
-            write (b' \\\\')
-        write (b'\n\\enddata\n')
+            write(' \\\\')
+        write('\n\\enddata\n')
 
-        if self.note is not None and len (self.note):
-            write (b'\\tablecomments{')
-            write (self.note)
-            write (b'}\n')
-
-        if self.refs is not None and len (self.refs):
-            write (b'\\tablerefs{')
-            write (self.refs)
-            write (b'}\n')
+        if self.note is not None and len(self.note):
+            write('\\tablecomments{')
+            write(self.note)
+            write('}\n')
+
+        if self.refs is not None and len(self.refs):
+            write('\\tablerefs{')
+            write(self.refs)
+            write('}\n')
 
-        for noteinfo in sorted ((ni for ni in itervalues (self._notes)
+        for noteinfo in sorted((ni for ni in itervalues(self._notes)
                                  if ni[0] is not None), key=lambda ni: ni[0]):
-            write (b'\\tablenotetext{')
-            write (chr (ord ('a') + noteinfo[0]).encode ('ascii'))
-            write (b'}{')
-            write (noteinfo[1])
-            write (b'}\n')
-
-        write (br'\end{')
-        write (self.environment)
-        write (b'}\n% end TableBuilder table\n')
+            write('\\tablenotetext{')
+            write(chr(ord('a') + noteinfo[0]))
+            write('}{')
+            write(noteinfo[1])
+            write('}\n')
+
+        write('\\end{')
+        write(self.environment)
+        write('}\n% end TableBuilder table\n')
 
 
-class BasicFormatter (object):
+class BasicFormatter(object):
     """Base class for formatting table cells in a TableBuilder.
 
     Generally a formatter will also provide methods for turning input data
     into fancified LaTeX output that can be used by the column's "data
     function".
 
     """
-    def colinfo (self, builder):
+    def colinfo(self, builder):
         """Return (nlcol, colspec, headprefix), where:
 
         nlcol      - The number of LaTeX columns encompassed by this logical
                      column.
         colspec    - Its LaTeX column specification (None to force user to
                      specify).
         headprefix - Prefix applied before heading items in {} (e.g.,
                      "\\colhead").
 
         """
-        return 1, None, b'\\colhead'
+        return 1, None, '\\colhead'
 
 
 
-class BoolFormatter (BasicFormatter):
+class BoolFormatter(BasicFormatter):
     """Format booleans. Attributes `truetext` and `falsetext` set what shows up
     for true and false values, respectively.
 
     """
-    truetext = b'$\\bullet$'
-    falsetext = b''
+    truetext = '$\\bullet$'
+    falsetext = ''
 
-    def colinfo (self, builder):
-        return 1, b'c', b'\\colhead'
+    def colinfo(self, builder):
+        return 1, 'c', '\\colhead'
 
-    def format (self, value):
+    def format(self, value):
         if value:
             return self.truetext
         return self.falsetext
 
 
-class MaybeNumberFormatter (BasicFormatter):
+class MaybeNumberFormatter(BasicFormatter):
     """Format Python objects. If it's a number, format it as such, without any
     fancy column alignment, but with a specifiable number of decimal places.
     Otherwise, call latexify() on it.
 
     """
-    def __init__ (self, nplaces=1, align=b'c'):
+    def __init__(self, nplaces=1, align='c'):
         self.nplaces = nplaces
         self.align = align
 
-    def colinfo (self, builder):
-        return 1, self.align, b'\\colhead'
+    def colinfo(self, builder):
+        return 1, self.align, '\\colhead'
 
-    def format (self, datum, nplaces=None):
+    def format(self, datum, nplaces=None):
         if datum is None:
-            return b''
+            return ''
 
         try:
-            v = float (datum)
+            v = float(datum)
         except TypeError:
-            return latexify (datum)
+            return latexify(datum)
         else:
             if nplaces is None:
                 nplaces = self.nplaces
-            return b'$%.*f$' % (nplaces, v)
+            return '$%.*f$' % (nplaces, v)
 
 
-class AlignedNumberFormatter (BasicFormatter):
+class AlignedNumberFormatter(BasicFormatter):
     """Format numbers. Allows the number of decimal places to be specified, and
     aligns the numbers at the decimal point.
 
     """
-    def __init__ (self, nplaces=1):
+    def __init__(self, nplaces=1):
         self.nplaces = nplaces
 
-    def colinfo (self, builder):
-        return 2, b'r@{}l', b'\\multicolumn{2}{c}'
+    def colinfo(self, builder):
+        return 2, 'r@{}l', '\\multicolumn{2}{c}'
 
-    def format (self, datum, nplaces=None):
+    def format(self, datum, nplaces=None):
         if datum is None:
-            return b' & '
+            return ' & '
         if nplaces is None:
             nplaces = self.nplaces
 
-        return latexify_n2col (float (datum), nplaces=nplaces)
+        return latexify_n2col(float(datum), nplaces=nplaces)
 
 
-class UncertFormatter (BasicFormatter):
+class UncertFormatter(BasicFormatter):
     """Format measurements (cf. pwkit.msmt) with detailed uncertainty information,
     possibly including asymmetric uncertainties. Because of the latter
     possibility, table rows have to be made extra-high to maintain evenness.
 
     """
-    strut = br'\rule{0pt}{3ex}'
+    strut = r'\rule{0pt}{3ex}'
 
-    def colinfo (self, builder):
-        return 3, b'r@{}l@{\,}l', b'\\multicolumn{3}{c}'
+    def colinfo(self, builder):
+        return 3, r'r@{}l@{\,}l', r'\multicolumn{3}{c}'
 
-    def format (self, datum, **kwargs):
+    def format(self, datum, **kwargs):
         if datum is None:
-            return b' & & ' + self.strut
-        return latexify_u3col (datum, **kwargs) + self.strut
+            return ' & & ' + self.strut
+        return latexify_u3col(datum, **kwargs) + self.strut
 
 
-class LimitFormatter (BasicFormatter):
+class LimitFormatter(BasicFormatter):
     """Format measurements (cf pwkit.msmt) with nice-looking limit information.
     Specific uncertainty information is discarded. The default formats do not
     involve fancy subscripts or superscripts, so row struts are not needed ...
     by default.
 
     """
-    strut = br''
+    strut = ''
 
-    def colinfo (self, builder):
-        return 3, br'r@{\,}r@{}l', br'\multicolumn{3}{c}'
+    def colinfo(self, builder):
+        return 3, r'r@{\,}r@{}l', r'\multicolumn{3}{c}'
 
-    def format (self, datum, **kwargs):
+    def format(self, datum, **kwargs):
         if datum is None:
-            return b' & & ' + self.strut
-        return latexify_l3col (datum, **kwargs) + self.strut
+            return ' & & ' + self.strut
+        return latexify_l3col(datum, **kwargs) + self.strut
```

### Comparing `pwkit-0.8.9/pwkit/v1msmt.py` & `pwkit-1.0.0/pwkit/msmt.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 expm1      - exp(x) - 1
 exp        - As named.
 fmtinfo    - Get (typetag, text, is_imprecise) for textual round-tripping.
 isfinite   - True if the value is well-defined and finite.
 liminfo    - Get (limtype, repval)
 limtype    - -1 if the datum is an upper limit; 1 if lower; 0 otherwise.
 log10      - As named.
-log1p      - log (1+x)
+log1p      - log(1+x)
 log2       - As named.
 log        - As named.
 negative   - -x
 reciprocal - 1/x
 repval     - Get a "representative" value if x (in case it is uncertain).
 sin        - As named.
 sqrt       - As named.
@@ -69,21 +69,21 @@
 uval_dtype                 - The Numpy dtype of Uval data (often ignored!)
 uval_nsamples              - Number of samples used when constructing Uvals
 uval_unary_math            - Dict of unary math functions operating on Uvals.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''LimitError Lval Textual Uval absolute arccos arcsin arctan cos errinfo
+__all__ = str('''LimitError Lval Textual Uval absolute arccos arcsin arctan cos errinfo
     expm1 exp fmtinfo isfinite is_measurement liminfo limtype log10 log1p log2
     log negative reciprocal repval sin sqrt square tan unwrap add divide floor_divide
     multiply power subtract true_divide typealign find_gamma_params
     pk_scoreatpercentile sample_double_norm sample_gamma lval_unary_math
     parsers scalar_unary_math textual_unary_math UQUANT_UNCERT
-    uval_default_repval_method uval_dtype uval_nsamples uval_unary_math''').split ()
+    uval_default_repval_method uval_dtype uval_nsamples uval_unary_math''').split()
 
 import operator, six
 from six.moves import range
 
 import numpy as np
 
 from . import PKError, text_type, unicode_to_str
@@ -96,37 +96,37 @@
 
 # This is a copy of scipy.stats' scoreatpercentile() function with simplified
 # functionality. This way we don't depend on scipy, and we can count on the
 # ability to handle vector `per`, which earlier versions incorrectly didn't.
 # I'm also tempted to make percentiles be in [0, 1], not [0, 100], but
 # gratuitous incompatibilities seem unwise.
 
-def pk_scoreatpercentile (a, per):
-    asort = np.sort (a)
-    vper = np.atleast_1d (per)
+def pk_scoreatpercentile(a, per):
+    asort = np.sort(a)
+    vper = np.atleast_1d(per)
 
-    if np.any ((vper < 0) | (vper > 100)):
-        raise ValueError ('`per` must be in the range [0, 100]')
+    if np.any((vper < 0) | (vper > 100)):
+        raise ValueError('`per` must be in the range [0, 100]')
 
     fidx = vper / 100. * (asort.size - 1)
     # clipping iidx here gets the right behavior for per = 100:
-    iidx = np.minimum (fidx.astype (np.int), asort.size - 2)
+    iidx = np.minimum(fidx.astype(np.int), asort.size - 2)
     res = (iidx + 1 - fidx) * asort[iidx] + (fidx - iidx) * asort[iidx + 1]
 
-    if np.isscalar (per):
+    if np.isscalar(per):
         return res[0]
     return res
 
 
 # Double-normal distribution -- that is, pasting together two normal
 # distributions with unequal left and right variances. Skew-normal distributions
 # are mathematically purer but turn out to be just obnoxiously hard to work with.
 # Double-normals are ad-hoc but also much more tractable.
 
-def sample_double_norm (mean, std_upper, std_lower, size):
+def sample_double_norm(mean, std_upper, std_lower, size):
     """Note that this function requires Scipy."""
     from scipy.special import erfinv
 
     # There's probably a better way to do this. We first draw percentiles
     # uniformly between 0 and 1. We want the peak of the distribution to occur
     # at `mean`. However, if we assign 50% of the samples to the lower half
     # and 50% to the upper half, the side with the smaller variance will be
@@ -134,73 +134,73 @@
     # PDF. Therefore we need to divide points between the two halves with a
     # fraction `cutoff` (defined below) going to the lower half. Having
     # partitioned them this way, we can then use the standard Gaussian
     # quantile function to go from percentiles to sample values -- except that
     # we must remap from [0, cutoff] to [0, 0.5] and from [cutoff, 1] to [0.5,
     # 1].
 
-    samples = np.empty (size)
-    percentiles = np.random.uniform (0., 1., size)
+    samples = np.empty(size)
+    percentiles = np.random.uniform(0., 1., size)
     cutoff = std_lower / (std_lower + std_upper)
 
     w = (percentiles < cutoff)
     percentiles[w] *= 0.5 / cutoff
-    samples[w] = mean + np.sqrt (2) * std_lower * erfinv (2 * percentiles[w] - 1)
+    samples[w] = mean + np.sqrt(2) * std_lower * erfinv(2 * percentiles[w] - 1)
 
     w = ~w
     percentiles[w] = 1 - (1 - percentiles[w]) * 0.5 / (1 - cutoff)
-    samples[w] = mean + np.sqrt (2) * std_upper * erfinv (2 * percentiles[w] - 1)
+    samples[w] = mean + np.sqrt(2) * std_upper * erfinv(2 * percentiles[w] - 1)
 
     return samples
 
 
 # Utilities for gamma distributions. We want these for values that are
 # presented as being (skew)normal but must be positive. If the uncertainty is
 # not much smaller than the value, the samples can cross zero in significant
 # numbers and lead to all sorts of bad behavior in some kinds of computation
 # (e.g., taking logarithms, which we do a lot).
 
-def sample_gamma (alpha, beta, size):
+def sample_gamma(alpha, beta, size):
     """This is mostly about recording the conversion between Numpy/Scipy
     conventions and Wikipedia conventions. Some equations:
 
     mean = alpha / beta
     variance = alpha / beta**2
     mode = (alpha - 1) / beta [if alpha > 1; otherwise undefined]
-    skewness = 2 / sqrt (alpha)
+    skewness = 2 / sqrt(alpha)
     """
 
     if alpha <= 0:
-        raise ValueError ('alpha must be positive; got %e' % alpha)
+        raise ValueError('alpha must be positive; got %e' % alpha)
     if beta <= 0:
-        raise ValueError ('beta must be positive; got %e' % beta)
-    return np.random.gamma (alpha, scale=1./beta, size=size)
+        raise ValueError('beta must be positive; got %e' % beta)
+    return np.random.gamma(alpha, scale=1./beta, size=size)
 
 
-def find_gamma_params (mode, std):
+def find_gamma_params(mode, std):
     """Given a modal value and a standard deviation, compute corresponding
     parameters for the gamma distribution.
 
     Intended to be used to replace normal distributions when the value must be
     positive and the uncertainty is comparable to the best value. Conversion
     equations determined from the relations given in the sample_gamma()
     docs.
 
     """
     if mode < 0:
-        raise ValueError ('input mode must be positive for gamma; got %e' % mode)
+        raise ValueError('input mode must be positive for gamma; got %e' % mode)
 
     var = std**2
-    beta = (mode + np.sqrt (mode**2 + 4 * var)) / (2 * var)
+    beta = (mode + np.sqrt(mode**2 + 4 * var)) / (2 * var)
     j = 2 * var / mode**2
-    alpha = (j + 1 + np.sqrt (2 * j + 1)) / j
+    alpha = (j + 1 + np.sqrt(2 * j + 1)) / j
 
     if alpha <= 1:
-        raise ValueError ('couldn\'t compute self-consistent gamma parameters: '
-                          'mode=%e std=%e alpha=%e beta=%e' % (mode, std, alpha, beta))
+        raise ValueError('couldn\'t compute self-consistent gamma parameters: '
+                         'mode=%e std=%e alpha=%e beta=%e' % (mode, std, alpha, beta))
 
     return alpha, beta
 
 
 # Scalar math.
 #
 # What's going on here is that we want to provide a library of standard math
@@ -237,52 +237,52 @@
 
 
 # The fundamental "Uval" class.
 #
 # These have a more extensive math/operator library than Lval and Textual
 # since it's so easy to implement things.
 
-def _to_uval_info (value):
-    if isinstance (value, Uval):
+def _to_uval_info(value):
+    if isinstance(value, Uval):
         return value.d
-    return float (value) # broadcasting FTW
+    return float(value) # broadcasting FTW
 
 
-def _make_uval_operator (opfunc):
-    def uvalopfunc (uval, other):
+def _make_uval_operator(opfunc):
+    def uvalopfunc(uval, other):
         try:
-            otherd = _to_uval_info (other)
+            otherd = _to_uval_info(other)
         except Exception:
             return NotImplemented
-        return Uval (opfunc (uval.d, otherd))
+        return Uval(opfunc(uval.d, otherd))
     return uvalopfunc
 
 
-def _make_uval_rev_operator (opfunc):
-    def uvalopfunc (uval, other):
+def _make_uval_rev_operator(opfunc):
+    def uvalopfunc(uval, other):
         try:
-            otherd = _to_uval_info (other)
+            otherd = _to_uval_info(other)
         except Exception:
             return NotImplemented
-        return Uval (opfunc (otherd, uval.d))
+        return Uval(opfunc(otherd, uval.d))
     return uvalopfunc
 
 
-def _make_uval_inpl_operator (opfunc):
-    def uvalopfunc (uval, other):
+def _make_uval_inpl_operator(opfunc):
+    def uvalopfunc(uval, other):
         try:
-            otherd = _to_uval_info (other)
+            otherd = _to_uval_info(other)
         except Exception:
             return NotImplemented
-        uval.d = opfunc (uval.d, otherd)
+        uval.d = opfunc(uval.d, otherd)
         return uval
     return uvalopfunc
 
 
-class Uval (object):
+class Uval(object):
     """An empirical uncertain value, represented by samples.
 
     Constructors are:
 
     - :meth:`Uval.from_other`
     - :meth:`Uval.from_fixed`
     - :meth:`Uval.from_norm`
@@ -302,80 +302,80 @@
     ``unicode() str() repr() [latexification]  + -(sub) * // / % ** += -= *= //= %= /= **= -(neg) ~ abs()``
 
     """
     __slots__ = ('d', )
 
     # Initialization.
 
-    def __init__ (self, data):
+    def __init__(self, data):
         self.d = data
 
     @staticmethod
-    def from_other (o):
-        if isinstance (o, Uval):
-            return Uval (o.d.copy ())
-        if np.isscalar (o):
-            return Uval.from_fixed (o)
-        raise ValueError ('cannot convert %r to a Uval' % o)
+    def from_other(o):
+        if isinstance(o, Uval):
+            return Uval(o.d.copy())
+        if np.isscalar(o):
+            return Uval.from_fixed(o)
+        raise ValueError('cannot convert %r to a Uval' % o)
 
     @staticmethod
-    def from_fixed (v):
-        return Uval (np.zeros (uval_nsamples, dtype=uval_dtype) + v)
+    def from_fixed(v):
+        return Uval(np.zeros(uval_nsamples, dtype=uval_dtype) + v)
 
     @staticmethod
-    def from_norm (mean, std):
+    def from_norm(mean, std):
         if std < 0:
-            raise ValueError ('std must be positive')
-        return Uval (np.random.normal (mean, std, uval_nsamples))
+            raise ValueError('std must be positive')
+        return Uval(np.random.normal(mean, std, uval_nsamples))
 
     @staticmethod
-    def from_unif (lower_incl, upper_excl):
+    def from_unif(lower_incl, upper_excl):
         if upper_excl <= lower_incl:
-            raise ValueError ('upper_excl must be greater than lower_incl')
-        return Uval (np.random.uniform (lower_incl, upper_excl, uval_nsamples))
+            raise ValueError('upper_excl must be greater than lower_incl')
+        return Uval(np.random.uniform(lower_incl, upper_excl, uval_nsamples))
 
     @staticmethod
-    def from_double_norm (mean, std_upper, std_lower):
+    def from_double_norm(mean, std_upper, std_lower):
         if std_upper <= 0:
-            raise ValueError ('double-norm upper stddev must be positive')
+            raise ValueError('double-norm upper stddev must be positive')
         if std_lower <= 0:
-            raise ValueError ('double-norm lower stddev must be positive')
-        return Uval (sample_double_norm (mean, std_upper, std_lower, uval_nsamples))
+            raise ValueError('double-norm lower stddev must be positive')
+        return Uval(sample_double_norm(mean, std_upper, std_lower, uval_nsamples))
 
     @staticmethod
-    def from_gamma (alpha, beta):
+    def from_gamma(alpha, beta):
         if alpha <= 0:
-            raise ValueError ('gamma parameter `alpha` must be positive')
+            raise ValueError('gamma parameter `alpha` must be positive')
         if beta <= 0:
-            raise ValueError ('gamma parameter `beta` must be positive')
-        return Uval (sample_gamma (alpha, beta, uval_nsamples))
+            raise ValueError('gamma parameter `beta` must be positive')
+        return Uval(sample_gamma(alpha, beta, uval_nsamples))
 
     @staticmethod
-    def from_pcount (nevents):
+    def from_pcount(nevents):
         """We assume a Poisson process. nevents is the number of events in
         some interval. The distribution of values is the distribution of the
         Poisson rate parameter given this observed number of events, where the
         "rate" is in units of events per interval of the same duration. The
         max-likelihood value is nevents, but the mean value is nevents + 1.
         The gamma distribution is obtained by assuming an improper, uniform
         prior for the rate between 0 and infinity."""
         if nevents < 0:
-            raise ValueError ('Poisson parameter `nevents` must be nonnegative')
-        return Uval (np.random.gamma (nevents + 1, size=uval_nsamples))
+            raise ValueError('Poisson parameter `nevents` must be nonnegative')
+        return Uval(np.random.gamma(nevents + 1, size=uval_nsamples))
 
 
     # Interrogation. Would be nice to have a way to estimate the
     # distribution's mode -- when a scientist writes V = X +- Y, I think they
     # usually think of X as the maximum likelihood value, which is the modal
     # value. Maybe a kernel density estimator do this sensibly? Anyway, I
     # don't think we're in a position to unilaterally declare what the "best"
     # representative value is, so we provide options and let the caller
     # decide.
 
-    def repvals (self, method):
+    def repvals(self, method):
         """Compute representative statistical values for this Uval. `method`
         may be either 'pct' or 'gauss'.
 
         Returns (best, plus_one_sigma, minus_one_sigma), where `best` is the
         "best" value in some sense, and the others correspond to values at
         the ~84 and 16 percentile limits, respectively. Because of the
         sampled nature of the Uval system, there is no single method to
@@ -385,85 +385,85 @@
         values.
 
         The "gauss" method computes the mean μ and standard deviation σ of the
         samples and returns [μ, μ+σ, μ-σ].
 
         """
         if method == 'pct':
-            return pk_scoreatpercentile (self.d, [50., 84.134, 15.866])
+            return pk_scoreatpercentile(self.d, [50., 84.134, 15.866])
         if method == 'gauss':
-            m, s = self.d.mean (), self.d.std ()
-            return np.asarray ([m, m + s, m - s])
-        raise ValueError ('unknown representative-value method "%s"' % method)
+            m, s = self.d.mean(), self.d.std()
+            return np.asarray([m, m + s, m - s])
+        raise ValueError('unknown representative-value method "%s"' % method)
 
 
     # Textualization.
 
-    def text_pieces (self, method, uplaces=2):
+    def text_pieces(self, method, uplaces=2, use_exponent=True):
         """Return (main, dhigh, dlow, sharedexponent), all as strings. The
         delta terms do not have sign indicators. Any item except the first
         may be None.
 
         `method` is passed to Uval.repvals() to compute representative
         statistical limits.
 
         """
-        md, hi, lo = self.repvals (method)
+        md, hi, lo = self.repvals(method)
 
         if hi == lo:
             return '%g' % lo, None, None, None
 
-        if not np.isfinite ([lo, md, hi]).all ():
-            raise ValueError ('got nonfinite values when formatting Uval')
+        if not np.isfinite([lo, md, hi]).all():
+            raise ValueError('got nonfinite values when formatting Uval')
 
         # Deltas. Round to limited # of places because we don't actually know
         # the fourth moment of the thing we're trying to describe.
 
         from numpy import abs, ceil, floor, log10
 
         dh = hi - md
         dl = md - lo
 
         if dh <= 0:
-            raise ValueError ('strange problem formatting Uval; '
-                              'hi=%g md=%g dh=%g' % (hi, md, dh))
+            raise ValueError('strange problem formatting Uval; '
+                             'hi=%g md=%g dh=%g' % (hi, md, dh))
         if dl <= 0:
-            raise ValueError ('strange problem formatting Uval; '
-                              'lo=%g md=%g dl=%g' % (lo, md, dl))
+            raise ValueError('strange problem formatting Uval; '
+                             'lo=%g md=%g dl=%g' % (lo, md, dl))
 
-        p = int (ceil (log10 (dh)))
-        rdh = round (dh * 10**(-p), uplaces) * 10**p
-        p = int (ceil (log10 (dl)))
-        rdl = round (dl * 10**(-p), uplaces) * 10**p
+        p = int(ceil(log10(dh)))
+        rdh = round(dh * 10**(-p), uplaces) * 10**p
+        p = int(ceil(log10(dl)))
+        rdl = round(dl * 10**(-p), uplaces) * 10**p
 
         # The least significant place to worry about is the L.S.P. of one of
         # the deltas, which we can find relative to its M.S.P. Any precision
         # in the datum beyond this point is false.
 
-        lsp = int (ceil (log10 (min (rdh, rdl)))) - uplaces
+        lsp = int(ceil(log10(min(rdh, rdl)))) - uplaces
 
         # We should round the datum since it might be something like
         # 0.999+-0.1 and we're about to try to decide what its most
         # significant place is. Might get -1 rather than 0.
 
-        rmd = round (md, -lsp)
+        rmd = round(md, -lsp)
 
         if rmd == -0.: # 0 = -0, too, but no problem there.
             rmd = 0.
 
         # The most significant place to worry about is the M.S.P. of any of
         # the datum or the deltas. rdl and rdl must be positive, but not
         # necessarily rmd.
 
-        msp = int (floor (log10 (max (abs (rmd), rdh, rdl))))
+        msp = int(floor(log10(max(abs(rmd), rdh, rdl))))
 
-        # If we're not very large or very small, don't use scientific
-        # notation.
+        # If we're not very large or very small, or it's been explicitly
+        # disabled, don't use scientific notation.
 
-        if msp > -3 and msp < 3:
+        if (msp > -3 and msp < 3) or not use_exponent:
             srmd = '%.*f' % (-lsp, rmd)
             srdh = '%.*f' % (-lsp, rdh)
             srdl = '%.*f' % (-lsp, rdl)
             return srmd, srdh, srdl, None
 
         # Use scientific notation. Adjust values, then format.
 
@@ -471,64 +471,64 @@
         ardh = rdh * 10**-msp
         ardl = rdl * 10**-msp
         prec = msp - lsp
 
         sarmd = '%.*f' % (prec, armd)
         sardh = '%.*f' % (prec, ardh)
         sardl = '%.*f' % (prec, ardl)
-        return sarmd, sardh, sardl, str (msp)
+        return sarmd, sardh, sardl, str(msp)
 
 
-    def format (self, method, parenexp=True, uplaces=2):
-        main, dh, dl, exp = self.text_pieces (method, uplaces=uplaces)
+    def format(self, method, parenexp=True, uplaces=2, use_exponent=True):
+        main, dh, dl, exp = self.text_pieces(method, uplaces=uplaces, use_exponent=use_exponent)
 
         if exp is not None and not parenexp:
             main += 'e' + exp
             if dh is not None:
                 dh += 'e' + exp
             if dl is not None:
                 dl += 'e' + exp
 
         if dh is None:
             pmterm = ''
         elif dh == dl:
             pmterm = 'pm' + dh
         else:
-            pmterm = ''.join (['p', dh, 'm', dl])
+            pmterm = ''.join(['p', dh, 'm', dl])
 
         if exp is not None and parenexp:
             return '(%s%s)e%s' % (main, pmterm, exp)
 
         return main + pmterm
 
 
-    def __unicode__ (self):
+    def __unicode__(self):
         try:
-            return self.format (uval_default_repval_method)
+            return self.format(uval_default_repval_method)
         except ValueError:
             return '{bad samples}'
 
     __str__ = unicode_to_str
 
 
-    def __repr__ (self):
-        formatted = self.format (uval_default_repval_method)
-        v = pk_scoreatpercentile (self.d, [0, 2.5, 50, 97.5, 100])
+    def __repr__(self):
+        formatted = self.format(uval_default_repval_method)
+        v = pk_scoreatpercentile(self.d, [0, 2.5, 50, 97.5, 100])
         return '<Uval %s [min=%g l95=%g med=%g u95=%g max=%g]>' % \
-            ((formatted, ) + tuple (v))
+            ((formatted, ) + tuple(v))
 
 
-    def __pk_fmtinfo__ (self):
-        return 'u', self.format ('pct', parenexp=False), True
+    def __pk_fmtinfo__(self):
+        return 'u', self.format('pct', parenexp=False), True
 
 
-    def __pk_latex__ (self, method=None, uplaces=1, **kwargs):
+    def __pk_latex__(self, method=None, uplaces=1, use_exponent=True, **kwargs):
         if method is None:
             method = uval_default_repval_method
-        main, dh, dl, exp = self.text_pieces (method, uplaces=uplaces)
+        main, dh, dl, exp = self.text_pieces(method, uplaces=uplaces, use_exponent=use_exponent)
 
         if dh is None:
             return r'$%s$' % main
 
         if dh == dl:
             pmterm = r'\pm %s' % dh
         else:
@@ -536,186 +536,186 @@
 
         if exp is None:
             return '$%s %s$' % (main, pmterm)
 
         return r'$(%s %s) \times 10^{%s}$' % (main, pmterm, exp)
 
 
-    def __pk_latex_l3col__ (self, method=None, **kwargs):
+    def __pk_latex_l3col__(self, method=None, **kwargs):
         if method is None:
             method = uval_default_repval_method
-        v = self.repvals (method)[0]
+        v = self.repvals(method)[0]
 
         from .latex import latexify_n2col
-        return b'$\\sim$ & ' + latexify_n2col (v, **kwargs)
+        return b'$\\sim$ & ' + latexify_n2col(v, **kwargs)
 
 
-    def __pk_latex_u3col__ (self, method=None, uplaces=1, **kwargs):
+    def __pk_latex_u3col__(self, method=None, uplaces=1, use_exponent=True, **kwargs):
         if method is None:
             method = uval_default_repval_method
-        main, dh, dl, exp = self.text_pieces (method, uplaces=uplaces)
+        main, dh, dl, exp = self.text_pieces(method, uplaces=uplaces, use_exponent=use_exponent)
 
         if dh is None:
             return r'\multicolumn{3}{c}{$%s$}' % main
 
         if dh == dl:
             pmterm = r'$\pm\,%s$' % dh
         else:
             pmterm = r'$\pm\,^{%s}_{%s}$' % (dh, dl)
 
         if '.' not in main:
             mainterm = r'$%s$ & ' % main
         else:
-            mainterm = r'$%s$ & $.%s$' % tuple (main.split ('.'))
+            mainterm = r'$%s$ & $.%s$' % tuple(main.split('.'))
 
         if exp is None:
             return mainterm + ' & ' + pmterm
 
-        return ''.join (['$($', mainterm, ' & ', pmterm,
-                         r'$) \times 10^{%s}$' % exp])
+        return ''.join(['$($', mainterm, ' & ', pmterm,
+                        r'$) \times 10^{%s}$' % exp])
 
 
     # math -- http://docs.python.org/2/reference/datamodel.html#emulating-numeric-types
 
-    __add__ = _make_uval_operator (operator.add)
-    __sub__ = _make_uval_operator (operator.sub)
-    __mul__ = _make_uval_operator (operator.mul)
-    __floordiv__ = _make_uval_operator (operator.floordiv)
-    __mod__ = _make_uval_operator (operator.mod)
-    __divmod__ = _make_uval_operator (divmod)
-    __pow__ = _make_uval_operator (operator.pow)
+    __add__ = _make_uval_operator(operator.add)
+    __sub__ = _make_uval_operator(operator.sub)
+    __mul__ = _make_uval_operator(operator.mul)
+    __floordiv__ = _make_uval_operator(operator.floordiv)
+    __mod__ = _make_uval_operator(operator.mod)
+    __divmod__ = _make_uval_operator(divmod)
+    __pow__ = _make_uval_operator(operator.pow)
     # skipped: lshift, rshift, and, xor, or
     # used to do div too; Python 3 has no operator.div
-    __truediv__ = _make_uval_operator (operator.truediv)
+    __truediv__ = _make_uval_operator(operator.truediv)
 
-    __radd__ = _make_uval_rev_operator (operator.add)
-    __rsub__ = _make_uval_rev_operator (operator.sub)
-    __rmul__ = _make_uval_rev_operator (operator.mul)
-    __rfloordiv__ = _make_uval_rev_operator (operator.floordiv)
-    __rmod__ = _make_uval_rev_operator (operator.mod)
-    __rdivmod__ = _make_uval_rev_operator (divmod)
-    __rpow__ = _make_uval_rev_operator (operator.pow)
+    __radd__ = _make_uval_rev_operator(operator.add)
+    __rsub__ = _make_uval_rev_operator(operator.sub)
+    __rmul__ = _make_uval_rev_operator(operator.mul)
+    __rfloordiv__ = _make_uval_rev_operator(operator.floordiv)
+    __rmod__ = _make_uval_rev_operator(operator.mod)
+    __rdivmod__ = _make_uval_rev_operator(divmod)
+    __rpow__ = _make_uval_rev_operator(operator.pow)
     # skipped: rlshift, rrshift, rand, rxor, ror
     # as above, used to do rdiv too
-    __rtruediv__ = _make_uval_rev_operator (operator.truediv)
+    __rtruediv__ = _make_uval_rev_operator(operator.truediv)
 
-    __iadd__ = _make_uval_inpl_operator (operator.iadd)
-    __isub__ = _make_uval_inpl_operator (operator.isub)
-    __imul__ = _make_uval_inpl_operator (operator.imul)
-    __ifloordiv__ = _make_uval_inpl_operator (operator.ifloordiv)
-    __imod__ = _make_uval_inpl_operator (operator.imod)
-    __ipow__ = _make_uval_inpl_operator (operator.ipow)
+    __iadd__ = _make_uval_inpl_operator(operator.iadd)
+    __isub__ = _make_uval_inpl_operator(operator.isub)
+    __imul__ = _make_uval_inpl_operator(operator.imul)
+    __ifloordiv__ = _make_uval_inpl_operator(operator.ifloordiv)
+    __imod__ = _make_uval_inpl_operator(operator.imod)
+    __ipow__ = _make_uval_inpl_operator(operator.ipow)
     # skipped: ilshift, irshift, iand, ixor, ior
     # as above, used to do idiv too
-    __itruediv__ = _make_uval_inpl_operator (operator.itruediv)
+    __itruediv__ = _make_uval_inpl_operator(operator.itruediv)
 
-    def __neg__ (self):
+    def __neg__(self):
         self.d = -self.d
         return self
 
-    def __pos__ (self):
+    def __pos__(self):
         self.d = +self.d
         return self
 
-    def __abs__ (self):
-        self.d = np.abs (self.d)
+    def __abs__(self):
+        self.d = np.abs(self.d)
         return self
 
-    def __invert__ (self):
+    def __invert__(self):
         self.d = ~self.d
         return self
 
-    def __nonzero__ (self):
-        raise TypeError ('uncertain value cannot be reduced to a boolean scalar')
+    def __nonzero__(self):
+        raise TypeError('uncertain value cannot be reduced to a boolean scalar')
 
-    def __complex__ (self):
-        raise TypeError ('uncertain value cannot be reduced to a complex scalar')
+    def __complex__(self):
+        raise TypeError('uncertain value cannot be reduced to a complex scalar')
 
-    def __int__ (self):
-        raise TypeError ('uncertain value cannot be reduced to an integer scalar')
+    def __int__(self):
+        raise TypeError('uncertain value cannot be reduced to an integer scalar')
 
-    def __long__ (self):
-        raise TypeError ('uncertain value cannot be reduced to a long-integer scalar')
+    def __long__(self):
+        raise TypeError('uncertain value cannot be reduced to a long-integer scalar')
 
-    def __float__ (self):
-        raise TypeError ('uncertain value cannot be reduced to a float scalar')
+    def __float__(self):
+        raise TypeError('uncertain value cannot be reduced to a float scalar')
 
     # skipped: oct, hex, index, coerce
 
-    def __lt__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined "<" comparison')
+    def __lt__(self, other):
+        raise TypeError('uncertain value does not have a well-defined "<" comparison')
 
-    def __le__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined "<" comparison')
+    def __le__(self, other):
+        raise TypeError('uncertain value does not have a well-defined "<" comparison')
 
-    def __eq__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined "==" comparison')
+    def __eq__(self, other):
+        raise TypeError('uncertain value does not have a well-defined "==" comparison')
 
-    def __ne__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined "!=" comparison')
+    def __ne__(self, other):
+        raise TypeError('uncertain value does not have a well-defined "!=" comparison')
 
-    def __gt__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined ">" comparison')
+    def __gt__(self, other):
+        raise TypeError('uncertain value does not have a well-defined ">" comparison')
 
-    def __ge__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined ">=" comparison')
+    def __ge__(self, other):
+        raise TypeError('uncertain value does not have a well-defined ">=" comparison')
 
-    def __cmp__ (self, other):
-        raise TypeError ('uncertain value does not have a well-defined __cmp__ comparison')
+    def __cmp__(self, other):
+        raise TypeError('uncertain value does not have a well-defined __cmp__ comparison')
 
     __hash__ = None
 
 
-    def debug_distribution (self):
+    def debug_distribution(self):
         import omega as om
 
-        v = pk_scoreatpercentile (self.d, [50, 0, 0.270, 2.5, 97.5, 99.730, 100])
+        v = pk_scoreatpercentile(self.d, [50, 0, 0.270, 2.5, 97.5, 99.730, 100])
         median = v[0]
         v = v[1:]
 
-        print ('median=%g mean=%g'
-               % (median, self.d.mean ()))
-        print ('   abs: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g'
-               % tuple (v))
-        print ('   rel: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g'
-               % tuple (v - median))
-        print ('   scl: min=%.2f l3σ=%.2f l95%%=%.2f .. u95%%=%.2f u3σ=%.2f max=%.2f'
-               % tuple ((v - median) / np.abs (median)))
-        return om.quickHist (self.d, bins=25)
+        print('median=%g mean=%g'
+              % (median, self.d.mean()))
+        print('   abs: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g'
+              % tuple(v))
+        print('   rel: min=%g l3σ=%g l95%%=%g .. u95%%=%g u3σ=%g max=%g'
+              % tuple(v - median))
+        print('   scl: min=%.2f l3σ=%.2f l95%%=%.2f .. u95%%=%.2f u3σ=%.2f max=%.2f'
+              % tuple((v - median) / np.abs(median)))
+        return om.quickHist(self.d, bins=25)
 
 
-def _make_uval_unary_math (scalarfunc):
-    def uval_unary_math (v):
-        return Uval (scalarfunc (_to_uval_info (v)))
+def _make_uval_unary_math(scalarfunc):
+    def uval_unary_math(v):
+        return Uval(scalarfunc(_to_uval_info(v)))
     return uval_unary_math
 
 
-def _uval_unary_isfinite (v):
-    return np.all (np.isfinite (_to_uval_info (v)))
+def _uval_unary_isfinite(v):
+    return np.all(np.isfinite(_to_uval_info(v)))
 
 
 uval_unary_math = {
-    'absolute': _make_uval_unary_math (np.absolute),
-    'arccos': _make_uval_unary_math (np.arccos),
-    'arcsin': _make_uval_unary_math (np.arcsin),
-    'arctan': _make_uval_unary_math (np.arctan),
-    'cos': _make_uval_unary_math (np.cos),
-    'expm1': _make_uval_unary_math (np.expm1),
-    'exp': _make_uval_unary_math (np.exp),
+    'absolute': _make_uval_unary_math(np.absolute),
+    'arccos': _make_uval_unary_math(np.arccos),
+    'arcsin': _make_uval_unary_math(np.arcsin),
+    'arctan': _make_uval_unary_math(np.arctan),
+    'cos': _make_uval_unary_math(np.cos),
+    'expm1': _make_uval_unary_math(np.expm1),
+    'exp': _make_uval_unary_math(np.exp),
     'isfinite': _uval_unary_isfinite,
-    'log10': _make_uval_unary_math (np.log10),
-    'log1p': _make_uval_unary_math (np.log1p),
-    'log2': _make_uval_unary_math (np.log2),
-    'log': _make_uval_unary_math (np.log),
-    'negative': _make_uval_unary_math (np.negative),
-    'reciprocal': _make_uval_unary_math (lambda x: 1. / x),
-    'sin': _make_uval_unary_math (np.sin),
-    'sqrt': _make_uval_unary_math (np.sqrt),
-    'square': _make_uval_unary_math (np.square),
-    'tan': _make_uval_unary_math (np.tan),
+    'log10': _make_uval_unary_math(np.log10),
+    'log1p': _make_uval_unary_math(np.log1p),
+    'log2': _make_uval_unary_math(np.log2),
+    'log': _make_uval_unary_math(np.log),
+    'negative': _make_uval_unary_math(np.negative),
+    'reciprocal': _make_uval_unary_math(lambda x: 1. / x),
+    'sin': _make_uval_unary_math(np.sin),
+    'sqrt': _make_uval_unary_math(np.sqrt),
+    'square': _make_uval_unary_math(np.square),
+    'tan': _make_uval_unary_math(np.tan),
 }
 
 
 # Now, limiting values. I tried to do this within the context of the Uval
 # system, but it just never worked in a way that gave the results that people
 # would naively expect. Lvals are one level "above" Uvals: Lvals know about
 # Uvals, but not the other way around.
@@ -788,116 +788,116 @@
 _lval_kmap_exp = _lval_kmap_pow_above_one # same behavior
 
 _lval_kmap_log = {
     'tozero': 'pastzero',
 }
 
 
-class LimitError (PKError):
-    def __init__ (self):
-        super (LimitError, self).__init__ ('forbidden operation on a limit value')
+class LimitError(PKError):
+    def __init__(self):
+        super(LimitError, self).__init__('forbidden operation on a limit value')
 
 
-def _ordpair (v1, v2):
+def _ordpair(v1, v2):
     if v1 > v2:
         return (v2, v1)
     return (v1, v2)
 
 
-def _lval_add_towards_polarity (x, polarity):
+def _lval_add_towards_polarity(x, polarity):
     """Compute the appropriate Lval "kind" for the limit of value `x` towards
     `polarity`. Either 'toinf' or 'pastzero' depending on the sign of `x` and
     the infinity direction of polarity.
 
     """
     if x < 0:
         if polarity < 0:
-            return Lval ('toinf', x)
-        return Lval ('pastzero', x)
+            return Lval('toinf', x)
+        return Lval('pastzero', x)
     elif polarity > 0:
-        return Lval ('toinf', x)
-    return Lval ('pastzero', x)
+        return Lval('toinf', x)
+    return Lval('pastzero', x)
 
 
-class Lval (object):
+class Lval(object):
     """A container for either precise values or upper/lower limits. Constructed as
-    ``Lval (kind, value)``, where *kind* is ``"exact"``, ``"uncertain"``,
+    ``Lval(kind, value)``, where *kind* is ``"exact"``, ``"uncertain"``,
     ``"toinf"``, ``"tozero"``, ``"pastzero"``, or ``"undef"``. Most easily
     constructed via :meth:`Textual.parse`. Can also be constructed with
     :meth:`Lval.from_other`.
 
     Supported operations are
     ``unicode() str() repr() -(neg) abs() + - * / ** += -= *= /= **=``.
 
     """
     __slots__ = ('kind', 'value')
 
-    def __init__ (self, kind, value):
+    def __init__(self, kind, value):
         if kind not in _lval_pos_sigils:
-            raise ValueError ('unrecognized Lval kind %r' % kind)
-        if not np.isscalar (value):
-            raise ValueError ('Lvals must be scalars; got %r' % value)
+            raise ValueError('unrecognized Lval kind %r' % kind)
+        if not np.isscalar(value):
+            raise ValueError('Lvals must be scalars; got %r' % value)
         self.kind = kind
         self.value = value
 
     @staticmethod
-    def from_other (o):
-        if isinstance (o, Lval):
+    def from_other(o):
+        if isinstance(o, Lval):
             from copy import copy
-            return Lval (o.kind, copy (o.value))
-        if isinstance (o, Uval):
-            return Lval ('uncertain', o.repvals (uval_default_repval_method)[0])
-        if np.isscalar (o):
-            return Lval ('exact', float (o))
-        raise ValueError ('cannot convert %r to an Lval' % o)
+            return Lval(o.kind, copy(o.value))
+        if isinstance(o, Uval):
+            return Lval('uncertain', o.repvals(uval_default_repval_method)[0])
+        if np.isscalar(o):
+            return Lval('exact', float(o))
+        raise ValueError('cannot convert %r to an Lval' % o)
 
     # Textualization.
 
-    def __unicode__ (self):
+    def __unicode__(self):
         s = _lval_pos_sigils[self.kind]
         if self.value < 0:
             if s == '>':
                 s = '<'
             else:
-                s = s.replace ('<', '>')
+                s = s.replace('<', '>')
         return '%s%g' % (s, self.value)
 
     __str__ = unicode_to_str
 
-    def __repr__ (self):
+    def __repr__(self):
         return 'Lval(%r, %r)' % (self.kind, self.value)
 
-    def __pk_fmtinfo__ (self):
+    def __pk_fmtinfo__(self):
         # Only certain kinds of Lval can successfully be roundtripped through
         # text. Positive 'tozero' values need the 'P' flag; negative tozeros
         # are inexpressible.
         if self.kind == 'undef' or (self.kind == 'tozero' and self.value < 0):
-            raise ValueError ('no fmtinfo textualization of %r is possible' % self)
+            raise ValueError('no fmtinfo textualization of %r is possible' % self)
 
         if self.kind == 'tozero':
             return 'Pu', '<%g' % self.value, True
 
         s = _lval_pos_sigils[self.kind][0] # note: truncating << pastzero mode.
         if self.value < 0:
             if s == '>': # toinf, but we're negative.
                 s = '<'
             else: # tozero disallowed, so we must be pastzero
                 s = '>'
 
         return 'u', '%s%g' % (s, self.value), True
 
 
-    def __pk_latex__ (self, undefok=False, **kwargs):
+    def __pk_latex__(self, undefok=False, **kwargs):
         from .latex import latexify
-        base = latexify (self.value, **kwargs)
+        base = latexify(self.value, **kwargs)
 
         if self.kind == 'undef':
             if undefok:
                 return b''
-            raise ValueError ('tried to LaTeXify undefined Lval')
+            raise ValueError('tried to LaTeXify undefined Lval')
 
         if self.kind == 'exact':
             return b'' + base
 
         if self.kind == 'uncertain':
             return b'$\\sim$' + base
 
@@ -907,22 +907,22 @@
                 s = '<'
             else:
                 s = '>'
 
         return b'$%s$%s' % (s, base)
 
 
-    def __pk_latex_l3col__ (self, undefok=False, **kwargs):
+    def __pk_latex_l3col__(self, undefok=False, **kwargs):
         from .latex import latexify_n2col
-        base = latexify_n2col (self.value, **kwargs)
+        base = latexify_n2col(self.value, **kwargs)
 
         if self.kind == 'undef':
             if undefok:
                 return b' & & '
-            raise ValueError ('tried to LaTeXify undefined Lval')
+            raise ValueError('tried to LaTeXify undefined Lval')
 
         if self.kind == 'exact':
             return b'& ' + base
 
         if self.kind == 'uncertain':
             return b'$\\sim$ & ' + base
 
@@ -932,23 +932,27 @@
                 s = '<'
             else:
                 s = '>'
 
         return b'$%s$ & %s' % (s, base)
 
 
+    def __pk_latex_u3col__(self, **kwargs):
+        return br'\multicolumn{3}{c}{%s}' % self.__pk_latex__(**kwargs)
+
+
     # Math. We start with addition. It gets complicated!
 
-    def __neg__ (self):
-        return _lval_unary_negative (self)
+    def __neg__(self):
+        return _lval_unary_negative(self)
 
-    def __abs__ (self):
-        return _lval_unary_absolute (self)
+    def __abs__(self):
+        return _lval_unary_absolute(self)
 
-    def _polarity (self):
+    def _polarity(self):
         # -2  --  limit towards -infinity
         # -1  --  limit from a negative value to zero
         # 0   --  not a limit
         # +1  --  limit from a positive value to zero
         # +2  --  limit towards +infinity
 
         assert self.kind != 'undef'
@@ -966,356 +970,356 @@
         if self.kind == 'toinf':
             return +2
         if self.kind == 'tozero':
             return +1
         return -2
 
 
-    def __add__ (self, other):
+    def __add__(self, other):
         v1 = self
-        v2 = Lval.from_other (other)
+        v2 = Lval.from_other(other)
         tot = v1.value + v2.value
 
         # Rule 1: undef trumps all.
         if v1.kind == 'undef' or v2.kind == 'undef':
-            return Lval ('undef', tot)
+            return Lval('undef', tot)
 
         # Rule(s) 2: some combinations with exact/uncert values require no
         # checking of the kind or polarity.
-        k = _lval_kmap_add_unconditional.get (_ordpair (v1.kind, v2.kind))
+        k = _lval_kmap_add_unconditional.get(_ordpair(v1.kind, v2.kind))
         if k is not None:
-            return Lval (k, tot)
+            return Lval(k, tot)
 
         # Rule 3: if values have same sign and same kind, we can add
         # without needing to worry about changing the kind.
-        s1, s2 = np.sign (v1.value), np.sign (v2.value)
+        s1, s2 = np.sign(v1.value), np.sign(v2.value)
         if s1 == 0:
             s1 = 1.
         if s2 == 0:
             s2 = 1.
 
         if s1 == s2 and v1.kind == v2.kind:
-            return Lval (v1.kind, tot)
+            return Lval(v1.kind, tot)
 
         # Undefs and exact-ish pairs were dealt with in Rules 1 and 2; to-zero
         # and exact-ish were dealt with in Rule 2, and same-sign-same-kind was
         # dealt with in Rule 3. Therefore if we have two to-zeros, they must
         # be of opposite polarity. Rule 4: this goes to undef.
 
-        p1, p2 = v1._polarity (), v2._polarity ()
+        p1, p2 = v1._polarity(), v2._polarity()
 
-        if max (abs (p1), abs (p2)) == 1:
+        if max(abs(p1), abs(p2)) == 1:
             assert p1 == -p2
-            return Lval ('undef', tot)
+            return Lval('undef', tot)
 
         # The only remaining possibility is a combination of a limit to
         # infinity and something else. Make sure that p1 holds an infinity
         # limit.
 
-        if abs (p1) < 2:
+        if abs(p1) < 2:
             v1, v2 = v2, v1
             s1, s2 = s2, s1
             p1, p2 = p2, p1
 
         # Rule 5: to-infs of opposite signs go to undef.
         if p2 == -p1:
-            return Lval ('undef', tot)
+            return Lval('undef', tot)
 
         # Rule 6: to-infs of same sign are add-and-normalize.
         if p1 == p2:
-            return _lval_add_towards_polarity (tot, p1)
+            return _lval_add_towards_polarity(tot, p1)
 
         # Rule 7: to-inf and to-zero of same polarity give the to-inf.
         # Rule 8: to-inf and to-zero of opposite polarity are add-and-normalize.
-        if np.abs (p2) == 1:
+        if np.abs(p2) == 1:
             if p1 * p2 > 0:
                 return v1
-            return _lval_add_towards_polarity (tot, p1)
+            return _lval_add_towards_polarity(tot, p1)
 
         # Rule 9: to-inf and constant-ish are add-and-normalize.
         if p2 == 0:
-            return _lval_add_towards_polarity (tot, p1)
+            return _lval_add_towards_polarity(tot, p1)
 
         assert False, 'not reached'
 
     __radd__ = __add__
 
-    def __sub__ (self, other):
-        other = Lval.from_other (other)
+    def __sub__(self, other):
+        other = Lval.from_other(other)
         other = -other
         return self + other
 
-    def __rsub__ (self, other):
-        other = Lval.from_other (other)
+    def __rsub__(self, other):
+        other = Lval.from_other(other)
         return other + -self
 
-    def __iadd__ (self, other):
-        other = Lval.from_other (other)
+    def __iadd__(self, other):
+        other = Lval.from_other(other)
         tmp = self + other
         self.kind, self.value = tmp.kind, tmp.value
         return self
 
-    def __isub__ (self, other):
-        other = Lval.from_other (other)
+    def __isub__(self, other):
+        other = Lval.from_other(other)
         other = -other
         tmp = self + other
         self.kind, self.value = tmp.kind, tmp.value
         return self
 
     # Multiplication!
 
-    def __mul__ (self, other):
+    def __mul__(self, other):
         v1 = self
-        v2 = Lval.from_other (other)
+        v2 = Lval.from_other(other)
         negative = False
 
         if v1.value < 0:
             negative = not negative
             v1 = -v1
 
         if v2.value < 0:
             negative = not negative
             v2 = -v2
 
         prod = v1.value * v2.value
 
         if v1.kind == 'undef' or v2.kind == 'undef':
-            return Lval ('undef', prod)
+            return Lval('undef', prod)
 
-        ordkind = _ordpair (v1.kind, v2.kind)
+        ordkind = _ordpair(v1.kind, v2.kind)
 
-        if ordkind == ('toinf', 'tozero'):
-            rv = Lval ('toinf', 0.)
+        if ordkind ==('toinf', 'tozero'):
+            rv = Lval('toinf', 0.)
         else:
-            rv = Lval (_lval_kmap_mul[ordkind], prod)
+            rv = Lval(_lval_kmap_mul[ordkind], prod)
 
         if negative:
             return -rv
         return rv
 
     __rmul__ = __mul__
 
-    def __div__ (self, other):
-        other = Lval.from_other (other)
-        other = _lval_unary_reciprocal (other)
+    def __div__(self, other):
+        other = Lval.from_other(other)
+        other = _lval_unary_reciprocal(other)
         return self * other
 
-    def __rdiv__ (self, other):
-        other = Lval.from_other (other)
-        tmp = _lval_unary_reciprocal (self)
+    def __rdiv__(self, other):
+        other = Lval.from_other(other)
+        tmp = _lval_unary_reciprocal(self)
         return other * tmp
 
     __truediv__ = __div__
 
     __rtruediv__ = __rdiv__
 
-    def __imul__ (self, other):
-        other = Lval.from_other (other)
+    def __imul__(self, other):
+        other = Lval.from_other(other)
         tmp = self * other
         self.kind, self.value = tmp.kind, tmp.value
         return self
 
-    def __idiv__ (self, other):
-        other = Lval.from_other (other)
-        other = _lval_unary_reciprocal (other)
+    def __idiv__(self, other):
+        other = Lval.from_other(other)
+        other = _lval_unary_reciprocal(other)
         tmp = self * other
         self.kind, self.value = tmp.kind, tmp.value
         return self
 
     __itruediv__ = __idiv__
 
     # Exponentiation.
 
-    def __pow__ (self, other, modulo=None):
+    def __pow__(self, other, modulo=None):
         if modulo is not None:
-            raise ValueError ('powmod behavior forbidden with Lvals')
+            raise ValueError('powmod behavior forbidden with Lvals')
 
         try:
-            v = float (other)
+            v = float(other)
         except TypeError:
-            raise ValueError ('Lvals can only be exponentiated by exact values')
+            raise ValueError('Lvals can only be exponentiated by exact values')
 
         if self.kind == 'undef':
             # It's not worth trying to get a reasonable value in this case.
-            return Lval ('undef', np.nan)
+            return Lval('undef', np.nan)
 
         if v == 0:
-            return Lval ('exact', 1.)
+            return Lval('exact', 1.)
 
         reciprocate = (v < 0)
         if reciprocate:
             v = -v
 
-        i = int (v)
+        i = int(v)
 
         if v != i:
             # For us, fractional powers are only defined on positive numbers,
             # which gives us a fairly small number of valid cases to worry
             # about.
             if self.value <= 0 or self.kind == 'pastzero':
-                return Lval ('undef', np.nan)
-            rv = Lval (self.kind, self.value**v)
+                return Lval('undef', np.nan)
+            rv = Lval(self.kind, self.value**v)
         else:
             # We can deal with integer exponentiation as a series of
             # multiplies. Not the most efficient, but reduces the chance for
             # bugs.
-            rv = Lval.from_other (self)
-            for _ in range (i - 1):
+            rv = Lval.from_other(self)
+            for _ in range(i - 1):
                 rv *= self
 
         if reciprocate:
-            rv = _lval_unary_reciprocal (rv)
+            rv = _lval_unary_reciprocal(rv)
         return rv
 
 
-    def __rpow__ (self, other, modulo=None):
+    def __rpow__(self, other, modulo=None):
         if modulo is not None:
-            raise ValueError ('powmod behavior forbidden with Lvals')
+            raise ValueError('powmod behavior forbidden with Lvals')
 
         if self.kind == 'undef':
-            return Lval ('undef', np.nan)
+            return Lval('undef', np.nan)
 
         if self.kind == 'exact':
             # In this very special case, we can delegate.
             return other ** self.value
 
         # In all other cases, we're exponentiating by a fractional value,
         # so we're only valid for nonnegative numbers.
 
         try:
-            v = float (other)
+            v = float(other)
         except TypeError:
-            raise ValueError ('Lvals can only exponentiate exact values')
+            raise ValueError('Lvals can only exponentiate exact values')
 
         if v < 0:
-            raise ValueError ('Lvals can only exponentiate nonnegative values')
+            raise ValueError('Lvals can only exponentiate nonnegative values')
 
         reciprocate = (self.value < 0)
         exponent = self # NOTE: no use of 'self' from here on out!
         if reciprocate:
             exponent = -exponent
 
         if v == 0:
             if exponent.kind == 'pastzero':
-                return Lval ('undef', np.nan)
+                return Lval('undef', np.nan)
             # We ignore the fact that 0**0 = 1.
-            rv = Lval ('exact', 0.)
+            rv = Lval('exact', 0.)
         elif v < 1:
-            k = _lval_kmap_pow_zero_to_one.get (exponent.kind, exponent.kind)
-            rv = Lval (k, v**exponent.value)
+            k = _lval_kmap_pow_zero_to_one.get(exponent.kind, exponent.kind)
+            rv = Lval(k, v**exponent.value)
         else:
-            k = _lval_kmap_pow_above_one.get (exponent.kind, exponent.kind)
-            rv = Lval (k, v**exponent.value)
+            k = _lval_kmap_pow_above_one.get(exponent.kind, exponent.kind)
+            rv = Lval(k, v**exponent.value)
 
         if reciprocate:
-            rv = _lval_unary_reciprocal (rv)
+            rv = _lval_unary_reciprocal(rv)
         return rv
 
 
-    def __ipow__ (self, other, modulo=None):
-        tmp = pow (self, other, modulo)
+    def __ipow__(self, other, modulo=None):
+        tmp = pow(self, other, modulo)
         self.kind, self.value = tmp.kind, tmp.value
         return self
 
 
     __hash__ = None
 
 
-def _make_lval_unary_math_nolimits (scalarfunc):
-    def lval_unary_math_nolimits (v):
-        v = Lval.from_other (v)
+def _make_lval_unary_math_nolimits(scalarfunc):
+    def lval_unary_math_nolimits(v):
+        v = Lval.from_other(v)
         if v.kind == 'upper' or v.kind == 'lower':
-            raise LimitError ()
-        return Lval (v.kind, scalarfunc (value))
+            raise LimitError()
+        return Lval(v.kind, scalarfunc(value))
     return lval_unary_math_nolimits
 
 
-def _lval_unary_absolute (v):
-    v = Lval.from_other (v)
+def _lval_unary_absolute(v):
+    v = Lval.from_other(v)
 
     if v.kind == 'pastzero':
-        return Lval ('toinf', 0.) # can't argue with this!
-    return Lval (v.kind, abs (v.value))
+        return Lval('toinf', 0.) # can't argue with this!
+    return Lval(v.kind, abs(v.value))
 
 
-def _lval_unary_exp (v):
-    v = Lval.from_other (v)
+def _lval_unary_exp(v):
+    v = Lval.from_other(v)
 
     reciprocate = (v.value < 0)
     if reciprocate:
         v = -v
 
-    rv = Lval (_lval_kmap_exp.get (v.kind, v.kind), np.exp (v.value))
+    rv = Lval(_lval_kmap_exp.get(v.kind, v.kind), np.exp(v.value))
     if reciprocate:
-        rv = _lval_unary_reciprocal (rv)
+        rv = _lval_unary_reciprocal(rv)
     return rv
 
 
-def _lval_unary_isfinite (v):
-    v = Lval.from_other (v)
+def _lval_unary_isfinite(v):
+    v = Lval.from_other(v)
 
     if v.kind == 'undef':
         return False
-    return np.isfinite (v.value)
+    return np.isfinite(v.value)
 
 
-def _make_lval_unary_log (scalarfunc):
-    def lval_unary_log (v):
-        v = Lval.from_other (v)
+def _make_lval_unary_log(scalarfunc):
+    def lval_unary_log(v):
+        v = Lval.from_other(v)
         if v.value <= 0 or v.kind in ('undef', 'pastzero'):
-            return Lval ('undef', np.nan)
-        return Lval (_lval_kmap_log.get (v.kind, v.kind),
-                     scalarfunc (v.value))
+            return Lval('undef', np.nan)
+        return Lval(_lval_kmap_log.get(v.kind, v.kind),
+                    scalarfunc(v.value))
     return lval_unary_log
 
 
-def _lval_unary_negative (v):
+def _lval_unary_negative(v):
     # In this convenient case, the `kind` doesn't change.
-    v = Lval.from_other (v)
-    return Lval (v.kind, -v.value)
+    v = Lval.from_other(v)
+    return Lval(v.kind, -v.value)
 
 
-def _lval_unary_reciprocal (v):
-    v = Lval.from_other (v)
+def _lval_unary_reciprocal(v):
+    v = Lval.from_other(v)
     if v.value == 0:
-        return Lval ('undef', np.nan)
-    return Lval (_lval_kmap_reciprocal.get (v.kind, v.kind), 1. / v.value)
+        return Lval('undef', np.nan)
+    return Lval(_lval_kmap_reciprocal.get(v.kind, v.kind), 1. / v.value)
 
 
-def _lval_unary_sqrt (v):
-    v = Lval.from_other (v)
+def _lval_unary_sqrt(v):
+    v = Lval.from_other(v)
     return v ** 0.5
 
 
-def _lval_unary_square (v):
-    v = Lval.from_other (v)
+def _lval_unary_square(v):
+    v = Lval.from_other(v)
     return v * v
 
 
 lval_unary_math = {
     # The 'nolimits' entries could be improved with special-cased
     # implementations, but I'm not going to write them until the need arises.
     'absolute': _lval_unary_absolute,
-    'arccos': _make_lval_unary_math_nolimits (np.arccos),
-    'arcsin': _make_lval_unary_math_nolimits (np.arcsin),
-    'arctan': _make_lval_unary_math_nolimits (np.arctan),
-    'cos': _make_lval_unary_math_nolimits (np.cos),
-    'expm1': _make_lval_unary_math_nolimits (np.expm1),
+    'arccos': _make_lval_unary_math_nolimits(np.arccos),
+    'arcsin': _make_lval_unary_math_nolimits(np.arcsin),
+    'arctan': _make_lval_unary_math_nolimits(np.arctan),
+    'cos': _make_lval_unary_math_nolimits(np.cos),
+    'expm1': _make_lval_unary_math_nolimits(np.expm1),
     'exp': _lval_unary_exp,
     'isfinite': _lval_unary_isfinite,
-    'log10': _make_lval_unary_log (np.log10),
-    'log1p': _make_lval_unary_math_nolimits (np.log1p),
-    'log2': _make_lval_unary_log (np.log2),
-    'log': _make_lval_unary_log (np.log),
+    'log10': _make_lval_unary_log(np.log10),
+    'log1p': _make_lval_unary_math_nolimits(np.log1p),
+    'log2': _make_lval_unary_log(np.log2),
+    'log': _make_lval_unary_log(np.log),
     'negative': _lval_unary_negative,
     'reciprocal': _lval_unary_reciprocal,
-    'sin': _make_lval_unary_math_nolimits (np.sin),
+    'sin': _make_lval_unary_math_nolimits(np.sin),
     'sqrt': _lval_unary_sqrt,
     'square': _lval_unary_square,
-    'tan': _make_lval_unary_math_nolimits (np.tan),
+    'tan': _make_lval_unary_math_nolimits(np.tan),
 }
 
 
 # Finally, measurements represented in textual form. Textual forms can
 # represent exact values, Uvals, or Lvals.
 
 UQUANT_UNCERT = 0.2
@@ -1329,31 +1333,31 @@
 are 20% uncertain and give them to multiple decimal places. I'd rather be
 conservative with these values than overly optimistic.
 
 Code to do the appropriate parsing is in the Python uncertainties package, in
 its __init__.py:parse_error_in_parentheses().
 
 """
-_tkinds = frozenset (('none', 'log10', 'positive'))
-_dkinds = frozenset (('exact', 'symm', 'asymm', 'uncertain', 'upper', 'lower', 'unif'))
-_noextra_dkinds = frozenset (('exact', 'uncertain', 'upper', 'lower'))
-_yesextra_dkinds = frozenset (('symm', 'asymm'))
+_tkinds = frozenset(('none', 'log10', 'positive'))
+_dkinds = frozenset(('exact', 'symm', 'asymm', 'uncertain', 'upper', 'lower', 'unif'))
+_noextra_dkinds = frozenset(('exact', 'uncertain', 'upper', 'lower'))
+_yesextra_dkinds = frozenset(('symm', 'asymm'))
 
 
-def _split_decimal_col (floattext):
+def _split_decimal_col(floattext):
     if '.' not in floattext:
         return '$%s$ & ' % floattext
-    return '$%s$ & $.%s$ ' % tuple (floattext.split ('.'))
+    return '$%s$ & $.%s$ ' % tuple(floattext.split('.'))
 
 
-class Textual (object):
+class Textual(object):
     """A measurement recorded in textual form.
 
-    Textual.from_exact (text, tkind='none') - `text` is passed to float()
-    Textual.parse (text, tkind='none')      - `text` as described below.
+    Textual.from_exact(text, tkind='none') - `text` is passed to float()
+    Textual.parse(text, tkind='none')      - `text` as described below.
 
     Transformation kinds are 'none', 'log10', or 'positive'. Expressions for
     values take the form '1.234', '<2', '>3', '~7', '6to8', '7pm0.1', or
     '12p1m0.3'.
 
     Methods:
 
@@ -1364,103 +1368,103 @@
 
     Supported operations: unicode() str() repr() [latexification] -(neg) abs()
     + - * / **
 
     """
     __slots__ = ('tkind', 'dkind', 'data')
 
-    def __init__ (self, tkind, dkind, data):
+    def __init__(self, tkind, dkind, data):
         if tkind not in _tkinds:
-            raise ValueError ('unrecognized transformation kind "%s"' % tkind)
+            raise ValueError('unrecognized transformation kind "%s"' % tkind)
         if dkind not in _dkinds:
-            raise ValueError ('unrecognized distribution kind "%s"' % dkind)
+            raise ValueError('unrecognized distribution kind "%s"' % dkind)
         # FIXME: could/should check `data`.
 
         self.tkind = tkind
         self.dkind = dkind
         self.data = data
 
 
     @staticmethod
-    def from_exact (text, tkind='none'):
-        float (text) # check float-parseability.
-        return Textual (tkind, 'exact', text)
+    def from_exact(text, tkind='none'):
+        float(text) # check float-parseability.
+        return Textual(tkind, 'exact', text)
 
 
     @staticmethod
-    def parse (text, tkind='none'):
+    def parse(text, tkind='none'):
         # freestanding float() calls below are used to check
         # float-parseability of strings.
         # XXX: we do not check sanity when tkind is 'positive'!
 
         if text[0] == '~':
             dkind = 'uncertain'
             data = text[1:]
-            float (data)
+            float(data)
         elif text[0] == '<':
             dkind = 'upper'
             data = text[1:]
-            float (data)
+            float(data)
         elif text[0] == '>':
             dkind = 'lower'
             data = text[1:]
-            float (data)
+            float(data)
         elif 'to' in text:
-            lower, upper = text.split ('to')
-            f_lower = float (lower)
-            f_upper = float (upper)
+            lower, upper = text.split('to')
+            f_lower = float(lower)
+            f_upper = float(upper)
 
             if f_lower > f_upper:
                 upper, lower = lower, upper
                 f_upper, f_lower = f_lower, f_upper
 
             if f_lower < 0 and tkind == 'positive':
-                raise ValueError ('uniform interval is forced positive, but '
-                                  'got "%s"' % text)
+                raise ValueError('uniform interval is forced positive, but '
+                                 'got "%s"' % text)
 
             dkind = 'unif'
             data = (lower, upper)
         elif 'pm' in text:
-            val, uncert = text.split ('pm')
-            float (val)
-            f_uncert = float (uncert)
+            val, uncert = text.split('pm')
+            float(val)
+            f_uncert = float(uncert)
             if f_uncert <= 0.:
-                raise ValueError ('uncertainty values must be positive; got "%s"' % text)
+                raise ValueError('uncertainty values must be positive; got "%s"' % text)
 
             dkind = 'symm'
             data = (val, uncert)
         elif 'p' in text:
-            val, rhs = text.split ('p', 1)
-            high, low = rhs.split ('m', 1)
-            float (val) # checks parseability
-            f_high = float (high)
-            f_low = float (low)
+            val, rhs = text.split('p', 1)
+            high, low = rhs.split('m', 1)
+            float(val) # checks parseability
+            f_high = float(high)
+            f_low = float(low)
 
             if f_high <= 0:
-                raise ValueError ('asymmetrical upper uncertainty must be positive')
+                raise ValueError('asymmetrical upper uncertainty must be positive')
             if f_low <= 0:
-                raise ValueError ('asymmetrical lower uncertainty must be positive')
+                raise ValueError('asymmetrical lower uncertainty must be positive')
 
             dkind = 'asymm'
             data = (val, high, low)
         else:
             try: # plain float treated as unquantified
                 dkind = 'uncertain'
                 data = text
-                float (data)
+                float(data)
             except ValueError:
-                raise ValueError ('don\'t know how to parse measurement text: %s' % text)
+                raise ValueError('don\'t know how to parse measurement text: %s' % text)
 
-        return Textual (tkind, dkind, data)
+        return Textual(tkind, dkind, data)
 
 
     # Textualization -- keep this up here since this is so closely tied to
     # construction via parse(). Note that unparse() loses the `tkind` info.
 
-    def unparse (self):
+    def unparse(self):
         if self.dkind == 'exact':
             return self.data
         elif self.dkind == 'uncertain':
             return '~' + self.data
         elif self.dkind == 'symm':
             return self.data[0] + 'pm' + self.data[1]
         elif self.dkind == 'asymm':
@@ -1469,34 +1473,34 @@
             return '<' + self.data
         elif self.dkind == 'lower':
             return '>' + self.data
         elif self.dkind == 'unif':
             return self.data[0] + 'to' + self.data[1]
 
 
-    def __repr__ (self):
+    def __repr__(self):
         if self.tkind == 'none':
             ttext = ''
         else:
             ttext = ', %r' % (self.tkind, )
 
         if self.dkind == 'exact':
             return 'Textual.from_exact (%r%s)' % (self.data, ttext)
-        return 'Textual.parse(%r%s)' % (self.unparse (), ttext)
+        return 'Textual.parse(%r%s)' % (self.unparse(), ttext)
 
 
-    def __unicode__ (self):
+    def __unicode__(self):
         if self.tkind == 'none':
-            return self.unparse ()
-        return self.unparse () + ':' + self.tkind
+            return self.unparse()
+        return self.unparse() + ':' + self.tkind
 
     __str__ = unicode_to_str
 
-    def __pk_fmtinfo__ (self):
-        t = self.unparse ()
+    def __pk_fmtinfo__(self):
+        t = self.unparse()
 
         if self.tkind == 'log10':
             ttag = 'L'
         elif self.tkind == 'positive':
             ttag = 'P'
         else:
             ttag = ''
@@ -1508,193 +1512,193 @@
 
         return ttag + dtag, t, False
 
 
     # "Unwrapping" -- conversion into either a scalar, Uval, or Lval. The
     # ability to apply various data transforms complicates this process.
 
-    def _unwrap_pos (self):
+    def _unwrap_pos(self):
         dkind = self.dkind
 
         # Deal with the easy cases ...
 
         if dkind == 'exact':
-            return float (self.data)
+            return float(self.data)
 
         if dkind == 'upper':
             # Important case here: since we're positivized, the appropriate
             # Lval kind is 'tozero' rather than 'pastzero'. This allows
             # the caller to safely take the log or the reciprocal.
-            return Lval ('tozero', float (self.data))
+            return Lval('tozero', float(self.data))
 
         if dkind == 'lower':
-            return Lval ('toinf', float (self.data))
+            return Lval('toinf', float(self.data))
 
         if dkind == 'unif':
             # Limits should have been checked upon construction.
-            lower, upper = map (float, self.data)
-            return Uval.from_unif (lower, upper)
+            lower, upper = map(float, self.data)
+            return Uval.from_unif(lower, upper)
 
         # We have to get careful with the Uvals.
 
         if dkind == 'symm':
-            val = float (self.data[0])
-            uncert = float (self.data[1])
-            v = Uval.from_norm (val, uncert)
+            val = float(self.data[0])
+            uncert = float(self.data[1])
+            v = Uval.from_norm(val, uncert)
         elif dkind == 'uncertain':
-            val = float (self.data)
-            uncert = UQUANT_UNCERT * abs (val)
-            v = Uval.from_norm (val, uncert)
+            val = float(self.data)
+            uncert = UQUANT_UNCERT * abs(val)
+            v = Uval.from_norm(val, uncert)
         elif dkind == 'asymm':
-            val, dhigh, dlow = map (float, self.data)
-            v = Uval.from_double_norm (val, dhigh, dlow)
+            val, dhigh, dlow = map(float, self.data)
+            v = Uval.from_double_norm(val, dhigh, dlow)
 
-        nnonpos = np.where (v.d <= 0)[0].size
+        nnonpos = np.where(v.d <= 0)[0].size
 
         if nnonpos == 0:
             return v
 
         if nnonpos < 3:
             # Yay arbitrary cutoff. This is close enough to
             # positive that we just force things.
-            v.d = np.abs (v.d)
+            v.d = np.abs(v.d)
             return v
 
         # There are enough negative values that we're not comfortable with
         # drawing from a (double) normal distribution. Draw from a gamma
         # distribution instead.
 
         if dkind == 'asymm':
             # The gamma distribution only has two parameters, so what else can
             # we do?
             uncert = 0.5 * (dhigh + dlow)
 
-        alpha, beta = find_gamma_params (val, uncert)
-        return Uval.from_gamma (alpha, beta)
+        alpha, beta = find_gamma_params(val, uncert)
+        return Uval.from_gamma(alpha, beta)
 
 
-    def _unwrap_log (self):
+    def _unwrap_log(self):
         dkind = self.dkind
 
         if dkind == 'exact':
-            return 10**float (self.data)
+            return 10**float(self.data)
 
         if dkind == 'upper':
             # As with positive Textuals, it's important that we can return
             # a tozero limit here.
-            return Lval ('tozero', 10 ** float (self.data))
+            return Lval('tozero', 10 ** float(self.data))
 
         if dkind == 'lower':
-            return Lval ('toinf', 10 ** float (self.data))
+            return Lval('toinf', 10 ** float(self.data))
 
         if dkind == 'uncertain':
             # Assume UQUANT_UNCERT in (10**x), not in x itself
-            val = 10**float (self.data)
-            return Uval.from_norm (val, UQUANT_UNCERT * abs (val))
+            val = 10**float(self.data)
+            return Uval.from_norm(val, UQUANT_UNCERT * abs(val))
 
         if dkind == 'unif':
             # We'll yield a uniform distribution in log10(x), not x. I think
             # this is more desirable if someone writes "foo:Lu = 3.5to4.5".
-            lower, upper = map (float, self.data)
-            return 10**Uval.from_unif (lower, upper)
+            lower, upper = map(float, self.data)
+            return 10**Uval.from_unif(lower, upper)
 
         if dkind == 'symm':
-            val = float (self.data[0])
-            uncert = float (self.data[1])
-            return 10**Uval.from_norm (val, uncert)
+            val = float(self.data[0])
+            uncert = float(self.data[1])
+            return 10**Uval.from_norm(val, uncert)
 
         assert dkind == 'asymm'
-        val, dhigh, dlow = map (float, self.data)
-        return 10**Uval.from_double_norm (val, dhigh, dlow)
+        val, dhigh, dlow = map(float, self.data)
+        return 10**Uval.from_double_norm(val, dhigh, dlow)
 
 
-    def unwrap (self):
+    def unwrap(self):
         if self.tkind == 'log10':
-            return self._unwrap_log ()
+            return self._unwrap_log()
         if self.tkind == 'positive':
-            return self._unwrap_pos ()
+            return self._unwrap_pos()
 
         # No transformations applied:
         dkind = self.dkind
 
         if dkind == 'exact':
-            return float (self.data)
+            return float(self.data)
 
         if dkind == 'upper':
             # Limits of magnitude-type quantities should always be of tkind
             # 'log10' or 'positive', so that we can return a 'tozero' Lval
             # rather than 'pastzero'. This is important for taking reciprocals
             # and/or logarithms.
-            v = float (self.data)
+            v = float(self.data)
             if v < 0:
-                return Lval ('toinf', v)
-            return Lval ('pastzero', v)
+                return Lval('toinf', v)
+            return Lval('pastzero', v)
 
         if dkind == 'lower':
-            v = float (self.data)
+            v = float(self.data)
             if v < 0:
-                return Lval ('pastzero', v)
-            return Lval ('toinf', v)
+                return Lval('pastzero', v)
+            return Lval('toinf', v)
 
         if dkind == 'unif':
-            lower, upper = map (float, self.data)
-            return Uval.from_unif (lower, upper)
+            lower, upper = map(float, self.data)
+            return Uval.from_unif(lower, upper)
 
         if dkind == 'uncertain':
-            val = float (self.data)
-            return Uval.from_norm (val, UQUANT_UNCERT * abs (val))
+            val = float(self.data)
+            return Uval.from_norm(val, UQUANT_UNCERT * abs(val))
 
         if dkind == 'symm':
-            val = float (self.data[0])
-            uncert = float (self.data[1])
-            return Uval.from_norm (val, uncert)
+            val = float(self.data[0])
+            uncert = float(self.data[1])
+            return Uval.from_norm(val, uncert)
 
         assert dkind == 'asymm'
-        val, dhigh, dlow = map (float, self.data)
-        return Uval.from_double_norm (val, dhigh, dlow)
+        val, dhigh, dlow = map(float, self.data)
+        return Uval.from_double_norm(val, dhigh, dlow)
 
 
     # Other numerical helpers.
 
-    def repval (self, limitsok=False):
+    def repval(self, limitsok=False):
         """Get a best-effort representative value as a float. This can be
         DANGEROUS because it discards limit information, which is rarely wise."""
 
         if not limitsok and self.dkind in ('lower', 'upper'):
-            raise LimitError ()
+            raise LimitError()
 
         if self.dkind == 'unif':
-            lower, upper = map (float, self.data)
+            lower, upper = map(float, self.data)
             v = 0.5 * (lower + upper)
         elif self.dkind in _noextra_dkinds:
-            v = float (self.data)
+            v = float(self.data)
         elif self.dkind in _yesextra_dkinds:
-            v = float (self.data[0])
+            v = float(self.data[0])
         else:
-            raise RuntimeError ('can\'t happen')
+            raise RuntimeError('can\'t happen')
 
         if self.tkind == 'log10':
             return 10**v
         return v
 
 
-    def limtype (self):
+    def limtype(self):
         """Return -1 if this value is an upper limit, 1 if it is a lower
         limit, 0 otherwise."""
 
         if self.dkind == 'upper':
             return -1
         if self.dkind == 'lower':
             return 1
         return 0
 
 
     # Latexification.
 
-    def __pk_latex__ (self):
+    def __pk_latex__(self):
         if self.dkind == 'exact':
             return r'$%s$' % self.data
         if self.dkind == 'uncertain':
             return r'$\sim$$%s$' % self.data
         if self.dkind == 'symm':
             return r'$%s \pm %s$' % self.data
         if self.dkind == 'asymm':
@@ -1703,256 +1707,256 @@
             return r'$<$$%s$' % self.data
         if self.dkind == 'lower':
             return r'$>$$%s$' % self.data
         if self.dkind == 'unif':
             return r'$%s$--$%s$' % self.data
 
 
-    def __pk_latex_u3col__ (self):
+    def __pk_latex_u3col__(self):
         if self.dkind == 'exact':
             return r'\multicolumn{3}{c}{$%s$}' % self.data
         if self.dkind == 'uncertain':
             return r'\multicolumn{3}{c}{$\sim$$%s$}' % self.data
         if self.dkind == 'symm':
             return r'%s & $\pm\,%s$' % \
-                (_split_decimal_col (self.data[0]), self.data[1])
+                (_split_decimal_col(self.data[0]), self.data[1])
         if self.dkind == 'asymm':
             return r'%s & $\pm\,^{%s}_{%s}$' % \
-                (_split_decimal_col (self.data[0]), self.data[1], self.data[2])
+                (_split_decimal_col(self.data[0]), self.data[1], self.data[2])
         if self.dkind == 'upper':
             return r'\multicolumn{3}{c}{$<$$%s$}' % self.data
         if self.dkind == 'lower':
             return r'\multicolumn{3}{c}{$>$$%s$}' % self.data
         if self.dkind == 'unif':
             return r'\multicolumn{3}{c}{$%s$--$%s$}' % self.data
 
 
     # Unary math -- we do the same thing as _make_textual_unary_math_generic()
     # below. Unlike Uval and Lval, algebra on Textuals is emphatically not
     # closed -- the result is always a non-Textual.
 
-    def __neg__ (self):
-        return _dispatch_unary_math ('negative', False, self.unwrap ())
+    def __neg__(self):
+        return _dispatch_unary_math('negative', False, self.unwrap())
 
-    def __abs__ (self):
-        return _dispatch_unary_math ('absolute', False, self.unwrap ())
+    def __abs__(self):
+        return _dispatch_unary_math('absolute', False, self.unwrap())
 
     # Binary math -- we delegate to the functions that are defined below.
 
-    def __add__ (self, other):
-        return add (self, other)
+    def __add__(self, other):
+        return add(self, other)
 
-    def __sub__ (self, other):
-        return subtract (self, other)
+    def __sub__(self, other):
+        return subtract(self, other)
 
-    def __mul__ (self, other):
-        return multiply (self, other)
+    def __mul__(self, other):
+        return multiply(self, other)
 
-    def __div__ (self, other):
-        return divide (self, other)
+    def __div__(self, other):
+        return divide(self, other)
 
-    def __truediv__ (self, other):
-        return true_divide (self, other)
+    def __truediv__(self, other):
+        return true_divide(self, other)
 
-    def __pow__ (self, other, module=None):
+    def __pow__(self, other, module=None):
         if modulo is not None:
-            raise ValueError ('powmod behavior forbidden with Textuals')
-        return power (self, other)
+            raise ValueError('powmod behavior forbidden with Textuals')
+        return power(self, other)
 
-    def __radd__ (self, other):
-        return add (other, self)
+    def __radd__(self, other):
+        return add(other, self)
 
-    def __rsub__ (self, other):
-        return subtract (other, self)
+    def __rsub__(self, other):
+        return subtract(other, self)
 
-    def __rmul__ (self, other):
-        return multiply (other, self)
+    def __rmul__(self, other):
+        return multiply(other, self)
 
-    def __rdiv__ (self, other):
-        return divide (other, self)
+    def __rdiv__(self, other):
+        return divide(other, self)
 
-    def __rtruediv__ (self, other):
-        return true_divide (other, self)
+    def __rtruediv__(self, other):
+        return true_divide(other, self)
 
-    def __rpow__ (self, other, module=None):
+    def __rpow__(self, other, module=None):
         if modulo is not None:
-            raise ValueError ('powmod behavior forbidden with Textuals')
-        return power (other, self)
+            raise ValueError('powmod behavior forbidden with Textuals')
+        return power(other, self)
 
 
-def _dispatch_unary_math (name, check_textual, value):
-    if np.isscalar (value):
+def _dispatch_unary_math(name, check_textual, value):
+    if np.isscalar(value):
         table = scalar_unary_math
-    elif isinstance (value, Uval):
+    elif isinstance(value, Uval):
         table = uval_unary_math
-    elif isinstance (value, Lval):
+    elif isinstance(value, Lval):
         table = lval_unary_math
-    elif check_textual and isinstance (value, Textual):
+    elif check_textual and isinstance(value, Textual):
         table = textual_unary_math
     else:
-        raise ValueError ('cannot treat %r as a scalar for %s' % (value, name))
+        raise ValueError('cannot treat %r as a scalar for %s' % (value, name))
 
-    func = table.get (name)
+    func = table.get(name)
     if func is None:
-        raise ValueError ('no implementation of %s for %r' % (name, value))
-    return func (value)
+        raise ValueError('no implementation of %s for %r' % (name, value))
+    return func(value)
 
 
-def _make_textual_unary_math_generic (name):
+def _make_textual_unary_math_generic(name):
     # N.B.: unlike Uval and Lval functions, this assumes that `v` is in fact a
     # Textual.
-    def textual_unary_math_generic (val):
-        return _dispatch_unary_math (name, False, val.unwrap ())
+    def textual_unary_math_generic(val):
+        return _dispatch_unary_math(name, False, val.unwrap())
     return textual_unary_math_generic
 
 
-def _textual_unary_log10 (val):
+def _textual_unary_log10(val):
     if val.tkind == 'log10':
-        return Textual ('none', val.dkind, val.data)
-    return _dispatch_unary_math ('log10', False, val.unwrap ())
+        return Textual('none', val.dkind, val.data)
+    return _dispatch_unary_math('log10', False, val.unwrap())
 
 
 textual_unary_math = {
-    'absolute': _make_textual_unary_math_generic ('absolute'),
-    'arccos': _make_textual_unary_math_generic ('arccos'),
-    'arcsin': _make_textual_unary_math_generic ('arcsin'),
-    'arctan': _make_textual_unary_math_generic ('arctan'),
-    'cos': _make_textual_unary_math_generic ('cos'),
-    'expm1': _make_textual_unary_math_generic ('expm1'),
-    'exp': _make_textual_unary_math_generic ('exp'),
+    'absolute': _make_textual_unary_math_generic('absolute'),
+    'arccos': _make_textual_unary_math_generic('arccos'),
+    'arcsin': _make_textual_unary_math_generic('arcsin'),
+    'arctan': _make_textual_unary_math_generic('arctan'),
+    'cos': _make_textual_unary_math_generic('cos'),
+    'expm1': _make_textual_unary_math_generic('expm1'),
+    'exp': _make_textual_unary_math_generic('exp'),
     'isfinite': lambda v: True, # legal Textuals can never yield inf or nan
     'log10': _textual_unary_log10,
-    'log1p': _make_textual_unary_math_generic ('log1p'),
-    'log2': _make_textual_unary_math_generic ('log2'),
-    'log': _make_textual_unary_math_generic ('log'),
-    'negative': _make_textual_unary_math_generic ('negative'),
-    'reciprocal': _make_textual_unary_math_generic ('reciprocal'),
-    'sin': _make_textual_unary_math_generic ('sin'),
-    'sqrt': _make_textual_unary_math_generic ('sqrt'),
-    'square':  _make_textual_unary_math_generic ('square'),
-    'tan': _make_textual_unary_math_generic ('tan'),
+    'log1p': _make_textual_unary_math_generic('log1p'),
+    'log2': _make_textual_unary_math_generic('log2'),
+    'log': _make_textual_unary_math_generic('log'),
+    'negative': _make_textual_unary_math_generic('negative'),
+    'reciprocal': _make_textual_unary_math_generic('reciprocal'),
+    'sin': _make_textual_unary_math_generic('sin'),
+    'sqrt': _make_textual_unary_math_generic('sqrt'),
+    'square':  _make_textual_unary_math_generic('square'),
+    'tan': _make_textual_unary_math_generic('tan'),
 }
 
 
 # Now, a library of metadata-esque functions that will handle anything you
 # throw at them: scalars, Uvals, Lvals, and Textuals.
 
-def is_measurement (obj):
-    return np.isscalar (obj) or isinstance (obj, (Uval, Lval, Textual))
+def is_measurement(obj):
+    return np.isscalar(obj) or isinstance(obj, (Uval, Lval, Textual))
 
 
-def unwrap (msmt):
+def unwrap(msmt):
     """Convert the value into the most basic representation that we can do
     math on: float if possible, then Uval, then Lval."""
 
-    if np.isscalar (msmt):
-        return float (msmt)
-    if isinstance (msmt, (Uval, Lval)):
+    if np.isscalar(msmt):
+        return float(msmt)
+    if isinstance(msmt, (Uval, Lval)):
         return msmt
-    if isinstance (msmt, Textual):
-        return msmt.unwrap ()
-    raise ValueError ('don\'t know how to treat %r as a measurement' % msmt)
+    if isinstance(msmt, Textual):
+        return msmt.unwrap()
+    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
 
 
-def typealign (origmsmt1, origmsmt2):
+def typealign(origmsmt1, origmsmt2):
     msmt1 = origmsmt1
-    if isinstance (msmt1, Textual):
-        msmt1 = msmt1.unwrap ()
+    if isinstance(msmt1, Textual):
+        msmt1 = msmt1.unwrap()
     msmt2 = origmsmt2
-    if isinstance (msmt2, Textual):
-        msmt2 = msmt2.unwrap ()
+    if isinstance(msmt2, Textual):
+        msmt2 = msmt2.unwrap()
 
-    if isinstance (msmt1, Lval):
-        return msmt1, Lval.from_other (msmt2)
-    if isinstance (msmt2, Lval):
-        return Lval.from_other (msmt1), msmt2
-    if isinstance (msmt1, Uval):
-        return msmt1, Uval.from_other (msmt2)
-    if isinstance (msmt2, Uval):
-        return Uval.from_other (msmt1), msmt2
+    if isinstance(msmt1, Lval):
+        return msmt1, Lval.from_other(msmt2)
+    if isinstance(msmt2, Lval):
+        return Lval.from_other(msmt1), msmt2
+    if isinstance(msmt1, Uval):
+        return msmt1, Uval.from_other(msmt2)
+    if isinstance(msmt2, Uval):
+        return Uval.from_other(msmt1), msmt2
 
     try:
-        return float (msmt1), float (msmt2)
+        return float(msmt1), float(msmt2)
     except Exception:
-        raise ValueError ('cannot treat %r and %r as numeric types'
-                          % (origmsmt1, origmsmt2))
+        raise ValueError('cannot treat %r and %r as numeric types'
+                         % (origmsmt1, origmsmt2))
 
 
-def repval (msmt, limitsok=False):
+def repval(msmt, limitsok=False):
     """Get a best-effort representative value as a float. This is DANGEROUS
     because it discards limit information, which is rarely wise. m_liminfo()
     or m_unwrap() are recommended instead."""
 
-    if np.isscalar (msmt):
-        return float (msmt)
-    if isinstance (msmt, Uval):
-        return msmt.repvals (uval_default_repval_method)[0]
-    if isinstance (msmt, Lval):
-        if not limitsok and msmt.kind in ('tozero', 'toinf', 'pastzero'):
-            raise LimitError ()
+    if np.isscalar(msmt):
+        return float(msmt)
+    if isinstance(msmt, Uval):
+        return msmt.repvals(uval_default_repval_method)[0]
+    if isinstance(msmt, Lval):
+        if not limitsok and msmt.kind in('tozero', 'toinf', 'pastzero'):
+            raise LimitError()
         return msmt.value
-    if isinstance (msmt, Textual):
-        return msmt.repval (limitsok=limitsok)
+    if isinstance(msmt, Textual):
+        return msmt.repval(limitsok=limitsok)
 
-    raise ValueError ('don\'t know how to treat %r as a measurement' % msmt)
+    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
 
 
-def limtype (msmt):
+def limtype(msmt):
     """Return -1 if this value is some kind of upper limit, 1 if this value
     is some kind of lower limit, 0 otherwise."""
 
-    if np.isscalar (msmt):
+    if np.isscalar(msmt):
         return 0
-    if isinstance (msmt, Uval):
+    if isinstance(msmt, Uval):
         return 0
-    if isinstance (msmt, Lval):
+    if isinstance(msmt, Lval):
         if msmt.kind == 'undef':
-            raise ValueError ('no simple limit type for Lval %r' % msmt)
+            raise ValueError('no simple limit type for Lval %r' % msmt)
 
         # Quasi-hack here: limits of ('tozero', [positive number]) are
         # reported as upper limits. In a plot full of fluxes this would be
         # what makes sense, but note that this would be misleading if the
         # quantity in question was something that could go negative.
-        p = msmt._polarity ()
+        p = msmt._polarity()
         if p == -2 or p == 1:
             return -1
         if p == 2 or p == -1:
             return 1
         return 0
-    if isinstance (msmt, Textual):
-        return msmt.limtype ()
-    raise ValueError ('don\'t know how to treat %r as a measurement' % msmt)
+    if isinstance(msmt, Textual):
+        return msmt.limtype()
+    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
 
 
-def liminfo (msmt):
+def liminfo(msmt):
     """Return (limtype, repval). `limtype` is -1 for upper limits, 1 for lower
     limits, and 0 otherwise; repval is a best-effort representative scalar value
     for this measurement."""
 
-    return limtype (msmt), repval (msmt, limitsok=True)
+    return limtype(msmt), repval(msmt, limitsok=True)
 
 
-def errinfo (msmt):
+def errinfo(msmt):
     """Return (limtype, repval, errval1, errval2). Like m_liminfo, but also
     provides error bar information for values that have it."""
 
-    if isinstance (msmt, Textual):
-        msmt = msmt.unwrap ()
+    if isinstance(msmt, Textual):
+        msmt = msmt.unwrap()
 
-    if np.isscalar (msmt):
+    if np.isscalar(msmt):
         return 0, msmt, msmt, msmt
 
-    if isinstance (msmt, Uval):
-        rep, plus1, minus1 = msmt.repvals (uval_default_repval_method)
+    if isinstance(msmt, Uval):
+        rep, plus1, minus1 = msmt.repvals(uval_default_repval_method)
         return 0, rep, plus1, minus1
 
-    if isinstance (msmt, Lval):
-        return limtype (msmt), msmt.value, msmt.value, msmt.value
+    if isinstance(msmt, Lval):
+        return limtype(msmt), msmt.value, msmt.value, msmt.value
 
-    raise ValueError ('don\'t know how to treat %r as a measurement' % msmt)
+    raise ValueError('don\'t know how to treat %r as a measurement' % msmt)
 
 
 # Unary numerical functions.
 #
 # Here we just have to look up the appropriate table of unary math operations
 # and delegate. The implemented functions are those in the scalar_unary_math
 # dict.
@@ -1963,33 +1967,33 @@
 # deg2rad degrees fabs fix floor frexp hypot i0 imag ldexp modf rad2deg
 # radians real rint round_ sign signbit sinc sinh tanh trunc unwrap
 #
 # Skipped core Python unary operators:
 #
 # abs coerce complex hex index int invert float long neg nonzero oct pos
 
-def _make_wrapped_unary_math (name):
-    def unary_mathfunc (val):
-        rv = _dispatch_unary_math (name, True, val)
-        if not _dispatch_unary_math ('isfinite', True, rv):
-            raise ValueError ('out-of-bounds input %r to %s' % (val, name))
+def _make_wrapped_unary_math(name):
+    def unary_mathfunc(val):
+        rv = _dispatch_unary_math(name, True, val)
+        if not _dispatch_unary_math('isfinite', True, rv):
+            raise ValueError('out-of-bounds input %r to %s' % (val, name))
         return rv
     return unary_mathfunc
 
 
-def _init_unary_math ():
-    g = globals ()
+def _init_unary_math():
+    g = globals()
 
-    for name in six.iterkeys (scalar_unary_math):
+    for name in six.iterkeys(scalar_unary_math):
         if name == 'isfinite':
-            g[name] = lambda v: _dispatch_unary_math (name, True, v)
+            g[name] = lambda v: _dispatch_unary_math('isfinite', True, v)
         else:
-            g[name] = _make_wrapped_unary_math (name)
+            g[name] = _make_wrapped_unary_math(name)
 
-_init_unary_math ()
+_init_unary_math()
 
 
 # Binary numerical functions.
 #
 # Here we have to coerce the arguments to the ~"highest-level" type that's
 # relevant. Then we can delegate to the class's __op__ functions. Note that
 # there's no reasonable binary operator that can take two Textuals to another
@@ -2000,97 +2004,97 @@
 #
 # fmod maximum minimum mod=remainder logaddexp2 logaddexp
 #
 # Skipped core Python binary operators:
 #
 # and cmp eq ge gt le lshift lt ne or rshift xor
 
-def _make_wrapped_binary_math (opfunc):
-    def binary_mathfunc (val1, val2):
-        a1, a2 = typealign (val1, val2)
-        return opfunc (a1, a2)
+def _make_wrapped_binary_math(opfunc):
+    def binary_mathfunc(val1, val2):
+        a1, a2 = typealign(val1, val2)
+        return opfunc(a1, a2)
     return binary_mathfunc
 
 
-add = _make_wrapped_binary_math (operator.add)
-floor_divide = _make_wrapped_binary_math (operator.floordiv)
-multiply = _make_wrapped_binary_math (operator.mul)
-power = _make_wrapped_binary_math (operator.pow)
-subtract = _make_wrapped_binary_math (operator.sub)
-true_divide = _make_wrapped_binary_math (operator.truediv)
+add = _make_wrapped_binary_math(operator.add)
+floor_divide = _make_wrapped_binary_math(operator.floordiv)
+multiply = _make_wrapped_binary_math(operator.mul)
+power = _make_wrapped_binary_math(operator.pow)
+subtract = _make_wrapped_binary_math(operator.sub)
+true_divide = _make_wrapped_binary_math(operator.truediv)
 divide = true_divide # are we supposed to respect Py2 plain-div semantics?
 
 
 # Parsing and formatting of measurements and other quantities.
 
-def _parse_bool (text):
-    if not len (text):
+def _parse_bool(text):
+    if not len(text):
         return False
     if text == 'y':
         return True
-    raise ValueError ('illegal bool textualization: expect empty or "y"; '
-                      'got "%s"' % text)
+    raise ValueError('illegal bool textualization: expect empty or "y"; '
+                     'got "%s"' % text)
 
 
-def _maybe (subparse):
-    def parser (text):
-        if not len (text):
+def _maybe(subparse):
+    def parser(text):
+        if not len(text):
             return None
-        return subparse (text)
+        return subparse(text)
     return parser
 
 
 _ttkinds = {'': 'none', 'L': 'log10', 'P': 'positive'}
 
-def _maybe_parse_exact (text, tkind):
-    if not len (text):
+def _maybe_parse_exact(text, tkind):
+    if not len(text):
         return None
-    return Textual.from_exact (text, _ttkinds[tkind])
+    return Textual.from_exact(text, _ttkinds[tkind])
 
 
-def _maybe_parse_uncert (text, tkind):
-    if not len (text):
+def _maybe_parse_uncert(text, tkind):
+    if not len(text):
         return None
-    return Textual.parse (text, _ttkinds[tkind])
+    return Textual.parse(text, _ttkinds[tkind])
 
 
 parsers = {
     # maps 'type tag string' to 'parsing function'.
     'x': None,
     'b': _parse_bool,
-    'i': _maybe (int),
-    's': _maybe (text_type),
-    'f': lambda t: _maybe_parse_exact (t, ''),
-    'Lf': lambda t: _maybe_parse_exact (t, 'L'),
-    'Pf': lambda t: _maybe_parse_exact (t, 'P'),
-    'u': lambda t: _maybe_parse_uncert (t, ''),
-    'Lu': lambda t: _maybe_parse_uncert (t, 'L'),
-    'Pu': lambda t: _maybe_parse_uncert (t, 'P'),
+    'i': _maybe(int),
+    's': _maybe(text_type),
+    'f': lambda t: _maybe_parse_exact(t, ''),
+    'Lf': lambda t: _maybe_parse_exact(t, 'L'),
+    'Pf': lambda t: _maybe_parse_exact(t, 'P'),
+    'u': lambda t: _maybe_parse_uncert(t, ''),
+    'Lu': lambda t: _maybe_parse_uncert(t, 'L'),
+    'Pu': lambda t: _maybe_parse_uncert(t, 'P'),
 }
 
-def fmtinfo (value):
+def fmtinfo(value):
     """Returns (typetag, text, is_imprecise). Unlike other functions that operate
     on measurements, this also operates on bools, ints, and strings.
 
     """
     if value is None:
-        raise ValueError ('cannot format None!')
+        raise ValueError('cannot format None!')
 
-    if isinstance (value, text_type):
+    if isinstance(value, text_type):
         return '', value, False
 
-    if isinstance (value, bool):
-        # Note: isinstance (True, int) = True, so this must come before the next case.
+    if isinstance(value, bool):
+        # Note: isinstance(True, int) = True, so this must come before the next case.
         if value:
             return 'b', 'y', False
         return 'b', '', False
 
-    if isinstance (value, (int, long)):
-        return 'i', text_type (value), False
+    if isinstance(value, six.integer_types):
+        return 'i', text_type(value), False
 
-    if isinstance (value, float):
-        return 'f', text_type (value), True
+    if isinstance(value, float):
+        return 'f', text_type(value), True
 
-    if hasattr (value, '__pk_fmtinfo__'):
-        return value.__pk_fmtinfo__ ()
+    if hasattr(value, '__pk_fmtinfo__'):
+        return value.__pk_fmtinfo__()
 
-    raise ValueError ('don\'t know how to format %r as a measurement' % value)
+    raise ValueError('don\'t know how to format %r as a measurement' % value)
```

### Comparing `pwkit-0.8.9/pwkit/lsqmdl.py` & `pwkit-1.0.0/pwkit/lsqmdl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,339 +1,404 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2012-2014 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2012-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
-"""pwkit.lsqmdl - model data with least-squares fitting
+"""Model data with least-squares fitting
 
-Classes:
-
-Model                  - Modeling with any function using Levenberg-Marquardt.
-Parameter              - Information about a specific model parameter.
-PolynomialModel        - Modeling with polynomials.
-ScaleModel             - Modeling with a single scale factor.
-ComposedModel          - Modeling with combinations of pluggable components.
-
-ModelComponent         - Base class for ComposedModel components.
-AddConstantComponent   - Adds a single value to all data points.
-AddValuesComponent     - Adds a parameter for every data point.
-AddPolynomialComponent - Adds a polynomial.
-SeriesComponent        - Apply a set of subcomponents in series.
-MatMultComponent       - Combine subcomponents in a matrix multiplication.
-ScaleComponent         - Multiplies the data by a single value.
-
-Usage::
-
-  m = Model (func, data, [invsigma], [args]).solve (guess).print_soln ()
-      # func takes (p1, p2, p3[, *args]) and returns model data
-  m = PolynomialModel (maxexponent, x, data, [invsigma]).solve ().plot ()
-  m = ScaleModel (x, data, [invsigma]).solve ().show_cov ()
-      # data = m*x
-
-The invsigma are *inverse sigmas*, NOT inverse *variances* (the usual
-statistical weights). Since most applications deal in sigmas, take care to
-write::
-
-  m = Model (func, data, 1./uncerts) # right!
-
-not::
-
-  m = Model (func, data, uncerts) # WRONG
-
-If you have zero uncertainty on a measurement, too bad.
+This module provides tools for fitting models to data using least-squares
+optimization.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('Model PolynomialModel ScaleModel').split ()
+__all__ = 'ModelBase Model ComposedModel PolynomialModel ScaleModel'.split()
 
 import numpy as np
 try:
     # numpy 1.7
     import numpy.polynomial.polynomial as npoly
 except ImportError:
     import numpy.polynomial as npoly
 
 from six import get_function_code
 from six.moves import range, reduce
 from . import binary_type, text_type
 
 
-class Parameter (object):
-    """Information about a parameter in a least-squares model. These data may only
-    be obtained after solving least-squares problem.
-
-    These objects reference information from their parent objects, so changing
-    the parent will alter the apparent contents of these objects.
-
-    Properties:
-
-    index  - The parameter's index in the Model's arrays.
-    name   - The parameter's name.
-    value  - The parameter's value.
-    uncert - The uncertainty in value.
-    uval   - Accesses ``value`` and ``uncert`` as a ``pwkit.msmt.Uval``.
+class Parameter(object):
+    """Information about a parameter in a least-squares model.
+
+    These data may only be obtained after solving least-squares problem. These
+    objects reference information from their parent objects, so changing the
+    parent will alter the apparent contents of these objects.
 
     """
-    def __init__ (self, owner, index):
+    def __init__(self, owner, index):
         self._owner = owner
         self._index = index
 
-    def __repr__ (self):
+    def __repr__(self):
         return '<Parameter "%s" (#%d) of %s>' % (self.name, self._index, self._owner)
 
     @property
-    def index (self): # make this read-only
+    def index(self): # make this read-only
+        "The parameter's index in the Model's arrays."
         return self._index
 
     @property
-    def name (self):
+    def name(self):
+        "The parameter's name."
         return self._owner.pnames[self._index]
 
     @property
-    def value (self):
+    def value(self):
+        "The parameter's value."
         return self._owner.params[self._index]
 
     @property
-    def uncert (self):
+    def uncert(self):
+        "The uncertainty in :attr:`value`."
         return self._owner.puncerts[self._index]
 
     @property
-    def uval (self):
+    def uval(self):
+        "Accesses :attr:`value` and :attr:`uncert` as a :class:`pwkit.msmt.Uval`."
         from .msmt import Uval
-        return Uval.from_norm (self.value, self.uncert)
+        return Uval.from_norm(self.value, self.uncert)
 
 
-class _ModelBase (object):
+class ModelBase(object):
+    """An abstract base class holding data and a model for least-squares fitting.
 
-    """Data and a model for least-squares fitting. Attributes:
+    The models implemented in this module all derive from this class and so
+    inherit the attributes and methods described below.
 
-    data     - The data to be modeled.
-    invsigma - Weights: 1/σ for each data point.
-    params   - ndarray of solved model parameters.
-    puncerts - ndarray of 1-sigma uncerts on params.
-    pnames   - list of string names for parameters.
-    covar    - Covariance matrix of parameters.
-    mfunc    - A function f(...) evaluating model fixed at best params.
-    mdata    - The modeled data at the best params.
-    rchisq   - Reduced χ² of the fit.
-    resids   - resids = data - mdata.
+    A :class:`Parameter` data structure may be obtained by indexing this
+    object with either the parameter's numerical index or its name. I.e.::
 
-    Methods:
-
-    plot       - Plot the data and model (requires `omega`; assumes 1D data).
-    print_soln - Print information about the model solution.
-    set_data   - Set the data to be modeled.
-    show_cov   - Show the parameter covariance matrix with `pwkit.ndshow_gtk2`.
-    show_corr  - Show the parameter correlation matrix with `pwkit.ndshow_gtk2`.
-    solve      - Fit the model to the data.
-
-    A ``Parameter`` data structure may be obtained by indexing this object
-    with either the parameter's numerical index or its name. I.e.,
-
-      m = Model (...).solve (...)
+      m = Model(...).solve(...)
       p = m['slope']
-      print (p.name, p.value, p.uncert, p.uval)
+      print(p.name, p.value, p.uncert, p.uval)
 
     """
     data = None
+    "The data to be modeled; an *n*-dimensional Numpy array."
+
     invsigma = None
+    "Data weights: 1/σ for each data point."
+
     params = None
+    "After fitting, a Numpy ndarray of solved model parameters."
+
     puncerts = None
+    "After fitting, a Numpy ndarray of 1σ uncertainties on the model parameters."
+
     pnames = None
+    "A list of textual names for the parameters."
+
     covar = None
+    """After fitting, the variance-covariance matrix representing the parameter
+    uncertainties.
+
+    """
     mfunc = None
+    """After fitting, a callable function evaluating the model fixed at best params.
+
+    The resulting function may or may not take arguments depending on the particular
+    kind of model being evaluated.
+
+    """
     mdata = None
+    "After fitting, the modeled data at the best parameters."
+
+    chisq = None
+    "After fitting, the χ² of the fit."
+
     rchisq = None
+    "After fitting, the reduced χ² of the fit, or None if there are no degrees of freedom."
+
     resids = None
+    "After fitting, the residuals: ``resids = data - mdata``."
 
-    def __init__ (self, data, invsigma=None):
-        self.set_data (data, invsigma)
+    def __init__(self, data, invsigma=None):
+        self.set_data(data, invsigma)
 
 
-    def set_data (self, data, invsigma=None):
-        self.data = np.array (data, dtype=np.float, ndmin=1)
+    def set_data(self, data, invsigma=None):
+        """Set the data to be modeled.
+
+        Returns *self*.
+
+        """
+        self.data = np.array(data, dtype=np.float, ndmin=1)
 
         if invsigma is None:
-            self.invsigma = np.ones (self.data.shape)
+            self.invsigma = np.ones(self.data.shape)
         else:
-            i = np.array (invsigma, dtype=np.float)
-            self.invsigma = np.broadcast_arrays (self.data, i)[1] # allow scalar invsigma
+            i = np.array(invsigma, dtype=np.float)
+            self.invsigma = np.broadcast_arrays(self.data, i)[1] # allow scalar invsigma
 
         if self.invsigma.shape != self.data.shape:
-            raise ValueError ('data values and inverse-sigma values must have same shape')
+            raise ValueError('data values and inverse-sigma values must have same shape')
+
+        return self
 
 
-    def print_soln (self):
-        lmax = reduce (max, (len (x) for x in self.pnames), len ('r chi sq'))
+    def print_soln(self):
+        """Print information about the model solution."""
+        lmax = reduce(max,(len(x) for x in self.pnames), len('r chi sq'))
 
         if self.puncerts is None:
-            for pn, val in zip (self.pnames, self.params):
-                print ('%s: %14g' % (pn.rjust (lmax), val))
+            for pn, val in zip(self.pnames, self.params):
+                print('%s: %14g' % (pn.rjust(lmax), val))
         else:
-            for pn, val, err in zip (self.pnames, self.params, self.puncerts):
-                frac = abs (100. * err / val)
-                print ('%s: %14g +/- %14g (%.2f%%)' % (pn.rjust (lmax), val, err, frac))
-
-        if self.rchisq is None:
-            print ('%s: unknown/undefined' % ('r chi sq'.rjust (lmax)))
+            for pn, val, err in zip(self.pnames, self.params, self.puncerts):
+                frac = abs(100. * err / val)
+                print('%s: %14g +/- %14g (%.2f%%)' % (pn.rjust(lmax), val, err, frac))
+
+        if self.rchisq is not None:
+            print('%s: %14g' % ('r chi sq'.rjust(lmax), self.rchisq))
+        elif self.chisq is not None:
+            print('%s: %14g' % ('chi sq'.rjust(lmax), self.chisq))
         else:
-            print ('%s: %14g' % ('r chi sq'.rjust (lmax), self.rchisq))
+            print('%s: unknown/undefined' % ('r chi sq'.rjust(lmax)))
         return self
 
 
-    def __getitem__ (self, key):
-        if isinstance (key, binary_type):
+    def make_frozen_func(self, params):
+        """Return a data-generating model function frozen at the specified parameters.
+
+        As with the :attr:`mfunc` attribute, the resulting function may or may
+        not take arguments depending on the particular kind of model being
+        evaluated.
+
+        """
+        raise NotImplementedError()
+
+
+    def __getitem__(self, key):
+        if isinstance(key, binary_type):
             # If you're not using the unicode_literals __future__, things get
             # annoying really quickly without this.
-            key = text_type (key)
+            key = text_type(key)
 
-        if isinstance (key, int):
+        if isinstance(key, int):
             idx = key
-            if idx < 0 or idx >= len (self.pnames):
-                raise ValueError ('illegal parameter number %d' % key)
-        elif isinstance (key, text_type):
+            if idx < 0 or idx >= len(self.pnames):
+                raise ValueError('illegal parameter number %d' % key)
+        elif isinstance(key, text_type):
             try:
-                idx = self.pnames.index (key)
+                idx = self.pnames.index(key)
             except ValueError:
-                raise ValueError ('no such parameter named "%s"' % key)
+                raise ValueError('no such parameter named "%s"' % key)
         else:
-            raise ValueError ('illegal parameter key %r' % key)
+            raise ValueError('illegal parameter key %r' % key)
 
-        return Parameter (self, idx)
+        return Parameter(self, idx)
 
 
-    def plot (self, modelx, dlines=False, xmin=None, xmax=None,
-              ymin=None, ymax=None, **kwargs):
-        """This assumes that `data` is 1D and that `mfunc` takes one argument that
-        should be treated as the X variable.
+    def plot(self, modelx, dlines=False, xmin=None, xmax=None,
+             ymin=None, ymax=None, **kwargs):
+        """Plot the data and model (requires `omega`).
+
+        This assumes that `data` is 1D and that `mfunc` takes one argument
+        that should be treated as the X variable.
 
         """
         import omega as om
 
-        modelx = np.asarray (modelx)
+        modelx = np.asarray(modelx)
         if modelx.shape != self.data.shape:
-            raise ValueError ('modelx and data arrays must have same shape')
+            raise ValueError('modelx and data arrays must have same shape')
 
-        modely = self.mfunc (modelx)
+        modely = self.mfunc(modelx)
         sigmas = self.invsigma**-1 # TODO: handle invsigma = 0
 
-        vb = om.layout.VBox (2)
-        vb.pData = om.quickXYErr (modelx, self.data, sigmas,
-                                  'Data', lines=dlines, **kwargs)
+        vb = om.layout.VBox(2)
+        vb.pData = om.quickXYErr(modelx, self.data, sigmas,
+                                 'Data', lines=dlines, **kwargs)
 
         vb[0] = vb.pData
-        vb[0].addXY (modelx, modely, 'Model')
-        vb[0].setYLabel ('Y')
-        vb[0].rebound (False, True)
-        vb[0].setBounds (xmin, xmax, ymin, ymax)
+        vb[0].addXY(modelx, modely, 'Model')
+        vb[0].setYLabel('Y')
+        vb[0].rebound(False, True)
+        vb[0].setBounds(xmin, xmax, ymin, ymax)
 
-        vb[1] = vb.pResid = om.RectPlot ()
+        vb[1] = vb.pResid = om.RectPlot()
         vb[1].defaultField.xaxis = vb[1].defaultField.xaxis
-        vb[1].addXYErr (modelx, self.resids, sigmas, None, lines=False)
-        vb[1].setLabels ('X', 'Residuals')
-        vb[1].rebound (False, True)
+        vb[1].addXYErr(modelx, self.resids, sigmas, None, lines=False)
+        vb[1].setLabels('X', 'Residuals')
+        vb[1].rebound(False, True)
         # ignore Y values since residuals are on different scale:
-        vb[1].setBounds (xmin, xmax)
+        vb[1].setBounds(xmin, xmax)
 
-        vb.setWeight (0, 3)
+        vb.setWeight(0, 3)
         return vb
 
 
-    def show_cov (self):
+    def show_cov(self):
+        "Show the parameter covariance matrix with `pwkit.ndshow_gtk3`."
         # would be nice: labels with parameter names (hard because this is
         # ndshow, not omegaplot)
-        from .ndshow_gtk2 import view
-        view (self.covar, title='Covariance Matrix')
+        from .ndshow_gtk3 import view
+        view(self.covar, title='Covariance Matrix')
 
 
-    def show_corr (self):
-        from .ndshow_gtk2 import view
-        d = np.diag (self.covar) ** -0.5
+    def show_corr(self):
+        "Show the parameter correlation matrix with `pwkit.ndshow_gtk3`."
+        from .ndshow_gtk3 import view
+        d = np.diag(self.covar) ** -0.5
         corr = self.covar * d[np.newaxis,:] * d[:,np.newaxis]
-        view (corr, title='Correlation Matrix')
+        view(corr, title='Correlation Matrix')
+
+
+class Model(ModelBase):
+    """Models data with a generic nonlinear optimizer
+
+    Basic usage is::
+
+      def func(p1, p2, x):
+          simulated_data = p1 * x + p2
+          return simulated_data
+
+      x = [1, 2, 3]
+      data = [10, 14, 15.8]
+      mdl = Model(func, data, args=(x,)).solve(guess).print_soln()
+
+    The :class:`Model` constructor can take an optional argument ``invsigma``
+    after ``data``; it specifies *inverse sigmas*, **not** inverse *variances*
+    (the usual statistical weights), for the data points. Since most
+    applications deal in sigmas, take care to write::
+
+      m = Model(func, data, 1. / uncerts) # right!
+
+    not::
+
+      m = Model(func, data, uncerts) # WRONG
 
+    If you have zero uncertainty on a measurement, you must wind a way to
+    express that constraint without including that measurement as part of the
+    ``data`` vector.
 
-class Model (_ModelBase):
-    def __init__ (self, simple_func, data, invsigma=None, args=()):
+    """
+    lm_prob = None
+    """A :class:`pwkit.lmmin.Problem` instance describing the problem to be solved.
+
+    After setting up the data-generating function, you can access this item to
+    tune the solver.
+
+    """
+    def __init__(self, simple_func, data, invsigma=None, args=()):
         if simple_func is not None:
-            self.set_simple_func (simple_func, args)
+            self.set_simple_func(simple_func, args)
         if data is not None:
-            self.set_data (data, invsigma)
+            self.set_data(data, invsigma)
+
 
+    def set_func(self, func, pnames, args=()):
+        """Set the model function to use an efficient but tedious calling convention.
 
-    def set_func (self, func, pnames, args=()):
-        """This function creates the `lmmin.Problem` so that the caller can futz with
-        it before calling solve(), if so desired.
+        The function should obey the following convention::
+
+            def func(param_vec, *args):
+                modeled_data = { do something using param_vec }
+                return modeled_data
+
+        This function creates the :class:`pwkit.lmmin.Problem` so that the
+        caller can futz with it before calling :meth:`solve`, if so desired.
+
+        Returns *self*.
 
         """
         from .lmmin import Problem
 
         self.func = func
         self._args = args
-        self.pnames = list (pnames)
-        self.lm_prob = Problem (len (self.pnames))
+        self.pnames = list(pnames)
+        self.lm_prob = Problem(len(self.pnames))
         return self
 
 
-    def set_simple_func (self, func, args=()):
+    def set_simple_func(self, func, args=()):
+        """Set the model function to use a simple but somewhat inefficient calling
+        convention.
+
+        The function should obey the following convention::
+
+            def func(param0, param1, ..., paramN, *args):
+                modeled_data = { do something using the parameters }
+                return modeled_data
+
+        Returns *self*.
+
+        """
         code = get_function_code(func)
-        npar = code.co_argcount - len (args)
+        npar = code.co_argcount - len(args)
         pnames = code.co_varnames[:npar]
 
-        def wrapper (params, *args):
-            return func (*(tuple (params) + args))
+        def wrapper(params, *args):
+            return func(*(tuple(params) + args))
+
+        return self.set_func(wrapper, pnames, args)
 
-        return self.set_func (wrapper, pnames, args)
 
+    def make_frozen_func(self, params):
+        """Returns a model function frozen to the specified parameter values.
 
-    def make_frozen_func (self, params):
-        """Returns a model function frozen to the specified parameter values. Any
-        remaining arguments are left free and must be provided when the
+        Any remaining arguments are left free and must be provided when the
         function is called.
 
-        This just applies `functools.partial` to the `func` property of this
-        object.
+        For this model, the returned function is the application of
+        :func:`functools.partial` to the :attr:`func` property of this object.
 
         """
-        params = np.array (params, dtype=np.float, ndmin=1)
+        params = np.array(params, dtype=np.float, ndmin=1)
         from functools import partial
-        return partial (self.func, params)
+        return partial(self.func, params)
 
 
-    def solve (self, guess):
-        guess = np.array (guess, dtype=np.float, ndmin=1)
+    def solve(self, guess):
+        """Solve for the parameters, using an initial guess.
+
+        This uses the Levenberg-Marquardt optimizer described in
+        :mod:`pwkit.lmmin`.
+
+        Returns *self*.
+
+        """
+        guess = np.array(guess, dtype=np.float, ndmin=1)
         f = self.func
         args = self._args
 
-        def lmfunc (params, vec):
-            vec[:] = f (params, *args).flatten ()
+        def lmfunc(params, vec):
+            vec[:] = f(params, *args).flatten()
 
-        self.lm_prob.set_residual_func (self.data.flatten (),
-                                        self.invsigma.flatten (),
-                                        lmfunc, None)
-        self.lm_soln = soln = self.lm_prob.solve (guess)
+        self.lm_prob.set_residual_func(self.data.flatten(),
+                                       self.invsigma.flatten(),
+                                       lmfunc, None)
+        self.lm_soln = soln = self.lm_prob.solve(guess)
 
         self.params = soln.params
         self.puncerts = soln.perror
         self.covar = soln.covar
-        self.mfunc = self.make_frozen_func (soln.params)
+        self.mfunc = self.make_frozen_func(soln.params)
 
         # fvec = resids * invsigma = (data - mdata) * invsigma
-        self.resids = soln.fvec.reshape (self.data.shape) / self.invsigma
+        self.resids = soln.fvec.reshape(self.data.shape) / self.invsigma
         self.mdata = self.data - self.resids
 
+        # lm_soln.fnorm can be unreliable ("max(fnorm, fnorm1)" branch)
+        self.chisq = (self.lm_soln.fvec**2).sum()
         if soln.ndof > 0:
-            # lm_soln.fnorm can be unreliable ("max (fnorm, fnorm1)" branch)
-            self.rchisq = (self.lm_soln.fvec**2).sum () / soln.ndof
-        else:
-            self.rchisq = None
+            self.rchisq = self.chisq / soln.ndof
+
         return self
 
 
-class PolynomialModel (_ModelBase):
+class PolynomialModel(ModelBase):
     """Least-squares polynomial fit.
 
     Because this is a very specialized kind of problem, we don't need an
     initial guess to solve, and we can use fast built-in numerical routines.
 
     The output parameters are named "a0", "a1", ... and are stored in that
     order in PolynomialModel.params[]. We have ``y = sum(x**i * a[i])``, so
@@ -344,352 +409,364 @@
     uncertainties.
 
     Methods:
 
     as_nonlinear - Return a (lmmin-based) `Model` equivalent to self.
 
     """
-    def __init__ (self, maxexponent, x, data, invsigma=None):
+    def __init__(self, maxexponent, x, data, invsigma=None):
         self.maxexponent = maxexponent
-        self.x = np.array (x, dtype=np.float, ndmin=1, copy=False, subok=True)
-        self.set_data (data, invsigma)
+        self.x = np.array(x, dtype=np.float, ndmin=1, copy=False, subok=True)
+        self.set_data(data, invsigma)
+
+
+    def make_frozen_func(self, params):
+        return lambda x: npoly.polyval(x, params)
 
 
-    def solve (self):
-        self.pnames = ['a%d' % i for i in range (self.maxexponent + 1)]
-        # Based on my reading of the polyfit() docs, I think w=invsigma**2 is right...
-        self.params = npoly.polyfit (self.x, self.data, self.maxexponent,
-                                     w=self.invsigma**2)
+    def solve(self):
+        self.pnames = ['a%d' % i for i in range(self.maxexponent + 1)]
+        self.params = npoly.polyfit(self.x, self.data, self.maxexponent,
+                                    w=self.invsigma)
         self.puncerts = None # does anything provide this? could farm out to lmmin ...
         self.covar = None
-        self.mfunc = lambda x: npoly.polyval (x, self.params)
-        self.mdata = self.mfunc (self.x)
+        self.mfunc = self.make_frozen_func(self.params)
+        self.mdata = self.mfunc(self.x)
         self.resids = self.data - self.mdata
 
+        self.chisq = ((self.resids * self.invsigma)**2).sum()
         if self.x.size > self.maxexponent + 1:
-            self.rchisq = (((self.resids * self.invsigma)**2).sum ()
-                           / (self.x.size - (self.maxexponent + 1)))
-        else:
-            self.rchisq = None
+            self.rchisq = self.chisq / (self.x.size - (self.maxexponent + 1))
 
         return self
 
 
-    def as_nonlinear (self, params=None):
+    def as_nonlinear(self, params=None):
         """Return a `Model` equivalent to this object. The nonlinear solver is less
         efficient, but lets you freeze parameters, compute uncertainties, etc.
 
         If the `params` argument is provided, solve() will be called on the
         returned object with those parameters. If it is `None` and this object
         has parameters in `self.params`, those will be use. Otherwise, solve()
         will not be called on the returned object.
 
         """
         if params is None:
             params = self.params
 
-        nlm = Model (None, self.data, self.invsigma)
-        nlm.set_func (lambda p, x: npoly.polyval (x, p),
-                      self.pnames,
-                      args=(self.x,))
+        nlm = Model(None, self.data, self.invsigma)
+        nlm.set_func(lambda p, x: npoly.polyval(x, p),
+                     self.pnames,
+                     args=(self.x,))
 
         if params is not None:
-            nlm.solve (params)
+            nlm.solve(params)
         return nlm
 
 
-class ScaleModel (_ModelBase):
+class ScaleModel(ModelBase):
     """Solve `data = m * x` for `m`."""
 
-    def __init__ (self, x, data, invsigma=None):
-        self.x = np.array (x, dtype=np.float, ndmin=1, copy=False, subok=True)
-        self.set_data (data, invsigma)
+    def __init__(self, x, data, invsigma=None):
+        self.x = np.array(x, dtype=np.float, ndmin=1, copy=False, subok=True)
+        self.set_data(data, invsigma)
+
 
-    def solve (self):
+    def make_frozen_func(self, params):
+        return lambda x: params[0] * x
+
+
+    def solve(self):
         w2 = self.invsigma**2
-        sxx = np.dot (self.x**2, w2)
-        sxy = np.dot (self.x * self.data, w2)
+        sxx = np.dot(self.x**2, w2)
+        sxy = np.dot(self.x * self.data, w2)
         m = sxy / sxx
-        uc_m = 1. / np.sqrt (sxx)
+        uc_m = 1. / np.sqrt(sxx)
 
         self.pnames = ['m']
-        self.params = np.asarray ([m])
-        self.puncerts = np.asarray ([uc_m])
-        self.covar = self.puncerts.reshape ((1, 1))
+        self.params = np.asarray([m])
+        self.puncerts = np.asarray([uc_m])
+        self.covar = self.puncerts.reshape((1, 1))
         self.mfunc = lambda x: m * x
         self.mdata = m * self.x
         self.resids = self.data - self.mdata
-        self.rchisq = ((self.resids * self.invsigma)**2).sum () / (self.x.size - 1)
+        self.chisq = ((self.resids * self.invsigma)**2).sum()
+        self.rchisq = self.chisq / (self.x.size - 1)
         return self
 
 
 # lmmin-based model-fitting when the model is broken down into composable
 # components.
 
-class ModelComponent (object):
+class ModelComponent(object):
     npar = 0
     name = None
     pnames = ()
     nmodelargs = 0
 
     setguess = None
     setvalue = None
     setlimit = None
     _accum_mfunc = None
 
-    def __init__ (self, name=None):
+    def __init__(self, name=None):
         self.name = name
 
-    def _param_names (self):
+    def _param_names(self):
         """Overridable in case the list of parameter names needs to be
         generated on the fly."""
         return self.pnames
 
-    def finalize_setup (self):
+    def finalize_setup(self):
         """If the component has subcomponents, this should set their `name`,
         `setguess`, `setvalue`, and `setlimit` properties. It should also
         set `npar` (on self) to the final value."""
         pass
 
-    def prep_params (self):
+    def prep_params(self):
         """This should make any necessary calls to `setvalue` or `setlimit`,
         though in straightforward cases it should just be up to the user to
         do this. If the component has subcomponents, their `prep_params`
         functions should be called."""
         pass
 
-    def model (self, pars, mdata):
+    def model(self, pars, mdata):
         """Modify `mdata` based on `pars`."""
         pass
 
-    def deriv (self, pars, jac):
+    def deriv(self, pars, jac):
         """Compute the Jacobian. `jac[i]` is d`mdata`/d`pars[i]`."""
         pass
 
-    def extract (self, pars, perr, cov):
+    def extract(self, pars, perr, cov):
         """Extract fit results into the object for ease of inspection."""
         self.covar = cov
 
-    def _outputshape (self, *args):
+    def _outputshape(self, *args):
         """This is a helper for evaluating the model function at fixed parameters. To
         work in the ComposedModel paradigm, we have to allocate an empty array
         to hold the model output before we can fill it via the _accum_mfunc
         functions. We can't do that without knowing what size it will be. That
         size has to be a function of the "free" parameters to the model
         function that are implicit/fixed during the fitting process. Given these "free"
         parameters, _outputshape returns the shape that the output will have."""
-        raise NotImplementedError ()
+        raise NotImplementedError()
 
-    def mfunc (self, *args):
-        if len (args) != self.nmodelargs:
-            raise TypeError ('model function expected %d arguments, got %d' %
-                             (self.nmodelargs, len (args)))
+    def mfunc(self, *args):
+        if len(args) != self.nmodelargs:
+            raise TypeError('model function expected %d arguments, got %d' %
+                            (self.nmodelargs, len(args)))
 
-        result = np.zeros (self._outputshape (*args))
-        self._accum_mfunc (result, *args)
+        result = np.zeros(self._outputshape(*args))
+        self._accum_mfunc(result, *args)
         return result
 
 
-class ComposedModel (_ModelBase):
-    def __init__ (self, component, data, invsigma=None):
+class ComposedModel(ModelBase):
+    def __init__(self, component, data, invsigma=None):
         if component is not None:
-            self.set_component (component)
+            self.set_component(component)
         if data is not None:
-            self.set_data (data, invsigma)
+            self.set_data(data, invsigma)
 
 
-    def _component_setguess (self, vals, ofs=0):
-        vals = np.asarray (vals)
+    def _component_setguess(self, vals, ofs=0):
+        vals = np.asarray(vals)
         if ofs < 0 or ofs + vals.size > self.component.npar:
-            raise ValueError ('ofs %d, vals.size %d, npar %d' %
-                              (ofs, vals.size, self.component.npar))
+            raise ValueError('ofs %d, vals.size %d, npar %d' %
+                             (ofs, vals.size, self.component.npar))
         self.force_guess[ofs:ofs+vals.size] = vals
 
 
-    def _component_setvalue (self, cidx, val, fixed=False):
+    def _component_setvalue(self, cidx, val, fixed=False):
         if cidx < 0 or cidx >= self.component.npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, self.component.npar))
-        self.lm_prob.p_value (cidx, val, fixed=fixed)
+            raise ValueError('cidx %d, npar %d' % (cidx, self.component.npar))
+        self.lm_prob.p_value(cidx, val, fixed=fixed)
         self.force_guess[cidx] = val
 
 
-    def _component_setlimit (self, cidx, lower=-np.inf, upper=np.inf):
+    def _component_setlimit(self, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= self.component.npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, self.component.npar))
-        self.lm_prob.p_limit (cidx, lower, upper)
+            raise ValueError('cidx %d, npar %d' % (cidx, self.component.npar))
+        self.lm_prob.p_limit(cidx, lower, upper)
 
 
-    def set_component (self, component):
+    def set_component(self, component):
         self.component = component
 
         component.setguess = self._component_setguess
         component.setvalue = self._component_setvalue
         component.setlimit = self._component_setlimit
-        component.finalize_setup ()
+        component.finalize_setup()
 
         from .lmmin import Problem
-        self.lm_prob = Problem (component.npar)
-        self.force_guess = np.empty (component.npar)
-        self.force_guess.fill (np.nan)
-        self.pnames = list (component._param_names ())
+        self.lm_prob = Problem(component.npar)
+        self.force_guess = np.empty(component.npar)
+        self.force_guess.fill(np.nan)
+        self.pnames = list(component._param_names())
 
-        component.prep_params ()
+        component.prep_params()
 
 
-    def solve (self, guess=None):
+    def solve(self, guess=None):
         if guess is None:
             guess = self.force_guess
         else:
-            guess = np.array (guess, dtype=np.float, ndmin=1, copy=True)
+            guess = np.array(guess, dtype=np.float, ndmin=1, copy=True)
 
-            for i in range (self.force_guess.size):
-                if np.isfinite (self.force_guess[i]):
+            for i in range(self.force_guess.size):
+                if np.isfinite(self.force_guess[i]):
                     guess[i] = self.force_guess[i]
 
-        def model (pars, outputs):
-            outputs.fill (0)
-            self.component.model (pars, outputs)
+        def model(pars, outputs):
+            outputs.fill(0)
+            self.component.model(pars, outputs)
 
         self.lm_model = model
         self.lm_deriv = self.component.deriv
-        self.lm_prob.set_residual_func (self.data, self.invsigma, model,
-                                        self.component.deriv)
-        self.lm_soln = soln = self.lm_prob.solve (guess)
+        self.lm_prob.set_residual_func(self.data, self.invsigma, model,
+                                       self.component.deriv)
+        self.lm_soln = soln = self.lm_prob.solve(guess)
 
         self.params = soln.params
         self.puncerts = soln.perror
         self.covar = soln.covar
 
         # fvec = resids * invsigma = (data - mdata) * invsigma
-        self.resids = self.lm_soln.fvec.reshape (self.data.shape) / self.invsigma
+        self.resids = self.lm_soln.fvec.reshape(self.data.shape) / self.invsigma
         self.mdata = self.data - self.resids
 
+        # lm_soln.fnorm can be unreliable ("max(fnorm, fnorm1)" branch)
+        self.chisq = (self.lm_soln.fvec**2).sum()
         if soln.ndof > 0:
-            # lm_soln.fnorm can be unreliable ("max (fnorm, fnorm1)" branch)
-            self.rchisq = (self.lm_soln.fvec**2).sum () / soln.ndof
+            self.rchisq = self.chisq / soln.ndof
 
-        self.component.extract (soln.params, soln.perror, soln.covar)
+        self.component.extract(soln.params, soln.perror, soln.covar)
         return self
 
 
-    def mfunc (self, *args):
-        return self.component.mfunc (*args)
+    def make_frozen_func(self):
+        return self.component.mfunc
+
+
+    def mfunc(self, *args):
+        return self.component.mfunc(*args)
 
 
-    def debug_derivative (self, guess):
+    def debug_derivative(self, guess):
         """returns (explicit, auto)"""
         from .lmmin import check_derivative
-        return check_derivative (self.component.npar, self.data.size,
-                                 self.lm_model, self.lm_deriv, guess)
+        return check_derivative(self.component.npar, self.data.size,
+                                self.lm_model, self.lm_deriv, guess)
 
 
 # Now specific components useful in the above framework. The general strategy
 # is to err on the side of having additional parameters in the individual
 # classes, and the user can call setvalue() to fix them if they're not needed.
 
-class AddConstantComponent (ModelComponent):
+class AddConstantComponent(ModelComponent):
     npar = 1
     pnames = ('value', )
     nmodelargs = 0
 
-    def model (self, pars, mdata):
+    def model(self, pars, mdata):
         mdata += pars[0]
 
-    def deriv (self, pars, jac):
+    def deriv(self, pars, jac):
         jac[0] = 1.
 
-    def _outputshape (self):
-        return ()
+    def _outputshape(self):
+        return()
 
-    def extract (self, pars, perr, cov):
-        def _accum_mfunc (res):
+    def extract(self, pars, perr, cov):
+        def _accum_mfunc(res):
             res += pars[0]
         self._accum_mfunc = _accum_mfunc
 
         self.covar = cov
         self.f_value = pars[0]
         self.u_value = perr[0]
 
 
-class AddValuesComponent (ModelComponent):
+class AddValuesComponent(ModelComponent):
     """XXX terminology between this and AddConstant is mushy."""
     nmodelargs = 0
 
-    def __init__ (self, nvals, name=None):
-        super (AddValuesComponent, self).__init__ (name)
+    def __init__(self, nvals, name=None):
+        super(AddValuesComponent, self).__init__(name)
         self.npar = nvals
 
-    def _param_names (self):
-        for i in range (self.npar):
+    def _param_names(self):
+        for i in range(self.npar):
             yield 'v%d' % i
 
-    def model (self, pars, mdata):
+    def model(self, pars, mdata):
         mdata += pars
 
-    def deriv (self, pars, jac):
-        jac[:,:] = np.eye (self.npar)
+    def deriv(self, pars, jac):
+        jac[:,:] = np.eye(self.npar)
 
-    def _outputshape (self):
-        return (self.npar,)
+    def _outputshape(self):
+        return(self.npar,)
 
-    def extract (self, pars, perr, cov):
-        def _accum_mfunc (res):
+    def extract(self, pars, perr, cov):
+        def _accum_mfunc(res):
             res += pars
         self._accum_mfunc = _accum_mfunc
 
         self.covar = cov
         self.f_vals = pars
         self.u_vals = perr
 
 
-class AddPolynomialComponent (ModelComponent):
+class AddPolynomialComponent(ModelComponent):
     nmodelargs = 1
 
-    def __init__ (self, maxexponent, x, name=None):
-        super (AddPolynomialComponent, self).__init__ (name)
+    def __init__(self, maxexponent, x, name=None):
+        super(AddPolynomialComponent, self).__init__(name)
         self.npar = maxexponent + 1
-        self.x = np.array (x, dtype=np.float, ndmin=1, copy=False, subok=True)
+        self.x = np.array(x, dtype=np.float, ndmin=1, copy=False, subok=True)
 
-    def _param_names (self):
-        for i in range (self.npar):
+    def _param_names(self):
+        for i in range(self.npar):
             yield 'c%d' % i
 
-    def model (self, pars, mdata):
-        mdata += npoly.polyval (self.x, pars)
+    def model(self, pars, mdata):
+        mdata += npoly.polyval(self.x, pars)
 
-    def deriv (self, pars, jac):
-        w = np.ones_like (self.x)
+    def deriv(self, pars, jac):
+        w = np.ones_like(self.x)
 
-        for i in range (self.npar):
+        for i in range(self.npar):
             jac[i] = w
             w *= self.x
 
-    def _outputshape (self, x):
+    def _outputshape(self, x):
         return x.shape
 
-    def extract (self, pars, perr, cov):
-        def _accum_mfunc (res, x):
-            res += npoly.polyval (x, pars)
+    def extract(self, pars, perr, cov):
+        def _accum_mfunc(res, x):
+            res += npoly.polyval(x, pars)
         self._accum_mfunc = _accum_mfunc
 
         self.covar = cov
         self.f_coeffs = pars
         self.u_coeffs = perr
 
 
-def _broadcast_shapes (s1, s2):
+def _broadcast_shapes(s1, s2):
     """Given array shapes `s1` and `s2`, compute the shape of the array that would
     result from broadcasting them together."""
 
-    n1 = len (s1)
-    n2 = len (s2)
-    n = max (n1, n2)
+    n1 = len(s1)
+    n2 = len(s2)
+    n = max(n1, n2)
     res = [1] * n
 
-    for i in range (n):
+    for i in range(n):
         if i >= n1:
             c1 = 1
         else:
             c1 = s1[n1-1-i]
 
         if i >= n2:
             c2 = 1
@@ -697,395 +774,395 @@
             c2 = s2[n2-1-i]
 
         if c1 == 1:
             rc = c2
         elif c2 == 1 or c1 == c2:
             rc = c1
         else:
-            raise ValueError ('array shapes %r and %r are not compatible' % (s1, s2))
+            raise ValueError('array shapes %r and %r are not compatible' % (s1, s2))
 
         res[n-1-i] = rc
 
-    return tuple (res)
+    return tuple(res)
 
 
-class SeriesComponent (ModelComponent):
+class SeriesComponent(ModelComponent):
     """Apply a set of subcomponents in series, isolating each from the other. This
     is only valid if every subcomponent except the first is additive --
     otherwise, the Jacobian won't be right."""
 
-    def __init__ (self, components=(), name=None):
-        super (SeriesComponent, self).__init__ (name)
-        self.components = list (components)
+    def __init__(self, components=(), name=None):
+        super(SeriesComponent, self).__init__(name)
+        self.components = list(components)
 
 
-    def add (self, component):
+    def add(self, component):
         """This helps, but direct manipulation of self.components should be
         supported."""
-        self.components.append (component)
+        self.components.append(component)
         return self
 
 
-    def _param_names (self):
+    def _param_names(self):
         for c in self.components:
             pfx = c.name + '.' if c.name is not None else ''
-            for p in c._param_names ():
+            for p in c._param_names():
                 yield pfx + p
 
 
-    def _offset_setguess (self, ofs, npar, vals, subofs=0):
-        vals = np.asarray (vals)
+    def _offset_setguess(self, ofs, npar, vals, subofs=0):
+        vals = np.asarray(vals)
         if subofs < 0 or subofs + vals.size > npar:
-            raise ValueError ('subofs %d, vals.size %d, npar %d' %
-                              (subofs, vals.size, npar))
-        return self.setguess (vals, ofs + subofs)
+            raise ValueError('subofs %d, vals.size %d, npar %d' %
+                             (subofs, vals.size, npar))
+        return self.setguess(vals, ofs + subofs)
 
 
-    def _offset_setvalue (self, ofs, npar, cidx, value, fixed=False):
+    def _offset_setvalue(self, ofs, npar, cidx, value, fixed=False):
         if cidx < 0 or cidx >= npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, npar))
-        return self.setvalue (ofs + cidx, value, fixed)
+            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+        return self.setvalue(ofs + cidx, value, fixed)
 
 
-    def _offset_setlimit (self, ofs, npar, cidx, lower=-np.inf, upper=np.inf):
+    def _offset_setlimit(self, ofs, npar, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, npar))
-        return self.setlimit (ofs + cidx, lower, upper)
+            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+        return self.setlimit(ofs + cidx, lower, upper)
 
 
-    def finalize_setup (self):
+    def finalize_setup(self):
         from functools import partial
 
         ofs = 0
         self.nmodelargs = 0
 
-        for i, c in enumerate (self.components):
+        for i, c in enumerate(self.components):
             if c.name is None:
                 c.name = 'c%d' % i
 
-            c.setguess = partial (self._offset_setguess, ofs, c.npar)
-            c.setvalue = partial (self._offset_setvalue, ofs, c.npar)
-            c.setlimit = partial (self._offset_setlimit, ofs, c.npar)
-            c.finalize_setup ()
+            c.setguess = partial(self._offset_setguess, ofs, c.npar)
+            c.setvalue = partial(self._offset_setvalue, ofs, c.npar)
+            c.setlimit = partial(self._offset_setlimit, ofs, c.npar)
+            c.finalize_setup()
             ofs += c.npar
             self.nmodelargs += c.nmodelargs
 
         self.npar = ofs
 
 
-    def prep_params (self):
+    def prep_params(self):
         for c in self.components:
-            c.prep_params ()
+            c.prep_params()
 
 
-    def model (self, pars, mdata):
+    def model(self, pars, mdata):
         ofs = 0
 
         for c in self.components:
             p = pars[ofs:ofs+c.npar]
-            c.model (p, mdata)
+            c.model(p, mdata)
             ofs += c.npar
 
 
-    def deriv (self, pars, jac):
+    def deriv(self, pars, jac):
         ofs = 0
 
         for c in self.components:
             p = pars[ofs:ofs+c.npar]
             j = jac[ofs:ofs+c.npar]
-            c.deriv (p, j)
+            c.deriv(p, j)
             ofs += c.npar
 
 
-    def extract (self, pars, perr, cov):
+    def extract(self, pars, perr, cov):
         ofs = 0
 
         for c in self.components:
             n = c.npar
 
             spar = pars[ofs:ofs+n]
             serr = perr[ofs:ofs+n]
             scov = cov[ofs:ofs+n,ofs:ofs+n]
-            c.extract (spar, serr, scov)
+            c.extract(spar, serr, scov)
             ofs += n
 
 
-    def _outputshape (self, *args):
+    def _outputshape(self, *args):
         s = ()
         ofs = 0
 
         for c in self.components:
             cargs = args[ofs:ofs+c.nmodelargs]
-            s = _broadcast_shapes (s, c._outputshape (*cargs))
+            s = _broadcast_shapes(s, c._outputshape(*cargs))
             ofs += c.nmodelargs
 
         return s
 
 
-    def _accum_mfunc (self, res, *args):
+    def _accum_mfunc(self, res, *args):
         ofs = 0
 
         for c in self.components:
             cargs = args[ofs:ofs+c.nmodelargs]
-            c._accum_mfunc (res, *cargs)
+            c._accum_mfunc(res, *cargs)
             ofs += c.nmodelargs
 
 
-class MatMultComponent (ModelComponent):
+class MatMultComponent(ModelComponent):
     """Given a component yielding k**2 data points and k additional components,
     each yielding n data points. The result is [A]×[B], where A is the square
     matrix formed from the first component's output, and B is the (k, n)
     matrix of stacked output from the final k components.
 
     Parameters are ordered in same way as the components named above.
     """
 
-    def __init__ (self, k, name=None):
-        super (MatMultComponent, self).__init__ (name)
+    def __init__(self, k, name=None):
+        super(MatMultComponent, self).__init__(name)
         self.k = k
         self.acomponent = None
         self.bcomponents = [None] * k
 
 
-    def _param_names (self):
+    def _param_names(self):
         pfx = self.acomponent.name + '.' if self.acomponent.name is not None else ''
-        for p in self.acomponent._param_names ():
+        for p in self.acomponent._param_names():
             yield pfx + p
 
         for c in self.bcomponents:
             pfx = c.name + '.' if c.name is not None else ''
-            for p in c._param_names ():
+            for p in c._param_names():
                 yield pfx + p
 
 
-    def _offset_setguess (self, ofs, npar, vals, subofs=0):
-        vals = np.asarray (vals)
+    def _offset_setguess(self, ofs, npar, vals, subofs=0):
+        vals = np.asarray(vals)
         if subofs < 0 or subofs + vals.size > npar:
-            raise ValueError ('subofs %d, vals.size %d, npar %d' %
-                              (subofs, vals.size, npar))
-        return self.setguess (vals, ofs + subofs)
+            raise ValueError('subofs %d, vals.size %d, npar %d' %
+                             (subofs, vals.size, npar))
+        return self.setguess(vals, ofs + subofs)
 
 
-    def _offset_setvalue (self, ofs, npar, cidx, value, fixed=False):
+    def _offset_setvalue(self, ofs, npar, cidx, value, fixed=False):
         if cidx < 0 or cidx >= npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, npar))
-        return self.setvalue (ofs + cidx, value, fixed)
+            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+        return self.setvalue(ofs + cidx, value, fixed)
 
 
-    def _offset_setlimit (self, ofs, npar, cidx, lower=-np.inf, upper=np.inf):
+    def _offset_setlimit(self, ofs, npar, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, npar))
-        return self.setlimit (ofs + cidx, lower, upper)
+            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+        return self.setlimit(ofs + cidx, lower, upper)
 
 
-    def finalize_setup (self):
+    def finalize_setup(self):
         from functools import partial
 
         c = self.acomponent
 
         if c.name is None:
             c.name = 'a'
 
-        c.setguess = partial (self._offset_setguess, 0, c.npar)
-        c.setvalue = partial (self._offset_setvalue, 0, c.npar)
-        c.setlimit = partial (self._offset_setlimit, 0, c.npar)
-        c.finalize_setup ()
+        c.setguess = partial(self._offset_setguess, 0, c.npar)
+        c.setvalue = partial(self._offset_setvalue, 0, c.npar)
+        c.setlimit = partial(self._offset_setlimit, 0, c.npar)
+        c.finalize_setup()
         ofs = c.npar
         self.nmodelargs = c.nmodelargs
 
-        for i, c in enumerate (self.bcomponents):
+        for i, c in enumerate(self.bcomponents):
             if c.name is None:
                 c.name = 'b%d' % i
 
-            c.setguess = partial (self._offset_setguess, ofs, c.npar)
-            c.setvalue = partial (self._offset_setvalue, ofs, c.npar)
-            c.setlimit = partial (self._offset_setlimit, ofs, c.npar)
-            c.finalize_setup ()
+            c.setguess = partial(self._offset_setguess, ofs, c.npar)
+            c.setvalue = partial(self._offset_setvalue, ofs, c.npar)
+            c.setlimit = partial(self._offset_setlimit, ofs, c.npar)
+            c.finalize_setup()
             ofs += c.npar
             self.nmodelargs += c.nmodelargs
 
         self.npar = ofs
 
 
-    def prep_params (self):
-        self.acomponent.prep_params ()
+    def prep_params(self):
+        self.acomponent.prep_params()
 
         for c in self.bcomponents:
-            c.prep_params ()
+            c.prep_params()
 
 
-    def _sep_model (self, pars, nd):
+    def _sep_model(self, pars, nd):
         k = self.k
-        ma = np.zeros ((k, k))
-        mb = np.zeros ((k, nd))
+        ma = np.zeros((k, k))
+        mb = np.zeros((k, nd))
 
         c = self.acomponent
-        c.model (pars[:c.npar], ma.reshape (k**2))
+        c.model(pars[:c.npar], ma.reshape(k**2))
 
         pofs = c.npar
 
-        for i, c in enumerate (self.bcomponents):
+        for i, c in enumerate(self.bcomponents):
             p = pars[pofs:pofs+c.npar]
-            c.model (p, mb[i])
+            c.model(p, mb[i])
             pofs += c.npar
 
         return ma, mb
 
 
-    def model (self, pars, mdata):
+    def model(self, pars, mdata):
         k = self.k
         nd = mdata.size // k
-        ma, mb = self._sep_model (pars, nd)
-        np.dot (ma, mb, mdata.reshape ((k, nd)))
+        ma, mb = self._sep_model(pars, nd)
+        np.dot(ma, mb, mdata.reshape((k, nd)))
 
 
-    def deriv (self, pars, jac):
+    def deriv(self, pars, jac):
         k = self.k
         nd = jac.shape[1] // k
         npar = self.npar
 
-        ma, mb = self._sep_model (pars, nd)
-        ja = np.zeros ((npar, k, k))
-        jb = np.zeros ((npar, k, nd))
+        ma, mb = self._sep_model(pars, nd)
+        ja = np.zeros((npar, k, k))
+        jb = np.zeros((npar, k, nd))
 
         c = self.acomponent
-        c.deriv (pars[:c.npar], ja[:c.npar].reshape ((c.npar, k**2)))
+        c.deriv(pars[:c.npar], ja[:c.npar].reshape((c.npar, k**2)))
         pofs = c.npar
 
-        for i, c in enumerate (self.bcomponents):
+        for i, c in enumerate(self.bcomponents):
             p = pars[pofs:pofs+c.npar]
-            c.deriv (p, jb[pofs:pofs+c.npar,i,:])
+            c.deriv(p, jb[pofs:pofs+c.npar,i,:])
             pofs += c.npar
 
-        for i in range (self.npar):
-            jac[i] = (np.dot (ja[i], mb) + np.dot (ma, jb[i])).reshape (k * nd)
+        for i in range(self.npar):
+            jac[i] = (np.dot(ja[i], mb) + np.dot(ma, jb[i])).reshape(k * nd)
 
 
-    def extract (self, pars, perr, cov):
+    def extract(self, pars, perr, cov):
         c = self.acomponent
-        c.extract (pars[:c.npar], perr[:c.npar], cov[:c.npar,:c.npar])
+        c.extract(pars[:c.npar], perr[:c.npar], cov[:c.npar,:c.npar])
         ofs = c.npar
 
         for c in self.bcomponents:
             n = c.npar
 
             spar = pars[ofs:ofs+n]
             serr = perr[ofs:ofs+n]
             scov = cov[ofs:ofs+n,ofs:ofs+n]
-            c.extract (spar, serr, scov)
+            c.extract(spar, serr, scov)
             ofs += n
 
 
-    def _outputshape (self, *args):
+    def _outputshape(self, *args):
         aofs = self.acomponent.nmodelargs
         sb = ()
 
         for c in self.bcomponents:
             a = args[aofs:aofs+c.nmodelargs]
-            sb = _broadcast_shapes (sb, c._outputshape (*a))
+            sb = _broadcast_shapes(sb, c._outputshape(*a))
             aofs += c.nmodelargs
 
         return (self.k,) + sb
 
 
-    def _accum_mfunc (self, res, *args):
+    def _accum_mfunc(self, res, *args):
         k = self.k
         nd = res.shape[1]
 
-        ma = np.zeros ((k, k))
-        mb = np.zeros ((k, nd))
+        ma = np.zeros((k, k))
+        mb = np.zeros((k, nd))
 
         c = self.acomponent
-        c._accum_mfunc (ma.reshape (k**2), *(args[:c.nmodelargs]))
+        c._accum_mfunc(ma.reshape(k**2), *(args[:c.nmodelargs]))
         aofs = c.nmodelargs
 
-        for i, c in enumerate (self.bcomponents):
+        for i, c in enumerate(self.bcomponents):
             a = args[aofs:aofs+c.nmodelargs]
-            c._accum_mfunc (mb[i], *a)
+            c._accum_mfunc(mb[i], *a)
             aofs += c.nmodelargs
 
-        np.dot (ma, mb, res)
+        np.dot(ma, mb, res)
 
 
-class ScaleComponent (ModelComponent):
+class ScaleComponent(ModelComponent):
     npar = 1
 
-    def __init__ (self, subcomp=None, name=None):
-        super (ScaleComponent, self).__init__ (name)
-        self.setsubcomp (subcomp)
+    def __init__(self, subcomp=None, name=None):
+        super(ScaleComponent, self).__init__(name)
+        self.setsubcomp(subcomp)
 
 
-    def setsubcomp (self, subcomp):
+    def setsubcomp(self, subcomp):
         self.subcomp = subcomp
         return self
 
 
-    def _param_names (self):
+    def _param_names(self):
         yield 'factor'
 
         pfx = self.subcomp.name + '.' if self.subcomp.name is not None else ''
-        for p in self.subcomp._param_names ():
+        for p in self.subcomp._param_names():
             yield pfx + p
 
 
-    def _sub_setguess (self, npar, cidx, vals, ofs=0):
-        vals = np.asarray (vals)
+    def _sub_setguess(self, npar, cidx, vals, ofs=0):
+        vals = np.asarray(vals)
         if ofs < 0 or ofs + vals.size > npar:
-            raise ValueError ('ofs %d, vals.size %d, npar %d' %
-                              (ofs, vals.size, npar))
-        return self.setguess (vals, ofs + 1)
+            raise ValueError('ofs %d, vals.size %d, npar %d' %
+                             (ofs, vals.size, npar))
+        return self.setguess(vals, ofs + 1)
 
 
-    def _sub_setvalue (self, npar, cidx, value, fixed=False):
+    def _sub_setvalue(self, npar, cidx, value, fixed=False):
         if cidx < 0 or cidx >= npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, npar))
-        return self.setvalue (1 + cidx, value, fixed)
+            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+        return self.setvalue(1 + cidx, value, fixed)
 
 
-    def _sub_setlimit (self, npar, cidx, lower=-np.inf, upper=np.inf):
+    def _sub_setlimit(self, npar, cidx, lower=-np.inf, upper=np.inf):
         if cidx < 0 or cidx >= npar:
-            raise ValueError ('cidx %d, npar %d' % (cidx, npar))
-        return self.setlimit (1 + cidx, lower, upper)
+            raise ValueError('cidx %d, npar %d' % (cidx, npar))
+        return self.setlimit(1 + cidx, lower, upper)
 
 
-    def finalize_setup (self):
+    def finalize_setup(self):
         if self.subcomp.name is None:
             self.subcomp.name = 'c'
 
         from functools import partial
-        self.subcomp.setvalue = partial (self._sub_setvalue, self.subcomp.npar)
-        self.subcomp.setlimit = partial (self._sub_setvalue, self.subcomp.npar)
-        self.subcomp.finalize_setup ()
+        self.subcomp.setvalue = partial(self._sub_setvalue, self.subcomp.npar)
+        self.subcomp.setlimit = partial(self._sub_setvalue, self.subcomp.npar)
+        self.subcomp.finalize_setup()
 
         self.npar = self.subcomp.npar + 1
         self.nmodelargs = self.subcomp.nmodelargs
 
 
-    def prep_params (self):
-        self.subcomp.prep_params ()
+    def prep_params(self):
+        self.subcomp.prep_params()
 
 
-    def model (self, pars, mdata):
-        self.subcomp.model (pars[1:], mdata)
+    def model(self, pars, mdata):
+        self.subcomp.model(pars[1:], mdata)
         mdata *= pars[0]
 
 
-    def deriv (self, pars, jac):
-        self.subcomp.model (pars[1:], jac[0])
-        self.subcomp.deriv (pars[1:], jac[1:])
+    def deriv(self, pars, jac):
+        self.subcomp.model(pars[1:], jac[0])
+        self.subcomp.deriv(pars[1:], jac[1:])
         jac[1:] *= pars[0]
 
 
-    def extract (self, pars, perr, cov):
+    def extract(self, pars, perr, cov):
         self.f_factor = pars[0]
         self.u_factor = perr[0]
         self.c_factor = cov[0]
 
-        self.subcomp.extract (pars[1:], perr[1:], cov[1:,1:])
+        self.subcomp.extract(pars[1:], perr[1:], cov[1:,1:])
 
 
-    def _outputshape (self, *args):
-        return self.subcomp._outputshape (*args)
+    def _outputshape(self, *args):
+        return self.subcomp._outputshape(*args)
 
 
-    def _accum_mfunc (self, res, *args):
-        self.subcomp._accum_mfunc (res, *args)
+    def _accum_mfunc(self, res, *args):
+        self.subcomp._accum_mfunc(res, *args)
```

### Comparing `pwkit-0.8.9/pwkit/simpleenum.py` & `pwkit-1.0.0/pwkit/simpleenum.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/pdm.py` & `pwkit-1.0.0/pwkit/pdm.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/radio_cal_models.py` & `pwkit-1.0.0/pwkit/radio_cal_models.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/contours.py` & `pwkit-1.0.0/pwkit/contours.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/bblocks.py` & `pwkit-1.0.0/pwkit/bblocks.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/inifile.py` & `pwkit-1.0.0/pwkit/inifile.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/method_decorator.py` & `pwkit-1.0.0/pwkit/method_decorator.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/cgs.py` & `pwkit-1.0.0/pwkit/cgs.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data_gui_helpers.py` & `pwkit-1.0.0/pwkit/data_gui_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2012-2014 Peter Williams <peter@newton.cx> and collaborators
+# Copyright 2012-2014, 2019 Peter Williams <peter@newton.cx> and collaborators
 # Licensed under the MIT License.
 
 """pwkit.data_gui_helpers - helpers for GUIs looking at data arrays
 
 Classes:
 
 Clipper      - Map data into [0,1]
@@ -12,280 +12,299 @@
 
 Functions:
 
 data_to_argb32       - Turn arbitrary data values into ARGB32 colors.
 data_to_imagesurface - Turn arbitrary data values into a Cairo ImageSurface.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('data_to_argb32 Clipper ColorMapper LazyComputer Stretcher').split ()
+__all__ = '''
+data_to_argb32
+data_to_imagesurface
+Clipper
+ColorMapper
+LazyComputer
+Stretcher'''.split()
 
 import numpy as np
 from six.moves import range
 
 from . import colormaps
 
 
 DEFAULT_TILESIZE = 128
 
-class LazyComputer (object):
+class LazyComputer(object):
     buffer = None
     tilesize = None
     valid = None
 
-    def set_buffer (self, buffer):
+    def set_buffer(self, buffer):
         self.buffer = buffer
         return self
 
 
-    def alloc_buffer (self, template):
-        if np.ma.is_masked (template):
-            self.buffer = np.ma.empty (template.shape)
+    def alloc_buffer(self, template):
+        if np.ma.is_masked(template):
+            self.buffer = np.ma.empty(template.shape)
             self.buffer.mask = template.mask
         else:
-            self.buffer = np.empty (template.shape)
+            self.buffer = np.empty(template.shape)
         return self
 
 
-    def set_tile_size (self, tilesize=DEFAULT_TILESIZE):
+    def set_tile_size(self, tilesize=DEFAULT_TILESIZE):
         self.tilesize = tilesize
         h, w = self.buffer.shape
         nxt = (w + tilesize - 1) // tilesize
         nyt = (h + tilesize - 1) // tilesize
-        self.valid = np.zeros ((nyt, nxt))
+        self.valid = np.zeros((nyt, nxt))
         return self
 
 
-    def ensure_region_updated (self, data, xoffset, yoffset, width, height):
+    def ensure_region_updated(self, data, xoffset, yoffset, width, height):
         ts = self.tilesize
         buf = self.buffer
         valid = self.valid
-        func = self._make_func (np.ma.is_masked (data))
+        func = self._make_func(np.ma.is_masked(data))
 
         tilej = xoffset // ts
         tilei = yoffset // ts
         nxt = (xoffset + width + ts - 1) // ts - tilej
         nyt = (yoffset + height + ts - 1) // ts - tilei
 
         tyofs = tilei
         pyofs = tilei * ts
 
-        for i in range (nyt):
+        for i in range(nyt):
             txofs = tilej
             pxofs = tilej * ts
 
-            for j in range (nxt):
+            for j in range(nxt):
                 if not valid[tyofs,txofs]:
-                    func (data[pyofs:pyofs+ts,pxofs:pxofs+ts],
-                          buf[pyofs:pyofs+ts,pxofs:pxofs+ts])
+                    func(data[pyofs:pyofs+ts,pxofs:pxofs+ts],
+                         buf[pyofs:pyofs+ts,pxofs:pxofs+ts])
                     valid[tyofs,txofs] = 1
 
                 pxofs += ts
                 txofs += 1
             pyofs += ts
             tyofs += 1
 
         return self
 
 
-    def ensure_all_updated (self, data):
-        return self.ensure_region_updated (data, 0, 0, data.shape[1], data.shape[0])
+    def ensure_all_updated(self, data):
+        return self.ensure_region_updated(data, 0, 0, data.shape[1], data.shape[0])
 
 
-    def invalidate (self):
-        self.valid.fill (0)
+    def invalidate(self):
+        self.valid.fill(0)
         return self
 
 
-class Clipper (LazyComputer):
+class Clipper(LazyComputer):
     dmin = None
     dmax = None
 
-    def default_bounds (self, data):
-        dmin, dmax = data.min (), data.max ()
+    def default_bounds(self, data):
+        dmin, dmax = data.min(), data.max()
 
-        if not np.isfinite (dmin):
-            dmin = data[np.ma.where (np.isfinite (data))].min ()
-        if not np.isfinite (dmax):
-            dmax = data[np.ma.where (np.isfinite (data))].max ()
+        if not np.isfinite(dmin):
+            dmin = data[np.ma.where(np.isfinite(data))].min()
+        if not np.isfinite(dmax):
+            dmax = data[np.ma.where(np.isfinite(data))].max()
 
         self.dmin = dmin
         self.dmax = dmax
         return self
 
 
-    def _make_func (self, ismasked):
+    def _make_func(self, ismasked):
         dmin = self.dmin
         scale = 1. / (self.dmax - dmin)
 
         if ismasked:
-            def func (src, dest):
+            def func(src, dest):
                 # As of Numpy 1.13, the `mask` parameter gets turned into a
                 # scalar of we operate on the full MaskedArray object (e.g.,
                 # `dest` not `dest.data`), which causes the vector mask
                 # assignment to fail.
-                np.subtract (src, dmin, dest.data)
-                np.multiply (dest.data, scale, dest.data)
-                np.clip (dest.data, 0, 1, dest.data)
+                np.subtract(src, dmin, dest.data)
+                np.multiply(dest.data, scale, dest.data)
+                np.clip(dest.data, 0, 1, dest.data)
                 dest.mask[...] = src.mask
         else:
-            def func (src, dest):
-                np.subtract (src, dmin, dest)
-                np.multiply (dest, scale, dest)
-                np.clip (dest, 0, 1, dest)
+            def func(src, dest):
+                np.subtract(src, dmin, dest)
+                np.multiply(dest, scale, dest)
+                np.clip(dest, 0, 1, dest)
 
         return func
 
 
-class Stretcher (LazyComputer):
+class Stretcher(LazyComputer):
     """Assumes that its inputs are in [0, 1]. Maps its outputs to the same
     range.
 
     """
 
-    def passthrough (src, dest):
+    def passthrough(src, dest):
         dest[...] = src
 
+    def offset_cbrt(src, dest):
+        """This stretch is useful when you have values that are symmetrical around
+        zero, and you want to enhance contrasts at small values while
+        preserving sign.
+
+        """
+        np.subtract(src, 0.5, out=dest) # [0, 1] -> [-0.5, 0.5]
+        np.multiply(dest, 2, out=dest) # [-0.5, 0.5] => [-1, 1]
+        np.cbrt(dest, out=dest) # domain remains same
+        np.multiply(dest, 0.5, out=dest) # [-1, 1] => [-0.5, 0.5]
+        np.add(dest, 0.5, out=dest) # [-0.5, 0.5] => [0, 1]
+
     modes = {
         'linear': passthrough,
+        'offset_cbrt': offset_cbrt,
         'sqrt': np.sqrt,
         'square': np.square,
     }
 
-    def __init__ (self, mode):
+    def __init__(self, mode):
         if mode not in self.modes:
-            raise ValueError ('unrecognized Stretcher mode %r', mode)
+            raise ValueError('unrecognized Stretcher mode %r', mode)
 
         self.mode = mode
 
-    def _make_func (self, ismasked):
+    def _make_func(self, ismasked):
         return self.modes[self.mode]
 
 
-class ColorMapper (LazyComputer):
+class ColorMapper(LazyComputer):
     mapper = None
 
-    def __init__ (self, mapname):
+    def __init__(self, mapname):
         if mapname is not None:
-            self.mapper = colormaps.factory_map[mapname] ()
+            self.mapper = colormaps.factory_map[mapname]()
 
 
-    def alloc_buffer (self, template):
-        self.buffer = np.empty (template.shape, dtype=np.uint32)
-        self.buffer.fill (0xFF000000)
+    def alloc_buffer(self, template):
+        self.buffer = np.empty(template.shape, dtype=np.uint32)
+        self.buffer.fill(0xFF000000)
         return self
 
 
-    def _make_func (self, ismasked):
+    def _make_func(self, ismasked):
         mapper = self.mapper
 
         if not ismasked:
-            def func (src, dest):
-                mapped = mapper (src)
-                dest.fill (0xFF000000)
-                effscratch = (mapped[:,:,0] * 0xFF).astype (np.uint32)
-                np.left_shift (effscratch, 16, effscratch)
-                np.bitwise_or (dest, effscratch, dest)
-                effscratch = (mapped[:,:,1] * 0xFF).astype (np.uint32)
-                np.left_shift (effscratch, 8, effscratch)
-                np.bitwise_or (dest, effscratch, dest)
-                effscratch = (mapped[:,:,2] * 0xFF).astype (np.uint32)
-                np.bitwise_or (dest, effscratch, dest)
+            def func(src, dest):
+                mapped = mapper(src)
+                dest.fill(0xFF000000)
+                effscratch = (mapped[:,:,0] * 0xFF).astype(np.uint32)
+                np.left_shift(effscratch, 16, effscratch)
+                np.bitwise_or(dest, effscratch, dest)
+                effscratch = (mapped[:,:,1] * 0xFF).astype(np.uint32)
+                np.left_shift(effscratch, 8, effscratch)
+                np.bitwise_or(dest, effscratch, dest)
+                effscratch = (mapped[:,:,2] * 0xFF).astype(np.uint32)
+                np.bitwise_or(dest, effscratch, dest)
         else:
-            scratch2 = np.zeros ((self.tilesize, self.tilesize), dtype=np.uint32)
+            scratch2 = np.zeros((self.tilesize, self.tilesize), dtype=np.uint32)
 
-            def func (src, dest):
+            def func(src, dest):
                 effscratch2 = scratch2[:dest.shape[0],:dest.shape[1]]
-                mapped = mapper (src)
+                mapped = mapper(src)
 
-                dest.fill (0xFF000000)
-                effscratch = (mapped[:,:,0] * 0xFF).astype (np.uint32)
-                np.left_shift (effscratch, 16, effscratch)
-                np.bitwise_or (dest, effscratch, dest)
-                effscratch = (mapped[:,:,1] * 0xFF).astype (np.uint32)
-                np.left_shift (effscratch, 8, effscratch)
-                np.bitwise_or (dest, effscratch, dest)
-                effscratch = (mapped[:,:,2] * 0xFF).astype (np.uint32)
-                np.bitwise_or (dest, effscratch, dest)
+                dest.fill(0xFF000000)
+                effscratch = (mapped[:,:,0] * 0xFF).astype(np.uint32)
+                np.left_shift(effscratch, 16, effscratch)
+                np.bitwise_or(dest, effscratch, dest)
+                effscratch = (mapped[:,:,1] * 0xFF).astype(np.uint32)
+                np.left_shift(effscratch, 8, effscratch)
+                np.bitwise_or(dest, effscratch, dest)
+                effscratch = (mapped[:,:,2] * 0xFF).astype(np.uint32)
+                np.bitwise_or(dest, effscratch, dest)
 
-                np.invert (src.mask, effscratch2)
-                np.multiply (dest, effscratch2, dest)
+                np.invert(src.mask, effscratch2)
+                np.multiply(dest, effscratch2, dest)
 
         return func
 
 
-def data_to_argb32 (data, cmin=None, cmax=None, stretch='linear', cmap='black_to_blue'):
+def data_to_argb32(data, cmin=None, cmax=None, stretch='linear', cmap='black_to_blue'):
     """Turn arbitrary data values into ARGB32 colors.
 
     There are three steps to this process: clipping the data values to a
     maximum and minimum; stretching the spacing between those values; and
     converting their amplitudes into colors with some kind of color map.
 
     `data`    - Input data; can (and should) be a MaskedArray if some values are
                 invalid.
     `cmin`    - The data clip minimum; all values <= cmin are treated
-                identically. If None (the default), `data.min ()` is used.
+                identically. If None (the default), `data.min()` is used.
     `cmax`    - The data clip maximum; all values >= cmax are treated
-                identically. If None (the default), `data.max ()` is used.
+                identically. If None (the default), `data.max()` is used.
     `stretch` - The stretch function name; 'linear', 'sqrt', or 'square'; see
                 the Stretcher class.
     `cmap`    - The color map name; defaults to 'black_to_blue'. See the
                 `pwkit.colormaps` module for more choices.
 
     Returns a Numpy array of the same shape as `data` with dtype `np.uint32`,
     which represents the ARGB32 colorized version of the data. If your
     colormap is restricted to a single R or G or B channel, you can make color
     images by bitwise-or'ing together different such arrays.
 
     """
     # This could be more efficient, but whatever. This lets us share code with
     # the ndshow module.
 
-    clipper = Clipper ()
-    clipper.alloc_buffer (data)
-    clipper.set_tile_size ()
-    clipper.dmin = cmin if cmin is not None else data.min ()
-    clipper.dmax = cmax if cmax is not None else data.max ()
-    clipper.ensure_all_updated (data)
-
-    stretcher = Stretcher (stretch)
-    stretcher.alloc_buffer (clipper.buffer)
-    stretcher.set_tile_size ()
-    stretcher.ensure_all_updated (clipper.buffer)
-
-    mapper = ColorMapper (cmap)
-    mapper.alloc_buffer (stretcher.buffer)
-    mapper.set_tile_size ()
-    mapper.ensure_all_updated (stretcher.buffer)
+    clipper = Clipper()
+    clipper.alloc_buffer(data)
+    clipper.set_tile_size()
+    clipper.dmin = cmin if cmin is not None else data.min()
+    clipper.dmax = cmax if cmax is not None else data.max()
+    clipper.ensure_all_updated(data)
+
+    stretcher = Stretcher(stretch)
+    stretcher.alloc_buffer(clipper.buffer)
+    stretcher.set_tile_size()
+    stretcher.ensure_all_updated(clipper.buffer)
+
+    mapper = ColorMapper(cmap)
+    mapper.alloc_buffer(stretcher.buffer)
+    mapper.set_tile_size()
+    mapper.ensure_all_updated(stretcher.buffer)
 
     return mapper.buffer
 
 
-def data_to_imagesurface (data, **kwargs):
+def data_to_imagesurface(data, **kwargs):
     """Turn arbitrary data values into a Cairo ImageSurface.
 
     The method and arguments are the same as data_to_argb32, except that the
     data array will be treated as 2D, and higher dimensionalities are not
     allowed. The return value is a Cairo ImageSurface object.
 
     Combined with the write_to_png() method on ImageSurfaces, this is an easy
     way to quickly visualize 2D data.
 
     """
     import cairo
 
-    data = np.atleast_2d (data)
+    data = np.atleast_2d(data)
     if data.ndim != 2:
-        raise ValueError ('input array may not have more than 2 dimensions')
+        raise ValueError('input array may not have more than 2 dimensions')
 
-    argb32 = data_to_argb32 (data, **kwargs)
+    argb32 = data_to_argb32(data, **kwargs)
 
     format = cairo.FORMAT_ARGB32
     height, width = argb32.shape
-    stride = cairo.ImageSurface.format_stride_for_width (format, width)
+    stride = cairo.ImageSurface.format_stride_for_width(format, width)
 
     if argb32.strides[0] != stride:
-        raise ValueError ('stride of data array not compatible with ARGB32')
+        raise ValueError('stride of data array not compatible with ARGB32')
 
-    return cairo.ImageSurface.create_for_data (argb32, format,
-                                               width, height, stride)
+    return cairo.ImageSurface.create_for_data(argb32, format,
+                                              width, height, stride)
```

### Comparing `pwkit-0.8.9/pwkit/slurp.py` & `pwkit-1.0.0/pwkit/slurp.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/colormaps.py` & `pwkit-1.0.0/pwkit/colormaps.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/astutil.py` & `pwkit-1.0.0/pwkit/astutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -738,14 +738,64 @@
     cache_dir = os.path.join(paths.get_cache_dir(), 'pwkit')
     loader = Loader(cache_dir)
     planets = loader('de421.bsp')
     ts = loader.timescale()
     return planets, ts
 
 
+# Hack to implement epochs-of-position. For what it's worth, Skyfield is
+# MIT-licensed like us.
+
+try:
+    from skyfield.api import Star, T0
+except ImportError:
+    def PromoEpochStar(**kwargs):
+        raise NotImplementedError('the "skyfield" package is required for this functionality')
+else:
+    class PromoEpochStar(Star):
+        """A customized version of the Skyfield Star class that accepts a new
+        epoch-of-position parameter.
+
+        Derived from the Skyfield source as of commit 49c2467b (2018 Mar 28).
+
+        """
+        def __init__(self, jd_of_position=T0, **kwargs):
+            super(PromoEpochStar, self).__init__(**kwargs)
+            self.jd_of_position = jd_of_position
+
+        def __repr__(self):
+            opts = []
+            for name in 'ra_mas_per_year dec_mas_per_year parallax_mas radial_km_per_s jd_of_position names'.split():
+                value = getattr(self, name)
+                if value:
+                    opts.append(', {0}={1!r}'.format(name, value))
+            return 'PromoEpochStar(ra_hours={0!r}, dec_degrees={1!r}{2})'.format(
+                self.ra.hours, self.dec.degrees, ''.join(opts))
+
+        def _observe_from_bcrs(self, observer):
+            from numpy import outer
+            from skyfield.constants import C_AUDAY
+            from skyfield.functions import length_of
+            from skyfield.relativity import light_time_difference
+
+            position, velocity = self._position_au, self._velocity_au_per_d
+            t = observer.t
+            dt = light_time_difference(position, observer.position.au)
+            if t.shape:
+                position = (outer(velocity, t.tdb + dt - self.jd_of_position).T + position).T
+            else:
+                position = position + velocity * (t.tdb + dt - self.jd_of_position)
+            vector = position - observer.position.au
+            distance = length_of(vector)
+            light_time = distance / C_AUDAY
+            return vector, (observer.velocity.au_per_d.T - velocity).T, light_time
+
+    del Star, T0
+
+
 _vizurl = 'http://vizier.u-strasbg.fr/viz-bin/asu-tsv'
 
 def get_2mass_epoch (tmra, tmdec, debug=False):
     """Given a 2MASS position, look up the epoch when it was observed.
 
     This function uses the CDS Vizier web service to look up information in
     the 2MASS point source database. Arguments are:
@@ -975,14 +1025,18 @@
             # Based on experience with PM, this may be possible
             if complain:
                 print_ ('AstrometryInfo: swapped positional uncertainty '
                         'major/minor axes', file=sys.stderr)
             self.pos_u_maj, self.pos_u_min = self.pos_u_min, self.pos_u_maj
             self.pos_u_pa += 0.5 * np.pi
 
+        if self.pos_epoch is None:
+            if complain:
+                print_('AstrometryInfo: assuming epoch of position is J2000.0', file=sys.stderr)
+
         if self.promo_ra is None:
             if complain:
                 print_ ('AstrometryInfo: assuming zero proper motion', file=sys.stderr)
         elif self.promo_u_maj is None:
             if complain:
                 print_ ('AstrometryInfo: no uncertainty on proper motion', file=sys.stderr)
         elif self.promo_u_maj < self.promo_u_min:
@@ -1022,48 +1076,41 @@
 
         If *complain* is True, print out warnings for incomplete information.
 
         This function relies on the external :mod:`skyfield` package.
 
         """
         import sys
-        from skyfield.api import Star
 
-        self.verify (complain=complain)
+        self.verify(complain=complain)
 
         planets, ts = load_skyfield_data() # might download stuff from the internet
         earth = planets['earth']
         t = ts.tdb(jd = mjd + 2400000.5)
 
         # "Best" position. The implementation here is a bit weird to keep
         # parallelism with predict().
 
         args = {
             'ra_hours': self.ra * R2H,
             'dec_degrees': self.dec * R2D,
         }
 
-        if self.pos_epoch is not None and self.pos_epoch != 51544.5:
-            print_ ('AstrometryInfo.predict_without_uncertainties(): '
-                    'ignoring epoch of position!', file=sys.stderr)
-            ### o.promoepoch = self.pos_epoch + 2400000.5
-        ###else:
-        ###    if complain:
-        ###        print_ ('AstrometryInfo.predict(): assuming epoch of position is J2000.0', file=sys.stderr)
-        ###    o.promoepoch = 2451545.0 # J2000.0
+        if self.pos_epoch is not None:
+            args['jd_of_position'] = self.pos_epoch + 2400000.5
 
         if self.promo_ra is not None:
             args['ra_mas_per_year'] = self.promo_ra
             args['dec_mas_per_year'] = self.promo_dec
         if self.parallax is not None:
             args['parallax_mas'] = self.parallax
         if self.vradial is not None:
             args['radial_km_per_s'] = self.vradial
 
-        bestra, bestdec, _ = earth.at(t).observe(Star(**args)).radec()
+        bestra, bestdec, _ = earth.at(t).observe(PromoEpochStar(**args)).radec()
         return bestra.radians, bestdec.radians
 
 
     def predict (self, mjd, complain=True, n=20000):
         """Predict the object position at a given MJD.
 
         The return value is a tuple ``(ra, dec, major, minor, pa)``, all in
@@ -1075,15 +1122,14 @@
         The uncertainty ellipse parameters are sigmas, not FWHM. These may be
         converted with the :data:`S2F` constant.
 
         This function relies on the external :mod:`skyfield` package.
 
         """
         import sys
-        from skyfield.api import Star
         from . import ellipses
 
         self.verify (complain=complain)
 
         planets, ts = load_skyfield_data() # might download stuff from the internet
         earth = planets['earth']
         t = ts.tdb(jd = mjd + 2400000.5)
@@ -1091,31 +1137,26 @@
         # "Best" position.
 
         args = {
             'ra_hours': self.ra * R2H,
             'dec_degrees': self.dec * R2D,
         }
 
-        if self.pos_epoch is not None and self.pos_epoch != 51544.5:
-            print_ ('AstrometryInfo.predict(): ignoring epoch of position!', file=sys.stderr)
-            ### o.promoepoch = self.pos_epoch + 2400000.5
-        ###else:
-        ###    if complain:
-        ###        print_ ('AstrometryInfo.predict(): assuming epoch of position is J2000.0', file=sys.stderr)
-        ###    o.promoepoch = 2451545.0 # J2000.0
+        if self.pos_epoch is not None:
+            args['jd_of_position'] = self.pos_epoch + 2400000.5
 
         if self.promo_ra is not None:
             args['ra_mas_per_year'] = self.promo_ra
             args['dec_mas_per_year'] = self.promo_dec
         if self.parallax is not None:
             args['parallax_mas'] = self.parallax
         if self.vradial is not None:
             args['radial_km_per_s'] = self.vradial
 
-        bestra, bestdec, _ = earth.at(t).observe(Star(**args)).radec()
+        bestra, bestdec, _ = earth.at(t).observe(PromoEpochStar(**args)).radec()
         bestra = bestra.radians
         bestdec = bestdec.radians
 
         # Monte Carlo to get an uncertainty. As always, astronomy position
         # angle convention requires that we treat declination as X and RA as
         # Y. First, we check sanity and generate randomized parameters:
 
@@ -1163,15 +1204,15 @@
         for i in range (n):
             args['ra_hours'] = ras[i] * R2H
             args['dec_degrees'] = decs[i] * R2D
             args['ra_mas_per_year'] = pmras[i]
             args['dec_mas_per_year'] = pmdecs[i]
             args['parallax_mas'] = parallaxes[i]
             args['radial_km_per_s'] = vradials[i]
-            ara, adec, _ = earth.at(t).observe(Star(**args)).radec()
+            ara, adec, _ = earth.at(t).observe(PromoEpochStar(**args)).radec()
             results[i] = adec.radians, ara.radians
 
         maj, min, pa = ellipses.bivell (*ellipses.databiv (results))
 
         # All done.
 
         return bestra, bestdec, maj, min, pa
```

### Comparing `pwkit-0.8.9/pwkit/tabfile.py` & `pwkit-1.0.0/pwkit/tabfile.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/kwargv.py` & `pwkit-1.0.0/pwkit/kwargv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2012-2015 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2012-2015, 2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """The :mod:`pwkit.kwargv` module provides a framework for parsing
 keyword-style arguments to command-line programs. It’s designed so that you
 can easily make a routine with complex, structured configuration parameters
 that can also be driven from the command line.
 
 Keywords are defined by declaring a subclass of the
 :class:`ParseKeywords` class with fields corresponding to the
 support keywords::
 
   from pwkit.kwargv import ParseKeywords, Custom
 
-  class MyConfig (ParseKeywords):
+  class MyConfig(ParseKeywords):
       foo = 1
       bar = str
       multi = [int]
-      extra = Custom (float, required=True)
+      extra = Custom(float, required=True)
 
-      @Custom (str)
-      def declination (value):
+      @Custom(str)
+      def declination(value):
           from pwkit.astutil import parsedeglat
-          return parsedeglat (value)
+          return parsedeglat(value)
 
 Instantiating the subclass fills in all defaults. Calling the
 :meth:`ParseKeywords.parse` method parses a list of strings (defaulting to
 ``sys.argv[1:]``) and updates the instance’s properties. This framework is
 designed so that you can provide complex configuration to an algorithm either
 programmatically, or on the command line. A typical use would be::
 
   from pwkit.kwargv import ParseKeywords, Custom
 
-  class MyConfig (ParseKeywords):
+  class MyConfig(ParseKeywords):
       niter = 1
       input = str
       scales = [int]
       # ...
 
-  def my_complex_algorithm (cfg):
+  def my_complex_algorithm(cfg):
      from pwkit.io import Path
-     data = Path (cfg.input).read_fits ()
+     data = Path(cfg.input).read_fits()
 
-     for i in range (cfg.niter):
+     for i in range(cfg.niter):
          # ....
 
-  def call_algorithm_in_code ():
-      cfg = MyConfig ()
+  def call_algorithm_in_code():
+      cfg = MyConfig()
       cfg.input = 'testfile.fits'
       # ...
-      my_complex_algorithm (cfg)
+      my_complex_algorithm(cfg)
 
   if __name__ == '__main__':
-      cfg = MyConfig ().parse ()
-      my_complex_algorithm (cfg)
+      cfg = MyConfig().parse()
+      my_complex_algorithm(cfg)
 
 You could then execute the module as a program and specify arguments in the
 form ``./program niter=5 input=otherfile.fits``.
 
 
 Keyword Specification Format
 ----------------------------
@@ -94,67 +94,67 @@
 See the :class:`KeywordInfo` documentation for specification of additional
 keyword properties that may be specified. The ``Custom`` name is simply an
 alias for :class:`KeywordInfo`.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Custom KwargvError ParseError KeywordInfo ParseKeywords basic').split ()
+__all__ = str('Custom KwargvError ParseError KeywordInfo ParseKeywords basic').split()
 
 import six
 from six.moves import range
 from . import Holder, PKError, text_type
 
 
-class KwargvError (PKError):
+class KwargvError(PKError):
     """Raised when invalid arguments have been provided."""
 
 
-class ParseError (KwargvError):
+class ParseError(KwargvError):
     """Raised when the structure of the arguments appears legitimate, but a
     particular value cannot be parsed into its expected type.
 
     """
 
 
-def basic (args=None):
+def basic(args=None):
     """Parse the string list *args* as a set of keyword arguments in a very
     simple-minded way, splitting on equals signs. Returns a
     :class:`pwkit.Holder` instance with attributes set to strings. The form
     ``+foo`` is mapped to setting ``foo = True`` on the :class:`pwkit.Holder`
     instance. If *args* is ``None``, ``sys.argv[1:]`` is used. Raises
     :exc:`KwargvError` on invalid arguments (i.e., ones without an equals sign
     or a leading plus sign).
 
     """
     if args is None:
         import sys
         args = sys.argv[1:]
 
-    parsed = Holder ()
+    parsed = Holder()
 
     for arg in args:
         if arg[0] == '+':
-            for kw in arg[1:].split (','):
-                parsed.set_one (kw, True)
+            for kw in arg[1:].split(','):
+                parsed.set_one(kw, True)
             # avoid analogous -a,b,c syntax because it gets confused with -a --help, etc.
         else:
-            t = arg.split ('=', 1)
-            if len (t) < 2:
-                raise KwargvError ('don\'t know what to do with argument "%s"', arg)
-            if not len (t[1]):
-                raise KwargvError ('empty value for keyword argument "%s"', t[0])
-            parsed.set_one (t[0], t[1])
+            t = arg.split('=', 1)
+            if len(t) < 2:
+                raise KwargvError('don\'t know what to do with argument "%s"', arg)
+            if not len(t[1]):
+                raise KwargvError('empty value for keyword argument "%s"', t[0])
+            parsed.set_one(t[0], t[1])
 
     return parsed
 
 
 # The fancy, full-featured system.
 
-class KeywordInfo (object):
+class KeywordInfo(object):
     """Properties that a keyword argument may have.
 
     """
     parser = None
     """A callable used to convert the argument text to a Python value.
     This attribute is assigned automatically upon setup."""
 
@@ -201,271 +201,279 @@
     """
     _attrname = None
 
     # This isn't used on Keyword*Info* instances, but adding a dummy here makes
     # the docs much saner:
     uiname = None
     """The name of the keyword as parsed from the command-line. For instance,
-    ``some_value = Custom (int, uiname="some-value")`` will result in a
+    ``some_value = Custom(int, uiname="some-value")`` will result in a
     keyword that the user sets by calling ``./program some-value=3``. This
     provides a mechanism to support keyword names that are not legal Python
     identifiers.
 
     """
 
 
-class KeywordOptions (Holder):
+class KeywordOptions(Holder):
     uiname = None
     subval = None
 
-    def __init__ (self, subval, **kwargs):
-        self.set (**kwargs)
+    def __init__(self, subval, **kwargs):
+        self.set(**kwargs)
         self.subval = subval
 
-    def __call__ (self, fixupfunc):
+    def __call__(self, fixupfunc):
         # Slightly black magic. Grayish magic. This lets us be used as
         # a decorator on "fixup" functions to modify or range-check
         # the parsed argument value.
         self.fixupfunc = fixupfunc
         return self
 
 
 Custom = KeywordOptions # sugar for users
 
 
-def _parse_bool (s):
-    s = s.lower ()
+def _parse_bool(s):
+    s = s.lower()
 
-    if s in 'y yes t true on 1'.split ():
+    if s in 'y yes t true on 1'.split():
         return True
-    if s in 'n no f false off 0'.split ():
+    if s in 'n no f false off 0'.split():
         return False
-    raise ParseError ('don\'t know how to interpret "%s" as a boolean' % s)
+    raise ParseError('don\'t know how to interpret "%s" as a boolean' % s)
 
 
-def _val_to_parser (v):
-    if isinstance (v, bool):
+def _val_to_parser(v):
+    if isinstance(v, bool):
         return _parse_bool
-    if isinstance (v, (int, float, text_type)):
+    if isinstance(v, (int, float, text_type)):
         return v.__class__
-    raise ValueError ('can\'t figure out how to parse %r' % v)
+    raise ValueError('can\'t figure out how to parse %r' % v)
 
 
-def _val_or_func_to_parser (v):
+def _val_or_func_to_parser(v):
     if v is bool:
         return _parse_bool
-    if callable (v):
+    if callable(v):
         return v
-    return _val_to_parser (v)
+    return _val_to_parser(v)
 
 
-def _val_or_func_to_default (v):
-    if callable (v):
+def _val_or_func_to_default(v):
+    if callable(v):
         return None
-    if isinstance (v, (int, float, bool, text_type)):
+    if isinstance(v, (int, float, bool, text_type)):
         return v
     raise ValueError
 
     ('can\'t figure out a default for %r' % v)
 
 
-def _handle_flex_list (ki, ks):
-    assert len (ks) == 1
+def _handle_flex_list(ki, ks):
+    assert len(ks) == 1
     elemparser = ks[0]
     # I don't think 'foo = [0]' will be useful ...
-    assert callable (elemparser)
+    assert callable(elemparser)
 
-    def flexlistparse (val):
-        return [elemparser (i) for i in val.split (ki.sep)]
+    def flexlistparse(val):
+        return [elemparser(i) for i in val.split(ki.sep)]
 
     return flexlistparse, []
 
 
-def _handle_fixed_list (ki, ks):
-    parsers = [_val_or_func_to_parser (sks) for sks in ks]
-    defaults = [_val_or_func_to_default (sks) for sks in ks]
-    ntot = len (parsers)
-
-    def fixlistparse (val):
-        items = val.split (ki.sep)
-        ngot = len (items)
+def _handle_fixed_list(ki, ks):
+    parsers = [_val_or_func_to_parser(sks) for sks in ks]
+    defaults = [_val_or_func_to_default(sks) for sks in ks]
+    ntot = len(parsers)
+
+    def fixlistparse(val):
+        items = val.split(ki.sep)
+        ngot = len(items)
 
         if ngot < ki.minvals:
             if ki.minvals == ntot:
-                raise ParseError ('expected exactly %d values, but only got %d',
-                                  ntot, ngot)
-            raise ParseError ('expected between %d and %d values, but only got %d',
-                              ki.minvals, ntot, ngot)
+                raise ParseError('expected exactly %d values, but only got %d',
+                                 ntot, ngot)
+            raise ParseError('expected between %d and %d values, but only got %d',
+                             ki.minvals, ntot, ngot)
         if ngot > ntot:
-            raise ParseError ('expected between %d and %d values, but got %d',
-                              ki.minvals, ntot, ngot)
+            raise ParseError('expected between %d and %d values, but got %d',
+                             ki.minvals, ntot, ngot)
 
-        result = list (defaults) # make a copy
-        for i in range (ngot):
-            result[i] = parsers[i] (items[i])
+        result = list(defaults) # make a copy
+        for i in range(ngot):
+            result[i] = parsers[i](items[i])
         return result
 
-    return fixlistparse, list (defaults) # make a copy
+    return fixlistparse, list(defaults) # make a copy
 
 
-class ParseKeywords (Holder):
+class ParseKeywords(Holder):
     """The template class for defining your keyword arguments. A subclass of
     :class:`pwkit.Holder`. Declare attributes in a subclass following the
     scheme described above, then call the :meth:`ParseKeywords.parse` method.
 
     """
-    def __init__ (self):
+    def __init__(self):
         kwspecs = self.__class__.__dict__
         kwinfos = {}
 
         # Process our keywords, as specified by the class attributes, into a
         # form more friendly for parsing, and check for things we don't
         # understand. 'kw' is the keyword name exposed to the user; 'attrname'
         # is the name of the attribute to set on the resulting object.
 
-        for kw, ks in six.iteritems (kwspecs):
+        for kw, ks in six.iteritems(kwspecs):
             if kw[0] == '_':
                 continue
 
-            ki = KeywordInfo ()
+            ki = KeywordInfo()
             ko = None
             attrname = kw
 
-            if isinstance (ks, KeywordOptions):
+            if isinstance(ks, KeywordOptions):
                 ko = ks
                 ks = ko.subval
 
                 if ko.uiname is not None:
                     kw = ko.uiname
 
-            if callable (ks):
+            if callable(ks):
                 # expected to be a type (int, float, ...).
                 # This branch would get taken for methods, too,
                 # which sorta makes sense?
-                parser = _val_or_func_to_parser (ks)
-                default = _val_or_func_to_default (ks)
-            elif isinstance (ks, list) and len (ks) == 1:
-                parser, default = _handle_flex_list (ki, ks)
-            elif isinstance (ks, list) and len (ks) > 1:
-                parser, default = _handle_fixed_list (ki, ks)
+                parser = _val_or_func_to_parser(ks)
+                default = _val_or_func_to_default(ks)
+            elif isinstance(ks, list) and len(ks) == 1:
+                parser, default = _handle_flex_list(ki, ks)
+            elif isinstance(ks, list) and len(ks) > 1:
+                parser, default = _handle_fixed_list(ki, ks)
             else:
-                parser = _val_to_parser (ks)
-                default = _val_or_func_to_default (ks)
+                parser = _val_to_parser(ks)
+                default = _val_or_func_to_default(ks)
 
             ki._attrname = attrname
             ki.parser = parser
             ki.default = default
 
             if ko is not None: # override with user-specified options
-                ki.__dict__.update (ko.__dict__)
+                ki.__dict__.update(ko.__dict__)
 
             if ki.required:
                 # makes sense, and prevents trying to call fixupfunc on
                 # weird default values of fixed lists.
                 ki.default = None
             elif ki.repeatable:
                 ki.default = []
             elif ki.fixupfunc is not None and ki.default is not None:
                 # kinda gross structure here, oh well.
-                ki.default = ki.fixupfunc (ki.default)
+                ki.default = ki.fixupfunc(ki.default)
 
             kwinfos[kw] = ki
 
         # Apply defaults, save parse info, done
 
-        for kw, ki in six.iteritems (kwinfos):
-            self.set_one (ki._attrname, ki.default)
+        for kw, ki in six.iteritems(kwinfos):
+            self.set_one(ki._attrname, ki.default)
 
         self._kwinfos = kwinfos
 
 
-    def parse (self, args=None):
+    def parse(self, args=None):
         """Parse textual keywords as described by this class’s attributes, and update
         this instance’s attributes with the parsed values. *args* is a list of
         strings; if ``None``, it defaults to ``sys.argv[1:]``. Returns *self*
         for convenience. Raises :exc:`KwargvError` if invalid keywords are
         encountered.
 
         See also :meth:`ParseKeywords.parse_or_die`.
 
         """
         if args is None:
             import sys
             args = sys.argv[1:]
 
-        seen = set ()
+        seen = set()
 
         for arg in args:
-            t = arg.split ('=', 1)
-            if len (t) < 2:
-                raise KwargvError ('don\'t know what to do with argument "%s"', arg)
+            t = arg.split('=', 1)
+            if len(t) < 2:
+                raise KwargvError('don\'t know what to do with argument "%s"', arg)
 
             kw, val = t
-            ki = self._kwinfos.get (kw)
+            ki = self._kwinfos.get(kw)
 
             if ki is None:
-                raise KwargvError ('unrecognized keyword argument "%s"', kw)
+                raise KwargvError('unrecognized keyword argument "%s"', kw)
 
-            if not len (val):
-                raise KwargvError ('empty value for keyword argument "%s"', kw)
+            if not len(val):
+                raise KwargvError('empty value for keyword argument "%s"', kw)
 
             try:
-                pval = ki.parser (val)
+                pval = ki.parser(val)
             except ParseError as e :
-                raise KwargvError ('cannot parse value "%s" for keyword '
-                                   'argument "%s": %s', val, kw, e)
+                raise KwargvError('cannot parse value "%s" for keyword '
+                                  'argument "%s": %s', val, kw, e)
             except Exception as e:
                 if ki.printexc:
-                    raise KwargvError ('cannot parse value "%s" for keyword '
-                                       'argument "%s": %s', val, kw, e)
-                raise KwargvError ('cannot parse value "%s" for keyword '
-                                   'argument "%s"', val, kw)
-
-            if ki.maxvals is not None and len (pval) > ki.maxvals:
-                raise KwargvError ('keyword argument "%s" may have at most %d'
-                                   ' values, but got %s ("%s")', kw,
-                                   ki.maxvals, len (pval), val)
+                    raise KwargvError('cannot parse value "%s" for keyword '
+                                      'argument "%s": %s', val, kw, e)
+                raise KwargvError('cannot parse value "%s" for keyword '
+                                  'argument "%s"', val, kw)
+
+            if ki.maxvals is not None and len(pval) > ki.maxvals:
+                raise KwargvError('keyword argument "%s" may have at most %d'
+                                  ' values, but got %s ("%s")', kw,
+                                  ki.maxvals, len(pval), val)
 
             if ki.scale is not None:
                 pval = pval * ki.scale
 
             if ki.fixupfunc is not None:
-                pval = ki.fixupfunc (pval)
+                pval = ki.fixupfunc(pval)
 
             if ki.repeatable:
                 # We can't just unilaterally append to the preexisting
                 # list, since if we did that starting with the default value
                 # we'd mutate the default list.
-                cur = self.get (ki._attrname)
-                if not len (cur):
+                cur = self.get(ki._attrname)
+                if not len(cur):
                     pval = [pval]
                 else:
-                    cur.append (pval)
+                    cur.append(pval)
                     pval = cur
 
-            seen.add (kw)
-            self.set_one (ki._attrname, pval)
+            seen.add(kw)
+            self.set_one(ki._attrname, pval)
 
-        for kw, ki in six.iteritems (self._kwinfos):
-            if ki.required and kw not in seen:
-                raise KwargvError ('required keyword argument "%s" was not '
-                                   'provided', kw)
+        for kw, ki in six.iteritems(self._kwinfos):
+            if kw not in seen:
+                if ki.required:
+                    raise KwargvError('required keyword argument "%s" was not provided', kw)
+
+                # If there's a fixup, process it even if the keyword wasn't
+                # provided. This lets code use "interesting" defaults with
+                # types that you might prefer to use when launching a task
+                # programmatically; e.g. a default output stream that is
+                # `sys.stdout`, not "-".
+                if ki.fixupfunc is not None:
+                    self.set_one(ki._attrname, ki.fixupfunc(None))
 
         return self # convenience
 
 
-    def parse_or_die (self, args=None):
+    def parse_or_die(self, args=None):
         """Like :meth:`ParseKeywords.parse`, but calls :func:`pkwit.cli.die` if a
         :exc:`KwargvError` is raised, printing the exception text. Returns
         *self* for convenience.
 
         """
         from .cli import die
 
         try:
-            return self.parse (args)
+            return self.parse(args)
         except KwargvError as e:
-            die (e)
+            die(e)
 
 
 if __name__ == '__main__':
-    print (basic ())
+    print(basic())
```

### Comparing `pwkit-0.8.9/pwkit/ndshow_gtk3.py` & `pwkit-1.0.0/pwkit/ndshow_gtk3.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,244 +44,243 @@
 
 """
 
 # TODO: very redundant with ndshow_gtk2, of course!
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Cycler Viewer Viewport cycle view').split ()
+__all__ = str('Cycler Viewer Viewport cycle view').split()
 
 import sys, time
 from six.moves import range
 import numpy as np
 import cairo
 # There is a gi.repository.cairo but it barely exposes any API, and it seems
 # like you're not really supposed to use it.
 import gi
-gi.require_version ('Gdk', '3.0')
-gi.require_version ('Gtk', '3.0')
+gi.require_version('Gdk', '3.0')
+gi.require_version('Gtk', '3.0')
 from gi.repository import GLib, GObject, Gdk, Gtk
 
 from . import PKError
 from .data_gui_helpers import Clipper, ColorMapper
 
 
 DRAG_TYPE_NONE = 0
 DRAG_TYPE_PAN = 1
 DRAG_TYPE_TUNER = 2
 
 DEFAULT_WIN_WIDTH = 800
 DEFAULT_WIN_HEIGHT = 600
 
 
-class Viewport (Gtk.DrawingArea):
+class Viewport(Gtk.DrawingArea):
     __gtype_name__ = 'Viewport'
 
-    bgpattern = GObject.Property (type=GObject.TYPE_PYOBJECT)
-    getshape = GObject.Property (type=GObject.TYPE_PYOBJECT)
-    settuning = GObject.Property (type=GObject.TYPE_PYOBJECT)
-    getsurface = GObject.Property (type=GObject.TYPE_PYOBJECT)
-    onmotion = GObject.Property (type=GObject.TYPE_PYOBJECT)
-    drawoverlay = GObject.Property (type=GObject.TYPE_PYOBJECT)
+    bgpattern = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    getshape = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    settuning = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    getsurface = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    onmotion = GObject.Property(type=GObject.TYPE_PYOBJECT)
+    drawoverlay = GObject.Property(type=GObject.TYPE_PYOBJECT)
 
-    centerx = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
-    centery = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
+    centerx = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
+    centery = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
     # The data pixel coordinate of the central pixel of the displayed window.
 
-    scale = GObject.Property (type=GObject.TYPE_FLOAT, default=-1.)
+    scale = GObject.Property(type=GObject.TYPE_FLOAT, default=-1.)
     # From data space to viewer space: e.g., scale = 2 means that each data
     # pixel occupies 2 pixels on-screen.
 
-    needtune = GObject.Property (type=GObject.TYPE_BOOLEAN, default=True)
-    tunerx = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
-    tunery = GObject.Property (type=GObject.TYPE_FLOAT, default=1.)
-    tunerscale = GObject.Property (type=GObject.TYPE_FLOAT, default=200.)
-
-    drag_type = GObject.Property (type=GObject.TYPE_INT, default=DRAG_TYPE_NONE)
-    drag_win_x0 = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
-    drag_win_y0 = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
-    drag_dc_x0 = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
-    drag_dc_y0 = GObject.Property (type=GObject.TYPE_FLOAT, default=0.)
-
-    def __init__ (self):
-        super (Viewport, self).__init__ ()
-        self.add_events (Gdk.EventMask.POINTER_MOTION_MASK |
-                         Gdk.EventMask.BUTTON_PRESS_MASK |
-                         Gdk.EventMask.BUTTON_RELEASE_MASK |
-                         Gdk.EventMask.SCROLL_MASK)
-        self.connect ('draw', self._on_draw)
-        self.connect ('scroll-event', self._on_scroll)
-        self.connect ('button-press-event', self._on_button_press)
-        self.connect ('button-release-event', self._on_button_release)
-        self.connect ('motion-notify-event', self._on_motion_notify)
-
-        self.bgpattern = cairo.SolidPattern (0.1, 0.1, 0.1)
-
-
-    def set_shape_getter (self, getshape):
-        if getshape is not None and not callable (getshape):
-            raise ValueError ()
+    needtune = GObject.Property(type=GObject.TYPE_BOOLEAN, default=True)
+    tunerx = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
+    tunery = GObject.Property(type=GObject.TYPE_FLOAT, default=1.)
+    tunerscale = GObject.Property(type=GObject.TYPE_FLOAT, default=200.)
+
+    drag_type = GObject.Property(type=GObject.TYPE_INT, default=DRAG_TYPE_NONE)
+    drag_win_x0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
+    drag_win_y0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
+    drag_dc_x0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
+    drag_dc_y0 = GObject.Property(type=GObject.TYPE_FLOAT, default=0.)
+
+    def __init__(self):
+        super(Viewport, self).__init__()
+        self.add_events(Gdk.EventMask.POINTER_MOTION_MASK |
+                        Gdk.EventMask.BUTTON_PRESS_MASK |
+                        Gdk.EventMask.BUTTON_RELEASE_MASK |
+                        Gdk.EventMask.SCROLL_MASK)
+        self.connect('draw', self._on_draw)
+        self.connect('scroll-event', self._on_scroll)
+        self.connect('button-press-event', self._on_button_press)
+        self.connect('button-release-event', self._on_button_release)
+        self.connect('motion-notify-event', self._on_motion_notify)
+
+        self.bgpattern = cairo.SolidPattern(0.1, 0.1, 0.1)
+
+
+    def set_shape_getter(self, getshape):
+        if getshape is not None and not callable(getshape):
+            raise ValueError()
         self.getshape = getshape
         return self
 
 
-    def set_tuning_setter (self, settuning):
-        if settuning is not None and not callable (settuning):
-            raise ValueError ()
+    def set_tuning_setter(self, settuning):
+        if settuning is not None and not callable(settuning):
+            raise ValueError()
         self.settuning = settuning
         self.needtune = True
         return self
 
 
-    def set_surface_getter (self, getsurface):
-        if getsurface is not None and not callable (getsurface):
-            raise ValueError ()
+    def set_surface_getter(self, getsurface):
+        if getsurface is not None and not callable(getsurface):
+            raise ValueError()
         self.getsurface = getsurface
         return self
 
 
-    def set_motion_handler (self, onmotion):
-        if onmotion is not None and not callable (onmotion):
-            raise ValueError ()
+    def set_motion_handler(self, onmotion):
+        if onmotion is not None and not callable(onmotion):
+            raise ValueError()
         self.onmotion = onmotion
         return self
 
 
-    def set_overlay_drawer (self, drawoverlay):
-        if drawoverlay is not None and not callable (drawoverlay):
-            raise ValueError ()
+    def set_overlay_drawer(self, drawoverlay):
+        if drawoverlay is not None and not callable(drawoverlay):
+            raise ValueError()
         self.drawoverlay = drawoverlay
         return self
 
 
-    def autoscale (self):
+    def autoscale(self):
         if self.getshape is None:
-            raise PKError ('must be called after setting shape-getter')
+            raise PKError('must be called after setting shape-getter')
 
-        aw = self.get_allocated_width ()
-        ah = self.get_allocated_height ()
+        aw = self.get_allocated_width()
+        ah = self.get_allocated_height()
 
-        dw, dh = self.getshape ()
+        dw, dh = self.getshape()
 
-        wratio = float (aw) / dw
-        hratio = float (ah) / dh
+        wratio = float(aw) / dw
+        hratio = float(ah) / dh
 
-        self.scale = min (wratio, hratio)
+        self.scale = min(wratio, hratio)
         self.centerx = 0.5 * (dw - 1)
         self.centery = 0.5 * (dh - 1)
-        self.queue_draw ()
+        self.queue_draw()
         return self
 
 
-    def center (self):
+    def center(self):
         if self.getshape is None:
-            raise PKError ('must be called after setting shape-getter')
+            raise PKError('must be called after setting shape-getter')
 
-        dw, dh = self.getshape ()
+        dw, dh = self.getshape()
         self.centerx = 0.5 * (dw - 1)
         self.centery = 0.5 * (dh - 1)
-        self.queue_draw ()
+        self.queue_draw()
         return self
 
 
-    def write_data_as_png (self, filename):
+    def write_data_as_png(self, filename):
         if self.getshape is None:
-            raise PKError ('must be called after setting shape-getter')
+            raise PKError('must be called after setting shape-getter')
         if self.getsurface is None:
-            raise PKError ('must be called after setting surface-getter')
+            raise PKError('must be called after setting surface-getter')
 
         if self.needtune:
-            self.settuning (self.tunerx, self.tunery)
+            self.settuning(self.tunerx, self.tunery)
             self.needtune = False
 
-        dw, dh = self.getshape ()
-        surface, xoffset, yoffset = self.getsurface (0, 0, dw, dh)
-        surface.write_to_png (filename)
+        dw, dh = self.getshape()
+        surface, xoffset, yoffset = self.getsurface(0, 0, dw, dh)
+        surface.write_to_png(filename)
 
 
-    def write_view_as_png (self, filename):
+    def write_view_as_png(self, filename):
         if self.getshape is None:
-            raise PKError ('must be called after setting shape-getter')
+            raise PKError('must be called after setting shape-getter')
         if self.getsurface is None:
-            raise PKError ('must be called after setting surface-getter')
+            raise PKError('must be called after setting surface-getter')
 
-        width = self.get_allocated_width ()
-        height = self.get_allocated_height ()
+        width = self.get_allocated_width()
+        height = self.get_allocated_height()
 
-        stride = cairo.ImageSurface.format_stride_for_width (cairo.FORMAT_ARGB32,
-                                                             width)
+        stride = cairo.ImageSurface.format_stride_for_width(cairo.FORMAT_ARGB32,
+                                                            width)
         assert stride % 4 == 0 # stride is in bytes
-        viewdata = np.empty ((height, stride // 4), dtype=np.uint32)
-        viewsurface = cairo.ImageSurface.create_for_data (viewdata, cairo.FORMAT_ARGB32,
-                                                          width, height, stride)
-        ctxt = cairo.Context (viewsurface)
-        self._draw_in_context (ctxt, width, height)
-        viewsurface.write_to_png (filename)
+        viewdata = np.empty((height, stride // 4), dtype=np.uint32)
+        viewsurface = cairo.ImageSurface.create_for_data(viewdata, cairo.FORMAT_ARGB32,
+                                                         width, height, stride)
+        ctxt = cairo.Context(viewsurface)
+        self._draw_in_context(ctxt, width, height)
+        viewsurface.write_to_png(filename)
 
 
-    def get_pointer_data_coords (self):
+    def get_pointer_data_coords(self):
         if self.scale < 0.:
-            self.autoscale ()
+            self.autoscale()
 
-        x, y = self.get_pointer ()
-        dx = x - 0.5 * self.get_allocated_width ()
-        dy = y - 0.5 * self.get_allocated_height ()
+        x, y = self.get_pointer()
+        dx = x - 0.5 * self.get_allocated_width()
+        dy = y - 0.5 * self.get_allocated_height()
         datax = self.centerx + dx / self.scale
         datay = self.centery + dy / self.scale
         return datax, datay
 
 
-    def _on_draw (self, widget, ctxt):
+    def _on_draw(self, widget, ctxt):
         if self.getshape is None or self.getsurface is None:
             return False
 
-        width = self.get_allocated_width ()
-        height = self.get_allocated_height ()
+        width = self.get_allocated_width()
+        height = self.get_allocated_height()
 
         if self.getshape is None or self.getsurface is None:
-            raise PKError ('must be called after setting shape-getter '
-                           'and surface-getter')
+            raise PKError('must be called after setting shape-getter '
+                          'and surface-getter')
 
         if self.scale < 0.:
-            self.autoscale ()
+            self.autoscale()
         if self.needtune:
-            self.settuning (self.tunerx, self.tunery)
+            self.settuning(self.tunerx, self.tunery)
             self.needtune = False
 
         # Our data coordinates have integral pixel values being in the
         # centers of pixels; Cairo uses edges. That's the origin of the
         # minus one.
         seendatawidth = width / self.scale
         xoffset = 0.5 * (seendatawidth - 1) - self.centerx
         seendataheight = height / self.scale
         yoffset = 0.5 * (seendataheight - 1) - self.centery
 
-        surface, xoffset, yoffset = self.getsurface (xoffset, yoffset,
-                                                     seendatawidth, seendataheight)
+        surface, xoffset, yoffset = self.getsurface(xoffset, yoffset,
+                                                    seendatawidth, seendataheight)
 
-        ctxt.save ()
-        ctxt.set_source (self.bgpattern)
-        ctxt.paint ()
-        ctxt.scale (self.scale, self.scale)
-        ctxt.set_source_surface (surface, xoffset, yoffset)
-        pat = ctxt.get_source ()
-        pat.set_extend (cairo.EXTEND_NONE)
-        pat.set_filter (cairo.FILTER_NEAREST)
-        ctxt.paint ()
-        ctxt.restore ()
+        ctxt.save()
+        ctxt.set_source(self.bgpattern)
+        ctxt.paint()
+        ctxt.scale(self.scale, self.scale)
+        ctxt.set_source_surface(surface, xoffset, yoffset)
+        pat = ctxt.get_source()
+        pat.set_extend(cairo.EXTEND_NONE)
+        pat.set_filter(cairo.FILTER_NEAREST)
+        ctxt.paint()
+        ctxt.restore()
 
         if self.drawoverlay is not None:
-            self.drawoverlay (ctxt, width, height,
-                              -xoffset, -yoffset, self.scale)
+            self.drawoverlay(ctxt, width, height, -xoffset, -yoffset, self.scale)
 
         return False
 
 
-    def _on_scroll (self, alsoself, event):
-        modmask = Gtk.accelerator_get_default_mod_mask ()
+    def _on_scroll(self, alsoself, event):
+        modmask = Gtk.accelerator_get_default_mod_mask()
 
         if (event.state & modmask) in (0, Gdk.ModifierType.CONTROL_MASK):
             oldscale = self.scale
             newscale = self.scale
 
             if event.state & modmask == Gdk.ModifierType.CONTROL_MASK:
                 factor = 1.2
@@ -294,15 +293,15 @@
             if event.direction == Gdk.ScrollDirection.DOWN:
                 newscale /= factor
 
             if newscale == oldscale:
                 return False
 
             self.scale = newscale
-            self.queue_draw ()
+            self.queue_draw()
             return True
 
         if (event.state & modmask) == Gdk.ModifierType.SHIFT_MASK:
             oldscale = self.tunerscale
             newscale = self.tunerscale
 
             if event.direction == Gdk.ScrollDirection.UP:
@@ -316,19 +315,19 @@
 
             self.tunerscale = newscale
             return True
 
         return False
 
 
-    def _on_button_press (self, alsoself, event):
-        modmask = Gtk.accelerator_get_default_mod_mask ()
+    def _on_button_press(self, alsoself, event):
+        modmask = Gtk.accelerator_get_default_mod_mask()
 
         if event.type == Gdk.EventType.BUTTON_PRESS and event.button == 1:
-            self.grab_add ()
+            self.grab_add()
             self.drag_win_x0 = event.x
             self.drag_win_y0 = event.y
 
             if (event.state & modmask) == 0:
                 self.drag_type = DRAG_TYPE_PAN
                 self.drag_dc_x0 = self.centerx
                 self.drag_dc_y0 = self.centery
@@ -339,43 +338,43 @@
                 self.drag_dc_x0 = self.tunerx
                 self.drag_dc_y0 = self.tunery
                 return True
 
             return False
 
         if event.type == Gdk.EventType._2BUTTON_PRESS and event.button == 1:
-            dx = event.x - 0.5 * self.get_allocated_width ()
-            dy = event.y - 0.5 * self.get_allocated_height ()
+            dx = event.x - 0.5 * self.get_allocated_width()
+            dy = event.y - 0.5 * self.get_allocated_height()
 
             if (event.state & modmask) == 0:
                 self.centerx += dx / self.scale
                 self.centery += dy / self.scale
             elif (event.state & modmask) == Gdk.ModifierType.SHIFT_MASK:
                 self.tunerx += dx / self.tunerscale
                 self.tunery += dy / self.tunerscale
                 self.needtune = True
             else:
                 return False
 
-            self.queue_draw ()
+            self.queue_draw()
             # Prevent the drag-release code from running. (Double-click events
             # are preceded by single-click events.)
-            self.grab_remove ()
+            self.grab_remove()
             self.drag_type = DRAG_TYPE_NONE
             return True
 
         return False
 
 
-    def _on_button_release (self, alsoself, event):
+    def _on_button_release(self, alsoself, event):
         if event.type == Gdk.EventType.BUTTON_RELEASE and event.button == 1:
             if self.drag_type == DRAG_TYPE_NONE:
                 return False
 
-            self.grab_remove ()
+            self.grab_remove()
             dx = self.drag_win_x0 - event.x
             dy = self.drag_win_y0 - event.y
 
             if self.drag_type == DRAG_TYPE_PAN:
                 self.centerx = self.drag_dc_x0 + dx / self.scale
                 self.centery = self.drag_dc_y0 + dy / self.scale
             elif self.drag_type == DRAG_TYPE_TUNER:
@@ -384,126 +383,126 @@
                 self.needtune = True
             else:
                 return False
 
             self.drag_win_x0 = self.drag_win_y0 = 0.
             self.drag_dc_x0 = self.drag_dc_y0 = 0.
             self.drag_type = DRAG_TYPE_NONE
-            self.queue_draw ()
+            self.queue_draw()
             return True
 
         return False
 
-    def _on_motion_notify (self, alsoself, event):
+    def _on_motion_notify(self, alsoself, event):
         if self.onmotion is not None:
-            dx = event.x - 0.5 * self.get_allocated_width ()
-            dy = event.y - 0.5 * self.get_allocated_height ()
+            dx = event.x - 0.5 * self.get_allocated_width()
+            dy = event.y - 0.5 * self.get_allocated_height()
             datax = self.centerx + dx / self.scale
             datay = self.centery + dy / self.scale
-            self.onmotion (datax, datay)
+            self.onmotion(datax, datay)
 
         if self.drag_type == DRAG_TYPE_NONE:
             return False
         elif self.drag_type == DRAG_TYPE_PAN:
             self.centerx = self.drag_dc_x0 + (self.drag_win_x0 - event.x) / self.scale
             self.centery = self.drag_dc_y0 + (self.drag_win_y0 - event.y) / self.scale
         elif self.drag_type == DRAG_TYPE_TUNER:
             self.tunerx = self.drag_dc_x0 + (event.x - self.drag_win_x0) / self.tunerscale
             self.tunery = self.drag_dc_y0 + (event.y - self.drag_win_y0) / self.tunerscale
             self.needtune = True
 
-        self.queue_draw ()
+        self.queue_draw()
         return True
 
 
-class Viewer (object):
-    def __init__ (self, title='Array Viewer', default_width=DEFAULT_WIN_WIDTH,
-                  default_height=DEFAULT_WIN_HEIGHT):
-        self.viewport = Viewport ()
-        self.win = Gtk.Window (Gtk.WindowType.TOPLEVEL)
-        self.win.set_title (title)
-        self.win.set_default_size (default_width, default_height)
-        self.win.connect ('key-press-event', self._on_key_press)
+class Viewer(object):
+    def __init__(self, title='Array Viewer', default_width=DEFAULT_WIN_WIDTH,
+                 default_height=DEFAULT_WIN_HEIGHT):
+        self.viewport = Viewport()
+        self.win = Gtk.Window(type=Gtk.WindowType.TOPLEVEL)
+        self.win.set_title(title)
+        self.win.set_default_size(default_width, default_height)
+        self.win.connect('key-press-event', self._on_key_press)
 
-        vb = Gtk.VBox ()
-        vb.pack_start (self.viewport, True, True, 2)
-        hb = Gtk.HBox ()
-        vb.pack_start (hb, False, True, 2)
+        vb = Gtk.VBox()
+        vb.pack_start(self.viewport, True, True, 2)
+        hb = Gtk.HBox()
+        vb.pack_start(hb, False, True, 2)
 
-        self.status_label = Gtk.Label ()
-        self.status_label.set_alignment (0, 0.5)
-        hb.pack_start (self.status_label, True, True, 2)
+        self.status_label = Gtk.Label()
+        self.status_label.set_alignment(0, 0.5)
+        hb.pack_start(self.status_label, True, True, 2)
 
-        self.status_label.set_markup ('Temp')
+        self.status_label.set_markup('Temp')
 
-        self.win.add (vb)
+        self.win.add(vb)
 
 
-    def set_shape_getter (self, getshape):
-        self.viewport.set_shape_getter (getshape)
+    def set_shape_getter(self, getshape):
+        self.viewport.set_shape_getter(getshape)
         return self
 
 
-    def set_tuning_setter (self, settuning):
-        self.viewport.set_tuning_setter (settuning)
+    def set_tuning_setter(self, settuning):
+        self.viewport.set_tuning_setter(settuning)
         return self
 
 
-    def set_surface_getter (self, getsurface):
-        self.viewport.set_surface_getter (getsurface)
+    def set_surface_getter(self, getsurface):
+        self.viewport.set_surface_getter(getsurface)
         return self
 
 
-    def set_status_formatter (self, fmtstatus):
-        def onmotion (x, y):
-            self.status_label.set_markup (fmtstatus (x, y))
-        self.viewport.set_motion_handler (onmotion)
+    def set_status_formatter(self, fmtstatus):
+        def onmotion(x, y):
+            self.status_label.set_markup(fmtstatus(x, y))
+        self.viewport.set_motion_handler(onmotion)
         return self
 
 
-    def set_overlay_drawer (self, drawoverlay):
-        self.viewport.set_overlay_drawer (drawoverlay)
+    def set_overlay_drawer(self, drawoverlay):
+        self.viewport.set_overlay_drawer(drawoverlay)
         return self
 
 
-    def _on_key_press (self, widget, event):
-        kn = Gdk.keyval_name (event.keyval)
-        modmask = Gtk.accelerator_get_default_mod_mask ()
+    def _on_key_press(self, widget, event):
+        kn = Gdk.keyval_name(event.keyval)
+        modmask = Gtk.accelerator_get_default_mod_mask()
         isctrl = (event.state & modmask) == Gdk.ModifierType.CONTROL_MASK
 
         if kn == 'a' and isctrl:
-            self.viewport.autoscale ()
+            self.viewport.autoscale()
             return True
 
         if kn == 'e' and isctrl:
-            self.viewport.center ()
+            self.viewport.center()
             return True
 
         if kn == 'f' and isctrl:
-            self.win.fullscreen ()
+            self.win.fullscreen()
             return True
 
         if kn == 'Escape':
-            self.win.unfullscreen ()
+            self.win.unfullscreen()
             return True
 
         if kn == 'w' and isctrl:
-            self.win.destroy ()
+            self.win.destroy()
             return True
 
         if kn == '1' and isctrl:
             self.viewport.scale = 1.
-            self.viewport.queue_draw ()
+            self.viewport.queue_draw()
             return True
 
         if kn == 's' and isctrl:
-            print ('Writing data.png ...', end='')
-            sys.stdout.flush ()
-            self.viewport.write_data_as_png ('data.png')
-            print ('done')
+            print('Writing data.png ...', end='')
+            sys.stdout.flush()
+            self.viewport.write_data_as_png('data.png')
+            print('done')
             return True
 
         if kn == 'z':
             if isctrl:
                 self.viewport.scale *= 1.2
             else:
                 self.viewport.scale *= 1.05
@@ -517,415 +516,459 @@
                 self.viewport.scale /= 1.05
             self.viewport.queue_draw()
             return True
 
         return False
 
 
-def view (array, title='Array Viewer', colormap='black_to_blue', toworld=None,
-          drawoverlay=None, yflip=False, tostatus=None, run_main=True):
+def view(array, title='Array Viewer', colormap='black_to_blue', toworld=None,
+         drawoverlay=None, yflip=False, tostatus=None, run_main=True):
     if toworld is not None and tostatus is not None:
-        raise ValueError ('only one of "toworld" and "tostatus" may be given')
+        raise ValueError('only one of "toworld" and "tostatus" may be given')
 
-    clipper = Clipper ()
-    clipper.alloc_buffer (array)
-    clipper.set_tile_size ()
-    clipper.default_bounds (array)
+    clipper = Clipper()
+    clipper.alloc_buffer(array)
+    clipper.set_tile_size()
+    clipper.default_bounds(array)
     processed = clipper.buffer
 
-    mapper = ColorMapper (colormap)
-    mapper.alloc_buffer (array)
-    mapper.set_tile_size ()
+    mapper = ColorMapper(colormap)
+    mapper.alloc_buffer(array)
+    mapper.set_tile_size()
 
     h, w = array.shape
-    stride = cairo.ImageSurface.format_stride_for_width (cairo.FORMAT_ARGB32,
-                                                         w)
+    stride = cairo.ImageSurface.format_stride_for_width(cairo.FORMAT_ARGB32, w)
     assert stride % 4 == 0 # stride is in bytes
     assert stride == 4 * w # size of buffer is set in mapper
-    imagesurface = cairo.ImageSurface.create_for_data (mapper.buffer,
-                                                       cairo.FORMAT_ARGB32,
-                                                       w, h, stride)
+    imagesurface = cairo.ImageSurface.create_for_data(mapper.buffer,
+                                                      cairo.FORMAT_ARGB32,
+                                                      w, h, stride)
 
-    def getshape ():
+    def getshape():
         return w, h
 
     orig_min = clipper.dmin
     orig_span = clipper.dmax - orig_min
 
-    def settuning (tunerx, tunery):
+    def settuning(tunerx, tunery):
         clipper.dmin = orig_span * tunerx + orig_min
         clipper.dmax = orig_span * tunery + orig_min
-        clipper.invalidate ()
-        mapper.invalidate ()
+        clipper.invalidate()
+        mapper.invalidate()
 
-    def getsurface (xoffset, yoffset, width, height):
-        pxofs = max (int (np.floor (-xoffset)), 0)
-        pyofs = max (int (np.floor (-yoffset)), 0)
-        pw = min (int (np.ceil (width)), w - pxofs)
-        ph = min (int (np.ceil (height)), h - pyofs)
+    def getsurface(xoffset, yoffset, width, height):
+        pxofs = max(int(np.floor(-xoffset)), 0)
+        pyofs = max(int(np.floor(-yoffset)), 0)
+        pw = min(int(np.ceil(width)), w - pxofs)
+        ph = min(int(np.ceil(height)), h - pyofs)
 
-        clipper.ensure_region_updated (array, pxofs, pyofs, pw, ph)
-        mapper.ensure_region_updated (processed, pxofs, pyofs, pw, ph)
+        clipper.ensure_region_updated(array, pxofs, pyofs, pw, ph)
+        mapper.ensure_region_updated(processed, pxofs, pyofs, pw, ph)
 
         return imagesurface, xoffset, yoffset
 
     # I originally had the is_masked call inside fmtstatus and somehow it
     # ended up causing large lags in the label updates. Can't be that
     # CPU-intensive, right??
 
-    nomask = not np.ma.is_masked (array) or array.mask is np.ma.nomask
+    nomask = not np.ma.is_masked(array) or array.mask is np.ma.nomask
 
     if tostatus is None:
         if toworld is None:
             tostatus = lambda t: ''
         else:
             from .astutil import fmthours, fmtdeglat
 
-            def tostatus (y_and_x):
-                lat, lon = toworld (y_and_x)
-                return 'lat=%s lon=%s' % (fmtdeglat (lat), fmthours (lon))
+            def tostatus(y_and_x):
+                lat, lon = toworld(y_and_x)
+                return 'lat=%s lon=%s' % (fmtdeglat(lat), fmthours(lon))
 
 
-    def fmtstatus (x, y):
+    def fmtstatus(x, y):
         s = ''
-        row = int (np.floor (y + 0.5))
-        col = int (np.floor (x + 0.5))
+        row = int(np.floor(y + 0.5))
+        col = int(np.floor(x + 0.5))
         if row >= 0 and col >= 0 and row < h and col < w:
             if nomask or not array.mask[row,col]:
                 s += '%g ' % array[row,col]
         if yflip:
             y = h - 1 - y
             row = h - 1 - row
 
         s += '[%d,%d] x=%.1f y=%.1f %s' % \
-            (row, col, x, y, tostatus (np.array ([y, x])))
+             (row, col, x, y, tostatus(np.array([y, x])))
         return s
 
-    viewer = Viewer (title=title)
-    viewer.set_shape_getter (getshape)
-    viewer.set_tuning_setter (settuning)
-    viewer.set_surface_getter (getsurface)
-    viewer.set_status_formatter (fmtstatus)
-    viewer.set_overlay_drawer (drawoverlay)
-    viewer.win.show_all ()
+    viewer = Viewer(title=title)
+    viewer.set_shape_getter(getshape)
+    viewer.set_tuning_setter(settuning)
+    viewer.set_surface_getter(getsurface)
+    viewer.set_status_formatter(fmtstatus)
+    viewer.set_overlay_drawer(drawoverlay)
+    viewer.win.show_all()
 
     if run_main:
-        viewer.win.connect ('destroy', Gtk.main_quit)
-        Gtk.main ()
+        viewer.win.connect('destroy', Gtk.main_quit)
+        Gtk.main()
     else:
-        viewer.win.connect ('destroy', lambda e: viewer.win.destroy ())
+        viewer.win.connect('destroy', lambda e: viewer.win.destroy())
 
 
-class Cycler (Viewer):
+class Cycler(Viewer):
     getn = None
     getshapei = None
     getdesci = None
     settuningi = None
     getsurfacei = None
 
     i = None
     sourceid = None
     needtune = None
 
-    def __init__ (self, title='Array Cycler', default_width=DEFAULT_WIN_WIDTH,
-                  default_height=DEFAULT_WIN_HEIGHT, cadence=0.6):
+    def __init__(self, title='Array Cycler', default_width=DEFAULT_WIN_WIDTH,
+                 default_height=DEFAULT_WIN_HEIGHT, cadence=0.6):
         self.cadence = cadence
 
-        self.viewport = Viewport ()
-        self.win = Gtk.Window (Gtk.WindowType.TOPLEVEL)
-        self.win.set_title (title)
-        self.win.set_default_size (default_width, default_height)
-        self.win.connect ('key-press-event', self._on_key_press)
-        self.win.connect ('realize', self._on_realize)
-        self.win.connect ('unrealize', self._on_unrealize)
-
-        vb = Gtk.VBox ()
-        vb.pack_start (self.viewport, True, True, 2)
-        hb = Gtk.HBox ()
-        vb.pack_start (hb, False, True, 2)
-        self.status_label = Gtk.Label ()
-        self.status_label.set_alignment (0, 0.5)
-        hb.pack_start (self.status_label, True, True, 2)
-        self.plane_label = Gtk.Label ()
-        self.plane_label.set_alignment (0, 0.5)
-        hb.pack_start (self.plane_label, True, True, 2)
-        self.desc_label = Gtk.Label ()
-        hb.pack_start (self.desc_label, True, True, 2)
-        self.cycle_tbutton = Gtk.ToggleButton ('Cycle')
-        hb.pack_start (self.cycle_tbutton, False, True, 2)
-        self.win.add (vb)
-
-        self.viewport.set_shape_getter (self._get_shape)
-        self.viewport.set_surface_getter (self._get_surface)
-        self.viewport.set_tuning_setter (self._set_tuning)
-
-        self.cycle_tbutton.set_active (True)
-
-
-    def set_n_getter (self, getn):
-        if not callable (getn):
-            raise ValueError ('not callable')
+        self.viewport = Viewport()
+        self.win = Gtk.Window(type=Gtk.WindowType.TOPLEVEL)
+        self.win.set_title(title)
+        self.win.set_default_size(default_width, default_height)
+        self.win.connect('key-press-event', self._on_key_press)
+        self.win.connect('realize', self._on_realize)
+        self.win.connect('unrealize', self._on_unrealize)
+
+        vb = Gtk.VBox()
+        vb.pack_start(self.viewport, True, True, 2)
+        hb = Gtk.HBox()
+        vb.pack_start(hb, False, True, 2)
+        self.status_label = Gtk.Label()
+        self.status_label.set_alignment(0, 0.5)
+        hb.pack_start(self.status_label, True, True, 2)
+        self.plane_label = Gtk.Label()
+        self.plane_label.set_alignment(0, 0.5)
+        hb.pack_start(self.plane_label, True, True, 2)
+        self.desc_label = Gtk.Label()
+        hb.pack_start(self.desc_label, True, True, 2)
+        self.cycle_tbutton = Gtk.ToggleButton(label='Cycle')
+        hb.pack_start(self.cycle_tbutton, False, True, 2)
+        self.win.add(vb)
+
+        self.viewport.set_shape_getter(self._get_shape)
+        self.viewport.set_surface_getter(self._get_surface)
+        self.viewport.set_tuning_setter(self._set_tuning)
+
+        self.cycle_tbutton.set_active(True)
+
+
+    def set_n_getter(self, getn):
+        if not callable(getn):
+            raise ValueError('not callable')
         self.getn = getn
         return self
 
 
-    def _get_shape (self):
+    def _get_shape(self):
         if self.i is None:
-            self.set_current (0)
-        return self.getshapei (self.i)
+            self.set_current(0)
+        return self.getshapei(self.i)
 
 
-    def set_shape_getter (self, getshapei):
-        if not callable (getshapei):
-            raise ValueError ('not callable')
+    def set_shape_getter(self, getshapei):
+        if not callable(getshapei):
+            raise ValueError('not callable')
         self.getshapei = getshapei
         return self
 
 
-    def set_desc_getter (self, getdesci):
-        if not callable (getdesci):
-            raise ValueError ('not callable')
+    def set_desc_getter(self, getdesci):
+        if not callable(getdesci):
+            raise ValueError('not callable')
         self.getdesci = getdesci
         return self
 
 
-    def _set_tuning (self, tunerx, tunery):
+    def _set_tuning(self, tunerx, tunery):
         if self.i is None:
-            self.set_current (0)
-        self.settuningi (self.i, tunerx, tunery)
-        self.needtune.fill (True)
+            self.set_current(0)
+        self.settuningi(self.i, tunerx, tunery)
+        self.needtune.fill(True)
         self.needtune[self.i] = False
+        self.last_tunerx = tunerx
+        self.last_tunery = tunery
 
 
-    def set_tuning_setter (self, settuningi):
-        if not callable (settuningi):
-            raise ValueError ('not callable')
+    def set_tuning_setter(self, settuningi):
+        if not callable(settuningi):
+            raise ValueError('not callable')
         self.settuningi = settuningi
-        self.viewport.set_tuning_setter (self._set_tuning) # force retune
+        self.viewport.set_tuning_setter(self._set_tuning) # force retune
         return self
 
 
-    def _get_surface (self, xoffset, yoffset, width, height):
+    def _get_surface(self, xoffset, yoffset, width, height):
         if self.i is None:
-            self.set_current (0)
-        return self.getsurfacei (self.i, xoffset, yoffset, width, height)
+            self.set_current(0)
+        return self.getsurfacei(self.i, xoffset, yoffset, width, height)
 
 
-    def set_surface_getter (self, getsurfacei):
-        if not callable (getsurfacei):
-            raise ValueError ('not callable')
+    def set_surface_getter(self, getsurfacei):
+        if not callable(getsurfacei):
+            raise ValueError('not callable')
         self.getsurfacei = getsurfacei
         return self
 
 
-    def set_status_formatter (self, fmtstatusi):
+    def set_status_formatter(self, fmtstatusi):
         if fmtstatusi is None:
-            self.viewport.set_motion_handler (None)
+            self.viewport.set_motion_handler(None)
         else:
-            def onmotion (x, y):
-                self.status_label.set_markup (fmtstatusi (self.i, x, y))
-            self.viewport.set_motion_handler (onmotion)
+            def onmotion(x, y):
+                self.status_label.set_markup(fmtstatusi(self.i, x, y))
+            self.viewport.set_motion_handler(onmotion)
         return self
 
 
-    def set_overlay_drawer (self, drawoverlay):
-        self.viewport.set_overlay_drawer (drawoverlay)
+    def set_overlay_drawer(self, drawoverlay):
+        self.viewport.set_overlay_drawer(drawoverlay)
         return self
 
 
-    def set_current (self, index):
-        n = self.getn ()
+    def set_current(self, index):
+        n = self.getn()
         index = index % n
 
         if self.needtune is None or self.needtune.size != n:
-            self.needtune = np.ones (n, dtype=np.bool_)
+            self.needtune = np.ones(n, dtype=np.bool_)
 
         if index == self.i:
             return
 
         if self.needtune[index]:
             # Force the viewport to call settuning the next time it needs to
-            self.viewport.set_tuning_setter (self._set_tuning)
+            self.viewport.set_tuning_setter(self._set_tuning)
 
         self.i = index
-        self.plane_label.set_markup ('<b>Current plane:</b> %d of %d' %
-                                     (self.i + 1, n))
-        self.desc_label.set_text (self.getdesci (self.i))
+        self.plane_label.set_markup('<b>Current plane:</b> %d of %d' %
+                                    (self.i + 1, n))
+        self.desc_label.set_text(self.getdesci(self.i))
 
         if self.viewport.onmotion is not None:
-            datax, datay = self.viewport.get_pointer_data_coords ()
-            self.viewport.onmotion (datax, datay)
+            datax, datay = self.viewport.get_pointer_data_coords()
+            self.viewport.onmotion(datax, datay)
 
-        self.viewport.queue_draw ()
+        self.viewport.queue_draw()
 
 
-    def _on_realize (self, widget):
+    def _on_realize(self, widget):
         if self.sourceid is not None:
             return
-        self.sourceid = GLib.timeout_add (int (self.cadence * 1000), self._do_cycle)
+        self.sourceid = GLib.timeout_add(int(self.cadence * 1000), self._do_cycle)
 
 
-    def _on_unrealize (self, widget):
+    def _on_unrealize(self, widget):
         if self.sourceid is None:
             return
-        GLib.source_remove (self.sourceid)
+        GLib.source_remove(self.sourceid)
         self.sourceid = None
 
 
-    def _do_cycle (self):
-        if self.cycle_tbutton.get_active ():
-            self.set_current (self.i + 1)
+    def _do_cycle(self):
+        if self.cycle_tbutton.get_active():
+            self.set_current(self.i + 1)
         return True
 
 
-    def _on_key_press (self, widget, event):
-        kn = Gdk.keyval_name (event.keyval)
-        modmask = Gtk.accelerator_get_default_mod_mask ()
+    def _on_key_press(self, widget, event):
+        kn = Gdk.keyval_name(event.keyval)
+        modmask = Gtk.accelerator_get_default_mod_mask()
         isctrl = (event.state & modmask) == Gdk.ModifierType.CONTROL_MASK
 
         if kn == 'j' and isctrl:
-            self.set_current (self.i - 1)
+            self.set_current(self.i - 1)
             return True
 
         if kn == 'k' and isctrl:
-            self.set_current (self.i + 1)
+            self.set_current(self.i + 1)
             return True
 
         if kn == 'c' and isctrl:
-            self.cycle_tbutton.set_active (not self.cycle_tbutton.get_active ())
+            self.cycle_tbutton.set_active(not self.cycle_tbutton.get_active())
             return True
 
-        return super (Cycler, self)._on_key_press (widget, event)
+        return super(Cycler, self)._on_key_press(widget, event)
+
 
+def cycle(arrays, descs=None, cadence=0.6, toworlds=None,
+          drawoverlay=None, yflip=False, tostatuses=None, run_main=True,
+          save_after_viewing=None):
+    """Interactively display a series of 2D data arrays.
+
+    arrays
+      An iterable of 2D arrays (a 3D array works).
+    descs
+      An iterable of text descriptions, one for each array
+    cadence
+      The time delay before the next array is shown, in seconds.
+    tostatuses
+      An iterable of functions that convert cursor positions to a textual
+      status output corresponding to that position. FIXME details needed.
+    toworlds
+      An iterable of functions that convert cursor positions to a
+      latitude/longitude pair that is displayed in the status output.
+      The `tostatuses` keyword is a more generic version of this.
+      FIXME details needed.
+    drawoverlay
+      An optional function that draws an overlay on the display after
+      the underlying data image is presented. FIXME details needed.
+    yflip
+      If true, have the numerical *y* coordinates have 0 refer to the
+      bottom of the image. Note that the data array is still drawn such
+      that its first row appears at the top!
+    run_main
+      If true, run the Gtk mainloop explicitly so that the function does
+      not return until the window is closed. If false, no mainloop is run.
+      If the application happens to already be running a mainloop in the
+      background, the window will appear and the user will be able to
+      interact with it while this thread continues executing.
+    save_after_viewing
+      If set to a string containing an integer percent-formatting specifier,
+      the data will be written to a series of PNG files after the window is
+      closed.
 
-def cycle (arrays, descs=None, cadence=0.6, toworlds=None,
-           drawoverlay=None, yflip=False, tostatuses=None, run_main=True):
-    n = len (arrays)
+    """
+    n = len(arrays)
     amin = amax = h = w = None
 
     if toworlds is not None and tostatuses is not None:
-        raise ValueError ('only one of "toworlds" and "tostatuses" may be given')
+        raise ValueError('only one of "toworlds" and "tostatuses" may be given')
 
     if descs is None:
         descs = [''] * n
 
     for array in arrays:
         thish, thisw = array.shape
-        thismin, thismax = array.min (), array.max ()
+        thismin, thismax = array.min(), array.max()
 
-        if not np.isfinite (thismin):
-            thismin = array[np.ma.where (np.isfinite (array))].min ()
-        if not np.isfinite (thismax):
-            thismax = array[np.ma.where (np.isfinite (array))].max ()
+        if not np.isfinite(thismin):
+            thismin = array[np.ma.where(np.isfinite(array))].min()
+        if not np.isfinite(thismax):
+            thismax = array[np.ma.where(np.isfinite(array))].max()
 
         if amin is None:
             w, h, amin, amax = thisw, thish, thismin, thismax
         else:
             if thisw != w:
-                raise ValueError ('array widths not all equal')
+                raise ValueError('array widths not all equal')
             if thish != h:
-                raise ValueError ('array heights not all equal')
+                raise ValueError('array heights not all equal')
 
-            amin = min (amin, thismin)
-            amax = max (amax, thismax)
+            amin = min(amin, thismin)
+            amax = max(amax, thismax)
 
-    stride = cairo.ImageSurface.format_stride_for_width (cairo.FORMAT_ARGB32, w)
+    stride = cairo.ImageSurface.format_stride_for_width(cairo.FORMAT_ARGB32, w)
     assert stride % 4 == 0 # stride is in bytes
-    imgdata = np.empty ((n, h, stride // 4), dtype=np.uint32)
-    fixed = np.empty ((n, h, w), dtype=np.int32)
-    antimask = np.empty ((n, h, w), dtype=np.bool_)
+    imgdata = np.empty((n, h, stride // 4), dtype=np.uint32)
+    fixed = np.empty((n, h, w), dtype=np.int32)
+    antimask = np.empty((n, h, w), dtype=np.bool_)
     surfaces = [None] * n
 
-    imgdata.fill (0xFF000000)
+    imgdata.fill(0xFF000000)
 
-    for i, array in enumerate (arrays):
-        surfaces[i] = cairo.ImageSurface.create_for_data (imgdata[i], cairo.FORMAT_ARGB32,
-                                                          w, h, stride)
+    for i, array in enumerate(arrays):
+        surfaces[i] = cairo.ImageSurface.create_for_data(imgdata[i], cairo.FORMAT_ARGB32,
+                                                         w, h, stride)
 
-        if np.ma.is_masked (array):
-            filled = array.filled (amin)
+        if np.ma.is_masked(array):
+            filled = array.filled(amin)
             antimask[i] = ~array.mask
         else:
             filled = array
-            antimask[i].fill (True)
+            antimask[i].fill(True)
 
         fixed[i] = (filled - amin) * (0x0FFFFFF0 / (amax - amin))
 
-    def getn ():
+    def getn():
         return n
 
-    def getshapei (i):
+    def getshapei(i):
         return w, h
 
-    def getdesci (i):
+    def getdesci(i):
         return descs[i]
 
-    clipped = np.zeros ((h, w), dtype=np.int32) # scratch arrays -- two needed
-    clipped2 = np.zeros ((h, w), dtype=np.uint32) # to make numpy ufunc casting happy
+    clipped = np.zeros((h, w), dtype=np.int32) # scratch arrays -- two needed
+    clipped2 = np.zeros((h, w), dtype=np.uint32) # to make numpy ufunc casting happy
 
-    def settuningi (i, tunerx, tunery):
-        np.bitwise_and (imgdata[i], 0xFF000000, imgdata[i])
+    def settuningi(i, tunerx, tunery):
+        np.bitwise_and(imgdata[i], 0xFF000000, imgdata[i])
 
-        fmin = int (0x0FFFFFF0 * tunerx)
-        fmax = int (0x0FFFFFF0 * tunery)
+        fmin = int(0x0FFFFFF0 * tunerx)
+        fmax = int(0x0FFFFFF0 * tunery)
 
         if fmin == fmax:
-            np.add (imgdata[i], 255 * (fixed[i] > fmin).astype(np.uint32), imgdata[i])
+            np.add(imgdata[i], 255 * (fixed[i] > fmin).astype(np.uint32), imgdata[i])
         else:
-            np.clip (fixed[i], fmin, fmax, clipped)
-            np.subtract (clipped, fmin, clipped)
-            np.multiply (clipped, 255. / (fmax - fmin), clipped2, casting='unsafe')
-            np.add (imgdata[i], clipped2, imgdata[i])
+            np.clip(fixed[i], fmin, fmax, clipped)
+            np.subtract(clipped, fmin, clipped)
+            np.multiply(clipped, 255. / (fmax - fmin), clipped2, casting='unsafe')
+            np.add(imgdata[i], clipped2, imgdata[i])
 
-        np.multiply (imgdata[i], antimask[i], imgdata[i])
+        np.multiply(imgdata[i], antimask[i], imgdata[i])
 
-    def getsurfacei (i, xoffset, yoffset, width, height):
+    def getsurfacei(i, xoffset, yoffset, width, height):
         return surfaces[i], xoffset, yoffset
 
     # see comment in view()
-    nomasks = [not np.ma.is_masked (a) or a.mask is np.ma.nomask
+    nomasks = [not np.ma.is_masked(a) or a.mask is np.ma.nomask
                for a in arrays]
 
     if tostatuses is None:
         if toworlds is None:
             tostatuses = [None] * n
         else:
             from .astutil import fmthours, fmtdeglat
 
-            def make_status_func (toworld):
-                def status (y_and_x):
-                    lat, lon = toworld (y_and_x)
-                    return 'lat=%s lon=%s' % (fmtdeglat (lat),
-                                              fmthours (lon))
+            def make_status_func(toworld):
+                def status(y_and_x):
+                    lat, lon = toworld(y_and_x)
+                    return 'lat=%s lon=%s' % (fmtdeglat(lat),
+                                              fmthours(lon))
 
-            tostatuses = [make_status_func (toworlds[i]) for i in range (n)]
+            tostatuses = [make_status_func(toworlds[i]) for i in range(n)]
 
-    def fmtstatusi (i, x, y):
+    def fmtstatusi(i, x, y):
         s = ''
-        row = int (np.floor (y + 0.5))
-        col = int (np.floor (x + 0.5))
+        row = int(np.floor(y + 0.5))
+        col = int(np.floor(x + 0.5))
         if row >= 0 and col >= 0 and row < h and col < w:
             if nomasks[i] or not arrays[i].mask[row,col]:
                 s += '%g ' % arrays[i][row,col]
         if yflip:
             y = h - 1 - y
             row = h - 1 - row
         s += '[%d,%d] x=%.1f y=%.1f' % (row, col, x, y)
         if tostatuses[i] is not None:
-            s += ' ' + tostatuses[i] (np.array ([y, x]))
+            s += ' ' + tostatuses[i](np.array([y, x]))
         return s
 
-    cycler = Cycler ()
-    cycler.set_n_getter (getn)
-    cycler.set_shape_getter (getshapei)
-    cycler.set_desc_getter (getdesci)
-    cycler.set_tuning_setter (settuningi)
-    cycler.set_surface_getter (getsurfacei)
-    cycler.set_status_formatter (fmtstatusi)
-    cycler.set_overlay_drawer (drawoverlay)
-    cycler.win.show_all ()
+    cycler = Cycler()
+    cycler.set_n_getter(getn)
+    cycler.set_shape_getter(getshapei)
+    cycler.set_desc_getter(getdesci)
+    cycler.set_tuning_setter(settuningi)
+    cycler.set_surface_getter(getsurfacei)
+    cycler.set_status_formatter(fmtstatusi)
+    cycler.set_overlay_drawer(drawoverlay)
+    cycler.win.show_all()
 
     if run_main:
-        cycler.win.connect ('destroy', Gtk.main_quit)
-        Gtk.main ()
+        cycler.win.connect('destroy', Gtk.main_quit)
+        Gtk.main()
     else:
-        cycler.win.connect ('destroy', lambda e: cycler.win.destroy ())
+        cycler.win.connect('destroy', lambda e: cycler.win.destroy())
+
+    if save_after_viewing is not None:
+        for i in range(n):
+            filename = save_after_viewing % (i,)
+            settuningi(i, cycler.last_tunerx,  cycler.last_tunery)
+            surface, xoffset, yoffset = getsurfacei(i, 0, 0, w, h)
+            surface.write_to_png(filename)
```

### Comparing `pwkit-0.8.9/pwkit/synphot.py` & `pwkit-1.0.0/pwkit/synphot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2014 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2014-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
-"""pwkit.synphot - Synthetic photometry and database of instrumental bandpasses.
+"""Synthetic photometry and database of instrumental bandpasses.
 
 The basic structure is that we have a registry of bandpass info. You can use
 it to create Bandpass objects that can perform various calculations,
 especially the computation of synthetic photometry given a spectral model.
 Some key attributes of each bandpass are pre-computed so that certain
 operations can be done without needing to load the actual bandpass profile
 (though so far none of these profiles are very large at all).
 
-Classes:
+The bandpass definitions built into this module are:
 
-AlreadyDefinedError - Raised when re-registering bandpass info.
-Bandpass            - Performs standard computations given a bandpass profile.
-NotDefinedError     - Raised when needed bandpass info is unavailable.
-Registry            - A registry of known bandpass profiles.
+* 2MASS (JHK)
+* Bessell (UBVRI)
+* GALEX (NUV, FUV)
+* LMIRCam on LBT
+* MEarth
+* Mauna Kea Observatory (MKO) (JHKLM)
+* SDSS (u' g' r' i' z')
+* Swift (UVW1)
+* WISE (1234)
 
-Functions:
+**Classes:**
 
-get_std_registry - Retrieve a Registry pre-filled with builtin telescope info.
-(unlisted)       - Various internal utilities may be useful for reference.
+.. autosummary::
+   AlreadyDefinedError
+   Bandpass
+   NotDefinedError
+   Registry
 
-Variables:
+**Functions:**
 
-builtin_registrars - Hashtable of functions to register the builtin telescopes.
+.. autosummary::
+   get_std_registry
 
+Various internal utilities may be useful for reference but are not documented here.
+
+**Variables:**
+
+.. autosummary::
+   builtin_registrars
 
 Example
 -------
 
-from pwkit import synphot as ps, cgs as pc, msmt as pm
-reg = ps.get_std_registry ()
-print (reg.telescopes ()) # list known telescopes
-print (reg.bands ('2MASS')) # list known 2MASS bands
-bp = reg.get ('2MASS', 'Ks')
-mag = 12.83
-mjy = pm.repval (bp.mag_to_fnu (mag) * pc.jypercgs * 1e3)
-print ('%.2f mag is %.2f mjy in 2MASS/Ks' % (mag, mjy))
+::
+
+  from pwkit import synphot as ps, cgs as pc, msmt as pm
+  reg = ps.get_std_registry()
+  print(reg.telescopes()) # list known telescopes
+  print(reg.bands('2MASS')) # list known 2MASS bands
+  bp = reg.get('2MASS', 'Ks')
+  mag = 12.83
+  mjy = pm.repval(bp.mag_to_fnu(mag) * pc.jypercgs * 1e3)
+  print('%.2f mag is %.2f mjy in 2MASS/Ks' % (mag, mjy))
 
 
 Conventions
 -----------
 
 It is very important to maintain consistent conventions throughout.
 
@@ -71,295 +88,291 @@
 This module requires Scipy and Pandas. It doesn't reeeeallllly need Pandas but
 it's convenient.
 
 References
 ----------
 
 Casagrande & VandenBerg (2014; arxiv:1407.6095) has a lot of good stuff; see
-  also references therein.
+also references therein.
 
 References for specific bandpasses are given in their implementation
 docstrings.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('''AlreadyDefinedError Bandpass NotDefinedError Registry
-                  builtin_registrars get_std_registry''').split ()
+__all__ = '''
+AlreadyDefinedError
+Bandpass
+NotDefinedError
+Registry
+builtin_registrars
+get_std_registry'''.split()
 
 import numpy as np, pandas as pd, pkg_resources
 
 from . import Holder, PKError, cgs, msmt
 
 
 # Data loading
 
-def bandpass_data_stream (name):
-    return pkg_resources.resource_stream ('pwkit', 'data/bandpasses/' + name)
+def bandpass_data_stream(name):
+    return pkg_resources.resource_stream('pwkit', 'data/bandpasses/' + name)
 
-def bandpass_data_frame (name, colnames):
-    a = np.loadtxt (bandpass_data_stream (name)).T
-    mapped = dict ((c, a[i]) for i, c in enumerate (colnames.split ()))
-    return pd.DataFrame (mapped)
+def bandpass_data_frame(name, colnames):
+    a = np.loadtxt(bandpass_data_stream(name)).T
+    mapped = dict((c, a[i]) for i, c in enumerate(colnames.split()))
+    return pd.DataFrame(mapped)
 
-def bandpass_data_fits (name):
+def bandpass_data_fits(name):
     from astropy.io.fits import open
-    return open (bandpass_data_stream (name))
+    return open(bandpass_data_stream(name))
 
 
 # Simple, careful conversions
 
-def fnu_cgs_to_flam_ang (fnu_cgs, pivot_angstrom):
+def fnu_cgs_to_flam_ang(fnu_cgs, pivot_angstrom):
     """erg/s/cm²/Hz → erg/s/cm²/Å"""
     return 1e8 * cgs.c / pivot_angstrom**2 * fnu_cgs
 
 
-def flam_ang_to_fnu_cgs (flam_ang, pivot_angstrom):
+def flam_ang_to_fnu_cgs(flam_ang, pivot_angstrom):
     """erg/s/cm²/Å → erg/s/cm²/Hz"""
     return 1e-8 / cgs.c * pivot_angstrom**2 * flam_ang
 
 
-def abmag_to_fnu_cgs (abmag):
+def abmag_to_fnu_cgs(abmag):
     """Convert an AB magnitude to f_ν in erg/s/cm²/Hz."""
     return cgs.cgsperjy * 3631. * 10**(-0.4 * abmag)
 
 
-def abmag_to_flam_ang (abmag, pivot_angstrom):
+def abmag_to_flam_ang(abmag, pivot_angstrom):
     """Convert an AB magnitude to f_λ in erg/s/cm²/Å. AB magnitudes are f_ν
     quantities, so a pivot wavelength is needed.
 
     """
-    return fnu_cgs_to_flam_ang (abmag_to_fnu_cgs (abmag), pivot_angstrom)
+    return fnu_cgs_to_flam_ang(abmag_to_fnu_cgs(abmag), pivot_angstrom)
 
 
-def ghz_to_ang (ghz):
+def ghz_to_ang(ghz):
     """Convert a photon frequency in GHz to its wavelength in Ångström."""
     return 0.1 * cgs.c / ghz
 
 
-def flat_ee_bandpass_pivot_wavelength (wavelen1, wavelen2):
+def flat_ee_bandpass_pivot_wavelength(wavelen1, wavelen2):
     """Compute the pivot wavelength of a bandpass that's flat in equal-energy
     terms. It turns out to be their harmonic mean.
 
     """
-    return np.sqrt (wavelen1 * wavelen2)
+    return np.sqrt(wavelen1 * wavelen2)
 
 
-def pivot_wavelength_ee (bpass):
+def pivot_wavelength_ee(bpass):
     """Compute pivot wavelength assuming equal-energy convention.
 
     `bpass` should have two properties, `resp` and `wlen`. The units of `wlen`
     can be anything, and `resp` need not be normalized in any particular way.
 
     """
     from scipy.integrate import simps
-    return np.sqrt (simps (bpass.resp, bpass.wlen) /
-                    simps (bpass.resp / bpass.wlen**2, bpass.wlen))
+    return np.sqrt(simps(bpass.resp, bpass.wlen) /
+                   simps(bpass.resp / bpass.wlen**2, bpass.wlen))
 
 
-def pivot_wavelength_qe (bpass):
+def pivot_wavelength_qe(bpass):
     """Compute pivot wavelength assuming quantum-efficiency convention. Note that
     this is NOT what we generally use in this module.
 
     `bpass` should have two properties, `resp` and `wlen`. The units of `wlen`
     can be anything, and `resp` need not be normalized in any particular way.
 
     """
     from scipy.integrate import simps
-    return np.sqrt (simps (bpass.resp * bpass.wlen, bpass.wlen) /
-                    simps (bpass.resp / bpass.wlen, bpass.wlen))
+    return np.sqrt(simps(bpass.resp * bpass.wlen, bpass.wlen) /
+                   simps(bpass.resp / bpass.wlen, bpass.wlen))
 
 
-def interpolated_halfmax_points (x, y):
+def interpolated_halfmax_points(x, y):
     """Given a curve y(x), find the x coordinates of points that have half the
     value of max(y), using linear interpolation. We're assuming that y(x) has
     a bandpass-ish shape, i.e., a single maximum and a drop to zero as we go
     to the edges of the function's domain. We also assume that x is sorted
     increasingly.
 
     """
     from scipy.interpolate import interp1d
     from scipy.optimize import fmin
 
-    x = np.asarray (x)
-    y = np.asarray (y)
-    halfmax = 0.5 * y.max ()
+    x = np.asarray(x)
+    y = np.asarray(y)
+    halfmax = 0.5 * y.max()
 
     # Guess from the actual samples.
 
     delta = y - halfmax
     guess1 = 0
     while delta[guess1] < 0:
         guess1 += 1
     guess2 = y.size - 1
     while delta[guess2] < 0:
         guess2 -= 1
 
     # Interpolate for fanciness.
 
-    terp = interp1d (x, y, kind='linear', bounds_error=False, fill_value=0.)
-    x1 = fmin (lambda x: (terp (x) - halfmax)**2, x[guess1], disp=False)
-    x2 = fmin (lambda x: (terp (x) - halfmax)**2, x[guess2], disp=False)
+    terp = interp1d(x, y, kind='linear', bounds_error=False, fill_value=0.)
+    x1 = fmin(lambda x: (terp(x) - halfmax)**2, x[guess1], disp=False)
+    x2 = fmin(lambda x: (terp(x) - halfmax)**2, x[guess2], disp=False)
 
-    x1 = np.asscalar (x1)
-    x2 = np.asscalar (x2)
+    x1 = np.asscalar(x1)
+    x2 = np.asscalar(x2)
 
     if x1 == x2:
-        raise PKError ('halfmax finding failed')
+        raise PKError('halfmax finding failed')
 
     if x1 > x2:
         x1, x2 = x2, x1
 
     return x1, x2
 
 
 
 # Organized storage of the bandpass info. This way we're extensible (ooh aah)
 # and we don't have to run a bunch of code on module import.
 
-class AlreadyDefinedError (PKError):
-    pass
+class AlreadyDefinedError(PKError):
+    """Raised when re-registering bandpass info."""
 
-class NotDefinedError (PKError):
-    pass
+class NotDefinedError(PKError):
+    """Raised when needed bandpass info is unavailable."""
 
 
-class Bandpass (object):
+class Bandpass(object):
     """Computations regarding a particular filter bandpass.
 
-    Functions:
-
-    calc_halfmax_points   - Calculate the wavelengths of the filter half-maximum values.
-    calc_pivot_wavelength - Calculate the filter's pivot wavelength.
-    halfmax_points        - Get the filter half-maximum points (calculated if not cached).
-    jy_to_flam            - Convert Jy in this filter to a f_λ.
-    mag_to_flam           - Convert a magnitude in this filter to a f_λ.
-    mag_to_fnu            - Convert a magnitude in this filter to a f_ν.
-    pivot_wavelength      - Get the filter's pivot wavelength (calculated if not cached).
-    synphot               - Compute synthetic photometry given a model spectrum.
-
-    Attributes:
-
-    band             - The name of this bandpass' associated band.
-    native_flux_kind - Which kind of flux this bandpass is calibrated to: 'flam', 'fnu', or 'none'.
-    registry         - This object's parent Registry instance.
-    telescope        - The name of this bandpass' associated telescope.
-
     The underlying bandpass shape is assumed to be sampled at discrete points.
-    It is stored in _data and loaded on-demand. The object is a Pandas
-    DataFrame containing at least the columns 'wlen' and 'resp'. The former
-    holds the wavelengths of the sample points, in Ångström and in ascending
-    order. The latter gives the response curve in the EE convention. No
-    particular normalization is assumed. Other columns may be present but are
-    not used generically.
+    It is stored in ``_data`` and loaded on-demand. The object is a Pandas
+    DataFrame containing at least the columns ``wlen`` and ``resp``. The
+    former holds the wavelengths of the sample points, in Ångström and in
+    ascending order. The latter gives the response curve in the EE convention.
+    No particular normalization is assumed. Other columns may be present but
+    are not used generically.
 
     """
     _data = None
     native_flux_kind = 'none'
+    "Which kind of flux this bandpass is calibrated to: 'flam', 'fnu', or 'none'."
 
     # These are set by the registry on construction:
     registry = None
+    "This object's parent Registry instance."
+
     telescope = None
+    "The name of this bandpass' associated telescope."
+
     band = None
+    "The name of this bandpass' associated band."
 
-    def _ensure_data (self):
+    def _ensure_data(self):
         if self._data is None:
-            self._data = self._load_data (self.band)
+            self._data = self._load_data(self.band)
         return self._data
 
 
-    def calc_pivot_wavelength (self):
+    def calc_pivot_wavelength(self):
         """Compute and return the bandpass' pivot wavelength.
 
         This value is computed directly from the bandpass data, not looked up
         in the Registry. Most of the values in the Registry were in fact
         derived from this function originally.
 
         """
-        d = self._ensure_data ()
-        return pivot_wavelength_ee (d)
+        d = self._ensure_data()
+        return pivot_wavelength_ee(d)
 
 
-    def pivot_wavelength (self):
+    def pivot_wavelength(self):
         """Get the bandpass' pivot wavelength.
 
         Unlike calc_pivot_wavelength(), this function will use a cached
         value if available.
 
         """
-        wl = self.registry._pivot_wavelengths.get ((self.telescope, self.band))
+        wl = self.registry._pivot_wavelengths.get((self.telescope, self.band))
         if wl is not None:
             return wl
 
-        wl = self.calc_pivot_wavelength ()
-        self.registry.register_pivot_wavelength (self.telescope, self.band, wl)
+        wl = self.calc_pivot_wavelength()
+        self.registry.register_pivot_wavelength(self.telescope, self.band, wl)
         return wl
 
 
-    def calc_halfmax_points (self):
-        d = self._ensure_data ()
-        return interpolated_halfmax_points (d.wlen, d.resp)
+    def calc_halfmax_points(self):
+        """Calculate the wavelengths of the filter half-maximum values.
+
+        """
+        d = self._ensure_data()
+        return interpolated_halfmax_points(d.wlen, d.resp)
 
 
-    def halfmax_points (self):
+    def halfmax_points(self):
         """Get the bandpass' half-maximum wavelengths. These can be used to
         compute a representative bandwidth, or for display purposes.
 
         Unlike calc_halfmax_points(), this function will use a cached value if
         available.
 
         """
-        t = self.registry._halfmaxes.get ((self.telescope, self.band))
+        t = self.registry._halfmaxes.get((self.telescope, self.band))
         if t is not None:
             return t
 
-        t = self.calc_halfmax_points ()
-        self.registry.register_halfmaxes (self.telescope, self.band, t[0], t[1])
+        t = self.calc_halfmax_points()
+        self.registry.register_halfmaxes(self.telescope, self.band, t[0], t[1])
         return t
 
 
-    def mag_to_fnu (self, mag):
+    def mag_to_fnu(self, mag):
         """Convert a magnitude in this band to a f_ν flux density.
 
         It is assumed that the magnitude has been computed in the appropriate
         photometric system. The definition of "appropriate" will vary from
         case to case.
 
         """
         if self.native_flux_kind == 'flam':
-            return flam_ang_to_fnu_cgs (self.mag_to_flam (mag), self.pivot_wavelength ())
-        raise PKError ('dont\'t know how to get f_ν from mag for bandpass %s/%s',
-                       self.telescope, self.band)
+            return flam_ang_to_fnu_cgs(self.mag_to_flam(mag), self.pivot_wavelength())
+        raise PKError('dont\'t know how to get f_ν from mag for bandpass %s/%s',
+                      self.telescope, self.band)
 
 
-    def mag_to_flam (self, mag):
+    def mag_to_flam(self, mag):
         """Convert a magnitude in this band to a f_λ flux density.
 
         It is assumed that the magnitude has been computed in the appropriate
         photometric system. The definition of "appropriate" will vary from
         case to case.
 
         """
         if self.native_flux_kind == 'fnu':
-            return fnu_cgs_to_flam_ang (self.mag_to_fnu (mag), self.pivot_wavelength ())
-        raise PKError ('dont\'t know how to get f_λ from mag for bandpass %s/%s',
-                       self.telescope, self.band)
+            return fnu_cgs_to_flam_ang(self.mag_to_fnu(mag), self.pivot_wavelength())
+        raise PKError('dont\'t know how to get f_λ from mag for bandpass %s/%s',
+                      self.telescope, self.band)
 
 
-    def jy_to_flam (self, jy):
+    def jy_to_flam(self, jy):
         """Convert a f_ν flux density measured in Janskys to a f_λ flux density.
 
         This conversion is bandpass-dependent because it depends on the pivot
         wavelength of the bandpass used to measure the flux density.
 
         """
-        return fnu_cgs_to_flam_ang (cgs.cgsperjy * jy, self.pivot_wavelength ())
+        return fnu_cgs_to_flam_ang(cgs.cgsperjy * jy, self.pivot_wavelength())
 
 
-    def synphot (self, wlen, flam):
+    def synphot(self, wlen, flam):
         """`wlen` and `flam` give a tabulated model spectrum in wavelength and f_λ
         units. We interpolate linearly over both the model and the bandpass
         since they're both discretely sampled.
 
         Note that quadratic interpolation is both much slower and can blow up
         fatally in some cases. The latter issue might have to do with really large
         X values that aren't zero-centered, maybe?
@@ -368,31 +381,31 @@
         complaints the way quadrature did. I should probably acquire some idea
         about what's going on under the hood.
 
         """
         from scipy.interpolate import interp1d
         from scipy.integrate import romberg
 
-        d = self._ensure_data ()
+        d = self._ensure_data()
 
-        mflam = interp1d (wlen, flam,
-                          kind='linear',
-                          bounds_error=False, fill_value=0)
-
-        mresp = interp1d (d.wlen, d.resp,
-                          kind='linear',
-                          bounds_error=False, fill_value=0)
-
-        bmin = d.wlen.min ()
-        bmax = d.wlen.max ()
-
-        numer = romberg (lambda x: mresp (x) * mflam (x),
-                         bmin, bmax, divmax=20)
-        denom = romberg (lambda x: mresp (x),
-                         bmin, bmax, divmax=20)
+        mflam = interp1d(wlen, flam,
+                         kind='linear',
+                         bounds_error=False, fill_value=0)
+
+        mresp = interp1d(d.wlen, d.resp,
+                         kind='linear',
+                         bounds_error=False, fill_value=0)
+
+        bmin = d.wlen.min()
+        bmax = d.wlen.max()
+
+        numer = romberg(lambda x: mresp(x) * mflam(x),
+                        bmin, bmax, divmax=20)
+        denom = romberg(lambda x: mresp(x),
+                        bmin, bmax, divmax=20)
         return numer / denom
 
 
     def blackbody(self, T):
         """Calculate the contribution of a blackbody through this filter. *T* is the
         blackbody temperature in Kelvin. Returns a band-averaged spectrum in
         f_λ units.
@@ -414,282 +427,280 @@
         numer_samples = d.resp * np.pi * blambda(d.wlen * 1e-8, T) * 1e-8
 
         numer = simps(numer_samples, d.wlen)
         denom = simps(d.resp, d.wlen)
         return numer / denom
 
 
-class Registry (object):
+class Registry(object):
     """A registry of known bandpass properties.
 
-    Methods:
-
-    bands                     - Return a list of bands associated with a telescope.
-    get                       - Get a Bandpass object for a known telescope and filter.
-    register_bpass            - Register a Bandpass class.
-    register_halfmaxes        - Register precomputed half-max points.
-    register_pivot_wavelength - Register precomputed pivot wavelengths.
-    telescopes                - Return a list of telescopes known to this registry.
-
     """
-    def __init__ (self):
+    def __init__(self):
         self._pivot_wavelengths = {}
         self._halfmaxes = {}
         self._bpass_classes = {}
         self._seen_bands = {}
 
 
-    def _note (self, telescope, band):
-        q = self._seen_bands.setdefault (telescope, set ())
+    def _note(self, telescope, band):
+        q = self._seen_bands.setdefault(telescope, set())
         if band is not None:
-            q.add (band)
+            q.add(band)
 
 
-    def telescopes (self):
+    def telescopes(self):
         """Return a list of telescopes known to this registry."""
-        return self._seen_bands.keys ()
+        return self._seen_bands.keys()
 
 
-    def bands (self, telescope):
+    def bands(self, telescope):
         """Return a list of bands associated with the specified telescope."""
-        q = self._seen_bands.get (telescope)
+        q = self._seen_bands.get(telescope)
         if q is None:
             return []
-        return list (q)
+        return list(q)
 
 
-    def register_pivot_wavelength (self, telescope, band, wlen):
+    def register_pivot_wavelength(self, telescope, band, wlen):
+        """Register precomputed pivot wavelengths."""
         if (telescope, band) in self._pivot_wavelengths:
-            raise AlreadyDefinedError ('pivot wavelength for %s/%s already '
-                                       'defined', telescope, band)
-        self._note (telescope, band)
+            raise AlreadyDefinedError('pivot wavelength for %s/%s already '
+                                      'defined', telescope, band)
+        self._note(telescope, band)
         self._pivot_wavelengths[telescope,band] = wlen
         return self
 
 
-    def register_halfmaxes (self, telescope, band, lower, upper):
+    def register_halfmaxes(self, telescope, band, lower, upper):
+        """Register precomputed half-max points."""
+
         if (telescope, band) in self._halfmaxes:
-            raise AlreadyDefinedError ('half-max points for %s/%s already '
-                                       'defined', telescope, band)
-        self._note (telescope, band)
+            raise AlreadyDefinedError('half-max points for %s/%s already '
+                                      'defined', telescope, band)
+        self._note(telescope, band)
         self._halfmaxes[telescope,band] = (lower, upper)
         return self
 
 
-    def register_bpass (self, telescope, klass):
+    def register_bpass(self, telescope, klass):
+        """Register a Bandpass class."""
+
         if telescope in self._bpass_classes:
-            raise AlreadyDefinedError ('bandpass class for %s already '
-                                       'defined', telescope)
-        self._note (telescope, None)
+            raise AlreadyDefinedError('bandpass class for %s already '
+                                      'defined', telescope)
+        self._note(telescope, None)
         self._bpass_classes[telescope] = klass
         return self
 
 
-    def get (self, telescope, band):
-        klass = self._bpass_classes.get (telescope)
+    def get(self, telescope, band):
+        """Get a Bandpass object for a known telescope and filter."""
+
+        klass = self._bpass_classes.get(telescope)
         if klass is None:
-            raise NotDefinedError ('bandpass data for %s not defined', telescope)
+            raise NotDefinedError('bandpass data for %s not defined', telescope)
 
-        bp = klass ()
+        bp = klass()
         bp.registry = self
         bp.telescope = telescope
         bp.band = band
         return bp
 
 
 builtin_registrars = {}
+"Hashtable of functions to register the builtin telescopes."
 
-
-def get_std_registry ():
+def get_std_registry():
     """Get a Registry object pre-filled with information for standard
     telescopes.
 
     """
     from six import itervalues
-    reg = Registry ()
-    for fn in itervalues (builtin_registrars):
-        fn (reg)
+    reg = Registry()
+    for fn in itervalues(builtin_registrars):
+        fn(reg)
     return reg
 
 
 # Now, builtin information for a variety of telescopes. Document these
 # aggressively! I have these in alphabetical order. 2MASS is first.
 
-class TwomassBandpass (Bandpass):
+class TwomassBandpass(Bandpass):
     native_flux_kind = 'flam'
 
-    def _load_data (self, band):
-        df = bandpass_data_frame ('filter_2mass_' + band + '.dat', 'wlen resp')
+    def _load_data(self, band):
+        df = bandpass_data_frame('filter_2mass_' + band + '.dat', 'wlen resp')
         df.wlen *= 1e4 # micron to Angstrom
         return df
 
     _zeropoints = {
         # 2MASS Explanatory Supplement (VI.4.a) and Cohen+ 2003.
         # I've converted W/cm²/μm to erg/s/cm²/Å (factor of 1e3).
-        'J': msmt.Uval.from_norm (3.129e-10, 5.464e-12),
-        'H': msmt.Uval.from_norm (1.133e-10, 2.212e-12),
-        'Ks': msmt.Uval.from_norm (4.283e-11, 8.053e-13),
+        'J': msmt.Uval.from_norm(3.129e-10, 5.464e-12),
+        'H': msmt.Uval.from_norm(1.133e-10, 2.212e-12),
+        'Ks': msmt.Uval.from_norm(4.283e-11, 8.053e-13),
     }
 
-    def mag_to_flam (self, mag):
+    def mag_to_flam(self, mag):
         return self._zeropoints[self.band] * 10**(-0.4 * mag)
 
 
-def register_2mass (reg):
-    reg.register_bpass ('2MASS', TwomassBandpass)
+def register_2mass(reg):
+    reg.register_bpass('2MASS', TwomassBandpass)
 
     # Computed myself from the filter response curves.
-    reg.register_pivot_wavelength ('2MASS', 'J', 12371.)
-    reg.register_pivot_wavelength ('2MASS', 'H', 16457.)
-    reg.register_pivot_wavelength ('2MASS', 'Ks', 21603.)
+    reg.register_pivot_wavelength('2MASS', 'J', 12371.)
+    reg.register_pivot_wavelength('2MASS', 'H', 16457.)
+    reg.register_pivot_wavelength('2MASS', 'Ks', 21603.)
 
     # Computed from filter responses using interpolator.
-    reg.register_halfmaxes ('2MASS', 'J', 11316., 13465.)
-    reg.register_halfmaxes ('2MASS', 'H', 15182., 17792.)
-    reg.register_halfmaxes ('2MASS', 'Ks', 20242., 23026.)
+    reg.register_halfmaxes('2MASS', 'J', 11316., 13465.)
+    reg.register_halfmaxes('2MASS', 'H', 15182., 17792.)
+    reg.register_halfmaxes('2MASS', 'Ks', 20242., 23026.)
 
 builtin_registrars['2MASS'] = register_2mass
 
 
 # Standard Bessell filters reproducing the Johnson/Cousins UBVRI photometric
 # system, using Blanton & Roweis (2007) AB corrections to get a flux density
 # scale. We don't support U since it's a bit funky; see Bessell (1990).
 
-class BessellBandpass (Bandpass):
+class BessellBandpass(Bandpass):
     native_flux_kind = 'fnu'
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """Bessell (1990) tries to determine standard filter responses that reproduce
         the Johnson/Cousins UBVRI photometric systems. Things are inherently
         imprecise because of the subtle differences between different workers'
         instruments and conventions, so it's not worth getting too worked up
         over precision.
 
         """
-        return bandpass_data_frame ('filter_bessell_' + band + '.dat', 'wlen resp')
+        return bandpass_data_frame('filter_bessell_' + band + '.dat', 'wlen resp')
 
     _ab_corrections = {
         # Entries are m_AB - m_Vega. Data are from Blanton & Roweis (2007). We
         # skip ugriz and JHK_s since SDSS/2MASS-specific works should give
         # as-good or better results, I'd hope.
         'U': 0.79,
         'B': -0.09,
         'V': 0.02,
         'R': 0.21,
         'I': 0.45,
     }
 
-    def mag_to_fnu (self, mag):
+    def mag_to_fnu(self, mag):
         """Convert a magnitude in the Johnson-Cousins system to a flux density. This
         is inherently not-so-precise since the actual conversion depends on
         the spectrum of the target and the actual passband of the filter used
         to make the observation, and a J-C magnitude is usually derived from
         instrumental magnitudes via some ad-hoc-ish transformation. But the
         following will be about right.
 
         """
-        return abmag_to_fnu_cgs (mag + self._ab_corrections[self.band])
+        return abmag_to_fnu_cgs(mag + self._ab_corrections[self.band])
 
 
-def register_bessell (reg):
-    reg.register_bpass ('Bessell', BessellBandpass)
+def register_bessell(reg):
+    reg.register_bpass('Bessell', BessellBandpass)
 
     # I computed these myself from the per-energy response curves.
-    reg.register_pivot_wavelength ('Bessell', 'B', 4370.)
-    reg.register_pivot_wavelength ('Bessell', 'V', 5478.)
-    reg.register_pivot_wavelength ('Bessell', 'R', 6496.)
-    reg.register_pivot_wavelength ('Bessell', 'I', 8020.)
+    reg.register_pivot_wavelength('Bessell', 'B', 4370.)
+    reg.register_pivot_wavelength('Bessell', 'V', 5478.)
+    reg.register_pivot_wavelength('Bessell', 'R', 6496.)
+    reg.register_pivot_wavelength('Bessell', 'I', 8020.)
 
     # Ditto.
-    reg.register_halfmaxes ('Bessell', 'B', 3885., 4832.)
-    reg.register_halfmaxes ('Bessell', 'V', 5013., 5865.)
-    reg.register_halfmaxes ('Bessell', 'R', 5653., 7220.)
-    reg.register_halfmaxes ('Bessell', 'I', 7283., 8826.)
+    reg.register_halfmaxes('Bessell', 'B', 3885., 4832.)
+    reg.register_halfmaxes('Bessell', 'V', 5013., 5865.)
+    reg.register_halfmaxes('Bessell', 'R', 5653., 7220.)
+    reg.register_halfmaxes('Bessell', 'I', 7283., 8826.)
 
 builtin_registrars['Bessell'] = register_bessell
 
 
 # GALEX
 
-class GalexBandpass (Bandpass):
+class GalexBandpass(Bandpass):
     # TODO: there are GALEX magnitudes, but the data products give flux
     # densities directly, so I haven't bothered to look up the conversions.
     native_flux_kind = 'none'
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """From Morrissey+ 2005, with the actual data coming from
         http://www.astro.caltech.edu/~capak/filters/. According to the latter,
         these are in QE units and thus need to be multiplied by the wavelength
         when integrating per-energy.
 
         """
         # `band` should be 'nuv' or 'fuv'
-        df = bandpass_data_frame ('filter_galex_' + band + '.dat', 'wlen resp')
+        df = bandpass_data_frame('filter_galex_' + band + '.dat', 'wlen resp')
         df.resp *= df.wlen # QE -> EE response convention.
         return df
 
 
-def register_galex (reg):
-    reg.register_bpass ('GALEX', GalexBandpass)
+def register_galex(reg):
+    reg.register_bpass('GALEX', GalexBandpass)
 
     # I computed these myself from the per-energy response curves.
-    reg.register_pivot_wavelength ('GALEX', 'nuv', 2305.)
-    reg.register_pivot_wavelength ('GALEX', 'fuv', 1537.)
+    reg.register_pivot_wavelength('GALEX', 'nuv', 2305.)
+    reg.register_pivot_wavelength('GALEX', 'fuv', 1537.)
 
     # Ditto.
-    reg.register_halfmaxes ('GALEX', 'nuv', 1956., 2746.)
-    reg.register_halfmaxes ('GALEX', 'fuv', 1415., 1646.)
+    reg.register_halfmaxes('GALEX', 'nuv', 1956., 2746.)
+    reg.register_halfmaxes('GALEX', 'fuv', 1415., 1646.)
 
 builtin_registrars['GALEX'] = register_galex
 
 
 # LMIRCam on the LBT.
 
-class LmircamBandpass (Bandpass):
+class LmircamBandpass(Bandpass):
     native_flux_kind = 'fnu'
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """Filter responses for LBT's LMIRCam. Emailed to me privately by Jarron
         Leisenring on 2014 May 8.
 
         """
         # `band` should be 'L'.
-        df = bandpass_data_frame ('filter_lbt_lmircam_' + band + '.dat', 'wlen resp')
+        df = bandpass_data_frame('filter_lbt_lmircam_' + band + '.dat', 'wlen resp')
         df.wlen *= 1e4 # micron to Angstrom
         df.resp *= df.wlen # QE to equal-energy response.
         return df
 
 
-    def mag_to_fnu (self, mag):
+    def mag_to_fnu(self, mag):
         """Compute F_ν for LBT LMIRCam data. This was for a one-off thing and I don't
         know if there's a reliable calibration of the photometric system to
         flux densities. It should be on an MKO-ish system, but who knows. I
         added this function to use the different pivot wavelength of the
         LMIRCam L filter, which is described as similar to, but not quite the
         same, as the MKO L'.
 
         """
         return cgs.cgsperjy * MkoBandpass._zeropoints[self.band + 'p'] * 10**(-0.4 * mag)
 
 
-def register_lbt (reg):
+def register_lbt(reg):
     # Numbers calculated manually.
-    reg.register_bpass ('LBT/LMIRCam', LmircamBandpass)
-    reg.register_pivot_wavelength ('LBT/LMIRCam', 'L', 36696.)
-    reg.register_halfmaxes ('LBT/LMIRCam', 'L', 34142., 39947.)
+    reg.register_bpass('LBT/LMIRCam', LmircamBandpass)
+    reg.register_pivot_wavelength('LBT/LMIRCam', 'L', 36696.)
+    reg.register_halfmaxes('LBT/LMIRCam', 'L', 34142., 39947.)
 
 builtin_registrars['LBT'] = register_lbt
 
 
 # MEarth. No absolute flux calibration available.
 
-class MearthBandpass (Bandpass):
+class MearthBandpass(Bandpass):
     native_flux_kind = 'none'
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """Filter response the MEarth camera. I currently only have the CCD+RG715
         system, not the interference-filter setup that was tried briefly. The
         docs say that the filter responses are somewhat different before and
         after the interference-filter experiment, but I don't think the
         information we have is sensitive to changes on those levels. The data
         were fundamentally made by reading points off of data sheets so
         they're not going to be the most accurate.
@@ -698,49 +709,49 @@
         approximations to the CCD and RG715 response curves emailed to me by
         Jonathan Irwin on 2014 Jul 11. I should write up something explaining
         what I did for posterity/reproducibility. AFAIK the response curves
         aren't published anywhere besides a hard-to-read plot in Nutzman &
         Charbonneau (2008).
 
         """
-        df = bandpass_data_frame ('filter_mearth_' + band + '.dat', 'wlen resp')
+        df = bandpass_data_frame('filter_mearth_' + band + '.dat', 'wlen resp')
         df.resp *= df.wlen # QE to equal-energy response.
         return df
 
 
-def register_mearth (reg):
-    reg.register_bpass ('MEarth', MearthBandpass)
-    reg.register_pivot_wavelength ('MEarth', 'ccd715', 8286.)
-    reg.register_halfmaxes ('MEarth', 'ccd715', 7148., 9360.)
+def register_mearth(reg):
+    reg.register_bpass('MEarth', MearthBandpass)
+    reg.register_pivot_wavelength('MEarth', 'ccd715', 8286.)
+    reg.register_halfmaxes('MEarth', 'ccd715', 7148., 9360.)
 
 builtin_registrars['MEarth'] = register_mearth
 
 
 # The Mauna Kea Observatory (MKO) IR filter system.
 
-class MkoBandpass (Bandpass):
+class MkoBandpass(Bandpass):
     native_flux_kind = 'fnu'
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """Filter responses for MKO NIR filters as specified in Tokunaga+ 2002 (see
         also Tokunaga+ 2005). I downloaded the L' profile from
         http://irtfweb.ifa.hawaii.edu/~nsfcam/hist/filters.2006.html.
 
         Pivot wavelengths from Tokunaga+ 2005 (Table 2) confirm that the
         profile is in QE convention, although my calculation of the pivot
         wavelength for L' is actually closer if I assume otherwise. M' and K_s
         are substantially better in QE convention, though, and based on the
         paper and nomenclature it seems more appropriate.
 
         """
         # `band` should be 'Lp'.
-        df = bandpass_data_frame ('filter_mko_' + band + '.dat', 'wlen resp')
+        df = bandpass_data_frame('filter_mko_' + band + '.dat', 'wlen resp')
         # Put in increasing wavelength order:
         df = df[::-1]
-        df.index = np.arange (df.shape[0])
+        df.index = np.arange(df.shape[0])
         df.wlen *= 1e4 # micron to Angstrom
         df.resp *= df.wlen # QE to equal-energy response.
         return df
 
     _zeropoints = {
         # From Tokunaga+ (2005), sort of. They list Vega flux densities for
         # different MKO filters, and note that IR magnitude systems are
@@ -755,40 +766,40 @@
         'Kp': 686.,
         'Ks': 670.,
         'K': 645.,
         'Lp': 249.,
         'Mp': 163.,
     }
 
-    def mag_to_fnu (self, mag):
+    def mag_to_fnu(self, mag):
         """Compute F_ν for an MKO IR filter band. There are some problems here since
         "MKO" is filters, not a photometric system, but people try to make
         Vega = 0.
 
         """
         return cgs.cgsperjy * self._zeropoints[self.band] * 10**(-0.4 * mag)
 
 
-def register_mko (reg):
-    reg.register_bpass ('MKO', MkoBandpass)
+def register_mko(reg):
+    reg.register_bpass('MKO', MkoBandpass)
     # From Tokunaga+ (2005), since my calculation is a fair bit different.
-    reg.register_pivot_wavelength ('MKO', 'Lp', 37520.)
+    reg.register_pivot_wavelength('MKO', 'Lp', 37520.)
     # Mine?
-    reg.register_halfmaxes ('MKO', 'Lp', 34276., 41228.)
+    reg.register_halfmaxes('MKO', 'Lp', 34276., 41228.)
 
 builtin_registrars['MKO'] = register_mko
 
 
 # Sloan Digital Sky Survey primed photometric system. We fake things a bit and
 # use the bandpasses for the unprimed filters on the main survey telescope.
 
-class SdssBandpass (Bandpass):
+class SdssBandpass(Bandpass):
     native_flux_kind = 'fnu'
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """Filter responses for SDSS. Data table from
         https://www.sdss3.org/binaries/filter_curves.fits, as linked from
         https://www.sdss3.org/instruments/camera.php#Filters. SHA1 hash of the
         file is d3f638c41e21489ba7d6dbe7bb8217d938f21184. "Determined by Jim
         Gunn in June 2001." Doi+ 2010 have updated estimates but these are
         per-column in the SDSS camera, which we don't care about.
 
@@ -805,27 +816,27 @@
         Wavelengths are in Angstrom. Based on the pivot wavelengths listed in
         http://www.astro.ljmu.ac.uk/~ikb/research/mags-fluxes/, the data table
         stores QE responses, so we have to convert them to equal-energy
         responses. Responses both including and excluding the atmosphere are
         included; I use the former.
 
         """
-        h = bandpass_data_fits ('sdss3_filter_responses.fits')
-        section = 'ugriz'.index (band[0]) + 1
+        h = bandpass_data_fits('sdss3_filter_responses.fits')
+        section = 'ugriz'.index(band[0]) + 1
         d = h[section].data
         if d.wavelength.dtype.isnative:
-            df = pd.DataFrame ({'wlen': d.wavelength, 'resp': d.respt})
+            df = pd.DataFrame({'wlen': d.wavelength, 'resp': d.respt})
         else:
-            df = pd.DataFrame ({'wlen': d.wavelength.byteswap (True).newbyteorder (),
-                                'resp': d.respt.byteswap (True).newbyteorder ()})
+            df = pd.DataFrame({'wlen': d.wavelength.byteswap(True).newbyteorder(),
+                               'resp': d.respt.byteswap(True).newbyteorder()})
         df.resp *= df.wlen # QE to equal-energy response.
         return df
 
 
-    def mag_to_fnu (self, mag):
+    def mag_to_fnu(self, mag):
         """SDSS *primed* magnitudes to F_ν. The primed magnitudes are the "USNO"
         standard-star system defined in Smith+ (2002AJ....123.2121S) and
         Fukugita+ (1996AJ....111.1748F). This system is anchored to the AB
         magnitude system, and as far as I can tell it is not known to have
         measurable offsets from that system. (As of DR10, the *unprimed* SDSS
         system is known to have small offsets from AB, but I do not believe
         that that necessarily has implications for u'g'r'i'z'.)
@@ -835,100 +846,100 @@
         telescope. The whole reason for the existence of both the primed and
         unprimed ugriz systems is that their responses do not quite match. For
         my current application, which involves a completely different
         telescope anyway, the difference shouldn't matter.
 
         """
         # `band` should be 'up', 'gp', 'rp', 'ip', or 'zp'.
-        if len (band) != 2 or band[1] != 'p':
-            raise ValueError ('band: ' + band)
-        return abmag_to_fnu_cgs (mag)
+        if len(band) != 2 or band[1] != 'p':
+            raise ValueError('band: ' + band)
+        return abmag_to_fnu_cgs(mag)
 
 
-def register_sdss (reg):
-    reg.register_bpass ('SDSS', SdssBandpass)
+def register_sdss(reg):
+    reg.register_bpass('SDSS', SdssBandpass)
 
     # I computed these myself.
-    reg.register_pivot_wavelength ('SDSS', 'up', 3557.)
-    reg.register_pivot_wavelength ('SDSS', 'gp', 4702.)
-    reg.register_pivot_wavelength ('SDSS', 'rp', 6176.)
-    reg.register_pivot_wavelength ('SDSS', 'ip', 7490.)
-    reg.register_pivot_wavelength ('SDSS', 'zp', 8947.)
+    reg.register_pivot_wavelength('SDSS', 'up', 3557.)
+    reg.register_pivot_wavelength('SDSS', 'gp', 4702.)
+    reg.register_pivot_wavelength('SDSS', 'rp', 6176.)
+    reg.register_pivot_wavelength('SDSS', 'ip', 7490.)
+    reg.register_pivot_wavelength('SDSS', 'zp', 8947.)
 
     # Ditto.
-    reg.register_halfmaxes ('SDSS', 'up', 3295., 3861.)
-    reg.register_halfmaxes ('SDSS', 'gp', 4160., 5335.)
-    reg.register_halfmaxes ('SDSS', 'rp', 5622., 6753.)
-    reg.register_halfmaxes ('SDSS', 'ip', 6917., 8171.)
-    reg.register_halfmaxes ('SDSS', 'zp', 8291., 9290.)
+    reg.register_halfmaxes('SDSS', 'up', 3295., 3861.)
+    reg.register_halfmaxes('SDSS', 'gp', 4160., 5335.)
+    reg.register_halfmaxes('SDSS', 'rp', 5622., 6753.)
+    reg.register_halfmaxes('SDSS', 'ip', 6917., 8171.)
+    reg.register_halfmaxes('SDSS', 'zp', 8291., 9290.)
 
 builtin_registrars['SDSS'] = register_sdss
 
 
 # Swift.
 
-class SwiftUvotBandpass (Bandpass):
+class SwiftUvotBandpass(Bandpass):
     # Swift routines output flux densities automatically so I haven't bothered
     # to look up the conversion from their magnitude system.
     native_flux_kind = 'none'
 
     _band_map = { 'UVW1': 'uw1' }
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """In-flight effective areas for the Swift UVOT, as obtained from the CALDB.
         See Breeveld+ 2011. XXX: confirm that these are equal-energy, not
         quantum-efficiency.
 
         """
-        d = bandpass_data_fits ('sw' + self._band_map[band] + '_20041120v106.arf')[1].data
+        d = bandpass_data_fits('sw' + self._band_map[band] + '_20041120v106.arf')[1].data
 
         # note:
         #   data.WAVE_MIN[i] < data.WAVE_MIN[i+1], but
         #   data.WAVE_MIN[i] > data.WAVE_MAX[i] (!)
         #   data.WAVE_MIN[i] = data.WAVE_MAX[i+1] (!)
 
         wmid = 0.5 * (d.WAVE_MIN + d.WAVE_MAX) # in Ångström
-        df = pd.DataFrame ({'wlen': wmid, 'resp': d.SPECRESP,
-                            'wlo': d.WAVE_MAX, 'whi': d.WAVE_MIN})
+        df = pd.DataFrame({'wlen': wmid, 'resp': d.SPECRESP,
+                           'wlo': d.WAVE_MAX, 'whi': d.WAVE_MIN})
         return df
 
 
-def register_swift (reg):
-    reg.register_bpass ('Swift/UVOT', SwiftUvotBandpass)
+def register_swift(reg):
+    reg.register_bpass('Swift/UVOT', SwiftUvotBandpass)
     # Computed manually from Breeveld+2011 response.
-    reg.register_pivot_wavelength ('Swift/UVOT', 'UVW1', 2517.)
-    reg.register_halfmaxes ('Swift/UVOT', 'UVW1', 2278., 2931.)
+    reg.register_pivot_wavelength('Swift/UVOT', 'UVW1', 2517.)
+    reg.register_halfmaxes('Swift/UVOT', 'UVW1', 2278., 2931.)
 
 builtin_registrars['Swift'] = register_swift
 
 
 # WISE
 
-class WiseBandpass (Bandpass):
+class WiseBandpass(Bandpass):
     native_flux_kind = 'fnu'
 
     _filter_subsets = {
         # The WISE filter tables are all on a common grid, which means that
         # some of them have responses that are largely essentially zero. We
         # manually clip the arrays using the numbers below.
         1: (10, 150),
         2: (140, 290),
         3: (440, 1520),
         4: (1640, 2550),
     }
 
-    def _load_data (self, band):
+    def _load_data(self, band):
         """From the WISE All-Sky Explanatory Supplement, IV.4.h.i.1, and Jarrett+
         2011. These are relative response per erg and so can be integrated
         directly against F_nu spectra. Wavelengths are in micron,
         uncertainties are in parts per thousand.
 
         """
         # `band` should be 1, 2, 3, or 4.
-        df = bandpass_data_frame ('filter_wise_' + str (band) + '.dat', 'wlen resp uncert')
+        df = bandpass_data_frame('filter_wise_' + str(band) + '.dat', 'wlen resp uncert')
         df.wlen *= 1e4 # micron to Angstrom
         df.uncert *= df.resp / 1000. # parts per thou. to absolute values.
         lo, hi = self._filter_subsets[band]
         df = df[lo:hi] # clip zero parts of response.
         return df
 
     _zeropoints = {
@@ -936,27 +947,27 @@
         # corrections are necessary for sources with unusual spectra.
         1: 309.540,
         2: 171.787,
         3: 31.674,
         4: 8.363,
     }
 
-    def mag_to_fnu (self, mag):
+    def mag_to_fnu(self, mag):
         return cgs.cgsperjy * self._zeropoints[self.band] * 10**(-0.4 * mag)
 
 
-def register_wise (reg):
-    reg.register_bpass ('WISE', WiseBandpass)
+def register_wise(reg):
+    reg.register_bpass('WISE', WiseBandpass)
 
     # I computed these myself from the per-energy response curves.
-    reg.register_pivot_wavelength ('WISE', 1, 33682.)
-    reg.register_pivot_wavelength ('WISE', 2, 46179.)
-    reg.register_pivot_wavelength ('WISE', 3, 120731.)
-    reg.register_pivot_wavelength ('WISE', 4, 221942.)
+    reg.register_pivot_wavelength('WISE', 1, 33682.)
+    reg.register_pivot_wavelength('WISE', 2, 46179.)
+    reg.register_pivot_wavelength('WISE', 3, 120731.)
+    reg.register_pivot_wavelength('WISE', 4, 221942.)
 
     # Ditto.
-    reg.register_halfmaxes ('WISE', 1, 31476., 37834.)
-    reg.register_halfmaxes ('WISE', 2, 40906., 51980.)
-    reg.register_halfmaxes ('WISE', 3, 100777., 163535.)
-    reg.register_halfmaxes ('WISE', 4, 198530., 245927.)
+    reg.register_halfmaxes('WISE', 1, 31476., 37834.)
+    reg.register_halfmaxes('WISE', 2, 40906., 51980.)
+    reg.register_halfmaxes('WISE', 3, 100777., 163535.)
+    reg.register_halfmaxes('WISE', 4, 198530., 245927.)
 
 builtin_registrars['WISE'] = register_wise
```

### Comparing `pwkit-0.8.9/pwkit/cli/multitool.py` & `pwkit-1.0.0/pwkit/cli/multitool.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/cli/__init__.py` & `pwkit-1.0.0/pwkit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/cli/astrotool.py` & `pwkit-1.0.0/pwkit/cli/astrotool.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,15 +383,16 @@
 class Summfits (multitool.Command):
     name = 'summfits'
     argspec = '<path>'
     summary = 'Summarize contents of a FITS file.'
 
     _commentary_card_names = frozenset (('HISTORY', 'COMMENT'))
     _skip_headers = frozenset (('XTENSION', 'BITPIX', 'SIMPLE', 'EXTEND',
-                                'EXTNAME', 'PCOUNT', 'GCOUNT', 'TFIELDS'))
+                                'EXTNAME', 'PCOUNT', 'GCOUNT', 'TFIELDS',
+                                '')) # <= STScI FITS files can use blank keys for spacing
     _skip_prefixes = frozenset (('NAXIS', 'TTYPE', 'TFORM', 'TDIM', 'TUNIT'))
 
     def invoke (self, args, **kwargs):
         if len (args) != 1:
             raise multitool.UsageError ('summfits expected 1 argument')
 
         try:
@@ -437,23 +438,24 @@
 
             output (1, 'HDU %*d = %*s: kind=%s size=%d ver=%s level=%s',
                     hduidxwidth, hduidx, hdunamewidth, hdu.name, kind, hdu.size,
                     hdu.ver, hdu.level)
 
             output (2, '%d headers (some omitted)', len (hdu.header))
 
-            for k in hdu.header.keys ():
+            for k, value, comment in hdu.header.cards:
                 if k in self._commentary_card_names or k in self._skip_headers:
                     continue
+
                 for pfx in self._skip_prefixes:
-                    if k.startswith (pfx):
+                    if k.startswith(pfx):
                         break
                 else:
                     # We did not break out of the loop -> shouldn't be skipped.
-                    output (3, '%-8s = %r # %s', k, hdu.header[k], hdu.header.comments[k])
+                    output(3, '%-8s = %r # %s', k, value, comment)
 
             for ck in self._commentary_card_names:
                 # hacky linewrapping logic here
                 if ck not in hdu.header:
                     continue
 
                 buf = ''
```

### Comparing `pwkit-0.8.9/pwkit/cli/wrapout.py` & `pwkit-1.0.0/pwkit/cli/wrapout.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright 2014-2015 Peter Williams <peter@newton.cx> and collaborators
 # Licensed under the MIT License.
 
 """pwkit.cli.wrapout - the 'wrapout' program."""
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('commandline').split ()
+__all__ = str('commandline').split()
 
 import os, signal, sys, time
 
 from . import die, propagate_sigint
 
 usage = """usage: wrapout [-ces] [-a name] <command> [command args...]
 
@@ -64,235 +64,237 @@
 
 
 from ..io import get_stdout_bytes, get_stderr_bytes
 binary_stdout = get_stdout_bytes()
 binary_stderr = get_stderr_bytes()
 
 
-class Wrapper (object):
+class Wrapper(object):
     # I like !! for errors and ** for info, but those are nigh-un-grep-able.
     markers = [b' -- ', b' EE ', b' II ']
     use_colors = False
     echo_stderr = False
     propagate_signals = False
     destination = None
     slurp_factory = None
 
     _red = b''
     _cyan = b''
     _bold = b''
     _reset = b''
     _kind_prefixes = [b'', b'', b'']
 
-    def __init__ (self, destination=None):
+    def __init__(self, destination=None):
         if destination is None:
             self.destination = binary_stdout
         else:
             self.destination = destination
 
 
-    def output (self, kind, line):
+    def output(self, kind, line):
+        "*line* should be bytes"
         self.destination.write(b''.join([
             self._cyan,
-            b't=%07d' % (time.time () - self._t0),
+            b't=%07d' % (time.time() - self._t0),
             self._reset,
             self._kind_prefixes[kind],
             self.markers[kind],
             line,
             self._reset,
         ]))
-        self.destination.flush ()
+        self.destination.flush()
 
 
-    def output_stderr (self, text):
+    def output_stderr(self, text):
+        "*text* should be bytes"
         binary_stderr.write(b''.join([
             self._red,
-            b't=%07d' % (time.time () - self._t0),
+            b't=%07d' % (time.time() - self._t0),
             self._reset,
-            ' ',
+            b' ',
             text,
         ]))
-        binary_stderr.flush ()
+        binary_stderr.flush()
 
 
-    def outpar (self, name, value):
-        line = ('%s = %s\n' % (name, value)).encode ('utf-8')
-        self.output (OUTKIND_EXTRA, line)
+    def outpar(self, name, value):
+        line = ('%s = %s\n' % (name, value)).encode('utf-8')
+        self.output(OUTKIND_EXTRA, line)
 
 
-    def launch (self, cmd, argv, env=None, cwd=None):
+    def launch(self, cmd, argv, env=None, cwd=None):
         slurp_factory = self.slurp_factory
         if slurp_factory is None:
             from ..slurp import Slurper as slurp_factory
 
         if self.use_colors:
             self._red = ansi_red
             self._cyan = ansi_cyan
             self._bold = ansi_bold
             self._reset = ansi_reset
-            self._kind_prefixes = ['', self._red, self._bold]
+            self._kind_prefixes = [b'', self._red, self._bold]
 
-        self._t0 = time.time ()
-        self.outpar ('start_time', time.strftime (rfc3339_fmt))
-        self.outpar ('exec', cmd)
-        self.outpar ('argv', ' '.join (repr (s) for s in argv))
+        self._t0 = time.time()
+        self.outpar('start_time', time.strftime(rfc3339_fmt))
+        self.outpar('exec', cmd)
+        self.outpar('argv', ' '.join(repr(s) for s in argv))
 
         midline_kind = None
         stderr_midline = False
 
-        with slurp_factory (argv=argv, executable=cmd, env=env, cwd=cwd,
-                            propagate_signals=self.propagate_signals) as slurp:
+        with slurp_factory(argv=argv, executable=cmd, env=env, cwd=cwd,
+                           propagate_signals=self.propagate_signals) as slurp:
             # Here's where we get tricky since we want to output partially
             # complete lines, but we may have to switch between different
             # types of output or informational messages.
 
             for etype, data in slurp:
                 if etype == 'forwarded-signal':
-                    if self.midline_kind is not None:
-                        self.destination.write (b'\n')
+                    if midline_kind is not None:
+                        self.destination.write(b'\n')
                         midline_kind = None
-                    self.output (OUTKIND_EXTRA, 'forwarded signal %d to child\n' % data)
+                    self.output(OUTKIND_EXTRA, b'forwarded signal %d to child\n' % data)
                 elif etype in ('stdout', 'stderr'):
-                    if not len (data):
+                    if not len(data):
                         continue # EOF, nothing for us to do.
 
                     kind = OUTKIND_STDERR if etype == 'stderr' else OUTKIND_STDOUT
 
                     if midline_kind is not None and midline_kind != kind:
-                        self.destination.write (b'\n')
+                        self.destination.write(b'\n')
                         midline_kind = None
 
-                    lines = data.split (b'\n')
+                    lines = data.split(b'\n')
 
                     if midline_kind is None:
-                        self.output (kind, lines[0]) # start a new line
+                        self.output(kind, lines[0]) # start a new line
                     else:
                         # If we're here, we must be continuing a line
-                        self.destination.write (lines[0])
+                        self.destination.write(lines[0])
 
                     for line in lines[1:-1]:
                         # mid-lines are straightforward
-                        self.destination.write (b'\n')
-                        self.output (kind, line)
+                        self.destination.write(b'\n')
+                        self.output(kind, line)
 
-                    if len (lines) == 1:
-                        self.destination.flush ()
+                    if len(lines) == 1:
+                        self.destination.flush()
                         midline_kind = kind
-                    elif not len (lines[-1]):
+                    elif not len(lines[-1]):
                         # We ended right on a newline, which is convenient.
-                        self.destination.write (b'\n')
-                        self.destination.flush ()
+                        self.destination.write(b'\n')
+                        self.destination.flush()
                         midline_kind = None
                     else:
                         # We ended with a partial line.
-                        self.destination.write (b'\n')
-                        self.output (kind, lines[-1])
+                        self.destination.write(b'\n')
+                        self.output(kind, lines[-1])
                         midline_kind = kind
 
                     if self.echo_stderr and kind == OUTKIND_STDERR:
                         # We use a different format since the intended usage
                         # is that the main output is being logged elsewhere;
                         # this should be terser and distinguishable from the
                         # stdout output.
                         if stderr_midline:
-                            binary_stderr.write (lines[0])
+                            binary_stderr.write(lines[0])
                         else:
-                            self.output_stderr (lines[0])
+                            self.output_stderr(lines[0])
 
                         for line in lines[1:-1]:
-                            binary_stderr.write (b'\n')
-                            self.output_stderr (line)
+                            binary_stderr.write(b'\n')
+                            self.output_stderr(line)
 
-                        if len (lines) == 1:
-                            binary_stderr.flush ()
+                        if len(lines) == 1:
+                            binary_stderr.flush()
                             stderr_midline = True
-                        elif not len (lines[-1]):
-                            binary_stderr.write (b'\n')
-                            binary_stderr.flush ()
+                        elif not len(lines[-1]):
+                            binary_stderr.write(b'\n')
+                            binary_stderr.flush()
                             stderr_midline = False
                         else:
-                            binary_stderr.write (b'\n')
-                            self.output_stderr (lines[-1])
+                            binary_stderr.write(b'\n')
+                            self.output_stderr(lines[-1])
                             stderr_midline = True
 
-        self.outpar ('finish_time', time.strftime (rfc3339_fmt))
-        self.outpar ('elapsed_seconds', int (round (time.time () - self._t0)))
-        self.outpar ('exitcode', slurp.proc.returncode)
+        self.outpar('finish_time', time.strftime(rfc3339_fmt))
+        self.outpar('elapsed_seconds', int(round(time.time() - self._t0)))
+        self.outpar('exitcode', slurp.proc.returncode)
 
         # note: subprocess pre-processes exit codes, so shouldn't use
         # os.WIFSIGNALED, os.WTERMSIG, etc.
 
         if slurp.proc.returncode < 0:
             signum = -slurp.proc.returncode
-            self.output (OUTKIND_STDERR,
-                         b'process killed by signal %d\n' % signum)
+            self.output(OUTKIND_STDERR,
+                        b'process killed by signal %d\n' % signum)
 
             if self.propagate_signals:
-                signal.signal (signum, signal.SIG_DFL)
-                os.kill (os.getpid (), signum) # sayonara
+                signal.signal(signum, signal.SIG_DFL)
+                os.kill(os.getpid(), signum) # sayonara
         elif slurp.proc.returncode != 0:
-            self.output (OUTKIND_STDERR, b'process exited with error code\n')
+            self.output(OUTKIND_STDERR, b'process exited with error code\n')
 
         return slurp.proc.returncode
 
 
-def commandline (argv=None):
+def commandline(argv=None):
     if argv is None:
         argv = sys.argv
 
     # NOTE: we do NOT initialize stdout and stderr to be Unicode streams
     # since we're actually intentionally writing raw bytes to them.
-    propagate_sigint ()
+    propagate_sigint()
 
-    args = list (argv[1:])
+    args = list(argv[1:])
     use_colors = None
     echo_stderr = False
     propagate_signals = True
     argv0 = None
 
-    while len (args):
+    while len(args):
         if args[0] == '-c':
             use_colors = True
             args = args[1:]
         elif args[0] == '-e':
             echo_stderr = True
             args = args[1:]
         elif args[0] == '-s':
             propagate_signals = False
             args = args[1:]
         elif args[0] == '-a':
-            if len (args) < 2:
-                die ('another argument must come after the "-a" option')
+            if len(args) < 2:
+                die('another argument must come after the "-a" option')
             argv0 = args[1]
             args = args[2:]
         elif args[0] == '--':
             args = args[1:]
             break
         elif args[0][0] == '-':
-            die ('unrecognized option "%s"', args[0])
+            die('unrecognized option "%s"', args[0])
         else:
             # End of option arguments.
             break
 
-    if len (args) < 1:
-        print (usage.strip (), file=sys.stderr)
-        sys.exit (0)
+    if len(args) < 1:
+        print(usage.strip(), file=sys.stderr)
+        sys.exit(0)
 
     subcommand = args[0]
     subargv = args
     if argv0 is not None:
         subargv[0] = argv0
 
     if use_colors is None:
-        use_colors = binary_stdout.isatty ()
+        use_colors = binary_stdout.isatty()
 
-    wrapper = Wrapper ()
+    wrapper = Wrapper()
     wrapper.use_colors = use_colors
     wrapper.echo_stderr = echo_stderr
     wrapper.propagate_signals = propagate_signals
-    sys.exit (wrapper.launch (subcommand, subargv))
+    sys.exit(wrapper.launch(subcommand, subargv))
 
 
 if __name__ == '__main__':
     # Note that the standard wrapper created by setup.py does not actually
     # follow this code path! It invokes commandline() directly.
-    commandline ()
+    commandline()
```

### Comparing `pwkit-0.8.9/pwkit/cli/imtool.py` & `pwkit-1.0.0/pwkit/cli/imtool.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/cli/latexdriver.py` & `pwkit-1.0.0/pwkit/cli/latexdriver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,212 +1,216 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2014-2016 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2014-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """pwkit.cli.latexdriver - the 'latexdriver' program.
 
 This used to be a nice little shell script, but for portability it's better to
 do this in Python. And now we can optionally provide some BibTeX-related
 magic.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('commandline').split ()
+__all__ = 'commandline'.split()
 
 import signal, six, subprocess, sys
 from six.moves import range
 
 from .. import PKError
 from ..io import Path
 from . import *
 
 
 # This batch of code implements the magic BibTeX merging feature.
 
-def cited_names_from_aux_file (stream):
+def cited_names_from_aux_file(stream):
     """Parse a LaTeX ".aux" file and generate a list of names cited according to
     LaTeX ``\\citation`` commands. Repeated names are generated only once. The
     argument should be a opened I/O stream.
 
     """
-    cited = set ()
+    cited = set()
 
     for line in stream:
-        if not line.startswith (r'\citation{'):
+        if not line.startswith(r'\citation{'):
             continue
 
-        line = line.rstrip ()
+        line = line.rstrip()
         if line[-1] != '}':
             continue # should issue a warning or something
 
         entries = line[10:-1]
 
-        for name in entries.split (','):
-            name = name.strip ()
+        for name in entries.split(','):
+            name = name.strip()
 
             if name not in cited:
                 yield name
-                cited.add (name)
+                cited.add(name)
 
 
-def merge_bibtex_collections (citednames, maindict, extradicts, allow_missing=False):
+def merge_bibtex_collections(citednames, maindict, extradicts, allow_missing=False):
     """There must be a way to be efficient and stream output instead of loading
     everything into memory at once, but, meh.
 
     Note that we augment `citednames` with all of the names in `maindict`. The
     intention is that if we've gone to the effort of getting good data for
     some record, we don't want to trash it if the citation is temporarily
     removed (even if it ought to be manually recoverable from version
     control). Seems better to err on the side of preservation; I can write a
     quick pruning tool later if needed.
 
     """
     allrecords = {}
 
     for ed in extradicts:
-        allrecords.update (ed)
+        allrecords.update(ed)
 
-    allrecords.update (maindict)
+    allrecords.update(maindict)
 
     missing = []
     from collections import OrderedDict
-    records = OrderedDict ()
+    records = OrderedDict()
     from itertools import chain
-    wantednames = sorted (chain (citednames, six.viewkeys (maindict)))
+    wantednames = sorted(chain(citednames, six.viewkeys(maindict)))
 
     for name in wantednames:
-        rec = allrecords.get (name)
+        rec = allrecords.get(name)
         if rec is None:
-            missing.append (name)
+            missing.append(name)
         else:
             records[name] = rec
 
-    if len (missing) and not allow_missing:
+    if len(missing) and not allow_missing:
         # TODO: custom exception so caller can actually see what's missing;
         # could conceivably stub out missing records or something.
-        raise PKError ('missing BibTeX records: %s', ' '.join (missing))
+        raise PKError('missing BibTeX records: %s', ' '.join(missing))
 
     return records
 
 
-def get_bibtex_dict (stream):
+def get_bibtex_dict(stream):
     from bibtexparser.bparser import BibTexParser
-    parser = BibTexParser ()
+    parser = BibTexParser()
     parser.ignore_nonstandard_types = False
     parser.homogenise_fields = False
 
     # TODO: one bit of homogenization that might be nice: it seems that
     # newlines get preserved, in `author` records at least. Those should be
     # replaced with spaces (and multiple spaces collapsed if needed).
 
-    return parser.parse_file (stream).get_entry_dict ()
+    return parser.parse_file(stream).get_entry_dict()
 
 
-def write_bibtex_dict (stream, entries):
+def write_bibtex_dict(stream, entries):
     """bibtexparser.write converts the entire database to one big string and
     writes it out in one go. I'm sure it will always all fit in RAM but some
     things just will not stand.
 
     """
     from bibtexparser.bwriter import BibTexWriter
 
-    writer = BibTexWriter ()
+    writer = BibTexWriter()
     writer.indent = '  '
     writer.entry_separator = ''
     first = True
 
     for rec in entries:
         if first:
             first = False
         else:
-            stream.write (b'\n')
-        stream.write (writer._entry_to_bibtex (rec).encode('utf8'))
+            stream.write(b'\n')
+        stream.write(writer._entry_to_bibtex(rec).encode('utf8'))
 
 
-def merge_bibtex_with_aux (auxpath, mainpath, extradir, parse=get_bibtex_dict, allow_missing=False):
+def merge_bibtex_with_aux(auxpath, mainpath, extradir, parse=get_bibtex_dict, allow_missing=False):
     """Merge multiple BibTeX files into a single homogeneously-formatted output,
     using a LaTeX .aux file to know which records are worth paying attention
     to.
 
     The file identified by `mainpath` will be overwritten with the new .bib
     contents. This function is intended to be used in a version-control
     context.
 
     Files matching the glob "*.bib" in `extradir` will be read in to
     supplement the information in `mainpath`. Records already in the file in
     `mainpath` always take precedence.
 
     """
-    auxpath = Path (auxpath)
-    mainpath = Path (mainpath)
-    extradir = Path (extradir)
+    auxpath = Path(auxpath)
+    mainpath = Path(mainpath)
+    extradir = Path(extradir)
+
+    with auxpath.open('rt') as aux:
+        citednames = sorted(cited_names_from_aux_file(aux))
+
+    main = mainpath.try_open(mode='rt')
+    if main is None:
+        maindict = {}
+    else:
+        maindict = parse(main)
+        main.close()
 
-    with auxpath.open ('rt') as aux:
-        citednames = sorted (cited_names_from_aux_file (aux))
-
-    with mainpath.try_open (mode='rt', null_if_noexist=True) as main:
-        maindict = parse (main)
-
-    def gen_extra_dicts ():
+    def gen_extra_dicts():
         # If extradir does not exist, Path.glob() will return an empty list,
         # which seems acceptable to me.
-        for item in sorted (extradir.glob ('*.bib')):
-            with item.open ('rt') as extra:
-                yield parse (extra)
+        for item in sorted(extradir.glob('*.bib')):
+            with item.open('rt') as extra:
+                yield parse(extra)
 
-    merged = merge_bibtex_collections (citednames, maindict, gen_extra_dicts (),
-                                       allow_missing=allow_missing)
+    merged = merge_bibtex_collections(citednames, maindict, gen_extra_dicts(),
+                                      allow_missing=allow_missing)
 
-    with mainpath.make_tempfile (want='handle', resolution='overwrite') as newbib:
-        write_bibtex_dict (newbib, six.viewvalues (merged))
+    with mainpath.make_tempfile(want='handle', resolution='overwrite') as newbib:
+        write_bibtex_dict(newbib, six.viewvalues(merged))
 
 
 # This batch of code implements the filename-recorder-to-Makefile magic.
 
-def convert_fls_to_makefile (flspath, finalpath, prefix, replacement, work, mfpath, foreign_deps_ok):
+def convert_fls_to_makefile(flspath, finalpath, prefix, replacement, work, mfpath, foreign_deps_ok):
     texpwd = None
 
-    with flspath.open ('rt') as fls, mfpath.open ('wt') as mf:
-        mf.write (six.text_type (finalpath))
-        mf.write (':')
+    with flspath.open('rt') as fls, mfpath.open('wt') as mf:
+        mf.write(six.text_type(finalpath))
+        mf.write(':')
 
         for line in fls:
-            kind, path = line.strip ().split (None, 1)
-            path = Path (path)
+            kind, path = line.strip().split(None, 1)
+            path = Path(path)
 
             if kind == 'PWD':
                 texpwd = path # this is always the first line
                 if prefix is not None:
-                    r_prefix = six.text_type ((texpwd / prefix).resolve ())
-                r_work = six.text_type ((texpwd / work).resolve ())
+                    r_prefix = six.text_type((texpwd / prefix).resolve())
+                r_work = six.text_type((texpwd / work).resolve())
 
             if kind != 'INPUT':
                 continue
 
             # properly handles absolute and relative `path`:
-            r_full = six.text_type ((texpwd / path).resolve ())
+            r_full = six.text_type((texpwd / path).resolve())
 
-            if r_full.startswith (r_work):
+            if r_full.startswith(r_work):
                 continue # ignore .bbl, etc
 
             if prefix is not None:
-                if r_full.startswith (r_prefix):
-                    r_full = r_full[len (r_prefix) + 1:]
+                if r_full.startswith(r_prefix):
+                    r_full = r_full[len(r_prefix) + 1:]
 
                     if replacement is not None:
                         r_full = replacement + r_full
                 elif not foreign_deps_ok:
-                    warn ('unexpected dependent file path %r' % r_full)
+                    warn('unexpected dependent file path %r' % r_full)
                     continue
 
-            mf.write (' ')
-            mf.write (r_full)
+            mf.write(' ')
+            mf.write(r_full)
 
-        mf.write ('\n')
+        mf.write('\n')
 
 
 # The actual command-line program
 
 usage = """latexdriver [-lAxbBRq] [-eSTYLE] [-ESTYLE] [-M<args>] input.tex output.pdf
 
 Drive (xe)latex sensibly. Create output.pdf from input.tex, rerunning as
@@ -233,262 +237,267 @@
 default_args = ['-interaction', 'nonstopmode',
                 '-halt-on-error',
                 '-file-line-error']
 
 max_iterations = 10
 
 
-def logrun (command, boring_args, interesting_arg, logpath, quiet=False, reckless=False):
+def logrun(command, boring_args, interesting_arg, logpath, quiet=False, reckless=False):
     if not quiet:
-        if len (boring_args):
-            print ('+', command, '...', interesting_arg)
+        if len(boring_args):
+            print('+', command, '...', interesting_arg)
         else:
-            print ('+', command, interesting_arg)
+            print('+', command, interesting_arg)
 
     argv = [command] + boring_args + [interesting_arg]
 
     try:
-        with logpath.open ('wb') as f:
-            print ('## running:', ' '.join (argv), file=f)
-            f.flush ()
-            subprocess.check_call (argv, stdout=f, stderr=f)
+        with logpath.open('wb') as f:
+            print('## running:', ' '.join(argv), file=f)
+            f.flush()
+            subprocess.check_call(argv, stdout=f, stderr=f)
     except subprocess.CalledProcessError as e:
         if quiet:
-            print ('ran:', ' '.join (argv), file=sys.stderr)
+            print('ran:', ' '.join(argv), file=sys.stderr)
 
-        with logpath.open ('rt') as f:
+        with logpath.open('rt') as f:
             for line in f:
-                print (line, end='', file=sys.stderr)
-        print (file=sys.stderr)
+                print(line, end='', file=sys.stderr)
+        print(file=sys.stderr)
 
         if e.returncode == -signal.SIGINT:
-            raise KeyboardInterrupt () # make sure to propagate SIGINT
+            raise KeyboardInterrupt() # make sure to propagate SIGINT
 
         if e.returncode > 0:
-            msg = 'command "%s" failed with exit status %d' % (' '.join (argv),
+            msg = 'command "%s" failed with exit status %d' % (' '.join(argv),
                                                                e.returncode)
         else:
-            msg = 'command "%s" killed by signal %d' % (' '.join (argv),
+            msg = 'command "%s" killed by signal %d' % (' '.join(argv),
                                                         -e.returncode)
 
         if reckless:
-            warn (msg + '; ignoring')
+            warn(msg + '; ignoring')
         else:
-            die (msg)
+            die(msg)
     except Exception:
         if quiet:
-            print ('ran:', ' '.join (argv), file=sys.stderr)
+            print('ran:', ' '.join(argv), file=sys.stderr)
         raise
 
 
-def bib_export (style, auxpath, bibpath, no_tool_ok=False, quiet=False, ignore_missing=False):
+def bib_export(style, auxpath, bibpath, no_tool_ok=False, quiet=False, ignore_missing=False):
     args = ['bib', 'btexport']
     if ignore_missing:
         args += ['-i']
     args += [style, str(auxpath)]
 
     if not quiet:
-        print ('+', ' '.join (args), '>' + str(bibpath))
+        print('+', ' '.join(args), '>' + str(bibpath))
 
     try:
-        with bibpath.open ('wb') as f:
-            subprocess.check_call (args, stdout=f)
+        with bibpath.open('wb') as f:
+            subprocess.check_call(args, stdout=f)
     except OSError as e:
         if e.errno == 2 and no_tool_ok:
-            bibpath.try_unlink ()
+            bibpath.try_unlink()
             return
         if quiet:
-            print ('ran:', ' '.join (args), file=sys.stderr)
+            print('ran:', ' '.join(args), file=sys.stderr)
         raise
     except subprocess.CalledProcessError as e:
         if quiet:
-            print ('ran:', ' '.join (args), file=sys.stderr)
+            print('ran:', ' '.join(args), file=sys.stderr)
         if e.returncode > 0:
-            die ('command "%s >%s" failed with exit status %d',
-                 ' '.join (args), bibpath, e.returncode)
+            die('command "%s >%s" failed with exit status %d',
+                ' '.join(args), bibpath, e.returncode)
         elif e.returncode == -signal.SIGINT:
-            raise KeyboardInterrupt () # make sure to propagate SIGINT
+            raise KeyboardInterrupt() # make sure to propagate SIGINT
         else:
-            die ('command "%s >%s" killed by signal %d',
-                 ' '.join (args), bibpath, -e.returncode)
+            die('command "%s >%s" killed by signal %d',
+                ' '.join(args), bibpath, -e.returncode)
 
 
-def just_smart_bibtools(bib_style, aux):
+def just_smart_bibtools(bib_style, aux, bib):
     """Tectonic has taken over most of the features that this tool used to provide,
     but here's a hack to keep my smart .bib file generation working.
 
     """
-    assert aux.endswith('.aux')
-    bib = aux[:-4] + '.bib'
+    extradir = Path('.bibtex')
+    extradir.ensure_dir(parents=True)
 
-    extradir = Path ('.bibtex')
-    extradir.ensure_dir (parents=True)
+    bib_export(bib_style, aux, extradir / 'ZZ_bibtools.bib',
+               no_tool_ok=True, quiet=True, ignore_missing=True)
+    merge_bibtex_with_aux(aux, bib, extradir)
 
-    bib_export (bib_style, aux, extradir / 'ZZ_bibtools.bib',
-                no_tool_ok=True, quiet=True, ignore_missing=True)
-    merge_bibtex_with_aux (aux, bib, extradir)
 
-
-def commandline (argv=None):
+def commandline(argv=None):
     if argv is None:
         argv = sys.argv
-        propagate_sigint ()
-        unicode_stdio ()
+        propagate_sigint()
+        unicode_stdio()
 
-    check_usage (usage, argv, usageifnoargs='long')
+    check_usage(usage, argv, usageifnoargs='long')
 
     bib_style = None
     makefile_prefix = None
     makefile_replacement = None
     makefile_dest = None
     engine_args = default_args
     engine = 'pdflatex'
 
     # Hooray hack
 
     if argv[1] == '--just-smart-bibtools':
-        assert len(argv) == 4
-        bib_style = argv[2]
-        auxpath = argv[3]
-        just_smart_bibtools(bib_style, auxpath)
+        if len(argv) == 4:
+            bib_style = argv[2]
+            auxpath = argv[3]
+            assert auxpath.endswith('.aux')
+            bibpath = auxpath[:-4] + '.bib'
+        elif len(argv) == 5:
+            bib_style = argv[2]
+            auxpath = argv[3]
+            bibpath = argv[4]
+        else:
+            die('--just-smart-bibtools expects exactly 2 or 3 additional arguments')
+        just_smart_bibtools(bib_style, auxpath, bibpath)
         return
 
     # I should probably start using a real arg parser.
 
-    do_bibtex = pop_option ('b', argv)
-    do_smart_bibtex = pop_option ('B', argv)
-    do_xetex = pop_option ('x', argv)
-    do_letterpaper = pop_option ('l', argv)
-    do_a4paper = pop_option ('A', argv)
-    do_reckless = pop_option ('R', argv)
-    do_foreign_deps = pop_option ('f', argv)
-    quiet = pop_option ('q', argv)
+    do_bibtex = pop_option('b', argv)
+    do_smart_bibtex = pop_option('B', argv)
+    do_xetex = pop_option('x', argv)
+    do_letterpaper = pop_option('l', argv)
+    do_a4paper = pop_option('A', argv)
+    do_reckless = pop_option('R', argv)
+    do_foreign_deps = pop_option('f', argv)
+    quiet = pop_option('q', argv)
     do_smart_bibtools = False
 
-    for i in range (1, len (argv)):
-        if argv[i].startswith ('-e') or argv[i].startswith ('-E'):
-            do_smart_bibtools = argv[i].startswith ('-E')
+    for i in range(1, len(argv)):
+        if argv[i].startswith('-e') or argv[i].startswith('-E'):
+            do_smart_bibtools = argv[i].startswith('-E')
             bib_style = argv[i][2:]
             del argv[i]
             break
 
-    for i in range (1, len (argv)):
-        if argv[i].startswith ('-M'):
-            pieces = argv[i][2:].split (',', 2)
-            if len (pieces) == 2:
+    for i in range(1, len(argv)):
+        if argv[i].startswith('-M'):
+            pieces = argv[i][2:].split(',', 2)
+            if len(pieces) == 2:
                 makefile_prefix, makefile_dest = pieces
-            elif len (pieces) == 3:
+            elif len(pieces) == 3:
                 makefile_prefix, makefile_replacement, makefile_dest = pieces
             else:
-                wrong_usage (usage, 'could not parse -M argument')
+                wrong_usage(usage, 'could not parse -M argument')
             del argv[i]
             break
 
-    if len (argv) != 3:
-        wrong_usage (usage, 'expect exactly 2 non-option arguments')
+    if len(argv) != 3:
+        wrong_usage(usage, 'expect exactly 2 non-option arguments')
 
     if do_letterpaper and do_a4paper:
-        wrong_usage (usage, 'only one of "-l" and "-A" may be specified')
+        wrong_usage(usage, 'only one of "-l" and "-A" may be specified')
 
-    input = Path (argv[1])
-    output = Path (argv[2])
+    input = Path(argv[1])
+    output = Path(argv[2])
 
     if do_smart_bibtools:
         do_smart_bibtex = True
     if bib_style is not None or do_smart_bibtex:
         do_bibtex = True
     if do_xetex:
         engine = 'xelatex'
     if do_letterpaper:
         engine_args += ['-papersize', 'letter']
     if do_a4paper:
         engine_args += ['-papersize', 'A4']
     if makefile_dest is not None:
         engine_args += ['-recorder']
 
-    if not input.exists ():
-        die ('input "%s" does not exist', input)
+    if not input.exists():
+        die('input "%s" does not exist', input)
 
     base = input.stem
-    if not len (base):
-        die ('failed to strip extension from input path "%s"', input)
+    if not len(base):
+        die('failed to strip extension from input path "%s"', input)
 
     # I stash the annoying LaTeX output files in a hidden directory called
     # .latexwork. However, some LaTeX distributions refuse to write to hidden
     # paths by default. I figured out how to hack the configuration, but
     # that's not a scalable solution. Instead I just create a temporary
     # symlink with an acceptable name -- good jorb security.
-    workdir = input.with_name ('.latexwork')
-    workalias = input.with_name ('_latexwork')
+    workdir = input.with_name('.latexwork')
+    workalias = input.with_name('_latexwork')
 
-    workdir.ensure_dir (parents=True)
-    workalias.rellink_to (workdir, force=True)
+    workdir.ensure_dir(parents=True)
+    workalias.rellink_to(workdir, force=True)
 
     job = workalias / base
     tlog = workalias / (base + '.hllog')
     blog = workalias / (base + '.hlblg')
     engine_args += ['-jobname', str(job)]
 
     try:
-        logrun (engine, engine_args, base, tlog, quiet=quiet)
+        logrun(engine, engine_args, base, tlog, quiet=quiet)
 
         if do_bibtex:
-            bib = input.with_suffix ('.bib')
-            aux = job.with_suffix ('.aux')
+            bib = input.with_suffix('.bib')
+            aux = job.with_suffix('.aux')
 
             if do_smart_bibtex:
-                extradir = input.with_name ('.bibtex')
+                extradir = input.with_name('.bibtex')
 
                 if bib_style is not None:
-                    extradir.ensure_dir (parents=True)
-                    bib_export (bib_style, aux, extradir / 'ZZ_bibtools.bib',
-                                no_tool_ok=True, quiet=quiet, ignore_missing=True)
+                    extradir.ensure_dir(parents=True)
+                    bib_export(bib_style, aux, extradir / 'ZZ_bibtools.bib',
+                               no_tool_ok=True, quiet=quiet, ignore_missing=True)
 
                 if not quiet:
-                    print ('+', '(generate and normalize)', bib)
-                merge_bibtex_with_aux (aux, bib, extradir)
+                    print('+', '(generate and normalize)', bib)
+                merge_bibtex_with_aux(aux, bib, extradir)
             elif bib_style is not None:
-                bib_export (bib_style, aux, bib, quiet=quiet)
+                bib_export(bib_style, aux, bib, quiet=quiet)
 
-            job.with_suffix ('.bib').rellink_to (bib, force=True)
-            logrun ('bibtex', [], str(job), blog, reckless=do_reckless, quiet=quiet)
+            job.with_suffix('.bib').rellink_to(bib, force=True)
+            logrun('bibtex', [], str(job), blog, reckless=do_reckless, quiet=quiet)
 
-            with blog.open ('rt') as f:
+            with blog.open('rt') as f:
                 for line in f:
                     if 'Warning' in line:
-                        print (line, end='', file=sys.stderr)
+                        print(line, end='', file=sys.stderr)
 
             # force at least one extra run:
-            logrun (engine, engine_args, base, tlog, quiet=quiet)
+            logrun(engine, engine_args, base, tlog, quiet=quiet)
 
-        for _ in range (max_iterations):
+        for _ in range(max_iterations):
             keepgoing = False
 
             # longtables seem to always tell you to rerun latex. Stripping out
             # lines containing "longtable" makes us ignore these prompts.
-            with tlog.open ('rt') as f:
+            with tlog.open('rt') as f:
                 for line in f:
                     if 'longtable' in line:
                         continue
                     if 'Rerun' in line:
                         keepgoing = True
                         break
 
             if not keepgoing:
                 break
 
-            logrun (engine, engine_args, base, tlog, quiet=quiet)
+            logrun(engine, engine_args, base, tlog, quiet=quiet)
         else:
             # we didn't break out of the loop -- ie hit max_iterations
-            die ('too many iterations; check "%s"', tlog)
+            die('too many iterations; check "%s"', tlog)
 
-        job.with_suffix ('.pdf').rename (output)
+        job.with_suffix('.pdf').rename(output)
 
         if makefile_dest is not None:
-            convert_fls_to_makefile (job.with_suffix ('.fls'), output,
-                                     Path (makefile_prefix),
-                                     makefile_replacement,
-                                     workalias,
-                                     Path (makefile_dest),
-                                     do_foreign_deps)
+            convert_fls_to_makefile(job.with_suffix('.fls'), output,
+                                    Path(makefile_prefix),
+                                    makefile_replacement,
+                                    workalias,
+                                    Path(makefile_dest),
+                                    do_foreign_deps)
     finally:
-        workalias.unlink ()
+        workalias.unlink()
```

### Comparing `pwkit-0.8.9/pwkit/ninja_syntax.py` & `pwkit-1.0.0/pwkit/ninja_syntax.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/__init__.py` & `pwkit-1.0.0/pwkit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2014-2016 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2014-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """A toolkit for science and astronomy in Python.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-# In Python 2, the items in __all__ should be bytes strings. In Python 3, they
-# should be Unicode. (http://stackoverflow.com/a/19913680/3760486) If you
-# don't use __future__.unicode_literals, you can just write `__all__ =
-# ["foo"]` and it's fine, but we do, which causes problems on Py 2.
-# Fortunately, to work on both cases we just need to do this:
-__all__ = str ('''Holder PKError binary_type reraise_context text_type unicode_to_str''').split ()
+__all__ = 'Holder PKError binary_type reraise_context text_type unicode_to_str'.split()
 
-__version__ = '0.8.9' # also edit ../setup.py, ../docs/source/conf.py!
+__version__ = '1.0.0' # also edit ../setup.py, ../docs/source/conf.py!
 
 # Simultaneous Python 2/3 compatibility through the 'six' module. I started
 # out hoping that I could do this all "in-house" without adding the dep, but
 # it became clear that 'six' was going to end up being helpful.
 
 import six
 from six import binary_type, text_type
 
 if six.PY2:
-    unicode_to_str = lambda s: s.__unicode__ ().encode ('utf8')
+    unicode_to_str = lambda s: s.__unicode__().encode('utf8')
 else:
-    unicode_to_str = lambda s: s.__unicode__ ()
+    unicode_to_str = lambda s: s.__unicode__()
 
 
-class PKError (Exception):
+class PKError(Exception):
     """A generic base class for exceptions.
 
     All custom exceptions raised by :mod:`pwkit` modules should be subclasses
     of this class.
 
     The constructor automatically applies old-fashioned ``printf``-like
     (``%``-based) string formatting if more than one argument is given::
 
-      PKError ('my format string says %r, %d', myobj, 12345)
+      PKError('my format string says %r, %d', myobj, 12345)
       # has text content equal to:
       'my format string says %r, %d' % (myobj, 12345)
 
     If only a single argument is given, the exception text is its
     stringification without applying ``printf``-style formatting.
 
     """
-    def __init__ (self, fmt, *args):
-        if not len (args):
-            self.args = (text_type (fmt), )
+    def __init__(self, fmt, *args):
+        if not len(args):
+            self.args = (text_type(fmt), )
         else:
-            self.args = (text_type (fmt) % args, )
+            self.args = (text_type(fmt) % args, )
 
-    def __unicode__ (self):
+    def __unicode__(self):
         return self.args[0]
 
     __str__ = unicode_to_str
 
-    def __repr__ (self):
-        return 'PKError(' + repr (self.args[0]) + ')'
+    def __repr__(self):
+        return 'PKError(' + repr(self.args[0]) + ')'
 
 
-def reraise_context (fmt, *args):
+def reraise_context(fmt, *args):
     """Reraise an exception with its message modified to specify additional
     context.
 
     This function tries to help provide context when a piece of code
     encounters an exception while trying to get something done, and it wishes
     to propagate contextual information farther up the call stack. It only
     makes sense in Python 2, which does not provide Python 3’s `exception
@@ -83,149 +78,149 @@
 
       from pwkit import reraise_context
       from pwkit.io import Path
 
       filename = 'my-filename.txt'
 
       try:
-        f = Path (filename).open ('rt')
-        for line in f.readlines ():
+        f = Path(filename).open('rt')
+        for line in f.readlines():
           # do stuff ...
       except Exception as e:
-        reraise_context ('while reading "%r"', filename)
+        reraise_context('while reading "%r"', filename)
         # The exception is reraised and so control leaves this function.
 
     If an exception with text ``"bad value"`` were to be raised inside the
     ``try`` block in the above example, its text would be modified to read
     ``"while reading \"my-filename.txt\": bad value"``.
 
     """
     import sys
 
-    if len (args):
+    if len(args):
         cstr = fmt % args
     else:
-        cstr = text_type (fmt)
+        cstr = text_type(fmt)
 
-    ex = sys.exc_info ()[1]
+    ex = sys.exc_info()[1]
 
-    if isinstance (ex, EnvironmentError):
+    if isinstance(ex, EnvironmentError):
         ex.strerror = '%s: %s' % (cstr, ex.strerror)
         ex.args = (ex.errno, ex.strerror)
     else:
-        if len (ex.args):
+        if len(ex.args):
             cstr = '%s: %s' % (cstr, ex.args[0])
         ex.args = (cstr, ) + ex.args[1:]
 
     raise
 
 
-class Holder (object):
+class Holder(object):
     """Create a new :class:`Holder`. Any keyword arguments will be assigned as
-    properties on the object itself, for instance, ``o = Holder (foo=1)``
+    properties on the object itself, for instance, ``o = Holder(foo=1)``
     yields an object such that ``o.foo`` is 1.
 
     The *__decorating* keyword is used to implement the :class:`Holder`
     decorator functionality, described below.
 
     """
-    def __init__ (self, __decorating=None, **kwargs):
+    def __init__(self, __decorating=None, **kwargs):
         import types
 
         if __decorating is None:
             values = kwargs
-        elif isinstance (__decorating, six.class_types):
+        elif isinstance(__decorating, six.class_types):
             # We're decorating a class definition. Transform the definition
             # into a Holder instance thusly:
-            values = dict (kv for kv in six.iteritems (__decorating.__dict__)
-                           if not kv[0].startswith ('__'))
+            values = dict(kv for kv in six.iteritems(__decorating.__dict__)
+                          if not kv[0].startswith('__'))
         else:
             # You could imagine allowing @Holder on a function and doing
             # something with its return value, but I can't think of a use that
             # would be more sensible than just creating and returning a Holder
             # directly.
-            raise ValueError ('unexpected use of Holder as a decorator (on %r)'
-                              % __decorating)
+            raise ValueError('unexpected use of Holder as a decorator (on %r)'
+                             % __decorating)
 
-        self.set (**values)
+        self.set(**values)
 
-    def __unicode__ (self):
+    def __unicode__(self):
         d = self.__dict__
-        s = sorted (six.iterkeys (d))
-        return '{' + ', '.join ('%s=%s' % (k, d[k]) for k in s) + '}'
+        s = sorted(six.iterkeys(d))
+        return u'{' + u', '.join(u'%s=%s' % (k, d[k]) for k in s) + u'}'
 
     __str__ = unicode_to_str
 
-    def __repr__ (self):
+    def __repr__(self):
         d = self.__dict__
-        s = sorted (six.iterkeys (d))
+        s = sorted(six.iterkeys(d))
         return '%s(%s)' % (self.__class__.__name__,
-                            ', '.join ('%s=%r' % (k, d[k]) for k in s))
+                            ', '.join('%s=%r' % (k, d[k]) for k in s))
 
-    def __iter__ (self):
-        return six.iteritems (self.__dict__)
+    def __iter__(self):
+        return six.iteritems(self.__dict__)
 
-    def __contains__ (self, key):
+    def __contains__(self, key):
         return key in self.__dict__
 
-    def set (self, **kwargs):
+    def set(self, **kwargs):
         """For each keyword argument, sets an attribute on this :class:`Holder` to its
         value.
 
         Equivalent to::
 
-          for key, value in kwargs.iteritems ():
-            setattr (self, key, value)
+          for key, value in kwargs.iteritems():
+            setattr(self, key, value)
 
         Returns *self*.
 
         """
-        self.__dict__.update (kwargs)
+        self.__dict__.update(kwargs)
         return self
 
-    def get (self, name, defval=None):
+    def get(self, name, defval=None):
         """Get an attribute on this :class:`Holder`.
 
-        Equivalent to ``getattr (self, name, defval)``.
+        Equivalent to ``getattr(self, name, defval)``.
 
         """
-        return self.__dict__.get (name, defval)
+        return self.__dict__.get(name, defval)
 
-    def set_one (self, name, value):
+    def set_one(self, name, value):
         """Set a single attribute on this object.
 
-        Equivalent to ``setattr (self, name, value)``. Returns *self*.
+        Equivalent to ``setattr(self, name, value)``. Returns *self*.
 
         """
         self.__dict__[name] = value
         return self
 
-    def has (self, name):
+    def has(self, name):
         """Return whether the named attribute has been set on this object.
 
         This can more naturally be expressed by writing ``name in self``.
 
         """
         return name in self.__dict__
 
-    def copy (self):
+    def copy(self):
         """Return a shallow copy of this object.
 
         """
-        new = self.__class__ ()
-        new.__dict__ = dict (self.__dict__)
+        new = self.__class__()
+        new.__dict__ = dict(self.__dict__)
         return new
 
-    def to_dict (self):
+    def to_dict(self):
         """Return a copy of this object converted to a :class:`dict`.
 
         """
-        return self.__dict__.copy ()
+        return self.__dict__.copy()
 
-    def to_pretty (self, format='str'):
+    def to_pretty(self, format='str'):
         """Return a string with a prettified version of this object’s contents.
 
         The format is a multiline string where each line is of the form ``key
         = value``. If the *format* argument is equal to ``"str"``, each
         ``value`` is the stringification of the value; if it is ``"repr"``, it
         is its :func:`repr`.
 
@@ -235,17 +230,17 @@
 
         """
         if format == 'str':
             template = '%-*s = %s'
         elif format == 'repr':
             template = '%-*s = %r'
         else:
-            raise ValueError ('unrecognied value for "format": %r' % format)
+            raise ValueError('unrecognized value for "format": %r' % format)
 
         d = self.__dict__
         maxlen = 0
 
-        for k in six.iterkeys (d):
-            maxlen = max (maxlen, len (k))
+        for k in six.iterkeys(d):
+            maxlen = max(maxlen, len(k))
 
-        return '\n'.join (template % (maxlen, k, d[k])
-                          for k in sorted (six.iterkeys (d)))
+        return '\n'.join(template % (maxlen, k, d[k])
+                         for k in sorted(six.iterkeys(d)))
```

### Comparing `pwkit-0.8.9/pwkit/phoenix.py` & `pwkit-1.0.0/pwkit/phoenix.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/numutil.py` & `pwkit-1.0.0/pwkit/numutil.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,170 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2014-2015 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2014-2019 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """The :mod:`numpy` and :mod:`scipy` packages provide a whole host of
 routines, but there are still some that are missing. The :mod:`pwkit.numutil`
 module provides several useful additions.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('''broadcastize dfsmooth fits_recarray_to_data_frame make_step_lcont
+__all__ = '''broadcastize dfsmooth fits_recarray_to_data_frame make_step_lcont
            make_step_rcont make_tophat_ee make_tophat_ei make_tophat_ie
            make_tophat_ii parallel_newton parallel_quad rms unit_tophat_ee
            unit_tophat_ei unit_tophat_ie unit_tophat_ii usmooth weighted_mean
-           weighted_mean_df weighted_variance''').split ()
+           weighted_mean_df weighted_variance'''.split()
 
 import functools
 from six.moves import range
 import numpy as np
 
 from .method_decorator import method_decorator
 
 
-def _broadcastize_spec_to_scalar_filter (s):
+def _broadcastize_spec_to_scalar_filter(s):
     if s is None:
         # This return value is independent of the inputs altogether.
         return lambda x: x
     if s == 0:
         # This return value has the same shape as the input(s). If we
         # promoted to a 1-element vector, we need to demote.
         return np.asscalar
     if s == 1:
         # This return value is a larger vector of the input(s). If we promoted
         # from a scalar, we drop the final axis. We asarray() the result for
         # convenience/robustness.
-        return lambda x: np.asarray (x)[...,0]
+        return lambda x: np.asarray(x)[...,0]
 
-    raise ValueError ('unrecognized @broadcastize ret_spec value %r' % s)
+    raise ValueError('unrecognized @broadcastize ret_spec value %r' % s)
 
 
-class _Broadcaster (method_decorator):
+class _Broadcaster(method_decorator):
     # _BroadcasterDecorator must set self._n_arr and _scalar_ret_filter on creation.
 
-    def fixup (self, newobj):
+    def fixup(self, newobj):
         # This function is used by the method_decorator superclass.
-        newobj._n_arr = object.__getattribute__ (self, '_n_arr')
-        newobj._force_float = object.__getattribute__ (self, '_force_float')
-        newobj._scalar_ret_filter = object.__getattribute__ (self, '_scalar_ret_filter')
-
-    def __call__ (self, *args, **kwargs):
-        n_arr = object.__getattribute__ (self, '_n_arr')
-        force_float = object.__getattribute__ (self, '_force_float')
-
-        if len (args) < n_arr:
-            raise TypeError ('expected at least %d arguments, got %d'
-                             % (n_arr, len (args)))
+        newobj._n_arr = object.__getattribute__(self, '_n_arr')
+        newobj._force_float = object.__getattribute__(self, '_force_float')
+        newobj._scalar_ret_filter = object.__getattribute__(self, '_scalar_ret_filter')
+
+    def __call__(self, *args, **kwargs):
+        n_arr = object.__getattribute__(self, '_n_arr')
+        force_float = object.__getattribute__(self, '_force_float')
+
+        if len(args) < n_arr:
+            raise TypeError('expected at least %d arguments, got %d'
+                             % (n_arr, len(args)))
 
-        bc_raw = np.broadcast_arrays (*args[:n_arr])
+        bc_raw = np.broadcast_arrays(*args[:n_arr])
         if force_float:
-            bc_raw = tuple (np.asfarray (a) for a in bc_raw)
-        bc_1d = tuple (np.atleast_1d (a) for a in bc_raw)
+            bc_raw = tuple(np.asfarray(a) for a in bc_raw)
+        bc_1d = tuple(np.atleast_1d(a) for a in bc_raw)
         rest = args[n_arr:]
-        result = super (_Broadcaster, self).__call__ (*(bc_1d + rest), **kwargs)
+        result = super(_Broadcaster, self).__call__(*(bc_1d + rest), **kwargs)
 
         if bc_raw[0].ndim == 0:
             # Inputs were all scalars. We need to filter the output(s) to
             # remove extra axes.
-            scalar_ret_filter = object.__getattribute__ (self, '_scalar_ret_filter')
-            result = scalar_ret_filter (result)
+            scalar_ret_filter = object.__getattribute__(self, '_scalar_ret_filter')
+            result = scalar_ret_filter(result)
 
         return result
 
 
-class _BroadcasterDecorator (object):
+class _BroadcasterDecorator(object):
     """Decorator to make functions automatically work on vectorized arguments. See
     the pwkit documentation for usage information.
 
     """
-    def __init__ (self, n_arr, ret_spec=0, force_float=True):
-        self._n_arr = int (n_arr)
+    def __init__(self, n_arr, ret_spec=0, force_float=True):
+        self._n_arr = int(n_arr)
         if self._n_arr < 1:
-            raise ValueError ('broadcastiz\'ed function must take at least 1 '
-                              'array argument')
+            raise ValueError('broadcastiz\'ed function must take at least 1 '
+                             'array argument')
 
-        self._force_float = bool (force_float)
+        self._force_float = bool(force_float)
 
-        if isinstance (ret_spec, tuple):
-            filters = tuple (_broadcastize_spec_to_scalar_filter (s) for s in ret_spec)
-            self._scalar_ret_filter = lambda r: tuple (f (v) for f, v in zip (filters, r))
+        if isinstance(ret_spec, tuple):
+            filters = tuple(_broadcastize_spec_to_scalar_filter(s) for s in ret_spec)
+            self._scalar_ret_filter = lambda r: tuple(f(v) for f, v in zip(filters, r))
         else:
-            self._scalar_ret_filter = _broadcastize_spec_to_scalar_filter (ret_spec)
+            self._scalar_ret_filter = _broadcastize_spec_to_scalar_filter(ret_spec)
 
 
-    def __call__ (self, subfunc):
-        b = _Broadcaster (subfunc)
+    def __call__(self, subfunc):
+        b = _Broadcaster(subfunc)
         b._n_arr = self._n_arr
         b._force_float = self._force_float
         b._scalar_ret_filter = self._scalar_ret_filter
         return b
 
 broadcastize = _BroadcasterDecorator
 
 
 # Very misc.
 
-def fits_recarray_to_data_frame (recarray, drop_nonscalar_ok=True):
+def fits_recarray_to_data_frame(recarray, drop_nonscalar_ok=True):
     """Convert a FITS data table, stored as a Numpy record array, into a Pandas
     DataFrame object. By default, non-scalar columns are discarded, but if
     *drop_nonscalar_ok* is False then a :exc:`ValueError` is raised. Column
     names are lower-cased. Example::
 
       from pwkit import io, numutil
-      hdu_list = io.Path ('my-table.fits').read_fits ()
+      hdu_list = io.Path('my-table.fits').read_fits()
       # assuming the first FITS extension is a binary table:
-      df = numutil.fits_recarray_to_data_frame (hdu_list[1].data)
+      df = numutil.fits_recarray_to_data_frame(hdu_list[1].data)
 
     FITS data are big-endian, whereas nowadays almost everything is
     little-endian. This seems to be an issue for Pandas DataFrames, where
     ``df[['col1', 'col2']]`` triggers an assertion for me if the underlying
     data are not native-byte-ordered. This function normalizes the read-in
     data to native endianness to avoid this.
 
     See also :meth:`pwkit.io.Path.read_fits_bintable`.
 
     """
     from pandas import DataFrame
 
-    def normalize ():
+    def normalize():
         for column in recarray.columns:
             n = column.name
             d = recarray[n]
 
             if d.ndim != 1:
                 if not drop_nonscalar_ok:
-                    raise ValueError ('input must have only scalar columns')
+                    raise ValueError('input must have only scalar columns')
                 continue
 
             if d.dtype.isnative:
-                yield (n.lower (), d)
+                yield (n.lower(), d)
             else:
-                yield (n.lower (), d.byteswap (True).newbyteorder ())
+                yield (n.lower(), d.byteswap(True).newbyteorder())
 
-    return DataFrame (dict (normalize ()))
+    return DataFrame(dict(normalize()))
 
 
-def data_frame_to_astropy_table (dataframe):
+def data_frame_to_astropy_table(dataframe):
     """This is a backport of the Astropy method
    :meth:`astropy.table.table.Table.from_pandas`. It converts a Pandas
    :class:`pandas.DataFrame` object to an Astropy
    :class:`astropy.table.Table`.
 
     """
     from astropy.utils import OrderedDict
     from astropy.table import Table, Column, MaskedColumn
     from astropy.extern import six
 
     out = OrderedDict()
 
     for name in dataframe.columns:
         column = dataframe[name]
-        mask = np.array (column.isnull ())
-        data = np.array (column)
+        mask = np.array(column.isnull())
+        data = np.array(column)
 
         if data.dtype.kind == 'O':
             # If all elements of an object array are string-like or np.nan
             # then coerce back to a native numpy str/unicode array.
             string_types = six.string_types
             if six.PY3:
                 string_types += (bytes,)
@@ -182,15 +182,15 @@
             out[name] = MaskedColumn(data=data, name=name, mask=mask)
         else:
             out[name] = Column(data=data, name=name)
 
     return Table(out)
 
 
-def page_data_frame (df, pager_argv=['less'], **kwargs):
+def page_data_frame(df, pager_argv=['less'], **kwargs):
     """Render a DataFrame as text and send it to a terminal pager program (e.g.
     `less`), so that one can browse a full table conveniently.
 
     df
       The DataFrame to view
     pager_argv: default ``['less']``
       A list of strings passed to :class:`subprocess.Popen` that launches
@@ -199,98 +199,98 @@
       Additional keywords are passed to :meth:`pandas.DataFrame.to_string`.
 
     Returns ``None``. Execution blocks until the pager subprocess exits.
 
     """
     import codecs, subprocess, sys
 
-    pager = subprocess.Popen (pager_argv, shell=False,
-                              stdin=subprocess.PIPE,
-                              close_fds=True)
+    pager = subprocess.Popen(pager_argv, shell=False,
+                             stdin=subprocess.PIPE,
+                             close_fds=True)
 
     try:
-        enc = codecs.getwriter (sys.stdout.encoding or 'utf8') (pager.stdin)
-        df.to_string (enc, **kwargs)
+        enc = codecs.getwriter(sys.stdout.encoding or 'utf8')(pager.stdin)
+        df.to_string(enc, **kwargs)
     finally:
-        enc.close ()
-        pager.stdin.close ()
-        pager.wait ()
+        enc.close()
+        pager.stdin.close()
+        pager.wait()
 
 
 # Chunked averaging of data tables
 
-def slice_around_gaps (values, maxgap):
+def slice_around_gaps(values, maxgap):
     """Given an ordered array of values, generate a set of slices that traverse
     all of the values. Within each slice, no gap between adjacent values is
     larger than `maxgap`. In other words, these slices break the array into
     chunks separated by gaps of size larger than maxgap.
 
     """
     if not (maxgap > 0):
         # above test catches NaNs, other weird cases
-        raise ValueError ('maxgap must be positive; got %r' % maxgap)
+        raise ValueError('maxgap must be positive; got %r' % maxgap)
 
-    values = np.asarray (values)
+    values = np.asarray(values)
     delta = values[1:] - values[:-1]
 
-    if np.any (delta < 0):
-        raise ValueError ('values must be in nondecreasing order')
+    if np.any(delta < 0):
+        raise ValueError('values must be in nondecreasing order')
 
-    whgap = np.where (delta > maxgap)[0] + 1
+    whgap = np.where(delta > maxgap)[0] + 1
     prev_idx = None
 
     for gap_idx in whgap:
-        yield slice (prev_idx, gap_idx)
+        yield slice(prev_idx, gap_idx)
         prev_idx = gap_idx
 
-    yield slice (prev_idx, None)
+    yield slice(prev_idx, None)
 
 
-def slice_evenly_with_gaps (values, target_len, maxgap):
+def slice_evenly_with_gaps(values, target_len, maxgap):
     """Given an ordered array of values, generate a set of slices that traverse
     all of the values. Each slice contains about `target_len` items. However,
     no slice contains a gap larger than `maxgap`, so a slice may contain only
     a single item (if it is surrounded on both sides by a large gap). If a
     non-gapped run of values does not divide evenly into `target_len`, the
     algorithm errs on the side of making the slices contain more than
     `target_len` items, rather than fewer. It also attempts to keep the slice
     size uniform within each non-gapped run.
 
     """
     if not (target_len > 0):
-        raise ValueError ('target_len must be positive; got %r' % target_len)
+        raise ValueError('target_len must be positive; got %r' % target_len)
 
-    values = np.asarray (values)
+    values = np.asarray(values)
     l = values.size
 
-    for gapslice in slice_around_gaps (values, maxgap):
-        start, stop, ignored_stride = gapslice.indices (l)
+    for gapslice in slice_around_gaps(values, maxgap):
+        start, stop, ignored_stride = gapslice.indices(l)
         num_elements = stop - start
-        nsegments = int (np.floor (float (num_elements) / target_len))
-        nsegments = max (nsegments, 1)
-        nsegments = min (nsegments, num_elements)
+        nsegments = int(np.floor(float(num_elements) / target_len))
+        nsegments = max(nsegments, 1)
+        nsegments = min(nsegments, num_elements)
         segment_len = num_elements / nsegments
         offset = 0.
         prev = start
 
-        for _ in range (nsegments):
+        for _ in range(nsegments):
             offset += segment_len
-            next = start + int (round (offset))
+            next = start + int(round(offset))
             if next > prev:
-                yield slice (prev, next)
+                yield slice(prev, next)
             prev = next
 
 
-def reduce_data_frame (df, chunk_slicers,
-                       avg_cols=(),
-                       uavg_cols=(),
-                       minmax_cols=(),
-                       nchunk_colname='nchunk',
-                       uncert_prefix='u',
-                       min_points_per_chunk=3):
+def reduce_data_frame(df, chunk_slicers,
+                      avg_cols=(),
+                      uavg_cols=(),
+                      minmax_cols=(),
+                      nchunk_colname='nchunk',
+                      uncert_prefix='u',
+                      min_points_per_chunk=3):
     """"Reduce" a DataFrame by collapsing rows in grouped chunks. Returns another
     DataFrame with similar columns but fewer rows.
 
     Arguments:
 
     df
       The input :class:`pandas.DataFrame`.
@@ -317,57 +317,57 @@
 
     Returns a new :class:`pandas.DataFrame`.
 
     """
     subds = [df.iloc[idx] for idx in chunk_slicers]
     subds = [sd for sd in subds if sd.shape[0] >= min_points_per_chunk]
 
-    chunked = df.__class__ ({nchunk_colname: np.zeros (len (subds), dtype=np.int)})
+    chunked = df.__class__({nchunk_colname: np.zeros(len(subds), dtype=np.int)})
 
     # Some future-proofing: allow possibility of different ways of mapping
     # from a column giving a value to a column giving its uncertainty.
 
     uncert_col_name = lambda c: uncert_prefix + c
 
-    for i, subd in enumerate (subds):
+    for i, subd in enumerate(subds):
         label = chunked.index[i]
         chunked.loc[label,nchunk_colname] = subd.shape[0]
 
         for col in avg_cols:
-            chunked.loc[label,col] = subd[col].mean ()
+            chunked.loc[label,col] = subd[col].mean()
 
         for col in uavg_cols:
-            ucol = uncert_col_name (col)
-            v, u = weighted_mean (subd[col], subd[ucol])
+            ucol = uncert_col_name(col)
+            v, u = weighted_mean(subd[col], subd[ucol])
             chunked.loc[label,col] = v
             chunked.loc[label,ucol] = u
 
         for col in minmax_cols:
-            chunked.loc[label, 'min_'+col] = subd[col].min ()
-            chunked.loc[label, 'max_'+col] = subd[col].max ()
+            chunked.loc[label, 'min_'+col] = subd[col].min()
+            chunked.loc[label, 'max_'+col] = subd[col].max()
 
     return chunked
 
 
-def reduce_data_frame_evenly_with_gaps (df, valcol, target_len, maxgap, **kwargs):
+def reduce_data_frame_evenly_with_gaps(df, valcol, target_len, maxgap, **kwargs):
     """"Reduce" a DataFrame by collapsing rows in grouped chunks, grouping based on
     gaps in one of the columns.
 
     This function combines :func:`reduce_data_frame` with
     :func:`slice_evenly_with_gaps`.
 
     """
-    return reduce_data_frame (df,
-                              slice_evenly_with_gaps (df[valcol], target_len, maxgap),
+    return reduce_data_frame(df,
+                              slice_evenly_with_gaps(df[valcol], target_len, maxgap),
                               **kwargs)
 
 
 # Smooth a timeseries with uncertainties
 
-def usmooth (window, uncerts, *data, **kwargs):
+def usmooth(window, uncerts, *data, **kwargs):
     """Smooth data series according to a window, weighting based on uncertainties.
 
     Arguments:
 
     window
       The smoothing window.
     uncerts
@@ -380,51 +380,51 @@
       points will be discarded.
 
     Returns: ``(s_uncerts, s_data[0], s_data[1], ...)``, the smoothed
     uncertainties and data series.
 
     Example::
 
-        u, x, y = numutil.usmooth (np.hamming (7), u, x, y)
+        u, x, y = numutil.usmooth(np.hamming(7), u, x, y)
 
     """
-    window = np.asarray (window)
-    uncerts = np.asarray (uncerts)
+    window = np.asarray(window)
+    uncerts = np.asarray(uncerts)
 
-    # Hacky keyword argument handling because you can't write "def foo (*args,
+    # Hacky keyword argument handling because you can't write "def foo(*args,
     # k=0)".
 
-    k = kwargs.pop ('k', None)
+    k = kwargs.pop('k', None)
 
-    if len (kwargs):
-        raise TypeError ("smooth() got an unexpected keyword argument '%s'"
-                         % kwargs.keys ()[0])
+    if len(kwargs):
+        raise TypeError("smooth() got an unexpected keyword argument '%s'"
+                        % kwargs.keys()[0])
 
     # Done with kwargs futzing.
 
     if k is None:
         k = window.size
 
-    conv = lambda q, r: np.convolve (q, r, mode='valid')
+    conv = lambda q, r: np.convolve(q, r, mode='valid')
 
     if uncerts is None:
-        w = np.ones_like (x)
+        w = np.ones_like(x)
     else:
         w = uncerts ** -2
 
-    cw = conv (w, window)
-    cu = np.sqrt (conv (w, window**2)) / cw
-    result = [cu] + [conv (w * np.asarray (x), window) / cw for x in data]
+    cw = conv(w, window)
+    cu = np.sqrt(conv(w, window**2)) / cw
+    result = [cu] + [conv(w * np.asarray(x), window) / cw for x in data]
 
     if k != 1:
         result = [x[::k] for x in result]
     return result
 
 
-def dfsmooth (window, df, ucol, k=None):
+def dfsmooth(window, df, ucol, k=None):
     """Smooth a :class:`pandas.DataFrame` according to a window, weighting based on
     uncertainties.
 
     Arguments are:
 
     window
       The smoothing window.
@@ -440,45 +440,92 @@
 
     Returns: a smoothed data frame.
 
     The returned data frame has a default integer index.
 
     Example::
 
-        sdata = numutil.dfsmooth (np.hamming (7), data, 'u_temp')
+        sdata = numutil.dfsmooth(np.hamming(7), data, 'u_temp')
 
     """
     import pandas as pd
 
     if k is None:
         k = window.size
 
-    conv = lambda q, r: np.convolve (q, r, mode='valid')
+    conv = lambda q, r: np.convolve(q, r, mode='valid')
     w = df[ucol] ** -2
-    invcw = 1. / conv (w, window)
+    invcw = 1. / conv(w, window)
 
     # XXX: we're not smoothing the index.
 
     res = {}
 
     for col in df.columns:
         if col == ucol:
-            res[col] = np.sqrt (conv (w, window**2)) * invcw
+            res[col] = np.sqrt(conv(w, window**2)) * invcw
         else:
-            res[col] = conv (w * df[col], window) * invcw
+            res[col] = conv(w * df[col], window) * invcw
 
-    res = pd.DataFrame (res)
+    res = pd.DataFrame(res)
     return res[::k]
 
 
+def smooth_data_frame_with_gaps(
+        window, df, uncert_col,
+        time_col, max_gap,
+        min_points_per_chunk = 3,
+        k = None,
+):
+    """Smooth a :class:`pandas.DataFrame` according to a window, weighting based
+    on uncertainties, and breaking the smoothing process at gaps in a time
+    axis.
+
+    Arguments are:
+
+    window
+      The smoothing window.
+    df
+      The :class:`pandas.DataFrame`.
+    uncert_col
+      The name of the column in *df* that contains the uncertainties to weight
+      by.
+    time_col
+      The name of the column in *df* that contains the time-like quantities used
+      to determine where the gaps are.
+    max_gap
+      If a difference larger than this value is encountered in ``df[time_col]``,
+      the smoothing will be discontinuous around this gap. Therefore the units
+      of this column are whatever the units of ``df[time_col]`` are.
+    k = None
+      If specified, only every *k*-th point of the results will be kept. If k
+      is None (the default), it is set to ``window.size``, i.e. correlated
+      points will be discarded. This decimation does not cross over gaps.
+    min_points_per_chunk = 3
+      When gaps are identified, if any chunk of data has fewer than this many
+      elements, it is dropped altogether. This counting happens before
+      decimation by *k*.
+
+    Returns: a smoothed data frame with a default integer index.
+
+    """
+    import pandas as pd
+
+    chunk_slicers = slice_around_gaps(df[time_col], max_gap)
+    subds = [df.iloc[idx] for idx in chunk_slicers]
+    subds = [sd for sd in subds if sd.shape[0] >= min_points_per_chunk]
+    chunks = [dfsmooth(window, subd, uncert_col, k=k) for subd in subds]
+    return pd.concat(chunks, ignore_index=True)
+
+
 # Parallelized versions of various routines that don't operate vectorially
 # even though sometimes it'd be nice to pretend that they do.
 
-def parallel_newton (func, x0, fprime=None, par_args=(), simple_args=(), tol=1.48e-8,
-                     maxiter=50, parallel=True, **kwargs):
+def parallel_newton(func, x0, fprime=None, par_args=(), simple_args=(), tol=1.48e-8,
+                    maxiter=50, parallel=True, **kwargs):
     """A parallelized version of :func:`scipy.optimize.newton`.
 
     Arguments:
 
     func
       The function to search for zeros, called as ``f(x, [*par_args...], [*simple_args...])``.
     x0
@@ -509,55 +556,55 @@
     of the parameters named above.
 
     The *simple_args* are passed to each function identically for each
     integration. They do not need to be Pickle-able.
 
     Example::
 
-       >>> parallel_newton (lambda x, a: x - 2 * a, 2,
-                            par_args=(np.arange (6),))
+       >>> parallel_newton(lambda x, a: x - 2 * a, 2,
+                           par_args=(np.arange(6),))
        <<< array([  0.,   2.,   4.,   6.,   8.,  10.])
-       >>> parallel_newton (lambda x: np.sin (x), np.arange (6))
+       >>> parallel_newton(lambda x: np.sin(x), np.arange(6))
        <<< array([  0.00000000e+00,   3.65526589e-26,   3.14159265e+00,
                     3.14159265e+00,   3.14159265e+00,   6.28318531e+00])
 
     """
     from scipy.optimize import newton
 
     from .parallel import make_parallel_helper
-    phelp = make_parallel_helper (parallel)
+    phelp = make_parallel_helper(parallel)
 
-    if not isinstance (par_args, tuple):
-        raise ValueError ('par_args must be a tuple')
+    if not isinstance(par_args, tuple):
+        raise ValueError('par_args must be a tuple')
 
-    if not isinstance (simple_args, tuple):
-        raise ValueError ('simple_args must be a tuple')
+    if not isinstance(simple_args, tuple):
+        raise ValueError('simple_args must be a tuple')
 
-    bc_raw = np.broadcast_arrays (x0, tol, maxiter, *par_args)
-    bc_1d = tuple (np.atleast_1d (a) for a in bc_raw)
+    bc_raw = np.broadcast_arrays(x0, tol, maxiter, *par_args)
+    bc_1d = tuple(np.atleast_1d(a) for a in bc_raw)
 
-    def gen_var_args ():
-        for i in range (bc_1d[0].size):
-            yield tuple (x.flat[i] for x in bc_1d)
+    def gen_var_args():
+        for i in range(bc_1d[0].size):
+            yield tuple(x.flat[i] for x in bc_1d)
 
-    def helper (i, _, var_args):
+    def helper(i, _, var_args):
         x0, tol, maxiter = var_args[:3]
         args = var_args[3:] + simple_args
-        return newton (func, x0, fprime=fprime, args=args, tol=tol,
+        return newton(func, x0, fprime=fprime, args=args, tol=tol,
                        maxiter=maxiter, **kwargs)
 
-    with phelp.get_ppmap () as ppmap:
-        result = np.asarray (ppmap (helper, None, gen_var_args ()))
+    with phelp.get_ppmap() as ppmap:
+        result = np.asarray(ppmap(helper, None, gen_var_args()))
 
     if bc_raw[0].ndim == 0:
-        return np.asscalar (result)
+        return np.asscalar(result)
     return result
 
 
-def parallel_quad (func, a, b, par_args=(), simple_args=(), parallel=True, **kwargs):
+def parallel_quad(func, a, b, par_args=(), simple_args=(), parallel=True, **kwargs):
     """A parallelized version of :func:`scipy.integrate.quad`.
 
     Arguments are:
 
     func
       The function to integrate, called as ``f(x, [*par_args...], [*simple_args...])``.
     a
@@ -586,19 +633,19 @@
     the return value has shape (2,).
 
     The *simple_args* are passed to each integrand function identically for each
     integration. They do not need to be Pickle-able.
 
     Example::
 
-      >>> parallel_quad (lambda x, u, v, q: u * x + v,
-                         0, # a
-                         [3, 4], # b
-                         (np.arange (6).reshape ((3,2)), np.arange (3).reshape ((3,1))), # par_args
-                         ('hello',),)
+      >>> parallel_quad(lambda x, u, v, q: u * x + v,
+                        0, # a
+                        [3, 4], # b
+                        (np.arange(6).reshape((3,2)), np.arange(3).reshape((3,1))), # par_args
+                        ('hello',),)
 
     Computes six integrals and returns an array of shape ``(2,3,2)``. The
     functions that are evaluated are::
 
       [[ 0*x + 0, 1*x + 0 ],
        [ 2*x + 1, 3*x + 1 ],
        [ 4*x + 2, 5*x + 2 ]]
@@ -611,277 +658,277 @@
 
     In all cases the unused fourth parameter *q* is ``'hello'``.
 
     """
     from scipy.integrate import quad
 
     from .parallel import make_parallel_helper
-    phelp = make_parallel_helper (parallel)
+    phelp = make_parallel_helper(parallel)
 
-    if not isinstance (par_args, tuple):
-        raise ValueError ('par_args must be a tuple')
+    if not isinstance(par_args, tuple):
+        raise ValueError('par_args must be a tuple')
 
-    if not isinstance (simple_args, tuple):
-        raise ValueError ('simple_args must be a tuple')
+    if not isinstance(simple_args, tuple):
+        raise ValueError('simple_args must be a tuple')
 
-    bc_raw = np.broadcast_arrays (a, b, *par_args)
-    bc_1d = tuple (np.atleast_1d (a) for a in bc_raw)
+    bc_raw = np.broadcast_arrays(a, b, *par_args)
+    bc_1d = tuple(np.atleast_1d(a) for a in bc_raw)
 
-    def gen_var_args ():
-        for i in range (bc_1d[0].size):
-            yield tuple (x.flat[i] for x in bc_1d)
+    def gen_var_args():
+        for i in range(bc_1d[0].size):
+            yield tuple(x.flat[i] for x in bc_1d)
 
-    def helper (i, _, var_args):
+    def helper(i, _, var_args):
         a, b = var_args[:2]
-        return quad (func, a, b, var_args[2:] + simple_args, **kwargs)
+        return quad(func, a, b, var_args[2:] + simple_args, **kwargs)
 
-    with phelp.get_ppmap () as ppmap:
-        result_list = ppmap (helper, None, gen_var_args ())
+    with phelp.get_ppmap() as ppmap:
+        result_list = ppmap(helper, None, gen_var_args())
 
     if bc_raw[0].ndim == 0:
-        return np.asarray (result_list[0])
+        return np.asarray(result_list[0])
 
-    result_arr = np.empty ((2,) + bc_raw[0].shape)
-    for i in range (bc_1d[0].size):
+    result_arr = np.empty((2,) + bc_raw[0].shape)
+    for i in range(bc_1d[0].size):
         result_arr[0].flat[i], result_arr[1].flat[i] = result_list[i]
     return result_arr
 
 
 # Some miscellaneous numerical tools
 
-def rms (x):
+def rms(x):
     """Return the square root of the mean of the squares of ``x``."""
-    return np.sqrt (np.square (x).mean ())
+    return np.sqrt(np.square(x).mean())
 
 
-def weighted_mean (values, uncerts, **kwargs):
-    values = np.asarray (values)
-    uncerts = np.asarray (uncerts)
+def weighted_mean(values, uncerts, **kwargs):
+    values = np.asarray(values)
+    uncerts = np.asarray(uncerts)
     weights = uncerts ** -2
-    wt_mean, wt_sum = np.average (values, weights=weights, returned=True, **kwargs)
+    wt_mean, wt_sum = np.average(values, weights=weights, returned=True, **kwargs)
     return wt_mean, wt_sum ** -0.5
 
 
-def weighted_mean_df (df, **kwargs):
+def weighted_mean_df(df, **kwargs):
     """The same as :func:`weighted_mean`, except the argument is expected to be a
    two-column :class:`pandas.DataFrame` whose first column gives the data
    values and second column gives their uncertainties. Returns
    ``(weighted_mean, uncertainty_in_mean)``.
 
     """
-    return weighted_mean (df[df.columns[0]], df[df.columns[1]], **kwargs)
+    return weighted_mean(df[df.columns[0]], df[df.columns[1]], **kwargs)
 
 
-def weighted_variance (x, weights):
+def weighted_variance(x, weights):
     """Return the variance of a weighted sample.
 
     The weighted sample mean is calculated and subtracted off, so the returned
     variance is upweighted by ``n / (n - 1)``. If the sample mean is known to
-    be zero, you should just compute ``np.average (x**2, weights=weights)``.
+    be zero, you should just compute ``np.average(x**2, weights=weights)``.
 
     """
-    n = len (x)
+    n = len(x)
     if n < 3:
-        raise ValueError ('cannot calculate meaningful variance of fewer '
-                          'than three samples')
-    wt_mean = np.average (x, weights=weights)
-    return np.average (np.square (x - wt_mean), weights=weights) * n / (n - 1)
+        raise ValueError('cannot calculate meaningful variance of fewer '
+                         'than three samples')
+    wt_mean = np.average(x, weights=weights)
+    return np.average(np.square(x - wt_mean), weights=weights) * n / (n - 1)
 
 
 # Tophat functions -- numpy doesn't have anything built-in (that I know of)
 # that does this in a convenient way that I'd like. These are useful for
 # defining functions in a piecewise-ish way, although also pay attention to
 # the existence of np.piecewise!
 #
 # We're careful with inclusivity/exclusivity of the bounds since that can be
 # important.
 
-def unit_tophat_ee (x):
+def unit_tophat_ee(x):
     """Tophat function on the unit interval, left-exclusive and right-exclusive.
     Returns 1 if 0 < x < 1, 0 otherwise.
 
     """
-    x = np.asarray (x)
-    x1 = np.atleast_1d (x)
-    r = ((0 < x1) & (x1 < 1)).astype (x.dtype)
+    x = np.asarray(x)
+    x1 = np.atleast_1d(x)
+    r = ((0 < x1) & (x1 < 1)).astype(x.dtype)
     if x.ndim == 0:
-        return np.asscalar (r)
+        return np.asscalar(r)
     return r
 
 
-def unit_tophat_ei (x):
+def unit_tophat_ei(x):
     """Tophat function on the unit interval, left-exclusive and right-inclusive.
     Returns 1 if 0 < x <= 1, 0 otherwise.
 
     """
-    x = np.asarray (x)
-    x1 = np.atleast_1d (x)
-    r = ((0 < x1) & (x1 <= 1)).astype (x.dtype)
+    x = np.asarray(x)
+    x1 = np.atleast_1d(x)
+    r = ((0 < x1) & (x1 <= 1)).astype(x.dtype)
     if x.ndim == 0:
-        return np.asscalar (r)
+        return np.asscalar(r)
     return r
 
 
-def unit_tophat_ie (x):
+def unit_tophat_ie(x):
     """Tophat function on the unit interval, left-inclusive and right-exclusive.
     Returns 1 if 0 <= x < 1, 0 otherwise.
 
     """
-    x = np.asarray (x)
-    x1 = np.atleast_1d (x)
-    r = ((0 <= x1) & (x1 < 1)).astype (x.dtype)
+    x = np.asarray(x)
+    x1 = np.atleast_1d(x)
+    r = ((0 <= x1) & (x1 < 1)).astype(x.dtype)
     if x.ndim == 0:
-        return np.asscalar (r)
+        return np.asscalar(r)
     return r
 
 
-def unit_tophat_ii (x):
+def unit_tophat_ii(x):
     """Tophat function on the unit interval, left-inclusive and right-inclusive.
     Returns 1 if 0 <= x <= 1, 0 otherwise.
 
     """
-    x = np.asarray (x)
-    x1 = np.atleast_1d (x)
-    r = ((0 <= x1) & (x1 <= 1)).astype (x.dtype)
+    x = np.asarray(x)
+    x1 = np.atleast_1d(x)
+    r = ((0 <= x1) & (x1 <= 1)).astype(x.dtype)
     if x.ndim == 0:
-        return np.asscalar (r)
+        return np.asscalar(r)
     return r
 
 
-def make_tophat_ee (lower, upper):
+def make_tophat_ee(lower, upper):
     """Return a ufunc-like tophat function on the defined range, left-exclusive
     and right-exclusive. Returns 1 if lower < x < upper, 0 otherwise.
 
     """
-    if not np.isfinite (lower):
-        raise ValueError ('"lower" argument must be finite number; got %r' % lower)
-    if not np.isfinite (upper):
-        raise ValueError ('"upper" argument must be finite number; got %r' % upper)
-
-    def range_tophat_ee (x):
-        x = np.asarray (x)
-        x1 = np.atleast_1d (x)
-        r = ((lower < x1) & (x1 < upper)).astype (x.dtype)
+    if not np.isfinite(lower):
+        raise ValueError('"lower" argument must be finite number; got %r' % lower)
+    if not np.isfinite(upper):
+        raise ValueError('"upper" argument must be finite number; got %r' % upper)
+
+    def range_tophat_ee(x):
+        x = np.asarray(x)
+        x1 = np.atleast_1d(x)
+        r = ((lower < x1) & (x1 < upper)).astype(x.dtype)
         if x.ndim == 0:
-            return np.asscalar (r)
+            return np.asscalar(r)
         return r
 
     range_tophat_ee.__doc__ = ('Ranged tophat function, left-exclusive and '
                                'right-exclusive. Returns 1 if %g < x < %g, '
                                '0 otherwise.') % (lower, upper)
     return range_tophat_ee
 
 
-def make_tophat_ei (lower, upper):
+def make_tophat_ei(lower, upper):
     """Return a ufunc-like tophat function on the defined range, left-exclusive
     and right-inclusive. Returns 1 if lower < x <= upper, 0 otherwise.
 
     """
-    if not np.isfinite (lower):
-        raise ValueError ('"lower" argument must be finite number; got %r' % lower)
-    if not np.isfinite (upper):
-        raise ValueError ('"upper" argument must be finite number; got %r' % upper)
-
-    def range_tophat_ei (x):
-        x = np.asarray (x)
-        x1 = np.atleast_1d (x)
-        r = ((lower < x1) & (x1 <= upper)).astype (x.dtype)
+    if not np.isfinite(lower):
+        raise ValueError('"lower" argument must be finite number; got %r' % lower)
+    if not np.isfinite(upper):
+        raise ValueError('"upper" argument must be finite number; got %r' % upper)
+
+    def range_tophat_ei(x):
+        x = np.asarray(x)
+        x1 = np.atleast_1d(x)
+        r = ((lower < x1) & (x1 <= upper)).astype(x.dtype)
         if x.ndim == 0:
-            return np.asscalar (r)
+            return np.asscalar(r)
         return r
 
     range_tophat_ei.__doc__ = ('Ranged tophat function, left-exclusive and '
                                'right-inclusive. Returns 1 if %g < x <= %g, '
                                '0 otherwise.') % (lower, upper)
     return range_tophat_ei
 
 
-def make_tophat_ie (lower, upper):
+def make_tophat_ie(lower, upper):
     """Return a ufunc-like tophat function on the defined range, left-inclusive
     and right-exclusive. Returns 1 if lower <= x < upper, 0 otherwise.
 
     """
-    if not np.isfinite (lower):
-        raise ValueError ('"lower" argument must be finite number; got %r' % lower)
-    if not np.isfinite (upper):
-        raise ValueError ('"upper" argument must be finite number; got %r' % upper)
-
-    def range_tophat_ie (x):
-        x = np.asarray (x)
-        x1 = np.atleast_1d (x)
-        r = ((lower <= x1) & (x1 < upper)).astype (x.dtype)
+    if not np.isfinite(lower):
+        raise ValueError('"lower" argument must be finite number; got %r' % lower)
+    if not np.isfinite(upper):
+        raise ValueError('"upper" argument must be finite number; got %r' % upper)
+
+    def range_tophat_ie(x):
+        x = np.asarray(x)
+        x1 = np.atleast_1d(x)
+        r = ((lower <= x1) & (x1 < upper)).astype(x.dtype)
         if x.ndim == 0:
-            return np.asscalar (r)
+            return np.asscalar(r)
         return r
 
     range_tophat_ie.__doc__ = ('Ranged tophat function, left-inclusive and '
                                'right-exclusive. Returns 1 if %g <= x < %g, '
                                '0 otherwise.') % (lower, upper)
     return range_tophat_ie
 
 
-def make_tophat_ii (lower, upper):
+def make_tophat_ii(lower, upper):
     """Return a ufunc-like tophat function on the defined range, left-inclusive
     and right-inclusive. Returns 1 if lower < x < upper, 0 otherwise.
 
     """
-    if not np.isfinite (lower):
-        raise ValueError ('"lower" argument must be finite number; got %r' % lower)
-    if not np.isfinite (upper):
-        raise ValueError ('"upper" argument must be finite number; got %r' % upper)
-
-    def range_tophat_ii (x):
-        x = np.asarray (x)
-        x1 = np.atleast_1d (x)
-        r = ((lower <= x1) & (x1 <= upper)).astype (x.dtype)
+    if not np.isfinite(lower):
+        raise ValueError('"lower" argument must be finite number; got %r' % lower)
+    if not np.isfinite(upper):
+        raise ValueError('"upper" argument must be finite number; got %r' % upper)
+
+    def range_tophat_ii(x):
+        x = np.asarray(x)
+        x1 = np.atleast_1d(x)
+        r = ((lower <= x1) & (x1 <= upper)).astype(x.dtype)
         if x.ndim == 0:
-            return np.asscalar (r)
+            return np.asscalar(r)
         return r
 
     range_tophat_ii.__doc__ = ('Ranged tophat function, left-inclusive and '
                                'right-inclusive. Returns 1 if %g <= x <= %g, '
                                '0 otherwise.') % (lower, upper)
     return range_tophat_ii
 
 
 # Step functions
 
-def make_step_lcont (transition):
+def make_step_lcont(transition):
     """Return a ufunc-like step function that is left-continuous. Returns 1 if
     x > transition, 0 otherwise.
 
     """
-    if not np.isfinite (transition):
-        raise ValueError ('"transition" argument must be finite number; got %r' % transition)
+    if not np.isfinite(transition):
+        raise ValueError('"transition" argument must be finite number; got %r' % transition)
 
-    def step_lcont (x):
-        x = np.asarray (x)
-        x1 = np.atleast_1d (x)
-        r = (x1 > transition).astype (x.dtype)
+    def step_lcont(x):
+        x = np.asarray(x)
+        x1 = np.atleast_1d(x)
+        r = (x1 > transition).astype(x.dtype)
         if x.ndim == 0:
-            return np.asscalar (r)
+            return np.asscalar(r)
         return r
 
     step_lcont.__doc__ = ('Left-continuous step function. Returns 1 if x > %g, '
                           '0 otherwise.') % (transition,)
     return step_lcont
 
 
-def make_step_rcont (transition):
+def make_step_rcont(transition):
     """Return a ufunc-like step function that is right-continuous. Returns 1 if
     x >= transition, 0 otherwise.
 
     """
-    if not np.isfinite (transition):
-        raise ValueError ('"transition" argument must be finite number; got %r' % transition)
+    if not np.isfinite(transition):
+        raise ValueError('"transition" argument must be finite number; got %r' % transition)
 
-    def step_rcont (x):
-        x = np.asarray (x)
-        x1 = np.atleast_1d (x)
-        r = (x1 >= transition).astype (x.dtype)
+    def step_rcont(x):
+        x = np.asarray(x)
+        x1 = np.atleast_1d(x)
+        r = (x1 >= transition).astype(x.dtype)
         if x.ndim == 0:
-            return np.asscalar (r)
+            return np.asscalar(r)
         return r
 
     step_rcont.__doc__ = ('Right-continuous step function. Returns 1 if x >= '
                           '%g, 0 otherwise.') % (transition,)
     return step_rcont
```

### Comparing `pwkit-0.8.9/pwkit/lmmin.py` & `pwkit-1.0.0/pwkit/lmmin.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/immodel.py` & `pwkit-1.0.0/pwkit/immodel.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/ellipses.py` & `pwkit-1.0.0/pwkit/ellipses.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/sherpa.py` & `pwkit-1.0.0/pwkit/sherpa.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/io.py` & `pwkit-1.0.0/pwkit/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -906,30 +906,34 @@
                            format, format)
 
         with self.open ('rb') as f:
             return reader (f, **kwargs)
 
 
     def read_pickle (self):
-        """Open the file, unpickle one object from it using :mod:`cPickle`, and return
+        """Open the file, unpickle one object from it using :mod:`pickle`, and return
         it.
 
         """
         gen = self.read_pickles ()
         value = gen.next ()
         gen.close ()
         return value
 
 
     def read_pickles (self):
         """Generate a sequence of objects by opening the path and unpickling items
         until EOF is reached.
 
         """
-        import cPickle as pickle
+        try:
+            import cPickle as pickle
+        except ImportError:
+            import pickle
+
         with self.open (mode='rb') as f:
             while True:
                 try:
                     obj = pickle.load (f)
                 except EOFError:
                     break
                 yield obj
@@ -1011,15 +1015,19 @@
 
 
     def write_pickles (self, objs):
         """*objs* must be iterable. Write each of its values to this path in sequence
         using :mod:`cPickle`.
 
         """
-        import cPickle as pickle
+        try:
+            import cPickle as pickle
+        except ImportError:
+            import pickle
+
         with self.open (mode='wb') as f:
             for obj in objs:
                 pickle.dump (obj, f)
 
 
     def write_yaml (self, data, encoding=None, errors=None, newline=None, **kwargs):
         """Read *data* to this path as a YAML document.
```

### Comparing `pwkit-0.8.9/pwkit/unicode_to_latex.py` & `pwkit-1.0.0/pwkit/unicode_to_latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- mode: python; coding: utf-8 -*-
 # This work is dedicated to the public domain.
 
 """unicode_to_latex - what it says
 
-Provides unicode_to_latex(u) and unicode_to_latex_string(u).
+Provides ``unicode_to_latex(u)``, ``unicode_to_latex_bytes(u)``, and
+``unicode_to_latex_string(u)``.
 
-unicode_to_latex returns ASCII bytes that can be fed to LaTeX to
+``unicode_to_latex_bytes`` returns ASCII bytes that can be fed to LaTeX to
 reproduce the Unicode string 'u' as closely as possible.
 
-unicode_to_latex_string returns a Unicode string rather than bytes.
-That is::
+``unicode_to_latex_string`` returns a Unicode string rather than bytes.
 
-  unicode_to_latex(u) = unicode_to_latex_string(u).encode('ascii').
-"""
+``unicode_to_latex`` returns the ``str`` type: bytes on Python 2, Unicode on
+Python 3.
 
-from __future__ import absolute_import, division, print_function, unicode_literals
+"""
 
-__all__ = str ('unicode_to_latex unicode_to_latex_string').split ()
+from __future__ import absolute_import, division, print_function
 
-from . import text_type
+__all__ = 'unicode_to_latex unicode_to_latex_bytes unicode_to_latex_string'.split()
 
 # Based on https://gist.github.com/798549 (owned by github user piquadrat),
 # but modified to make a table usable with unicode.translate(). I had to
 # comment out a few things and also tweak various of the conversions to make
 # the LaTeX more natural. There were also some surprising missing conversions
 # (e.g. u2010 -> -).
 
@@ -879,16 +879,16 @@
     u"\u2267": br"\geqq{}",
     u"\u2268": br"\lneqq{}",
     u"\u2269": br"\gneqq{}",
     u"\u226A": br"\ll{}",
     u"\u226B": br"\gg{}",
     u"\u226C": br"\between{}",
     u"\u226D": br"\not\kern-0.3em\times{}",
-    u"\u226E": br"\not&lt;",
-    u"\u226F": br"\not&gt;",
+    u"\u226E": br"\not<",
+    u"\u226F": br"\not>",
     u"\u2270": br"\not\leq{}",
     u"\u2271": br"\not\geq{}",
     u"\u2272": br"\lessequivlnt{}",
     u"\u2273": br"\greaterequivlnt{}",
     u"\u2274": br"\ElsevierGlyph{2274}",
     u"\u2275": br"\ElsevierGlyph{2275}",
     u"\u2276": br"\lessgtr{}",
@@ -1313,15 +1313,15 @@
     u"\u296F": br"\ReverseUpEquilibrium{}",
     u"\u2970": br"\RoundImplies{}",
     u"\u297C": br"\ElsevierGlyph{E214}",
     u"\u297D": br"\ElsevierGlyph{E215}",
     u"\u2980": br"\Elztfnc{}",
     u"\u2985": br"\ElsevierGlyph{3018}",
     u"\u2986": br"\Elroang{}",
-    u"\u2993": br"&lt;\kern-0.58em(",
+    u"\u2993": br"<\kern-0.58em(",
     u"\u2994": br"\ElsevierGlyph{E291}",
     u"\u2999": br"\Elzddfnc{}",
     u"\u299C": br"\Angle{}",
     u"\u29A0": br"\Elzlpargt{}",
     u"\u29B5": br"\ElsevierGlyph{E260}",
     u"\u29B6": br"\ElsevierGlyph{E61B}",
     u"\u29CA": br"\ElzLap{}",
@@ -2391,12 +2391,17 @@
 #    u"\u2AA2\u0338": r"\NotNestedGreaterGreater{}",
 #    u"\u2AAF\u0338": r"\not\preceq{}",
 #    u"\u2AB0\u0338": r"\not\succeq{}",
 #    u"\u2AC5\u0338": r"\nsubseteqq{}",
 #    u"\u2AC6\u0338": r"\nsupseteqq",
 #    u"\u2AFD\u20E5": r"{\rlap{\textbackslash}{{/}\!\!{/}}}",
 
-from six import iteritems
-unicode_to_latex_table = dict ((ord (k), text_type (v))
-                               for k, v in iteritems (unicode_to_latex_table_base))
-unicode_to_latex_string = lambda u: u.translate (unicode_to_latex_table)
-unicode_to_latex = lambda u: u.translate (unicode_to_latex_table).encode ('ascii')
+from six import PY2, iteritems, text_type
+
+unicode_to_latex_table = dict((ord(k), v.decode('ascii')) for k, v in iteritems(unicode_to_latex_table_base))
+unicode_to_latex_string = lambda u: u.translate(unicode_to_latex_table)
+unicode_to_latex_bytes = lambda u: u.translate(unicode_to_latex_table).encode('ascii')
+
+if PY2:
+    unicode_to_latex = unicode_to_latex_bytes
+else:
+    unicode_to_latex = unicode_to_latex_string
```

### Comparing `pwkit-0.8.9/pwkit/astimage.py` & `pwkit-1.0.0/pwkit/astimage.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/sas/data.py` & `pwkit-1.0.0/pwkit/environments/sas/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -331,14 +331,76 @@
                         self.targ_name,
                         lines=False)
         self._plot_add_gtis (p, ccdnum)
         p.setLabels ('MJD - %.0f' % self.mjd0, 'PI')
         return p
 
 
+    def plot_lightcurve (self, ccd_id=None, bin_energies=False):
+        # XXX CIAO COPY/PASTE DOES THIS EVEN WORK???
+        import omega as om
+        from ...bblocks import tt_bblock
+        from ..ciao.data import tight_bounds
+
+        if ccd_id is None:
+            if len (self.gti) != 1:
+                raise Exception ('must specify ccd_id')
+            ccd_id = list(self.gti.keys())[0]
+
+        kev = self.events['pi'] * 1e-3 # XXXXXXX
+        vb = om.layout.VBox (2)
+
+        if kev.size == 0:
+            vb[0] = om.RectPlot()
+            vb[1] = om.RectPlot()
+            tmin = self.gti[ccd_id]['start_dmjd'].min()
+            tmax = self.gti[ccd_id]['stop_dmjd'].max()
+            if np.isnan(tmin):
+                tmin, tmax = -1., 1.
+            emin, emax = -1., 1.
+            rmin, rmax = -1., 1.
+        else:
+            bbinfo = tt_bblock (
+                self.gti[ccd_id]['start_dmjd'],
+                self.gti[ccd_id]['stop_dmjd'],
+                self.events['dmjd'].sort_values(),
+                intersect_with_bins = True,
+            )
+            cps = bbinfo.rates / 86400
+
+            tmin, tmax = tight_bounds (bbinfo.ledges[0], bbinfo.redges[-1])
+            emin, emax = tight_bounds (kev.min (), kev.max ())
+            rmin, rmax = tight_bounds (cps.min (), cps.max ())
+
+            vb[0] = om.RectPlot ()
+            csp = om.rect.ContinuousSteppedPainter (keyText='%d events' % (self.events.shape[0]))
+            csp.setFloats (np.concatenate ((bbinfo.ledges, bbinfo.redges[-1:])),
+                           np.concatenate ((cps, [0])))
+            vb[0].add (csp)
+
+            if bin_energies:
+                vb[1] = self._plot_binned_event_energies(
+                    bbinfo,
+                    energy_scale = 1e-3,
+                    dsn = 0
+                )
+            else:
+                vb[1] = om.quickXY (self.events['dmjd'], kev, None, lines=0)
+
+        vb[0].setBounds (tmin, tmax, rmin, rmax)
+        vb[0].setYLabel ('Count rate (ct/s)')
+        vb[0].bpainter.paintLabels = False
+        self._plot_add_gtis (vb[0], ccd_id)
+
+        vb[1].setBounds (tmin, tmax, emin, emax)
+        vb[1].setLabels ('MJD - %d' % self.mjd0, 'Energy (keV)')
+        self._plot_add_gtis (vb[1], ccd_id)
+        return vb
+
+
 class Lightcurve (GTIData, RegionData):
     filter = None
     "Filter used as a string; e.g. 'Medium'."
 
     binsize = None
     "The bin size used when creating the light curve, in seconds."
```

### Comparing `pwkit-0.8.9/pwkit/environments/sas/__init__.py` & `pwkit-1.0.0/pwkit/environments/sas/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2015 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2015-2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """sas - running software in the SAS environment
 
 To use, export an environment variable $PWKIT_SAS pointing to the SAS
 installation root. The files $PWKIT_SAS/RELEASE and $PWKIT_SAS/setsas.sh
 should exist. The "current calibration files" (CCF) should be accessible as
@@ -86,177 +86,186 @@
 ZZZ
   file extension
 
 See the ``make-*-aliases`` commands for tools that generate symlinks with saner
 names.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('').split ()
+__all__ = ''.split()
 
 import io, os.path, six
 
 from ... import PKError, cli
 from ...cli import multitool
 from ...io import Path
 from .. import Environment, prepend_environ_path, user_data_path
 
 
-class SasEnvironment (Environment):
+class SasEnvironment(Environment):
     _odfdir = None
     _revnum = None
     _obsid = None
     _sumsas = None
     _installdir = None
     _heaenv = None
 
-    def __init__ (self, manifest, installdir=None, heaenv=None):
+    def __init__(self, manifest, installdir=None, heaenv=None):
         if installdir is None:
-            installdir = self._default_installdir ()
+            installdir = self._default_installdir()
         if heaenv is None:
             from .. import heasoft
-            heaenv = heasoft.HeasoftEnvironment ()
+            heaenv = heasoft.HeasoftEnvironment()
 
-        self._installdir = os.path.abspath (installdir)
+        self._installdir = os.path.abspath(installdir)
         self._heaenv = heaenv
 
-        manifest = Path (manifest)
+        # TODO: I used to read the manifest file to infer both the revolution
+        # number and obsid, but in the case of 0673000145, the obsid mentioned
+        # in the manifest is different! (But close: 0673000101.) So now I glob
+        # the containing directory for that.
 
-        for line in manifest.read_lines ():
-            if not line.startswith ('File '):
+        manifest = Path(manifest)
+
+        for line in manifest.read_lines():
+            if not line.startswith('File '):
                 continue
 
-            bits = line.split ()[1].split ('_')
-            if len (bits) < 3:
+            bits = line.split()[1].split('_')
+            if len(bits) < 3:
                 continue
 
             self._revnum = bits[0] # note: kept as a string; not an int
+            break
+
+        self._odfdir = Path(manifest).resolve().parent
+
+        for p in self._odfdir.glob('%s_*_*.FIT' % self._revnum):
+            bits = p.name.split('_')
             self._obsid = bits[1]
             break
 
-        self._odfdir = manifest.resolve ().parent
-        self._sumsas = self._odfdir / ('%s_%s_SCX00000SUM.SAS' % (self._revnum,
-                                                                  self._obsid))
+        self._sumsas = self._odfdir / ('%s_%s_SCX00000SUM.SAS' % (self._revnum, self._obsid))
 
 
-    def _default_installdir (self):
-        d = os.environ.get ('PWKIT_SAS')
+    def _default_installdir(self):
+        d = os.environ.get('PWKIT_SAS')
         if d is None:
-            raise PKError ('SAS installation directory must be specified '
-                           'in the $PWKIT_SAS environment variable')
+            raise PKError('SAS installation directory must be specified '
+                          'in the $PWKIT_SAS environment variable')
         return d
 
 
-    def modify_environment (self, env):
-        self._heaenv.modify_environment (env)
+    def modify_environment(self, env):
+        self._heaenv.modify_environment(env)
 
-        def path (*args):
-            return os.path.join (self._installdir, *args)
+        def path(*args):
+            return os.path.join(self._installdir, *args)
 
-        env[b'SAS_DIR'] = path ()
-        env[b'SAS_PATH'] = env[b'SAS_DIR']
-        env[b'SAS_CCFPATH'] = path ('ccf')
-        env[b'SAS_ODF'] = str (self._sumsas) # but see _preexec
-        env[b'SAS_CCF'] = str (self._odfdir / 'ccf.cif')
-
-        prepend_environ_path (env, b'PATH', path ('bin'))
-        prepend_environ_path (env, b'LD_LIBRARY_PATH', path ('libextra'))
-        prepend_environ_path (env, b'LD_LIBRARY_PATH', path ('lib'))
-        prepend_environ_path (env, b'PERL5LIB', path ('lib', 'perl5'))
-
-        env[b'SAS_BROWSER'] = b'firefox' # yay hardcoding
-        env[b'SAS_IMAGEVIEWER'] = b'ds9'
-        env[b'SAS_SUPPRESS_WARNING'] = b'1'
-        env[b'SAS_VERBOSITY'] = b'4'
+        env['SAS_DIR'] = path()
+        env['SAS_PATH'] = env['SAS_DIR']
+        env['SAS_CCFPATH'] = path('ccf')
+        env['SAS_ODF'] = str(self._sumsas) # but see _preexec
+        env['SAS_CCF'] = str(self._odfdir / 'ccf.cif')
+
+        prepend_environ_path(env, 'PATH', path('bin'))
+        prepend_environ_path(env, 'LD_LIBRARY_PATH', path('libextra'))
+        prepend_environ_path(env, 'LD_LIBRARY_PATH', path('lib'))
+        prepend_environ_path(env, 'PERL5LIB', path('lib', 'perl5'))
+
+        env['SAS_BROWSER'] = 'firefox' # yay hardcoding
+        env['SAS_IMAGEVIEWER'] = 'ds9'
+        env['SAS_SUPPRESS_WARNING'] = '1'
+        env['SAS_VERBOSITY'] = '4'
 
         # These can be helpful:
-        env[b'PWKIT_SAS_REVNUM'] = self._revnum
-        env[b'PWKIT_SAS_OBSID'] = self._obsid
+        env['PWKIT_SAS_REVNUM'] = self._revnum
+        env['PWKIT_SAS_OBSID'] = self._obsid
 
         return env
 
 
-    def _preexec (self, env, printbuilds=True):
+    def _preexec(self, env, printbuilds=True):
         from ...cli import wrapout
 
         # Need to compile the CCF info?
 
-        cif = env[b'SAS_CCF']
-        if not os.path.exists (cif):
+        cif = env['SAS_CCF']
+        if not os.path.exists(cif):
             if printbuilds:
-                print ('[building %s]' % cif)
+                print('[building %s]' % cif)
 
-            env['SAS_ODF'] = str (self._odfdir)
+            env['SAS_ODF'] = str(self._odfdir)
             log = self._odfdir / 'cifbuild.log'
 
-            with log.open ('wb') as f:
-                w = wrapout.Wrapper (f)
+            with log.open('wb') as f:
+                w = wrapout.Wrapper(f)
                 w.use_colors = True
-                if w.launch ('cifbuild', ['cifbuild'], env=env, cwd=str (self._odfdir)):
-                    raise PKError ('failed to build CIF; see %s', log)
+                if w.launch('cifbuild', ['cifbuild'], env=env, cwd=str(self._odfdir)):
+                    raise PKError('failed to build CIF; see %s', log)
 
-            if not os.path.exists (cif):
+            if not os.path.exists(cif):
                 # cifbuild can exit with status 0 whilst still having failed
-                raise PKError ('failed to build CIF; see %s', log)
+                raise PKError('failed to build CIF; see %s', log)
 
-            env['SAS_ODF'] = str (self._sumsas)
+            env['SAS_ODF'] = str(self._sumsas)
 
         # Need to generate SUM.SAS file?
 
-        if not self._sumsas.exists ():
+        if not self._sumsas.exists():
             if printbuilds:
-                print ('[building %s]' % self._sumsas)
+                print('[building %s]' % self._sumsas)
 
-            env['SAS_ODF'] = str (self._odfdir)
+            env['SAS_ODF'] = str(self._odfdir)
             log = self._odfdir / 'odfingest.log'
 
-            with log.open ('wb') as f:
-                w = wrapout.Wrapper (f)
+            with log.open('wb') as f:
+                w = wrapout.Wrapper(f)
                 w.use_colors = True
-                if w.launch ('odfingest', ['odfingest'], env=env, cwd=str (self._odfdir)):
-                    raise PKError ('failed to build CIF; see %s', log)
+                if w.launch('odfingest', ['odfingest'], env=env, cwd=str(self._odfdir)):
+                    raise PKError('failed to build CIF; see %s', log)
 
-            env['SAS_ODF'] = str (self._sumsas)
+            env['SAS_ODF'] = str(self._sumsas)
 
 
 # Command-line interface
 
-class Exec (multitool.Command):
+class Exec(multitool.Command):
     name = 'exec'
     argspec = '<manifest> <command> [args...]'
     summary = 'Run a program in SAS.'
     more_help = '''Due to the way SAS works, the path to a MANIFEST.nnnnn file in an ODF
 directory must be specified, and all operations work on the specified data
 set.'''
 
-    def invoke (self, args, **kwargs):
-        if len (args) < 2:
-            raise multitool.UsageError ('exec requires at least 2 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) < 2:
+            raise multitool.UsageError('exec requires at least 2 arguments')
 
         manifest = args[0]
         progargv = args[1:]
 
-        env = SasEnvironment (manifest)
-        env.execvpe (progargv)
+        env = SasEnvironment(manifest)
+        env.execvpe(progargv)
 
 
-class MakeEPICAliases (multitool.Command):
+class MakeEPICAliases(multitool.Command):
     name = 'make-epic-aliases'
     argspec = '<srcdir> <destdir>'
     summary = 'Generate user-friendly aliases to XMM-Newton EPIC data files.'
     more_help = '''destdir should already not exist and will be created. <srcdir> should
 be the ODF directory, containing a file named MANIFEST.<numbers> and many others.'''
 
-    INSTRUMENT = slice (16, 18)
-    EXPFLAG = slice (18, 19) # 'S': sched, 'U': unsched; 'X': N/A
-    EXPNO = slice (19, 22)
-    CCDNO = slice (22, 24)
-    DTYPE = slice (24, 27)
-    EXTENSION = slice (28, None)
+    INSTRUMENT = slice(16, 18)
+    EXPFLAG = slice(18, 19) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPNO = slice(19, 22)
+    CCDNO = slice(22, 24)
+    DTYPE = slice(24, 27)
+    EXTENSION = slice(28, None)
 
     instrmap = {
         'M1': 'mos1',
         'M2': 'mos2',
         'PN': 'pn',
         'RM': 'radmon',
     }
@@ -287,62 +296,62 @@
         'pmh': 'hk_main',
         'pth': 'hk_bright_pixels',
         'rie': 'reduced_imaging',
         'tmh': 'hk_thermal_limits',
         'tie': 'timing',
     }
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('make-epic-aliases requires exactly 2 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError('make-epic-aliases requires exactly 2 arguments')
 
-        srcdir = Path (args[0])
-        destdir = Path (args[1])
+        srcdir = Path(args[0])
+        destdir = Path(args[1])
 
-        srcpaths = [x for x in srcdir.iterdir () if len (x.name) > 28]
+        srcpaths = [x for x in srcdir.iterdir() if len(x.name) > 28]
 
         # Sorted list of exposure numbers.
 
-        expnos = dict ((i, set ()) for i in six.iterkeys (self.instrmap))
+        expnos = dict((i, set()) for i in six.iterkeys(self.instrmap))
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
-            expno = int (p.name[self.EXPNO])
+            expno = int(p.name[self.EXPNO])
             dtype = p.name[self.DTYPE]
 
             if expno > 0 and dtype not in ('DLI', 'ODI'):
-                expnos[instr].add (expno)
+                expnos[instr].add(expno)
 
         expseqs = {}
 
-        for k, v in six.iteritems (expnos):
-            expseqs[self.instrmap[k]] = dict ((n, i) for i, n in enumerate (sorted (v)))
+        for k, v in six.iteritems(expnos):
+            expseqs[self.instrmap[k]] = dict((n, i) for i, n in enumerate(sorted(v)))
 
         # Do it.
 
-        stems = set ()
-        destdir.mkdir () # intentionally crash if exists; easiest approach
+        stems = set()
+        destdir.mkdir() # intentionally crash if exists; easiest approach
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
             eflag = p.name[self.EXPFLAG]
             expno = p.name[self.EXPNO]
             ccdno = p.name[self.CCDNO]
             dtype = p.name[self.DTYPE]
             ext = p.name[self.EXTENSION]
 
             instr = self.instrmap[instr]
-            expno = int (expno)
-            dtype = self.dtypemap[dtype.lower ()]
+            expno = int(expno)
+            dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             if expno > 0 and dtype not in ('discarded_lines', 'offset_data'):
                 expno = expseqs[instr][expno]
 
             if instr == 'radmon' and dtype == 'hk_extraheating_config':
                 dtype = 'rates'
@@ -353,34 +362,34 @@
                 stem = '%s_%s.%s' % (instr, dtype, ext)
             elif dtype in ('discarded_lines', 'offset_data'):
                 stem = '%s_%s_e%03d_c%s.%s' % (instr, dtype, expno, ccdno, ext)
             else:
                 stem = '%s_e%03d_c%s_%s.%s' % (instr, expno, ccdno, dtype, ext)
 
             if stem in stems:
-                cli.die ('short identifier clash: %r', stem)
-            stems.add (stem)
+                cli.die('short identifier clash: %r', stem)
+            stems.add(stem)
 
-            (destdir / stem).rellink_to (p)
+            (destdir / stem).rellink_to(p)
 
 
-class MakeOMAliases (multitool.Command):
+class MakeOMAliases(multitool.Command):
     name = 'make-om-aliases'
     argspec = '<srcdir> <destdir>'
     summary = 'Generate user-friendly aliases to XMM-Newton OM data files.'
     more_help = 'destdir should already not exist and will be created.'
 
-    PROD_TYPE = slice (0, 1) # 'P': final product; 'F': intermediate
-    OBSID = slice (1, 11)
-    EXPFLAG = slice (11, 12) # 'S': sched, 'U': unsched; 'X': N/A
-    EXPNO = slice (14, 17) # (12-14 is the string 'OM')
-    DTYPE = slice (17, 23)
-    WINNUM = slice (23, 24)
-    SRCNUM = slice (24, 27)
-    EXTENSION = slice (28, None)
+    PROD_TYPE = slice(0, 1) # 'P': final product; 'F': intermediate
+    OBSID = slice(1, 11)
+    EXPFLAG = slice(11, 12) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPNO = slice(14, 17) # (12-14 is the string 'OM')
+    DTYPE = slice(17, 23)
+    WINNUM = slice(23, 24)
+    SRCNUM = slice(24, 27)
+    EXTENSION = slice(28, None)
 
     extmap = {
         'ASC': 'txt',
         'FIT': 'fits',
         'PDF': 'pdf',
         'PS': 'ps',
     }
@@ -390,81 +399,81 @@
         'simage': 'image_sky',
         'swsrli': 'source_list',
         'timesr': 'lightcurve',
         'tshplt': 'tracking_plot',
         'tstrts': 'tracking_stars',
     }
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('make-om-aliases requires exactly 2 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError('make-om-aliases requires exactly 2 arguments')
 
         from fnmatch import fnmatch
         srcdir, destdir = args
 
-        srcfiles = [x for x in os.listdir (srcdir)
-                    if x[0] == 'P' and len (x) > 28]
+        srcfiles = [x for x in os.listdir(srcdir)
+                    if x[0] == 'P' and len(x) > 28]
 
         # Sorted list of exposure numbers.
 
-        expnos = set ()
+        expnos = set()
 
         for f in srcfiles:
-            if not fnmatch (f, 'P*IMAGE_*.FIT'):
+            if not fnmatch(f, 'P*IMAGE_*.FIT'):
                 continue
-            expnos.add (f[self.EXPNO])
+            expnos.add(f[self.EXPNO])
 
-        expseqs = dict ((n, i) for i, n in enumerate (sorted (expnos)))
+        expseqs = dict((n, i) for i, n in enumerate(sorted(expnos)))
 
         # Do it.
 
-        idents = set ()
-        os.mkdir (destdir) # intentionally crash if exists; easiest approach
+        idents = set()
+        os.mkdir(destdir) # intentionally crash if exists; easiest approach
 
         for f in srcfiles:
             ptype = f[self.PROD_TYPE]
             obsid = f[self.OBSID]
             eflag = f[self.EXPFLAG]
             expno = f[self.EXPNO]
             dtype = f[self.DTYPE]
             winnum = f[self.WINNUM]
             srcnum = f[self.SRCNUM]
             ext = f[self.EXTENSION]
 
             seq = expseqs[expno]
-            dtype = self.dtypemap[dtype.lower ()]
+            dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             # There's only one clash, and it's easy:
             if dtype == 'lightcurve' and ext == 'pdf':
                 continue
 
             ident = (seq, dtype)
             if ident in idents:
-                cli.die ('short identifier clash: %r', ident)
-            idents.add (ident)
+                cli.die('short identifier clash: %r', ident)
+            idents.add(ident)
 
-            oldpath = os.path.join (srcdir, f)
-            newpath = os.path.join (destdir, '%s.%02d.%s' % (dtype, seq, ext))
-            os.symlink (os.path.relpath (oldpath, destdir), newpath)
+            oldpath = os.path.join(srcdir, f)
+            newpath = os.path.join(destdir, '%s.%02d.%s' % (dtype, seq, ext))
+            os.symlink(os.path.relpath(oldpath, destdir), newpath)
 
 
-class MakeRGSAliases (multitool.Command):
+class MakeRGSAliases(multitool.Command):
     name = 'make-rgs-aliases'
     argspec = '<srcdir> <destdir>'
     summary = 'Generate user-friendly aliases to XMM-Newton RGS data files.'
     more_help = '''destdir should already not exist and will be created. <srcdir> should
 be the ODF directory, containing a file named MANIFEST.<numbers> and many others.'''
 
-    INSTRUMENT = slice (16, 18)
-    EXPFLAG = slice (18, 19) # 'S': sched, 'U': unsched; 'X': N/A
-    EXPNO = slice (19, 22)
-    CCDNO = slice (22, 24)
-    DTYPE = slice (24, 27)
-    EXTENSION = slice (28, None)
+    INSTRUMENT = slice(16, 18)
+    EXPFLAG = slice(18, 19) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPNO = slice(19, 22)
+    CCDNO = slice(22, 24)
+    DTYPE = slice(24, 27)
+    EXTENSION = slice(28, None)
 
     instrmap = {
         'R1': 'rgs1',
         'R2': 'rgs2',
     }
 
     extmap = {
@@ -479,59 +488,59 @@
         'hte': 'high_time_res',
         'ofx': 'offset',
         'pch': 'hk_ccd_temp',
         'pfh': 'hk_periodic',
         'spe': 'spectra',
     }
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('make-rgs-aliases requires exactly 2 arguments')
-
-        srcdir = Path (args[0])
-        destdir = Path (args[1])
-        srcpaths = [x for x in srcdir.iterdir () if len (x.name) > 28]
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError('make-rgs-aliases requires exactly 2 arguments')
+
+        srcdir = Path(args[0])
+        destdir = Path(args[1])
+        srcpaths = [x for x in srcdir.iterdir() if len(x.name) > 28]
 
         # Sorted list of exposure numbers.
 
-        expnos = dict ((i, set ()) for i in six.iterkeys (self.instrmap))
+        expnos = dict((i, set()) for i in six.iterkeys(self.instrmap))
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
-            expno = int (p.name[self.EXPNO])
+            expno = int(p.name[self.EXPNO])
             if expno > 0 and expno < 900:
-                expnos[instr].add (expno)
+                expnos[instr].add(expno)
 
         expseqs = {}
 
-        for k, v in six.iteritems (expnos):
-            expseqs[self.instrmap[k]] = dict ((n, i) for i, n in enumerate (sorted (v)))
+        for k, v in six.iteritems(expnos):
+            expseqs[self.instrmap[k]] = dict((n, i) for i, n in enumerate(sorted(v)))
 
         # Do it.
 
-        stems = set ()
-        destdir.mkdir () # intentionally crash if exists; easiest approach
+        stems = set()
+        destdir.mkdir() # intentionally crash if exists; easiest approach
 
         for p in srcpaths:
             instr = p.name[self.INSTRUMENT]
             if instr not in self.instrmap:
                 continue
 
             eflag = p.name[self.EXPFLAG]
             expno = p.name[self.EXPNO]
             ccdno = p.name[self.CCDNO]
             dtype = p.name[self.DTYPE]
             ext = p.name[self.EXTENSION]
 
             instr = self.instrmap[instr]
-            expno = int (expno)
-            dtype = self.dtypemap[dtype.lower ()]
+            expno = int(expno)
+            dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             if expno > 0 and expno < 900:
                 expno = expseqs[instr][expno]
 
             if ccdno == '00' and dtype != 'aux':
                 stem = '%s_%s.%s' % (instr, dtype, ext)
@@ -539,33 +548,33 @@
                 stem = '%s_e%03d_%s.%s' % (instr, expno, dtype, ext)
             elif dtype == 'diagnostic':
                 stem = '%s_%s_e%03d_c%s.%s' % (instr, dtype, expno, ccdno, ext)
             else:
                 stem = '%s_e%03d_c%s_%s.%s' % (instr, expno, ccdno, dtype, ext)
 
             if stem in stems:
-                cli.die ('short identifier clash: %r', stem)
-            stems.add (stem)
+                cli.die('short identifier clash: %r', stem)
+            stems.add(stem)
 
-            (destdir / stem).rellink_to (p)
+            (destdir / stem).rellink_to(p)
 
 
-class MakeSCAliases (multitool.Command):
+class MakeSCAliases(multitool.Command):
     name = 'make-sc-aliases'
     argspec = '<srcdir> <destdir>'
     summary = 'Generate user-friendly aliases to XMM-Newton spacecraft (SC) data files.'
     more_help = '''destdir should already not exist and will be created. <srcdir> should
 be the ODF directory, containing a file named MANIFEST.<numbers> and many others.'''
 
-    INSTRUMENT = slice (16, 18)
-    EXPFLAG = slice (18, 19) # 'S': sched, 'U': unsched; 'X': N/A
-    EXPNO = slice (19, 22)
-    CCDNO = slice (22, 24)
-    DTYPE = slice (24, 27)
-    EXTENSION = slice (28, None)
+    INSTRUMENT = slice(16, 18)
+    EXPFLAG = slice(18, 19) # 'S': sched, 'U': unsched; 'X': N/A
+    EXPNO = slice(19, 22)
+    CCDNO = slice(22, 24)
+    DTYPE = slice(24, 27)
+    EXTENSION = slice(28, None)
 
     extmap = {
         'ASC': 'txt',
         'FIT': 'fits',
         'SAS': 'txt',
     }
 
@@ -585,27 +594,27 @@
         'ras': 'raw_attitude',
         'ros': 'recon_orbit',
         'sum': 'summary',
         'tcs': 'raw_time_corr',
         'tcx': 'recon_time_corr',
     }
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 2:
-            raise multitool.UsageError ('make-sc-aliases requires exactly 2 arguments')
+    def invoke(self, args, **kwargs):
+        if len(args) != 2:
+            raise multitool.UsageError('make-sc-aliases requires exactly 2 arguments')
 
-        srcdir = Path (args[0])
-        destdir = Path (args[1])
+        srcdir = Path(args[0])
+        destdir = Path(args[1])
 
-        srcfiles = [x for x in srcdir.iterdir () if len (x.name) > 28]
+        srcfiles = [x for x in srcdir.iterdir() if len(x.name) > 28]
 
         # Do it.
 
-        idents = set ()
-        destdir.mkdir () # intentionally crash if exists; easiest approach
+        idents = set()
+        destdir.mkdir() # intentionally crash if exists; easiest approach
 
         for p in srcfiles:
             instr = p.name[self.INSTRUMENT]
             if instr != 'SC':
                 continue
 
             # none of these are actually useful for SC files:
@@ -615,80 +624,80 @@
             dtype = p.name[self.DTYPE]
             ext = p.name[self.EXTENSION]
 
             # One conflict, easy to resolve
             if dtype == 'SUM' and ext == 'ASC':
                 continue
 
-            dtype = self.dtypemap[dtype.lower ()]
+            dtype = self.dtypemap[dtype.lower()]
             ext = self.extmap[ext]
 
             ident = dtype
             if ident in idents:
-                cli.die ('short identifier clash: %r', ident)
-            idents.add (ident)
+                cli.die('short identifier clash: %r', ident)
+            idents.add(ident)
 
-            (destdir / (dtype + '.' + ext)).rellink_to (p)
+            (destdir / (dtype + '.' + ext)).rellink_to(p)
 
 
-class Shell (multitool.Command):
+class Shell(multitool.Command):
     # XXX we hardcode bash! and we copy/paste from environments/__init__.py
     name = 'shell'
     argspec = '<manifest>'
     summary = 'Start an interactive shell in the SAS environment.'
     help_if_no_args = False
     more_help = '''Due to the way SAS works, the path to a MANIFEST.nnnnn file in an ODF
 directory must be specified, and all operations work on the specified data
 set.'''
 
-    def invoke (self, args, **kwargs):
-        if len (args) != 1:
-            raise multitool.UsageError ('shell expects exactly 1 argument')
+    def invoke(self, args, **kwargs):
+        if len(args) != 1:
+            raise multitool.UsageError('shell expects exactly 1 argument')
 
-        env = SasEnvironment (args[0])
+        env = SasEnvironment(args[0])
 
         from tempfile import NamedTemporaryFile
-        with NamedTemporaryFile (delete=False) as f:
-            print ('''[ -e ~/.bashrc ] && source ~/.bashrc
+        with NamedTemporaryFile(delete=False, mode='wt') as f:
+            print('''[ -e ~/.bashrc ] && source ~/.bashrc
 PS1="SAS(%s) $PS1"
 rm %s''' % (env._obsid, f.name), file=f)
 
-        env.execvpe (['bash', '--rcfile', f.name, '-i'])
+        env.execvpe(['bash', '--rcfile', f.name, '-i'])
 
 
-class UpdateCcf (multitool.Command):
+class UpdateCcf(multitool.Command):
     name = 'update-ccf'
     argspec = ''
     summary = 'Update the SAS "current calibration files".'
     more_help = 'This executes an rsync command to make sure the files are up-to-date.'
     help_if_no_args = False
 
-    def invoke (self, args, **kwargs):
-        if len (args):
-            raise multitool.UsageError ('update-ccf expects no arguments')
+    def invoke(self, args, **kwargs):
+        if len(args):
+            raise multitool.UsageError('update-ccf expects no arguments')
 
-        sasdir = os.environ.get ('PWKIT_SAS')
+        sasdir = os.environ.get('PWKIT_SAS')
         if sasdir is None:
-            cli.die ('environment variable $PWKIT_SAS must be set')
+            cli.die('environment variable $PWKIT_SAS must be set')
 
-        os.chdir (os.path.join (sasdir, 'ccf'))
-        os.execvp ('rsync', ['rsync',
-                             '-av',
-                             '--delete',
-                             '--delete-after',
-                             '--force',
-                             '--include=*.CCF',
-                             '--exclude=*/',
-                             'xmm.esac.esa.int::XMM_VALID_CCF',
-                             '.'])
+        os.chdir(os.path.join(sasdir, 'ccf'))
+        os.execvp('rsync', ['rsync',
+                            '-av',
+                            '--delete',
+                            '--delete-after',
+                            '--force',
+                            '--include=*.CCF',
+                            '--exclude=*/',
+                            'xmm.esac.esa.int::XMM_VALID_CCF',
+                            '.'])
 
 
-class SasTool (multitool.Multitool):
+class SasTool(multitool.Multitool):
     cli_name = 'pkenvtool sas'
     summary = 'Run tools in the SAS environment.'
 
 
-def commandline (argv):
+def commandline(argv):
     from six import itervalues
-    tool = SasTool ()
-    tool.populate (itervalues (globals ()))
-    tool.commandline (argv)
+    tool = SasTool()
+    tool.populate(itervalues(globals()))
+    tool.commandline(argv)
```

### Comparing `pwkit-0.8.9/pwkit/environments/heasoft.py` & `pwkit-1.0.0/pwkit/environments/heasoft.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/__init__.py` & `pwkit-1.0.0/pwkit/environments/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2015 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2015, 2017 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 """pwkit.environments - working with external software environments
 
 Classes:
 
   Environment - base class for launching programs in an external environment.
@@ -21,222 +21,222 @@
 
 Standard usage is to create an `Environment` instance, then use its
 `launch(argv, ...)` method to run programs in the specified environment.
 `launch()` returns a `subprocess.Popen` instance that can be used in the
 standard ways.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
 """For reference: the Python docs state that Python automatically decodes
 Unicode environment variables as UTF-8 on non-Windows, so we don't need to be
 crazy about bytes-ifying values.
 
 """
-__all__ = str ('Environment prepend_environ_path prepend_path user_data_path').split ()
+__all__ = 'Environment prepend_environ_path prepend_path user_data_path'.split()
 
 import os, subprocess, sys
 
 from .. import cli
 from ..cli import multitool
 
 
-class Environment (object):
-    def modify_environment (self, environ):
+class Environment(object):
+    def modify_environment(self, environ):
         """Modify the passed-in dictionary of environment variables to be suitable for
         executing programs in this software environment. Make sure to copy
         os.environ() if you don't want to modify it for the current process.
 
         """
-        raise NotImplementedError ()
+        raise NotImplementedError()
 
 
-    def _preexec (self, env, **kwargs):
+    def _preexec(self, env, **kwargs):
         pass
 
 
-    def launch (self, argv, stdin=None, stdout=None, stderr=None,
-                close_fds=False, env=None, shell=False, cwd=None,
-                preexec_fn=None, **kwargs):
+    def launch(self, argv, stdin=None, stdout=None, stderr=None,
+               close_fds=False, env=None, shell=False, cwd=None,
+               preexec_fn=None, executable=None, **kwargs):
         if env is None:
             env = os.environ
 
-        env = self.modify_environment (env.copy ())
-        self._preexec (env, **kwargs)
-        return subprocess.Popen (argv, stdin=stdin, stdout=stdout,
-                                 stderr=stderr, close_fds=close_fds,
-                                 env=env, shell=shell, cwd=cwd,
-                                 preexec_fn=preexec_fn)
+        env = self.modify_environment(env.copy())
+        self._preexec(env, **kwargs)
+        return subprocess.Popen(argv, stdin=stdin, stdout=stdout,
+                                stderr=stderr, close_fds=close_fds,
+                                env=env, shell=shell, cwd=cwd,
+                                preexec_fn=preexec_fn, executable=executable)
 
-    def execvpe (self, argv, env=None, **kwargs):
+    def execvpe(self, argv, env=None, **kwargs):
         if env is None:
             env = os.environ
 
-        env = self.modify_environment (env.copy ())
-        self._preexec (env, **kwargs)
+        env = self.modify_environment(env.copy())
+        self._preexec(env, **kwargs)
         # unlike subprocess.Popen, execvpe doesn't use the new path to find
         # the program. But we're about to replace ourselves with the new
         # program, so no worries about mutating os.environ. If the exec fails
         # the mutation will remain, though.
         os.environ['PATH'] = env['PATH']
-        os.execvpe (argv[0], argv, env)
+        os.execvpe(argv[0], argv, env)
 
-    def slurp (self, **kwargs):
+    def slurp(self, **kwargs):
         from ..slurp import Slurper
-        return Slurper (subproc_factory=self.launch, **kwargs)
+        return Slurper(subproc_factory=self.launch, **kwargs)
 
-    def get_wrapout_wrapper (self, **kwargs):
+    def get_wrapout_wrapper(self, **kwargs):
         from ..cli.wrapout import Wrapper
-        w = Wrapper (**kwargs)
+        w = Wrapper(**kwargs)
         w.slurp_factory = self.slurp
         return w
 
 
-def prepend_path (orig, text, pathsep=os.pathsep):
+def prepend_path(orig, text, pathsep=os.pathsep):
     """Returns a $PATH-like environment variable with `text` prepended. `orig` is
     the original variable value, or None. `pathsep` is the character
     separating path elements, defaulting to `os.pathsep`.
 
     Example:
 
-    newpath = cli.prepend_path (oldpath, '/mypackage/bin')
+    newpath = cli.prepend_path(oldpath, '/mypackage/bin')
 
     See also `prepend_environ_path`.
 
     """
     if orig is None:
         orig = ''
-    if not len (orig):
+    if not len(orig):
         return text
-    return ''.join ([text, pathsep, orig])
+    return ''.join([text, pathsep, orig])
 
 
-def prepend_environ_path (env, name, text, pathsep=os.pathsep):
+def prepend_environ_path(env, name, text, pathsep=os.pathsep):
     """Prepend `text` into a $PATH-like environment variable. `env` is a
     dictionary of environment variables and `name` is the variable name.
     `pathsep` is the character separating path elements, defaulting to
     `os.pathsep`. The variable will be created if it is not already in `env`.
     Returns `env`.
 
     Example::
 
-      prepend_environ_path (env, str('PATH'), str('/mypackage/bin'))
+      prepend_environ_path(env, 'PATH', '/mypackage/bin')
 
-    The `str` calls are necessary for Python 2/3 compatibility.
+    The `name` and `text` arguments should be `str` objects; that is, bytes in
+    Python 2 and Unicode in Python 3. Literal strings will be OK unless you
+    use the ``from __future__ import unicode_literals`` feature.
 
     """
-    env[name] = prepend_path (env.get (name), text, pathsep=pathsep)
+    env[name] = prepend_path(env.get(name), text, pathsep=pathsep)
     return env
 
 
-def _make_user_data_pather ():
-    datadir = os.environ.get (str('XDG_DATA_HOME'),
-                              str(os.path.expanduser ('~/.local/share')))
+def _make_user_data_pather():
+    datadir = os.environ.get('XDG_DATA_HOME', os.path.expanduser('~/.local/share'))
 
-    def pathfunc (*args):
-        return os.path.join (datadir, *args)
+    def pathfunc(*args):
+        return os.path.join(datadir, *args)
 
     return pathfunc
 
-user_data_path = _make_user_data_pather ()
+user_data_path = _make_user_data_pather()
 
 
 # Command-line access
 
-class DefaultExecCommand (multitool.Command):
+class DefaultExecCommand(multitool.Command):
     name = 'exec'
     argspec = '<command> [args...]'
     summary = 'Run a program in the environment.'
 
-    def invoke (self, args, envclass=None, **kwargs):
-        if len (args) < 1:
-            raise multitool.UsageError ('exec requires at least 1 argument')
+    def invoke(self, args, envclass=None, **kwargs):
+        if len(args) < 1:
+            raise multitool.UsageError('exec requires at least 1 argument')
 
-        envclass ().execvpe (args)
+        envclass().execvpe(args)
 
 
-class DefaultShellCommand (multitool.Command):
+class DefaultShellCommand(multitool.Command):
     # XXX we hardcode bash!
     name = 'shell'
     argspec = ''
     summary = 'Start an interactive shell in the environment.'
     help_if_no_args = False
 
-    def invoke (self, args, envname=None, envclass=None, **kwargs):
-        if len (args):
-            raise multitool.UsageError ('shell expects no arguments')
+    def invoke(self, args, envname=None, envclass=None, **kwargs):
+        if len(args):
+            raise multitool.UsageError('shell expects no arguments')
 
         from tempfile import NamedTemporaryFile
-        with NamedTemporaryFile (mode='wt', delete=False) as f:
-            print ('''[ -e ~/.bashrc ] && source ~/.bashrc
+        with NamedTemporaryFile(mode='wt', delete=False) as f:
+            print('''[ -e ~/.bashrc ] && source ~/.bashrc
 PS1="%s $PS1"
 rm %s''' % (envname, f.name), file=f)
 
-        envclass ().execvpe (['bash',
-                              '--rcfile', f.name,
-                              '-i'])
+        envclass().execvpe(['bash',
+                            '--rcfile', f.name,
+                            '-i'])
 
 
-class DefaultTool (multitool.Multitool):
-    def __init__ (self, envname, envclass, module):
-        super (DefaultTool, self).__init__ ()
+class DefaultTool(multitool.Multitool):
+    def __init__(self, envname, envclass, module):
+        super(DefaultTool, self).__init__()
         self.envname = envname
         self.envclass = envclass
         self.module = module
 
         self.cli_name = 'pkenvtool ' + envname
         self.summary = 'Run tools in the %s environment.' % envname
 
 
-    def invoke_command (self, cmd, args, **kwargs):
-        return super (DefaultTool, self).invoke_command (cmd, args,
-                                                         envname=self.envname,
-                                                         envclass=self.envclass,
-                                                         module=self.module,
-                                                         **kwargs)
+    def invoke_command(self, cmd, args, **kwargs):
+        return super(DefaultTool, self).invoke_command(cmd, args,
+                                                       envname=self.envname,
+                                                       envclass=self.envclass,
+                                                       module=self.module,
+                                                       **kwargs)
 
 
-def _default_env_commandline (envname, module, argv):
+def _default_env_commandline(envname, module, argv):
     from six import itervalues
 
-    for name in dir (module):
-        v = getattr (module, name)
-        if v is not Environment and issubclass (v, Environment):
+    for name in dir(module):
+        v = getattr(module, name)
+        if v is not Environment and issubclass(v, Environment):
             envclass = v
             break
     else:
-        cli.die ('internal error: cannot identify environment class for %s',
-                 envname)
+        cli.die('internal error: cannot identify environment class for %s', envname)
 
-    tool = DefaultTool (envname, envclass, module)
-    tool.populate (itervalues (globals ()))
-    tool.commandline (argv)
+    tool = DefaultTool(envname, envclass, module)
+    tool.populate(itervalues(globals()))
+    tool.commandline(argv)
 
 
-def commandline (argv=sys.argv):
-    cli.propagate_sigint ()
-    cli.backtrace_on_usr1 ()
-    cli.unicode_stdio ()
+def commandline(argv=sys.argv):
+    cli.propagate_sigint()
+    cli.backtrace_on_usr1()
+    cli.unicode_stdio()
 
-    if len (argv) < 2 or argv[1] in ('-h', '--help'):
-        print ('''usage: pkenvtool <environment> [args...]
+    if len(argv) < 2 or argv[1] in ('-h', '--help'):
+        print('''usage: pkenvtool <environment> [args...]
 
 Where acceptable "args" depend on the environment in question.''')
         return
 
     envname = argv[1]
-    if not len (envname) or envname[0] == '.':
-        cli.die ('illegal environment name %r', envname)
+    if not len(envname) or envname[0] == '.':
+        cli.die('illegal environment name %r', envname)
 
     from importlib import import_module
 
     try:
-        envmod = import_module ('.' + envname, package=__package__)
+        envmod = import_module('.' + envname, package=__package__)
     except Exception:
-        cli.die ('unable to load module for environment %r', envname)
+        cli.die('unable to load module for environment %r', envname)
 
     modargv = ['pkenvtool ' + argv[1]] + argv[2:]
 
-    if hasattr (envmod, 'commandline'):
-        envmod.commandline (modargv)
+    if hasattr(envmod, 'commandline'):
+        envmod.commandline(modargv)
     else:
-        _default_env_commandline (envname, envmod, modargv)
+        _default_env_commandline(envname, envmod, modargv)
```

### Comparing `pwkit-0.8.9/pwkit/environments/jupyter/__init__.py` & `pwkit-1.0.0/pwkit/environments/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/ciao/data.py` & `pwkit-1.0.0/pwkit/environments/ciao/data.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/ciao/__init__.py` & `pwkit-1.0.0/pwkit/environments/ciao/__init__.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/ciao/analysis.py` & `pwkit-1.0.0/pwkit/environments/ciao/analysis.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/spwglue.py` & `pwkit-1.0.0/pwkit/environments/casa/spwglue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,108 +1,110 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2013-2015 Peter Williams <peter@newton.cx> and collaborators
+# Copyright 2013-2015, 2017 Peter Williams <peter@newton.cx> and collaborators
 # Licensed under the MIT License
 
 """pwkit.environments.casa.spwglue - merge spectral windows in a MeasurementSet
 
 I find that merging windows in this way offers a lot of advantages. This
 procesing step is very slow, however.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Progress Config spwglue spwglue_cli').split ()
+__all__ = str('Progress Config spwglue spwglue_cli').split()
 
 import six
 from six.moves import range
 import numpy as np
 from ... import binary_type, text_type
 from ...kwargv import ParseKeywords, Custom
 from ...cli import check_usage, die
 from . import util
 from .util import sanitize_unicode as b
 
-def _sfmt (t):
+def _sfmt(t):
     # Format timespan (t in seconds)
     if t < 90:
         return '%.0fs' % t
     if t < 4000:
         return '%.1fm' % (t / 60)
     if t < 90000:
         return '%.1fh' % (t / 3600)
     return '%.1fd' % (t / 86400)
 
 
-class Progress (object):
+class Progress(object):
     """This could be split out; it's useful."""
     elapsed = None
 
     prefix = None
     totitems = None
     tstart = None
     unbufout = None
     tlastprint = None
 
-    def __enter__ (self):
+    def __enter__(self):
         return self
 
 
-    def __exit__ (self, etype, eval, etb):
+    def __exit__(self, etype, eval, etb):
         if self.tstart is not None:
-            self.finish (etype is None)
+            self.finish(etype is None)
         return False
 
 
-    def start (self, totitems, prefix=''):
+    def start(self, totitems, prefix=''):
         import time, os
         self.totitems = totitems
         self.prefix = prefix
-        self.tstart = time.time ()
+        self.tstart = time.time()
         self.tlastprint = 0
-        self.unbufout = os.fdopen (os.dup (1), 'w', 0)
+        self.unbufout = os.fdopen(os.dup(1), 'wb', 0)
 
 
-    def progress (self, curitems):
+    def progress(self, curitems):
         import time
-        now = time.time ()
+        now = time.time()
         if now - self.tlastprint < 1:
             return
 
         elapsed = now - self.tstart
-        li = len (str (self.totitems))
+        li = len(str(self.totitems))
 
         if curitems == 0:
             msg = '%5.1f%% (%*d/%d) elapsed %s ETA %s total %s' % \
-                  (0., li, 0, self.totitems, _sfmt (elapsed), '?', '?')
+                  (0., li, 0, self.totitems, _sfmt(elapsed), '?', '?')
         else:
             pct = 100. * curitems / self.totitems
             total = 1. * elapsed * self.totitems / curitems
             eta = total - elapsed
             msg = '%5.1f%% (%*d/%d) elapsed %s ETA %s total %s' % \
-                  (pct, li, curitems, self.totitems, _sfmt (elapsed),
-                   _sfmt (eta), _sfmt (total))
+                  (pct, li, curitems, self.totitems, _sfmt(elapsed),
+                   _sfmt(eta), _sfmt(total))
 
-        print (self.prefix, msg.ljust (60), end='\r', file=self.unbufout)
+        full_msg = '%s %s\r' % (self.prefix, msg.ljust(60))
+        self.unbufout.write(full_msg.encode('utf8'))
         self.tlastprint = now
 
 
-    def finish (self, success=True):
+    def finish(self, success=True):
         import time
-        now = time.time ()
+        now = time.time()
         self.elapsed = now - self.tstart
 
         if not success:
-            print (file=self.unbufout)
+            print(file=self.unbufout)
         else:
             msg = '100.0%% (%d/%d) elapsed %s ETA 0s total %s' % \
-                  (self.totitems, self.totitems, _sfmt (self.elapsed),
-                   _sfmt (self.elapsed))
-            print (self.prefix, msg.ljust (60), file=self.unbufout)
+                  (self.totitems, self.totitems, _sfmt(self.elapsed),
+                   _sfmt(self.elapsed))
+            full_msg = '%s %s\n' % (self.prefix, msg.ljust(60))
+            self.unbufout.write(full_msg.encode('utf8'))
 
-        self.unbufout.close ()
+        self.unbufout.close()
         self.tstart = self.unbufout = None
         self.tlastprint = self.totitems = None
 
 
 spwglue_doc = \
 """
 casatask spwglue vis=MS out=MS mapping=SPWi-SPWj[,SPWl-SPWm,...]
@@ -133,43 +135,43 @@
   Another optional field ID number, used for fixing up MSes where one
   pointing is accidentally assigned two field IDs. Both "field" and
   "hackfield" are extracted from the dataset, but the output is changed
   so that all the records refer to "field" only. Disallowed if "field" is
   a list of fields.
 
 meanbp=
-  Path to a pickled numpy array giving the mean amplitude bandpass of the
+  Path to a saved numpy array giving the mean amplitude bandpass of the
   *glued* SPWs. The data are divided by the square of this array, thereby
   taking out this effect. (Each visibility is affected by the bandpasses of
   the two antennas contributing to its baseline, which is why we square the
   bandpass solution.) This makes it easier to run automated RFI flaggers on
   the data without losing excessive numbers of edge channels.
 
 corr_to_main=false
   If true, move the CORRECTED_DATA column to the main DATA column while gluing.
 
 loglevel=
   Logging detail level. Default is info. Options are
     severe warn info info1 info2 info3 info4 info5 debug1 debug2 debugging
 """
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
-    out = Custom ([str], required=True)
-
-    @Custom ([str], required=True)
-    def mapping (bits):
-        def parse (item):
-            t1, t2 = map (int, item.split ('-'))
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
+    out = Custom([str], required=True)
+
+    @Custom([str], required=True)
+    def mapping(bits):
+        def parse(item):
+            t1, t2 = list(map(int, item.split('-')))
             assert t2 >= t1, 'can\'t do reverse-order mappings'
-            return range (t1, t2 + 1)
+            return list(range(t1, t2 + 1))
         try:
-            return [parse (b) for b in bits]
+            return [parse(b) for b in bits]
         except Exception as e:
-            die ('unparseable or illegal "mapping" value "%s": %s', ','.join (bits), e)
+            die('unparseable or illegal "mapping" value "%s": %s', ','.join(bits), e)
 
     field = [int]
     hackfield = int
     meanbp = str
     corr_to_main = False
 
     loglevel = 'info' # XXXXXX
@@ -177,50 +179,50 @@
 
 # Different things that we do with columns in the SPECTRAL_WINDOW table:
 # match  - scalar values that should all agree
 # first  - scalar values and we'll keep the first
 # scsum  - scalar values and we'll keep the sum
 # concat - vectors that we'll concatenate
 # empty  - column should be empty (ndim = -1)
-_spw_match_cols = frozenset ('MEAS_FREQ_REF FLAG_ROW FREQ_GROUP FREQ_GROUP_NAME '
-                             'IF_CONV_CHAIN NET_SIDEBAND BBC_NO'.split ())
-_spw_first_cols = frozenset ('DOPPLER_ID REF_FREQUENCY NAME'.split ())
-_spw_scsum_cols = frozenset ('NUM_CHAN TOTAL_BANDWIDTH'.split ())
-_spw_concat_cols = frozenset ('CHAN_FREQ CHAN_WIDTH EFFECTIVE_BW RESOLUTION'.split ())
-_spw_empty_cols = frozenset ('ASSOC_SPW_ID ASSOC_NATURE'.split ())
+_spw_match_cols = frozenset('MEAS_FREQ_REF FLAG_ROW FREQ_GROUP FREQ_GROUP_NAME '
+                            'IF_CONV_CHAIN NET_SIDEBAND BBC_NO'.split())
+_spw_first_cols = frozenset('DOPPLER_ID REF_FREQUENCY NAME'.split())
+_spw_scsum_cols = frozenset('NUM_CHAN TOTAL_BANDWIDTH'.split())
+_spw_concat_cols = frozenset('CHAN_FREQ CHAN_WIDTH EFFECTIVE_BW RESOLUTION'.split())
+_spw_empty_cols = frozenset('ASSOC_SPW_ID ASSOC_NATURE'.split())
 
 
-def _spwproc_match (spwtb, colname, inspws, outdata):
+def _spwproc_match(spwtb, colname, inspws, outdata):
     theval = None
 
     for inspw in inspws:
-        v = b(spwtb.getcell (b(colname), inspw))
+        v = b(spwtb.getcell(b(colname), inspw))
         if theval is None:
             theval = v
         elif theval != v:
-            die ('glued spws should all have same value of %s column but don\'t', colname)
+            die('glued spws should all have same value of %s column but don\'t', colname)
 
     outdata[colname] = theval
 
 
-def _spwproc_first (spwtb, colname, inspws, outdata):
-    outdata[colname] = b(spwtb.getcell (b(colname), inspws[0]))
+def _spwproc_first(spwtb, colname, inspws, outdata):
+    outdata[colname] = b(spwtb.getcell(b(colname), inspws[0]))
 
 
-def _spwproc_scsum (spwtb, colname, inspws, outdata):
+def _spwproc_scsum(spwtb, colname, inspws, outdata):
     sum = 0
     for inspw in inspws:
-        sum += spwtb.getcell (b(colname), inspw)
+        sum += spwtb.getcell(b(colname), inspw)
     outdata[colname] = sum
 
 
-def _spwproc_concat (spwtb, colname, inspws, outdata):
+def _spwproc_concat(spwtb, colname, inspws, outdata):
     clist = []
     for inspw in inspws:
-        clist += b(list (spwtb.getcell (b(colname), inspw)))
+        clist += b(list(spwtb.getcell(b(colname), inspw)))
     outdata[colname] = clist
 
 
 # Similar info for the main visibility data:
 # ident   - define a unique visibility dump
 # smatch  - scalars that should match precisely
 # sapprox - scalars that should match approximately (to 1e-5) [1]
@@ -231,322 +233,321 @@
 # empty   - columns that should be blank
 #
 # [1] This feature implemented since EVLA dataset
 # 11A-266.sb4865287.eb4875705.55772.08031621527.ms has 22 rows out of ~9
 # million that have an EXPOSURE value that differs from the others by 1 part
 # in ~10^9.
 
-_vis_ident_cols = 'ARRAY_ID FIELD_ID TIME ANTENNA1 ANTENNA2'.split ()
-_vis_smatch_cols = frozenset ('''FEED1 FEED2 OBSERVATION_ID PROCESSOR_ID
-                              SCAN_NUMBER STATE_ID'''.split ())
-_vis_sapprox_cols = frozenset ('EXPOSURE INTERVAL TIME_CENTROID'.split ())
-_vis_vmatch_cols = frozenset ('UVW WEIGHT SIGMA'.split ())
-_vis_or_cols = frozenset ('FLAG_ROW'.split ())
-_vis_pconcat_cols = frozenset ('FLAG DATA MODEL_DATA CORRECTED_DATA WEIGHT_SPECTRUM'.split ())
-_vis_data_cols = frozenset ('DATA MODEL_DATA CORRECTED_DATA'.split ())
-_vis_empty_cols = frozenset ('FLAG_CATEGORY'.split ())
+_vis_ident_cols = 'ARRAY_ID FIELD_ID TIME ANTENNA1 ANTENNA2'.split()
+_vis_smatch_cols = frozenset('FEED1 FEED2 OBSERVATION_ID PROCESSOR_ID SCAN_NUMBER STATE_ID'.split())
+_vis_sapprox_cols = frozenset('EXPOSURE INTERVAL TIME_CENTROID'.split())
+_vis_vmatch_cols = frozenset('UVW WEIGHT SIGMA'.split())
+_vis_or_cols = frozenset('FLAG_ROW'.split())
+_vis_pconcat_cols = frozenset('FLAG DATA MODEL_DATA CORRECTED_DATA WEIGHT_SPECTRUM'.split())
+_vis_data_cols = frozenset('DATA MODEL_DATA CORRECTED_DATA'.split())
+_vis_empty_cols = frozenset('FLAG_CATEGORY'.split())
 _vis_pconcat_dtypes = {'FLAG': np.bool, 'DATA': np.complex128, 'MODEL_DATA': np.complex128,
                        'CORRECTED_DATA': np.complex128, 'WEIGHT_SPECTRUM': np.float64}
 
 _np_converters = {
     #np.bool_: bool,
     #np.int32: int,
     #np.float64: float,
     np.ndarray: lambda x: x,
     np.bool_: np.int32,
     np.int32: lambda x: x,
     np.float64: lambda x: x,
     int: np.int32,
 }
 
-def spwglue (cfg):
-    nout = len (cfg.out)
-    nfield = len (cfg.field)
+def spwglue(cfg):
+    nout = len(cfg.out)
+    nfield = len(cfg.field)
 
     if (nout != 1 or nfield != 0) and (nout != nfield):
-        die ('%d outputs requested, but only %d fields listed', nout, nfield)
+        die('%d outputs requested, but only %d fields listed', nout, nfield)
     if nout != 1 and cfg.hackfield is not None:
-        die ('"hackfield" keyword is not compatible with multiple output sets')
+        die('"hackfield" keyword is not compatible with multiple output sets')
 
     if nfield == 0:
         cfg.field = [None]
 
-    with Progress () as p:
-        for idx, (out, field) in enumerate (zip (cfg.out, cfg.field)):
-            _spwglue (cfg, p, out, field, nfield, idx)
+    with Progress() as p:
+        for idx, (out, field) in enumerate(zip(cfg.out, cfg.field)):
+            _spwglue(cfg, p, out, field, nfield, idx)
 
 
-def fillsmall (path, rows):
-    tb = util.tools.table ()
-    tb.open (b(path), nomodify=False)
-    tb.addrows (len (rows))
+def fillsmall(path, rows):
+    tb = util.tools.table()
+    tb.open(b(path), nomodify=False)
+    tb.addrows(len(rows))
 
     try:
-        for i, data in enumerate (rows):
-            for col, val in six.iteritems (data):
-                tb.putcell (b(col), i, val)
+        for i, data in enumerate(rows):
+            for col, val in six.iteritems(data):
+                tb.putcell(b(col), i, val)
     except Exception as e:
-        raise Exception ('error putting: %d %s %s (%s): %s' % (i, col, val, val.__class__, e))
+        raise Exception('error putting: %d %s %s (%s): %s' % (i, col, val, val.__class__, e))
 
-    tb.close ()
+    tb.close()
 
 
-def _spwglue (cfg, prog, thisout, thisfield, nfields, fieldidx):
+def _spwglue(cfg, prog, thisout, thisfield, nfields, fieldidx):
     import os.path
 
     if cfg.hackfield is not None:
         assert thisfield is not None
 
-    nout = len (cfg.mapping)
+    nout = len(cfg.mapping)
 
     if cfg.meanbp is None:
         invsqmeanbp = None
     else:
         try:
-            invsqmeanbp = np.load (cfg.meanbp)
+            invsqmeanbp = np.load(cfg.meanbp)
         except Exception as e:
-            die ('couldn\'t open bandpass file "%s": %s (%s)', cfg.meanbp,
-                 e, e.__class__.__name__)
+            die('couldn\'t open bandpass file "%s": %s (%s)', cfg.meanbp,
+                e, e.__class__.__name__)
 
-        if np.any (invsqmeanbp <= 0):
-            die ('illegal bandpass file "%s": some values are nonpositive',
-                 cfg.meanbp)
+        if np.any(invsqmeanbp <= 0):
+            die('illegal bandpass file "%s": some values are nonpositive',
+                cfg.meanbp)
 
         invsqmeanbp **= -2
 
     # Read in spw and dd info and make sure everything is in order.
 
-    tb = util.tools.table ()
-    tb.open (b(os.path.join (cfg.vis, 'SPECTRAL_WINDOW')))
-    spwcols = tb.colnames ()
-    spwout = [dict () for i in range (nout)]
+    tb = util.tools.table()
+    tb.open(b(os.path.join(cfg.vis, 'SPECTRAL_WINDOW')))
+    spwcols = tb.colnames()
+    spwout = [dict() for i in range(nout)]
 
     for col in spwcols:
         if col in _spw_match_cols:
-            for i in range (nout):
-                _spwproc_match (tb, col, cfg.mapping[i], spwout[i])
+            for i in range(nout):
+                _spwproc_match(tb, col, cfg.mapping[i], spwout[i])
         elif col in _spw_first_cols:
-            for i in range (nout):
-                _spwproc_first (tb, col, cfg.mapping[i], spwout[i])
+            for i in range(nout):
+                _spwproc_first(tb, col, cfg.mapping[i], spwout[i])
         elif col in _spw_scsum_cols:
-            for i in range (nout):
-                _spwproc_scsum (tb, col, cfg.mapping[i], spwout[i])
+            for i in range(nout):
+                _spwproc_scsum(tb, col, cfg.mapping[i], spwout[i])
         elif col in _spw_concat_cols:
-            for i in range (nout):
-                _spwproc_concat (tb, col, cfg.mapping[i], spwout[i])
+            for i in range(nout):
+                _spwproc_concat(tb, col, cfg.mapping[i], spwout[i])
         elif col in _spw_empty_cols:
             pass
         else:
-            die ('don\'t know how to handle SPECTRAL_WINDOW column "%s" in %s"',
-                 col, cfg.vis)
+            die('don\'t know how to handle SPECTRAL_WINDOW column "%s" in %s"',
+                col, cfg.vis)
 
-    numchans = tb.getcol (b'NUM_CHAN')
-    tb.close ()
+    numchans = tb.getcol(b'NUM_CHAN')
+    tb.close()
     inspw2outspw = {}
 
-    for i in range (nout):
+    for i in range(nout):
         ofs = 0
 
         for inspw in cfg.mapping[i]:
             if inspw in inspw2outspw:
-                die ('spw %d gets duplicated in mapping', inspw)
+                die('spw %d gets duplicated in mapping', inspw)
             inspw2outspw[inspw] = (i, ofs)
             ofs += numchans[inspw]
 
     # We only handle 1:1 mappings between DD and SPW.
-    tb.open (b(os.path.join (cfg.vis, 'DATA_DESCRIPTION')))
-    ddflagrows = np.asarray (tb.getcol (b'FLAG_ROW'))
-    ddpids = np.asarray (tb.getcol (b'POLARIZATION_ID'))
-    ddspws = np.asarray (tb.getcol (b'SPECTRAL_WINDOW_ID'))
-    tb.close ()
+    tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
+    ddflagrows = np.asarray(tb.getcol(b'FLAG_ROW'))
+    ddpids = np.asarray(tb.getcol(b'POLARIZATION_ID'))
+    ddspws = np.asarray(tb.getcol(b'SPECTRAL_WINDOW_ID'))
+    tb.close()
     indd2outdd = {}
-    ddout = [{'SPECTRAL_WINDOW_ID': np.int32(i)} for i in range (nout)]
+    ddout = [{'SPECTRAL_WINDOW_ID': np.int32(i)} for i in range(nout)]
 
-    for i in range (ddspws.size):
+    for i in range(ddspws.size):
         inspw = ddspws[i]
 
         if inspw not in inspw2outspw:
             continue # this dd gets dropped in the processing
 
         outspw, outofs = inspw2outspw[inspw]
         indd2outdd[i] = (outspw, outofs)
 
-        fr = ddout[outspw].get ('FLAG_ROW')
+        fr = ddout[outspw].get('FLAG_ROW')
         if fr is None:
             ddout[outspw]['FLAG_ROW'] = np.int32(ddflagrows[i]) # hack: have to convert bool->int for some reason
         elif ddflagrows[i] != fr:
-            die ('dd %d glued into output spw %d has different FLAG_ROW ident', i, outspw)
+            die('dd %d glued into output spw %d has different FLAG_ROW ident', i, outspw)
 
-        pid = ddout[outspw].get ('POLARIZATION_ID')
+        pid = ddout[outspw].get('POLARIZATION_ID')
         if pid is None:
             ddout[outspw]['POLARIZATION_ID'] = ddpids[i]
         elif ddpids[i] != pid:
-            die ('dd %d glued into output spw %d has different POLARIZATION ident', i, outspw)
+            die('dd %d glued into output spw %d has different POLARIZATION ident', i, outspw)
 
     # We don't actually do any sanity checking with the SOURCE table, but we
     # do need to modify it. Let's just load it up here while we're loading up
     # all of the other small tables.
 
-    tb = util.tools.table ()
-    tb.open (b(os.path.join (cfg.vis, 'SOURCE')))
-    srccols = [c for c in tb.colnames ()
-               if tb.iscelldefined (c, 0)] # at least POSITION is undefined
-    srckeys = set ()
+    tb = util.tools.table()
+    tb.open(b(os.path.join(cfg.vis, 'SOURCE')))
+    srccols = [c for c in tb.colnames()
+               if tb.iscelldefined(c, 0)] # at least POSITION is undefined
+    srckeys = set()
     srcout = []
 
-    for i in range (tb.nrows ()):
-        data = dict ((c, b(tb.getcell (b(c), i))) for c in srccols)
-        m = inspw2outspw.get (data['SPECTRAL_WINDOW_ID'])
+    for i in range(tb.nrows()):
+        data = dict((c, b(tb.getcell(b(c), i))) for c in srccols)
+        m = inspw2outspw.get(data['SPECTRAL_WINDOW_ID'])
         if m is None:
             continue # this spw is being dropped
 
         data['SPECTRAL_WINDOW_ID'] = np.int32(m[0])
         key = (data['SOURCE_ID'], data['TIME'], data['INTERVAL'], m[0])
 
         if key in srckeys:
             # XXX: should verify that rest of data are identical, but too lazy.
             continue
 
-        srcout.append (data)
-        srckeys.add (key)
+        srcout.append(data)
+        srckeys.add(key)
 
     # Need this for buffer prealloc
 
-    tb.open (b(os.path.join (cfg.vis, 'POLARIZATION')))
-    numcorrs = tb.getcol (b'NUM_CORR')
-    tb.close ()
+    tb.open(b(os.path.join(cfg.vis, 'POLARIZATION')))
+    numcorrs = tb.getcol(b'NUM_CORR')
+    tb.close()
 
     # We've done all the preparation we can. Time to start copying. tb.copy()
     # will clobber existing tables, so do our best to ensure that there isn't
     # anything preexisting so far. Of course someone could put a table in the
     # destination between this mkdir and the actual copy.
 
-    os.mkdir (thisout)
+    os.mkdir(thisout)
 
     # Copy the overall table structure without contents.
 
-    tb.open (b(cfg.vis))
-    tb.copy (newtablename=b(thisout), deep=True, valuecopy=True,
-             norows=True).close () # copy() returns the new table.
-    tb.close ()
+    tb.open(b(cfg.vis))
+    tb.copy(newtablename=b(thisout), deep=True, valuecopy=True,
+            norows=True).close() # copy() returns the new table.
+    tb.close()
 
-    for item in os.listdir (cfg.vis):
-        if not os.path.exists (os.path.join (cfg.vis, item, 'table.dat')):
+    for item in os.listdir(cfg.vis):
+        if not os.path.exists(os.path.join(cfg.vis, item, 'table.dat')):
             continue
-        if item in 'SPECTRAL_WINDOW DATA_DESCRIPTION SOURCE'.split ():
+        if item in 'SPECTRAL_WINDOW DATA_DESCRIPTION SOURCE'.split():
             continue # will handle these manually
         if item == 'SYSPOWER':
             continue # XXX; large and unused
         if item == 'SORTED_TABLE':
             continue # XXX; copies main data rows; not sure what to do about it
 
-        tb.open (b(os.path.join (cfg.vis, item)))
-        tb.copy (b(os.path.join (thisout, item)), deep=False, valuecopy=True,
-                 norows=False).close ()
-        tb.close ()
+        tb.open(b(os.path.join(cfg.vis, item)))
+        tb.copy(b(os.path.join(thisout, item)), deep=False, valuecopy=True,
+                norows=False).close()
+        tb.close()
 
     # The rewritten small tables.
 
-    fillsmall (os.path.join (thisout, 'SPECTRAL_WINDOW'), spwout)
-    fillsmall (os.path.join (thisout, 'DATA_DESCRIPTION'), ddout)
-    fillsmall (os.path.join (thisout, 'SOURCE'), srcout)
+    fillsmall(os.path.join(thisout, 'SPECTRAL_WINDOW'), spwout)
+    fillsmall(os.path.join(thisout, 'DATA_DESCRIPTION'), ddout)
+    fillsmall(os.path.join(thisout, 'SOURCE'), srcout)
 
     # Rewriting the main table.
 
-    tb.open (b(cfg.vis))
-    colnames = [c for c in tb.colnames ()
+    tb.open(b(cfg.vis))
+    colnames = [c for c in tb.colnames()
                 if c not in _vis_empty_cols]
     nchunk = 1024
 
-    dt = util.tools.table ()
-    dt.open (b(thisout), nomodify=False)
+    dt = util.tools.table()
+    dt.open(b(thisout), nomodify=False)
 
     if cfg.corr_to_main:
-        dt.removecols ([b'CORRECTED_DATA'])
+        dt.removecols([b'CORRECTED_DATA'])
 
     outrow = 0
 
-    for outspw in range (nout):
-        q = ' or '.join ('DATA_DESC_ID == %d' % t[0] for t in six.iteritems (indd2outdd)
-                         if t[1][0] == outspw)
+    for outspw in range(nout):
+        q = ' or '.join('DATA_DESC_ID == %d' % t[0] for t in six.iteritems(indd2outdd)
+                        if t[1][0] == outspw)
         if cfg.hackfield is not None:
             q = '(FIELD_ID == %s or FIELD_ID == %s) and (%s)' % (thisfield, cfg.hackfield, q)
         elif thisfield is not None:
             q = 'FIELD_ID == %s and (%s)' % (thisfield, q)
         if cfg.hackfield is not None:
             sortlist = 'ARRAY_ID, TIME, ANTENNA1, ANTENNA2, DATA_DESC_ID'
         else:
             sortlist = 'ARRAY_ID, FIELD_ID, TIME, ANTENNA1, ANTENNA2, DATA_DESC_ID'
-        st = tb.query (b(q), sortlist=b(sortlist))
+        st = tb.query(b(q), sortlist=b(sortlist))
         inrow = 0
-        nq = st.nrows ()
+        nq = st.nrows()
 
         ncorr = numcorrs[ddout[outspw]['POLARIZATION_ID']]
         nchan = spwout[outspw]['NUM_CHAN']
         curident = None
         curout = {}
 
         if invsqmeanbp is not None and nchan != invsqmeanbp.size:
-            die ('need to apply bandpass of %d channels, but output spw %d has '
-                 '%d channels', invsqmeanbp.size, outspw, nchan)
+            die('need to apply bandpass of %d channels, but output spw %d has '
+                '%d channels', invsqmeanbp.size, outspw, nchan)
 
         for col in colnames:
             if col in _vis_pconcat_cols:
-                curout[col] = np.zeros ((ncorr, nchan), dtype=_vis_pconcat_dtypes[col])
+                curout[col] = np.zeros((ncorr, nchan), dtype=_vis_pconcat_dtypes[col])
             else:
                 curout[col] = None
 
-        def dump ():
+        def dump():
             # increment outrow after calling.
-            dt.addrows (1)
+            dt.addrows(1)
             for col in colnames:
                 v = curout[col]
-                v = _np_converters[v.__class__] (v)
+                v = _np_converters[v.__class__](v)
 
                 if invsqmeanbp is not None and col in _vis_data_cols:
                     v *= invsqmeanbp
 
                 if not cfg.corr_to_main:
-                    dt.putcell (b(col), outrow, v)
+                    dt.putcell(b(col), outrow, v)
                 elif col == 'DATA':
                     pass # ignore; will be overwritten by CORRECTED_DATA
                 else:
                     if col == 'CORRECTED_DATA':
                         outcol = 'DATA'
                     else:
                         outcol = col
-                    dt.putcell (b(outcol), outrow, v)
+                    dt.putcell(b(outcol), outrow, v)
 
-                if isinstance (v, np.ndarray):
-                    v.fill (0)
+                if isinstance(v, np.ndarray):
+                    v.fill(0)
                 else:
                     curout[col] = None
 
-        prog.start (nq, '%d/%d' % (nout * fieldidx + outspw + 1, nout * nfields))
+        prog.start(nq, '%d/%d' % (nout * fieldidx + outspw + 1, nout * nfields))
 
         while inrow < nq:
-            prog.progress (inrow)
+            prog.progress(inrow)
 
             vdata = {}
             for col in colnames:
-                vdata[col] = st.getcol (col, inrow, nchunk)
+                vdata[col] = st.getcol(col, inrow, nchunk)
 
             nread = vdata['TIME'].size
 
             if cfg.hackfield is not None:
-                vdata['FIELD_ID'].fill (thisfield)
+                vdata['FIELD_ID'].fill(thisfield)
 
-            for i in range (nread):
+            for i in range(nread):
                 outspw, outofs = indd2outdd[vdata['DATA_DESC_ID'][i]]
-                newident = tuple (vdata[c][i] for c in _vis_ident_cols)
+                newident = tuple(vdata[c][i] for c in _vis_ident_cols)
 
                 if newident != curident:
                     # Starting a new record
                     if curident is not None:
-                        dump ()
+                        dump()
                         outrow += 1
                     curident = newident
 
                     for col in colnames:
                         if (col in _vis_ident_cols or
                             col in _vis_smatch_cols or
                             col in _vis_sapprox_cols or
@@ -556,49 +557,49 @@
                             curout[col] = vdata[col][...,i]
                         elif col in _vis_pconcat_cols:
                             d = vdata[col][...,i]
                             curout[col][:,outofs:outofs+d.shape[1]] = d
                         elif col == 'DATA_DESC_ID':
                             curout['DATA_DESC_ID'] = outspw
                         else:
-                            die ('unhandled vis column %s', col)
+                            die('unhandled vis column %s', col)
                 else:
                     # Continuing an existing record
                     for col in colnames:
                         if col in _vis_ident_cols or col == 'DATA_DESC_ID' or col == 'WEIGHT' \
                                or col == 'SIGMA':
                             pass
                         elif col in _vis_smatch_cols:
                             if vdata[col][i] != curout[col]:
-                                die ('changing value for column %s within a glued record', col)
+                                die('changing value for column %s within a glued record', col)
                         elif col in _vis_sapprox_cols:
-                            if abs ((vdata[col][i] - curout[col]) / curout[col]) > 1e-5:
-                                die ('excessively changing value for column %s within a glued record', col)
+                            if abs((vdata[col][i] - curout[col]) / curout[col]) > 1e-5:
+                                die('excessively changing value for column %s within a glued record', col)
                         elif col in _vis_vmatch_cols:
-                            if not np.all (vdata[col][...,i] == curout[col]):
-                                die ('changing value for column %s within a glued record: %r , %r', col,
-                                     vdata[col][...,i], curout[col])
+                            if not np.all(vdata[col][...,i] == curout[col]):
+                                die('changing value for column %s within a glued record: %r , %r', col,
+                                    vdata[col][...,i], curout[col])
                         elif col in _vis_or_cols:
                             curout[col] |= vdata[col][i]
                         elif col in _vis_pconcat_cols:
                             d = vdata[col][...,i]
                             curout[col][:,outofs:outofs+d.shape[1]] = d
                         else:
-                            die ('unhandled vis column %s', col)
+                            die('unhandled vis column %s', col)
 
             inrow += nread
 
         if curout['TIME'] is not None:
-            dump () # finish this last record.
+            dump() # finish this last record.
             outrow += 1
 
-        prog.finish ()
+        prog.finish()
 
-    dt.close ()
-    tb.close ()
+    dt.close()
+    tb.close()
 
 
-def spwglue_cli (argv):
-    check_usage (spwglue_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    util.logger (cfg.loglevel)
-    spwglue (cfg)
+def spwglue_cli(argv):
+    check_usage(spwglue_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    util.logger(cfg.loglevel)
+    spwglue(cfg)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_plotants.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_plotants.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/closures.py` & `pwkit-1.0.0/pwkit/environments/casa/closures.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 __all__ = str ('Config ClosureCalculator closures_cli').split ()
 
 import collections
 import six, numpy as np
-from six.moves import range
+from six.moves import range, zip
 
 from ...cli import check_usage, die
 from ...kwargv import ParseKeywords, Custom
 from ...environments.casa import util
 from ...environments.casa.util import sanitize_unicode as b
 
 closures_doc = \
@@ -594,15 +594,15 @@
         tb.open (b(cfg.vis + '/DATA_DESCRIPTION'), nomodify=True)
         ddid_to_polid = tb.getcol (b'POLARIZATION_ID')
         ddid_to_spwid = tb.getcol (b'SPECTRAL_WINDOW_ID')
         tb.close ()
 
         tb.open (b(cfg.vis + '/POLARIZATION'), nomodify=True)
         polid_to_polns = {}
-        for i in xrange (tb.nrows ()):
+        for i in range (tb.nrows ()):
             polid_to_polns[i] = tb.getcell (b'CORR_TYPE', i)
         tb.close ()
 
         tb.open (b(cfg.vis + '/ANTENNA'), nomodify=True)
         self.ant_names = tb.getcol (b'NAME')
         self.ant_stations = tb.getcol (b'STATION')
         tb.close ()
@@ -699,15 +699,15 @@
     def _finish_timeslot (self):
         """We have loaded in all of the visibilities in one timeslot. We can now
         compute the phase closure triples.
 
         XXX: we should only process independent triples. Are we???
 
         """
-        for fpol, aps in self.ap_by_fpol.iteritems ():
+        for fpol, aps in self.ap_by_fpol.items ():
             aps = sorted (aps)
             nap = len (aps)
 
             for i1, ap1 in enumerate (aps):
                 for i2 in range (i1, nap):
                     ap2 = aps[i2]
                     bp1 = (ap1, ap2)
@@ -789,38 +789,38 @@
         self.all_bps = sorted (self.all_bps)
         self.all_times = np.sort (list (self.all_times))
 
         # Antpols by DDID, time:
         data = []
         descs = []
 
-        for ddid, stats in self.ap_time_stats_by_ddid.iteritems ():
+        for ddid, stats in self.ap_time_stats_by_ddid.items ():
             mean, scat = postproc (stats.finish (self.all_times, self.all_aps))
             data.append (mean / scat)
             descs.append ('DDID %d' % ddid)
 
         print ('Viewing X axis: antpol; Y axis: time; iteration: DDID (~= spwid) ...')
         ndshow_gtk3.cycle (data, descs, run_main=True)
 
         # Antpols by DDID, freq:
         data = []
         descs = []
 
-        for ddid, stats in self.ap_spec_stats_by_ddid.iteritems ():
+        for ddid, stats in self.ap_spec_stats_by_ddid.items ():
             mean, scat = postproc (stats.finish (self.all_aps))
             data.append (mean / scat)
             descs.append ('DDID %d' % ddid)
 
         print ('Viewing X axis: frequency; Y axis: antpol; iteration: DDID ...')
         ndshow_gtk3.cycle (data, descs, run_main=True)
 
         # Antpols by DDID
         p = om.RectPlot ()
 
-        for ddid, stats in self.ap_stats_by_ddid.iteritems ():
+        for ddid, stats in self.ap_stats_by_ddid.items ():
             ok, mean, scat = postproc_mask (stats.finish (self.all_aps))
             p.addXYErr (np.arange (len (self.all_aps))[ok], mean, scat, 'DDID %d' % ddid)
 
         p.setBounds (-0.5, len (self.all_aps) - 0.5)
         p.setLabels ('Antpol number', 'Mean closure phase (rad)')
         p.addHLine (0, keyText=None, zheight=-1)
         print ('Viewing everything grouped by antpol ...')
@@ -839,20 +839,19 @@
             ni = self._getname (ants[i])
             nj = self._getname (ants[j])
 
             if i <= j:
                 return '%s-%s %s' % (ni, nj, util.pol_names[pol1])
             return '%s-%s %s' % (nj, ni, util.pol_names[pol2])
 
-        for ddid, stats in self.bp_stats_by_ddid.iteritems ():
+        for ddid, stats in self.bp_stats_by_ddid.items ():
             mean, scat = postproc (stats.finish (self.all_bps))
             nmean = mean / scat
-            from itertools import izip
             pol1, pol2, ants, grid = grid_bp_data (self.all_bps,
-                                                   izip (self.all_bps, nmean))
+                                                   zip(self.all_bps, nmean))
             data.append (grid)
             descs.append ('DDID %d' % ddid)
             tostatuses.append (lambda yx: bpgrid_status (pol1, pol2, ants, yx))
 
         print ('Viewing X axis: antpol1; Y axis: antpol2; iteration: DDID ...')
         ndshow_gtk3.cycle (data, descs, tostatuses=tostatuses, run_main=True)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/dftphotom.py` & `pwkit-1.0.0/pwkit/environments/casa/dftphotom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- mode: python; coding: utf-8 -*-
 # Copyright 2012-2015 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
-"""pwkit.environments.casa.dftphotom - point-source photometry from visibilities
+"""This module implements an algorithm to compute light curves for point
+sources in interferometric visibility data. CASA doesn’t have a task to do this.
 
-CASA doesn't yet have a task to do this.
+The algorithm is accessible from the command line as ``casatask dftphotom``,
+but it can also be invoked from within Python. For help on usage from the
+command line, run ``casatask dftphotom --help``. The command’s help text will
+also describe some of the parameters below in more detail than is currently
+found here.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('Config dftphotom dftphotom_cli').split ()
+__all__ = 'Config dftphotom dftphotom_cli'.split()
 
 import six, sys, os.path, numpy as np
 from six.moves import range
 
 from ... import binary_type, text_type
 # Note: zany spacing so that Sphinx can parse the file correctly.
 from . ..astutil import *
@@ -71,15 +76,15 @@
   uncertainties are assessed from the scatter of all the visibilities
   in each timeslot. If true, we trust that variance=1/weight and
   propagate this in the standard way.
 
 format=[humane(default)|pandas]
   The format of the output. The default is "humane" which is described
   below. The "pandas" format is slightly less human-friendly but can
-  be read directly into a Pandas DataFrame with pandas.read_table ().
+  be read directly into a Pandas DataFrame with pandas.read_table().
 
 IMPORTANT: the fundamental assumption of this task is that the only
 signal in the visibilities is from a point source at the phasing
 center. We also assume that all sampled polarizations get equal
 contributions from the source (though you can resample the Stokes
 parameters on the fly, so this is not quite the same thing as
 requiring the source be unpolarized).
@@ -91,69 +96,83 @@
 with sorted MJDs, one record for each timestamp present in the dataset,
 with all fluxes in ujy. dt is simply (MJD - MJD[0]) * 1440. The units
 of re, im, mag, and their uncertainties are microjansky by default,
 but see the datascale keyword, and there's no way to know if the
 data have actually been flux-calibrated or not.
 """
 
-class HumaneOutputFormat (object):
-    def header (self, cfg):
+class HumaneOutputFormat(object):
+    def header(self, cfg):
         pass
 
-    def row (self, cfg, mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n):
-        print ('%12.5f %6.2f %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d' %
-               (mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
-               file=cfg.outstream)
+    def row(self, cfg, mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n):
+        print('%12.5f %6.2f %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d' %
+              (mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
+              file=cfg.outstream)
 
 
-class PandasOutputFormat (object):
-    def header (self, cfg):
-        print ('mjd dtmin re ure im uim abs uabs nsamp'.replace (' ', '\t'),
-               file=cfg.outstream)
+class PandasOutputFormat(object):
+    def header(self, cfg):
+        print('mjd dtmin re ure im uim abs uabs nsamp'.replace(' ', '\t'),
+              file=cfg.outstream)
 
-    def row (self, cfg, *args):
-        print ('\t'.join (str (x) for x in args), file=cfg.outstream)
+    def row(self, cfg, *args):
+        print('\t'.join(str(x) for x in args), file=cfg.outstream)
 
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
+    """The path to the visibility MeasurementSet to process. No default; you
+    must specify a value before calling :func:`dftphotom`."""
+
     datacol = 'data'
+    """A string specifying which visibility data column to process: ``data``,
+    ``corrected_data``, or ``model_data``. Default ``'data'``.
+
+    """
     believeweights = False
+    """Whether to trust that the data-weight information in the MS accurately
+    describe the noise in their corresponding visibilities. Default False.
 
-    @Custom (str, uiname='out')
-    def outstream (val):
+    """
+    @Custom(str, uiname='out')
+    def outstream(val):
         if val is None:
             return sys.stdout
         try:
-            return open (val, 'w')
+            return open(val, 'w')
         except Exception as e:
-            die ('cannot open path "%s" for writing', val)
+            die('cannot open path "%s" for writing', val)
 
     datascale = 1e6
-
-    @Custom (str, default='humane')
-    def format (val):
+    """The amount by which to scale the computed values before emitting them as
+    text. The default is 1e6, which means that the output will be in
+    microJanskys if the underlying data are calibrated to Jansky units.
+
+    """
+    @Custom(str, default='humane')
+    def format(val):
         if val is None or val == 'humane':
-            return HumaneOutputFormat ()
+            return HumaneOutputFormat()
 
         if val == 'pandas':
-            return PandasOutputFormat ()
+            return PandasOutputFormat()
 
-        die ('unrecognized output format %r', val)
+        die('unrecognized output format %r', val)
 
-    @Custom ([str, str], default=None)
-    def rephase (val):
+    @Custom([str, str], default=None)
+    def rephase(val):
         if val is None:
             return None
 
         try:
-            ra = parsehours (val[0])
-            dec = parsedeglat (val[1])
+            ra = parsehours(val[0])
+            dec = parsedeglat(val[1])
         except Exception as e:
-            die ('cannot parse "rephase" values as RA/dec: %s', e)
+            die('cannot parse "rephase" values as RA/dec: %s', e)
         return ra, dec
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
@@ -164,18 +183,25 @@
     taql = str
     time = str
     uvdist = str
 
     loglevel = 'warn'
 
 
-def dftphotom (cfg):
-    tb = util.tools.table ()
-    ms = util.tools.ms ()
-    me = util.tools.measures ()
+def dftphotom(cfg):
+    """Run the discrete-Fourier-transform photometry algorithm.
+
+    See the module-level documentation and the output of ``casatask dftphotom
+    --help`` for help. All of the algorithm configuration is specified in the
+    *cfg* argument, which is an instance of :class:`Config`.
+
+    """
+    tb = util.tools.table()
+    ms = util.tools.ms()
+    me = util.tools.measures()
 
     # Read stuff in. Even if the weight values don't have their
     # absolute scale set correctly, we can still use them to set the
     # relative weighting of the data points.
     #
     # datacol is (ncorr, nchan, nchunk)
     # flag is (ncorr, nchan, nchunk)
@@ -189,174 +215,182 @@
     # selectinit() is broken, but the invocation here is good because it
     # affects the results from ms.range() and friends.
 
     if ':' in (cfg.spw or ''):
         warn('it looks like you are attempting to select channels within one or more spws')
         warn('this is NOT IMPLEMENTED; I will average over the whole spw instead')
 
-    ms.open (b(cfg.vis))
-    totrows = ms.nrow ()
-    ms_sels = dict ((n, cfg.get (n)) for n in util.msselect_keys
-                    if cfg.get (n) is not None)
-    ms.msselect (b(ms_sels))
+    ms.open(b(cfg.vis))
+    totrows = ms.nrow()
+    ms_sels = dict((n, cfg.get(n)) for n in util.msselect_keys
+                   if cfg.get(n) is not None)
+    ms.msselect(b(ms_sels))
 
-    rangeinfo = ms.range (b'data_desc_id field_id'.split ())
+    rangeinfo = ms.range(b'data_desc_id field_id'.split())
     ddids = rangeinfo['data_desc_id']
     fields = rangeinfo['field_id']
-    colnames = [cfg.datacol] + 'flag weight time axis_info'.split ()
+    colnames = [cfg.datacol] + 'flag weight time axis_info'.split()
     rephase = (cfg.rephase is not None)
 
     if fields.size != 1:
         # I feel comfortable making this a fatal error, even if we're
         # not rephasing.
-        die ('selected data should contain precisely one field; got %d', fields.size)
+        die('selected data should contain precisely one field; got %d', fields.size)
 
     if rephase:
         fieldid = fields[0]
-        tb.open (b(os.path.join (cfg.vis, 'FIELD')))
-        phdirinfo = tb.getcell (b'PHASE_DIR', fieldid)
-        tb.close ()
+        tb.open(b(os.path.join(cfg.vis, 'FIELD')))
+        phdirinfo = tb.getcell(b'PHASE_DIR', fieldid)
+        tb.close()
 
         if phdirinfo.shape[1] != 1:
-            die ('trying to rephase but target field (#%d) has a '
-                 'time-variable phase center, which I can\'t handle', fieldid)
+            die('trying to rephase but target field (#%d) has a '
+                'time-variable phase center, which I can\'t handle', fieldid)
         ra0, dec0 = phdirinfo[:,0] # in radians.
 
         # based on intflib/pwflux.py, which was copied from
         # hex/hex-lib-calcgainerr:
 
         dra = cfg.rephase[0] - ra0
         dec = cfg.rephase[1]
-        l = np.sin (dra) * np.cos (dec)
-        m = np.sin (dec) * np.cos (dec0) - np.cos (dra) * np.cos (dec) * np.sin (dec0)
-        n = np.sin (dec) * np.sin (dec0) + np.cos (dra) * np.cos (dec) * np.cos (dec0)
+        l = np.sin(dra) * np.cos(dec)
+        m = np.sin(dec) * np.cos(dec0) - np.cos(dra) * np.cos(dec) * np.sin(dec0)
+        n = np.sin(dec) * np.sin(dec0) + np.cos(dra) * np.cos(dec) * np.cos(dec0)
         n -= 1 # makes the work below easier
-        lmn = np.asarray ([l, m, n])
-        colnames.append ('uvw')
+        lmn = np.asarray([l, m, n])
+        colnames.append('uvw')
 
         # Also need this although 99% of the time `ddid` and `spwid` are the same
-        tb.open (b(os.path.join (cfg.vis, 'DATA_DESCRIPTION')))
-        ddspws = np.asarray (tb.getcol (b'SPECTRAL_WINDOW_ID'))
-        tb.close ()
+        tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
+        ddspws = np.asarray(tb.getcol(b'SPECTRAL_WINDOW_ID'))
+        tb.close()
 
     tbins = {}
     colnames = b(colnames)
 
-    for ddindex, ddid in enumerate (ddids):
+    for ddindex, ddid in enumerate(ddids):
         # Starting in CASA 4.6, selectinit(ddid) stopped actually filtering
         # your data to match the specified DDID! What garbage. Work around
         # with our own filtering.
         ms_sels['taql'] = 'DATA_DESC_ID == %d' % ddid
         ms.msselect(b(ms_sels))
 
-        ms.selectinit (ddid)
+        ms.selectinit(ddid)
         if cfg.polarization is not None:
-            ms.selectpolarization (b(cfg.polarization.split (',')))
-        ms.iterinit (maxrows=4096)
-        ms.iterorigin ()
+            ms.selectpolarization(b(cfg.polarization.split(',')))
+        ms.iterinit(maxrows=4096)
+        ms.iterorigin()
 
         while True:
-            cols = ms.getdata (items=colnames)
+            cols = ms.getdata(items=colnames)
 
             if rephase:
                 # With appropriate spw/DDID selection, `freqs` has shape
                 # (nchan, 1). Convert to m^-1 so we can multiply against UVW
                 # directly.
                 freqs = cols['axis_info']['freq_axis']['chan_freq']
                 assert freqs.shape[1] == 1, 'internal inconsistency, chan_freq??'
                 freqs = freqs[:,0] * util.INVERSE_C_MS
 
-            for i in range (cols['time'].size): # all records
+            for i in range(cols['time'].size): # all records
                 time = cols['time'][i]
                 # get out of UTC as fast as we can! For some reason
                 # giving 'unit=s' below doesn't do what one might hope it would.
                 # CASA can convert to a variety of timescales; TAI is probably
                 # the safest conversion in terms of being helpful while remaining
                 # close to the fundamental data, but TT is possible and should
                 # be perfectly precise for standard applications.
-                mq = me.epoch (b'utc', b({'value': time / 86400., 'unit': 'd'}))
-                mjdtt = me.measure (b(mq), b'tt')['m0']['value']
+                mq = me.epoch(b'utc', b({'value': time / 86400., 'unit': 'd'}))
+                mjdtt = me.measure(b(mq), b'tt')['m0']['value']
 
-                tdata = tbins.get (mjdtt, None)
+                tdata = tbins.get(mjdtt, None)
                 if tdata is None:
                     tdata = tbins[mjdtt] = [0., 0., 0., 0., 0]
 
                 if rephase:
                     uvw = cols['uvw'][:,i]
-                    ph = np.exp ((0-2j) * np.pi * np.dot (lmn, uvw) * freqs)
+                    ph = np.exp((0-2j) * np.pi * np.dot(lmn, uvw) * freqs)
 
-                for j in range (cols['flag'].shape[0]): # all polns
+                for j in range(cols['flag'].shape[0]): # all polns
                     # We just average together all polarizations right now!
                     # (Not actively, but passively by just iterating over them.)
                     data = cols[cfg.datacol][j,:,i]
                     flags = cols['flag'][j,:,i]
 
                     # XXXXX casacore is currently (ca. 2012) broken and
                     # returns the raw weights from the dataset rather than
                     # applying the polarization selection. Fortunately all of
                     # our weights are the same, and you can never fetch more
                     # pol types than the dataset has, so this bit works
                     # despite the bug.
 
-                    w = np.where (~flags)[0]
+                    w = np.where(~flags)[0]
                     if not w.size:
                         continue # all flagged
 
                     if rephase:
                         data *= ph
 
-                    d = data[w].mean ()
+                    d = data[w].mean()
                     # account for flagged parts. 90% sure this is the
                     # right thing to do:
                     wt = cols['weight'][j,i] * w.size / data.size
                     wd = wt * d
                     # note a little bit of a hack here to encode real^2 and
                     # imag^2 separately:
                     wd2 = wt * (d.real**2 + (1j) * d.imag**2)
 
                     tdata[0] += wd
                     tdata[1] += wd2
                     tdata[2] += wt
                     tdata[3] += wt**2
                     tdata[4] += 1
 
-            if not ms.iternext ():
+            if not ms.iternext():
                 break
 
         ms.reset() # reset selection filter so we can get next DDID
 
-    ms.close ()
+    ms.close()
 
     # Could gain some efficiency by using a better data structure than a dict().
-    smjd = sorted (six.iterkeys (tbins))
-    cfg.format.header (cfg)
+    smjd = sorted(six.iterkeys(tbins))
+    cfg.format.header(cfg)
 
     for mjd in smjd:
         wd, wd2, wt, wt2, n = tbins[mjd]
-        if n == 0:
-            continue # could be all flagged
+        if n < 3: # not enough data for meaningful statistics
+            continue
 
         dtmin = 1440 * (mjd - smjd[0])
         r_sc = wd.real / wt * cfg.datascale
         i_sc = wd.imag / wt * cfg.datascale
         r2_sc = wd2.real / wt * cfg.datascale**2
         i2_sc = wd2.imag / wt * cfg.datascale**2
 
         if cfg.believeweights:
             ru_sc = wt**-0.5 * cfg.datascale
             iu_sc = wt**-0.5 * cfg.datascale
         else:
             rv_sc = r2_sc - r_sc**2 # variance among real/imag msmts
             iv_sc = i2_sc - i_sc**2
-            ru_sc = np.sqrt (rv_sc * wt2) / wt # uncert in mean real/img values
-            iu_sc = np.sqrt (iv_sc * wt2) / wt
-
-        mag = np.sqrt (r_sc**2 + i_sc**2)
-        umag = np.sqrt (r_sc**2 * ru_sc**2 + i_sc**2 * iu_sc**2) / mag
-        cfg.format.row (cfg, mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n)
-
+            ru_sc = np.sqrt(rv_sc * wt2) / wt # uncert in mean real/img values
+            iu_sc = np.sqrt(iv_sc * wt2) / wt
 
-def dftphotom_cli (argv):
-    check_usage (dftphotom_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    util.logger (cfg.loglevel)
-    dftphotom (cfg)
+        mag = np.sqrt(r_sc**2 + i_sc**2)
+        umag = np.sqrt(r_sc**2 * ru_sc**2 + i_sc**2 * iu_sc**2) / mag
+        cfg.format.row(cfg, mjd, dtmin, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n)
+
+
+def dftphotom_cli(argv):
+    """Command-line access to the :func:`dftphotom` algorithm.
+
+    This function implements the behavior of the command-line ``casatask
+    dftphotom`` tool, wrapped up into a single callable function. The argument
+    *argv* is a list of command-line arguments, in Unix style where the zeroth
+    item is the name of the command.
+
+    """
+    check_usage(dftphotom_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    util.logger(cfg.loglevel)
+    dftphotom(cfg)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_importalma.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_importalma.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_setjy.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_setjy.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/polmodel.py` & `pwkit-1.0.0/pwkit/environments/casa/polmodel.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/gpdiagnostics.py` & `pwkit-1.0.0/pwkit/environments/casa/gpdiagnostics.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_importevla.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_importevla.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/dftspect.py` & `pwkit-1.0.0/pwkit/environments/casa/dftspect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2012, 2016 Peter Williams <peter@newton.cx> and collaborators.
+# Copyright 2012, 2016, 2018 Peter Williams <peter@newton.cx> and collaborators.
 # Licensed under the MIT License.
 
 # NB. This is super-redundant with msphotom but it seems impractical
 # to combine them.
 
 """High-resolution point-source spectra from visibilities
 
 CASA doesn't yet have a task to do this.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('Config dftspect dftspect_cli').split ()
+__all__ = str('Config dftspect dftspect_cli').split()
 
 import six, sys, os.path, numpy as np
 from six.moves import range
 
 from ... import binary_type, text_type
 from ...astutil import *
 from ...cli import check_usage, die
@@ -67,15 +67,15 @@
   is equal to 1/weight. In this case uncertainties are assessed from the
   scatter of all the visibilities in each timeslot. If true, we trust that
   variance=1/weight and propagate this in the standard way.
 
 format=[humane(default)|pandas]
   The format of the output. The default is "humane" which is described below.
   The "pandas" format is slightly less human-friendly but can be read directly
-  into a Pandas DataFrame with pandas.read_table ().
+  into a Pandas DataFrame with pandas.read_table().
 
 IMPORTANT: the fundamental assumption of this task is that the only signal in
 the visibilities is from a point source at the phasing center. We also assume
 that all sampled polarizations get equal contributions from the source (though
 you can resample the Stokes parameters on the fly, so this is not quite the
 same thing as requiring the source be unpolarized).
 
@@ -85,69 +85,69 @@
 
 sorted by frequency, where the frequency is the mean frequency of its
 associated spectral window. The units of re, im, mag, and their uncertainties
 are microjansky by default, but see the datascale keyword, and there's no way
 to know if the data have actually been flux-calibrated or not.
 """
 
-class HumaneOutputFormat (object):
-    def header (self, cfg):
+class HumaneOutputFormat(object):
+    def header(self, cfg):
         pass
 
-    def row (self, cfg, freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n):
-        print ('%10.2f %2d %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d' %
-               (freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
-               file=cfg.outstream)
+    def row(self, cfg, freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n):
+        print('%10.2f %2d %10.2f %10.2f %10.2f %10.2f %10.2f %10.2f %d' %
+              (freq, spwnum, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n),
+              file=cfg.outstream)
 
 
-class PandasOutputFormat (object):
-    def header (self, cfg):
-        print ('freq spwnum re ure im uim abs uabs nsamp'.replace (' ', '\t'),
-               file=cfg.outstream)
+class PandasOutputFormat(object):
+    def header(self, cfg):
+        print('freq spwnum re ure im uim abs uabs nsamp'.replace(' ', '\t'),
+              file=cfg.outstream)
 
-    def row (self, cfg, *args):
-        print ('\t'.join (str (x) for x in args), file=cfg.outstream)
+    def row(self, cfg, *args):
+        print('\t'.join(str(x) for x in args), file=cfg.outstream)
 
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
     datacol = 'data'
     believeweights = False
 
-    @Custom (str, uiname='out')
-    def outstream (val):
+    @Custom(str, uiname='out')
+    def outstream(val):
         if val is None:
             return sys.stdout
         try:
-            return open (val, 'w')
+            return open(val, 'w')
         except Exception as e:
-            die ('cannot open path "%s" for writing', val)
+            die('cannot open path "%s" for writing', val)
 
     datascale = 1e6
 
-    @Custom (str, default='humane')
-    def format (val):
+    @Custom(str, default='humane')
+    def format(val):
         if val is None or val == 'humane':
-            return HumaneOutputFormat ()
+            return HumaneOutputFormat()
 
         if val == 'pandas':
-            return PandasOutputFormat ()
+            return PandasOutputFormat()
 
-        die ('unrecognized output format %r', val)
+        die('unrecognized output format %r', val)
 
-    @Custom ([str, str], default=None)
-    def rephase (val):
+    @Custom([str, str], default=None)
+    def rephase(val):
         if val is None:
             return None
 
         try:
-            ra = parsehours (val[0])
-            dec = parsedeglat (val[1])
+            ra = parsehours(val[0])
+            dec = parsedeglat(val[1])
         except Exception as e:
-            die ('cannot parse "rephase" values as RA/dec: %s', e)
+            die('cannot parse "rephase" values as RA/dec: %s', e)
         return ra, dec
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
@@ -158,17 +158,17 @@
     taql = str
     time = str
     uvdist = str
 
     loglevel = 'warn'
 
 
-def dftspect (cfg):
-    tb = util.tools.table ()
-    ms = util.tools.ms ()
+def dftspect(cfg):
+    tb = util.tools.table()
+    ms = util.tools.ms()
 
     # Read stuff in. Even if the weight values don't have their
     # absolute scale set correctly, we can still use them to set the
     # relative weighting of the data points.
     #
     # datacol is (ncorr, nchan, nchunk)
     # flag is (ncorr, nchan, nchunk)
@@ -178,164 +178,164 @@
     # axis_info.corr_axis is (ncorr)
     # axis_info.freq_axis.chan_freq is (nchan, 1) [for now?]
     #
     # Note that we apply msselect() again when reading the data because
     # selectinit() is broken, but the invocation here is good because it
     # affects the results from ms.range() and friends.
 
-    ms.open (b(cfg.vis))
-    ms_sels = dict ((n, cfg.get (n)) for n in util.msselect_keys
-                    if cfg.get (n) is not None)
-    ms.msselect (b(ms_sels))
+    ms.open(b(cfg.vis))
+    ms_sels = dict((n, cfg.get(n)) for n in util.msselect_keys
+                   if cfg.get(n) is not None)
+    ms.msselect(b(ms_sels))
 
-    rangeinfo = ms.range (b'data_desc_id field_id'.split ())
+    rangeinfo = ms.range(b'data_desc_id field_id'.split())
     ddids = rangeinfo['data_desc_id']
     fields = rangeinfo['field_id']
-    colnames = [cfg.datacol] + 'flag weight axis_info'.split ()
+    colnames = [cfg.datacol] + 'flag weight axis_info'.split()
     rephase = (cfg.rephase is not None)
 
     if fields.size != 1:
         # I feel comfortable making this a fatal error, even if we're
         # not rephasing.
-        die ('selected data should contain precisely one field; got %d', fields.size)
+        die('selected data should contain precisely one field; got %d', fields.size)
 
-    tb.open (b(os.path.join (cfg.vis, 'DATA_DESCRIPTION')))
-    ddspws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    tb.close ()
-
-    tb.open (b(os.path.join (cfg.vis, 'SPECTRAL_WINDOW')))
-    spwmfreqs = np.zeros (tb.nrows ())
-    for i in xrange (spwmfreqs.size):
-        spwmfreqs[i] = tb.getcell (b'CHAN_FREQ', i).mean () * 1e-9 # -> GHz
-    tb.close ()
+    tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
+    ddspws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    tb.close()
+
+    tb.open(b(os.path.join(cfg.vis, 'SPECTRAL_WINDOW')))
+    spwmfreqs = np.zeros(tb.nrows())
+    for i in range(spwmfreqs.size):
+        spwmfreqs[i] = tb.getcell(b'CHAN_FREQ', i).mean() * 1e-9 # -> GHz
+    tb.close()
 
     if rephase:
         fieldid = fields[0]
-        tb.open (b(os.path.join (cfg.vis, 'FIELD')))
-        phdirinfo = tb.getcell (b'PHASE_DIR', fieldid)
-        tb.close ()
+        tb.open(b(os.path.join(cfg.vis, 'FIELD')))
+        phdirinfo = tb.getcell(b'PHASE_DIR', fieldid)
+        tb.close()
 
         if phdirinfo.shape[1] != 1:
-            die ('trying to rephase but target field (#%d) has a '
-                 'time-variable phase center, which I can\'t handle', fieldid)
+            die('trying to rephase but target field (#%d) has a '
+                'time-variable phase center, which I can\'t handle', fieldid)
         ra0, dec0 = phdirinfo[:,0] # in radians.
 
         # based on intflib/pwflux.py, which was copied from
         # hex/hex-lib-calcgainerr:
 
         dra = cfg.rephase[0] - ra0
         dec = cfg.rephase[1]
-        l = np.sin (dra) * np.cos (dec)
-        m = np.sin (dec) * np.cos (dec0) - np.cos (dra) * np.cos (dec) * np.sin (dec0)
-        n = np.sin (dec) * np.sin (dec0) + np.cos (dra) * np.cos (dec) * np.cos (dec0)
+        l = np.sin(dra) * np.cos(dec)
+        m = np.sin(dec) * np.cos(dec0) - np.cos(dra) * np.cos(dec) * np.sin(dec0)
+        n = np.sin(dec) * np.sin(dec0) + np.cos(dra) * np.cos(dec) * np.cos(dec0)
         n -= 1 # makes the work below easier
-        lmn = np.asarray ([l, m, n])
-        colnames.append ('uvw')
+        lmn = np.asarray([l, m, n])
+        colnames.append('uvw')
 
     spwbins = {}
     colnames = b(colnames)
 
     for ddid in ddids:
         # Starting in CASA 4.6, selectinit(ddid) stopped actually filtering
         # your data to match the specified DDID! What garbage. Work around
         # with our own filtering.
         ms_sels['taql'] = 'DATA_DESC_ID == %d' % ddid
         ms.msselect(b(ms_sels))
 
-        ms.selectinit (ddid)
+        ms.selectinit(ddid)
         if cfg.polarization is not None:
-            ms.selectpolarization (b(cfg.polarization.split (',')))
-        ms.iterinit ()
-        ms.iterorigin ()
+            ms.selectpolarization(b(cfg.polarization.split(',')))
+        ms.iterinit()
+        ms.iterorigin()
 
         spw = ddspws[ddid]
-        sdata = spwbins.get (spw)
+        sdata = spwbins.get(spw)
         if sdata is None: # might have multiple ddids going to one spw
             sdata = spwbins[spw] = [0., 0., 0., 0., 0]
 
         while True:
-            cols = ms.getdata (items=colnames)
+            cols = ms.getdata(items=colnames)
 
             if rephase:
                 # With appropriate spw/DDID selection, `freqs` has shape
                 # (nchan, 1). Convert to m^-1 so we can multiply against UVW
                 # directly.
                 freqs = cols['axis_info']['freq_axis']['chan_freq']
                 assert freqs.shape[1] == 1, 'internal inconsistency, chan_freq??'
                 freqs = freqs[:,0] * util.INVERSE_C_MS
 
-            for i in xrange (cols['flag'].shape[-1]): # all records
+            for i in range(cols['flag'].shape[-1]): # all records
                 if rephase:
                     uvw = cols['uvw'][:,i]
-                    ph = np.exp ((0-2j) * np.pi * np.dot (lmn, uvw) * freqs)
+                    ph = np.exp((0-2j) * np.pi * np.dot(lmn, uvw) * freqs)
 
-                for j in xrange (cols['flag'].shape[0]): # all polns
+                for j in range(cols['flag'].shape[0]): # all polns
                     data = cols[cfg.datacol][j,:,i]
                     flags = cols['flag'][j,:,i]
 
                     # XXXXX casacore is currently broken and returns the raw
                     # weights from the dataset rather than applying the
                     # polarization selection. Fortunately all of our weights
                     # are the same, and you can never fetch more pol types
                     # than the dataset has, so this bit works despite the bug.
 
-                    w = np.where (~flags)[0]
+                    w = np.where(~flags)[0]
                     if not w.size:
                         continue # all flagged
 
                     if rephase:
                         data *= ph
 
-                    d = data[w].mean ()
+                    d = data[w].mean()
                     # account for flagged parts. 90% sure this is the
                     # right thing to do:
                     wt = cols['weight'][j,i] * w.size / data.size
                     wd = wt * d
                     # note a little bit of a hack here to encode real^2 and
                     # imag^2 separately:
                     wd2 = wt * (d.real**2 + (1j) * d.imag**2)
 
                     sdata[0] += wd
                     sdata[1] += wd2
                     sdata[2] += wt
                     sdata[3] += wt**2
                     sdata[4] += 1
 
-            if not ms.iternext ():
+            if not ms.iternext():
                 break
 
         ms.reset() # reset selection filter so we can get next DDID
 
-    ms.close ()
+    ms.close()
 
-    spws = sorted (six.iterkeys (spwbins), key=lambda s: spwmfreqs[s])
-    cfg.format.header (cfg)
+    spws = sorted(six.iterkeys(spwbins), key=lambda s: spwmfreqs[s])
+    cfg.format.header(cfg)
 
     for spw in spws:
         wd, wd2, wt, wt2, n = spwbins[spw]
-        if n == 0:
-            continue # could be all flagged
+        if n < 3: # not enough data for meaningful statistics
+            continue
 
         r_sc = wd.real / wt * cfg.datascale
         i_sc = wd.imag / wt * cfg.datascale
         r2_sc = wd2.real / wt * cfg.datascale**2
         i2_sc = wd2.imag / wt * cfg.datascale**2
 
         if cfg.believeweights:
             ru_sc = wt**-0.5 * cfg.datascale
             iu_sc = wt**-0.5 * cfg.datascale
         else:
             rv_sc = r2_sc - r_sc**2 # variance among real/imag msmts
             iv_sc = i2_sc - i_sc**2
-            ru_sc = np.sqrt (rv_sc * wt2) / wt # uncert in mean real/img values
-            iu_sc = np.sqrt (iv_sc * wt2) / wt
+            ru_sc = np.sqrt(rv_sc * wt2) / wt # uncert in mean real/img values
+            iu_sc = np.sqrt(iv_sc * wt2) / wt
 
-        mag = np.sqrt (r_sc**2 + i_sc**2)
-        umag = np.sqrt (r_sc**2 * ru_sc**2 + i_sc**2 * iu_sc**2) / mag
-        cfg.format.row (cfg, spwmfreqs[spw], spw, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n)
+        mag = np.sqrt(r_sc**2 + i_sc**2)
+        umag = np.sqrt(r_sc**2 * ru_sc**2 + i_sc**2 * iu_sc**2) / mag
+        cfg.format.row(cfg, spwmfreqs[spw], spw, r_sc, ru_sc, i_sc, iu_sc, mag, umag, n)
 
 
-def dftspect_cli (argv):
-    checkusage (dftspect_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    util.logger (cfg.loglevel)
-    dftspect (cfg)
+def dftspect_cli(argv):
+    checkusage(dftspect_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    util.logger(cfg.loglevel)
+    dftspect(cfg)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_genantpos.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_genantpos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2015 Peter Williams <peter@newton.cx> and collaborators
+# Copyright 2015, 2017 Peter Williams <peter@newton.cx> and collaborators
 # Licensed under the MIT License
 
 """This file is a casapy script. Do not use it as a module.
 
 It is also not intended to be invoked directly through pkcasascript. See
 `pwkit.environments.casa.tasks.gencal`.
 
 """
 
-def in_casapy (helper, vis=None):
+def in_casapy(helper, vis=None):
     """This function is run inside the weirdo casapy IPython environment! A
     strange set of modules is available, and the
     `pwkit.environments.casa.scripting` system sets up a very particular
     environment to allow encapsulated scripting.
 
     """
-    import sys, cPickle as pickle
+    import numpy as np, sys
     from correct_ant_posns import correct_ant_posns
 
-    info = correct_ant_posns (vis, False)
-    if len (info) != 3 or info[0] != 0 or not len (info[1]):
-        helper.die ('failed to fetch VLA antenna positions; got %r', info)
+    info = correct_ant_posns(vis, False)
+    if len(info) != 3 or info[0] != 0 or not len(info[1]):
+        helper.die('failed to fetch VLA antenna positions; got %r', info)
 
     antenna = info[1]
     parameter = info[2]
 
-    with open (helper.temppath ('info.pkl'), 'w') as f:
-        pickle.dump (antenna, f)
-        pickle.dump (parameter, f)
+    with open(helper.temppath('info.npy'), 'wb') as f:
+        np.save(f, antenna)
+        np.save(f, parameter)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/__init__.py` & `pwkit-1.0.0/pwkit/environments/casa/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,114 +50,114 @@
 - If you do have a full CASA installation available on your compuer, the
   :mod:`pwkit.environments.casa.scripting` module allows you to drive it from
   Python code in a way that allows you to analyze its output, check for
   error conditions, and so on. This is useful for certain features that are not
   currently available in the :mod:`~pwkit.environments.casa.tasks` module.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('CasaEnvironment CasaTool commandline').split ()
+__all__ = 'CasaEnvironment CasaTool commandline'.split()
 
 import glob, io, os.path
 
 from ... import PKError, cli
 from ...cli import multitool
 from .. import Environment, prepend_environ_path, user_data_path
 
 
-class CasaEnvironment (Environment):
+class CasaEnvironment(Environment):
     _rootdir = None
 
-    def __init__ (self, rootdir=None):
+    def __init__(self, rootdir=None):
         if rootdir is None:
-            rootdir = self._default_rootdir ()
+            rootdir = self._default_rootdir()
 
-        self._rootdir = os.path.abspath (rootdir)
+        self._rootdir = os.path.abspath(rootdir)
 
 
-    def _default_rootdir (self):
-        d = os.environ.get ('PWKIT_CASA')
+    def _default_rootdir(self):
+        d = os.environ.get('PWKIT_CASA')
         if d is None:
-            raise PKError ('CASA installation directory must be specified '
-                           'in the $PWKIT_CASA environment variable')
+            raise PKError('CASA installation directory must be specified '
+                          'in the $PWKIT_CASA environment variable')
         return d
 
 
-    def modify_environment (self, env):
+    def modify_environment(self, env):
         """Maintaining compatibility with different CASA versions is a pain."""
 
         # Ugh. I don't see any way out of special-casing the RPM-based
         # installations ... which only exist on NRAO computers, AFAICT.
         # Hardcoding 64-bitness, hopefully that won't come back to bite me.
-        is_rpm_install = self._rootdir.startswith ('/usr/lib64/casapy/release/')
+        is_rpm_install = self._rootdir.startswith('/usr/lib64/casapy/release/')
 
-        def path (*args):
-            return os.path.join (self._rootdir, *args)
+        def path(*args):
+            return os.path.join(self._rootdir, *args)
 
-        env['CASAROOT'] = path ()
-        env['CASAPATH'] = ' '.join ([path (),
-                                      os.uname ()[0].lower (),
-                                      'local',
-                                      os.uname ()[1]])
+        env['CASAROOT'] = path()
+        env['CASAPATH'] = ' '.join([path(),
+                                    os.uname()[0].lower(),
+                                    'local',
+                                    os.uname()[1]])
 
         if is_rpm_install:
-            env['CASA_INSTALLATION_TYPE'] = b'rpm-installation'
-            prepend_environ_path (env, 'PATH', b'/usr/lib64/casa/01/bin')
-            prepend_environ_path (env, 'PATH', path ('bin'))
+            env['CASA_INSTALLATION_TYPE'] = 'rpm-installation'
+            prepend_environ_path(env, 'PATH', '/usr/lib64/casa/01/bin')
+            prepend_environ_path(env, 'PATH', path('bin'))
         else:
-            env['CASA_INSTALLATION_TYPE'] = b'tar-installation'
+            env['CASA_INSTALLATION_TYPE'] = 'tar-installation'
 
-            lib = 'lib64' if os.path.isdir (path ('lib64')) else 'lib'
+            lib = 'lib64' if os.path.isdir(path('lib64')) else 'lib'
             # 4.3.1 comes with both python2.6 and python2.7???
-            pydir = sorted (glob.glob (path (lib, 'python2*')))[-1]
+            pydir = sorted(glob.glob(path(lib, 'python2*')))[-1]
 
-            tcldir = path ('share', 'tcl')
-            if os.path.isdir (tcldir):
+            tcldir = path('share', 'tcl')
+            if os.path.isdir(tcldir):
                 env['TCL_LIBRARY'] = tcldir
             else:
-                tcl_versioned_dirs = glob.glob (path ('share', 'tcl*'))
-                if len (tcl_versioned_dirs):
+                tcl_versioned_dirs = glob.glob(path('share', 'tcl*'))
+                if len(tcl_versioned_dirs):
                     env['TCL_LIBRARY'] = tcl_versioned_dirs[-1]
 
-            bindir = path (lib, 'casa', 'bin')
-            if not os.path.isdir (bindir):
-                bindir = path (lib, 'casapy', 'bin')
-            prepend_environ_path (env, 'PATH', bindir)
+            bindir = path(lib, 'casa', 'bin')
+            if not os.path.isdir(bindir):
+                bindir = path(lib, 'casapy', 'bin')
+            prepend_environ_path(env, 'PATH', bindir)
 
             env['CASA_INSTALLATION_DIRECTORY'] = env['CASAROOT']
             env['__CASAPY_PYTHONDIR'] = pydir
-            env['MATPLOTLIBRC'] = path ('share', 'matplotlib')
+            env['MATPLOTLIBRC'] = path('share', 'matplotlib')
             env['PYTHONHOME'] = env['CASAROOT']
-            env['TK_LIBRARY'] = path ('share', 'tk')
-            env['QT_PLUGIN_PATH'] = path (lib, 'qt4', 'plugins')
+            env['TK_LIBRARY'] = path('share', 'tk')
+            env['QT_PLUGIN_PATH'] = path(lib, 'qt4', 'plugins')
 
-            prepend_environ_path (env, 'LD_LIBRARY_PATH', path (lib))
+            prepend_environ_path(env, 'LD_LIBRARY_PATH', path(lib))
             # should we overwite PYTHONPATH instead?
-            prepend_environ_path (env, 'PYTHONPATH', os.path.join (pydir, 'site-packages'))
-            prepend_environ_path (env, 'PYTHONPATH', os.path.join (pydir, 'heuristics'))
-            prepend_environ_path (env, 'PYTHONPATH', pydir)
+            prepend_environ_path(env, 'PYTHONPATH', os.path.join(pydir, 'site-packages'))
+            prepend_environ_path(env, 'PYTHONPATH', os.path.join(pydir, 'heuristics'))
+            prepend_environ_path(env, 'PYTHONPATH', pydir)
 
         return env
 
 
 # Command-line interface
 
 from .. import DefaultExecCommand, DefaultShellCommand
 
-class CasaTool (multitool.Multitool):
+class CasaTool(multitool.Multitool):
     cli_name = 'pkenvtool casa'
     summary = 'Run programs in the CASA environment.'
 
-    def invoke_command (self, cmd, args, **kwargs):
-        return super (CasaTool, self).invoke_command (cmd, args,
-                                                      envname='casa',
-                                                      envclass=CasaEnvironment,
-                                                      module=__package__,
-                                                      **kwargs)
+    def invoke_command(self, cmd, args, **kwargs):
+        return super(CasaTool, self).invoke_command(cmd, args,
+                                                    envname='casa',
+                                                    envclass=CasaEnvironment,
+                                                    module=__package__,
+                                                    **kwargs)
 
 
-def commandline (argv):
+def commandline(argv):
     from six import itervalues
-    tool = CasaTool ()
-    tool.populate (itervalues (globals ()))
-    tool.commandline (argv)
+    tool = CasaTool()
+    tool.populate(itervalues(globals()))
+    tool.commandline(argv)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/tasks.py` & `pwkit-1.0.0/pwkit/environments/casa/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from . import util
 from ... import binary_type, reraise_context, text_type, PKError
 from ...cli import check_usage, wrong_usage, warn, die
 from ...kwargv import ParseKeywords, Custom
 
 # Keep the tasks alphabetized!
 
-__all__ = str ('''
+__all__ = str('''
 applycal applycal_cli ApplycalConfig
 bpplot bpplot_cli BpplotConfig
 clearcal clearcal_cli
 closures_cli
 concat concat_cli
 delcal delcal_cli
 delmod_cli
@@ -53,51 +53,50 @@
 gpplot gpplot_cli GpplotConfig
 image2fits image2fits_cli
 importalma importalma_cli
 importevla importevla_cli
 listobs listobs_cli
 listsdm listsdm_cli
 mfsclean mfsclean_cli MfscleanConfig
-mjd2date_cli
+mjd2date mjd2date_cli
 mstransform mstransform_cli MstransformConfig
 plotants plotants_cli
 plotcal plotcal_cli PlotcalConfig
 polmodel_cli
 setjy setjy_cli SetjyConfig
 split split_cli SplitConfig
 spwglue_cli
 tsysplot tsysplot_cli TsysplotConfig
 uvsub uvsub_cli UvsubConfig
 xyphplot xyphplot_cli XyphplotConfig
 commandline
-''').split ()
+''').split()
 
 
 # Some utilities
 
 from .util import sanitize_unicode as b
 
 precal_doc = \
 """
-*** Pre-applied calibrations:
+**Pre-applied calibrations**
 
 gaintable=
   Comma-separated list of calibration tables to apply on-the-fly
   before solving
 
 gainfield=
   SEMICOLON-separated list of field selections to apply for each gain table.
   If there are fewer items than there are gaintable items, the list is
   padded with blank items, implying no selection by field.
 
 interp=
   COMMA-separated list of interpolation types to use for each gain
   table. If there are fewer items, the list is padded with 'linear'
-  entries. Allowed values:
-    nearest linear cubic spline
+  entries. Allowed values: nearest linear cubic spline
 
 spwmap=
   SEMICOLON-separated list of spectral window mappings for each
   existing gain table; each record is a COMMA-separated list of
   integers. For the i'th spw in the dataset, spwmap[i] specifies
   the record in the gain table to use. For instance [0, 0, 1, 1]
   maps four spws in the UV data to just two spectral windows in
@@ -115,129 +114,182 @@
 parang=
   Whether to apply parallactic angle rotation correction
   (default: false)
 """
 
 stdsel_doc = \
 """
-*** Standard data selection keywords:
-
-antenna=
-array=
-correlation=
-field=
-intent=
-observation=
-scan=
-spw=
-taql=
-timerange=
-uvrange=
+Standard data selection keywords
+  This task can filter input data using any of the following keywords,
+  specified as in the standard CASA interface: ``antenna``, ``array``,
+  ``correlation``, ``field``, ``intent``, ``observation``, ``scan``, ``spw``,
+  ``taql``, ``timerange``, ``uvrange``.
 """
 
 loglevel_doc = \
 """
 loglevel=
-  Level of detail from CASA logging system. Default: warn; allowed:
-    severe warn info info1 info2 info3 info4 info5 debug1 debug2 debugging
+  Level of detail from CASA logging system. Default value is ``warn``. Allowed
+  values are: ``severe``, ``warn``, ``info``, ``info1``, ``info2``, ``info3``,
+  ``info4``, ``info5``, ``debug1``, ``debug2``, ``debugging``.
 """
 
-def extractmsselect (cfg, havearray=False, havecorr=False, haveintent=True,
-                     intenttoscanintent=False, taqltomsselect=True,
-                     observationtoobs=False):
+def extractmsselect(cfg, havearray=False, havecorr=False, haveintent=True,
+                    intenttoscanintent=False, taqltomsselect=True,
+                    observationtoobs=False):
     # expects cfg to have:
     #  antenna [correlation] field intent observation scan spw taql timerange uvrange
     # fills a dict with:
     #  baseline [correlation] field intent (msselect|taql) observation scan spw time uvrange
 
     selkws = {}
 
-    direct = 'field scan spw uvrange'.split ()
-    indirect = 'antenna:baseline timerange:time'.split ()
+    direct = 'field scan spw uvrange'.split()
+    indirect = 'antenna:baseline timerange:time'.split()
 
     if havearray:
-        indirect.append ('array:subarray')
+        indirect.append('array:subarray')
 
     if havecorr:
-        direct.append ('correlation')
+        direct.append('correlation')
 
     if haveintent:
         if intenttoscanintent:
-            indirect.append ('intent:scanintent')
+            indirect.append('intent:scanintent')
         else:
-            direct.append ('intent')
+            direct.append('intent')
 
     if observationtoobs:
-        indirect.append ('observation:obs')
+        indirect.append('observation:obs')
     else:
-        direct.append ('observation')
+        direct.append('observation')
 
     if taqltomsselect:
-        indirect.append ('taql:msselect')
+        indirect.append('taql:msselect')
     else:
-        direct.append ('taql')
+        direct.append('taql')
 
     for k in direct:
-        selkws[k] = getattr (cfg, k) or ''
+        selkws[k] = getattr(cfg, k) or ''
 
     for p in indirect:
-        ck, sk = p.split (':')
-        selkws[sk] = getattr (cfg, ck) or ''
+        ck, sk = p.split(':')
+        selkws[sk] = getattr(cfg, ck) or ''
 
     return selkws
 
 
-def applyonthefly (cb, cfg):
+def applyonthefly(cb, cfg):
     # expects cfg to have:
     #   gaintable gainfield interp spwmap opacity gaincurve parang
 
-    n = len (cfg.gaintable)
+    n = len(cfg.gaintable)
 
     # fill in missing values, taking care not to mutate cfg.
 
-    gainfields = list (cfg.gainfield)
-    interps = list (cfg.interp)
-    spwmaps = list (cfg.spwmap)
-
-    if len (gainfields) < n:
-        gainfields += [''] * (n - len (gainfields))
-    elif len (gainfields) > n:
-        raise ValueError ('more "gainfield" entries than "gaintable" entries')
-
-    if len (interps) < n:
-        interps += ['linear'] * (n - len (interps))
-    elif len (interps) > n:
-        raise ValueError ('more "interp" entries than "gaintable" entries')
-
-    if len (spwmaps) < n:
-        spwmaps += [[-1]] * (n - len (spwmaps))
-    elif len (spwmaps) > n:
-        raise ValueError ('more "spwmap" entries than "gaintable" entries')
+    gainfields = list(cfg.gainfield)
+    interps = list(cfg.interp)
+    spwmaps = list(cfg.spwmap)
+
+    if len(gainfields) < n:
+        gainfields += [''] * (n - len(gainfields))
+    elif len(gainfields) > n:
+        raise ValueError('more "gainfield" entries than "gaintable" entries')
+
+    if len(interps) < n:
+        interps += ['linear'] * (n - len(interps))
+    elif len(interps) > n:
+        raise ValueError('more "interp" entries than "gaintable" entries')
+
+    if len(spwmaps) < n:
+        spwmaps += [[-1]] * (n - len(spwmaps))
+    elif len(spwmaps) > n:
+        raise ValueError('more "spwmap" entries than "gaintable" entries')
 
-    for table, field, interp, spwmap in zip (cfg.gaintable, gainfields,
+    for table, field, interp, spwmap in zip(cfg.gaintable, gainfields,
                                              interps, spwmaps):
-        cb.setapply (table=b(table), field=b(field), interp=b(interp), spwmap=b(spwmap),
+        cb.setapply(table=b(table), field=b(field), interp=b(interp), spwmap=b(spwmap),
                      t=0., calwt=True)
 
-    if len (cfg.opacity):
-        cb.setapply (type=b'TOPAC', opacity=b(cfg.opacity), t=-1, calwt=True)
+    if len(cfg.opacity):
+        cb.setapply(type=b'TOPAC', opacity=b(cfg.opacity), t=-1, calwt=True)
 
     if cfg.gaincurve:
-        cb.setapply (type=b'GAINCURVE', t=-1, calwt=True)
+        cb.setapply(type=b'GAINCURVE', t=-1, calwt=True)
 
     if cfg.parang:
-        cb.setapply (type=b'P')
+        cb.setapply(type=b'P')
+
+
+_kwcli_cfg_class_doc_template = """\
+This is a configuration object for the ``%(taskname)s`` task. This object
+contains no methods. Rather it contains placeholders (and default values) for
+parameters that can be passed to :func:`%(taskname)s`.
+
+The following documentation is written to target the **command-line** version
+of this task, which may be invoked as ``casatask %(taskname)s``. “Keywords”
+refer attributes of this structure, “comma-separated lists” should become
+Python lists, and so on.
+
+%(bulk)s
+"""
+
+def makecfgdoc(taskname, doc):
+    """In Python 2.x you can't alter the __doc__ of a class after you define it,
+    so we need to provide a function that does the munging when we define each
+    class. This is that function.
+
+    """
+    doc_args = dict(
+        bulk = '\n'.join(l for l in doc.splitlines() if not l.startswith ('casatask ')),
+        taskname = taskname
+    )
+
+    return _kwcli_cfg_class_doc_template % doc_args
+
+_kwcli_impl_doc_template = """\
+The ``%(taskname)s`` task.
+
+cfg
+    A :class:`%(cfgname)s` object.
+
+This function runs the ``%(taskname)s`` task. *For documentation of the
+general functionality of this task and the parameters it takes*, see the
+documentation for the :class:`%(cfgname)s` object below. Example::
+
+    from pwkit.environments.casa import tasks
 
+    cfg = tasks.%(cfgname)s()
+    cfg.vis = 'mydataset.ms'
+    # ... set other parameters ...
+    tasks.%(taskname)s(cfg)
+
+This task may also be invoked through the command line, as ``casatask
+%(taskname)s``. Run ``casatask %(taskname)s --help`` to see another version of
+the documentation provided below.
+
+"""
+
+def makekwcli(doc, cfgclass, impl):
+    def kwclifunc(argv):
+        check_usage(doc, argv, usageifnoargs=True)
+        cfg = cfgclass().parse(argv[1:])
+        util.logger(cfg.loglevel)
+        impl(cfg)
+
+    # Doc magic
+
+    doc_args = dict(
+        bulk = '\n'.join(l for l in doc.splitlines() if not l.startswith ('casatask ')),
+        cfgname = cfgclass.__name__,
+        taskname = impl.__name__,
+    )
+
+    impl.__doc__ = _kwcli_impl_doc_template % doc_args
 
-def makekwcli (doc, cfgclass, impl):
-    def kwclifunc (argv):
-        check_usage (doc, argv, usageifnoargs=True)
-        cfg = cfgclass ().parse (argv[1:])
-        util.logger (cfg.loglevel)
-        impl (cfg)
     return kwclifunc
 
 
 # applycal
 
 applycal_doc = \
 """
@@ -251,25 +303,29 @@
 
 calwt=
   Write out calibrated weights as well as calibrated visibilities.
   Default: false
 """ + precal_doc + stdsel_doc + loglevel_doc
 
 
-class ApplycalConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class ApplycalConfig(ParseKeywords):
+    __doc__ = makecfgdoc('applycal', applycal_doc)
+
+    vis = Custom(str, required=True)
     calwt = False
     # skipping: flagbackup
 
     gaintable = [str]
-    gainfield = Custom ([str], sep=';')
+    gainfield = Custom([str], sep=';')
     interp = [str]
-    @Custom ([str], sep=';')
-    def spwmap (v):
-        return [map (int, e.split (',')) for e in v]
+    @Custom([str], sep=';')
+    def spwmap(v):
+        if v is None:
+            return None
+        return [list(map(int, e.split(','))) for e in v]
     opacity = [float]
     gaincurve = False
     parang = False
 
     antenna = str
     field = str
     intent = str
@@ -281,29 +337,29 @@
     uvrange = str
 
     applymode = 'calflag' # almost never want to change this
 
     loglevel = 'warn'
 
 
-def applycal (cfg):
-    cb = util.tools.calibrater ()
-    cb.open (filename=b(cfg.vis), compress=False, addcorr=True, addmodel=False)
+def applycal(cfg):
+    cb = util.tools.calibrater()
+    cb.open(filename=b(cfg.vis), compress=False, addcorr=True, addmodel=False)
 
-    selkws = extractmsselect (cfg)
+    selkws = extractmsselect(cfg)
     selkws['chanmode'] = 'none' # ?
-    cb.selectvis (**b(selkws))
+    cb.selectvis(**selkws)
 
-    applyonthefly (cb, cfg)
+    applyonthefly(cb, cfg)
 
-    cb.correct (b(cfg.applymode))
-    cb.close ()
+    cb.correct(b(cfg.applymode))
+    cb.close()
 
 
-applycal_cli = makekwcli (applycal_doc, ApplycalConfig, applycal)
+applycal_cli = makekwcli(applycal_doc, ApplycalConfig, applycal)
 
 
 # bpplot
 #
 # plotcal() can do this, but it is slow, ugly, and has not-very-informative
 # output. Yes, CASA is so crappy that I can even speed up bandpass plotting
 # by an order of magnitude.
@@ -336,151 +392,209 @@
 
 margins=TOP,RIGHT,LEFT,BOTTOM
   If saving to a file, the plot margins in the same units as the dims.
   The default is 4 on every side.
 """ + loglevel_doc
 
 
-class BpplotConfig (ParseKeywords):
-    caltable = Custom (str, required=True)
+class BpplotConfig(ParseKeywords):
+    __doc__ = makecfgdoc('bpplot', bpplot_doc)
+
+    caltable = Custom(str, required=True)
     dest = str
     dims = [1000, 600]
     margins = [4, 4, 4, 4]
     loglevel = 'warn'
 
 
-def bpplot (cfg):
+def bpplot(cfg):
     import omega as om, omega.render
     from ... import numutil
 
-    if isinstance (cfg.dest, omega.render.Pager):
+    if isinstance(cfg.dest, omega.render.Pager):
         # This is for non-CLI invocation.
         pager = cfg.dest
     elif cfg.dest is None:
         import omega.gtk3
-        pager = om.makeDisplayPager ()
+        pager = om.makeDisplayPager()
     else:
-        pager = om.makePager (cfg.dest,
+        pager = om.makePager(cfg.dest,
                               dims=cfg.dims,
                               margins=cfg.margins,
-                              style=om.styles.ColorOnWhiteVector ())
+                              style=om.styles.ColorOnWhiteVector())
 
-    tb = util.tools.table ()
+    tb = util.tools.table()
 
-    tb.open (binary_type (cfg.caltable), nomodify=True)
-    spws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    ants = tb.getcol (b'ANTENNA1')
-    vals = tb.getcol (b'CPARAM')
-    flags = tb.getcol (b'FLAG')
-    tb.close ()
-
-    tb.open (binary_type (os.path.join (cfg.caltable, 'ANTENNA')), nomodify=True)
-    names = tb.getcol (b'NAME')
-    tb.close ()
+    # Initial recon
 
-    npol, nchan, nsoln = vals.shape
+    tb.open(cfg.caltable, nomodify=True)
+    spws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    ants = tb.getcol(b'ANTENNA1')
+    tb.close()
 
-    # see what we've got
+    tb.open(os.path.join(cfg.caltable, 'ANTENNA'), nomodify=True)
+    names = tb.getcol(b'NAME')
+    tb.close()
+
+    nsoln = ants.size
+
+    # Load up and organize main data. We can't load CPARAM and FLAG all at
+    # once since different spws might have different nchans and/or npols.
 
     antpols = {}
-    seenspws = set ()
+    seenspws = set()
+    vals = [None] * nsoln
+    flags = [None] * nsoln
+    npol = {}
+    nchan = {}
+
+    tb.open(cfg.caltable, nomodify=True)
+
+    for isoln in range(nsoln):
+        vals[isoln] = this_vals = tb.getcell(b'CPARAM', isoln)
+        flags[isoln] = this_flags = tb.getcell(b'FLAG', isoln)
+        this_spw = spws[isoln]
+        this_npol, this_nchan = this_vals.shape
+
+        prev_npol = npol.get(this_spw)
+        if prev_npol is None:
+            npol[this_spw] = this_npol
+        elif this_npol != prev_npol:
+            raise Exception('assumptions violated: npol varies by solution for spw %s' % this_spw)
+
+        prev_nchan = nchan.get(this_spw)
+        if prev_nchan is None:
+            nchan[this_spw] = this_nchan
+        elif this_nchan != prev_nchan:
+            raise Exception('assumptions violated: nchan varies by solution for spw %s' % this_spw)
+
+        for ipol in range(this_npol):
+            if not this_flags[ipol].all():  # make sure to ignore completely-flagged records
+                 k = (ants[isoln], ipol)
+                 byspw = antpols.get(k)
+                 if byspw is None:
+                     antpols[k] = byspw = []
+
+                 byspw.append((spws[isoln], isoln))
+                 seenspws.add(spws[isoln])
+
+    tb.close()
+
+    seenspws = sorted(seenspws)
+    spw_to_offset = {}
+    tot_seen_nchan = 0
 
-    for ipol in range (npol):
-        for isoln in range (nsoln):
-            if not flags[ipol,:,isoln].all ():
-                k = (ants[isoln], ipol)
-                byspw = antpols.get (k)
-                if byspw is None:
-                    antpols[k] = byspw = []
-
-                byspw.append ((spws[isoln], isoln))
-                seenspws.add (spws[isoln])
-
-    seenspws = sorted (seenspws)
-    spw_to_offset = dict ((spwid, spwofs * nchan)
-                          for spwofs, spwid in enumerate (seenspws))
+    for ispw in seenspws:
+        spw_to_offset[ispw] = tot_seen_nchan
+        tot_seen_nchan += nchan[ispw]
 
     # normalize phases to avoid distracting wraps
 
-    for iant, ipol in sorted (six.iterkeys (antpols)):
+    for iant, ipol in sorted(six.iterkeys(antpols)):
         for ispw, isoln in antpols[iant,ipol]:
-            f = flags[ipol,:,isoln]
-            meanph = np.angle (vals[ipol,~f,isoln].mean ())
-            vals[ipol,:,isoln] *= np.exp (-1j * meanph)
+            f = flags[isoln][ipol]
+            meanph = np.angle(vals[isoln][ipol,~f].mean())
+            vals[isoln][ipol] *= np.exp(-1j * meanph)
 
     # find plot limits
 
-    okvals = vals[np.where (~flags)]
+    max_am = None
+
+    for isoln in range(nsoln):
+        this_vals = vals[isoln]
+        this_flags = flags[isoln]
+
+        okvals = this_vals[np.where(~this_flags)]
+        if not okvals.size:
+            continue
+
+        this_max_am = np.abs(okvals).max()
+        this_min_am = np.abs(okvals).min()
+        this_max_ph = np.angle(okvals, deg=True).max()
+        this_min_ph = np.angle(okvals, deg=True).min()
+
+        if max_am is None:
+            max_am = this_max_am
+            min_am = this_min_am
+            max_ph = this_max_ph
+            min_ph = this_min_ph
+        else:
+            max_am = max(max_am, this_max_am)
+            min_am = min(min_am, this_min_am)
+            max_ph = max(max_ph, this_max_ph)
+            min_ph = min(min_ph, this_min_ph)
 
-    max_am = np.abs (okvals).max ()
-    min_am = np.abs (okvals).min ()
     span = max_am - min_am
+    if span == 0:
+        span = 0.1 * max_am
+    if span == 0:
+        span = 1
     max_am += 0.05 * span
     min_am -= 0.05 * span
 
-    max_ph = np.angle (okvals, deg=True).max ()
-    min_ph = np.angle (okvals, deg=True).min ()
     span = max_ph - min_ph
+    if span == 0:
+        span = 60
     max_ph += 0.05 * span
     min_ph -= 0.05 * span
     if max_ph > 160:
         max_ph = 180
     if min_ph < -160:
         min_ph = -180
 
     polnames = 'RL' # XXX: identification doesn't seem to be stored in cal table
 
     # plot away
 
-    for iant, ipol in sorted (six.iterkeys (antpols)):
-        p_am = om.RectPlot ()
-        p_ph = om.RectPlot ()
+    for iant, ipol in sorted(six.iterkeys(antpols)):
+        p_am = om.RectPlot()
+        p_ph = om.RectPlot()
 
         for ispw, isoln in antpols[iant,ipol]:
-            f = flags[ipol,:,isoln]
-            a = np.abs (vals[ipol,:,isoln])
-            p = np.angle (vals[ipol,:,isoln], deg=True)
-            w = np.where (~f)[0]
+            f = flags[isoln][ipol]
+            a = np.abs(vals[isoln][ipol])
+            p = np.angle(vals[isoln][ipol], deg=True)
+            w = np.where(~f)[0]
 
-            for s in numutil.slice_around_gaps (w, 1):
+            for s in numutil.slice_around_gaps(w, 1):
                 wsub = w[s]
                 if wsub.size == 0:
                     continue # Should never happen, but eh.
                 else:
                     # It'd also be pretty weird to have a spectral window
-                    # containing just one (valid) channel, but it could
+                    # containing just one(valid) channel, but it could
                     # happen.
                     lines = (wsub.size > 1)
 
-                p_am.addXY (wsub + spw_to_offset[ispw], a[wsub], None,
+                p_am.addXY(wsub + spw_to_offset[ispw], a[wsub], None,
                             lines=lines, dsn=ispw)
-                p_ph.addXY (wsub + spw_to_offset[ispw], p[wsub], None,
+                p_ph.addXY(wsub + spw_to_offset[ispw], p[wsub], None,
                             lines=lines, dsn=ispw)
 
-        p_am.setBounds (xmin=0,
-                        xmax=len (seenspws) * nchan,
+        p_am.setBounds(xmin=0,
+                        xmax=tot_seen_nchan,
                         ymin=min_am,
                         ymax=max_am)
-        p_ph.setBounds (xmin=0,
-                        xmax=len (seenspws) * nchan,
+        p_ph.setBounds(xmin=0,
+                        xmax=tot_seen_nchan,
                         ymin=min_ph,
                         ymax=max_ph)
-        p_am.addKeyItem ('%s %s' % (names[iant], polnames[ipol]))
+        p_am.addKeyItem('%s %s' % (names[iant], polnames[ipol]))
 
         p_am.bpainter.paintLabels = False
-        p_am.setYLabel ('Amplitude')
-        p_ph.setLabels ('Normalized channel', 'De-meaned Phase (deg)')
+        p_am.setYLabel('Amplitude')
+        p_ph.setLabels('Normalized channel', 'De-meaned Phase(deg)')
 
-        vb = om.layout.VBox (2)
+        vb = om.layout.VBox(2)
         vb[0] = p_am
         vb[1] = p_ph
-        vb.setWeight (0, 2.5)
-        pager.send (vb)
+        vb.setWeight(0, 2.5)
+        pager.send(vb)
 
-bpplot_cli = makekwcli (bpplot_doc, BpplotConfig, bpplot)
+bpplot_cli = makekwcli(bpplot_doc, BpplotConfig, bpplot)
 
 
 # clearcal
 
 clearcal_doc = \
 """
 casatask clearcal [-w] <vis1> [more vises...]
@@ -506,60 +620,85 @@
                              'option': 0,
                              'shape': None,
                              'valueType': 'float'}
 clearcal_imaging_dminfo_tmpl = {'TYPE': 'TiledShapeStMan',
                                 'SPEC': {'DEFAULTTILESHAPE': [32, 128]},
                                 'NAME': 'imagingweight'}
 
-def clearcal (vis, weightonly=False):
-    tb = util.tools.table ()
-    cb = util.tools.calibrater ()
+def clearcal(vis, weightonly=False):
+    """Fill the imaging and calibration columns (``MODEL_DATA``,
+    ``CORRECTED_DATA``, ``IMAGING_WEIGHT``) of each measurement set with
+    default values, creating the columns if necessary.
+
+    vis (string)
+      Path to the input measurement set
+    weightonly (boolean)
+      If true, just create the ``IMAGING_WEIGHT`` column; do not fill
+      in the visibility data columns.
+
+    If you want to reset calibration models, these days you probably want
+    :func:`delmod_cli`. If you want to quickly make the columns go away, you
+    probably want :func:`delcal`.
+
+    Example::
+
+      from pwkit.environments.casa import tasks
+      tasks.clearcal('myvis.ms')
+
+    """
+    tb = util.tools.table()
+    cb = util.tools.calibrater()
 
     # cb.open() will create the tables if they're not present, so
     # if that's the case, we don't actually need to run initcalset()
 
-    tb.open (b(vis), nomodify=False)
-    colnames = tb.colnames ()
-    needinit = ('MODEL_DATA' in colnames) or ('CORRECTED_DATA' in colnames)
+    tb.open(b(vis), nomodify=False)
+    colnames = tb.colnames()
+    needinit = ('MODEL_DATA' in colnames) or('CORRECTED_DATA' in colnames)
     if 'IMAGING_WEIGHT' not in colnames:
-        c = dict (clearcal_imaging_col_tmpl)
-        c['shape'] = tb.getcell (b'DATA', 0).shape[-1:]
-        tb.addcols ({b'IMAGING_WEIGHT': c}, clearcal_imaging_dminfo_tmpl)
-    tb.close ()
+        c = dict(clearcal_imaging_col_tmpl)
+        c['shape'] = tb.getcell(b'DATA', 0).shape[-1:]
+        tb.addcols({b'IMAGING_WEIGHT': c}, clearcal_imaging_dminfo_tmpl)
+    tb.close()
 
     if not weightonly:
-        cb.open (b(vis))
+        import casadef
+
+        if casadef.casa_version.startswith('5.'):
+            cb.setvi(old=True, quiet=False)
+
+        cb.open(b(vis))
         if needinit:
-            cb.initcalset ()
-        cb.close ()
+            cb.initcalset()
+        cb.close()
 
 
-def clearcal_cli (argv):
-    check_usage (clearcal_doc, argv, usageifnoargs=True)
+def clearcal_cli(argv):
+    check_usage(clearcal_doc, argv, usageifnoargs=True)
 
-    argv = list (argv)
+    argv = list(argv)
     weightonly = '-w' in argv
     if weightonly:
-        sys.argv.remove ('-w')
+        sys.argv.remove('-w')
 
-    if len (argv) < 2:
-        wrong_usage (clearcal_doc, 'need at least one argument')
+    if len(argv) < 2:
+        wrong_usage(clearcal_doc, 'need at least one argument')
 
-    util.logger ()
+    util.logger()
     for vis in argv[1:]:
-        clearcal (b(vis), weightonly=weightonly)
+        clearcal(b(vis), weightonly=weightonly)
 
 
 # closures
 #
 # Shim for a separate module
 
-def closures_cli (argv):
+def closures_cli(argv):
     from .closures import closures_cli
-    closures_cli (argv)
+    closures_cli(argv)
 
 
 # concat
 
 concat_doc = \
 """
 casatask concat [-s] <input vises ...> <output vis>
@@ -568,58 +707,73 @@
 
 -s - sort the output in time
 """
 
 concat_freqtol = 1e-5
 concat_dirtol = 1e-5
 
-def concat (invises, outvis, timesort=False):
-    tb = util.tools.table ()
-    ms = util.tools.ms ()
+def concat(invises, outvis, timesort=False):
+    """Concatenate visibility measurement sets.
+
+    invises (list of str)
+      Paths to the input measurement sets
+    outvis (str)
+      Path to the output measurement set.
+    timesort (boolean)
+      If true, sort the output in time after concatenation.
+
+    Example::
 
-    if os.path.exists (outvis):
-        raise RuntimeError ('output "%s" already exists' % outvis)
+      from pwkit.environments.casa import tasks
+      tasks.concat(['epoch1.ms', 'epoch2.ms'], 'combined.ms')
+
+    """
+    tb = util.tools.table()
+    ms = util.tools.ms()
+
+    if os.path.exists(outvis):
+        raise RuntimeError('output "%s" already exists' % outvis)
 
     for invis in invises:
-        if not os.path.isdir (invis):
-            raise RuntimeError ('input "%s" does not exist' % invis)
+        if not os.path.isdir(invis):
+            raise RuntimeError('input "%s" does not exist' % invis)
 
-    tb.open (b(invises[0]))
-    tb.copy (b(outvis), deep=True, valuecopy=True)
-    tb.close ()
+    tb.open(b(invises[0]))
+    tb.copy(b(outvis), deep=True, valuecopy=True)
+    tb.close()
 
-    ms.open (b(outvis), nomodify=False)
+    ms.open(b(outvis), nomodify=False)
 
     for invis in invises[1:]:
-        ms.concatenate (msfile=b(invis), freqtol=b(concat_freqtol),
+        ms.concatenate(msfile=b(invis), freqtol=b(concat_freqtol),
                         dirtol=b(concat_dirtol))
 
-    ms.writehistory (message=b'taskname=tasklib.concat', origin=b'tasklib.concat')
-    ms.writehistory (message=b('vis = ' + ', '.join (invises)), origin=b'tasklib.concat')
-    ms.writehistory (message=b('timesort = ' + 'FT'[int (timesort)]), origin=b'tasklib.concat')
+    ms.writehistory(message=b'taskname=tasklib.concat', origin=b'tasklib.concat')
+    ms.writehistory(message=b('vis = ' + ', '.join(invises)), origin=b'tasklib.concat')
+    ms.writehistory(message=b('timesort = ' + 'FT'[int(timesort)]), origin=b'tasklib.concat')
 
     if timesort:
-        ms.timesort ()
+        ms.timesort()
 
-    ms.close ()
+    ms.close()
 
 
-def concat_cli (argv):
-    check_usage (concat_doc, argv, usageifnoargs=True)
+def concat_cli(argv):
+    check_usage(concat_doc, argv, usageifnoargs=True)
 
-    argv = list (argv)
+    argv = list(argv)
     timesort = '-s' in argv
     if timesort:
-        sys.argv.remove ('-s')
+        sys.argv.remove('-s')
 
-    if len (argv) < 3:
-        wrong_usage (concat_doc, 'need at least two arguments')
+    if len(argv) < 3:
+        wrong_usage(concat_doc, 'need at least two arguments')
 
-    util.logger ()
-    concat (argv[1:-1], argv[-1], timesort)
+    util.logger()
+    concat(argv[1:-1], argv[-1], timesort)
 
 
 # delcal
 #
 # Not a CASA task. Delmod on steroids, at least when delmod
 # is operating on scratch columns and not OTF models.
 
@@ -627,36 +781,53 @@
 """
 casatask delcal <ms> [mses...]
 
 Delete the MODEL_DATA and CORRECTED_DATA columns from MSes.
 """
 
 
-def delcal (mspath):
-    wantremove = 'MODEL_DATA CORRECTED_DATA'.split ()
-    tb = util.tools.table ()
-    tb.open (b(mspath), nomodify=False)
-    cols = frozenset (tb.colnames ())
+def delcal(mspath):
+    """Delete the ``MODEL_DATA`` and ``CORRECTED_DATA`` columns from a measurement set.
+
+    mspath (str)
+      The path to the MS to modify
+
+    Example::
+
+      from pwkit.environments.casa import tasks
+      tasks.delcal('dataset.ms')
+
+    """
+    wantremove = 'MODEL_DATA CORRECTED_DATA'.split()
+    tb = util.tools.table()
+    tb.open(b(mspath), nomodify=False)
+    cols = frozenset(tb.colnames())
     toremove = [b(c) for c in wantremove if c in cols]
-    if len (toremove):
-        tb.removecols (toremove)
-    tb.close ()
-    return toremove
+    if len(toremove):
+        tb.removecols(toremove)
+    tb.close()
+
+    # We want to return a `str` type, which is what we already
+    # have in Python 2 but not in 3.
+    if six.PY2:
+        return toremove
+    else:
+        return [c.decode('utf8') for c in toremove]
 
 
-def delcal_cli (argv):
-    check_usage (delcal_doc, argv, usageifnoargs=True)
-    util.logger ()
+def delcal_cli(argv):
+    check_usage(delcal_doc, argv, usageifnoargs=True)
+    util.logger()
 
     for mspath in argv[1:]:
-        removed = delcal (mspath)
-        if len (removed):
-            print ('%s: removed %s' % (mspath, ', '.join (removed)))
+        removed = delcal(mspath)
+        if len(removed):
+            print('%s: removed %s' % (mspath, ', '.join(removed)))
         else:
-            print ('%s: nothing to remove' % mspath)
+            print('%s: nothing to remove' % mspath)
 
 
 # delmod
 
 delmod_doc = \
 """
 casatask delmod <MS...>
@@ -666,52 +837,68 @@
 
 If you want to delete the scratch columns, use delcal. If you
 want to clear the scratch columns, use clearcal. I'm torn
 between wanting better terminology and not wanting to be
 gratuitously different from CASA.
 """
 
-def delmod_cli (argv, alter_logger=True):
-    check_usage (delmod_doc, argv, usageifnoargs=True)
+def delmod_cli(argv, alter_logger=True):
+    """Command-line access to ``delmod`` functionality.
+
+    The ``delmod`` task deletes "on-the-fly" model information from a
+    Measurement Set. It is so easy to implement that a standalone
+    function is essentially unnecessary. Just write::
+
+      from pwkit.environments.casa import util
+      cb = util.tools.calibrater()
+      cb.open('datasaet.ms', addcorr=False, addmodel=False)
+      cb.delmod(otf=True, scr=False)
+      cb.close()
+
+    If you want to delete the scratch columns, use :func:`delcal`. If you want
+    to clear the scratch columns, use :func:`clearcal`.
+
+    """
+    check_usage(delmod_doc, argv, usageifnoargs=True)
     if alter_logger:
-        util.logger ()
+        util.logger()
 
-    cb = util.tools.calibrater ()
+    cb = util.tools.calibrater()
 
     for mspath in argv[1:]:
-        cb.open (b(mspath), addcorr=False, addmodel=False)
-        cb.delmod (otf=True, scr=False)
-        cb.close ()
+        cb.open(b(mspath), addcorr=False, addmodel=False)
+        cb.delmod(otf=True, scr=False)
+        cb.close()
 
 
 # dftdynspec
 #
 # Shim for a separate module
 
-def dftdynspec_cli (argv):
+def dftdynspec_cli(argv):
     from .dftdynspec import dftdynspec_cli
-    dftdynspec_cli (argv)
+    dftdynspec_cli(argv)
 
 
 # dftphotom
 #
 # Shim for a separate module
 
-def dftphotom_cli (argv):
+def dftphotom_cli(argv):
     from .dftphotom import dftphotom_cli
-    dftphotom_cli (argv)
+    dftphotom_cli(argv)
 
 
 # dftspect
 #
 # Shim for a separate module
 
-def dftspect_cli (argv):
+def dftspect_cli(argv):
     from .dftspect import dftspect_cli
-    dftspect_cli (argv)
+    dftspect_cli(argv)
 
 
 # elplot
 #
 # See bpplot() -- CASA plotcal can do this in a certain sense, but it's slow
 # and ugly.
 
@@ -727,96 +914,98 @@
 dest=PATH
   If specified, plots are saved to this file -- the format is inferred
   from the extension, which must allow multiple pages to be saved. If
   unspecified, the plots are displayed using a Gtk3 backend.
 
 dims=WIDTH,HEIGHT
   If saving to a file, the dimensions of a each page. These are in points
-  for vector formats (PDF, PS) and pixels for bitmaps (PNG). Defaults to
+  for vector formats(PDF, PS) and pixels for bitmaps(PNG). Defaults to
   1000, 600.
 
 margins=TOP,RIGHT,LEFT,BOTTOM
   If saving to a file, the plot margins in the same units as the dims.
   The default is 4 on every side.
 """ + loglevel_doc
 
 
-class ElplotConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class ElplotConfig(ParseKeywords):
+    __doc__ = makecfgdoc('elplot', elplot_doc)
+
+    vis = Custom(str, required=True)
     dest = str
     dims = [1000, 600]
     margins = [4, 4, 4, 4]
     loglevel = 'warn'
 
 
-def elplot (cfg):
+def elplot(cfg):
     import omega as om, omega.render
 
-    if isinstance (cfg.dest, omega.render.Pager):
+    if isinstance(cfg.dest, omega.render.Pager):
         # This is for non-CLI invocation.
         pager = cfg.dest
     elif cfg.dest is None:
         import omega.gtk3
-        pager = om.makeDisplayPager ()
+        pager = om.makeDisplayPager()
     else:
-        pager = om.makePager (cfg.dest,
+        pager = om.makePager(cfg.dest,
                               dims=cfg.dims,
                               margins=cfg.margins,
-                              style=om.styles.ColorOnWhiteVector ())
+                              style=om.styles.ColorOnWhiteVector())
 
-    ms = util.tools.ms ()
-    me = util.tools.measures ()
+    ms = util.tools.ms()
+    me = util.tools.measures()
 
-    ms.open (binary_type (cfg.vis), nomodify=True)
-    scans = ms.range ([b'scan_number'])['scan_number']
+    ms.open(cfg.vis, nomodify=True)
+    scans = ms.range([b'scan_number'])['scan_number']
 
-    md = ms.metadata ()
-    field_names = md.namesforfields ()
-    obs = md.observatoryposition ()
-    me.doframe (b(obs))
-    timetmpl = md.timerangeforobs (0)['begin']
+    md = ms.metadata()
+    field_names = md.namesforfields()
+    obs = md.observatoryposition()
+    me.doframe(b(obs))
+    timetmpl = md.timerangeforobs(0)['begin']
 
-    mjd0 = int (np.floor (md.timesforscan (scans[0]).min () / 86400))
+    mjd0 = int(np.floor(md.timesforscan(scans[0]).min() / 86400))
 
     field_dsns = {}
 
-    p = om.RectPlot ()
+    p = om.RectPlot()
 
     for scan in scans:
-        mjds = md.timesforscan (scan=scan) / 86400
+        mjds = md.timesforscan(scan=scan) / 86400
 
-        fields = md.fieldsforscan (scan=scan)
+        fields = md.fieldsforscan(scan=scan)
         if fields.size != 1:
             import sys
-            print ('warning: scan %d does not contain one field: %r' % (scan, fields))
+            print('warning: scan %d does not contain one field: %r' % (scan, fields))
         field = fields[0]
 
-        fdir = ms.getfielddirmeas (fieldid=field)
-        els = np.empty (mjds.size)
+        fdir = ms.getfielddirmeas(fieldid=field)
+        els = np.empty(mjds.size)
 
-        for i in xrange (mjds.size):
+        for i in range(mjds.size):
             timetmpl['m0']['value'] = mjds[i]
-            me.doframe (b(timetmpl))
-            els[i] = me.measure (b(fdir), b'AZEL')['m1']['value'] * 180 / np.pi
+            me.doframe(b(timetmpl))
+            els[i] = me.measure(b(fdir), b'AZEL')['m1']['value'] * 180 / np.pi
 
-        dsn = field_dsns.get (field)
+        dsn = field_dsns.get(field)
         kt = None
 
         if dsn is None:
-            dsn = len (field_dsns)
+            dsn = len(field_dsns)
             field_dsns[field] = dsn
             kt = field_names[field]
 
-        p.addXY (mjds - mjd0, els, kt, dsn=dsn)
+        p.addXY(mjds - mjd0, els, kt, dsn=dsn)
 
-    p.setLabels ('MJD - %d (day)' % mjd0, 'Elevation (deg)')
-    pager.send (p)
-    pager.done ()
+    p.setLabels('MJD - %d(day)' % mjd0, 'Elevation(deg)')
+    pager.send(p)
+    pager.done()
 
-elplot_cli = makekwcli (elplot_doc, ElplotConfig, elplot)
+elplot_cli = makekwcli(elplot_doc, ElplotConfig, elplot)
 
 
 # extractbpflags
 #
 # Not a CASA task, but I've found this to be very useful.
 
 extractbpflags_doc = \
@@ -836,111 +1025,126 @@
 which the R and L bandpass solutions have different flags. But in CASA the
 flags seem to always be the same.
 
 We're assuming that the channelization of the bandpass solution and the data
 are the same.
 """
 
-def extractbpflags (calpath, deststream):
-    tb = util.tools.table ()
-    tb.open (b(os.path.join (calpath, 'ANTENNA')))
-    antnames = tb.getcol (b'NAME')
-    tb.close ()
+def extractbpflags(calpath, deststream):
+    """Make a flags file out of a bandpass calibration table
+
+    calpath (str)
+      The path to the bandpass calibration table
+    deststream (stream-like object, e.g. an opened file)
+      Where to write the flags data
 
-    tb.open (b(calpath))
+    Below is documentation written for the command-line interface to this
+    functionality:
+
+    """
+    tb = util.tools.table()
+    tb.open(b(os.path.join(calpath, 'ANTENNA')))
+    antnames = tb.getcol(b'NAME')
+    tb.close()
+
+    tb.open(b(calpath))
     try:
-        t = tb.getkeyword (b'VisCal')
+        t = tb.getkeyword(b'VisCal')
     except RuntimeError:
-        raise PKError ('no "VisCal" keyword in %s; it doesn\'t seem to be a '
+        raise PKError('no "VisCal" keyword in %s; it doesn\'t seem to be a '
                        'bandpass calibration table', calpath)
 
     if t != 'B Jones':
-        raise PKError ('table %s doesn\'t seem to be a bandpass calibration '
+        raise PKError('table %s doesn\'t seem to be a bandpass calibration '
                        'table; its type is "%s"', calpath, t)
 
-    def emit (antidx, spwidx, chanstart, chanend):
+    def emit(antidx, spwidx, chanstart, chanend):
         # Channel ranges are inclusive, unlike Python syntax.
-        print ("antenna='%s&*' spw='%d:%d~%d' reason='BANDPASS_FLAGGED'" % \
-               (antnames[antidx], spwidx, chanstart, chanend), file=deststream)
+        print("antenna='%s&*' spw='%d:%d~%d' reason='BANDPASS_FLAGGED'" % \
+              (antnames[antidx], spwidx, chanstart, chanend), file=deststream)
 
-    for row in range (tb.nrows ()):
-        ant = tb.getcell (b'ANTENNA1', row)
-        spw = tb.getcell (b'SPECTRAL_WINDOW_ID', row)
-        flag = tb.getcell (b'FLAG', row)
+    for row in range(tb.nrows()):
+        ant = tb.getcell(b'ANTENNA1', row)
+        spw = tb.getcell(b'SPECTRAL_WINDOW_ID', row)
+        flag = tb.getcell(b'FLAG', row)
 
         # This is the logical 'or' of the two polarizations: i.e., anything that
         # is flagged in either poln is flagged in this.
-        sqflag = ~((~flag).prod (axis=0, dtype=np.bool))
+        sqflag = ~((~flag).prod(axis=0, dtype=np.bool))
 
         runstart = None
 
-        for i in range (sqflag.size):
+        for i in range(sqflag.size):
             if sqflag[i]:
                 # This channel is flagged. Start a run if not already in one.
                 if runstart is None:
                     runstart = i
             elif runstart is not None:
                 # The current run just ended.
-                emit (ant, spw, runstart, i - 1)
+                emit(ant, spw, runstart, i - 1)
                 runstart = None
 
         if runstart is not None:
-            emit (ant, spw, runstart, i)
+            emit(ant, spw, runstart, i)
+
+    tb.close()
 
-    tb.close ()
+extractbpflags.__doc__ += extractbpflags_doc
 
 
-def extractbpflags_cli (argv):
-    check_usage (extractbpflags_doc, argv, usageifnoargs='long')
+def extractbpflags_cli(argv):
+    check_usage(extractbpflags_doc, argv, usageifnoargs='long')
 
-    if len (argv) != 2:
-        wrong_usage (extractbpflags_doc, 'expect one MS name as an argument')
+    if len(argv) != 2:
+        wrong_usage(extractbpflags_doc, 'expect one MS name as an argument')
 
-    extractbpflags (argv[1], sys.stdout)
+    extractbpflags(argv[1], sys.stdout)
 
 
 # flagcmd
 
 flagcmd_doc = \
 """
 casatask flagcmd vis= [keywords..]
 
 Flag data using auto-generated lists of flagging commands.
 
 """
 
-class FlagcmdConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class FlagcmdConfig(ParseKeywords):
+    __doc__ = makecfgdoc('flagcmd', flagcmd_doc)
+
+    vis = Custom(str, required=True)
     inpmode = 'table'
     useapplied = False
     action = 'apply'
     flagbackup = True
     loglevel = 'warn'
 
 
-def flagcmd (cfg):
+def flagcmd(cfg):
     from .scripting import CasapyScript
-    script = os.path.join (os.path.dirname (__file__), 'cscript_flagcmd.py')
+    script = os.path.join(os.path.dirname(__file__), 'cscript_flagcmd.py')
 
-    args = dict (
+    args = dict(
         vis = cfg.vis,
         inpmode = cfg.inpmode,
         useapplied = cfg.useapplied,
         action = cfg.action,
         flagbackup = cfg.flagbackup,
     )
 
-    with CasapyScript (script, **b(args)):
+    with CasapyScript(script, **args):
         pass
 
-flagcmd_cli = makekwcli (flagcmd_doc, FlagcmdConfig, flagcmd)
+flagcmd_cli = makekwcli(flagcmd_doc, FlagcmdConfig, flagcmd)
 
 
 # flaglist. Not quite a CASA task; something like
-# flagcmd (vis=, inpmode='list', inpfile=, flagbackup=False)
+# flagcmd(vis=, inpmode='list', inpfile=, flagbackup=False)
 #
 # We have to reproduce a lot of the dumb logic from the flaghelper.py module
 # because we can't import it because it drags in the whole casapy pile of
 # stuff.
 
 flaglist_doc = \
 """
@@ -951,209 +1155,222 @@
 flagbackup=False)'.
 
 This implementation must emulate the CASA modules that load up the
 flagging commands and may not be precisely compatible with the CASA
 version.
 """
 
-class FlaglistConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    inpfile = Custom (str, required=True)
+class FlaglistConfig(ParseKeywords):
+    __doc__ = makecfgdoc('flaglist', flaglist_doc)
+
+    vis = Custom(str, required=True)
+    inpfile = Custom(str, required=True)
     datacol = 'data'
     loglevel = 'warn'
 
 
-def flaglist (cfg):
+def flaglist(cfg):
     from ast import literal_eval
 
     try:
         factory = util.tools.agentflagger
     except AttributeError:
         factory = util.tools.testflagger
 
-    af = factory ()
-    af.open (b(cfg.vis), 0.0)
-    af.selectdata ()
-
-    for row, origline in enumerate (open (cfg.inpfile)):
-        origline = origline.rstrip ()
-        if not len (origline):
+    af = factory()
+    af.open(b(cfg.vis), 0.0)
+    af.selectdata()
+
+    for row, origline in enumerate(open(cfg.inpfile)):
+        origline = origline.rstrip()
+        if not len(origline):
             continue
         if origline[0] == '#':
             continue
 
         # emulating flaghelper.py here and elsewhere ...
-        bits = origline.replace ('true', 'True').replace ('false', 'False').split (' ')
+        bits = origline.replace('true', 'True').replace('false', 'False').split(' ')
         params = {}
         lastkey = None
 
         for bit in bits:
-            subbits = bit.split ('=', 1)
+            subbits = bit.split('=', 1)
 
-            if len (subbits) == 1:
+            if len(subbits) == 1:
                 assert lastkey is not None, 'illegal flag list syntax'
                 params[lastkey] += ' ' + bit
             else:
                 params[subbits[0]] = subbits[1]
                 lastkey = subbits[0]
 
         assert 'ntime' not in params, 'cannot handle "ntime" flag key'
 
-        for key in params.keys ():
+        for key in list(params.keys()):
             val = params[key]
 
             try:
-                val = literal_eval (val)
+                val = literal_eval(val)
             except ValueError:
-                val = val.strip ('\'"')
+                val = val.strip('\'"')
 
             params[key] = val
 
         params['name'] = 'agent_%d' % row
-        params['datacolumn'] = cfg.datacol.upper ()
+        params['datacolumn'] = cfg.datacol.upper()
         params['apply'] = True
 
-        params.setdefault ('mode', 'manual')
+        params.setdefault('mode', 'manual')
 
-        if not af.parseagentparameters (b(params)):
-            raise Exception ('cannot parse flag line: %s' % origline)
+        if not af.parseagentparameters(b(params)):
+            raise Exception('cannot parse flag line: %s' % origline)
 
-    af.init ()
+    af.init()
     # A summary report would be nice. run() should return
-    # info but I can't get it to do so. (I'm just trying to
+    # info but I can't get it to do so.(I'm just trying to
     # copy the task_flagdata.py implementation.)
-    af.run (True, True)
-    af.done ()
+    af.run(True, True)
+    af.done()
 
 
-flaglist_cli = makekwcli (flaglist_doc, FlaglistConfig, flaglist)
+flaglist_cli = makekwcli(flaglist_doc, FlaglistConfig, flaglist)
 
 
 # flagmanager. Not really complicated enough to make it worth making a
 # modular implementation to be driven from the CLI.
 
 flagmanager_doc = \
 """
 casatask flagmanager list <ms>
 casatask flagmanager save <ms> <name>
 casatask flagmanager restore <ms> <name>
 casatask flagmanager delete <ms> <name>
 """
 
-def flagmanager_cli (argv, alter_logger=True):
-    check_usage (flagmanager_doc, argv, usageifnoargs=True)
+def flagmanager_cli(argv, alter_logger=True):
+    """Command-line access to ``flagmanager`` functionality.
+
+    The ``flagmanager`` task manages tables of flags associated with
+    measurement sets. Its features are easy to implement that a standalone
+    library function is essentially unnecessary. See the source code to this
+    function for the tool calls that implement different parts of the
+    ``flagmanager`` functionality.
+
+    """
+    check_usage(flagmanager_doc, argv, usageifnoargs=True)
 
-    if len (argv) < 3:
-        wrong_usage (flagmanager_doc, 'expect at least a mode and an MS name')
+    if len(argv) < 3:
+        wrong_usage(flagmanager_doc, 'expect at least a mode and an MS name')
 
     mode = argv[1]
     ms = argv[2]
 
     if alter_logger:
         if mode == 'list':
-            util.logger ('info')
+            util.logger('info')
         elif mode == 'delete':
             # it WARNs 'deleting version xxx' ... yargh
-            util.logger ('severe')
+            util.logger('severe')
         else:
-            util.logger ()
+            util.logger()
 
     try:
         factory = util.tools.agentflagger
     except AttributeError:
         factory = util.tools.testflagger
 
-    af = factory ()
-    af.open (b(ms))
+    af = factory()
+    af.open(b(ms))
 
     if mode == 'list':
-        if len (argv) != 3:
-            wrong_usage (flagmanager_doc, 'expect exactly one argument in list mode')
-        af.getflagversionlist ()
+        if len(argv) != 3:
+            wrong_usage(flagmanager_doc, 'expect exactly one argument in list mode')
+        af.getflagversionlist()
     elif mode == 'save':
-        if len (argv) != 4:
-            wrong_usage (flagmanager_doc, 'expect exactly two arguments in save mode')
+        if len(argv) != 4:
+            wrong_usage(flagmanager_doc, 'expect exactly two arguments in save mode')
         from time import strftime
         name = argv[3]
-        af.saveflagversion (versionname=b(name), merge=b'replace',
-                            comment=b('created %s (casatask flagmanager)'
-                                      % strftime ('%Y-%m-%dT%H:%M:%SZ')))
+        af.saveflagversion(versionname=b(name), merge=b'replace',
+                            comment=b('created %s(casatask flagmanager)'
+                                      % strftime('%Y-%m-%dT%H:%M:%SZ')))
     elif mode == 'restore':
-        if len (argv) != 4:
-            wrong_usage (flagmanager_doc, 'expect exactly two arguments in restore mode')
+        if len(argv) != 4:
+            wrong_usage(flagmanager_doc, 'expect exactly two arguments in restore mode')
         name = argv[3]
-        af.restoreflagversion (versionname=b(name), merge=b'replace')
+        af.restoreflagversion(versionname=b(name), merge=b'replace')
     elif mode == 'delete':
-        if len (argv) != 4:
-            wrong_usage (flagmanager_doc, 'expect exactly two arguments in delete mode')
+        if len(argv) != 4:
+            wrong_usage(flagmanager_doc, 'expect exactly two arguments in delete mode')
         name = argv[3]
 
-        if not os.path.isdir (os.path.join (ms + '.flagversions', 'flags.' + name)):
-            # This condition only results in a WARN from deleteflagversion ()!
-            raise RuntimeError ('version "%s" doesn\'t exist in "%s.flagversions"'
+        if not os.path.isdir(os.path.join(ms + '.flagversions', 'flags.' + name)):
+            # This condition only results in a WARN from deleteflagversion()!
+            raise RuntimeError('version "%s" doesn\'t exist in "%s.flagversions"'
                                 % (name, ms))
 
-        af.deleteflagversion (versionname=b(name))
+        af.deleteflagversion(versionname=b(name))
     else:
-        wrong_usage (flagmanager_doc, 'unknown flagmanager mode "%s"' % mode)
+        wrong_usage(flagmanager_doc, 'unknown flagmanager mode "%s"' % mode)
 
-    af.done ()
+    af.done()
 
 
 # flagzeros. Not quite a CASA task; something like
-# flagdata (vis=, mode='clip', clipzeros=True, flagbackup=False)
+# flagdata(vis=, mode='clip', clipzeros=True, flagbackup=False)
 
 flagzeros_doc = \
 """
 casatask flagzeros vis= [datacol=]
 
 Flag zero data points in the specified data column.
 """
 
-class FlagzerosConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class FlagzerosConfig(ParseKeywords):
+    __doc__ = makecfgdoc('flagzeros', flagzeros_doc)
+
+    vis = Custom(str, required=True)
     datacol = 'data'
     loglevel = 'warn'
 
 
-def flagzeros (cfg):
+def flagzeros(cfg):
     try:
         factory = util.tools.agentflagger
     except AttributeError:
         factory = util.tools.testflagger
 
-    af = factory ()
-    af.open (b(cfg.vis), 0.0)
-    af.selectdata ()
-    pars = dict (datacolumn=cfg.datacol.upper (),
+    af = factory()
+    af.open(b(cfg.vis), 0.0)
+    af.selectdata()
+    pars = dict(datacolumn=cfg.datacol.upper(),
                  clipzeros=True, name='CLIP', mode='clip',
                  apply=True)
-    af.parseagentparameters (pars)
-    af.init ()
+    af.parseagentparameters(pars)
+    af.init()
     # A summary report would be nice. run() should return
-    # info but I can't get it to do so. (I'm just trying to
+    # info but I can't get it to do so.(I'm just trying to
     # copy the task_flagdata.py implementation.)
-    af.run (True, True)
-    af.done ()
+    af.run(True, True)
+    af.done()
 
 
-flagzeros_cli = makekwcli (flagzeros_doc, FlagzerosConfig, flagzeros)
+flagzeros_cli = makekwcli(flagzeros_doc, FlagzerosConfig, flagzeros)
 
 
 # fluxscale
 
 fluxscale_doc = \
 """
 casatask fluxscale vis=<MS> caltable=<MS> fluxtable=<new MS> reference=<fields> transfer=<fields> [keywords]
 
 Write a new calibation table determining the fluxes for intermediate calibrators
 from known reference sources
 
 vis=
-  The visibility dataset. (Shouldn't be needed, but ...)
+  The visibility dataset.(Shouldn't be needed, but ...)
 
 caltable=
   The preexisting calibration table with gains associated with more than one source.
 
 fluxtable=
   The path of a new calibration table to create
 
@@ -1175,79 +1392,81 @@
   map from the data to the gains. For instance, refspwmap=1,1,3,3 means that spw 0
   will have its flux calculated using the gains for spw 1.
 """ + loglevel_doc
 
 # Not supported in CASA 3.4:
 #incremental=
 #  Boolean, default false. If true, create an "incremental" table where the amplitudes
-#  are correction factors, not absolute gains. (I.e., for the reference sources,
+#  are correction factors, not absolute gains.(I.e., for the reference sources,
 #  the amplitudes will be unity.)
 
 
-class FluxscaleConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    caltable = Custom (str, required=True)
-    fluxtable = Custom (str, required=True)
-    reference = Custom ([str], required=True)
-    transfer = Custom ([str], required=True)
+class FluxscaleConfig(ParseKeywords):
+    __doc__ = makecfgdoc('fluxscale', fluxscale_doc)
+
+    vis = Custom(str, required=True)
+    caltable = Custom(str, required=True)
+    fluxtable = Custom(str, required=True)
+    reference = Custom([str], required=True)
+    transfer = Custom([str], required=True)
 
     listfile = str
     append = False
     refspwmap = [int]
     #incremental = False
 
     loglevel = 'warn'
 
 
-def fluxscale (cfg):
-    cb = util.tools.calibrater ()
+def fluxscale(cfg):
+    cb = util.tools.calibrater()
 
     reference = cfg.reference
-    if isinstance (reference, (list, tuple)):
-        reference = ','.join (reference)
+    if isinstance(reference,(list, tuple)):
+        reference = ','.join(reference)
 
     transfer = cfg.transfer
-    if isinstance (transfer, (list, tuple)):
-        transfer = ','.join (transfer)
+    if isinstance(transfer,(list, tuple)):
+        transfer = ','.join(transfer)
 
     refspwmap = cfg.refspwmap
-    if not len (refspwmap):
+    if not len(refspwmap):
         refspwmap = [-1]
 
-    cb.open (b(cfg.vis), compress=False, addcorr=False, addmodel=False)
-    result = cb.fluxscale (tablein=b(cfg.caltable), tableout=b(cfg.fluxtable),
+    cb.open(b(cfg.vis), compress=False, addcorr=False, addmodel=False)
+    result = cb.fluxscale(tablein=b(cfg.caltable), tableout=b(cfg.fluxtable),
                            reference=b(reference), transfer=b(transfer),
                            listfile=b(cfg.listfile or ''),
                            append=cfg.append, refspwmap=b(refspwmap))
                            #incremental=cfg.incremental)
-    cb.close ()
+    cb.close()
     return result
 
 
-fluxscale_cli = makekwcli (fluxscale_doc, FluxscaleConfig, fluxscale)
+fluxscale_cli = makekwcli(fluxscale_doc, FluxscaleConfig, fluxscale)
 
 
 # ft
 #
 # We derive 'nterms' from len(model), and always derive reffreq
 # from the model images. These seem like safe constraints?
 
 ft_doc = \
 """
 casatask ft vis=<MS> [keywords]
 
-Fill in (or update) the MODEL_DATA column of a Measurement Set with
+Fill in(or update) the MODEL_DATA column of a Measurement Set with
 visibilities computed from an image or list of components.
 
 vis=
   The path to the measurement set
 
 model=
   Comma-separated list of model images, each giving successive
-  Taylor terms of a spectral model for each source. (It's fine
+  Taylor terms of a spectral model for each source.(It's fine
   to have just one model, and this will do what you want.) The
   reference frequency for the Taylor expansion is taken from
   the first image.
 
 complist=
   Path to a CASA ComponentList Measurement Set to use in the modeling.
   I don't know what happens if you specify both this and "model".
@@ -1265,16 +1484,18 @@
   in a MS to enable later on-the-fly computation of the UV model.
 
 usescratch=
   Foo.
 """ + stdsel_doc + loglevel_doc
 
 
-class FtConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class FtConfig(ParseKeywords):
+    __doc__ = makecfgdoc('ft', ft_doc)
+
+    vis = Custom(str, required=True)
     model = [str]
     complist = str
     incremental = False
     wprojplanes = int
     usescratch = False
 
     antenna = str
@@ -1285,41 +1506,41 @@
     taql = str
     timerange = str
     uvrange = str
 
     loglevel = 'warn'
 
 
-def ft (cfg):
-    im = util.tools.imager ()
+def ft(cfg):
+    im = util.tools.imager()
 
-    im.open (b(cfg.vis), usescratch=cfg.usescratch)
-    im.selectvis (**b(extractmsselect (cfg, haveintent=False,
-                                       taqltomsselect=False)))
-    nmodel = len (cfg.model)
+    im.open(b(cfg.vis), usescratch=cfg.usescratch)
+    im.selectvis(**extractmsselect(cfg, haveintent=False,
+                                   taqltomsselect=False))
+    nmodel = len(cfg.model)
 
     if nmodel > 1:
-        ia = util.tools.image ()
-        ia.open (b(cfg.model[0]))
+        ia = util.tools.image()
+        ia.open(b(cfg.model[0]))
         # This gives Hz:
-        reffreq = ia.coordsys ().referencevalue (type=b'spectral')['numeric'][0]
-        ia.close ()
-        im.settaylorterms (ntaylorterms=nmodel, reffreq=reffreq)
+        reffreq = ia.coordsys().referencevalue(type=b'spectral')['numeric'][0]
+        ia.close()
+        im.settaylorterms(ntaylorterms=nmodel, reffreq=reffreq)
 
     if cfg.wprojplanes is not None:
-        im.defineimage ()
-        im.setoptions (ftmachine=b'wproject', wprojplanes=cfg.wprojplanes)
+        im.defineimage()
+        im.setoptions(ftmachine=b'wproject', wprojplanes=cfg.wprojplanes)
 
-    im.ft (model=b(cfg.model),
+    im.ft(model=b(cfg.model),
            complist=b(cfg.complist or ''),
            incremental=cfg.incremental)
-    im.close ()
+    im.close()
 
 
-ft_cli = makekwcli (ft_doc, FtConfig, ft)
+ft_cli = makekwcli(ft_doc, FtConfig, ft)
 
 
 # gaincal
 #
 # I've folded in the bandpass functionality since there's
 # so much overlap. Some limitations that this leads to:
 #
@@ -1337,15 +1558,15 @@
   Input dataset
 
 caltable=
   Output calibration table (can exist if append=True)
 
 gaintype=
   Kind of gain solution:
-    G       - gains per poln and spw (default)
+    G       - gains per poln and spw(default)
     T       - like G, but one value for all polns
     GSPLINE - like G, with a spline fit. "Experimental"
     B       - bandpass
     BPOLY   - bandpass with polynomial fit. "Somewhat experimental"
     K       - antenna-based delays
     KCROSS  - global cross-hand delay ; use parang=True
     D       - solve for instrumental leakage
@@ -1356,44 +1577,43 @@
     Xf      - above with per-channel phase terms
     D+X     - D and X. "Not normally done"
     Df+X    - Df and X. Presumably also not normally done.
     XY+QU   - ?
     XYf+QU  - ?
 
 calmode=
-  What parameters to solve for: amplitude ("a"), phase ("p"), or both
+  What parameters to solve for: amplitude("a"), phase("p"), or both
   ("ap"). Default is "ap". Not used in bandpass solutions.
 
 solint=
   Solution interval; this is an upper bound, but solutions
   will be broken across certain boundaries according to "combine".
-  'inf'    - solutions as long as possible (the default)
+  'inf'    - solutions as long as possible(the default)
   'int'    - one solution per integration
-  (str)    - a specific time with units (e.g. '5min')
+  (str)    - a specific time with units(e.g. '5min')
   (number) - a specific time in seconds
 
 combine=
-  Comma-separated list of boundary types; solutions will NOT be
-  broken across these boundaries. Types are:
-    field scan spw
+  Comma-separated list of boundary types; solutions will NOT be broken across
+  these boundaries. Types are: ``field``, ``scan``, ``spw``.
 
 refant=
   Comma-separated list of reference antennas in decreasing
   priority order.
 
 solnorm=
   Normalize solution amplitudes to 1 after solving (only applies
   to gaintypes G, T, B). Also normalizes bandpass phases to zero
   when solving for bandpasses. Default: false.
 
 append=
   Whether to append solutions to an existing table. If the table
   exists and append=False, the table is overwritten! (Default: false)
 """ + precal_doc + """
-*** Low-level parameters:
+**Low-level parameters**
 
 minblperant=
   Number of baselines for each ant in order to solve (default: 4)
 
 minsnr=
   Min. SNR for acceptable solutions (default: 3.0)
 
@@ -1402,40 +1622,42 @@
   in seconds. Default is -1, meaning not to pre-average.
 
 smodel=I,Q,U,V
   Full-stokes point source model to use, if none is embedded in the vis file.
 """ + stdsel_doc + loglevel_doc
 
 
-class GaincalConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    caltable = Custom (str, required=True)
+class GaincalConfig(ParseKeywords):
+    __doc__ = makecfgdoc('gaincal', gaincal_doc)
+
+    vis = Custom(str, required=True)
+    caltable = Custom(str, required=True)
     gaintype = 'G'
     calmode = 'ap'
 
     solint = 'inf'
     combine = [str]
     refant = [str]
     solnorm = False
     append = False
     minblperant = 4
     minsnr = 3.0
     preavg = -1.0
 
     gaintable = [str]
-    gainfield = Custom ([str], sep=';')
+    gainfield = Custom([str], sep=';')
     interp = [str]
     opacity = [float]
     gaincurve = False
     parang = False
     smodel = [int]
 
-    @Custom ([str], sep=';')
-    def spwmap (v):
-        return [map (int, e.split (',')) for e in v]
+    @Custom([str], sep=';')
+    def spwmap(v):
+        return [list(map(int, e.split(','))) for e in v]
 
     # gaincal keywords: splinetime npointaver phasewrap
     # bandpass keywords: fillgaps degamp degphase visnorm maskcenter
     #   maskedge
 
     antenna = str
     field = str
@@ -1446,64 +1668,64 @@
     taql = str # msselect
     timerange = str
     uvrange = str
 
     loglevel = 'warn' # teeny hack for CLI
 
 
-def gaincal (cfg):
-    cb = util.tools.calibrater ()
-    cb.open (filename=b(cfg.vis), compress=False, addcorr=False, addmodel=False)
+def gaincal(cfg):
+    cb = util.tools.calibrater()
+    cb.open(filename=b(cfg.vis), compress=False, addcorr=False, addmodel=False)
 
-    selkws = extractmsselect (cfg)
+    selkws = extractmsselect(cfg)
     selkws['chanmode'] = 'none' # ?
-    cb.selectvis (**b(selkws))
+    cb.selectvis(**selkws)
 
-    applyonthefly (cb, cfg)
+    applyonthefly(cb, cfg)
 
-    if cfg.smodel is not None and len (cfg.smodel):
-        cb.setptmodel (cfg.smodel)
+    if cfg.smodel is not None and len(cfg.smodel):
+        cb.setptmodel(cfg.smodel)
 
     # Solve
 
     solkws = {}
 
-    for k in 'append preavg minblperant minsnr solnorm'.split ():
-        solkws[k] = getattr (cfg, k)
+    for k in 'append preavg minblperant minsnr solnorm'.split():
+        solkws[k] = getattr(cfg, k)
 
-    for p in 'caltable:table calmode:apmode'.split ():
-        ck, sk = p.split (':')
-        solkws[sk] = getattr (cfg, ck)
+    for p in 'caltable:table calmode:apmode'.split():
+        ck, sk = p.split(':')
+        solkws[sk] = getattr(cfg, ck)
 
-    if isinstance (cfg.solint, (int, float)):
+    if isinstance(cfg.solint,(int, float)):
         solkws['t'] = '%fs' % cfg.solint # sugar
     else:
-        solkws['t'] = str (cfg.solint)
+        solkws['t'] = str(cfg.solint)
 
-    if isinstance (cfg.refant, six.string_types):
+    if isinstance(cfg.refant, six.string_types):
         solkws['refant'] = cfg.refant
     else:
-        solkws['refant'] = ','.join (cfg.refant)
+        solkws['refant'] = ','.join(cfg.refant)
 
-    solkws['combine'] = ','.join (cfg.combine)
+    solkws['combine'] = ','.join(cfg.combine)
     solkws['phaseonly'] = False
-    solkws['type'] = cfg.gaintype.upper ()
+    solkws['type'] = cfg.gaintype.upper()
 
     if solkws['type'] == 'GSPLINE':
-        cb.setsolvegainspline (**b(solkws))
+        cb.setsolvegainspline(**solkws)
     elif solkws['type'] == 'BPOLY':
-        cb.setsolvebandpoly (**b(solkws))
+        cb.setsolvebandpoly(**solkws)
     else:
-        cb.setsolve (**b(solkws))
+        cb.setsolve(**solkws)
 
-    cb.solve ()
-    cb.close ()
+    cb.solve()
+    cb.close()
 
 
-gaincal_cli = makekwcli (gaincal_doc, GaincalConfig, gaincal)
+gaincal_cli = makekwcli(gaincal_doc, GaincalConfig, gaincal)
 
 
 # gencal
 
 gencal_doc = \
 """
 casatask gencal vis=<MS> caltable=<TBL> caltype=<TYPE> [keywords...]
@@ -1530,83 +1752,90 @@
   amp       - generic amplitude correction; needs parameter(s)
   ph        - generic phase correction; needs parameter(s)
   sbd       - single-band delay: phase slope for each SPW; needs parameter(s)
   mbd       - multi-band delay: phase slope for all SPWs; needs parameter(s)
   antpos    - antenna position corrections in ITRF; what you want; accepts parameter(s)
   antposvla - antenna position corrections in VLA frame; **not what you want**; accepts parameter(s)
   tsys      - tsys from ALMA syscal table
-  swpow     - EVLA switched-power and requantizer gains ("experimental")
+  swpow     - EVLA switched-power and requantizer gains("experimental")
   opac      - tropospheric opacity; needs parameter
   gc        - (E)VLA elevation-dependent gain curve
   eff       - (E)VLA antenna efficiency correction
   gceff     - combination of "gc" and "eff"
   rq        - EVLA requantizer gains; not what you want
   swp/rq    - EVLA switched-power gains divided by "rq"; not what you want
 
 parameter=
   Custom parameters for various caltypes. Dimensionality depends on selections applied.
   amp       - gain; dimensionless
   ph        - phase; degrees
   sbd       - delay; nanosec
   mbd       - delay; nanosec
-  antpos    - position offsets; ITRF meters (or look up automatically for EVLA if unspecified)
+  antpos    - position offsets; ITRF meters(or look up automatically for EVLA if unspecified)
   antposvla - position offsets; meters in VLA reference frame
-  opac      - opacity; dimensionless (nepers?)
+  opac      - opacity; dimensionless(nepers?)
 
 antenna=
+  Selection keyword, governing which solutions to generate and controlling shape
+  of "parameter" keyword.
+
 pol=
+  Analogous to "antenna"
+
 spw=
-  Selection keywords governing which solutions to generate and controlling shape
-  of "parameter" keyword.
+  Analogous to "antenna"
 """ + loglevel_doc
 
 
-class GencalConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    caltable = Custom (str, required=True)
-    caltype = Custom (str, required=True)
+class GencalConfig(ParseKeywords):
+    __doc__ = makecfgdoc('gencal', gencal_doc)
+
+    vis = Custom(str, required=True)
+    caltable = Custom(str, required=True)
+    caltype = Custom(str, required=True)
     parameter = [float]
 
     antenna = str
     pol = str
     spw = str
 
     loglevel = 'warn'
 
 
-def gencal (cfg):
-    cb = util.tools.calibrater ()
-    cb.open (filename=b(cfg.vis), compress=False, addcorr=False, addmodel=False)
+def gencal(cfg):
+    cb = util.tools.calibrater()
+    cb.open(filename=b(cfg.vis), compress=False, addcorr=False, addmodel=False)
 
     antenna = cfg.antenna or ''
     parameter = cfg.parameter
 
     if cfg.caltype == 'antpos' and cfg.antenna is None:
         # There's a Python module in casapy that implements this; I don't want
         # to shadow it entirely ...
-        import cPickle as pickle
         from .scripting import CasapyScript
 
-        script = os.path.join (os.path.dirname (__file__), 'cscript_genantpos.py')
+        script = os.path.join(os.path.dirname(__file__), 'cscript_genantpos.py')
 
-        with CasapyScript (script, vis=cfg.vis) as cs:
+        with CasapyScript(script, vis=cfg.vis) as cs:
             try:
-                with open (os.path.join (cs.workdir, 'info.pkl'), 'rb') as f:
-                    antenna = pickle.load (f)
-                    parameter = pickle.load (f)
+                with open(os.path.join(cs.workdir, 'info.npy'), 'rb') as f:
+                    antenna = np.load(f)
+                    parameter = np.load(f)
             except Exception:
-                reraise_context ('interal casapy script seemingly failed; no info.pkl')
+                reraise_context('interal casapy script seemingly failed; no info.npy')
 
-    cb.specifycal (caltable=b(cfg.caltable), time=b'', spw=b(cfg.spw or ''),
-                   antenna=b(antenna), pol=b(cfg.pol or ''), caltype=b(cfg.caltype),
-                   parameter=b(parameter))
-    cb.close ()
+        antenna = antenna.tostring()
 
+    cb.specifycal(caltable=b(cfg.caltable), time=b'', spw=b(cfg.spw or ''),
+                  antenna=b(antenna), pol=b(cfg.pol or ''), caltype=b(cfg.caltype),
+                  parameter=b(parameter))
+    cb.close()
 
-gencal_cli = makekwcli (gencal_doc, GencalConfig, gencal)
+
+gencal_cli = makekwcli(gencal_doc, GencalConfig, gencal)
 
 
 # getopacities
 #
 # This is a casapy script.
 
 getopacities_doc = \
@@ -1619,152 +1848,153 @@
 VLA wideband setup, in which the data come in 16 spectral windows,
 
   casatask getopacities unglued.ms weather.png 8,8
 
 will print 2 values, averaged over 8 spectral windows each.
 """
 
-def getopacities (ms, plotdest):
-    import cPickle as pickle
+def getopacities(ms, plotdest):
     from .scripting import CasapyScript
 
-    script = os.path.join (os.path.dirname (__file__), 'cscript_getopacities.py')
+    script = os.path.join(os.path.dirname(__file__), 'cscript_getopacities.py')
 
-    with CasapyScript (script, ms=ms, plotdest=plotdest) as cs:
+    with CasapyScript(script, ms=ms, plotdest=plotdest) as cs:
         try:
-            with open (os.path.join (cs.workdir, 'opac.npy'), 'rb') as f:
-                opac = pickle.load (f)
+            with open(os.path.join(cs.workdir, 'opac.npy'), 'rb') as f:
+                opac = np.load(f)
         except Exception:
-            reraise_context ('interal casapy script seemingly failed; no opac.npy')
+            reraise_context('interal casapy script seemingly failed; no opac.npy')
 
     return opac
 
 
-def getopacities_cli (argv):
-    check_usage (getopacities_doc, argv, usageifnoargs=True)
+def getopacities_cli(argv):
+    check_usage(getopacities_doc, argv, usageifnoargs=True)
 
-    if len (argv) not in (3, 4):
-        wrong_usage (getopacities_doc, 'expected 2 or 3 arguments')
+    if len(argv) not in(3, 4):
+        wrong_usage(getopacities_doc, 'expected 2 or 3 arguments')
 
-    opac = getopacities (argv[1], argv[2])
+    opac = getopacities(argv[1], argv[2])
 
-    if len (argv) > 3:
-        spwwidths = [int (x) for x in argv[3].split (',')]
+    if len(argv) > 3:
+        spwwidths = [int(x) for x in argv[3].split(',')]
         averaged = []
         idx = 0
 
         for width in spwwidths:
-            averaged.append (opac[idx:idx+width].mean ())
+            averaged.append(opac[idx:idx+width].mean())
             idx += width
 
         opac = averaged
 
-    print ('opacity = [%s]' % (', '.join ('%.5f' % q for q in opac)))
+    print('opacity = [%s]' % (', '.join('%.5f' % q for q in opac)))
 
 
 # gpdetrend
 
 gpdetrend_doc = \
 """
 casatask gpdetrend caltable=
 
 Remove long-term phase trends from a complex-gain calibration table. For each
-antenna/spw/pol, the complex gains are divided into separate chunks (e.g., the
+antenna/spw/pol, the complex gains are divided into separate chunks(e.g., the
 intention is for one chunk for each visit to the complex-gain calibrator). The
 mean phase within each chunk is divided out. The effect is to remove long-term
 phase trends from the calibration table, but preserve short-term ones.
 
 caltable=MS
   The input calibration Measurement Set
 
 maxtimegap=int
   Measured in minutes. Gaps between solutions of this duration or longer will
   lead to a new segment being considered. Default is four times the smallest
   time gap seen in the data set.
 """ + loglevel_doc
 
 
-class GpdetrendConfig (ParseKeywords):
-    caltable = Custom (str, required=True)
+class GpdetrendConfig(ParseKeywords):
+    __doc__ = makecfgdoc('gpdetrend', gpdetrend_doc)
+
+    caltable = Custom(str, required=True)
     maxtimegap = int
     loglevel = 'warn'
 
 
-def gpdetrend (cfg):
+def gpdetrend(cfg):
     from ... import numutil
 
-    tb = util.tools.table ()
+    tb = util.tools.table()
 
-    tb.open (binary_type (cfg.caltable), nomodify=False)
-    #fields = tb.getcol (b'FIELD_ID')
-    spws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    ants = tb.getcol (b'ANTENNA1')
-    vals = tb.getcol (b'CPARAM')
-    flags = tb.getcol (b'FLAG')
-    times = tb.getcol (b'TIME')
+    tb.open(cfg.caltable, nomodify=False)
+    #fields = tb.getcol(b'FIELD_ID')
+    spws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    ants = tb.getcol(b'ANTENNA1')
+    vals = tb.getcol(b'CPARAM')
+    flags = tb.getcol(b'FLAG')
+    times = tb.getcol(b'TIME')
 
     npol, unused, nsoln = vals.shape
     assert unused == 1, 'unexpected gain table structure!'
     vals = vals[:,0,:]
     flags = flags[:,0,:]
 
     # see what we've got
 
-    def seen_values (data):
-        return [idx for idx, count in enumerate (np.bincount (data)) if count]
+    def seen_values(data):
+        return [idx for idx, count in enumerate(np.bincount(data)) if count]
 
-    any_ok = ~(np.all (flags, axis=0)) # mask for solns where at least one pol is unflagged
-    #seenfields = seen_values (fields[any_ok])
-    seenspws = seen_values (spws[any_ok])
-    seenants = seen_values (ants[any_ok])
+    any_ok = ~(np.all(flags, axis=0)) # mask for solns where at least one pol is unflagged
+    #seenfields = seen_values(fields[any_ok])
+    seenspws = seen_values(spws[any_ok])
+    seenants = seen_values(ants[any_ok])
 
     # time gap?
 
     if cfg.maxtimegap is not None:
         maxtimegap = cfg.maxtimegap * 60 # min => seconds
     else:
-        stimes = np.sort (times)
-        dt = np.diff (stimes)
+        stimes = np.sort(times)
+        dt = np.diff(stimes)
         dt = dt[dt > 0]
-        maxtimegap = 4 * dt.min ()
+        maxtimegap = 4 * dt.min()
 
     # Remove average phase of each chunk
 
     for iant in seenants:
-        for ipol in range (npol):
+        for ipol in range(npol):
             filter = (ants == iant) & ~flags[ipol]
 
             for ispw in seenspws:
                 # XXX: do something by field?
-                sfilter = filter & (spws == ispw)
+                sfilter = filter &(spws == ispw)
                 t = times[sfilter]
                 if not t.size:
                     continue
 
-                for s in numutil.slice_around_gaps (t, maxtimegap):
-                    w = np.where (sfilter)[0][s]
-                    meanph = np.angle (vals[ipol,w].mean ())
-                    vals[ipol,w] *= np.exp (-1j * meanph)
+                for s in numutil.slice_around_gaps(t, maxtimegap):
+                    w = np.where(sfilter)[0][s]
+                    meanph = np.angle(vals[ipol,w].mean())
+                    vals[ipol,w] *= np.exp(-1j * meanph)
 
     # Rewrite and we're done.
 
-    tb.putcol (b'CPARAM', vals.reshape ((npol, 1, nsoln)))
-    tb.close ()
+    tb.putcol(b'CPARAM', vals.reshape((npol, 1, nsoln)))
+    tb.close()
 
 
-gpdetrend_cli = makekwcli (gpdetrend_doc, GpdetrendConfig, gpdetrend)
+gpdetrend_cli = makekwcli(gpdetrend_doc, GpdetrendConfig, gpdetrend)
 
 
 # gpdiagnostics
 #
 # Shim for a separate module
 
-def gpdiagnostics_cli (argv):
+def gpdiagnostics_cli(argv):
     from .gpdiagnostics import gpdiagnostics_cli
-    gpdiagnostics_cli (argv)
+    gpdiagnostics_cli(argv)
 
 
 # gpplot
 #
 # See bpplot() -- CASA plotcal can do this in a certain sense, but it's slow
 # and ugly.
 
@@ -1784,15 +2014,15 @@
 dest=PATH
   If specified, plots are saved to this file -- the format is inferred
   from the extension, which must allow multiple pages to be saved. If
   unspecified, the plots are displayed using a Gtk3 backend.
 
 dims=WIDTH,HEIGHT
   If saving to a file, the dimensions of a each page. These are in points
-  for vector formats (PDF, PS) and pixels for bitmaps (PNG). Defaults to
+  for vector formats(PDF, PS) and pixels for bitmaps(PNG). Defaults to
   1000, 600.
 
 margins=TOP,RIGHT,LEFT,BOTTOM
   If saving to a file, the plot margins in the same units as the dims.
   The default is 4 on every side.
 
 maxtimegap=10
@@ -1804,134 +2034,136 @@
   ignored.
 
 phaseonly=false
   If True, plot only phases, and not amplitudes.
 """ + loglevel_doc
 
 
-class GpplotConfig (ParseKeywords):
-    caltable = Custom (str, required=True)
+class GpplotConfig(ParseKeywords):
+    __doc__ = makecfgdoc('gpplot', gpplot_doc)
+
+    caltable = Custom(str, required=True)
     dest = str
     dims = [1000, 600]
     margins = [4, 4, 4, 4]
     maxtimegap = 10. # minutes
     mjdrange = [float]
     phaseonly = False
     loglevel = 'warn'
 
 
-def gpplot (cfg):
+def gpplot(cfg):
     import omega as om, omega.render
     from ... import numutil
 
-    if len (cfg.mjdrange) not in (0, 2):
-        raise Exception ('"mjdrange" parameter must provide exactly 0 or 2 numbers')
+    if len(cfg.mjdrange) not in(0, 2):
+        raise Exception('"mjdrange" parameter must provide exactly 0 or 2 numbers')
 
-    if isinstance (cfg.dest, omega.render.Pager):
+    if isinstance(cfg.dest, omega.render.Pager):
         # This is for non-CLI invocation.
         pager = cfg.dest
     elif cfg.dest is None:
         import omega.gtk3
-        pager = om.makeDisplayPager ()
+        pager = om.makeDisplayPager()
     else:
-        pager = om.makePager (cfg.dest,
+        pager = om.makePager(cfg.dest,
                               dims=cfg.dims,
                               margins=cfg.margins,
-                              style=om.styles.ColorOnWhiteVector ())
+                              style=om.styles.ColorOnWhiteVector())
 
-    tb = util.tools.table ()
+    tb = util.tools.table()
 
-    tb.open (binary_type (cfg.caltable), nomodify=True)
-    fields = tb.getcol (b'FIELD_ID')
-    spws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    ants = tb.getcol (b'ANTENNA1')
-    vals = tb.getcol (b'CPARAM')
-    flags = tb.getcol (b'FLAG')
-    times = tb.getcol (b'TIME')
-    tb.close ()
-
-    tb.open (binary_type (os.path.join (cfg.caltable, 'ANTENNA')), nomodify=True)
-    names = tb.getcol (b'NAME')
-    tb.close ()
+    tb.open(cfg.caltable, nomodify=True)
+    fields = tb.getcol(b'FIELD_ID')
+    spws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    ants = tb.getcol(b'ANTENNA1')
+    vals = tb.getcol(b'CPARAM')
+    flags = tb.getcol(b'FLAG')
+    times = tb.getcol(b'TIME')
+    tb.close()
+
+    tb.open(os.path.join(cfg.caltable, 'ANTENNA'), nomodify=True)
+    names = tb.getcol(b'NAME')
+    tb.close()
 
     npol, unused, nsoln = vals.shape
     assert unused == 1, 'unexpected gain table structure!'
     vals = vals[:,0,:]
     flags = flags[:,0,:]
 
     # Apply date filter by futzing with flags
 
     times /= 86400. # convert to MJD
 
-    if len (cfg.mjdrange):
-        flags |= (times < cfg.mjdrange[0]) | (times > cfg.mjdrange[1])
+    if len(cfg.mjdrange):
+        flags |= (times < cfg.mjdrange[0]) |(times > cfg.mjdrange[1])
 
     # see what we've got
 
-    def seen_values (data):
-        return [idx for idx, count in enumerate (np.bincount (data)) if count]
+    def seen_values(data):
+        return [idx for idx, count in enumerate(np.bincount(data)) if count]
 
-    any_ok = ~(np.all (flags, axis=0)) # mask for solns where at least one pol is unflagged
-    seenfields = seen_values (fields[any_ok])
-    seenspws = seen_values (spws[any_ok])
-    seenants = seen_values (ants[any_ok])
-
-    field_offsets = dict ((fieldid, idx) for idx, fieldid in enumerate (seenfields))
-    spw_offsets = dict ((spwid, idx) for idx, spwid in enumerate (seenspws))
-    ant_offsets = dict ((antid, idx) for idx, antid in enumerate (seenants))
+    any_ok = ~(np.all(flags, axis=0)) # mask for solns where at least one pol is unflagged
+    seenfields = seen_values(fields[any_ok])
+    seenspws = seen_values(spws[any_ok])
+    seenants = seen_values(ants[any_ok])
+
+    field_offsets = dict((fieldid, idx) for idx, fieldid in enumerate(seenfields))
+    spw_offsets = dict((spwid, idx) for idx, spwid in enumerate(seenspws))
+    ant_offsets = dict((antid, idx) for idx, antid in enumerate(seenants))
 
     # normalize phases to avoid distracting wraps
 
-    mean_amps = np.ones ((len (seenants), npol, len (seenspws)))
+    mean_amps = np.ones((len(seenants), npol, len(seenspws)))
 
     for iant in seenants:
-        for ipol in range (npol):
+        for ipol in range(npol):
             filter = (ants == iant) & ~flags[ipol]
 
             for ispw in seenspws:
-                sfilter = filter & (spws == ispw)
-                if not sfilter.any ():
+                sfilter = filter &(spws == ispw)
+                if not sfilter.any():
                     continue
 
-                meanph = np.angle (vals[ipol,sfilter].mean ())
-                vals[ipol,sfilter] *= np.exp (-1j * meanph)
-                meanam = np.abs (vals[ipol,sfilter]).mean ()
+                meanph = np.angle(vals[ipol,sfilter].mean())
+                vals[ipol,sfilter] *= np.exp(-1j * meanph)
+                meanam = np.abs(vals[ipol,sfilter]).mean()
                 mean_amps[ant_offsets[iant],ipol,spw_offsets[ispw]] = meanam
 
     # find plot limits
 
-    min_time = times[any_ok].min ()
-    max_time = times[any_ok].max ()
-    mjdref = int (np.floor (min_time))
+    min_time = times[any_ok].min()
+    max_time = times[any_ok].max()
+    mjdref = int(np.floor(min_time))
     times -= mjdref # convert to delta-MJD
     min_time = (min_time - mjdref)
     max_time = (max_time - mjdref)
     span = max_time - min_time
     if span <= 0:
         if max_time == 0:
             span = 1.
         else:
             span = 0.05 * max_time
     max_time += 0.05 * span
     min_time -= 0.05 * span
 
-    okvals = vals[np.where (~flags)]
-    max_am = np.abs (okvals).max ()
-    min_am = np.abs (okvals).min ()
+    okvals = vals[np.where(~flags)]
+    max_am = np.abs(okvals).max()
+    min_am = np.abs(okvals).min()
     span = max_am - min_am
     if span <= 0:
         if max_am == 0:
             span = 1.
         else:
             span = 0.05 * max_am
     max_am += 0.05 * span
     min_am -= 0.05 * span
 
-    max_ph = np.angle (okvals, deg=True).max ()
-    min_ph = np.angle (okvals, deg=True).min ()
+    max_ph = np.angle(okvals, deg=True).max()
+    min_ph = np.angle(okvals, deg=True).min()
     span = max_ph - min_ph
     if span <= 0:
         if max_ph == 0:
             span = 1.
         else:
             span = 0.05 * max_ph
     max_ph += 0.05 * span
@@ -1941,112 +2173,141 @@
     if min_ph < -160:
         min_ph = -180
 
     polnames = 'RL' # XXX: identification doesn't seem to be stored in cal table
     maxtimegap = cfg.maxtimegap / 1440 # => units of days
 
     for iant in seenants:
-        for ipol in range (npol):
+        for ipol in range(npol):
             filter = (ants == iant) & ~flags[ipol]
-            p_am = om.RectPlot ()
-            p_ph = om.RectPlot ()
+            p_am = om.RectPlot()
+            p_ph = om.RectPlot()
             anyseen = False
 
             for ispw in seenspws:
                 # XXX: do something by field
-                sfilter = filter & (spws == ispw)
+                sfilter = filter &(spws == ispw)
                 t = times[sfilter]
                 if not t.size:
                     continue
 
                 v = vals[ipol,sfilter]
-                a = np.abs (v)
-                p = np.angle (v, deg=True)
+                a = np.abs(v)
+                p = np.angle(v, deg=True)
                 kt = '%s %s spw#%d' % (names[iant], polnames[ipol], ispw)
 
-                for s in numutil.slice_around_gaps (t, maxtimegap):
+                for s in numutil.slice_around_gaps(t, maxtimegap):
                     tsub, asub, psub = t[s], a[s], p[s]
                     if tsub.size == 0:
                         continue # Should never happen, but eh.
                     else:
                         lines = (tsub.size > 1)
 
                     if cfg.phaseonly:
-                        p_ph.addXY (tsub, psub, kt, lines=lines, dsn=spw_offsets[ispw])
+                        p_ph.addXY(tsub, psub, kt, lines=lines, dsn=spw_offsets[ispw])
                     else:
-                        p_am.addXY (tsub, asub, kt, lines=lines, dsn=spw_offsets[ispw])
-                        p_ph.addXY (tsub, psub, None, lines=lines, dsn=spw_offsets[ispw])
+                        p_am.addXY(tsub, asub, kt, lines=lines, dsn=spw_offsets[ispw])
+                        p_ph.addXY(tsub, psub, None, lines=lines, dsn=spw_offsets[ispw])
                     anyseen = True
 
                     if kt is not None: # hack for per-spw "anyseen"-type checking
-                        p_am.addHLine (mean_amps[ant_offsets[iant],ipol,spw_offsets[ispw]], None,
+                        p_am.addHLine(mean_amps[ant_offsets[iant],ipol,spw_offsets[ispw]], None,
                                        zheight=-1, lineStyle={'color': 'faint'})
                     kt = None
 
             if not anyseen:
                 continue
 
-            p_ph.addHLine (0, None, zheight=-1, lineStyle={'color': 'faint'})
+            p_ph.addHLine(0, None, zheight=-1, lineStyle={'color': 'faint'})
 
-            p_am.setBounds (xmin=min_time,
+            p_am.setBounds(xmin=min_time,
                             xmax=max_time,
                             ymin=min_am,
                             ymax=max_am)
-            p_ph.setBounds (xmin=min_time,
+            p_ph.setBounds(xmin=min_time,
                             xmax=max_time,
                             ymin=min_ph,
                             ymax=max_ph)
 
             p_am.bpainter.paintLabels = False
-            p_am.setYLabel ('Amplitude')
-            p_ph.setLabels ('Time (MJD - %d)' % mjdref, 'De-meaned Phase (deg)')
+            p_am.setYLabel('Amplitude')
+            p_ph.setLabels('Time(MJD - %d)' % mjdref, 'De-meaned Phase(deg)')
 
             if cfg.phaseonly:
-                pager.send (p_ph)
+                pager.send(p_ph)
             else:
-                vb = om.layout.VBox (2)
+                vb = om.layout.VBox(2)
                 vb[0] = p_am
                 vb[1] = p_ph
-                vb.setWeight (0, 2.5)
-                pager.send (vb)
+                vb.setWeight(0, 2.5)
+                pager.send(vb)
 
-gpplot_cli = makekwcli (gpplot_doc, GpplotConfig, gpplot)
+gpplot_cli = makekwcli(gpplot_doc, GpplotConfig, gpplot)
 
 
 # image2fits
 #
 # This is basically the "exportfits" task with fewer options and a slightly
 # clearer name.
 
 image2fits_doc = \
 """
 casatask image2fits <input MS image> <output FITS image>
 
 Convert an image in MS format to FITS format.
 """
 
-def image2fits (mspath, fitspath, velocity=False, optical=False, bitpix=-32,
+def image2fits(mspath, fitspath, velocity=False, optical=False, bitpix=-32,
                 minpix=0, maxpix=-1, overwrite=False, dropstokes=False, stokeslast=True,
                 history=True, **kwargs):
-    ia = util.tools.image ()
-    ia.open (b(mspath))
-    ia.tofits (outfile=b(fitspath), velocity=velocity, optical=optical, bitpix=bitpix,
+    """Convert an image in MS format to FITS format.
+
+    mspath (str)
+      The path to the input MS.
+    fitspath (str)
+      The path to the output FITS file.
+    velocity (boolean)
+      (To be documented.)
+    optical (boolean)
+      (To be documented.)
+    bitpix (integer)
+      (To be documented.)
+    minpix (integer)
+      (To be documented.)
+    maxpix (integer)
+      (To be documented.)
+    overwrite (boolean)
+      Whether the task is allowed to overwrite an existing destination file.
+    dropstokes (boolean)
+      Whether the "Stokes" (polarization) axis of the image should be dropped.
+    stokeslast (boolean)
+      Whether the "Stokes" (polarization) axis of the image should be placed as the last
+      (innermost?) axis of the image cube.
+    history (boolean)
+      (To be documented.)
+    ``**kwargs``
+      Forwarded on to the ``tofits`` function of the CASA ``image`` tool.
+
+    """
+    ia = util.tools.image()
+    ia.open(b(mspath))
+    ia.tofits(outfile=b(fitspath), velocity=velocity, optical=optical, bitpix=bitpix,
                minpix=minpix, maxpix=maxpix, overwrite=overwrite, dropstokes=dropstokes,
                stokeslast=stokeslast, history=history, **kwargs)
-    ia.close ()
+    ia.close()
 
 
-def image2fits_cli (argv):
-    check_usage (image2fits_doc, argv, usageifnoargs=True)
-    util.logger ()
+def image2fits_cli(argv):
+    check_usage(image2fits_doc, argv, usageifnoargs=True)
+    util.logger()
 
-    if len (argv) != 3:
-        wrong_usage (image2fits_doc, 'expected exactly 2 arguments')
+    if len(argv) != 3:
+        wrong_usage(image2fits_doc, 'expected exactly 2 arguments')
 
-    image2fits (argv[1], argv[2])
+    image2fits(argv[1], argv[2])
 
 
 # importalma
 #
 # This is a casapy script. We don't reeeallly need to be, but there's enough
 # logic in CASA's task_importasdm.py that I'm not thrilled to copy/paste it
 # all.
@@ -2055,29 +2316,45 @@
 """
 casatask importalma <ASDM> <MS>
 
 Convert an ALMA low-level ASDM dataset to Measurement Set format. This
 implementation automatically infers the value of the "tbuff" parameter.
 """
 
-def importalma (asdm, ms):
+def importalma(asdm, ms):
+    """Convert an ALMA low-level ASDM dataset to Measurement Set format.
+
+    asdm (str)
+      The path to the input ASDM dataset.
+    ms (str)
+      The path to the output MS dataset.
+
+    This implementation automatically infers the value of the "tbuff"
+    parameter.
+
+    Example::
+
+      from pwkit.environments.casa import tasks
+      tasks.importalma('myalma.asdm', 'myalma.ms')
+
+    """
     from .scripting import CasapyScript
 
-    script = os.path.join (os.path.dirname (__file__), 'cscript_importalma.py')
-    with CasapyScript (script, asdm=asdm, ms=ms) as cs:
+    script = os.path.join(os.path.dirname(__file__), 'cscript_importalma.py')
+    with CasapyScript(script, asdm=asdm, ms=ms) as cs:
         pass
 
 
-def importalma_cli (argv):
-    check_usage (importalma_doc, argv, usageifnoargs=True)
+def importalma_cli(argv):
+    check_usage(importalma_doc, argv, usageifnoargs=True)
 
-    if len (argv) != 3:
-        wrong_usage (importalma_doc, 'expected exactly 2 arguments')
+    if len(argv) != 3:
+        wrong_usage(importalma_doc, 'expected exactly 2 arguments')
 
-    importalma (argv[1], argv[2])
+    importalma(argv[1], argv[2])
 
 
 # importevla
 #
 # This is a casapy script. We don't reeeallly need to be, but there's enough
 # logic in CASA's task_importevla.py that I'm not thrilled to copy/paste it
 # all.
@@ -2086,166 +2363,214 @@
 """
 casatask importevla <ASDM> <MS>
 
 Convert an EVLA low-level ASDM dataset to Measurement Set format. This
 implementation automatically infers the value of the "tbuff" parameter.
 """
 
-def importevla (asdm, ms):
+def importevla(asdm, ms):
+    """Convert an EVLA low-level SDM dataset to Measurement Set format.
+
+    asdm (str)
+      The path to the input ASDM dataset.
+    ms (str)
+      The path to the output MS dataset.
+
+    This implementation automatically infers the value of the "tbuff"
+    parameter.
+
+    Example::
+
+      from pwkit.environments.casa import tasks
+      tasks.importevla('myvla.sdm', 'myvla.ms')
+
+    """
     from .scripting import CasapyScript
 
     # Here's the best way I can figure to find the recommended value of tbuff
-    # (= 1.5 * integration time). Obviously you might have different
+    #(= 1.5 * integration time). Obviously you might have different
     # integration times in the dataset and such, and we're just going to
     # ignore that possibility.
 
-    bdfstem = os.listdir (os.path.join (asdm, 'ASDMBinary'))[0]
-    bdf = os.path.join (asdm, 'ASDMBinary', bdfstem)
+    bdfstem = os.listdir(os.path.join(asdm, 'ASDMBinary'))[0]
+    bdf = os.path.join(asdm, 'ASDMBinary', bdfstem)
     tbuff = None
 
-    with open (bdf) as f:
-        for linenum, line in enumerate (f):
+    with open(bdf, 'rb') as f:
+        for linenum, line in enumerate(f):
             if linenum > 60:
-                raise PKError ('cannot find integration time info in %s', bdf)
+                raise PKError('cannot find integration time info in %s', bdf)
 
-            if not line.startswith ('<sdmDataSubsetHeader'):
+            if not line.startswith(b'<sdmDataSubsetHeader'):
                 continue
 
             try:
-                i1 = line.index ('<interval>') + len ('<interval>')
-                i2 = line.index ('</interval>')
+                i1 = line.index(b'<interval>') + len(b'<interval>')
+                i2 = line.index(b'</interval>')
                 if i2 <= i1:
-                    raise ValueError ()
+                    raise ValueError()
             except ValueError:
-                raise PKError ('cannot parse integration time info in %s', bdf)
+                raise PKError('cannot parse integration time info in %s', bdf)
 
-            tbuff = float (line[i1:i2]) * 1.5e-9 # nanosecs, and want 1.5x
+            tbuff = float(line[i1:i2]) * 1.5e-9 # nanosecs, and want 1.5x
             break
 
     if tbuff is None:
-        raise PKError ('found no integration time info')
+        raise PKError('found no integration time info')
 
-    print ('importevla: %s -> %s with tbuff=%.2f' % (asdm, ms, tbuff))
+    print('importevla: %s -> %s with tbuff=%.2f' % (asdm, ms, tbuff))
 
-    script = os.path.join (os.path.dirname (__file__), 'cscript_importevla.py')
-    with CasapyScript (script, asdm=asdm, ms=ms, tbuff=tbuff) as cs:
+    script = os.path.join(os.path.dirname(__file__), 'cscript_importevla.py')
+    with CasapyScript(script, asdm=asdm, ms=ms, tbuff=tbuff) as cs:
         pass
 
 
-def importevla_cli (argv):
-    check_usage (importevla_doc, argv, usageifnoargs=True)
+def importevla_cli(argv):
+    check_usage(importevla_doc, argv, usageifnoargs=True)
 
-    if len (argv) != 3:
-        wrong_usage (importevla_doc, 'expected exactly 2 arguments')
+    if len(argv) != 3:
+        wrong_usage(importevla_doc, 'expected exactly 2 arguments')
 
-    importevla (argv[1], argv[2])
+    importevla(argv[1], argv[2])
 
 
 # listobs
 #
 # This one is mostly about the CLI.
 
 listobs_doc = \
 """
 casatask listobs <MS>
 
 Generate a standard "listobs" listing of visibility MS contents. If
 standard output is a TTY, the listing will be paged.
 """
 
-def listobs (vis):
-    """Generates a set of lines of output. Errors are only detected by looking
-    at the output."""
+def listobs(vis):
+    """Textually describe the contents of a measurement set.
+
+    vis (str)
+      The path to the dataset.
+    Returns
+      A generator of lines of human-readable output
+
+    Errors can only be detected by looking at the output. Example::
+
+      from pwkit.environments.casa import tasks
 
-    def inner_list (sink):
+      for line in tasks.listobs('mydataset.ms'):
+        print(line)
+
+    """
+    def inner_list(sink):
         try:
-            ms = util.tools.ms ()
-            ms.open (vis)
-            ms.summary (verbose=True)
-            ms.close ()
+            ms = util.tools.ms()
+            ms.open(vis)
+            ms.summary(verbose=True)
+            ms.close()
         except Exception as e:
-            sink.post (b'listobs failed: %s' % e, priority=b'SEVERE')
+            sink.post(b'listobs failed: %s' % e, priority=b'SEVERE')
 
-    for line in util.forkandlog (inner_list):
-        info = line.rstrip ().split ('\t', 3) # date, priority, origin, message
-        if len (info) > 3:
+    for line in util.forkandlog(inner_list):
+        info = line.rstrip().split('\t', 3) # date, priority, origin, message
+        if len(info) > 3:
             yield info[3]
         else:
             yield ''
 
 
-def listobs_cli (argv):
-    check_usage (listobs_doc, argv, usageifnoargs=True)
+def listobs_cli(argv):
+    check_usage(listobs_doc, argv, usageifnoargs=True)
 
-    if len (argv) != 2:
-        wrong_usage (listobs_doc, 'expect exactly one argument, the MS path')
+    if len(argv) != 2:
+        wrong_usage(listobs_doc, 'expect exactly one argument, the MS path')
 
     vis = argv[1]
 
     proc = None
     out = sys.stdout
 
-    if sys.stdout.isatty () or \
-           (hasattr (sys.stdout, 'stream') and sys.stdout.stream.isatty ()):
+    if sys.stdout.isatty() or \
+          (hasattr(sys.stdout, 'stream') and sys.stdout.stream.isatty()):
         # Send our output to a pager!
         import subprocess
-        pager = os.environ.get ('PAGER') or 'less -SRFX'
+        pager = os.environ.get('PAGER') or 'less -SRFX'
         try:
-            proc = subprocess.Popen (pager, stdin=subprocess.PIPE, close_fds=True,
+            proc = subprocess.Popen(pager, stdin=subprocess.PIPE, close_fds=True,
                                      shell=True)
         except Exception as e:
-            warn ('couldn\'t start pager %r: %s', pager, e)
+            warn('couldn\'t start pager %r: %s', pager, e)
         else:
             out = proc.stdin
 
-    for line in listobs (vis):
-        print (line, file=out)
+            if not six.PY2:
+                import codecs
+                out = codecs.getwriter('utf8')(out)
+
+    for line in listobs(vis):
+        print(line, file=out)
 
     if proc is not None:
-        proc.stdin.close ()
-        proc.wait () # ignore return code
+        proc.stdin.close()
+        proc.wait() # ignore return code
 
 
 # listsdm
 #
 # This one is mostly about the CLI.
 
 listsdm_doc = \
 """
 casatask listsdm <MS>
 
-Generate a standard "listsdm" listing of (A)SDM dataset contents. If standard
+Generate a standard "listsdm" listing of(A)SDM dataset contents. If standard
 output is a TTY, the listing will be paged.
 
 The CASA "listsdm" functionality is implemented in pure Python, so unlike the
 "listobs" case, here we alter the standard format to be more to our liking.
 
 """
 
-def listsdm (sdm, file=None):
-    """This code based on CASA's `task_listsdm.py`, with this version info:
+def listsdm(sdm, file=None):
+    """Generate a standard "listsdm" listing of(A)SDM dataset contents.
 
-    # v1.0: 2010.12.07, M. Krauss
-    # v1.1: 2011.02.23, M. Krauss: added functionality for ALMA data
-    #
-    # Original code based on readscans.py, courtesy S. Meyers
+    sdm (str)
+      The path to the (A)SDM dataset to parse
+    file (stream-like object, such as an opened file)
+      Where to print the human-readable listing. If unspecified, results
+      go to :data:`sys.stdout`.
+    Returns
+      A dictionary of information about the dataset. Contents not yet
+      documented.
+
+    Example::
+
+      from pwkit.environments.casa import tasks
+      tasks.listsdm('myalmaa.asdm')
+
+    This code based on CASA's `task_listsdm.py`, with this version info::
+
+      # v1.0: 2010.12.07, M. Krauss
+      # v1.1: 2011.02.23, M. Krauss: added functionality for ALMA data
+      #
+      # Original code based on readscans.py, courtesy S. Meyers
 
     """
     from xml.dom import minidom
     import string
 
-    def printf (fmt, *args):
-        if len (args):
+    def printf(fmt, *args):
+        if len(args):
             s = fmt % args
         else:
-            s = str (fmt)
-        print (s, file=file)
+            s = str(fmt)
+        print(s, file=file)
 
-    qa = util.tools.quanta ()
-    me = util.tools.measures ()
+    qa = util.tools.quanta()
+    me = util.tools.measures()
 
     list_scans = True
     list_antennas = False
     list_fields = True
     list_spws = False
 
     # read Scan.xml
@@ -2330,15 +2655,15 @@
 
         # get the field ID
         rowfieldid = rownode.getElementsByTagName('fieldId')
         fieldid = string.split(str(rowfieldid[0].childNodes[0].nodeValue), '_')[1]
         fieldIdList.append(fieldid)
 
     # read ConfigDescription.xml to relate the configuration
-    # description to a (set) of data description IDs
+    # description to a(set) of data description IDs
     xmlconfig = minidom.parse(sdm+'/ConfigDescription.xml')
     rowlist = xmlconfig.getElementsByTagName('row')
     configDescList = []
     dataDescList = []
     for rownode in rowlist:
 
         # get the configuration description
@@ -2376,17 +2701,17 @@
         spwIdDataDesc = str(rowSpwIdDataDesc[0].childNodes[0].nodeValue)
         spwIdDataDescList.append(spwIdDataDesc)
 
     # read SpectralWindow.xml, get information about number of
     # channels, reference frequency, baseband name, channel width.
     # Interesting that there seem to be multiple fields that give the
     # same information: chanFreqStart=reFreq,
-    # chanFreqStep=chanWidth=resolution.  Why? (Note: all units are Hz)
+    # chanFreqStep=chanWidth=resolution.  Why?(Note: all units are Hz)
     # Note: this is where the script breaks for ALMA data, since there
-    # are different tags in SpectraWindow.xml (for varying channel widths).
+    # are different tags in SpectraWindow.xml(for varying channel widths).
     xmlSpecWin = minidom.parse(sdm+'/SpectralWindow.xml')
     rowlist = xmlSpecWin.getElementsByTagName('row')
     spwIdList = []
     nChanList = []
     refFreqList = []
     chanWidthList = []
     basebandList = []
@@ -2439,16 +2764,16 @@
         rowSrcId = rownode.getElementsByTagName('sourceId')
 
         # convert to values or strings and append to relevent lists:
         fieldList.append(int(string.split(str(rowField[0].childNodes[0].nodeValue),'_')[1]))
         fieldNameList.append(str(rowName[0].childNodes[0].nodeValue))
         fieldCodeList.append(str(rowCode[0].childNodes[0].nodeValue))
         coordInfo = rowCoords[0].childNodes[0].nodeValue.split()
-        RADeg = float(coordInfo[3])*(180.0/np.pi)
-        DecDeg = float(coordInfo[4])*(180.0/np.pi)
+        RADeg = float(coordInfo[3])* (180.0/np.pi)
+        DecDeg = float(coordInfo[4])* (180.0/np.pi)
         RAInp = {'unit': 'deg', 'value': RADeg}
         DecInp = {'unit': 'deg', 'value': DecDeg}
         RAHMS = b(qa.formxxx(b(RAInp), format=b'hms'))
         DecDMS = b(qa.formxxx(b(DecInp), format=b'dms'))
         fieldRAList.append(RAHMS)
         fieldDecList.append(DecDMS)
         fieldSrcIDList.append(int(rowSrcId[0].childNodes[0].nodeValue))
@@ -2573,126 +2898,126 @@
         scandict[scanNum]['spws'] = spwOrdList
         scandict[scanNum]['nchan'] = nChanOrdList
         scandict[scanNum]['reffreq'] = rFreqOrdList
         scandict[scanNum]['chanwidth'] = cWidthOrdList
         scandict[scanNum]['baseband'] = bbandOrdList
 
     # report information to the logger
-    printf ('================================================================================')
-    printf ('   SDM File: %s', sdm)
-    printf ('================================================================================')
-    printf ('   Observer: %s', observerName)
-    printf ('   Facility: %s, %s-configuration', telescopeName, configName)
-    printf ('      Observed from %s to %s (UTC)', obsStart, obsEnd)
-    printf ('      Total integration time = %.2f seconds (%.2f hours)', intTime, intTime / 3600)
+    printf('================================================================================')
+    printf('   SDM File: %s', sdm)
+    printf('================================================================================')
+    printf('   Observer: %s', observerName)
+    printf('   Facility: %s, %s-configuration', telescopeName, configName)
+    printf('      Observed from %s to %s(UTC)', obsStart, obsEnd)
+    printf('      Total integration time = %.2f seconds(%.2f hours)', intTime, intTime / 3600)
 
     if list_scans:
-        printf (' ')
-        printf ('Scan listing:')
+        printf(' ')
+        printf('Scan listing:')
 
         maxspwlen = 0
 
-        for scaninfo in scandict.itervalues ():
+        for scaninfo in scandict.values():
             SPWs = []
             for spw in scaninfo['spws']:
                 SPWs += spw
 
-            scaninfo['spwstr'] = str (list (set (SPWs)))
-            maxspwlen = max (maxspwlen, len (scaninfo['spwstr']))
+            scaninfo['spwstr'] = str(list(set(SPWs)))
+            maxspwlen = max(maxspwlen, len(scaninfo['spwstr']))
 
         fmt = '  %-25s  %-4s %-5s %-15s %-*s %s'
-        printf (fmt, 'Timerange (UTC)', 'Scan', 'FldID', 'FieldName', maxspwlen, 'SpwIDs', 'Intent(s)')
+        printf(fmt, 'Timerange(UTC)', 'Scan', 'FldID', 'FieldName', maxspwlen, 'SpwIDs', 'Intent(s)')
 
-        for i, (scanid, scaninfo) in enumerate (scandict.iteritems ()):
-            printf (fmt, startTimeShort[i] + ' - ' + endTimeShort[i], scanid,
+        for i,(scanid, scaninfo) in enumerate(scandict.items()):
+            printf(fmt, startTimeShort[i] + ' - ' + endTimeShort[i], scanid,
                     scaninfo['field'], scaninfo['source'], maxspwlen,
                     scaninfo['spwstr'], scaninfo['intent'])
 
     if list_spws:
-        printf (' ')
-        printf ('Spectral window information:')
-        printf ('  SpwID  #Chans  Ch0(MHz)  ChWidth(kHz) TotBW(MHz)  Baseband')
+        printf(' ')
+        printf('Spectral window information:')
+        printf('  SpwID  #Chans  Ch0(MHz)  ChWidth(kHz) TotBW(MHz)  Baseband')
 
         for i in range(0, len(spwIdList)):
-            printf (' %s %s %s %s %s %s', string.split(spwIdList[i],
+            printf(' %s %s %s %s %s %s', string.split(spwIdList[i],
                                                        '_')[1].ljust(4), str(nChanList[i]).ljust(4),
                     str(refFreqList[i]/1e6).ljust(8),
                     str(np.array(chanWidthList[i])/1e3).ljust(8),
                     str(np.array(chanWidthList[i])*nChanList[i]/1e6).ljust(8),
                     basebandList[i].ljust(8))
 
     if list_fields:
-        printf (' ')
-        printf ('Field information:')
-        printf ('  FldID  Code   Name            RA            Dec             SrcID')
+        printf(' ')
+        printf('Field information:')
+        printf('  FldID  Code   Name            RA            Dec             SrcID')
 
         for i in range(0, len(fieldList)):
-            printf ('  %-6d %-6s %-15s %-13s %-15s %-5d', fieldList[i], fieldCodeList[i],
+            printf('  %-6d %-6s %-15s %-13s %-15s %-5d', fieldList[i], fieldCodeList[i],
                     fieldNameList[i], fieldRAList[i], fieldDecList[i],
                     fieldSrcIDList[i])
 
     if list_antennas:
-        printf (' ')
-        printf ('Antennas (%i):' % len(antList))
-        printf ('  ID    Name   Station   Diam.(m)  Lat.          Long.')
+        printf(' ')
+        printf('Antennas(%i):' % len(antList))
+        printf('  ID    Name   Station   Diam.(m)  Lat.          Long.')
 
         for i in range(0, len(antList)):
-            printf (' %s %s %s %s %s %s ', str(antList[i]).ljust(5),
+            printf(' %s %s %s %s %s %s ', str(antList[i]).ljust(5),
                     antNameList[i].ljust(6), assocStatList[i].ljust(5),
                     str(dishDiamList[i]).ljust(5), statLatList[i].ljust(12),
                     statLonList[i].ljust(12))
 
     # return the scan dictionary
     return scandict
 
 
-def listsdm_cli (argv):
-    check_usage (listsdm_doc, argv, usageifnoargs=True)
+def listsdm_cli(argv):
+    check_usage(listsdm_doc, argv, usageifnoargs=True)
 
-    if len (argv) != 2:
-        wrong_usage (listsdm_doc, 'expect exactly one argument, the SDM path')
+    if len(argv) != 2:
+        wrong_usage(listsdm_doc, 'expect exactly one argument, the SDM path')
 
     sdm = argv[1]
 
     proc = None
     out = sys.stdout
 
-    if sys.stdout.isatty () or \
-           (hasattr (sys.stdout, 'stream') and sys.stdout.stream.isatty ()):
+    if sys.stdout.isatty() or \
+          (hasattr(sys.stdout, 'stream') and sys.stdout.stream.isatty()):
         # Send our output to a pager!
         import subprocess
-        pager = os.environ.get ('PAGER') or 'less -SRFX'
+        pager = os.environ.get('PAGER') or 'less -SRFX'
         try:
-            proc = subprocess.Popen (pager, stdin=subprocess.PIPE, close_fds=True,
+            proc = subprocess.Popen(pager, stdin=subprocess.PIPE, close_fds=True,
                                      shell=True)
         except Exception as e:
-            warn ('couldn\'t start pager %r: %s', pager, e)
+            warn('couldn\'t start pager %r: %s', pager, e)
         else:
             out = proc.stdin
 
-    listsdm (sdm, file=out)
+    listsdm(sdm, file=out)
 
     if proc is not None:
-        proc.stdin.close ()
-        proc.wait () # ignore return code
+        proc.stdin.close()
+        proc.wait() # ignore return code
 
 
 # mfsclean
 #
 # This isn't a CASA task, but we're pulling out a subset of the functionality
 # of clean, which has a bajillion options and has a really gross implementation
 # in the library.
 
 mfsclean_doc = \
 """
 casatask mfsclean vis=[] [keywords]
 
 Drive the CASA imager with a very restricted set of options.
 
-For W-projection, set ftmachine='wproject' and wprojplanes=64 (or so).
+For W-projection, set ftmachine='wproject' and wprojplanes=64(or so).
 
 vis=
   Input visibility MS
 
 imbase=
   Base name of output files. We create files named "imbaseEXT"
   where EXT is all of "mask", "modelTT", "imageTT", "residualTT",
@@ -2705,22 +3030,24 @@
 mask = (blank) or path of CASA-format region text file
 niter = 500
 nterms = 1
 phasecenter = (blank) or 'J2000 12h34m56.7 -12d34m56.7'
 reffreq = 0 [GHz]
 stokes = I
 threshold = 0 [mJy]
-weighting = 'briggs' (robust=0.5) or 'natural'
+weighting = 'briggs'(robust=0.5) or 'natural'
 wprojplanes = 1
 
-""" + stdsel_doc + loglevel_doc.replace ('warn;', 'info;')
+""" + stdsel_doc + loglevel_doc.replace('warn;', 'info;')
 
-class MfscleanConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    imbase = Custom (str, required=True)
+class MfscleanConfig(ParseKeywords):
+    __doc__ = makecfgdoc('mfsclean', mfsclean_doc)
+
+    vis = Custom(str, required=True)
+    imbase = Custom(str, required=True)
 
     cell = 1. # arcsec
     ftmachine = 'ft'
     gain = 0.1
     imsize = [256, 256]
     mask = str
     minpb = 0.2
@@ -2762,23 +3089,23 @@
     timerange = str
     uvrange = str
     taql = str
 
     loglevel = 'info'
 
 
-specframenames = 'REST LSRK LSRD BARY GEO TOPO GALACTO LGROUP CMB'.split ()
+specframenames = 'REST LSRK LSRD BARY GEO TOPO GALACTO LGROUP CMB'.split()
 
 
-def mfsclean (cfg):
-    ms = util.tools.ms ()
-    im = util.tools.imager ()
-    tb = util.tools.table ()
-    qa = util.tools.quanta ()
-    ia = util.tools.image ()
+def mfsclean(cfg):
+    ms = util.tools.ms()
+    im = util.tools.imager()
+    tb = util.tools.table()
+    qa = util.tools.quanta()
+    ia = util.tools.image()
 
     # Filenames. TODO: make sure nothing exists
 
     mask = cfg.imbase + 'mask'
     pb = cfg.imbase + 'flux'
 
     if cfg.nterms == 1:
@@ -2789,171 +3116,189 @@
     else:
         # Note: the names for the 'alpha' and 'alpha.error' images are
         # generated automatically inside the C++ stuff by looking for image
         # names ending in 'tt0', so we're limited in our naming flexibility
         # here.
         models, restoreds, resids, psfs = [], [], [], []
 
-        for i in range (cfg.nterms):
-            models.append (cfg.imbase + 'model.tt%d' % i)
-            restoreds.append (cfg.imbase + 'image.tt%d' % i)
-            resids.append (cfg.imbase + 'residual.tt%d' % i)
-            psfs.append (cfg.imbase + 'psf.tt%d' % i)
+        for i in range(cfg.nterms):
+            models.append(cfg.imbase + 'model.tt%d' % i)
+            restoreds.append(cfg.imbase + 'image.tt%d' % i)
+            resids.append(cfg.imbase + 'residual.tt%d' % i)
+            psfs.append(cfg.imbase + 'psf.tt%d' % i)
 
     # Get info on our selected data for various things we need to figure
     # out later.
 
-    selkws = extractmsselect (cfg, havearray=False, haveintent=False, taqltomsselect=False)
-    ms.open (b(cfg.vis))
-    ms.msselect (b(selkws))
-    rangeinfo = ms.range (b'data_desc_id field_id'.split ())
+    selkws = extractmsselect(cfg, havearray=False, haveintent=False, taqltomsselect=False)
+    ms.open(b(cfg.vis))
+    ms.msselect(b(selkws))
+    rangeinfo = ms.range(b'data_desc_id field_id'.split())
     ddids = rangeinfo['data_desc_id']
     fields = rangeinfo['field_id']
 
     # Get the spectral frame from the first spw of the selected data
 
-    tb.open (b(os.path.join (cfg.vis, 'DATA_DESCRIPTION')))
-    ddspws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    tb.close ()
+    tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
+    ddspws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    tb.close()
     spw0 = ddspws[ddids[0]]
 
-    tb.open (b(os.path.join (cfg.vis, 'SPECTRAL_WINDOW')))
-    specframe = specframenames[tb.getcell (b'MEAS_FREQ_REF', spw0)]
-    tb.close ()
+    tb.open(b(os.path.join(cfg.vis, 'SPECTRAL_WINDOW')))
+    specframe = specframenames[tb.getcell(b'MEAS_FREQ_REF', spw0)]
+    tb.close()
 
     # Choose phase center
 
     if cfg.phasecenter is None:
-        phasecenter = int (fields[0])
+        phasecenter = int(fields[0])
     else:
         phasecenter = cfg.phasecenter
 
         if ':' in phasecenter:
             # phasecenter='J2000 19:06:48.568 40:11:06.68'
             # parses to "07:06:48.57 297.13.19.80"
             # Using hm/dm instead of ::/:: as separators makes it parse
             # correctly. No idea how the colons manage to parse both
             # without warning and totally wrongly.
-            warn ('you moron, who uses colons in sexagesimal?')
-            tmp1 = phasecenter.split ()
+            warn('you moron, who uses colons in sexagesimal?')
+            tmp1 = phasecenter.split()
             twiddled = False
-            if len (tmp1) == 3:
-                tmp2 = tmp1[1].split (':')
-                tmp3 = tmp1[2].split (':')
-                if len (tmp2) == 3 and len (tmp3) == 3:
+            if len(tmp1) == 3:
+                tmp2 = tmp1[1].split(':')
+                tmp3 = tmp1[2].split(':')
+                if len(tmp2) == 3 and len(tmp3) == 3:
                     tmp2 = tmp2[0] + 'h' + tmp2[1] + 'm' + tmp2[2]
                     tmp3 = tmp3[0] + 'd' + tmp3[1] + 'm' + tmp3[2]
-                    phasecenter = ' '.join ([tmp1[0], tmp2, tmp3])
+                    phasecenter = ' '.join([tmp1[0], tmp2, tmp3])
                     twiddled = True
             if twiddled:
-                warn ('attempted to fix it up: "%s"\n\n', phasecenter)
+                warn('attempted to fix it up: "%s"\n\n', phasecenter)
             else:
-                warn ('couldn\'t parse, left as-is; good luck\n\n')
+                warn('couldn\'t parse, left as-is; good luck\n\n')
 
     # Set up all of this junk
 
-    im.open (b(cfg.vis), usescratch=False)
-    im.selectvis (nchan=-1, start=0, step=1, usescratch=False, writeaccess=False, **b(selkws))
-    im.defineimage (nx=cfg.imsize[0], ny=cfg.imsize[1],
-                    cellx=qa.quantity (b(cfg.cell), b'arcsec'),
-                    celly=qa.quantity (b(cfg.cell), b'arcsec'),
+    im.open(b(cfg.vis), usescratch=False)
+    im.selectvis(nchan=-1, start=0, step=1, usescratch=False, writeaccess=False, **selkws)
+    im.defineimage(nx=cfg.imsize[0], ny=cfg.imsize[1],
+                    cellx=qa.quantity(b(cfg.cell), b'arcsec'),
+                    celly=qa.quantity(b(cfg.cell), b'arcsec'),
                     outframe=b(specframe), phasecenter=b(phasecenter),
                     stokes=cfg.stokes,
-                    spw=-1, # to verify: selectvis (spw=) good enough?
+                    spw=-1, # to verify: selectvis(spw=) good enough?
                     restfreq=b'', mode=b'mfs', veltype=b'radio',
                     nchan=-1, start=0, step=1, facets=1)
 
     if cfg.weighting == 'briggs':
-        im.weight (type=b'briggs', rmode=b'norm', robust=0.5, npixels=0) #noise=, mosaic=
+        im.weight(type=b'briggs', rmode=b'norm', robust=0.5, npixels=0) #noise=, mosaic=
     elif cfg.weighting == 'natural':
-        im.weight (type=b'natural', rmode=b'none')
+        im.weight(type=b'natural', rmode=b'none')
     else:
-        raise ValueError ('unknown weighting type "%s"' % cfg.weighting)
+        raise ValueError('unknown weighting type "%s"' % cfg.weighting)
 
-    # im.filter (...)
-    im.setscales (scalemethod=b'uservector', uservector=[0])
-    im.setsmallscalebias (0.6)
-    im.setmfcontrol ()
-    im.setvp (dovp=True)
-    im.makeimage (type=b'pb', image=b(pb), compleximage=b'', verbose=False)
-    im.setvp (dovp=False, verbose=False)
-    im.setoptions (ftmachine=b(cfg.ftmachine), wprojplanes=b(cfg.wprojplanes),
+    # im.filter(...)
+    im.setscales(scalemethod=b'uservector', uservector=[0])
+    im.setsmallscalebias(0.6)
+    im.setmfcontrol()
+    im.setvp(dovp=True)
+    im.makeimage(type=b'pb', image=b(pb), compleximage=b'', verbose=False)
+    im.setvp(dovp=False, verbose=False)
+    im.setoptions(ftmachine=b(cfg.ftmachine), wprojplanes=b(cfg.wprojplanes),
                    freqinterp=b'linear', padding=1.2, pastep=360.0, pblimit=b(cfg.minpb),
                    applypointingoffsets=False, dopbgriddingcorrections=True)
 
     if cfg.nterms > 1:
-        im.settaylorterms (ntaylorterms=cfg.nterms, reffreq=cfg.reffreq * 1e9)
+        im.settaylorterms(ntaylorterms=cfg.nterms, reffreq=cfg.reffreq * 1e9)
 
-    im.setmfcontrol (stoplargenegatives=-1, cyclefactor=1.5,
+    im.setmfcontrol(stoplargenegatives=-1, cyclefactor=1.5,
                      cyclespeedup=-1, minpb=cfg.minpb)
 
     # Create the mask
 
     if cfg.mask is None:
         maskstr = ''
     else:
         maskstr = mask
-        im.make (b(mask))
-        ia.open (b(mask))
-        maskcs = ia.coordsys ()
-        maskcs.setreferencecode (b(specframe), b'spectral', True)
-        ia.setcoordsys (maskcs.torecord ())
+        im.make(b(mask))
+        ia.open(b(mask))
+        maskcs = ia.coordsys()
+        maskcs.setreferencecode(b(specframe), b'spectral', True)
+        ia.setcoordsys(maskcs.torecord())
 
         if cfg.mask is not None:
-            rg = util.tools.regionmanager ()
-            regions = rg.fromtextfile (filename=b(cfg.mask),
-                                       shape=ia.shape (),
-                                       csys=maskcs.torecord ())
-            im.regiontoimagemask (mask=b(mask), region=regions)
+            rg = util.tools.regionmanager()
+            regions = rg.fromtextfile(filename=b(cfg.mask),
+                                       shape=ia.shape(),
+                                       csys=maskcs.torecord())
+            im.regiontoimagemask(mask=b(mask), region=regions)
 
-        ia.close ()
+        ia.close()
 
     # Create blank model(s). Diverging from task_clean even more
     # significantly than usual here.
 
     for model in models:
-        im.make (b(model))
+        im.make(b(model))
 
     # Go!
 
-    im.clean (algorithm=b'msmfs', niter=cfg.niter, gain=cfg.gain,
-              threshold=qa.quantity (b(cfg.threshold), b'mJy'),
+    im.clean(algorithm=b'msmfs', niter=cfg.niter, gain=cfg.gain,
+              threshold=qa.quantity(b(cfg.threshold), b'mJy'),
               model=b(models), residual=b(resids), image=b(restoreds),
               psfimage=b(psfs), mask=b(maskstr), interactive=False)
-    im.close ()
+    im.close()
 
 
-mfsclean_cli = makekwcli (mfsclean_doc, MfscleanConfig, mfsclean)
+mfsclean_cli = makekwcli(mfsclean_doc, MfscleanConfig, mfsclean)
 
 
 # mjd2date
 
 mjd2date_doc = \
 """
 casatask mjd2date <date>
 
 Convert an MJD to a date in the format used by CASA.
 
 """
-def mjd2date (mjd, precision=3):
+def mjd2date(mjd, precision=3):
+    """Convert an MJD to a data string in the format used by CASA.
+
+    mjd (numeric)
+      An MJD value in the UTC timescale.
+    precision (integer, default 3)
+      The number of digits of decimal precision in the seconds portion of
+      the returned string
+    Returns
+      A string representing the input argument in CASA format:
+      ``YYYY/MM/DD/HH:MM:SS.SSS``.
+
+    Example::
+
+      from pwkit.environment.casa import tasks
+      print(tasks.mjd2date(55555))
+      # yields '2010/12/25/00:00:00.000'
+
+    """
     from astropy.time import Time
-    dt = Time (mjd, format='mjd', scale='utc').to_datetime ()
-    fracsec = ('%.*f' % (precision, 1e-6 * dt.microsecond)).split ('.')[1]
+    dt = Time(mjd, format='mjd', scale='utc').to_datetime()
+    fracsec = ('%.*f' % (precision, 1e-6 * dt.microsecond)).split('.')[1]
     return '%04d/%02d/%02d/%02d:%02d:%02d.%s' % (
         dt.year, dt.month, dt.day, dt.hour, dt.minute, dt.second, fracsec
     )
 
 
-def mjd2date_cli (argv):
-    check_usage (mjd2date_doc, argv, usageifnoargs=True)
+def mjd2date_cli(argv):
+    check_usage(mjd2date_doc, argv, usageifnoargs=True)
 
-    if len (argv) != 2:
-        wrong_usage (mjd2date_doc, 'expect exactly one argument')
+    if len(argv) != 2:
+        wrong_usage(mjd2date_doc, 'expect exactly one argument')
 
-    print (mjd2date (float (argv[1])))
+    print(mjd2date(float(argv[1])))
 
 
 # mstransform
 
 mstransform_doc = \
 """
 casatask mstransform vis=[] [keywords]
@@ -2961,16 +3306,16 @@
 vis=
   Input visibility MS
 
 out=
   Output visibility MS
 
 datacolumn=corrected
-  The data column on which to operate. Comma-separated list of:
-    data, model, corrected, float_data, lag_data, all
+  The data column on which to operate. Comma-separated list of: ``data``,
+  ``model``, ``corrected``, ``float_data``, ``lag_data``, ``all``
 
 realmodelcol=False
   If true, turn a virtual model column into a real one.
 
 keepflags=True
   If false, discard completely-flagged rows.
 
@@ -2990,22 +3335,23 @@
   If true, put the data on a new spectral window structure or reference frame.
 
 timebin=<seconds>
   If specified, time-average the visibilities with the specified binning.
 
 timespan=<undefined>
   Allow averaging to span over potential discontinuities in the data set.
-  Comma-separated list of options; allowed values are:
-    scan, state
+  Comma-separated list of options; allowed values are: ``scan``, ``state``
 
 """ + stdsel_doc + loglevel_doc
 
-class MstransformConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    out = Custom (str, required=True)
+class MstransformConfig(ParseKeywords):
+    __doc__ = makecfgdoc('mstransform', mstransform_doc)
+
+    vis = Custom(str, required=True)
+    out = Custom(str, required=True)
 
     datacolumn = 'corrected'
     realmodelcol = False
     keepflags = True
     usewtspectrum = False
     combinespws = False
     chanaverage = False
@@ -3026,85 +3372,99 @@
     timerange = str
     uvrange = str
     taql = str
 
     loglevel = 'warn'
 
 
-def mstransform (cfg):
-    mt = util.tools.mstransformer ()
-    qa = util.tools.quanta ()
+def mstransform(cfg):
+    mt = util.tools.mstransformer()
+    qa = util.tools.quanta()
 
-    mtconfig = extractmsselect (cfg, havearray=True, havecorr=True, taqltomsselect=False)
+    mtconfig = extractmsselect(cfg, havearray=True, havecorr=True, taqltomsselect=False)
     mtconfig['inputms'] = cfg.vis
     mtconfig['outputms'] = cfg.out
 
     if not cfg.keepflags:
-        if len (mtconfig.get ('taql', '')):
-            mtconfig['taql'] += 'AND NOT (FLAG_ROW OR ALL(FLAG))'
+        if len(mtconfig.get('taql', '')):
+            mtconfig['taql'] += 'AND NOT(FLAG_ROW OR ALL(FLAG))'
         else:
-            mtconfig['taql'] = 'NOT (FLAG_ROW OR ALL(FLAG))'
+            mtconfig['taql'] = 'NOT(FLAG_ROW OR ALL(FLAG))'
 
     mtconfig['datacolumn'] = cfg.datacolumn
 
-    if 'MODEL' in cfg.datacolumn.upper () or cfg.datacolumn.upper () == 'ALL':
+    if 'MODEL' in cfg.datacolumn.upper() or cfg.datacolumn.upper() == 'ALL':
         mtconfig['realmodelcol'] = cfg.realmodelcol
 
-    mtconfig['combinespws'] = bool (cfg.combinespws)
-    mtconfig['hanning'] = bool (cfg.hanning)
+    mtconfig['combinespws'] = bool(cfg.combinespws)
+    mtconfig['hanning'] = bool(cfg.hanning)
 
     if cfg.chanaverage:
-        raise NotImplementedError ('mstransform: chanaverage')
+        raise NotImplementedError('mstransform: chanaverage')
 
     if cfg.regridms:
-        raise NotImplementedError ('mstransform: regridms')
+        raise NotImplementedError('mstransform: regridms')
 
     if cfg.timebin is not None:
         mtconfig['timeaverage'] = True
-        mtconfig['timebin'] = str (cfg.timebin) + 's'
-        mtconfig['timespan'] = ','.join (cfg.timespan)
+        mtconfig['timebin'] = str(cfg.timebin) + 's'
+        mtconfig['timespan'] = ','.join(cfg.timespan)
         # not implemented: maxuvwdistance
 
-    mt.config (b(mtconfig))
-    mt.open ()
-    mt.run ()
-    mt.done ()
+    mt.config(b(mtconfig))
+    mt.open()
+    mt.run()
+    mt.done()
 
     # not implemented: updating FLAG_CMD table
     # not implemented: updating history
 
 
-mstransform_cli = makekwcli (mstransform_doc, MstransformConfig, mstransform)
+mstransform_cli = makekwcli(mstransform_doc, MstransformConfig, mstransform)
 
 
 # plotants
 
 plotants_doc = \
 """
 casatask plotants <MS> <figfile>
 
 Plot the physical layout of the antennas described in the MS.
 """
 
-def plotants (vis, figfile):
+def plotants(vis, figfile):
+    """Plot the physical layout of the antennas described in the MS.
+
+    vis (str)
+      Path to the input dataset
+    figfile (str)
+      Path to the output image file.
+
+    The output image format will be inferred from the extension of *figfile*.
+    Example::
+
+      from pwkit.environments.casa import tasks
+      tasks.plotants('dataset.ms', 'antennas.png')
+
+    """
     from .scripting import CasapyScript
 
-    script = os.path.join (os.path.dirname (__file__), 'cscript_plotants.py')
+    script = os.path.join(os.path.dirname(__file__), 'cscript_plotants.py')
 
-    with CasapyScript (script, vis=vis, figfile=figfile) as cs:
+    with CasapyScript(script, vis=vis, figfile=figfile) as cs:
         pass
 
 
-def plotants_cli (argv):
-    check_usage (plotants_doc, argv, usageifnoargs=True)
+def plotants_cli(argv):
+    check_usage(plotants_doc, argv, usageifnoargs=True)
 
-    if len (argv) != 3:
-        wrong_usage (plotants_doc, 'expect exactly two arguments')
+    if len(argv) != 3:
+        wrong_usage(plotants_doc, 'expect exactly two arguments')
 
-    plotants (argv[1], argv[2])
+    plotants(argv[1], argv[2])
 
 
 # plotcal
 
 plotcal_doc = \
 """
 casatask plotcal caltable=<MS> [keywords]
@@ -3119,35 +3479,32 @@
 
 yaxis=
   amp antenna imag phase real snr
 
 iteration=
   antenna field spw time
 
-*** Data selection
+**Supported data selection keywords**
 
-antenna=
-field=
-poln=
-  RL R L XY X Y '/'
-spw=
-timerange=
+Limited data selection is supported. Allowed keywords are ``antenna``,
+``field``, ``poln``, ``spw``, and ``timerange``. The ``poln`` keyword may take
+on the values ``RL``, ``R``, ``L``, ``XY``, ``X``, ``Y``, and ``/``.
 
-*** Plot appearance options
+**Plot appearance options**
 
-plotsymbol=
-plotcolor=
-fontsize=
-figfile=
+To be documented. These keywords control the plot appearance: ``plotsymbol``,
+``plotcolor``, ``fontsize``, ``figfile``.
 
 """ + loglevel_doc
 
 
-class PlotcalConfig (ParseKeywords):
-    caltable = Custom (str, required=True)
+class PlotcalConfig(ParseKeywords):
+    __doc__ = makecfgdoc('plotcal', plotcal_doc)
+
+    caltable = Custom(str, required=True)
     xaxis = 'time'
     yaxis = 'amp'
     iteration = ''
 
     # not implemented: subplot, overplot, clearpanel, plotrange,
     # showflags, showgui
 
@@ -3159,62 +3516,61 @@
 
     antenna = ''
     field = ''
     poln = 'RL'
     spw = ''
     timerange = ''
 
+    loglevel = 'warn'
+
 
-def plotcal (cfg):
+def plotcal(cfg):
     # casa-tools plotting relies on invoking matplotlib in an internal Python
-    # interpreter (!), and it uses a very old version of matplotlib that's
+    # interpreter(!), and it uses a very old version of matplotlib that's
     # essentially incompatible with what's available in any up-to-date Python
-    # environment (e.g. Anaconda). Therefore we have to launch any plotcal
+    # environment(e.g. Anaconda). Therefore we have to launch any plotcal
     # operations as casapy scripts to ensure compatibility.
 
     from .scripting import CasapyScript
 
-    script = os.path.join (os.path.dirname (__file__), 'cscript_plotcal.py')
+    script = os.path.join(os.path.dirname(__file__), 'cscript_plotcal.py')
 
-    selectcals = b(dict (antenna = cfg.antenna,
+    selectcals = b(dict(antenna = cfg.antenna,
                          field = cfg.field,
-                         poln = cfg.poln.upper (),
+                         poln = cfg.poln.upper(),
                          spw = cfg.spw,
                          time = cfg.timerange))
 
-    plotoptions = b(dict (iteration = cfg.iteration,
+    plotoptions = b(dict(iteration = cfg.iteration,
                           plotrange = [0.0]*4,
                           plotsymbol = cfg.plotsymbol,
                           plotcolor = cfg.plotcolor,
                           markersize = cfg.markersize,
                           fontsize = cfg.fontsize))
 
-    with CasapyScript (script,
+    with CasapyScript(script,
                        caltable=b(cfg.caltable),
                        selectcals=selectcals,
                        plotoptions=plotoptions,
-                       xaxis=b(cfg.xaxis.upper ()),
-                       yaxis=b(cfg.yaxis.upper ()),
+                       xaxis=b(cfg.xaxis.upper()),
+                       yaxis=b(cfg.yaxis.upper()),
                        figfile=b(cfg.figfile)) as cs:
         pass
 
 
-def plotcal_cli (argv):
-    check_usage (plotcal_doc, argv, usageifnoargs=True)
-    cfg = PlotcalConfig ().parse (argv[1:])
-    plotcal (cfg)
+plotcal_cli = makekwcli(plotcal_doc, PlotcalConfig, plotcal)
 
 
 # polmodel
 #
 # Shim for a separate module
 
-def polmodel_cli (argv):
+def polmodel_cli(argv):
     from .polmodel import polmodel_cli
-    polmodel_cli (argv)
+    polmodel_cli(argv)
 
 
 # setjy
 
 setjy_doc = \
 """
 casatask setjy vis= [keywords]
@@ -3237,37 +3593,37 @@
   An image to use as the basis for the source's spatial structure and,
   potentialy, flux density (if fluxdensity=0). Only usable for Stokes
   I.  If the verbatim value of "modimage" can't be opened as a path,
   it is assumed to be relative to the CASA data directory; a typical
   value might be "nrao/VLA/CalModels/3C286_C.im".
 
 spindex=
+  If using ``fluxdensity``, these specify the spectral dependence of the values,
+  such that ``S = fluxdensity * (freq/reffreq)**spindex``. Reffreq is in GHz.
+  Default values are 0 and 1, giving no spectral dependence.
+
 reffreq=
-  If using fluxdensity, these specify the spectral dependence of the
-  values, such that S = fluxdensity * (freq/reffreq)**spindex. Reffreq
-  is in GHz. Default values are 0 and 1, giving no spectral
-  dependence.
+  See ``spindex``.
 
 standard='Perley-Butler 2013'
   Acceptable values are: Baars, Perley 90, Perley-Taylor 95,
   Perley-Taylor 99, Perley-Butler 2010, Perley-Butler 2013. You can
   specify the solar-system standard "Butler-JPL-Horizons 2012", but
   doing so farms out the work to a stock CASA installation.
 
-*** Supported data selection keywords:
+**Supported data selection keywords**
 
-field=
-observation=
-scan=
-spw=
-timerange=
+Only a subset of the standard data selection keywords are supported:
+``field``, ``observation``, ``scan``, ``spw``, ``timerange``..
 """ + loglevel_doc
 
-class SetjyConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class SetjyConfig(ParseKeywords):
+    __doc__ = makecfgdoc('setjy', setjy_doc)
+
+    vis = Custom(str, required=True)
     modimage = str
     fluxdensity = [-1., 0., 0., 0.]
     spindex = 0.
     reffreq = 1. # GHz
     standard = 'Perley-Butler 2013'
 
     field = str
@@ -3275,68 +3631,68 @@
     scan = str
     spw = str
     timerange = str
 
     loglevel = 'warn'
 
 
-def setjy (cfg):
+def setjy(cfg):
     if cfg.standard == 'Butler-JPL-Horizons 2012':
         # The CASA C++ code has stuff that fakes you into thinking that the
         # solar system flux density cal implementation is all in C++, but
         # actually the current implementation is all in Python in the core
         # CASA distribution. It'd be a real pain to duplicate so we farm it
         # out to a CASA distribution.
         from .scripting import CasapyScript
-        script = os.path.join (os.path.dirname (__file__), 'cscript_setjy.py')
-        args = dict (
+        script = os.path.join(os.path.dirname(__file__), 'cscript_setjy.py')
+        args = dict(
             vis = cfg.vis,
             standard = cfg.standard,
             field = cfg.field,
             observation = cfg.observation,
             scan = cfg.scan,
             spw = cfg.spw,
             timerange = cfg.timerange,
             scalebychan = True, # see below
         )
-        print ('Farming out to CASA ...')
-        with CasapyScript (script, **b(args)) as cs:
-            with open (os.path.join (cs.workdir, 'casa_stderr'), 'r') as f:
-                stderr = f.read ()
-            print (stderr)
+        print('Farming out to CASA ...')
+        with CasapyScript(script, **args) as cs:
+            with open(os.path.join(cs.workdir, 'casa_stderr'), 'r') as f:
+                stderr = f.read()
+            print(stderr)
         return
 
     kws = {}
 
-    for kw in 'field fluxdensity observation scan spw standard'.split ():
-        kws[kw] = getattr (cfg, kw) or ''
+    for kw in 'field fluxdensity observation scan spw standard'.split():
+        kws[kw] = getattr(cfg, kw) or ''
 
     kws['time'] = cfg.timerange or ''
-    kws['reffreq'] = str (cfg.reffreq) + 'GHz'
+    kws['reffreq'] = str(cfg.reffreq) + 'GHz'
     kws['spix'] = cfg.spindex
     kws['scalebychan'] = True # don't think you'd ever want false??
 
     if cfg.modimage is None:
         kws['modimage'] = ''
     else:
-        if os.path.isdir (cfg.modimage):
+        if os.path.isdir(cfg.modimage):
             mi = cfg.modimage
         else:
-            mi = util.datadir (cfg.modimage)
-            if not os.path.isdir (mi):
-                raise RuntimeError ('no model image "%s" or "%s"' % (cfg.modimage, mi))
+            mi = util.datadir(cfg.modimage)
+            if not os.path.isdir(mi):
+                raise RuntimeError('no model image "%s" or "%s"' % (cfg.modimage, mi))
         kws['modimage'] = mi
 
-    im = util.tools.imager ()
-    im.open (b(cfg.vis), usescratch=False) # don't think you'll ever want True?
-    im.setjy (**b(kws))
-    im.close ()
+    im = util.tools.imager()
+    im.open(b(cfg.vis), usescratch=False) # don't think you'll ever want True?
+    im.setjy(**kws)
+    im.close()
 
 
-setjy_cli = makekwcli (setjy_doc, SetjyConfig, setjy)
+setjy_cli = makekwcli(setjy_doc, SetjyConfig, setjy)
 
 
 # split
 #
 # note: spw=999 -> exception; scan=999 -> no output, or error, generated
 
 split_doc = \
@@ -3347,26 +3703,27 @@
   Time-average data into bins of "timebin" seconds; defaults to no averaging
 
 step=
   Frequency-average data in bins of "step" channels; defaults to no averaging
 
 col=all
   Extract the column "col" as the DATA column. If "all", copy all available
-  columns without renaming. Possible values:
-    all DATA MODEL_DATA CORRECTED_DATA FLOAT_DATA LAG_DATA
+  columns without renaming. Possible values: ``all``, ``DATA``, ``MODEL_DATA``,
+  ``CORRECTED_DATA``, ``FLOAT_DATA``, ``LAG_DATA``.
 
 combine=[col1,col2,...]
   When time-averaging, don't start a new bin when the specified columns change.
-  Acceptable column names:
-    scan state
+  Acceptable column names: ``scan``, ``state``.
 """ + stdsel_doc + loglevel_doc
 
-class SplitConfig (ParseKeywords):
-    vis = Custom (str, required=True)
-    out = Custom (str, required=True)
+class SplitConfig(ParseKeywords):
+    __doc__ = makecfgdoc('split', split_doc)
+
+    vis = Custom(str, required=True)
+    out = Custom(str, required=True)
 
     timebin = float # seconds
     step = 1
     col = 'all'
     combine = [str]
 
     antenna = str
@@ -3380,30 +3737,30 @@
     taql = str
     timerange = str
     uvrange = str
 
     loglevel = 'warn'
 
 
-def split (cfg):
+def split(cfg):
     import tempfile, shutil
 
-    kws = extractmsselect (cfg, havearray=True, havecorr=True,
+    kws = extractmsselect(cfg, havearray=True, havecorr=True,
                            observationtoobs=True, taqltomsselect=False)
     kws['whichcol'] = cfg.col
-    kws['combine'] = ','.join (cfg.combine)
+    kws['combine'] = ','.join(cfg.combine)
     kws['step'] = [cfg.step] # can be done on per-spw basis; we skip that
 
     if cfg.timebin is None:
         kws['timebin'] = '-1s'
     else:
-        kws['timebin'] = str (cfg.timebin) + 's'
+        kws['timebin'] = str(cfg.timebin) + 's'
 
-    ms = util.tools.ms ()
-    ms.open (b(cfg.vis))
+    ms = util.tools.ms()
+    ms.open(b(cfg.vis))
 
     # split() will merrily overwrite an existing MS, which I think is
     # very bad behavior. We try to prevent this in two steps: 1) claim
     # the desired output name in a way that will error out if it
     # already exists; 2) tell split() to create its outputs in an
     # empty temporary directory, to minimize the chances of blowing
     # away anything preexisting. In the pathological case, there's a
@@ -3421,224 +3778,226 @@
     # to make sure it's on the same device.
 
     didntmakeit = True
     renamed = False
     workdir = None
 
     try:
-        didntmakeit = os.mkdir (cfg.out, 0) # error raised if already exists.
+        didntmakeit = os.mkdir(cfg.out, 0) # error raised if already exists.
 
         try:
-            workdir = tempfile.mkdtemp (dir=os.path.dirname (cfg.out),
-                                        prefix=os.path.basename (cfg.out) + '_')
-            kws['outputms'] = os.path.join (workdir, os.path.basename (cfg.out))
-            ms.split (**b(kws))
-            os.rename (kws['outputms'], cfg.out)
+            workdir = tempfile.mkdtemp(dir=os.path.dirname(cfg.out),
+                                        prefix=os.path.basename(cfg.out) + '_')
+            kws['outputms'] = os.path.join(workdir, os.path.basename(cfg.out))
+            ms.split(**kws)
+            os.rename(kws['outputms'], cfg.out)
             renamed = True
         finally:
             if workdir is not None:
-                shutil.rmtree (workdir, ignore_errors=True)
+                shutil.rmtree(workdir, ignore_errors=True)
     finally:
         if not didntmakeit and not renamed:
             try:
-                os.rmdir (cfg.out)
+                os.rmdir(cfg.out)
             except:
                 pass
 
-    ms.close ()
+    ms.close()
 
 
-split_cli = makekwcli (split_doc, SplitConfig, split)
+split_cli = makekwcli(split_doc, SplitConfig, split)
 
 
 # spwglue
 #
 # Shim for a separate module
 
-def spwglue_cli (argv):
+def spwglue_cli(argv):
     from .spwglue import spwglue_cli
-    spwglue_cli (argv)
+    spwglue_cli(argv)
 
 
 # tsysplot
 #
 # See bpplot() -- CASA plotcal can do this in a certain sense, but it's slow
 # and ugly.
 
 tsysplot_doc = \
 """
 casatask tsysplot caltable= dest=
 
-Plot a system temperature (Tsys) calibration table.
+Plot a system temperature(Tsys) calibration table.
 
 caltable=MS
   The input calibration Measurement Set
 
 dest=PATH
   If specified, plots are saved to this file -- the format is inferred
   from the extension, which must allow multiple pages to be saved. If
   unspecified, the plots are displayed using a Gtk3 backend.
 
 dims=WIDTH,HEIGHT
   If saving to a file, the dimensions of a each page. These are in points
-  for vector formats (PDF, PS) and pixels for bitmaps (PNG). Defaults to
+  for vector formats(PDF, PS) and pixels for bitmaps(PNG). Defaults to
   1000, 600.
 
 margins=TOP,RIGHT,LEFT,BOTTOM
   If saving to a file, the plot margins in the same units as the dims.
   The default is 4 on every side.
 """ + loglevel_doc
 
 
-class TsysplotConfig (ParseKeywords):
-    caltable = Custom (str, required=True)
+class TsysplotConfig(ParseKeywords):
+    __doc__ = makecfgdoc('tsysplot', tsysplot_doc)
+
+    caltable = Custom(str, required=True)
     dest = str
     dims = [1000, 600]
     margins = [4, 4, 4, 4]
     loglevel = 'warn'
 
 
-def tsysplot (cfg):
+def tsysplot(cfg):
     import omega as om, omega.render
     from ... import numutil
 
-    if isinstance (cfg.dest, omega.render.Pager):
+    if isinstance(cfg.dest, omega.render.Pager):
         # This is for non-CLI invocation.
         pager = cfg.dest
     elif cfg.dest is None:
         import omega.gtk3
-        pager = om.makeDisplayPager ()
+        pager = om.makeDisplayPager()
     else:
-        pager = om.makePager (cfg.dest,
+        pager = om.makePager(cfg.dest,
                               dims=cfg.dims,
                               margins=cfg.margins,
-                              style=om.styles.ColorOnWhiteVector ())
+                              style=om.styles.ColorOnWhiteVector())
 
-    tb = util.tools.table ()
+    tb = util.tools.table()
 
-    tb.open (binary_type (cfg.caltable), nomodify=True)
-    fields = tb.getcol (b'FIELD_ID')
-    spws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    ants = tb.getcol (b'ANTENNA1')
-    vals = tb.getcol (b'FPARAM')
-    flags = tb.getcol (b'FLAG')
-    times = tb.getcol (b'TIME')
-    tb.close ()
-
-    tb.open (binary_type (os.path.join (cfg.caltable, 'ANTENNA')), nomodify=True)
-    antnames = tb.getcol (b'NAME')
-    tb.close ()
-
-    tb.open (binary_type (os.path.join (cfg.caltable, 'FIELD')), nomodify=True)
-    fieldnames = tb.getcol (b'NAME')
-    tb.close ()
+    tb.open(cfg.caltable, nomodify=True)
+    fields = tb.getcol(b'FIELD_ID')
+    spws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    ants = tb.getcol(b'ANTENNA1')
+    vals = tb.getcol(b'FPARAM')
+    flags = tb.getcol(b'FLAG')
+    times = tb.getcol(b'TIME')
+    tb.close()
+
+    tb.open(os.path.join(cfg.caltable, 'ANTENNA'), nomodify=True)
+    antnames = tb.getcol(b'NAME')
+    tb.close()
+
+    tb.open(os.path.join(cfg.caltable, 'FIELD'), nomodify=True)
+    fieldnames = tb.getcol(b'NAME')
+    tb.close()
 
     npol, nchan, nsoln = vals.shape
 
     # see what we've got
 
-    def seen_values (data):
-        return [idx for idx, count in enumerate (np.bincount (data)) if count]
+    def seen_values(data):
+        return [idx for idx, count in enumerate(np.bincount(data)) if count]
 
-    any_ok = ~(np.all (flags, axis=(0, 1)))
-    seenfields = seen_values (fields[any_ok])
-    field_offsets = dict ((fieldid, idx) for idx, fieldid in enumerate (seenfields))
-    seenants = seen_values (ants[any_ok])
-    ant_offsets = dict ((antid, idx) for idx, antid in enumerate (seenants))
+    any_ok = ~(np.all(flags, axis=(0, 1)))
+    seenfields = seen_values(fields[any_ok])
+    field_offsets = dict((fieldid, idx) for idx, fieldid in enumerate(seenfields))
+    seenants = seen_values(ants[any_ok])
+    ant_offsets = dict((antid, idx) for idx, antid in enumerate(seenants))
 
     apbyfield = {}
-    seenspws = set ()
+    seenspws = set()
 
     for ifield in seenfields:
         antpols = apbyfield[ifield] = {}
 
-        for ipol in range (npol):
-            for isoln in np.where (fields == ifield)[0]:
-                if not flags[ipol,:,isoln].all ():
+        for ipol in range(npol):
+            for isoln in np.where(fields == ifield)[0]:
+                if not flags[ipol,:,isoln].all():
                     k = (ants[isoln], ipol)
-                    byspw = antpols.get (k)
+                    byspw = antpols.get(k)
                     if byspw is None:
                         antpols[k] = byspw = []
 
-                    byspw.append ((spws[isoln], isoln))
-                    seenspws.add (spws[isoln])
+                    byspw.append((spws[isoln], isoln))
+                    seenspws.add(spws[isoln])
 
-    seenspws = sorted (seenspws)
-    spw_to_offset = dict ((spwid, spwofs * nchan)
-                          for spwofs, spwid in enumerate (seenspws))
+    seenspws = sorted(seenspws)
+    spw_to_offset = dict((spwid, spwofs * nchan)
+                          for spwofs, spwid in enumerate(seenspws))
 
     # find plot limits
 
-    min_time = times[any_ok].min ()
-    max_time = times[any_ok].max ()
-    mjdref = int (np.floor (min_time))
+    min_time = times[any_ok].min()
+    max_time = times[any_ok].max()
+    mjdref = int(np.floor(min_time))
     times -= mjdref # convert to delta-MJD
     min_time = (min_time - mjdref)
     max_time = (max_time - mjdref)
     span = max_time - min_time
     if span <= 0:
         if max_time == 0:
             span = 1.
         else:
             span = 0.05 * max_time
     max_time += 0.05 * span
     min_time -= 0.05 * span
 
-    okvals = vals[np.where (~flags)]
-    max_val = okvals.max ()
-    min_val = okvals.min ()
+    okvals = vals[np.where(~flags)]
+    max_val = okvals.max()
+    min_val = okvals.min()
     span = max_val - min_val
     if span <= 0:
         if max_val == 0:
             span = 1.
         else:
             span = 0.05 * max_val
     max_val += 0.05 * span
     min_val -= 0.05 * span
 
     polnames = 'XY' # XXX: identification doesn't seem to be stored in cal table
 
     # plot away
 
-    for iant, ipol in sorted (six.iterkeys (antpols)):
-        p = om.RectPlot ()
-        p.addKeyItem ('%s %s' % (antnames[iant], polnames[ipol]))
+    for iant, ipol in sorted(six.iterkeys(antpols)):
+        p = om.RectPlot()
+        p.addKeyItem('%s %s' % (antnames[iant], polnames[ipol]))
 
         for ifield in seenfields:
             antpols = apbyfield[ifield]
             kt = fieldnames[ifield]
 
             for ispw, isoln in antpols.get((iant,ipol), []):
                 f = flags[ipol,:,isoln]
                 v = vals[ipol,:,isoln]
-                w = np.where (~f)[0]
+                w = np.where(~f)[0]
 
-                for s in numutil.slice_around_gaps (w, 1):
+                for s in numutil.slice_around_gaps(w, 1):
                     wsub = w[s]
                     if wsub.size == 0:
                         continue # Should never happen, but eh.
                     else:
                         # It'd also be pretty weird to have a spectral window
-                        # containing just one (valid) channel, but it could
+                        # containing just one(valid) channel, but it could
                         # happen.
                         lines = (wsub.size > 1)
 
-                    p.addXY (wsub + spw_to_offset[ispw], v[wsub], kt,
+                    p.addXY(wsub + spw_to_offset[ispw], v[wsub], kt,
                              lines=lines, dsn=ifield)
                     kt = None
 
-        p.setBounds (xmin=0,
-                     xmax=len (seenspws) * nchan,
+        p.setBounds(xmin=0,
+                     xmax=len(seenspws) * nchan,
                      ymin=min_val,
                      ymax=max_val)
-        p.setLabels ('Normalized channel', 'System temperature (K)')
-        pager.send (p)
+        p.setLabels('Normalized channel', 'System temperature(K)')
+        pager.send(p)
 
 
-tsysplot_cli = makekwcli (tsysplot_doc, TsysplotConfig, tsysplot)
+tsysplot_cli = makekwcli(tsysplot_doc, TsysplotConfig, tsysplot)
 
 
 # uvsub
 #
 # We add UV selection keywords not supported by the CASA task.
 # I assume that they're honored ...
 
@@ -3653,16 +4012,18 @@
 
 reverse=
   Boolean, default false, which means to set CORRECTED = DATA - MODEL. If
   true, CORRECTED = DATA + MODEL.
 """ + stdsel_doc + loglevel_doc
 
 
-class UvsubConfig (ParseKeywords):
-    vis = Custom (str, required=True)
+class UvsubConfig(ParseKeywords):
+    __doc__ = makecfgdoc('uvsub', uvsub_doc)
+
+    vis = Custom(str, required=True)
     reverse = False
 
     antenna = str
     array = str
     field = str
     intent = str
     observation = str
@@ -3671,27 +4032,27 @@
     timerange = str
     uvrange = str
     taql = str
 
     loglevel = 'warn'
 
 
-def uvsub (cfg):
-    ms = util.tools.ms ()
+def uvsub(cfg):
+    ms = util.tools.ms()
 
-    ms.open (b(cfg.vis), nomodify=False)
-    ms.msselect (b(extractmsselect (cfg,
+    ms.open(b(cfg.vis), nomodify=False)
+    ms.msselect(b(extractmsselect(cfg,
                                     havearray=True,
                                     intenttoscanintent=True,
                                     taqltomsselect=False)))
-    ms.uvsub (reverse=cfg.reverse)
-    ms.close ()
+    ms.uvsub(reverse=cfg.reverse)
+    ms.close()
 
 
-uvsub_cli = makekwcli (uvsub_doc, UvsubConfig, uvsub)
+uvsub_cli = makekwcli(uvsub_doc, UvsubConfig, uvsub)
 
 
 # xyphplot
 #
 # This is nearly the same as bpplot.
 
 xyphplot_doc = \
@@ -3706,144 +4067,146 @@
 dest=PATH
   If specified, plots are saved to this file -- the format is inferred
   from the extension, which must allow multiple pages to be saved. If
   unspecified, the plots are displayed using a Gtk3 backend.
 
 dims=WIDTH,HEIGHT
   If saving to a file, the dimensions of a each page. These are in points
-  for vector formats (PDF, PS) and pixels for bitmaps (PNG). Defaults to
+  for vector formats(PDF, PS) and pixels for bitmaps(PNG). Defaults to
   1000, 600.
 
 margins=TOP,RIGHT,LEFT,BOTTOM
   If saving to a file, the plot margins in the same units as the dims.
   The default is 4 on every side.
 """ + loglevel_doc
 
 
-class XyphplotConfig (ParseKeywords):
-    caltable = Custom (str, required=True)
+class XyphplotConfig(ParseKeywords):
+    __doc__ = makecfgdoc('xyphplot', xyphplot_doc)
+
+    caltable = Custom(str, required=True)
     dest = str
     dims = [1000, 600]
     margins = [4, 4, 4, 4]
     loglevel = 'warn'
 
 
-def xyphplot (cfg):
+def xyphplot(cfg):
     import omega as om, omega.render
     from ... import numutil
 
-    if isinstance (cfg.dest, omega.render.Pager):
+    if isinstance(cfg.dest, omega.render.Pager):
         # This is for non-CLI invocation.
         pager = cfg.dest
     elif cfg.dest is None:
         import omega.gtk3
-        pager = om.makeDisplayPager ()
+        pager = om.makeDisplayPager()
     else:
-        pager = om.makePager (cfg.dest,
+        pager = om.makePager(cfg.dest,
                               dims=cfg.dims,
                               margins=cfg.margins,
-                              style=om.styles.ColorOnWhiteVector ())
+                              style=om.styles.ColorOnWhiteVector())
 
-    tb = util.tools.table ()
+    tb = util.tools.table()
 
     # Every antenna has the same solution, and only the first of two
     # polarizations is not just unity. And the solution is phase only. So this
     # is prett simple to plot!
 
-    tb.open (binary_type (cfg.caltable), nomodify=True)
-    spws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    vals = tb.getcol (b'CPARAM')
-    flags = tb.getcol (b'FLAG')
-    tb.close ()
+    tb.open(cfg.caltable, nomodify=True)
+    spws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    vals = tb.getcol(b'CPARAM')
+    flags = tb.getcol(b'FLAG')
+    tb.close()
 
     npol, nchan, nsoln = vals.shape
 
-    seenspws = np.unique (spws) # assume all available
-    spw_to_offset = dict ((spwid, spwofs * nchan)
-                          for spwofs, spwid in enumerate (seenspws))
+    seenspws = np.unique(spws) # assume all available
+    spw_to_offset = dict((spwid, spwofs * nchan)
+                          for spwofs, spwid in enumerate(seenspws))
 
     # find plot limits
 
-    okvals = vals[np.where (~flags)]
+    okvals = vals[np.where(~flags)]
 
-    max_ph = np.angle (okvals, deg=True).max ()
-    min_ph = np.angle (okvals, deg=True).min ()
+    max_ph = np.angle(okvals, deg=True).max()
+    min_ph = np.angle(okvals, deg=True).min()
     span = max_ph - min_ph
     max_ph += 0.05 * span
     min_ph -= 0.05 * span
     if max_ph > 160:
         max_ph = 180
     if min_ph < -160:
         min_ph = -180
 
     polnames = 'XY' # XXX: identification doesn't seem to be stored in cal table
 
     # plot away
 
-    p = om.RectPlot ()
+    p = om.RectPlot()
 
     for ispw in seenspws:
         ipol = 0
-        isoln = np.where ((spws == ispw) & ~np.all (flags, axis=(0,1)))[0][0]
+        isoln = np.where((spws == ispw) & ~np.all(flags, axis=(0,1)))[0][0]
 
         f = flags[ipol,:,isoln]
-        ph = np.angle (vals[ipol,:,isoln], deg=True)
-        w = np.where (~f)[0]
+        ph = np.angle(vals[ipol,:,isoln], deg=True)
+        w = np.where(~f)[0]
 
-        for s in numutil.slice_around_gaps (w, 1):
+        for s in numutil.slice_around_gaps(w, 1):
             wsub = w[s]
             if wsub.size == 0:
                 continue # Should never happen, but eh.
             else:
                 # It'd also be pretty weird to have a spectral window
-                # containing just one (valid) channel, but it could
+                # containing just one(valid) channel, but it could
                 # happen.
                 lines = (wsub.size > 1)
 
-            p.addXY (wsub + spw_to_offset[ispw], ph[wsub], None,
-                     lines=lines, dsn=ispw)
+            p.addXY(wsub + spw_to_offset[ispw], ph[wsub], None,
+                    lines=lines, dsn=ispw)
 
-        p.setBounds (xmin=0,
-                     xmax=len (seenspws) * nchan,
+        p.setBounds(xmin=0,
+                     xmax=len(seenspws) * nchan,
                      ymin=min_ph,
                      ymax=max_ph)
-        p.setLabels ('Normalized channel', 'Phase (deg)')
+        p.setLabels('Normalized channel', 'Phase(deg)')
 
-    pager.send (p)
+    pager.send(p)
 
-xyphplot_cli = makekwcli (xyphplot_doc, XyphplotConfig, xyphplot)
+xyphplot_cli = makekwcli(xyphplot_doc, XyphplotConfig, xyphplot)
 
 
 # Driver for command-line access. I wrote this before multitool, and it
 # doesn't seem particularly valuable to convert them to Multitool since the
 # current system works fine.
 
-def cmdline_usage (stream, exitcode):
-    print ('usage: casatask <task> [task-specific arguments]', file=stream)
-    print (file=stream)
-    print ('Supported tasks:', file=stream)
-    print (file=stream)
+def cmdline_usage(stream, exitcode):
+    print('usage: casatask <task> [task-specific arguments]', file=stream)
+    print(file=stream)
+    print('Supported tasks:', file=stream)
+    print(file=stream)
 
-    for name in sorted (six.iterkeys (globals ())):
-        if name.endswith ('_cli'):
-            print (name[:-4], file=stream)
+    for name in sorted(six.iterkeys(globals())):
+        if name.endswith('_cli'):
+            print(name[:-4], file=stream)
 
-    raise SystemExit (exitcode)
+    raise SystemExit(exitcode)
 
 
-def commandline (argv=None):
+def commandline(argv=None):
     if argv is None:
         argv = sys.argv
         from ... import cli
-        cli.propagate_sigint ()
-        cli.backtrace_on_usr1 ()
-        cli.unicode_stdio ()
+        cli.propagate_sigint()
+        cli.backtrace_on_usr1()
+        cli.unicode_stdio()
 
-    if len (argv) < 2 or argv[1] == '--help':
-        cmdline_usage (sys.stdout, 0)
+    if len(argv) < 2 or argv[1] == '--help':
+        cmdline_usage(sys.stdout, 0)
 
-    driver = globals ().get (argv[1] + '_cli')
+    driver = globals().get(argv[1] + '_cli')
     if driver is None:
-        die ('unknown task "%s"; run with no arguments for a list', argv[1])
+        die('unknown task "%s"; run with no arguments for a list', argv[1])
 
-    subargv = [' '.join (argv[:2])] + argv[2:]
-    driver (subargv)
+    subargv = [' '.join(argv[:2])] + argv[2:]
+    driver(subargv)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_flagcmd.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_flagcmd.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/scripting_driver.py` & `pwkit-1.0.0/pwkit/environments/casa/scripting_driver.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/scripting.py` & `pwkit-1.0.0/pwkit/environments/casa/scripting.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 write standalone scripts with a hashbang line of "#! /usr/bin/env
 pkcasascript" -- hashbang lines support only one extra command-line
 argument, so if we're using "env" we can't take a multitool approach.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('CasapyScript commandline').split ()
+__all__ = str('CasapyScript commandline').split()
 
 import os.path, shutil, signal, six, sys, tempfile
 from ... import PKError, cli, reraise_context
 from . import CasaEnvironment
 
 
 casapy_argv = ['casa', '--log2term', '--nogui', '-c']
@@ -32,15 +32,15 @@
     signal.SIGQUIT,
     signal.SIGTERM,
     signal.SIGUSR1,
     signal.SIGUSR2,
 ]
 
 
-class CasapyScript (object):
+class CasapyScript(object):
     """Context manager for launching a script in the casapy environment. This
     involves creating a temporary wrapper and then using the CasaEnvironment
     to run it in a temporary directory.
 
     When this context manager is entered, the script is launched and the
     calling process waits until it finishes. This object is returned. The
     `with` statement body is then executed so that information can be
@@ -71,175 +71,175 @@
     wrapped
       the path to the wrapper script run inside casapy.
 
     There is a very large overhead to running casapy scripts. The outer Python
     code sleeps for at least 5 seconds to allow various cleanups to happen.
 
     """
-    def __init__ (self, script, raise_on_error=True, **kwargs):
+    def __init__(self, script, raise_on_error=True, **kwargs):
         self.script = script
         self.kwargs = kwargs
         self.raise_on_error = raise_on_error
 
 
-    def __enter__ (self):
+    def __enter__(self):
         # We read in the entire script and save it in the wrapper. That way we
         # don't have to worry about dealing with file-not-found errors inside
         # casapy, where exception handling is annoying and the startup time is
         # significant.
 
         try:
-            with open (self.script) as f:
-                text = f.read ()
+            with open(self.script) as f:
+                text = f.read()
         except Exception:
-            reraise_context ('while trying to read %r', self.script)
+            reraise_context('while trying to read %r', self.script)
 
-        self.workdir = tempfile.mkdtemp (prefix='casascript', dir='.')
-        self.wrapped = os.path.join (self.workdir, 'wrapped.py')
+        self.workdir = tempfile.mkdtemp(prefix='casascript', dir='.')
+        self.wrapped = os.path.join(self.workdir, 'wrapped.py')
 
-        with open (self.wrapped, 'wb') as wrapper:
-            print ('_pkcs_script = ' + repr (self.script), file=wrapper)
-            print ('_pkcs_text = ' + repr (text), file=wrapper)
-            print ('_pkcs_kwargs = ' + repr (self.kwargs), file=wrapper)
-            print ('_pkcs_origcwd = ' + repr (os.getcwd ()), file=wrapper)
+        with open(self.wrapped, 'w') as wrapper:
+            print('_pkcs_script = ' + repr(self.script), file=wrapper)
+            print('_pkcs_text = ' + repr(text), file=wrapper)
+            print('_pkcs_kwargs = ' + repr(self.kwargs), file=wrapper)
+            print('_pkcs_origcwd = ' + repr(os.getcwd()), file=wrapper)
 
-            driver = __file__.replace ('.pyc', '.py').replace ('.py', '_driver.py')
-            with open (driver) as driver:
+            driver = __file__.replace('.pyc', '.py').replace('.py', '_driver.py')
+            with open(driver) as driver:
                 for line in driver:
-                    print (line, end='', file=wrapper)
+                    print(line, end='', file=wrapper)
 
-        def preexec ():
+        def preexec():
             # Start new session and process groups so that the module can kill all
             # CASA-related processes as best we can.
-            os.setsid ()
+            os.setsid()
 
             # We want to direct casapy's stdout and stderr to separate files since
             # they're full of chatter, while still giving the script access to
             # intentional output on the wrapper's stdout and stderr. At this
             # point, FD's 1 and 2 are the latter. We want to move them to FD's 3
             # and 4, while changing 1 and 2 to the temp files. The close_fds logic
             # of subprocess runs after this function, so we have to set close_fds
             # to False.
 
-            os.dup2 (1, 3) # dup2 closes target fd if needed.
-            os.dup2 (2, 4)
+            os.dup2(1, 3) # dup2 closes target fd if needed.
+            os.dup2(2, 4)
 
-            with open ('casa_stdout', 'wb') as stdout:
-                os.dup2 (stdout.fileno (), 1)
+            with open('casa_stdout', 'wb') as stdout:
+                os.dup2(stdout.fileno(), 1)
 
-            with open ('casa_stderr', 'wb') as stderr:
-                os.dup2 (stderr.fileno (), 2)
+            with open('casa_stderr', 'wb') as stderr:
+                os.dup2(stderr.fileno(), 2)
 
-        self.env = CasaEnvironment ()
-        self.proc = self.env.launch (casapy_argv + ['wrapped.py'],
-                                     cwd=self.workdir,
-                                     stdin=open (os.devnull, 'rb'),
-                                     preexec_fn=preexec,
-                                     close_fds=False)
+        self.env = CasaEnvironment()
+        self.proc = self.env.launch(casapy_argv + ['wrapped.py'],
+                                    cwd=self.workdir,
+                                    stdin=open(os.devnull, 'rb'),
+                                    preexec_fn=preexec,
+                                    close_fds=False)
 
         # Set up signal handlers to propagate to the child process. Copied from
         # wrapout.py.
         prev_handlers = {}
 
-        def handle (signum, frame):
-            self.proc.send_signal (signum)
+        def handle(signum, frame):
+            self.proc.send_signal(signum)
 
         for signum in signals_for_child:
-            prev_handlers[signum] = signal.signal (signum, handle)
+            prev_handlers[signum] = signal.signal(signum, handle)
 
-        self.exitcode = self.proc.wait ()
+        self.exitcode = self.proc.wait()
 
-        for signum, prev_handler in six.iteritems (prev_handlers):
-            signal.signal (signum, prev_handler)
+        for signum, prev_handler in six.iteritems(prev_handlers):
+            signal.signal(signum, prev_handler)
 
         # default: delte workdir on success or intentional script abort
         self.rmtree = (self.exitcode == 0 or self.exitcode == 127)
 
         if self.raise_on_error and self.exitcode != 0:
             # Note that we have to raise the exception here to prevent the
             # `with` statement body from executing. In that case __exit__
             # isn't called so we need to do that too.
-            self._cleanup ()
+            self._cleanup()
 
             if self.exitcode < 0:
-                raise PKError ('casapy was killed by signal %d', -self.exitcode)
+                raise PKError('casapy was killed by signal %d', -self.exitcode)
             elif self.exitcode == 127:
-                raise PKError ('the casapy script signaled an internal error')
+                raise PKError('the casapy script signaled an internal error')
             else:
-                raise PKError ('casapy exited with error code %d', self.exitcode)
+                raise PKError('casapy exited with error code %d', self.exitcode)
 
         return self
 
 
-    def __exit__ (self, etype, evalue, etb):
+    def __exit__(self, etype, evalue, etb):
         if etype is not None:
             self.rmtree = False
 
-        self._cleanup ()
+        self._cleanup()
         return False # propagate exceptions
 
 
-    def _cleanup (self):
+    def _cleanup(self):
         # Ugh, I hate having a hardcoded sleep, but it seems to be necessary
         # to let the watchdog clean everything up. Or something. The casapy
         # process tree is a mess several process groups being created, and I
         # think the only way we can really contain it is with cgroups, which
         # would be difficult and make us Linux-specific. Grrr.
         import time
-        time.sleep (4)
+        time.sleep(4)
 
         # If I'm interpreting things correctly, this bit is needed to kill
         # the "watchdog" process.
 
         try:
-            os.killpg (self.proc.pid, signal.SIGTERM)
+            os.killpg(self.proc.pid, signal.SIGTERM)
         except Exception as e:
             pass
 
-        time.sleep (1)
+        time.sleep(1)
 
         try:
-            os.killpg (self.proc.pid, signal.SIGKILL)
+            os.killpg(self.proc.pid, signal.SIGKILL)
         except Exception as e:
             pass
 
         # OK, blow away the directory.
 
         if not self.rmtree:
-            cli.warn ('preserving directory tree %r since script %r failed',
-                      self.workdir, self.script)
+            cli.warn('preserving directory tree %r since script %r failed',
+                     self.workdir, self.script)
         else:
-            shutil.rmtree (self.workdir, ignore_errors=True)
+            shutil.rmtree(self.workdir, ignore_errors=True)
 
 
 cli_usage = """pkcasascript <scriptfile> [more args...]
 
 Run a specially-designed script inside a CASA environment. This program is not
 meant for regular users. See the documentation of the module
 `pwkit.environments.casa.scripting` for more information."""
 
-def commandline (argv=None):
+def commandline(argv=None):
     if argv is None:
         argv = sys.argv
-        cli.propagate_sigint ()
-        cli.unicode_stdio ()
-        cli.backtrace_on_usr1 ()
+        cli.propagate_sigint()
+        cli.unicode_stdio()
+        cli.backtrace_on_usr1()
 
-    cli.check_usage (cli_usage, argv, usageifnoargs='long')
+    cli.check_usage(cli_usage, argv, usageifnoargs='long')
     script = argv[1]
     args = argv[2:]
 
     try:
-        with CasapyScript (script, cli_args=args) as cs:
+        with CasapyScript(script, cli_args=args) as cs:
             pass
     except Exception:
-        reraise_context ('when running casapy script %r', script)
+        reraise_context('when running casapy script %r', script)
 
     if cs.exitcode < 0:
         signum = -cs.exitcode
-        print ('casascript error: casapy died with signal %d' % signum)
-        signal.signal (signum, signal.SIG_DFL)
-        os.kill (os.getpid (), signum)
+        print('casascript error: casapy died with signal %d' % signum)
+        signal.signal(signum, signal.SIG_DFL)
+        os.kill(os.getpid(), signum)
     elif cs.exitcode:
         if cs.exitcode != 127:
-            print ('casascript error: casapy died with exit code %d' % cs.exitcode)
-        sys.exit (cs.exitcode)
+            print('casascript error: casapy died with exit code %d' % cs.exitcode)
+        sys.exit(cs.exitcode)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/dftdynspec.py` & `pwkit-1.0.0/pwkit/environments/casa/dftdynspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- mode: python; coding: utf-8 -*-
-# Copyright 2013, 2016-2017 Peter Williams <peter@newton.cx> and collaborators
+# Copyright 2013, 2016-2018 Peter Williams <peter@newton.cx> and collaborators
 # Licensed under the MIT License.
 
 # NB. This is super-redundant with both dftphotom and dftspect; things are
 # getting a little silly here. But I think it's faster to copy/paste/hack than
 # it is to merge everything into one uberprogram.
 
 """This module provides code to extract dynamic spectra from CASA Measurement
 Sets. CASA doesn't have a task that does this.
 
 """
-from __future__ import absolute_import, division, print_function, unicode_literals
+from __future__ import absolute_import, division, print_function
 
-__all__ = str ('Config Loader dftdynspec dftdynspec_cli').split ()
+__all__ = 'Config Loader dftdynspec dftdynspec_cli'.split()
 
 import io, os.path, sys
 import numpy as np
 import six
 from six.moves import range
 
 from ... import binary_type, text_type
 # Note: zany spacing so that Sphinx can parse the file correctly.
 from . ..astutil import *
 from . ..cli import check_usage, die
+from . ..io import get_stdout_bytes
 from . ..kwargv import ParseKeywords, Custom
 from . import util
 from .util import sanitize_unicode as b
 
 dftdynspec_doc = \
 """
 casatask dftdynspec vis=<MS> [keywords...]
@@ -76,38 +77,38 @@
 
 The output data are stored as a file containing several serialized Numpy
 arrays. The Python class `pwkit.environments.casa.dftdynspec.Loader` can be
 used to load the data into a Python program.
 
 """
 
-class Config (ParseKeywords):
-    vis = Custom (str, required=True)
+class Config(ParseKeywords):
+    vis = Custom(str, required=True)
     datacol = 'data'
     believeweights = False
 
-    @Custom (str, uiname='out')
-    def outstream (val):
+    @Custom(str, uiname='out')
+    def outstream(val):
         if val is None:
-            return sys.stdout
+            return get_stdout_bytes()
         try:
-            return open (val, 'w')
+            return open(val, 'wb')
         except Exception as e:
-            die ('cannot open path "%s" for writing', val)
+            die('cannot open path "%s" for writing', val)
 
-    @Custom ([str, str], default=None)
-    def rephase (val):
+    @Custom([str, str], default=None)
+    def rephase(val):
         if val is None:
             return None
 
         try:
-            ra = parsehours (val[0])
-            dec = parsedeglat (val[1])
+            ra = parsehours(val[0])
+            dec = parsedeglat(val[1])
         except Exception as e:
-            die ('cannot parse "rephase" values as RA/dec: %s', e)
+            die('cannot parse "rephase" values as RA/dec: %s', e)
         return ra, dec
 
     # MeasurementSet filters
     array = str
     baseline = str
     field = str
     observation = str
@@ -118,18 +119,18 @@
     taql = str
     time = str
     uvdist = str
 
     loglevel = 'warn'
 
 
-def dftdynspec (cfg):
-    tb = util.tools.table ()
-    ms = util.tools.ms ()
-    me = util.tools.measures ()
+def dftdynspec(cfg):
+    tb = util.tools.table()
+    ms = util.tools.ms()
+    me = util.tools.measures()
 
     # Read stuff in. Even if the weight values don't have their
     # absolute scale set correctly, we can still use them to set the
     # relative weighting of the data points.
     #
     # datacol is (ncorr, nchan, nchunk)
     # flag is (ncorr, nchan, nchunk)
@@ -143,140 +144,140 @@
     # selectinit() is broken, but the invocation here is good because it
     # affects the results from ms.range() and friends.
 
     if ':' in (cfg.spw or ''):
         warn('it looks like you are attempting to select channels within one or more spws')
         warn('this is NOT IMPLEMENTED; I will process the whole spw instead')
 
-    ms.open (b(cfg.vis))
-    totrows = ms.nrow ()
-    ms_sels = dict ((n, cfg.get (n)) for n in util.msselect_keys
-                    if cfg.get (n) is not None)
-    ms.msselect (b(ms_sels))
+    ms.open(b(cfg.vis))
+    totrows = ms.nrow()
+    ms_sels = dict((n, cfg.get(n)) for n in util.msselect_keys
+                   if cfg.get(n) is not None)
+    ms.msselect(b(ms_sels))
 
-    rangeinfo = ms.range (b'data_desc_id field_id'.split ())
+    rangeinfo = ms.range(b'data_desc_id field_id'.split())
     ddids = rangeinfo['data_desc_id']
     fields = rangeinfo['field_id']
-    colnames = [cfg.datacol] + 'flag weight time axis_info'.split ()
+    colnames = [cfg.datacol] + 'flag weight time axis_info'.split()
     rephase = (cfg.rephase is not None)
 
     if fields.size != 1:
         # I feel comfortable making this a fatal error, even if we're
         # not rephasing.
-        die ('selected data should contain precisely one field; got %d', fields.size)
+        die('selected data should contain precisely one field; got %d', fields.size)
 
-    tb.open (b(os.path.join (cfg.vis, 'DATA_DESCRIPTION')))
-    ddspws = tb.getcol (b'SPECTRAL_WINDOW_ID')
-    tb.close ()
+    tb.open(b(os.path.join(cfg.vis, 'DATA_DESCRIPTION')))
+    ddspws = tb.getcol(b'SPECTRAL_WINDOW_ID')
+    tb.close()
 
     # Get frequencies and precompute merged, sorted frequency array
     # FIXME: below we get 'freqs' on the fly; should honor that.
     # But then mapping and data storage get super inefficient.
 
-    tb.open (b(os.path.join (cfg.vis, 'SPECTRAL_WINDOW')))
-    nspw = tb.nrows ()
+    tb.open(b(os.path.join(cfg.vis, 'SPECTRAL_WINDOW')))
+    nspw = tb.nrows()
     spwfreqs = []
-    for i in xrange (nspw):
-        spwfreqs.append (tb.getcell (b'CHAN_FREQ', i) * 1e-9) # -> GHz
-    tb.close ()
+    for i in range(nspw):
+        spwfreqs.append(tb.getcell(b'CHAN_FREQ', i) * 1e-9) # -> GHz
+    tb.close()
 
-    allfreqs = set ()
+    allfreqs = set()
     for freqs in spwfreqs:
-        allfreqs.update (freqs)
-    allfreqs = np.asarray (sorted (allfreqs))
+        allfreqs.update(freqs)
+    allfreqs = np.asarray(sorted(allfreqs))
     nfreq = allfreqs.size
 
     freqmaps = []
-    for i in xrange (nspw):
-        freqmaps.append (np.searchsorted (allfreqs, spwfreqs[i]))
+    for i in range(nspw):
+        freqmaps.append(np.searchsorted(allfreqs, spwfreqs[i]))
 
     if rephase:
         fieldid = fields[0]
-        tb.open (b(os.path.join (cfg.vis, 'FIELD')))
-        phdirinfo = tb.getcell (b'PHASE_DIR', fieldid)
-        tb.close ()
+        tb.open(b(os.path.join(cfg.vis, 'FIELD')))
+        phdirinfo = tb.getcell(b'PHASE_DIR', fieldid)
+        tb.close()
 
         if phdirinfo.shape[1] != 1:
-            die ('trying to rephase but target field (#%d) has a '
-                 'time-variable phase center, which I can\'t handle', fieldid)
+            die('trying to rephase but target field (#%d) has a '
+                'time-variable phase center, which I can\'t handle', fieldid)
         ra0, dec0 = phdirinfo[:,0] # in radians.
 
         # based on intflib/pwflux.py, which was copied from
         # hex/hex-lib-calcgainerr:
 
         dra = cfg.rephase[0] - ra0
         dec = cfg.rephase[1]
-        l = np.sin (dra) * np.cos (dec)
-        m = np.sin (dec) * np.cos (dec0) - np.cos (dra) * np.cos (dec) * np.sin (dec0)
-        n = np.sin (dec) * np.sin (dec0) + np.cos (dra) * np.cos (dec) * np.cos (dec0)
+        l = np.sin(dra) * np.cos(dec)
+        m = np.sin(dec) * np.cos(dec0) - np.cos(dra) * np.cos(dec) * np.sin(dec0)
+        n = np.sin(dec) * np.sin(dec0) + np.cos(dra) * np.cos(dec) * np.cos(dec0)
         n -= 1 # makes the work below easier
-        lmn = np.asarray ([l, m, n])
-        colnames.append ('uvw')
+        lmn = np.asarray([l, m, n])
+        colnames.append('uvw')
 
     tbins = {}
     colnames = b(colnames)
 
-    for ddindex, ddid in enumerate (ddids):
+    for ddindex, ddid in enumerate(ddids):
         # Starting in CASA 4.6, selectinit(ddid) stopped actually filtering
         # your data to match the specified DDID! What garbage. Work around
         # with our own filtering.
         ms_sels['taql'] = 'DATA_DESC_ID == %d' % ddid
         ms.msselect(b(ms_sels))
 
-        ms.selectinit (ddid)
+        ms.selectinit(ddid)
         if cfg.polarization is not None:
-            ms.selectpolarization (b(cfg.polarization.split (',')))
-        ms.iterinit (maxrows=4096)
-        ms.iterorigin ()
+            ms.selectpolarization(b(cfg.polarization.split(',')))
+        ms.iterinit(maxrows=4096)
+        ms.iterorigin()
 
         spwid = ddspws[ddid]
 
         while True:
-            cols = ms.getdata (items=colnames)
+            cols = ms.getdata(items=colnames)
 
             if rephase:
                 # With appropriate spw/DDID selection, `freqs` has shape
                 # (nchan, 1). Convert to m^-1 so we can multiply against UVW
                 # directly.
                 freqs = cols['axis_info']['freq_axis']['chan_freq']
                 assert freqs.shape[1] == 1, 'internal inconsistency, chan_freq??'
                 freqs = freqs[:,0] * util.INVERSE_C_MS
 
-            for i in xrange (cols['time'].size): # all records
+            for i in range(cols['time'].size): # all records
                 time = cols['time'][i]
                 # get out of UTC as fast as we can! For some reason
                 # giving 'unit=s' below doesn't do what one might hope it would.
                 # CASA can convert to a variety of timescales; TAI is probably
                 # the safest conversion in terms of being helpful while remaining
                 # close to the fundamental data, but TT is possible and should
                 # be perfectly precise for standard applications.
-                mq = me.epoch (b'utc', b({'value': time / 86400., 'unit': 'd'}))
-                mjdtt = me.measure (b(mq), b'tt')['m0']['value']
+                mq = me.epoch(b'utc', b({'value': time / 86400., 'unit': 'd'}))
+                mjdtt = me.measure(b(mq), b'tt')['m0']['value']
 
-                tdata = tbins.get (mjdtt)
+                tdata = tbins.get(mjdtt)
                 if tdata is None:
-                    tdata = tbins[mjdtt] = np.zeros ((nfreq, 7))
+                    tdata = tbins[mjdtt] = np.zeros((nfreq, 7))
 
                 if rephase:
                     uvw = cols['uvw'][:,i]
-                    ph = np.exp ((0-2j) * np.pi * np.dot (lmn, uvw) * freqs)
+                    ph = np.exp((0-2j) * np.pi * np.dot(lmn, uvw) * freqs)
 
-                for j in xrange (cols['flag'].shape[0]): # all polns
+                for j in range(cols['flag'].shape[0]): # all polns
                     # We just average together all polarizations right now!
                     # (Not actively, but passively by just iterating over them.)
                     data = cols[cfg.datacol][j,:,i]
                     flags = cols['flag'][j,:,i]
 
                     # XXXXX casacore is currently broken and returns the raw
                     # weights from the dataset rather than applying the
                     # polarization selection. Fortunately all of our weights
                     # are the same, and you can never fetch more pol types
                     # than the dataset has, so this bit works despite the bug.
 
-                    w = np.where (~flags)[0]
+                    w = np.where(~flags)[0]
                     if not w.size:
                         continue # all flagged
 
                     if rephase:
                         data *= ph
 
                     m = freqmaps[spwid][w]
@@ -287,64 +288,64 @@
                     tdata[m,1] += wt * d.imag
                     tdata[m,2] += wt * d.real**2
                     tdata[m,3] += wt * d.imag**2
                     tdata[m,4] += wt
                     tdata[m,5] += wt**2
                     tdata[m,6] += 1
 
-            if not ms.iternext ():
+            if not ms.iternext():
                 break
 
         ms.reset() # reset selection filter so we can get next DDID
 
-    ms.close ()
+    ms.close()
 
     # Could gain some efficiency by using a better data structure than a dict().
 
-    smjd = np.asarray (sorted (six.iterkeys (tbins)))
-    data = np.zeros ((5, smjd.size, nfreq))
+    smjd = np.asarray(sorted(six.iterkeys(tbins)))
+    data = np.zeros((5, smjd.size, nfreq))
 
-    for tid in xrange (smjd.size):
+    for tid in range(smjd.size):
         mjd = smjd[tid]
 
         wr, wi, wr2, wi2, wt, wt2, n = tbins[mjd].T
-        w = np.where (n > 0)[0]
-        if w.size == 0:
-            continue # could be all flagged
+        w = np.where(n > 0)[0]
+        if w.size < 3: # not enough data for meaningful statistics
+            continue
 
         r = wr[w] / wt[w]
         i = wi[w] / wt[w]
 
         if cfg.believeweights:
             ru = wt[w]**-0.5
             iu = wt[w]**-0.5
         else:
             r2 = wr2[w] / wt[w]
             i2 = wi2[w] / wt[w]
             rv = r2 - r**2 # variance among real/imag msmts
             iv = i2 - i**2
-            ru = np.sqrt (rv * wt2[w]) / wt[w] # uncert in mean real/img values
-            iu = np.sqrt (iv * wt2[w]) / wt[w]
+            ru = np.sqrt(rv * wt2[w]) / wt[w] # uncert in mean real/img values
+            iu = np.sqrt(iv * wt2[w]) / wt[w]
 
         data[0,tid,w] = r
         data[1,tid,w] = ru
         data[2,tid,w] = i
         data[3,tid,w] = iu
         data[4,tid,w] = n[w]
 
-    np.save (cfg.outstream, smjd)
-    np.save (cfg.outstream, allfreqs)
-    np.save (cfg.outstream, data)
+    np.save(cfg.outstream, smjd)
+    np.save(cfg.outstream, allfreqs)
+    np.save(cfg.outstream, data)
 
 
-def dftdynspec_cli (argv):
-    check_usage (dftdynspec_doc, argv, usageifnoargs=True)
-    cfg = Config ().parse (argv[1:])
-    util.logger (cfg.loglevel)
-    dftdynspec (cfg)
+def dftdynspec_cli(argv):
+    check_usage(dftdynspec_doc, argv, usageifnoargs=True)
+    cfg = Config().parse(argv[1:])
+    util.logger(cfg.loglevel)
+    dftdynspec(cfg)
 
 
 class Loader(object):
     """Read in a dynamic-spectrum file produced by the `dftdynspec` task.
 
     **Constructor arguments**
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_plotcal.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_plotcal.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/environments/casa/cscript_getopacities.py` & `pwkit-1.0.0/pwkit/environments/casa/cscript_getopacities.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 """This file is a casapy script. Do not use it as a module.
 
 It is also useless to run directly via pkcasascript. Use
 `pwkit.environments.casa.tasks.getopacities`.
 
 """
 
-def in_casapy (helper, ms=None, plotdest=None):
+def in_casapy(helper, ms=None, plotdest=None):
     """This function is run inside the weirdo casapy IPython environment! A
     strange set of modules is available, and the
     `pwkit.environments.casa.scripting` system sets up a very particular
     environment to allow encapsulated scripting.
 
     """
-    import numpy as np, os, cPickle as pickle
+    import numpy as np, os
 
     if ms is None:
-        raise ValueError ('ms')
+        raise ValueError('ms')
     if plotdest is None:
-        raise ValueError ('plotdest')
+        raise ValueError('plotdest')
 
-    opac = helper.casans.plotweather (vis=ms, plotName=plotdest)
-    opac = np.asarray (opac)
-    with open (helper.temppath ('opac.npy'), 'wb') as f:
-        pickle.dump (opac, f)
+    opac = helper.casans.plotweather(vis=ms, plotName=plotdest)
+    opac = np.asarray(opac)
+    with open(helper.temppath('opac.npy'), 'wb') as f:
+        np.save(f, opac)
```

### Comparing `pwkit-0.8.9/pwkit/environments/casa/util.py` & `pwkit-1.0.0/pwkit/environments/casa/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 """This module provides low-level tools and utilities for interacting with the
 ``casac`` module provided by CASA.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('''INVERSE_C_MS INVERSE_C_MNS pol_names pol_to_miriad msselect_keys
-                  datadir logger forkandlog sanitize_unicode tools''').split ()
+__all__ = str('''INVERSE_C_MS INVERSE_C_MNS pol_names pol_to_miriad msselect_keys
+datadir logger forkandlog sanitize_unicode tools''').split()
 
 import six
-from ... import binary_type, text_type
+from ... import text_type
 
 # Some constants that can be useful.
 
 INVERSE_C_MS  = 3.3356409519815204e-09 # inverse speed of light in m/s
 INVERSE_C_MNS = 3.3356409519815204 # inverse speed of light in m/ns
 
 pol_names = {
@@ -51,19 +51,19 @@
     30: False, 31: False, 32: False,
 }
 
 # "polarization" is technically valid as an MS selection, but it pretty much
 # doesn't do what you'd want since records generally contain multiple pols.
 # ms.selectpolarization() should be used instead. Maybe ditto for spw?
 
-msselect_keys = frozenset ('array baseline field observation '
-                           'scan scaninent spw taql time uvdist'.split ())
+msselect_keys = frozenset('array baseline field observation '
+                          'scan scaninent spw taql time uvdist'.split())
 
 
-def sanitize_unicode (item):
+def sanitize_unicode(item):
     """Safely pass string values to the CASA tools.
 
     item
       A value to be passed to a CASA tool.
 
     In Python 2, the bindings to CASA tasks expect to receive all string values
     as binary data (:class:`str`) and not Unicode. But :mod:`pwkit` often uses
@@ -74,42 +74,42 @@
     will lead to errors.
 
     This helper function converts Unicode into UTF-8 encoded bytes for
     arguments that you might pass to a CASA tool. It will leave non-strings
     unchanged and recursively transform collections, so you can safely use it
     just about anywhere.
 
-    I usually import this as just ``b`` and write ``tool.method (b(arg))``, in
+    I usually import this as just ``b`` and write ``tool.method(b(arg))``, in
     analogy with the ``b''`` byte string syntax. This leads to code such as::
 
       from pwkit.environments.casa.util import tools, sanitize_unicode as b
 
       tb = tools.table()
       path = u'data.ms'
       tb.open(path) # => raises exception
       tb.open(b(path)) # => works
 
     """
-    if isinstance (item, text_type):
-        return item.encode ('utf8')
-    if isinstance (item, dict):
-        return dict ((sanitize_unicode (k), sanitize_unicode (v)) for k, v in six.iteritems (item))
-    if isinstance (item, (list, tuple)):
-        return item.__class__ (sanitize_unicode (x) for x in item)
+    if isinstance(item, text_type):
+        return item.encode('utf8')
+    if isinstance(item, dict):
+        return dict((sanitize_unicode(k), sanitize_unicode(v)) for k, v in six.iteritems(item))
+    if isinstance(item,(list, tuple)):
+        return item.__class__(sanitize_unicode(x) for x in item)
 
     from ...io import Path
-    if isinstance (item, Path):
-        return binary_type (item)
+    if isinstance(item, Path):
+        return str(item)
 
     return item
 
 
 # Finding the data directory
 
-def datadir (*subdirs):
+def datadir(*subdirs):
     """Get a path within the CASA data directory.
 
     subdirs
       Extra elements to append to the returned path.
 
     This function locates the directory where CASA resource data files (tables
     of time offsets, calibrator models, etc.) are stored. If called with no
@@ -124,60 +124,60 @@
       tb.open(cal_image_path)
 
     """
     import os.path
     data = None
 
     if 'CASAPATH' in os.environ:
-        data = os.path.join (os.environ['CASAPATH'].split ()[0], 'data')
+        data = os.path.join(os.environ['CASAPATH'].split()[0], 'data')
 
     if data is None:
         # The Conda CASA directory layout:
         try:
             import casadef
         except ImportError:
             pass
         else:
-            data = os.path.join (os.path.dirname (casadef.task_directory), 'data')
-            if not os.path.isdir (data):
+            data = os.path.join(os.path.dirname(casadef.task_directory), 'data')
+            if not os.path.isdir(data):
                 # Sigh, hack for CASA 4.7 + Conda; should be straightened out:
                 dn = os.path.dirname
                 data = os.path.join(dn(dn(dn(casadef.task_directory))), 'lib', 'casa', 'data')
-                if not os.path.isdir (data):
+                if not os.path.isdir(data):
                     data = None
 
     if data is None:
         import casac
 
         prevp = None
-        p = os.path.dirname (casac.__file__)
-        while len (p) and p != prevp:
-            data = os.path.join (p, 'data')
-            if os.path.isdir (data):
+        p = os.path.dirname(casac.__file__)
+        while len(p) and p != prevp:
+            data = os.path.join(p, 'data')
+            if os.path.isdir(data):
                 break
             prevp = p
-            p = os.path.dirname (p)
+            p = os.path.dirname(p)
 
-    if not os.path.isdir (data):
-        raise RuntimeError ('cannot identify CASA data directory')
+    if not os.path.isdir(data):
+        raise RuntimeError('cannot identify CASA data directory')
 
-    return os.path.join (data, *subdirs)
+    return os.path.join(data, *subdirs)
 
 
 # Trying to use the logging facility in a sane way.
 #
 # As soon as you create a logsink, it creates a file called casapy.log.
 # So we do some junk to not leave turds all around the filesystem.
 
-def _rmtree_error (func, path, excinfo):
+def _rmtree_error(func, path, excinfo):
     from ...cli import warn
-    warn ('couldn\'t delete temporary file %s: %s (%s)', path, excinfo[0], func)
+    warn('couldn\'t delete temporary file %s: %s (%s)', path, excinfo[0], func)
 
 
-def logger (filter='WARN'):
+def logger(filter='WARN'):
     """Set up CASA to write log messages to standard output.
 
     filter
       The log level filter: less urgent messages will not be shown. Valid values
       are strings: "DEBUG1", "INFO5", ... "INFO1", "INFO", "WARN", "SEVERE".
 
     This function creates and returns a CASA ”log sink” object that is
@@ -186,43 +186,43 @@
     directory; this function safely prevents such a file from being left
     around. This is particularly important if you don’t have write permissions
     to the current directory.
 
     """
     import os, shutil, tempfile
 
-    cwd = os.getcwd ()
+    cwd = os.getcwd()
     tempdir = None
 
     try:
-        tempdir = tempfile.mkdtemp (prefix='casautil')
+        tempdir = tempfile.mkdtemp(prefix='casautil')
 
         try:
-            os.chdir (tempdir)
-            sink = tools.logsink ()
-            sink.setlogfile (sanitize_unicode (os.devnull))
+            os.chdir(tempdir)
+            sink = tools.logsink()
+            sink.setlogfile(sanitize_unicode(os.devnull))
             try:
-                os.unlink ('casapy.log')
+                os.unlink('casapy.log')
             except OSError as e:
                 if e.errno != 2:
                     raise
                 # otherwise, it's a ENOENT, in which case, no worries.
         finally:
-            os.chdir (cwd)
+            os.chdir(cwd)
     finally:
         if tempdir is not None:
-            shutil.rmtree (tempdir, onerror=_rmtree_error)
+            shutil.rmtree(tempdir, onerror=_rmtree_error)
 
-    sink.showconsole (True)
-    sink.setglobal (True)
-    sink.filter (sanitize_unicode (filter.upper ()))
+    sink.showconsole(True)
+    sink.setglobal(True)
+    sink.filter(sanitize_unicode(filter.upper()))
     return sink
 
 
-def forkandlog (function, filter='INFO5', debug=False):
+def forkandlog(function, filter='INFO5', debug=False):
     """Fork a child process and read its CASA log output.
 
     function
       A function to run in the child process
     filter
       The CASA log level filter to apply in the child process: less urgent
       messages will not be shown. Valid values are strings: "DEBUG1", "INFO5",
@@ -253,16 +253,16 @@
     will not pollute the CASA log output. But, by the same token, the calling
     program will not be able to detect that the exception occurred except by
     its impact on the expected log output.
 
     """
     import sys, os
 
-    readfd, writefd = os.pipe ()
-    pid = os.fork ()
+    readfd, writefd = os.pipe()
+    pid = os.fork()
 
     if pid == 0:
         # Child process. We never leave this branch.
         #
         # Log messages of priority >WARN are sent to stderr regardless of the
         # status of log.showconsole(). The idea is for this subprocess to be
         # something super lightweight and constrained, so it seems best to
@@ -271,76 +271,76 @@
         #
         # I thought of using the default logger() setup and dup2'ing stderr to
         # the pipe fd, but then if anything else gets printed to stderr (e.g.
         # Python exception info), it'll get sent along the pipe too. The
         # caller would have to be much more complex to be able to detect and
         # handle such output.
 
-        os.close (readfd)
+        os.close(readfd)
 
         if not debug:
-            f = open (os.devnull, 'w')
-            os.dup2 (f.fileno (), 1)
-            os.dup2 (f.fileno (), 2)
-
-        sink = logger (filter=filter)
-        sink.setlogfile (b'/dev/fd/%d' % writefd)
-        function (sink)
-        sys.exit (0)
+            f = open(os.devnull, 'w')
+            os.dup2(f.fileno(), 1)
+            os.dup2(f.fileno(), 2)
+
+        sink = logger(filter=filter)
+        sink.setlogfile(b'/dev/fd/%d' % writefd)
+        function(sink)
+        sys.exit(0)
 
     # Original process.
 
-    os.close (writefd)
+    os.close(writefd)
 
-    with os.fdopen (readfd) as readhandle:
+    with os.fdopen(readfd) as readhandle:
         for line in readhandle:
             yield line
 
-    info = os.waitpid (pid, 0)
+    info = os.waitpid(pid, 0)
 
     if info[1]:
         # Because we're a generator, this is the only way for us to signal if
         # the process died. We could be rewritten as a context manager.
-        e = RuntimeError ('logging child process PID %d exited '
-                          'with error code %d' % tuple (info))
+        e = RuntimeError('logging child process PID %d exited '
+                         'with error code %d' % tuple(info))
         e.pid, e.exitcode = info
         raise e
 
 
 # Tool factories.
 
-class _Tools (object):
+class _Tools(object):
     """This class is structured so that it supports useful tab-completion
     interactively, but also so that new tools can be constructed if the
     underlying library provides them.
 
     """
     _builtinNames = '''agentflagger atmosphere calanalysis calibrater calplot
                      componentlist coordsys deconvolver fitter flagger
                      functional image imagepol imager logsink measures
                      msmetadata ms msplot mstransformer plotms regionmanager
                      simulator spectralline quanta table tableplot utils
-                     vlafiller vpmanager'''.split ()
+                     vlafiller vpmanager'''.split()
 
-    def __getattribute__ (self, n):
+    def __getattribute__(self, n):
         """Returns factories, not instances."""
         # We need to make this __getattribute__, not __getattr__, only because
         # we set the builtin names in the class __dict__ to enable tab-completion.
         import casac
 
-        if hasattr (casac, 'casac'): # casapy >= 4.0?
-            t = getattr (casac.casac, n, None)
+        if hasattr(casac, 'casac'): # casapy >= 4.0?
+            t = getattr(casac.casac, n, None)
             if t is None:
-                raise AttributeError ('tool "%s" not present' % n)
+                raise AttributeError('tool "%s" not present' % n)
             return t
         else:
             try:
-                return casac.homefinder.find_home_by_name (n + 'Home').create
+                return casac.homefinder.find_home_by_name(n + 'Home').create
             except Exception:
                 # raised exception is class 'homefinder.error'; it appears unavailable
                 # on the Python layer
-                raise AttributeError ('tool "%s" not present' % n)
+                raise AttributeError('tool "%s" not present' % n)
 
 for n in _Tools._builtinNames:
-    setattr (_Tools, n, None) # ease autocompletion
+    setattr(_Tools, n, None) # ease autocompletion
 
-tools = _Tools ()
+tools = _Tools()
```

### Comparing `pwkit-0.8.9/pwkit/parallel.py` & `pwkit-1.0.0/pwkit/parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 must design the parallel part of the function's operation to be implementable
 in terms of the standard library :func:`map` function. Then, give your
 function an optional ``parallel=True`` keyword argument and use the
 :func:`make_parallel_helper` function from this module like so::
 
   from pwkit.parallel import make_parallel_helper
 
-  def my_parallelizable_function (arg1, arg1, parallel=True):
+  def my_parallelizable_function(arg1, arg1, parallel=True):
       # Get a "parallel helper" object that can provide us with a parallelized
       # "map" function. The caller specifies how the parallelization is done;
       # we don't have to know the details.
-      phelp = make_parallel_helper (parallel)
+      phelp = make_parallel_helper(parallel)
       ...
 
       # When used as a context manager, the helper provides a function that
       # acts like the standard library function "map", except it may
       # parallelize its operation.
-      with phelp.get_map () as map:
-         results1 = map (my_subfunc1, subargs1)
+      with phelp.get_map() as map:
+         results1 = map(my_subfunc1, subargs1)
          ...
-         results2 = map (my_subfunc2, subargs2)
+         results2 = map(my_subfunc2, subargs2)
 
       ... do stuff with results1 and results2 ...
 
 Passing ``parallel=True`` to a function defined this way will cause it to
 parallelize ``map`` calls across all cores. Passing ``parallel=0.5`` will
 cause it to use about half your machine. Passing ``parallel=False`` will cause
 it to use serial processing. The helper must be used as a context manager (via
@@ -42,34 +42,35 @@
 instances support a "partially-Pickling" `map`-like function
 :meth:`ParallelHelper.get_ppmap` that works around Pickle-related limitations
 in the :mod:`multiprocessing` library.
 
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-__all__ = str ('make_parallel_helper').split ()
+__all__ = str('make_parallel_helper').split()
 
 import functools, signal
 from multiprocessing.pool import Pool
 from multiprocessing import Process, Queue, TimeoutError
+import six
 from six.moves import range
 
 
-def _initializer_wrapper (actual_initializer, *rest):
+def _initializer_wrapper(actual_initializer, *rest):
     """We ignore SIGINT. It's up to our parent to kill us in the typical condition
     of this arising from ``^C`` on a terminal. If someone is manually killing
     us with that signal, well... nothing will happen.
 
     """
-    signal.signal (signal.SIGINT, signal.SIG_IGN)
+    signal.signal(signal.SIGINT, signal.SIG_IGN)
     if actual_initializer is not None:
-        actual_initializer (*rest)
+        actual_initializer(*rest)
 
 
-class InterruptiblePool (Pool):
+class InterruptiblePool(Pool):
     """A modified version of `multiprocessing.pool.Pool` that has better
     behavior with regard to KeyboardInterrupts in the `map` method. Parameters:
 
     processes
       The number of worker processes to use; defaults to the number of CPUs.
     initializer
       Either None, or a callable that will be invoked by each worker
@@ -93,101 +94,101 @@
 
     This version is a drop-in replacement for multiprocessing.Pool ... as long
     as the map() method is the only one that needs to be interrupt-friendly.
 
     """
     wait_timeout = 3600
 
-    def __init__ (self, processes=None, initializer=None, initargs=(), **kwargs):
-        new_initializer = functools.partial (_initializer_wrapper, initializer)
-        super (InterruptiblePool, self).__init__ (processes, new_initializer,
-                                                  initargs, **kwargs)
+    def __init__(self, processes=None, initializer=None, initargs=(), **kwargs):
+        new_initializer = functools.partial(_initializer_wrapper, initializer)
+        super(InterruptiblePool, self).__init__(processes, new_initializer,
+                                                initargs, **kwargs)
 
 
-    def map (self, func, iterable, chunksize=None):
+    def map(self, func, iterable, chunksize=None):
         """Equivalent of `map` built-in, without swallowing KeyboardInterrupt.
 
         func
           The function to apply to the items.
         iterable
           An iterable of items that will have `func` applied to them.
 
         """
         # The key magic is that we must call r.get() with a timeout, because a
         # Condition.wait() without a timeout swallows KeyboardInterrupts.
-        r = self.map_async (func, iterable, chunksize)
+        r = self.map_async(func, iterable, chunksize)
 
         while True:
             try:
-                return r.get (self.wait_timeout)
+                return r.get(self.wait_timeout)
             except TimeoutError:
                 pass
             except KeyboardInterrupt:
-                self.terminate ()
-                self.join ()
+                self.terminate()
+                self.join()
                 raise
             # Other exceptions propagate up.
 
 
-class ParallelHelper (object):
+class ParallelHelper(object):
     """Object that helps genericize the setup needed for parallel computations.
     Each method returns a context manager that wraps up any resource
     allocation and deallocation that may need to occur to make the
     parallelization happen under the hood.
 
     :class:`ParallelHelper` objects should be obtained by calling
     :func:`make_parallel_helper`, not direct construction, unless you have
     special needs. See the documentation of that function for an example of
     the general usage pattern.
 
     Once you have a :class:`ParallelHelper` instance, usage should be
     something like::
 
-        with phelp.get_map () as map:
-            results_arr = map (my_function, my_args)
+        with phelp.get_map() as map:
+            results_arr = map(my_function, my_args)
 
     The partially-Pickling map works around a limitation in the
     multiprocessing library. This library spawns subprocesses and executes
     parallel tasks by sending them to the subprocesses, which means that the
     data describing the task must be pickle-able. There are hacks so that you
     can pass functions defined in the global namespace but they're pretty much
     useless in production code. The "partially-Pickling map" works around this
     by using a different method that allows some arguments to the map
     operation to avoid being pickled. (Instead, they are directly inherited by
     :func:`os.fork`-ed subprocesses.) See the docs for :func:`serial_ppmap` for
     usage information.
 
     """
-    def get_map (self):
+    def get_map(self):
         """Get a *context manager* that yields a function with the same call signature
         as the standard library function :func:`map`. Its results are the
         same, but it may evaluate the mapped function in parallel across
         multiple threads or processes --- the calling function should not have
         to particularly care about the details. Example usage is::
 
-            with phelp.get_map () as map:
-                results_arr = map (my_function, my_args)
+            with phelp.get_map() as map:
+                results_arr = map(my_function, my_args)
 
         The passed function and its arguments must be Pickle-able. The alternate
         method :meth:`get_ppmap` relaxes this restriction somewhat.
 
         """
-        raise NotImplementedError ('get_map() not available')
+        raise NotImplementedError('get_map() not available')
 
-    def get_ppmap (self):
+    def get_ppmap(self):
         """Get a *context manager* that yields a "partially-pickling map function". It
         can be used to perform a parallelized :func:`map` operation with some
         un-pickle-able arguments.
 
         The yielded function has the signature of :func:`serial_ppmap`. Its
         behavior is functionally equivalent to the following code, except that
         the calls to ``func`` may happen in parallel::
 
-            def ppmap (func, fixed_arg, var_arg_iter):
-                return [func (i, fixed_arg, x) for i, x in enumerate (var_arg_iter)]
+            def ppmap(func, fixed_arg, var_arg_iter):
+                return [func(i, fixed_arg, x) for i, x in enumerate(var_arg_iter)]
 
         The arguments to the ``ppmap`` function are:
 
         *func*
           A callable taking three arguments and returning a Pickle-able value.
         *fixed_arg*
           Any value, even one that is not pickle-able.
@@ -207,182 +208,182 @@
           ``ppmap``.
 
         This variant of the standard :func:`map` function exists to allow the
         parallel-processing system to work around :mod:`pickle`-related
         limitations in the :mod:`multiprocessing` library.
 
         """
-        raise NotImplementedError ('get_ppmap() not available')
+        raise NotImplementedError('get_ppmap() not available')
 
 
-class VacuousContextManager (object):
+class VacuousContextManager(object):
     """A context manager that just returns a static value and doesn't do anything
     clever with exceptions.
 
     """
-    def __init__ (self, value):
+    def __init__(self, value):
         self.value = value
-    def __enter__ (self):
+    def __enter__(self):
         return self.value
-    def __exit__ (self, etype, evalue, etb):
+    def __exit__(self, etype, evalue, etb):
         return False
 
 
-def serial_ppmap (func, fixed_arg, var_arg_iter):
+def serial_ppmap(func, fixed_arg, var_arg_iter):
     """A serial implementation of the "partially-pickling map" function returned
     by the :meth:`ParallelHelper.get_ppmap` interface. Its arguments are:
 
     *func*
       A callable taking three arguments and returning a Pickle-able value.
     *fixed_arg*
       Any value, even one that is not pickle-able.
     *var_arg_iter*
       An iterable that generates Pickle-able values.
 
     The functionality is::
 
-        def serial_ppmap (func, fixed_arg, var_arg_iter):
-            return [func (i, fixed_arg, x) for i, x in enumerate (var_arg_iter)]
+        def serial_ppmap(func, fixed_arg, var_arg_iter):
+            return [func(i, fixed_arg, x) for i, x in enumerate(var_arg_iter)]
 
     Therefore the arguments to your ``func`` function, which actually does the
     interesting computations, are:
 
     *index*
       The 0-based index number of the item being processed; often this can
       be ignored.
     *fixed_arg*
       The same *fixed_arg* that was passed to ``ppmap``.
     *var_arg*
       The *index*'th item in the *var_arg_iter* iterable passed to
       ``ppmap``.
 
     """
-    return [func (i, fixed_arg, x) for i, x in enumerate (var_arg_iter)]
+    return [func(i, fixed_arg, x) for i, x in enumerate(var_arg_iter)]
 
 
-class SerialHelper (ParallelHelper):
+class SerialHelper(ParallelHelper):
     """A :class:`ParallelHelper` that actually does serial processing."""
 
-    def __init__ (self, chunksize=None):
+    def __init__(self, chunksize=None):
         # We accept and discard some of the multiprocessing kwargs that turn
         # into noops so that we can present a uniform API.
         pass
 
-    def get_map (self):
-        return VacuousContextManager (map)
+    def get_map(self):
+        return VacuousContextManager(map)
 
-    def get_ppmap (self):
-        return VacuousContextManager (serial_ppmap)
+    def get_ppmap(self):
+        return VacuousContextManager(serial_ppmap)
 
 
-def multiprocessing_ppmap_worker (in_queue, out_queue, func, fixed_arg):
+def multiprocessing_ppmap_worker(in_queue, out_queue, func, fixed_arg):
     """Worker for the :mod:`multiprocessing` ppmap implementation. Strongly
     derived from code posted on StackExchange by "klaus se":
     `<http://stackoverflow.com/a/16071616/3760486>`_.
 
     """
     while True:
-        i, var_arg = in_queue.get ()
+        i, var_arg = in_queue.get()
         if i is None:
             break
-        out_queue.put ((i, func (i, fixed_arg, var_arg)))
+        out_queue.put((i, func(i, fixed_arg, var_arg)))
 
 
-class MultiprocessingPoolHelper (ParallelHelper):
+class MultiprocessingPoolHelper(ParallelHelper):
     """A :class:`ParallelHelper` that parallelizes computations using Python's
     :class:`multiprocessing.Pool` with a configurable number of processes.
     Actually, we use a wrapped version of :class:`multiprocessing.Pool` that
     handles :exc:`KeyboardInterrupt` exceptions more helpfully.
 
     """
-    class InterruptiblePoolContextManager (object):
-        def __init__ (self, methodname, methodkwargs={}, **kwargs):
+    class InterruptiblePoolContextManager(object):
+        def __init__(self, methodname, methodkwargs={}, **kwargs):
             self.methodname = methodname
             self.methodkwargs = methodkwargs
             self.kwargs = kwargs
 
-        def __enter__ (self):
+        def __enter__(self):
             from functools import partial
-            self.pool = InterruptiblePool (**self.kwargs)
-            func = getattr (self.pool, self.methodname)
-            return partial (func, **self.methodkwargs)
-
-        def __exit__ (self, etype, evalue, etb):
-            self.pool.terminate ()
-            self.pool.join ()
+            self.pool = InterruptiblePool(**self.kwargs)
+            func = getattr(self.pool, self.methodname)
+            return partial(func, **self.methodkwargs)
+
+        def __exit__(self, etype, evalue, etb):
+            self.pool.terminate()
+            self.pool.join()
             return False
 
 
-    def __init__ (self, chunksize=None, **pool_kwargs):
+    def __init__(self, chunksize=None, **pool_kwargs):
         self.chunksize = chunksize
         self.pool_kwargs = pool_kwargs
 
-    def get_map (self):
-        return self.InterruptiblePoolContextManager ('map',
-                                                     {'chunksize': self.chunksize},
-                                                     **self.pool_kwargs)
+    def get_map(self):
+        return self.InterruptiblePoolContextManager('map',
+                                                    {'chunksize': self.chunksize},
+                                                    **self.pool_kwargs)
 
 
-    def _ppmap (self, func, fixed_arg, var_arg_iter):
+    def _ppmap(self, func, fixed_arg, var_arg_iter):
         """The multiprocessing implementation of the partially-Pickling "ppmap"
         function. This doesn't use a Pool like map() does, because the whole
         problem is that Pool chokes on un-Pickle-able values. Strongly derived
         from code posted on StackExchange by "klaus se":
         `<http://stackoverflow.com/a/16071616/3760486>`_.
 
         This implementation could definitely be improved -- that's basically
         what the Pool class is all about -- but this gets us off the ground
         for those cases where the Pickle limitation is important.
 
         XXX This deadlocks if a child process crashes!!! XXX
         """
-        n_procs = self.pool_kwargs.get ('processes')
+        n_procs = self.pool_kwargs.get('processes')
         if n_procs is None:
             # Logic copied from multiprocessing.pool.Pool.__init__()
             try:
                 from multiprocessing import cpu_count
-                n_procs = cpu_count ()
+                n_procs = cpu_count()
             except NotImplementedError:
                 n_procs = 1
 
-        in_queue = Queue (1)
-        out_queue = Queue ()
-        procs = [Process (target=multiprocessing_ppmap_worker,
-                          args=(in_queue, out_queue, func, fixed_arg))
-                 for _ in range (n_procs)]
+        in_queue = Queue(1)
+        out_queue = Queue()
+        procs = [Process(target=multiprocessing_ppmap_worker,
+                         args=(in_queue, out_queue, func, fixed_arg))
+                 for _ in range(n_procs)]
 
         for p in procs:
             p.daemon = True
-            p.start ()
+            p.start()
 
         i = -1
 
-        for i, var_arg in enumerate (var_arg_iter):
-            in_queue.put ((i, var_arg))
+        for i, var_arg in enumerate(var_arg_iter):
+            in_queue.put((i, var_arg))
 
         n_items = i + 1
         result = [None] * n_items
 
         for p in procs:
-            in_queue.put ((None, None))
+            in_queue.put((None, None))
 
-        for _ in range (n_items):
-            i, value = out_queue.get ()
+        for _ in range(n_items):
+            i, value = out_queue.get()
             result[i] = value
 
         for p in procs:
-            p.join ()
+            p.join()
 
         return result
 
-    def get_ppmap (self):
-        return VacuousContextManager (self._ppmap)
+    def get_ppmap(self):
+        return VacuousContextManager(self._ppmap)
 
 
-def make_parallel_helper (parallel_arg, **kwargs):
+def make_parallel_helper(parallel_arg, **kwargs):
     """Return a :class:`ParallelHelper` object that can be used for easy
     parallelization of computations. *parallel_arg* is an object that lets the
     caller easily specify the kind of parallelization they are interested in.
     Allowed values are:
 
     False
       Serial processing only.
@@ -402,23 +403,23 @@
     The ``**kwargs`` are passed on to the appropriate :class:`ParallelHelper`
     constructor, if the caller wants to do something tricky.
 
     Expected usage is::
 
         from pwkit.parallel import make_parallel_helper
 
-        def sub_operation (arg):
+        def sub_operation(arg):
             ... do some computation ...
             return result
 
-        def my_parallelizable_function (arg1, arg2, parallel=True):
-            phelp = make_parallel_helper (parallel)
+        def my_parallelizable_function(arg1, arg2, parallel=True):
+            phelp = make_parallel_helper(parallel)
 
-            with phelp.get_map () as map:
-                op_results = map (sub_operation, args)
+            with phelp.get_map() as map:
+                op_results = map(sub_operation, args)
 
             ... reduce "op_results" in some way ...
             return final_result
 
     This means that ``my_parallelizable_function`` doesn't have to worry about
     all of the various fancy things the caller might want to do in terms of
     special parallel magic.
@@ -429,25 +430,25 @@
     :meth:`ParallelHelper.get_ppmap` variant. This returns a
     "partially-Pickling" map operation --- with a different calling signature
     --- that allows un-Pickle-able values to be used. See the documentation
     for :func:`serial_ppmap` for usage information.
 
     """
     if parallel_arg is True: # note: (True == 1) is True
-        return MultiprocessingPoolHelper (**kwargs)
+        return MultiprocessingPoolHelper(**kwargs)
 
     if parallel_arg is False or parallel_arg == 1:
-        return SerialHelper (**kwargs)
+        return SerialHelper(**kwargs)
 
     if parallel_arg > 0 and parallel_arg < 1:
         from multiprocessing import cpu_count
-        n = int (round (parallel_arg * cpu_count ()))
-        return MultiprocessingPoolHelper (processes=n, **kwargs)
+        n = int(round(parallel_arg * cpu_count()))
+        return MultiprocessingPoolHelper(processes=n, **kwargs)
 
-    if isinstance (parallel_arg, ParallelHelper):
+    if isinstance(parallel_arg, ParallelHelper):
         return parallel_arg
 
-    if isinstance (parallel_arg, (int, long)):
-        return MultiprocessingPoolHelper (processes=parallel_arg, **kwargs)
+    if isinstance(parallel_arg, six.integer_types):
+        return MultiprocessingPoolHelper(processes=parallel_arg, **kwargs)
 
-    raise ValueError ('don\'t understand make_parallel_helper() argument %r'
-                      % parallel_arg)
+    raise ValueError('don\'t understand make_parallel_helper() argument %r'
+                     % parallel_arg)
```

### Comparing `pwkit-0.8.9/pwkit/ndshow_gtk2.py` & `pwkit-1.0.0/pwkit/ndshow_gtk2.py`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/sdss3_filter_responses.fits` & `pwkit-1.0.0/pwkit/data/bandpasses/sdss3_filter_responses.fits`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_2mass_J.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_2mass_J.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_h.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_h.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_4.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_4.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_Mp.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_Mp.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_galex_fuv.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_galex_fuv.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_bessell_UX.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_bessell_UX.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_lbt_lmircam_L.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/swuw1_20041120v106.arf` & `pwkit-1.0.0/pwkit/data/bandpasses/swuw1_20041120v106.arf`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_galex_nuv.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_galex_nuv.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_mearth_ccd715.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_mearth_ccd715.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_2mass_H.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_2mass_H.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/nsfcam_jmk_trans.dat~` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_J.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-WL (Micrometers)	Transmission (%)
 1.5	-0.069444
 1.4998	-0.072506
 1.4996	-0.036984
 1.4994	-0.001541
 1.4992	0.013873
 1.499	-0.016951
 1.4988	-0.049287
```

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_Ks.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_Ks.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_2.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_2.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_1.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_1.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_wise_3.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_wise_3.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_2mass_Ks.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_2mass_Ks.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/pwkit/data/bandpasses/filter_mko_Lp.dat` & `pwkit-1.0.0/pwkit/data/bandpasses/filter_mko_Lp.dat`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/README.rst` & `pwkit-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pwkit-0.8.9/PKG-INFO` & `pwkit-1.0.0/pwkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pwkit
-Version: 0.8.9
+Version: 1.0.0
 Summary: Miscellaneous scientific and astronomical tools
 Home-page: https://github.com/pkgw/pwkit/
 Author: Peter Williams
 Author-email: peter@newton.cx
 License: MIT
 Description: This is a collection of Peter Williams' miscellaneous Python tools. I'm
             packaging them so that other people can install them off of PyPI and run
```

