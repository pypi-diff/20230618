# Comparing `tmp/propeller_design_tools-0.3.5.tar.gz` & `tmp/propeller_design_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propeller_design_tools-0.3.5.tar", last modified: Mon Jun 12 06:22:38 2023, max compression
+gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\.tmp-9op688tp\propeller_design_tools-0.4.0.tar", last modified: Sun Jun 18 00:37:31 2023, max compression
```

## Comparing `propeller_design_tools-0.3.5.tar` & `propeller_design_tools-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,375 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/
--rw-rw-rw-   0        0        0    35128 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     1378 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0       92 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     9237 2023-06-12 05:45:36.000000 propeller_design_tools-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:22:38.390107 propeller_design_tools-0.3.5/propdes/
--rw-rw-rw-   0        0        0      374 2023-06-12 05:36:14.000000 propeller_design_tools-0.3.5/propdes/__init__.py
--rw-rw-rw-   0        0        0    28174 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/airfoil.py
--rw-rw-rw-   0        0        0     4755 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.5/propdes/custom_opengl_classes.py
--rw-rw-rw-   0        0        0    17884 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/foil_ui_classes.py
--rw-rw-rw-   0        0        0    49090 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/funcs.py
--rw-rw-rw-   0        0        0    17339 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/helper_ui_classes.py
--rw-rw-rw-   0        0        0    15821 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      373 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/opt_ui_classes.py
--rw-rw-rw-   0        0        0    10726 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/optimizations.py
--rw-rw-rw-   0        0        0    15171 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36115 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/prop_creation_ui_classes.py
--rw-rw-rw-   0        0        0    52601 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/propeller.py
--rw-rw-rw-   0        0        0    17220 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/radialstation.py
--rw-rw-rw-   0        0        0     1624 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.5/propdes/science_spinbox_class.py
--rw-rw-rw-   0        0        0     3952 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/settings.py
--rw-rw-rw-   0        0        0     5590 2023-06-12 05:56:42.000000 propeller_design_tools-0.3.5/propdes/user_interface.py
--rw-rw-rw-   0        0        0     2749 2023-06-12 05:47:39.000000 propeller_design_tools-0.3.5/propdes/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0       92 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 06:22:38.000000 propeller_design_tools-0.3.5/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:22:38.400289 propeller_design_tools-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      141 2023-06-12 06:22:18.000000 propeller_design_tools-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/
+-rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    51932 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9400 2023-06-18 00:34:26.000000 propeller_design_tools-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/
+-rw-rw-rw-   0        0        0      481 2023-06-18 00:09:35.000000 propeller_design_tools-0.4.0/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28820 2022-05-20 22:03:53.000000 propeller_design_tools-0.4.0/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.4.0/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag35.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag36.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag37.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag38.dat
+-rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/boe103.dat
+-rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/boe106.dat
+-rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50416 2023-04-27 19:31:58.000000 propeller_design_tools-0.4.0/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16315 2023-04-26 19:09:09.000000 propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.4.0/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.4.0/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36995 2022-06-12 01:05:11.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
+-rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
+-rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
+-rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
+-rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
+-rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
+-rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
+-rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53871 2022-06-12 00:41:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.4.0/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.4.0/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.4.0/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      236 2023-06-17 23:50:58.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.4.0/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.4.0/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0    51932 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26656 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1866 2023-06-18 00:37:19.000000 propeller_design_tools-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-06-18 00:23:03.000000 propeller_design_tools-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `propeller_design_tools-0.3.5/LICENSE` & `propeller_design_tools-0.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
+GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `propeller_design_tools-0.3.5/MANIFEST.in` & `propeller_design_tools-0.4.0/MANIFEST.in`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-include propeller_design_tools/supporting_files/*.png
-include propeller_design_tools/supporting_files/*.wav
-include propeller_design_tools/supporting_files/*.txt
-
-include propeller_design_tools/foil_database/*.dat
-include propeller_design_tools/foil_database/*.exe
-
-include propeller_design_tools/prop_database/MyPropeller/blade_profiles/*.txt
-include propeller_design_tools/prop_database/MyPropeller/station_polars/*.polar
-include propeller_design_tools/prop_database/MyPropeller/*.meta
-include propeller_design_tools/prop_database/MyPropeller/*.xrop
-include propeller_design_tools/prop_database/MyPropeller/*.xrr
-
-include propeller_design_tools/prop_database/MyPropeller2/blade_profiles/*.txt
-include propeller_design_tools/prop_database/MyPropeller2/station_polars/*.polar
-include propeller_design_tools/prop_database/MyPropeller2/*.meta
-include propeller_design_tools/prop_database/MyPropeller2/*.xrop
-include propeller_design_tools/prop_database/MyPropeller2/*.xrr
-
-include propeller_design_tools/prop_database/MyPropeller3/blade_profiles/*.txt
-include propeller_design_tools/prop_database/MyPropeller3/station_polars/*.polar
-include propeller_design_tools/prop_database/MyPropeller3/*.meta
-include propeller_design_tools/prop_database/MyPropeller3/*.xrop
-include propeller_design_tools/prop_database/MyPropeller3/*.xrr
-
-include propeller_design_tools/prop_database/*.exe
-
+include propeller_design_tools/supporting_files/*.png
+include propeller_design_tools/supporting_files/*.wav
+include propeller_design_tools/supporting_files/*.txt
+
+include propeller_design_tools/foil_database/*.dat
+include propeller_design_tools/foil_database/*.exe
+
+include propeller_design_tools/prop_database/MyPropeller/blade_profiles/*.txt
+include propeller_design_tools/prop_database/MyPropeller/station_polars/*.polar
+include propeller_design_tools/prop_database/MyPropeller/*.meta
+include propeller_design_tools/prop_database/MyPropeller/*.xrop
+include propeller_design_tools/prop_database/MyPropeller/*.xrr
+
+include propeller_design_tools/prop_database/MyPropeller2/blade_profiles/*.txt
+include propeller_design_tools/prop_database/MyPropeller2/station_polars/*.polar
+include propeller_design_tools/prop_database/MyPropeller2/*.meta
+include propeller_design_tools/prop_database/MyPropeller2/*.xrop
+include propeller_design_tools/prop_database/MyPropeller2/*.xrr
+
+include propeller_design_tools/prop_database/MyPropeller3/blade_profiles/*.txt
+include propeller_design_tools/prop_database/MyPropeller3/station_polars/*.polar
+include propeller_design_tools/prop_database/MyPropeller3/*.meta
+include propeller_design_tools/prop_database/MyPropeller3/*.xrop
+include propeller_design_tools/prop_database/MyPropeller3/*.xrr
+
+include propeller_design_tools/prop_database/*.exe
+
```

### Comparing `propeller_design_tools-0.3.5/README.md` & `propeller_design_tools-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-propeller_design_tools (PDT)
-============================
----
-**Work in progress / incomplete documentation**
-
-Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
-
-Eventually I do plan to create better docs, but for now it's just what you see below and the source code itself.
-
----
-
-Description
-===========
-Python 3.7 package that provides exactly what it sounds 
-like by automating usage of the GPL-licensed 
-CLI-utilities XFOIL and XROTOR.
-
-Both utilities are published by professor Mark Drela (MIT).
-- XFOIL: for arbitrary 2D airfoil analysis
-- XROTOR: for arbitrary propeller design schemes
-
-IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
-currently this source code implements these as executables installed when pip installing this package -> this means if
-you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
-even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
-is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
-
-CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
-fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
-blade cl distribution target option for the first time you ever use this code, and then only venture into other options
-once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
-think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
-which in all honestly I have personally found to not really affect the outputs all that much with the exception
-(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
-of the design very much (< ~5-10 percent in all my experiences).
-
-For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
-you have the code at least generating an output without failing.  My personal favorite solver is obviously the 'vrtx'
-option, but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.
-Thank you all that is my TED talk.
-
-Purpose
-=======
-PDT seeks to provide the user a set of python3 utilities
-that can be used for arbitrary scripting efforts to automate
-usage of both XFOIL and XROTOR while implementing its own 
-unique python3.7-native algorithms to maintain local
-input files, meta files, databases, and results files and
-weave everything together for the user in a simple,
-meaningful way to aid in the initial / investigatory 
-stage of well-behaved propeller designs.
-
-Getting Started
-===============
-Installation
-------------
-`pip install propeller_design_tools`
-
-General Operation
------------------
-`import propeller_design_tools as pdt`
-
-PDT operates on two different "database" directories, defined
-by the user with:
-
-    pdt.set_airfoil_database(path: str)
-    pdt.set_propeller_database(path: str)
-
-**The user must set these two directories at the top 
-of every script right after the imports**
-
-*The airfoil directory will be used to store any foil / 
-XFOIL- related support files, and the propeller directory
-will be used similarly to store any propeller / XROTOR - 
-related support files.*
-
-Pre-Requisite: XFOIL and XROTOR Executables
--------------------------------------------
-(soon this section will be obsolete as I plan to implement a pure-python
-version of both XFOIL and XROTOR in the source code)
-
-In order to utilize any PDT functionality that depends on 
-running XFOIL, the "xfoil.exe" executable file needs to be
-in the user-set "airfoil_database" location. *Current pip 
-installations include the xfoil.exe file in the foil_database,
-there should theoretically be no need to download it manually.*
-
-[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
-
-Likewise, in order to utilize any PDT functionality that
-depends on running XROTOR, the "xrotor.exe" executable file
-needs to be in the user-set "propeller_database" location.
-*Current pip installations include the xrotor.exe file in the 
-default prop_database, there should theoretically be no need to 
-download it manually.*
-
-[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
-*(this is actually a link to "CROTOR", which I find is
-the easiest way to obtain a windows-executable of XROTOR)*
-
-[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
-
-Example Scripts / Workflow
---------------------------
-At a high-level, the current concept for PDT workflow is as 
-follows (after obtaining the required executables and pip-installing 
-the PDT package):
-
-0. Try out the (currently extremely buggy and incomplete) user interface!
-[example0_user_interface.py](
-   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
-   )
-
-   ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
-   ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
-   ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
-
-1. Obtain normalized airfoil coordinate files from
-[UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
--> save these files into the "airfoil_database" directory
-
-
-2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
-populate database data for the desired foil sections -> see 
-[example1_airfoil_analysis.py](
-   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
-   )
-
-   ![ex1-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-1.png)
-   ![ex1-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-2.png)
-
-
-3. Once the required 2D airfoil data is generated, PDT can then be used
-to automatically generate all the required 2D foil definition parameters
-required by XROTOR (these "station parameters" are essentially what 
-allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
-blade geometries) -> see
-[example2_radialstation_creation.py](
-   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
-   )
-
-   ![ex2-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex2-1.png)
-   
-   But this step is also automated & displayed by PDT when the user uses
-the builtin PDT propeller creation function -> see
-[example3_prop_creation.py](
-   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
-   )
-
-   ![ex3-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-1.png)
-
-   NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
-or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
-these are much faster than the (more accurate) 'vrtx' formulation, which you 
-can then move on to.
-
-   ![ex3-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-2.png)
-
-
-4. PDT's Propeller() object instances can generate 3D geometry files 
-including profle xyz coordinate listings, and .stl 3D geometry files -> see
-[example4_stl_generation.py](
-   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
-   )
-
-   ![ex4-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex4-1.png)
-
-Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
-using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
-is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
-
-5. Analyze a given Propeller() instance across a sweep of operating points -> see 
-[example5_prop_analysis.py](
-   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
-   )
-
-   ![ex5-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex5-1.png)
-
-
-6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
-prop design generation by means of maximizing or minimizing a given output / 
-calculated metric based on outputs, optionally taking into account different
-propeller operating points via the ability to define the propeller's "duty-cycle"
--> coming soon! This should elimiate the user's need to even input a value for the
+propeller_design_tools (PDT)
+============================
+---
+**Work in progress / incomplete documentation**
+
+Note: The graphical user interface for this should be functional for Linux users as well very soon!!!
+
+Eventually I do plan to create better docs, but for now it's just what you see below and the source code itself.
+
+---
+
+Description
+===========
+Python 3.7 package that provides exactly what it sounds 
+like by automating usage of the GPL-licensed 
+CLI-utilities XFOIL and XROTOR.
+
+Both utilities are published by professor Mark Drela (MIT).
+- XFOIL: for arbitrary 2D airfoil analysis
+- XROTOR: for arbitrary propeller design schemes
+
+IMPORTANT NOTE: to potentially aid in realizing errors are coming from XFOIL or XROTOR rather than this source code ->
+currently this source code implements these as executables installed when pip installing this package -> this means if
+you are having pip install errors and are on Linux it might be caused by that.  Actually, if you are having any errors,
+even in the GUI, and you are on Linux it might be caused by me not understanding until now much about Linux.  If this 
+is the case and you think you know what is causing the error, please feel free to reach out to me to let me know.
+
+CONTINUED: additionally, very soon I will be implementing a fix to automatically install all dependencies, which should
+fix many issues for Linux users, if not all of the current ones.  I also HIGHLY RECOMMEND to use only the "constant" 
+blade cl distribution target option for the first time you ever use this code, and then only venture into other options
+once you are familiar with the code more and can explain to me even what exactly Mark Drela means by this parameter.  I
+think it's just his way of saying the parameter that controls what you want each target section's operating AoA to be,
+which in all honestly I have personally found to not really affect the outputs all that much with the exception
+(obviously) of what each section's chord length will end up being.  It doesn't seem to impact overall realized efficiency
+of the design very much (< ~5-10 percent in all my experiences).
+
+For this same exact reason, it is also HIGHLY RECOMMENDED to use only the 'grad' or 'pot' solver options until you know
+you have the code at least generating an output without failing.  My personal favorite solver is obviously the 'vrtx'
+option, but XROTOR seems to be much less stable and take much, much longer to arrive at solutions when using 'vrtx'.
+Thank you all that is my TED talk.
+
+Purpose
+=======
+PDT seeks to provide the user a set of python3 utilities
+that can be used for arbitrary scripting efforts to automate
+usage of both XFOIL and XROTOR while implementing its own 
+unique python3.7-native algorithms to maintain local
+input files, meta files, databases, and results files and
+weave everything together for the user in a simple,
+meaningful way to aid in the initial / investigatory 
+stage of well-behaved propeller designs.
+
+Getting Started
+===============
+Installation
+------------
+`pip install propdes`
+
+General Operation
+-----------------
+`import propeller_design_tools as pdt`
+
+PDT operates on two different "database" directories, defined
+by the user with:
+
+    pdt.set_airfoil_database(path: str)
+    pdt.set_propeller_database(path: str)
+
+**The user must set these two directories at the top 
+of every script right after the imports**
+
+*The airfoil directory will be used to store any foil / 
+XFOIL- related support files, and the propeller directory
+will be used similarly to store any propeller / XROTOR - 
+related support files.*
+
+Pre-Requisite: XFOIL and XROTOR Executables
+-------------------------------------------
+(soon this section will be obsolete as I plan to implement a pure-python
+version of both XFOIL and XROTOR in the source code)
+
+In order to utilize any PDT functionality that depends on 
+running XFOIL, the "xfoil.exe" executable file needs to be
+in the user-set "airfoil_database" location. *Current pip 
+installations include the xfoil.exe file in the foil_database,
+there should theoretically be no need to download it manually.*
+
+[XFOIL executable and docs](https://web.mit.edu/drela/Public/web/xfoil/)
+
+Likewise, in order to utilize any PDT functionality that
+depends on running XROTOR, the "xrotor.exe" executable file
+needs to be in the user-set "propeller_database" location.
+*Current pip installations include the xrotor.exe file in the 
+default prop_database, there should theoretically be no need to 
+download it manually.*
+
+[CROTOR executable and docs](http://www.esotec.org/sw/crotor.html#download)
+*(this is actually a link to "CROTOR", which I find is
+the easiest way to obtain a windows-executable of XROTOR)*
+
+[actual XROTOR docs](https://web.mit.edu/drela/Public/web/xrotor/xrotor_doc.txt)
+
+Example Scripts / Workflow
+--------------------------
+At a high-level, the current concept for PDT workflow is as 
+follows (after obtaining the required executables and pip-installing 
+the PDT package):
+
+0. Try out the (currently extremely buggy and incomplete) user interface!
+[example0_user_interface.py](
+https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
+)
+
+   ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
+   ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
+   ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
+
+1. Obtain normalized airfoil coordinate files from
+[UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
+-> save these files into the "airfoil_database" directory
+
+
+2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
+populate database data for the desired foil sections -> see 
+[example1_airfoil_analysis.py](
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
+   )
+
+   ![ex1-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-1.png)
+   ![ex1-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-2.png)
+
+
+3. Once the required 2D airfoil data is generated, PDT can then be used
+to automatically generate all the required 2D foil definition parameters
+required by XROTOR (these "station parameters" are essentially what 
+allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
+blade geometries) -> see
+[example2_radialstation_creation.py](
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
+   )
+
+   ![ex2-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex2-1.png)
+   
+   But this step is also automated & displayed by PDT when the user uses
+the builtin PDT propeller creation function -> see
+[example3_prop_creation.py](
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
+   )
+
+   ![ex3-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-1.png)
+
+   NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
+or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
+these are much faster than the (more accurate) 'vrtx' formulation, which you 
+can then move on to.
+
+   ![ex3-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-2.png)
+
+
+4. PDT's Propeller() object instances can generate 3D geometry files 
+including profle xyz coordinate listings, and .stl 3D geometry files -> see
+[example4_stl_generation.py](
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
+   )
+
+   ![ex4-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex4-1.png)
+
+Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
+using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
+is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
+
+5. Analyze a given Propeller() instance across a sweep of operating points -> see 
+[example5_prop_analysis.py](
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
+   )
+
+   ![ex5-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex5-1.png)
+
+
+6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
+prop design generation by means of maximizing or minimizing a given output / 
+calculated metric based on outputs, optionally taking into account different
+propeller operating points via the ability to define the propeller's "duty-cycle"
+-> coming soon! This should elimiate the user's need to even input a value for the
 desired blade cl distribution altogether.)
```

### Comparing `propeller_design_tools-0.3.5/propdes/airfoil.py` & `propeller_design_tools-0.4.0/propeller_design_tools/airfoil.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,601 +1,601 @@
-import os
-import warnings
-from propdes import funcs
-from propdes.user_io import Error, Info, Warning
-from propdes.settings import get_foil_db
-import matplotlib
-matplotlib.use('TKAgg')
-import matplotlib.pyplot as plt
-import numpy as np
-from scipy.interpolate import griddata, interp1d
-
-
-class Airfoil(object):
-    def __init__(self, name: str, exact_namematch: bool = False, verbose: bool = True):
-        name_in = name
-        if '.' in name_in:
-            name, ext = os.path.splitext(name_in)
-            if not any([ex in ext.lower() for ex in ['.dat', '.txt']]):
-                raise Error('Only files with either ".dat" or ".txt" extensions may be used as airfoil '
-                              'coordinate files ({})'.format(name_in))
-            else:
-                self.name = name
-        else:
-            self.name = name_in
-
-        # check for foil database existence
-        if get_foil_db() is None:
-            raise Error('No airfoil database set -> use "pdt.set_airfoil_database(str)" to set one.')
-
-        # get the airfoil filename, filepath
-        fname = funcs.get_airfoil_file_from_db(self.name, exact_namematch=exact_namematch)
-        if verbose:
-            Info('Found airfoil coordinate file: {}'.format(fname))
-        self.coord_fpath = os.path.join(get_foil_db(), fname)
-
-        name, x_coords, y_coords = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=verbose)
-        _, xc_closed_te, yc_closed_te = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=False,
-                                                                           te_gap_set=0.0)
-        self.filename = os.path.basename(self.coord_fpath)
-        self.x_coords = np.array(x_coords)
-        self.y_coords = np.array(y_coords)
-        self.xc_closed_te = xc_closed_te
-        self.yc_closed_te = yc_closed_te
-
-        self.xfoil_coord_fpath = self.write_xfoil_coord_file()
-        self.polar_data = {}      # dictionary of dictionaries, keys are floats of Re
-        self.rectified_polar_data = {}
-
-        if os.path.exists(self.get_database_savepath()):
-            self.load_polar_data(verbose=verbose)
-
-    @property
-    def xfoil_relpath(self):
-        dr, fname = os.path.split(self.xfoil_coord_fpath)
-        return '/'.join([dr.split('\\')[-1], fname])
-
-    def get_database_savepath(self):
-        database_folder = os.path.join(get_foil_db(), 'polar_database')
-        savename, _ = os.path.splitext(os.path.basename(self.coord_fpath))
-        savepath = os.path.join('{}'.format(database_folder), '{}_polar_data.txt'.format(savename))
-        return savepath
-
-    def write_xfoil_coord_file(self):
-        xfoil_folder = os.path.join(get_foil_db(), 'for_xfoil')
-        if not os.path.exists(xfoil_folder):
-            os.mkdir(xfoil_folder)
-
-        savename, _ = os.path.splitext(os.path.basename(self.coord_fpath))
-        savepath = os.path.join(xfoil_folder, '{}.txt'.format(savename))
-        with open(savepath, 'w') as f:
-            f.write('{}\n\n'.format(self.name))
-            for coord in zip(self.x_coords, self.y_coords):
-                f.write('{x:.7f} {y:.7f}\n'.format(x=coord[0], y=coord[1]))
-        return savepath
-
-    def plot_geometry(self, fig=None, closed_te: bool = False):
-        if fig is None:
-            fig = plt.figure()
-            ax = fig.add_subplot(111)
-        else:
-            ax = fig.axes[0]
-
-        if closed_te:
-            ax.plot(self.xc_closed_te, self.yc_closed_te)
-        else:
-            ax.plot(self.x_coords, self.y_coords)
-
-        ax.set_aspect('equal')
-        ax.grid(True)
-        left, right = ax.get_xlim()
-        ax.set_ylim((left - right / 2), -(left - right / 2))
-        ax.set_title(self.filename)
-
-        return fig
-
-    def alpha_auto_range(self, re: int, ncrit: int, mach: float, verbose: bool = True, xfoil_verbose: bool = False,
-                         hide_windows: bool = True):
-        if verbose:
-            Info('Detecting range for alpha sweep, finding zero-lift angle-of-attack...')
-
-        def find_alpha_CL0():   # function to find zero lift aoa (A0deg)
-            funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[0], ncrit=ncrit, mach=mach,
-                            hide_windows=hide_windows, verbose=xfoil_verbose)
-            xout = funcs.read_xfoil_pacc_file(delete_after=True)
-            if xout is not None:    # just return if xfoil converged 1st try
-                return xout['alpha'][0]
-
-            # otherwise have to get upper and lower points and linearly interpolate
-            cl_lim = 0.02
-            clinc = 0.002
-            cl = 0
-            while xout is None:  # get an upper data point
-                cl += clinc
-                funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[cl], ncrit=ncrit, mach=mach,
-                                keypress_iternum=10, hide_windows=hide_windows, verbose=xfoil_verbose)
-                xout = funcs.read_xfoil_pacc_file(delete_after=True)
-                if xout is None and cl == cl_lim:
-                    err_txt = 'Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re)
-                    raise Error(err_txt)
-            a_up = xout['alpha'][0]
-            cl_up = xout['CL'][0]
-
-            cl = 0
-            xout = None
-            while xout is None:  # get a lower data point
-                cl -= clinc
-                funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[cl], ncrit=ncrit, mach=mach,
-                                keypress_iternum=10, hide_windows=hide_windows, verbose=xfoil_verbose)
-                xout = funcs.read_xfoil_pacc_file(delete_after=True)
-                if xout is None and cl == -cl_lim:
-                    raise Error('Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re))
-
-            a_low = xout['alpha'][0]
-            cl_low = xout['CL'][0]
-
-            da_dcl = (a_up - a_low) / (cl_up - cl_low)
-            dcl = 0 - cl_low
-            A0deg = a_low + dcl * da_dcl
-            return A0deg
-
-        def find_stall_angle(start_a: float = 5, ainc: float = 1.0, max_a: float = 25, press_iter: int = 5,
-                             dclda_threshold: float = 0.0):   # function to find stall angle
-            this_a = start_a - ainc         # initializing
-            this_cl = 0.0                   # initializing
-            aa = []                         # initializing
-            cl = []                         # initializing
-
-            while this_a < max_a:
-                last_a = this_a * 1
-                last_cl = this_cl * 1
-                this_a += ainc
-                funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, alpha=[this_a], ncrit=ncrit, mach=mach,
-                                keypress_iternum=press_iter, hide_windows=hide_windows, verbose=xfoil_verbose)
-                xout = funcs.read_xfoil_pacc_file(delete_after=True)
-                if xout is None:    # when no data was returned (didn't converge)
-                    continue
-                else:   # when data was returned (converged)
-                    this_cl = xout['CL'][0]  # CL value that was returned
-                    if len(aa) > 0:  # if it's not the first iteration, check for criteria
-                        dcl_da = (this_cl - last_cl) / (this_a - last_a)
-                        if dcl_da < dclda_threshold:
-                            return this_a
-                    aa.append(this_a)
-                    cl.append(this_cl)
-
-            if len(aa) > 0:     # made it to a_max, but converged at least once
-                return aa[-1] + 2
-            else:   # made it all the way to max_a without converging
-                # trace_txt = 'Airfoil.alpha_auto_range.find_stall_angle()'
-                # err_txt = 'Unable to find stall angle, max_a reached (foil={}, re={:.0f})'.format(self.name, re)
-                #
-                # info_d = {'func/method': trace_txt, 'Error Text': err_txt, 'dclda_threshold':
-                #     dclda_threshold, 'start_a': start_a, 'ainc': ainc, 'max_a': max_a}
-                # errplot_kwargs = {'x': aa, 'y': cl, 'xlbl': 'alpha (deg)', 'ylbl': 'CL', 'info_d': info_d}
-                # raise Error(err_txt, **errplot_kwargs)
-                return max_a
-
-        # use the functions above
-        zero_lift_aoa = find_alpha_CL0()
-        if verbose:
-            Info('Found alpha_CL0 = {}'.format(zero_lift_aoa), indent_level=1)
-            Info('Approximating stall angle...', indent_level=1)
-        a_stall = find_stall_angle(start_a=zero_lift_aoa + 12)
-        if verbose:
-            Info('Found a_stall = {}'.format(a_stall), indent_level=1)
-        alpha = np.arange(zero_lift_aoa - 1, a_stall + 2.5, 0.5)
-        if verbose:
-            Info('Determined alpha values: {}'.format(alpha))
-
-        return alpha
-
-    def calculate_xfoil_polars(self, hide_windows: bool = True, verbose: bool = True, xfoil_verbose: bool = False,
-                               **kwargs):
-        """
-        Used to interface with XFOIL and save database data.
-
-        :param re_list: Reynolds numbers to iterate across
-        :param alpha: Angle of Attack (AoA) to iterate across.  Defaults to None which attempts to sweep across
-                        the range of alpha values that are required to best characterize the foil's aero properties in
-                        XROTOR (from Zero-lift AoA up to AoA @ stall)
-        :param ncrit: Defaults to 9. From the XFOIL user docs about ncrit ->
-                         situation             Ncrit
-                      -----------------        -----
-                      sailplane                12-14
-                      motorglider              11-13
-                      clean wind tunnel        10-12
-                      average wind tunnel        9     <=  standard "e^9 method"
-                      dirty wind tunnel         4-8
-        :param mach: The Mach number of the flow
-        :param save_to_database: Defaults to True, which automatically makes the results save to the database
-        :return:
-        """
-
-        # KWARG conditioning
-        if 're' in kwargs:
-            re_list = kwargs.pop('re')
-            if not isinstance(re_list, list):
-                re_list = list(re_list)
-        else:
-            raise Error('Must input a value for KWARG "re"')
-
-        if 'alpha' in kwargs:
-            alpha_list = kwargs.pop('alpha')
-            if not isinstance(alpha_list, list):
-                if alpha_list is not None:
-                    alpha_list = list(alpha_list)
-        else:
-            alpha_list = None  # default -> alpha_list=None will trigger alpha-auto range
-
-        if 'ncrit' in kwargs:
-            ncrit_list = kwargs.pop('ncrit')
-            if not isinstance(ncrit_list, list):
-                ncrit_list = list(ncrit_list)
-        else:
-            ncrit_list = [9]  # default
-        for nc in ncrit_list:        # check ncrit in range
-            if nc not in range(4, 15):
-                raise Error('Parameter ncrit must be an integer 4-14 (got {})'.format(nc))
-
-        if 'mach' in kwargs:
-            mach_list = kwargs.pop('mach')
-            if not isinstance(mach_list, list):
-                mach_list = list(mach_list)
-        else:
-            mach_list = [0.0]  # default
-
-        if 'save_to_database' in kwargs:
-            save_to_database = kwargs.pop('save_to_database')
-        else:
-            save_to_database = True  # default
-
-        alpha_in = alpha_list
-        total_count = len(re_list) * len(mach_list) * len(ncrit_list)
-        count = 0
-        for ncrit in ncrit_list:
-            for mach in mach_list:
-                for re in re_list:
-                    count += 1
-                    re = int(re)
-                    if verbose:
-                        print()
-                        Info('Running polar # {} / {} (Re={}, mach={}, ncrit={}) ...'.format(count, total_count, re,
-                                                                                             mach, ncrit))
-
-                    if alpha_in is None:
-                        alpha_list = self.alpha_auto_range(re=re, ncrit=ncrit, mach=mach, verbose=verbose,
-                                                           xfoil_verbose=xfoil_verbose, hide_windows=hide_windows)
-
-                    if verbose:
-                        Info('Running XFOIL for:')
-                        Info('Foil: {}'.format(self.name), indent_level=1)
-                        Info('Re: {}'.format(re), indent_level=1)
-                        Info('Mach: {}'.format(mach), indent_level=1)
-                        Info('Ncrit: {}'.format(ncrit), indent_level=1)
-                        Info('alpha: {}'.format(alpha_list), indent_level=1)
-                    funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, alpha=alpha_list, ncrit=ncrit,
-                                    mach=mach, verbose=xfoil_verbose, hide_windows=hide_windows)
-                    if verbose:
-                        Info('Done')
-
-                    d = funcs.read_xfoil_pacc_file(delete_after=True)
-                    self.polar_data[(re, mach, ncrit)] = d
-
-        # exit method if not saving to database
-        if not save_to_database:
-            return
-
-        # save/append to database, start by making folder if it doesn't already exist
-        database_folder = os.path.join(get_foil_db(), 'polar_database')
-        if not os.path.exists(database_folder):
-            os.mkdir(database_folder)
-            if verbose:
-                Info('Created a "polar_database" to store XFOIL results')
-
-        # savename will be coordinate file name with _polar_data appended
-        savepath = self.get_database_savepath()
-
-        # append/overwrite data if file exists already, otherwise write data to a new file
-        if os.path.exists(savepath):
-            if verbose:
-                Info('Detected existing polar data for "{}" -> merging datasets'.format(self.name))
-            old_polar_data = funcs.read_polar_data_file(fpath=savepath)
-            merged = funcs.merge_polar_data_dicts(new=self.polar_data.copy(), old=old_polar_data)
-            os.remove(savepath)
-            funcs.save_polar_data_file(polar_data=merged, savepath=savepath, name=self.name)
-        else:
-            funcs.save_polar_data_file(polar_data=self.polar_data, savepath=savepath, name=self.name)
-        if verbose:
-            Info('Saved new polar data for "{}"'.format(self.name))
-
-    def get_valid_xfoil_params(self):
-        return ['alpha', 'CL', 'CD', 'CDp', 'CM', 'Top_Xtr', 'Bot_Xtr', 'CL/CD']
-
-    def plot_polar_data(self, x_param: str, y_param: str, re_list: list = None, mach_list: list = None,
-                        ncrit_list: list = None, xlims: tuple = None, ylims: tuple = None, rectified: bool = False,
-                        rect_kwargs: dict = {}, fig=None, **plot_kwargs):
-        """
-        Method to plot existing polar data.
-
-        :param x_param: the dictionary key for the x-axis data to plot.  Options are alpha, CL, CD, CDp, CM, Top_Xtr,
-            Bot_Xtr -> all directly returned from XFOIL, and CL/CD -> calculated by PDT.
-        :param y_param: the dictionary key for the y-axis data to plot.  Options are alpha, CL, CD, CDp, CM, Top_Xtr,
-            Bot_Xtr -> all directly returned from XFOIL, and CL/CD -> calculated by PDT.
-        :param re_list: list of reynolds numbers to plot. If given None, will plot all existing re.
-        :param mach_list: list of machs to plot.  If given None, will plot all existing mach.
-        :param ncrit_list: list of ncrits to plot.  If given None, will plot all existing ncrit.
-        :param xlims: 2-tuple of (xmin, xmax) for the plot
-        :param ylims: 2-tuple of (ymin, ymax) for the plot
-        :param rectified: bool, whether or not to plot the raw grid data, or rectify it first and plot that data
-        :param rect_kwargs: dictionary, the key-word arguments to pass along to rectify_polar_grids
-
-        :return fig: the pyplot.fig instance of the plot
-        :return ax: the pyplot.axes instance of the plot
-        """
-        if x_param not in self.get_valid_xfoil_params() or y_param not in self.get_valid_xfoil_params():
-            raise Error('"{}" is not a valid polar parameter combo for plotting'.
-                          format('({}, {})'.format(x_param, y_param)))
-
-        pol_data = self.polar_data
-        if rectified:
-            self.rectify_polar_grids(rect_kwargs=rect_kwargs)
-            pol_data = self.rectified_polar_data
-
-        if len(pol_data) == 0:
-            raise Error('No polar data to plot for "{}"! Use "calculate_xfoil_polars()" first'.format(self.name))
-
-        if 'marker' not in plot_kwargs:
-            plot_kwargs['marker'] = 'o'
-
-        # get the grid of polar lookup keys for the associated polar data
-        re_l, mach_l, ncrit_l = self.get_polar_data_grid()
-
-        # if a polar lookup key isn't given, plot all data across that lookup key by default
-        if re_list is None:
-            re_list = re_l
-        if mach_list is None:
-            mach_list = mach_l
-        if ncrit_list is None:
-            ncrit_list = ncrit_l
-
-        # enforce that the user input valid values
-        re_list = list(sorted([int(r) for r in re_list]))
-        mach_list = list(sorted([float(m) for m in mach_list]))
-        ncrit_list = list(sorted([int(n) for n in ncrit_list]))
-
-        # create figure and axes instance
-        if fig is None:
-            fig = plt.figure(figsize=(10, 8))
-            ax = fig.add_subplot(111)
-            subpl_adj_rt = 0.81
-        else:
-            ax = fig.axes[0]
-            subpl_adj_rt = 0.77
-
-        # plot em
-        for re_key in re_list:
-            plot_kwargs['c'] = plt.cm.jet(re_list.index(re_key) / len(re_list))
-            for mach_key in mach_list:
-                if max(mach_list) == 0:
-                    plot_kwargs['alpha'] = 1
-                else:
-                    plot_kwargs['alpha'] = 1.0 - mach_key / max(mach_list) / 2
-
-                for ncrit_key in ncrit_list:
-                    marker_cycle = ['o', 'v', '^', '<', '>', 's', '+', 'd', '2']
-                    plot_kwargs['marker'] = marker_cycle[ncrit_list.index(ncrit_key) % len(marker_cycle)]
-                    if (re_key, mach_key, ncrit_key) in pol_data.keys():
-                        d = pol_data[(re_key, mach_key, ncrit_key)]
-                        ax.plot(d[x_param], d[y_param], label='{:.1e}, {}, {}'.format(re_key, mach_key, ncrit_key), **plot_kwargs)
-                    else:
-                        Warning('Cannot find polar for {} @ Re = {}, Mach = {}, Ncrit = {}, skipping this one...'
-                                .format(self.name, re_key, mach_key, ncrit_key))
-
-        ax.grid(True)
-        ax.set_title('{}\nrectified={}'.format(self.filename, rectified))
-        ax.set_xlabel(x_param)
-        ax.set_ylabel(y_param)
-        if ylims is not None:
-            ax.set_ylim(ylims)
-        if xlims is not None:
-            ax.set_xlim(xlims)
-        ax.legend(loc='upper left', title='Re, Mach, Ncrit', bbox_to_anchor=(1.01, 1.0))
-        fig.subplots_adjust(left=0.09, right=subpl_adj_rt)
-
-        return fig, ax
-
-    def get_polar_data_grid(self):
-        re_list, mach_list, ncrit_list = [], [], []
-        for key in self.polar_data.keys():
-            re_list.append(key[0])
-            mach_list.append(key[1])
-            ncrit_list.append(key[2])
-        return list(sorted(set(re_list))), list(sorted(set(mach_list))), list(sorted(set(ncrit_list)))
-
-    def get_keys_2_interpolate(self):
-        k = self.get_valid_xfoil_params()
-        k.pop(k.index('CL/CD'))
-        return k
-
-    def rectify_polar_grids(self, **kwargs):
-        if not self.rectified_polar_data == {}:
-            return
-
-        if 'interp_kind' in kwargs:
-            interp_kind = kwargs.pop('interp_kind')
-        else:
-            interp_kind = 'linear'
-
-        rect_polar_data = self.polar_data.copy()
-
-        keys2rect = self.get_keys_2_interpolate()
-        if 'alpha' in keys2rect:
-            keys2rect.pop(keys2rect.index('alpha'))
-
-        alpha_mins = [np.min(pol['alpha']) for pol in rect_polar_data.values()]
-        alpha_maxes = [np.max(pol['alpha']) for pol in rect_polar_data.values()]
-
-        alpha_rect = np.linspace(np.min(alpha_mins), np.max(alpha_maxes), 50)
-        for pol in rect_polar_data.values():
-            for key in keys2rect:
-                ydata = pol[key]
-                pol_interpolator = interp1d(x=pol['alpha'], y=ydata, kind=interp_kind, fill_value='extrapolate')
-                with warnings.catch_warnings():
-                    warnings.simplefilter("ignore")
-                    pol[key] = pol_interpolator(alpha_rect)
-
-            pol['alpha'] = alpha_rect
-
-        self.rectified_polar_data = rect_polar_data
-
-    def interpolate_polar(self, npts: int, re: int, mach: float, ncrit: int, griddata_kwargs: dict = {}):
-        # check for inside convex hull of known (Re, Mach, nCrit) grid points
-        res, machs, ncrits = self.get_polar_data_grid()
-        if re > max(res) or re < min(res):
-            raise Error('Cannot interpolate a polar @ re value outside database limits (re={:.0f})'.format(re))
-        if mach > max(machs) or re < min(machs):
-            raise Error('Cannot interpolate a polar @ mach value outside database limits (mach={:.2f})'.format(mach))
-        if ncrit > max(ncrits) or re < min(ncrits):
-            raise Error('Cannot interpolate a polar @ ncrit value outside database limits (ncrit={:.0f})'.format(ncrit))
-
-        if 'method' not in griddata_kwargs:
-            griddata_kwargs['method'] = 'linear'
-        if 'rescale' not in griddata_kwargs:
-            griddata_kwargs['rescale'] = True
-
-        # send em right back if their desired polar is one of the grid points
-        if (re, mach, ncrit) in self.polar_data:
-            return self.polar_data[(re, mach, ncrit)].copy()
-
-        # rectify polar grids <-- what does this do again???
-        self.rectify_polar_grids(interp_kind='linear')
-
-        # get all the keys to interpolate, will interpolate across 2D planes of x=alpha, y=key
-        keys2interp = self.get_keys_2_interpolate()
-
-        # flatten values across database Re, mach, ncrit
-        flat_vals = {k: np.array([]) for k in keys2interp}
-        re_pts, mach_pts, ncrit_pts = [], [], []
-        for pol_key, pol in self.rectified_polar_data.items():
-            re_pts.extend([pol_key[0]] * len(pol['alpha']))
-            mach_pts.extend([pol_key[1]] * len(pol['alpha']))
-            ncrit_pts.extend([pol_key[2]] * len(pol['alpha']))
-            for key in keys2interp:
-                new_vals = np.append(flat_vals[key], pol[key].flatten())
-                flat_vals[key] = new_vals
-
-        alphas = flat_vals.pop('alpha')
-        keys2interp.pop(keys2interp.index('alpha'))
-        pol_interp = {}
-        alpha_interp = np.linspace(np.min(alphas), np.max(alphas), npts)
-        pol_interp['alpha'] = alpha_interp
-
-        if len(machs) == 1 and len(ncrits) == 1:    # if there's only 1 mach and 1 ncrit datapoint
-            points = np.full(shape=(len(alphas), 2), fill_value=np.nan)
-            points[:, 0] = np.array(re_pts)
-            points[:, -1] = alphas
-
-            pol_interp['re'] = re
-            pol_interp['mach'] = machs[0]
-            pol_interp['ncrit'] = ncrits[0]
-
-            for key in keys2interp:
-                values = flat_vals[key]
-                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
-                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
-                xi = np.hstack([re_interp, alpha_interp])
-                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
-
-        elif len(machs) == 1:    # so there's data across re and ncrit but only 1 mach
-            points = np.full(shape=(len(alphas), 3), fill_value=np.nan)
-            points[:, 0] = np.array(re_pts)
-            points[:, 1] = np.array(ncrit_pts)
-            points[:, -1] = alphas
-
-            pol_interp['re'] = re
-            pol_interp['mach'] = machs[0]
-            pol_interp['ncrit'] = ncrit
-
-            for key in keys2interp:
-                values = flat_vals[key]
-                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
-                ncrit_interp = np.ones(shape=(len(alpha_interp), 1)) * ncrit
-                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
-                xi = np.hstack([re_interp, ncrit_interp, alpha_interp])
-                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
-
-        elif len(ncrits) == 1:    # there's data across re and machs but only 1 ncrit
-            points = np.full(shape=(len(alphas), 3), fill_value=np.nan)
-            points[:, 0] = np.array(re_pts)
-            points[:, 1] = np.array(mach_pts)
-            points[:, -1] = alphas
-
-            pol_interp['re'] = re
-            pol_interp['mach'] = mach
-            pol_interp['ncrit'] = ncrits[0]
-
-            for key in keys2interp:
-                values = flat_vals[key]
-                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
-                mach_interp = np.ones(shape=(len(alpha_interp), 1)) * mach
-                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
-                xi = np.hstack([re_interp, mach_interp, alpha_interp])
-                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
-
-        elif len(res) > 1 and len(machs) > 1 and len(ncrits) > 1:   # there's data across all of res, machs, and ncrits
-            points = np.full(shape=(len(alphas), 4), fill_value=np.nan)
-            points[:, 0] = np.array(re_pts)
-            points[:, 1] = np.array(mach_pts)
-            points[:, 2] = np.array(ncrit_pts)
-            points[:, -1] = alphas
-
-            pol_interp['re'] = re
-            pol_interp['mach'] = mach
-            pol_interp['ncrit'] = ncrit
-
-            for key in keys2interp:
-                values = flat_vals[key]
-                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
-                mach_interp = np.ones(shape=(len(alpha_interp), 1)) * mach
-                ncrit_interp = np.ones(shape=(len(alpha_interp), 1)) * ncrit
-                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
-                xi = np.hstack([re_interp, mach_interp, ncrit_interp, alpha_interp])
-                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
-
-        scrubbed_pol = funcs.scrub_nans(d=pol_interp)
-        return scrubbed_pol
-
-    def load_polar_data(self, verbose: bool = True):
-        savepath = self.get_database_savepath()
-        if os.path.exists(savepath):
-            self.polar_data = funcs.read_polar_data_file(fpath=savepath)
-            re, mach, ncrit = self.get_polar_data_grid()
-            if verbose:
-                Info('Loaded existing polar data for "{}":'.format(self.name))
-                Info('Re={}\nMach={}\nNcrit={}'.format(re, mach, ncrit), indent_level=1)
-        else:
-            raise Error('Could not find polar data file: {}'.format(savepath))
-
-    def get_coords(self, n_interp: int = None):
-        if n_interp is None:
-            return np.vstack([self.x_coords, self.y_coords])
-        else:
-            raise Error('Code to interpolate more profile points is incomplete...')
-
-    def get_coords_closed_te(self, n_interp: int = None):
-        if n_interp is None:
-            return np.vstack([self.xc_closed_te, self.yc_closed_te])
-        else:
-            raise Error('Code to interpolate more profile points is incomplete...')
-
-    def plot_2D_trimesh(self):
-        fig = self.plot_geometry()
-        ax = fig.axes[0]
-
-        vectors = funcs.compute_profile_trimesh(profile_coords=self.get_coords())
-        for vector in vectors:
-            pt1, pt2, pt3 = vector
-            ax.plot([pt1[0], pt2[0]], [pt1[1], pt2[1]], color='r', ls='--', marker='o')
-            ax.plot([pt2[0], pt3[0]], [pt2[1], pt3[1]], color='r', ls='--', marker='o')
-            ax.plot([pt3[0], pt1[0]], [pt3[1], pt1[1]], color='r', ls='--', marker='o')
-
+import os
+import warnings
+from propeller_design_tools import funcs
+from propeller_design_tools.user_io import Error, Info, Warning
+from propeller_design_tools.settings import get_foil_db
+import matplotlib
+matplotlib.use('TKAgg')
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy.interpolate import griddata, interp1d
+
+
+class Airfoil(object):
+    def __init__(self, name: str, exact_namematch: bool = False, verbose: bool = True):
+        name_in = name
+        if '.' in name_in:
+            name, ext = os.path.splitext(name_in)
+            if not any([ex in ext.lower() for ex in ['.dat', '.txt']]):
+                raise Error('Only files with either ".dat" or ".txt" extensions may be used as airfoil '
+                              'coordinate files ({})'.format(name_in))
+            else:
+                self.name = name
+        else:
+            self.name = name_in
+
+        # check for foil database existence
+        if get_foil_db() is None:
+            raise Error('No airfoil database set -> use "pdt.set_airfoil_database(str)" to set one.')
+
+        # get the airfoil filename, filepath
+        fname = funcs.get_airfoil_file_from_db(self.name, exact_namematch=exact_namematch)
+        if verbose:
+            Info('Found airfoil coordinate file: {}'.format(fname))
+        self.coord_fpath = os.path.join(get_foil_db(), fname)
+
+        name, x_coords, y_coords = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=verbose)
+        _, xc_closed_te, yc_closed_te = funcs.read_airfoil_coordinate_file(fpath=self.coord_fpath, verbose=False,
+                                                                           te_gap_set=0.0)
+        self.filename = os.path.basename(self.coord_fpath)
+        self.x_coords = np.array(x_coords)
+        self.y_coords = np.array(y_coords)
+        self.xc_closed_te = xc_closed_te
+        self.yc_closed_te = yc_closed_te
+
+        self.xfoil_coord_fpath = self.write_xfoil_coord_file()
+        self.polar_data = {}      # dictionary of dictionaries, keys are floats of Re
+        self.rectified_polar_data = {}
+
+        if os.path.exists(self.get_database_savepath()):
+            self.load_polar_data(verbose=verbose)
+
+    @property
+    def xfoil_relpath(self):
+        dr, fname = os.path.split(self.xfoil_coord_fpath)
+        return '/'.join([dr.split('\\')[-1], fname])
+
+    def get_database_savepath(self):
+        database_folder = os.path.join(get_foil_db(), 'polar_database')
+        savename, _ = os.path.splitext(os.path.basename(self.coord_fpath))
+        savepath = os.path.join('{}'.format(database_folder), '{}_polar_data.txt'.format(savename))
+        return savepath
+
+    def write_xfoil_coord_file(self):
+        xfoil_folder = os.path.join(get_foil_db(), 'for_xfoil')
+        if not os.path.exists(xfoil_folder):
+            os.mkdir(xfoil_folder)
+
+        savename, _ = os.path.splitext(os.path.basename(self.coord_fpath))
+        savepath = os.path.join(xfoil_folder, '{}.txt'.format(savename))
+        with open(savepath, 'w') as f:
+            f.write('{}\n\n'.format(self.name))
+            for coord in zip(self.x_coords, self.y_coords):
+                f.write('{x:.7f} {y:.7f}\n'.format(x=coord[0], y=coord[1]))
+        return savepath
+
+    def plot_geometry(self, fig=None, closed_te: bool = False):
+        if fig is None:
+            fig = plt.figure()
+            ax = fig.add_subplot(111)
+        else:
+            ax = fig.axes[0]
+
+        if closed_te:
+            ax.plot(self.xc_closed_te, self.yc_closed_te)
+        else:
+            ax.plot(self.x_coords, self.y_coords)
+
+        ax.set_aspect('equal')
+        ax.grid(True)
+        left, right = ax.get_xlim()
+        ax.set_ylim((left - right / 2), -(left - right / 2))
+        ax.set_title(self.filename)
+
+        return fig
+
+    def alpha_auto_range(self, re: int, ncrit: int, mach: float, verbose: bool = True, xfoil_verbose: bool = False,
+                         hide_windows: bool = True):
+        if verbose:
+            Info('Detecting range for alpha sweep, finding zero-lift angle-of-attack...')
+
+        def find_alpha_CL0():   # function to find zero lift aoa (A0deg)
+            funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[0], ncrit=ncrit, mach=mach,
+                            hide_windows=hide_windows, verbose=xfoil_verbose)
+            xout = funcs.read_xfoil_pacc_file(delete_after=True)
+            if xout is not None:    # just return if xfoil converged 1st try
+                return xout['alpha'][0]
+
+            # otherwise have to get upper and lower points and linearly interpolate
+            cl_lim = 0.02
+            clinc = 0.002
+            cl = 0
+            while xout is None:  # get an upper data point
+                cl += clinc
+                funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[cl], ncrit=ncrit, mach=mach,
+                                keypress_iternum=10, hide_windows=hide_windows, verbose=xfoil_verbose)
+                xout = funcs.read_xfoil_pacc_file(delete_after=True)
+                if xout is None and cl == cl_lim:
+                    err_txt = 'Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re)
+                    raise Error(err_txt)
+            a_up = xout['alpha'][0]
+            cl_up = xout['CL'][0]
+
+            cl = 0
+            xout = None
+            while xout is None:  # get a lower data point
+                cl -= clinc
+                funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, cl=[cl], ncrit=ncrit, mach=mach,
+                                keypress_iternum=10, hide_windows=hide_windows, verbose=xfoil_verbose)
+                xout = funcs.read_xfoil_pacc_file(delete_after=True)
+                if xout is None and cl == -cl_lim:
+                    raise Error('Unable to find alpha @ CL0 (foil={}, re={:.0f})'.format(self.name, re))
+
+            a_low = xout['alpha'][0]
+            cl_low = xout['CL'][0]
+
+            da_dcl = (a_up - a_low) / (cl_up - cl_low)
+            dcl = 0 - cl_low
+            A0deg = a_low + dcl * da_dcl
+            return A0deg
+
+        def find_stall_angle(start_a: float = 5, ainc: float = 1.0, max_a: float = 25, press_iter: int = 5,
+                             dclda_threshold: float = 0.0):   # function to find stall angle
+            this_a = start_a - ainc         # initializing
+            this_cl = 0.0                   # initializing
+            aa = []                         # initializing
+            cl = []                         # initializing
+
+            while this_a < max_a:
+                last_a = this_a * 1
+                last_cl = this_cl * 1
+                this_a += ainc
+                funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, alpha=[this_a], ncrit=ncrit, mach=mach,
+                                keypress_iternum=press_iter, hide_windows=hide_windows, verbose=xfoil_verbose)
+                xout = funcs.read_xfoil_pacc_file(delete_after=True)
+                if xout is None:    # when no data was returned (didn't converge)
+                    continue
+                else:   # when data was returned (converged)
+                    this_cl = xout['CL'][0]  # CL value that was returned
+                    if len(aa) > 0:  # if it's not the first iteration, check for criteria
+                        dcl_da = (this_cl - last_cl) / (this_a - last_a)
+                        if dcl_da < dclda_threshold:
+                            return this_a
+                    aa.append(this_a)
+                    cl.append(this_cl)
+
+            if len(aa) > 0:     # made it to a_max, but converged at least once
+                return aa[-1] + 2
+            else:   # made it all the way to max_a without converging
+                # trace_txt = 'Airfoil.alpha_auto_range.find_stall_angle()'
+                # err_txt = 'Unable to find stall angle, max_a reached (foil={}, re={:.0f})'.format(self.name, re)
+                #
+                # info_d = {'func/method': trace_txt, 'Error Text': err_txt, 'dclda_threshold':
+                #     dclda_threshold, 'start_a': start_a, 'ainc': ainc, 'max_a': max_a}
+                # errplot_kwargs = {'x': aa, 'y': cl, 'xlbl': 'alpha (deg)', 'ylbl': 'CL', 'info_d': info_d}
+                # raise Error(err_txt, **errplot_kwargs)
+                return max_a
+
+        # use the functions above
+        zero_lift_aoa = find_alpha_CL0()
+        if verbose:
+            Info('Found alpha_CL0 = {}'.format(zero_lift_aoa), indent_level=1)
+            Info('Approximating stall angle...', indent_level=1)
+        a_stall = find_stall_angle(start_a=zero_lift_aoa + 12)
+        if verbose:
+            Info('Found a_stall = {}'.format(a_stall), indent_level=1)
+        alpha = np.arange(zero_lift_aoa - 1, a_stall + 2.5, 0.5)
+        if verbose:
+            Info('Determined alpha values: {}'.format(alpha))
+
+        return alpha
+
+    def calculate_xfoil_polars(self, hide_windows: bool = True, verbose: bool = True, xfoil_verbose: bool = False,
+                               **kwargs):
+        """
+        Used to interface with XFOIL and save database data.
+
+        :param re_list: Reynolds numbers to iterate across
+        :param alpha: Angle of Attack (AoA) to iterate across.  Defaults to None which attempts to sweep across
+                        the range of alpha values that are required to best characterize the foil's aero properties in
+                        XROTOR (from Zero-lift AoA up to AoA @ stall)
+        :param ncrit: Defaults to 9. From the XFOIL user docs about ncrit ->
+                         situation             Ncrit
+                      -----------------        -----
+                      sailplane                12-14
+                      motorglider              11-13
+                      clean wind tunnel        10-12
+                      average wind tunnel        9     <=  standard "e^9 method"
+                      dirty wind tunnel         4-8
+        :param mach: The Mach number of the flow
+        :param save_to_database: Defaults to True, which automatically makes the results save to the database
+        :return:
+        """
+
+        # KWARG conditioning
+        if 're' in kwargs:
+            re_list = kwargs.pop('re')
+            if not isinstance(re_list, list):
+                re_list = list(re_list)
+        else:
+            raise Error('Must input a value for KWARG "re"')
+
+        if 'alpha' in kwargs:
+            alpha_list = kwargs.pop('alpha')
+            if not isinstance(alpha_list, list):
+                if alpha_list is not None:
+                    alpha_list = list(alpha_list)
+        else:
+            alpha_list = None  # default -> alpha_list=None will trigger alpha-auto range
+
+        if 'ncrit' in kwargs:
+            ncrit_list = kwargs.pop('ncrit')
+            if not isinstance(ncrit_list, list):
+                ncrit_list = list(ncrit_list)
+        else:
+            ncrit_list = [9]  # default
+        for nc in ncrit_list:        # check ncrit in range
+            if nc not in range(4, 15):
+                raise Error('Parameter ncrit must be an integer 4-14 (got {})'.format(nc))
+
+        if 'mach' in kwargs:
+            mach_list = kwargs.pop('mach')
+            if not isinstance(mach_list, list):
+                mach_list = list(mach_list)
+        else:
+            mach_list = [0.0]  # default
+
+        if 'save_to_database' in kwargs:
+            save_to_database = kwargs.pop('save_to_database')
+        else:
+            save_to_database = True  # default
+
+        alpha_in = alpha_list
+        total_count = len(re_list) * len(mach_list) * len(ncrit_list)
+        count = 0
+        for ncrit in ncrit_list:
+            for mach in mach_list:
+                for re in re_list:
+                    count += 1
+                    re = int(re)
+                    if verbose:
+                        print()
+                        Info('Running polar # {} / {} (Re={}, mach={}, ncrit={}) ...'.format(count, total_count, re,
+                                                                                             mach, ncrit))
+
+                    if alpha_in is None:
+                        alpha_list = self.alpha_auto_range(re=re, ncrit=ncrit, mach=mach, verbose=verbose,
+                                                           xfoil_verbose=xfoil_verbose, hide_windows=hide_windows)
+
+                    if verbose:
+                        Info('Running XFOIL for:')
+                        Info('Foil: {}'.format(self.name), indent_level=1)
+                        Info('Re: {}'.format(re), indent_level=1)
+                        Info('Mach: {}'.format(mach), indent_level=1)
+                        Info('Ncrit: {}'.format(ncrit), indent_level=1)
+                        Info('alpha: {}'.format(alpha_list), indent_level=1)
+                    funcs.run_xfoil(foil_relpath=self.xfoil_relpath, re=re, alpha=alpha_list, ncrit=ncrit,
+                                    mach=mach, verbose=xfoil_verbose, hide_windows=hide_windows)
+                    if verbose:
+                        Info('Done')
+
+                    d = funcs.read_xfoil_pacc_file(delete_after=True)
+                    self.polar_data[(re, mach, ncrit)] = d
+
+        # exit method if not saving to database
+        if not save_to_database:
+            return
+
+        # save/append to database, start by making folder if it doesn't already exist
+        database_folder = os.path.join(get_foil_db(), 'polar_database')
+        if not os.path.exists(database_folder):
+            os.mkdir(database_folder)
+            if verbose:
+                Info('Created a "polar_database" to store XFOIL results')
+
+        # savename will be coordinate file name with _polar_data appended
+        savepath = self.get_database_savepath()
+
+        # append/overwrite data if file exists already, otherwise write data to a new file
+        if os.path.exists(savepath):
+            if verbose:
+                Info('Detected existing polar data for "{}" -> merging datasets'.format(self.name))
+            old_polar_data = funcs.read_polar_data_file(fpath=savepath)
+            merged = funcs.merge_polar_data_dicts(new=self.polar_data.copy(), old=old_polar_data)
+            os.remove(savepath)
+            funcs.save_polar_data_file(polar_data=merged, savepath=savepath, name=self.name)
+        else:
+            funcs.save_polar_data_file(polar_data=self.polar_data, savepath=savepath, name=self.name)
+        if verbose:
+            Info('Saved new polar data for "{}"'.format(self.name))
+
+    def get_valid_xfoil_params(self):
+        return ['alpha', 'CL', 'CD', 'CDp', 'CM', 'Top_Xtr', 'Bot_Xtr', 'CL/CD']
+
+    def plot_polar_data(self, x_param: str, y_param: str, re_list: list = None, mach_list: list = None,
+                        ncrit_list: list = None, xlims: tuple = None, ylims: tuple = None, rectified: bool = False,
+                        rect_kwargs: dict = {}, fig=None, **plot_kwargs):
+        """
+        Method to plot existing polar data.
+
+        :param x_param: the dictionary key for the x-axis data to plot.  Options are alpha, CL, CD, CDp, CM, Top_Xtr,
+            Bot_Xtr -> all directly returned from XFOIL, and CL/CD -> calculated by PDT.
+        :param y_param: the dictionary key for the y-axis data to plot.  Options are alpha, CL, CD, CDp, CM, Top_Xtr,
+            Bot_Xtr -> all directly returned from XFOIL, and CL/CD -> calculated by PDT.
+        :param re_list: list of reynolds numbers to plot. If given None, will plot all existing re.
+        :param mach_list: list of machs to plot.  If given None, will plot all existing mach.
+        :param ncrit_list: list of ncrits to plot.  If given None, will plot all existing ncrit.
+        :param xlims: 2-tuple of (xmin, xmax) for the plot
+        :param ylims: 2-tuple of (ymin, ymax) for the plot
+        :param rectified: bool, whether or not to plot the raw grid data, or rectify it first and plot that data
+        :param rect_kwargs: dictionary, the key-word arguments to pass along to rectify_polar_grids
+
+        :return fig: the pyplot.fig instance of the plot
+        :return ax: the pyplot.axes instance of the plot
+        """
+        if x_param not in self.get_valid_xfoil_params() or y_param not in self.get_valid_xfoil_params():
+            raise Error('"{}" is not a valid polar parameter combo for plotting'.
+                          format('({}, {})'.format(x_param, y_param)))
+
+        pol_data = self.polar_data
+        if rectified:
+            self.rectify_polar_grids(rect_kwargs=rect_kwargs)
+            pol_data = self.rectified_polar_data
+
+        if len(pol_data) == 0:
+            raise Error('No polar data to plot for "{}"! Use "calculate_xfoil_polars()" first'.format(self.name))
+
+        if 'marker' not in plot_kwargs:
+            plot_kwargs['marker'] = 'o'
+
+        # get the grid of polar lookup keys for the associated polar data
+        re_l, mach_l, ncrit_l = self.get_polar_data_grid()
+
+        # if a polar lookup key isn't given, plot all data across that lookup key by default
+        if re_list is None:
+            re_list = re_l
+        if mach_list is None:
+            mach_list = mach_l
+        if ncrit_list is None:
+            ncrit_list = ncrit_l
+
+        # enforce that the user input valid values
+        re_list = list(sorted([int(r) for r in re_list]))
+        mach_list = list(sorted([float(m) for m in mach_list]))
+        ncrit_list = list(sorted([int(n) for n in ncrit_list]))
+
+        # create figure and axes instance
+        if fig is None:
+            fig = plt.figure(figsize=(10, 8))
+            ax = fig.add_subplot(111)
+            subpl_adj_rt = 0.81
+        else:
+            ax = fig.axes[0]
+            subpl_adj_rt = 0.77
+
+        # plot em
+        for re_key in re_list:
+            plot_kwargs['c'] = plt.cm.jet(re_list.index(re_key) / len(re_list))
+            for mach_key in mach_list:
+                if max(mach_list) == 0:
+                    plot_kwargs['alpha'] = 1
+                else:
+                    plot_kwargs['alpha'] = 1.0 - mach_key / max(mach_list) / 2
+
+                for ncrit_key in ncrit_list:
+                    marker_cycle = ['o', 'v', '^', '<', '>', 's', '+', 'd', '2']
+                    plot_kwargs['marker'] = marker_cycle[ncrit_list.index(ncrit_key) % len(marker_cycle)]
+                    if (re_key, mach_key, ncrit_key) in pol_data.keys():
+                        d = pol_data[(re_key, mach_key, ncrit_key)]
+                        ax.plot(d[x_param], d[y_param], label='{:.1e}, {}, {}'.format(re_key, mach_key, ncrit_key), **plot_kwargs)
+                    else:
+                        Warning('Cannot find polar for {} @ Re = {}, Mach = {}, Ncrit = {}, skipping this one...'
+                                .format(self.name, re_key, mach_key, ncrit_key))
+
+        ax.grid(True)
+        ax.set_title('{}\nrectified={}'.format(self.filename, rectified))
+        ax.set_xlabel(x_param)
+        ax.set_ylabel(y_param)
+        if ylims is not None:
+            ax.set_ylim(ylims)
+        if xlims is not None:
+            ax.set_xlim(xlims)
+        ax.legend(loc='upper left', title='Re, Mach, Ncrit', bbox_to_anchor=(1.01, 1.0))
+        fig.subplots_adjust(left=0.09, right=subpl_adj_rt)
+
+        return fig, ax
+
+    def get_polar_data_grid(self):
+        re_list, mach_list, ncrit_list = [], [], []
+        for key in self.polar_data.keys():
+            re_list.append(key[0])
+            mach_list.append(key[1])
+            ncrit_list.append(key[2])
+        return list(sorted(set(re_list))), list(sorted(set(mach_list))), list(sorted(set(ncrit_list)))
+
+    def get_keys_2_interpolate(self):
+        k = self.get_valid_xfoil_params()
+        k.pop(k.index('CL/CD'))
+        return k
+
+    def rectify_polar_grids(self, **kwargs):
+        if not self.rectified_polar_data == {}:
+            return
+
+        if 'interp_kind' in kwargs:
+            interp_kind = kwargs.pop('interp_kind')
+        else:
+            interp_kind = 'linear'
+
+        rect_polar_data = self.polar_data.copy()
+
+        keys2rect = self.get_keys_2_interpolate()
+        if 'alpha' in keys2rect:
+            keys2rect.pop(keys2rect.index('alpha'))
+
+        alpha_mins = [np.min(pol['alpha']) for pol in rect_polar_data.values()]
+        alpha_maxes = [np.max(pol['alpha']) for pol in rect_polar_data.values()]
+
+        alpha_rect = np.linspace(np.min(alpha_mins), np.max(alpha_maxes), 50)
+        for pol in rect_polar_data.values():
+            for key in keys2rect:
+                ydata = pol[key]
+                pol_interpolator = interp1d(x=pol['alpha'], y=ydata, kind=interp_kind, fill_value='extrapolate')
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore")
+                    pol[key] = pol_interpolator(alpha_rect)
+
+            pol['alpha'] = alpha_rect
+
+        self.rectified_polar_data = rect_polar_data
+
+    def interpolate_polar(self, npts: int, re: int, mach: float, ncrit: int, griddata_kwargs: dict = {}):
+        # check for inside convex hull of known (Re, Mach, nCrit) grid points
+        res, machs, ncrits = self.get_polar_data_grid()
+        if re > max(res) or re < min(res):
+            raise Error('Cannot interpolate a polar @ re value outside database limits (re={:.0f})'.format(re))
+        if mach > max(machs) or re < min(machs):
+            raise Error('Cannot interpolate a polar @ mach value outside database limits (mach={:.2f})'.format(mach))
+        if ncrit > max(ncrits) or re < min(ncrits):
+            raise Error('Cannot interpolate a polar @ ncrit value outside database limits (ncrit={:.0f})'.format(ncrit))
+
+        if 'method' not in griddata_kwargs:
+            griddata_kwargs['method'] = 'linear'
+        if 'rescale' not in griddata_kwargs:
+            griddata_kwargs['rescale'] = True
+
+        # send em right back if their desired polar is one of the grid points
+        if (re, mach, ncrit) in self.polar_data:
+            return self.polar_data[(re, mach, ncrit)].copy()
+
+        # rectify polar grids <-- what does this do again???
+        self.rectify_polar_grids(interp_kind='linear')
+
+        # get all the keys to interpolate, will interpolate across 2D planes of x=alpha, y=key
+        keys2interp = self.get_keys_2_interpolate()
+
+        # flatten values across database Re, mach, ncrit
+        flat_vals = {k: np.array([]) for k in keys2interp}
+        re_pts, mach_pts, ncrit_pts = [], [], []
+        for pol_key, pol in self.rectified_polar_data.items():
+            re_pts.extend([pol_key[0]] * len(pol['alpha']))
+            mach_pts.extend([pol_key[1]] * len(pol['alpha']))
+            ncrit_pts.extend([pol_key[2]] * len(pol['alpha']))
+            for key in keys2interp:
+                new_vals = np.append(flat_vals[key], pol[key].flatten())
+                flat_vals[key] = new_vals
+
+        alphas = flat_vals.pop('alpha')
+        keys2interp.pop(keys2interp.index('alpha'))
+        pol_interp = {}
+        alpha_interp = np.linspace(np.min(alphas), np.max(alphas), npts)
+        pol_interp['alpha'] = alpha_interp
+
+        if len(machs) == 1 and len(ncrits) == 1:    # if there's only 1 mach and 1 ncrit datapoint
+            points = np.full(shape=(len(alphas), 2), fill_value=np.nan)
+            points[:, 0] = np.array(re_pts)
+            points[:, -1] = alphas
+
+            pol_interp['re'] = re
+            pol_interp['mach'] = machs[0]
+            pol_interp['ncrit'] = ncrits[0]
+
+            for key in keys2interp:
+                values = flat_vals[key]
+                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
+                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
+                xi = np.hstack([re_interp, alpha_interp])
+                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
+
+        elif len(machs) == 1:    # so there's data across re and ncrit but only 1 mach
+            points = np.full(shape=(len(alphas), 3), fill_value=np.nan)
+            points[:, 0] = np.array(re_pts)
+            points[:, 1] = np.array(ncrit_pts)
+            points[:, -1] = alphas
+
+            pol_interp['re'] = re
+            pol_interp['mach'] = machs[0]
+            pol_interp['ncrit'] = ncrit
+
+            for key in keys2interp:
+                values = flat_vals[key]
+                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
+                ncrit_interp = np.ones(shape=(len(alpha_interp), 1)) * ncrit
+                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
+                xi = np.hstack([re_interp, ncrit_interp, alpha_interp])
+                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
+
+        elif len(ncrits) == 1:    # there's data across re and machs but only 1 ncrit
+            points = np.full(shape=(len(alphas), 3), fill_value=np.nan)
+            points[:, 0] = np.array(re_pts)
+            points[:, 1] = np.array(mach_pts)
+            points[:, -1] = alphas
+
+            pol_interp['re'] = re
+            pol_interp['mach'] = mach
+            pol_interp['ncrit'] = ncrits[0]
+
+            for key in keys2interp:
+                values = flat_vals[key]
+                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
+                mach_interp = np.ones(shape=(len(alpha_interp), 1)) * mach
+                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
+                xi = np.hstack([re_interp, mach_interp, alpha_interp])
+                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
+
+        elif len(res) > 1 and len(machs) > 1 and len(ncrits) > 1:   # there's data across all of res, machs, and ncrits
+            points = np.full(shape=(len(alphas), 4), fill_value=np.nan)
+            points[:, 0] = np.array(re_pts)
+            points[:, 1] = np.array(mach_pts)
+            points[:, 2] = np.array(ncrit_pts)
+            points[:, -1] = alphas
+
+            pol_interp['re'] = re
+            pol_interp['mach'] = mach
+            pol_interp['ncrit'] = ncrit
+
+            for key in keys2interp:
+                values = flat_vals[key]
+                re_interp = np.ones(shape=(len(alpha_interp), 1)) * re
+                mach_interp = np.ones(shape=(len(alpha_interp), 1)) * mach
+                ncrit_interp = np.ones(shape=(len(alpha_interp), 1)) * ncrit
+                alpha_interp = np.reshape(alpha_interp, (len(alpha_interp), 1))
+                xi = np.hstack([re_interp, mach_interp, ncrit_interp, alpha_interp])
+                pol_interp[key] = griddata(points=points, values=values, xi=xi, **griddata_kwargs)
+
+        scrubbed_pol = funcs.scrub_nans(d=pol_interp)
+        return scrubbed_pol
+
+    def load_polar_data(self, verbose: bool = True):
+        savepath = self.get_database_savepath()
+        if os.path.exists(savepath):
+            self.polar_data = funcs.read_polar_data_file(fpath=savepath)
+            re, mach, ncrit = self.get_polar_data_grid()
+            if verbose:
+                Info('Loaded existing polar data for "{}":'.format(self.name))
+                Info('Re={}\nMach={}\nNcrit={}'.format(re, mach, ncrit), indent_level=1)
+        else:
+            raise Error('Could not find polar data file: {}'.format(savepath))
+
+    def get_coords(self, n_interp: int = None):
+        if n_interp is None:
+            return np.vstack([self.x_coords, self.y_coords])
+        else:
+            raise Error('Code to interpolate more profile points is incomplete...')
+
+    def get_coords_closed_te(self, n_interp: int = None):
+        if n_interp is None:
+            return np.vstack([self.xc_closed_te, self.yc_closed_te])
+        else:
+            raise Error('Code to interpolate more profile points is incomplete...')
+
+    def plot_2D_trimesh(self):
+        fig = self.plot_geometry()
+        ax = fig.axes[0]
+
+        vectors = funcs.compute_profile_trimesh(profile_coords=self.get_coords())
+        for vector in vectors:
+            pt1, pt2, pt3 = vector
+            ax.plot([pt1[0], pt2[0]], [pt1[1], pt2[1]], color='r', ls='--', marker='o')
+            ax.plot([pt2[0], pt3[0]], [pt2[1], pt3[1]], color='r', ls='--', marker='o')
+            ax.plot([pt3[0], pt1[0]], [pt3[1], pt1[1]], color='r', ls='--', marker='o')
+
```

### Comparing `propeller_design_tools-0.3.5/propdes/custom_opengl_classes.py` & `propeller_design_tools-0.4.0/propeller_design_tools/custom_opengl_classes.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from pyqtgraph.Qt import QtCore, QtGui
-import pyqtgraph.opengl as gl
-from pyqtgraph.opengl.GLGraphicsItem import GLGraphicsItem
-import OpenGL.GL as ogl
-import numpy as np
-
-
-class Custom3DAxis(gl.GLAxisItem):
-    """Class defined to extend 'gl.GLAxisItem'."""
-    def __init__(self, parent, color=(0,0,0,.6)):
-        # gl.GLAxisItem.__init__(self)
-        super(Custom3DAxis, self).__init__()
-        self.parent = parent
-        self.c = color
-
-    def add_labels(self, xlbl: str = None, ylbl: str = None, zlbl: str = None):
-        """Adds axes labels."""
-        x,y,z = self.size()
-        #X label
-        if xlbl is not None:
-            self.xLabel = gl.GLTextItem(pos=(x/2, -y/3, -z/20), text=xlbl)
-            self.parent.addItem(self.xLabel)
-        #Y label
-        if ylbl is not None:
-            self.yLabel = gl.GLTextItem(pos=(-x/3, y/2, -z/20), text=ylbl)
-            self.parent.addItem(self.yLabel)
-        #Z label
-        if zlbl is not None:
-            self.zLabel = gl.GLTextItem(pos=(-x/3, -y/3, z/2), text=zlbl)
-            self.parent.addItem(self.zLabel)
-
-    def add_tick_values(self, xticks=[], yticks=[], zticks=[]):
-        """Adds ticks values."""
-        x,y,z = self.size()
-        xtpos = np.linspace(0, x, len(xticks))
-        ytpos = np.linspace(0, y, len(yticks))
-        ztpos = np.linspace(0, z, len(zticks))
-        #X label
-        for i, xt in enumerate(xticks):
-            val = gl.GLTextItem(pos=(xtpos[i], -y/20, -z/20), text='{:.1f}'.format(xt))
-            self.parent.addItem(val)
-        #Y label
-        for i, yt in enumerate(yticks):
-            val = gl.GLTextItem(pos=(-x/20, ytpos[i], -z/20), text='{:.1f}'.format(yt))
-            self.parent.addItem(val)
-        #Z label
-        for i, zt in enumerate(zticks):
-            val = gl.GLTextItem(pos=(-x/20, -y/20, ztpos[i]), text='{:.1f}'.format(zt))
-            self.parent.addItem(val)
-
-    def paint(self):
-        self.setupGLState()
-        if self.antialias:
-            ogl.glEnable(ogl.GL_LINE_SMOOTH)
-            ogl.glHint(ogl.GL_LINE_SMOOTH_HINT, ogl.GL_NICEST)
-        ogl.glBegin(ogl.GL_LINES)
-
-        x,y,z = self.size()
-        #Draw Z
-        ogl.glColor4f(self.c[0], self.c[1], self.c[2], self.c[3])
-        ogl.glVertex3f(0, 0, 0)
-        ogl.glVertex3f(0, 0, z)
-        #Draw Y
-        ogl.glColor4f(self.c[0], self.c[1], self.c[2], self.c[3])
-        ogl.glVertex3f(0, 0, 0)
-        ogl.glVertex3f(0, y, 0)
-        #Draw X
-        ogl.glColor4f(self.c[0], self.c[1], self.c[2], self.c[3])
-        ogl.glVertex3f(0, 0, 0)
-        ogl.glVertex3f(x, 0, 0)
-        ogl.glEnd()
-
-
-class Custom3DArrow(GLGraphicsItem):
-    def __init__(self, view: gl.GLViewWidget, color: tuple = (0, 0, 1, 1), width: int = 2, length: float = None, tip_root: list = None):
-        super(Custom3DArrow, self).__init__()
-        self.view = view
-
-        if length is None and tip_root is None:
-            length = 1
-
-        if length is None:
-            assert len(tip_root) == 2
-            xtip, ytip, ztip = tip_root[0]
-            xroot, yroot, zroot = tip_root[1]
-            length = np.sqrt((xtip - xroot) ** 2 + (ytip - yroot) ** 2 + (ztip - zroot) ** 2)
-        else:
-            xtip, ytip, ztip = 0, 0, 0
-            xroot, yroot, zroot = 0, 0, -length
-            tip_root = [[xtip, ytip, ztip], [xroot, yroot, zroot]]
-        dx, dy, dz = [tip - root for tip, root in zip([xtip, ytip, ztip], [xroot, yroot, zroot])]
-        shaft_root = [xroot, yroot, zroot]
-        shaft_tip = [xroot + 0.75 * dx, yroot + 0.75 * dy, zroot + 0.75 * dz]
-
-        self.shaft = gl.GLLinePlotItem(pos=[shaft_root, shaft_tip], color=color, width=width, antialias=False, mode='line_strip', glOptions='opaque')
-        tip_length, tip_width = 0.25 * length, 0.08 * length
-        tip = gl.MeshData.cylinder(rows=2, cols=15, radius=[tip_width, 0.001 * tip_width], length=tip_length,
-                                   offset=False)
-        self.tip_mesh = gl.GLMeshItem(meshdata=tip, smooth=True, color=color, shader='shaded', glOptions='opaque')
-        self.view.addItem(self.shaft)
-        self.view.addItem(self.tip_mesh)
-
-        x_deg = np.rad2deg(np.arctan2(-dy, dz))
-        y_deg = np.rad2deg(np.arctan2(dx, -dz))
-        self.tip_mesh.translate(dx=0, dy=0, dz=-tip_length)
-        self.tip_mesh.rotate(x_deg, 1, 0, 0)
-        self.tip_mesh.rotate(y_deg, 0, 1, 0)
-        self.tip_mesh.translate(dx=xtip, dy=ytip, dz=ztip)
-
-    def translate(self, dx, dy, dz, local=False):
-        self.shaft.translate(dx, dy, dz, local=local)
-        self.tip_mesh.translate(dx, dy, dz, local=local)
-
-    def rotate(self, angle, x, y, z, local=False):
-        self.shaft.rotate(angle, x, y, z, local=local)
-        self.tip_mesh.rotate(angle, x, y, z, local=local)
+from pyqtgraph.Qt import QtCore, QtGui
+import pyqtgraph.opengl as gl
+from pyqtgraph.opengl.GLGraphicsItem import GLGraphicsItem
+import OpenGL.GL as ogl
+import numpy as np
+
+
+class Custom3DAxis(gl.GLAxisItem):
+    """Class defined to extend 'gl.GLAxisItem'."""
+    def __init__(self, parent, color=(0,0,0,.6)):
+        # gl.GLAxisItem.__init__(self)
+        super(Custom3DAxis, self).__init__()
+        self.parent = parent
+        self.c = color
+
+    def add_labels(self, xlbl: str = None, ylbl: str = None, zlbl: str = None):
+        """Adds axes labels."""
+        x,y,z = self.size()
+        #X label
+        if xlbl is not None:
+            self.xLabel = gl.GLTextItem(pos=(x/2, -y/3, -z/20), text=xlbl)
+            self.parent.addItem(self.xLabel)
+        #Y label
+        if ylbl is not None:
+            self.yLabel = gl.GLTextItem(pos=(-x/3, y/2, -z/20), text=ylbl)
+            self.parent.addItem(self.yLabel)
+        #Z label
+        if zlbl is not None:
+            self.zLabel = gl.GLTextItem(pos=(-x/3, -y/3, z/2), text=zlbl)
+            self.parent.addItem(self.zLabel)
+
+    def add_tick_values(self, xticks=[], yticks=[], zticks=[]):
+        """Adds ticks values."""
+        x,y,z = self.size()
+        xtpos = np.linspace(0, x, len(xticks))
+        ytpos = np.linspace(0, y, len(yticks))
+        ztpos = np.linspace(0, z, len(zticks))
+        #X label
+        for i, xt in enumerate(xticks):
+            val = gl.GLTextItem(pos=(xtpos[i], -y/20, -z/20), text='{:.1f}'.format(xt))
+            self.parent.addItem(val)
+        #Y label
+        for i, yt in enumerate(yticks):
+            val = gl.GLTextItem(pos=(-x/20, ytpos[i], -z/20), text='{:.1f}'.format(yt))
+            self.parent.addItem(val)
+        #Z label
+        for i, zt in enumerate(zticks):
+            val = gl.GLTextItem(pos=(-x/20, -y/20, ztpos[i]), text='{:.1f}'.format(zt))
+            self.parent.addItem(val)
+
+    def paint(self):
+        self.setupGLState()
+        if self.antialias:
+            ogl.glEnable(ogl.GL_LINE_SMOOTH)
+            ogl.glHint(ogl.GL_LINE_SMOOTH_HINT, ogl.GL_NICEST)
+        ogl.glBegin(ogl.GL_LINES)
+
+        x,y,z = self.size()
+        #Draw Z
+        ogl.glColor4f(self.c[0], self.c[1], self.c[2], self.c[3])
+        ogl.glVertex3f(0, 0, 0)
+        ogl.glVertex3f(0, 0, z)
+        #Draw Y
+        ogl.glColor4f(self.c[0], self.c[1], self.c[2], self.c[3])
+        ogl.glVertex3f(0, 0, 0)
+        ogl.glVertex3f(0, y, 0)
+        #Draw X
+        ogl.glColor4f(self.c[0], self.c[1], self.c[2], self.c[3])
+        ogl.glVertex3f(0, 0, 0)
+        ogl.glVertex3f(x, 0, 0)
+        ogl.glEnd()
+
+
+class Custom3DArrow(GLGraphicsItem):
+    def __init__(self, view: gl.GLViewWidget, color: tuple = (0, 0, 1, 1), width: int = 2, length: float = None, tip_root: list = None):
+        super(Custom3DArrow, self).__init__()
+        self.view = view
+
+        if length is None and tip_root is None:
+            length = 1
+
+        if length is None:
+            assert len(tip_root) == 2
+            xtip, ytip, ztip = tip_root[0]
+            xroot, yroot, zroot = tip_root[1]
+            length = np.sqrt((xtip - xroot) ** 2 + (ytip - yroot) ** 2 + (ztip - zroot) ** 2)
+        else:
+            xtip, ytip, ztip = 0, 0, 0
+            xroot, yroot, zroot = 0, 0, -length
+            tip_root = [[xtip, ytip, ztip], [xroot, yroot, zroot]]
+        dx, dy, dz = [tip - root for tip, root in zip([xtip, ytip, ztip], [xroot, yroot, zroot])]
+        shaft_root = [xroot, yroot, zroot]
+        shaft_tip = [xroot + 0.75 * dx, yroot + 0.75 * dy, zroot + 0.75 * dz]
+
+        self.shaft = gl.GLLinePlotItem(pos=[shaft_root, shaft_tip], color=color, width=width, antialias=False, mode='line_strip', glOptions='opaque')
+        tip_length, tip_width = 0.25 * length, 0.08 * length
+        tip = gl.MeshData.cylinder(rows=2, cols=15, radius=[tip_width, 0.001 * tip_width], length=tip_length,
+                                   offset=False)
+        self.tip_mesh = gl.GLMeshItem(meshdata=tip, smooth=True, color=color, shader='shaded', glOptions='opaque')
+        self.view.addItem(self.shaft)
+        self.view.addItem(self.tip_mesh)
+
+        x_deg = np.rad2deg(np.arctan2(-dy, dz))
+        y_deg = np.rad2deg(np.arctan2(dx, -dz))
+        self.tip_mesh.translate(dx=0, dy=0, dz=-tip_length)
+        self.tip_mesh.rotate(x_deg, 1, 0, 0)
+        self.tip_mesh.rotate(y_deg, 0, 1, 0)
+        self.tip_mesh.translate(dx=xtip, dy=ytip, dz=ztip)
+
+    def translate(self, dx, dy, dz, local=False):
+        self.shaft.translate(dx, dy, dz, local=local)
+        self.tip_mesh.translate(dx, dy, dz, local=local)
+
+    def rotate(self, angle, x, y, z, local=False):
+        self.shaft.rotate(angle, x, y, z, local=local)
+        self.tip_mesh.rotate(angle, x, y, z, local=local)
```

### Comparing `propeller_design_tools-0.3.5/propdes/foil_ui_classes.py` & `propeller_design_tools-0.4.0/propeller_design_tools/foil_ui_classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,434 +1,434 @@
-from propdes.funcs import delete_all_widgets_from_layout, get_all_airfoil_files, clear_foil_database, \
-    download_foil_coordinates
-from propdes.airfoil import Airfoil
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-import numpy as np
-try:
-    from PyQt5 import QtWidgets, QtCore
-    from propdes.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_PushButton, PDT_ComboBox, \
-        PDT_CheckBox, PDT_LineEdit
-    from propdes.helper_ui_classes import RangeLineEditWidget, SingleAxCanvas, AxesComboBoxWidget, \
-        Capturing
-except:
-    pass
-
-
-class FoilAnalysisWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(FoilAnalysisWidget, self).__init__()
-        self.main_win = main_win
-
-        # airfoil group
-        af_lay = QtWidgets.QHBoxLayout()
-        self.setLayout(af_lay)
-        af_left_lay = QtWidgets.QVBoxLayout()
-        af_lay.addLayout(af_left_lay)
-        af_center_lay = QtWidgets.QVBoxLayout()
-        af_lay.addLayout(af_center_lay)
-        af_right_lay = QtWidgets.QVBoxLayout()
-        af_lay.addLayout(af_right_lay)
-
-        # airfoil left
-        af_left_lay.addStretch()
-        self.exist_data_widg = ExistingFoilDataWidget(main_win=self.main_win)
-        af_left_lay.addWidget(self.exist_data_widg)
-        af_left_lay.addStretch()
-        self.add_foil_data_widg = AddFoilDataPointWidget(main_win=self.main_win)
-        af_left_lay.addWidget(self.add_foil_data_widg)
-        af_left_lay.addStretch()
-
-        # airfoil center
-        af_center_top_lay = QtWidgets.QFormLayout()
-        af_center_lay.addStretch()
-        af_center_lay.addLayout(af_center_top_lay)
-        self.select_foil_cb = PDT_ComboBox(width=150)
-        self.select_foil_cb.addItems(['None'] + get_all_airfoil_files())
-        self.select_foil_cb.currentTextChanged.connect(self.select_foil_cb_changed)
-        af_center_top_lay.addRow(PDT_Label('Select Foil:', font_size=14, bold=True), self.select_foil_cb)
-        self.foil_xy_canvas = SingleAxCanvas(self, width=4, height=4)
-        af_center_lay.addWidget(self.foil_xy_canvas)
-        self.foil_xy_navbar = NavigationToolbar(self.foil_xy_canvas, self)
-        af_center_lay.addWidget(self.foil_xy_navbar)
-        af_center_lay.setAlignment(self.foil_xy_navbar, QtCore.Qt.AlignHCenter)
-
-        af_center_bot_lay = QtWidgets.QFormLayout()
-        lbl = PDT_Label('Download a Foil\nfrom UIUC Database:', font_size=14, bold=True)
-        download_btn = PDT_PushButton('Download', font_size=12)
-        download_btn.clicked.connect(self.download_btn_clicked)
-        af_center_bot_lay.addRow(lbl, download_btn)
-        af_center_bot_lay.setAlignment(download_btn, QtCore.Qt.AlignBottom)
-        self.download_name_le = download_name_le = PDT_LineEdit(font_size=11, width=150)
-        af_center_bot_lay.addRow(PDT_Label('Foil Name:', font_size=12), download_name_le)
-        af_center_lay.addStretch()
-        af_center_lay.addLayout(af_center_bot_lay)
-        af_center_lay.addStretch()
-
-        # airfoil right
-        af_right_top_lay = QtWidgets.QHBoxLayout()
-        af_right_lay.addLayout(af_right_top_lay)
-        metrics_strs = ['alpha', 'CL', 'CD', 'CDp', 'CM', 'Top_Xtr', 'Bot_Xtr', 'CL/CD']
-        ax_cb_widg = AxesComboBoxWidget(x_txts=['x-axis'] + metrics_strs, y_txts=['y-axis'] + metrics_strs,
-                                        init_xtxt='CD', init_ytxt='CL')
-        self.af_yax_cb, self.af_xax_cb = ax_cb_widg.yax_cb, ax_cb_widg.xax_cb
-        self.af_yax_cb.currentTextChanged.connect(self.af_metric_cb_changed)
-        self.af_xax_cb.currentTextChanged.connect(self.af_metric_cb_changed)
-        af_right_top_lay.addStretch()
-        af_right_top_lay.addWidget(PDT_Label('Plot Metric:', font_size=14, bold=True))
-        af_right_top_lay.addWidget(ax_cb_widg)
-        af_right_top_lay.addStretch()
-
-        self.foil_metric_canvas = SingleAxCanvas(self, width=8, height=5.5)
-        af_right_lay.addWidget(self.foil_metric_canvas)
-        self.metric_navbar = NavigationToolbar(self.foil_metric_canvas, self)
-        metric_nav_layout = QtWidgets.QHBoxLayout()
-        metric_nav_layout.addStretch()
-        metric_nav_layout.addWidget(self.metric_navbar)
-        metric_nav_layout.addStretch()
-        af_right_lay.addLayout(metric_nav_layout)
-
-    @property
-    def foil(self):
-        return self.main_win.foil
-
-    def download_btn_clicked(self):
-        foil_txt = self.download_name_le.text()
-        if foil_txt.strip() == '':
-            return
-        foil_txt = '{}.dat'.format(foil_txt) if not foil_txt.endswith('.dat') else foil_txt
-
-        with Capturing() as output:
-            successful = download_foil_coordinates(foil_str=foil_txt)
-        self.main_win.print(output)
-
-        if successful:
-            self.main_win.af_db_select_widg.update_found_lbl()
-            self.main_win.repop_select_foil_cb()
-            self.select_foil_cb.setCurrentText(foil_txt)
-
-    def af_metric_cb_changed(self):
-        self.foil_metric_canvas.axes.clear()
-        self.foil_metric_canvas.draw()
-        y_txt, x_txt = self.af_yax_cb.currentText(), self.af_xax_cb.currentText()
-        if y_txt == 'y-axis' or x_txt == 'x-axis':
-            return
-
-        if self.foil is None:
-            return
-
-        if len(self.foil.polar_data) == 0:
-            self.main_win.print('No data for current foil')
-            return
-
-        re_2_plot = self.exist_data_widg.get_re_to_plot()
-        mach_2_plot = self.exist_data_widg.get_machs_to_plot()
-        ncrit_2_plot = self.exist_data_widg.get_ncrits_to_plot()
-
-        with Capturing() as output:
-            self.foil.plot_polar_data(x_param=x_txt, y_param=y_txt, re_list=re_2_plot, mach_list=mach_2_plot,
-                                      ncrit_list=ncrit_2_plot, fig=self.foil_metric_canvas.figure)
-        self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
-
-        self.foil_metric_canvas.draw()
-
-    def select_foil_cb_changed(self, foil_txt):
-        self.main_win.print('Changing Current Foil...')
-        self.foil_xy_canvas.axes.clear()
-        if not foil_txt == 'None':
-            try:
-
-                with Capturing() as output:
-                    self.main_win.foil = Airfoil(name=foil_txt, exact_namematch=True)
-                self.main_win.console_te.append('\n'.join(output))
-
-            except Exception as e:
-                with Capturing() as output:
-                    self.main_win.print(e)
-                self.main_win.console_te.append('\n'.join(output))
-                self.main_win.foil = None
-        else:
-            self.main_win.foil = None
-
-        self.exist_data_widg.update_airfoil(af=self.foil)
-        if self.main_win.foil is not None:
-            self.foil.plot_geometry(fig=self.foil_xy_canvas.figure)
-            self.af_metric_cb_changed()  # updates the metric plot
-        else:
-            self.foil_xy_canvas.axes.clear()
-            self.foil_metric_canvas.axes.clear()
-        self.foil_xy_canvas.draw()
-        self.foil_metric_canvas.draw()
-
-
-class ExistingFoilDataWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(ExistingFoilDataWidget, self).__init__()
-        self.main_win = main_win
-
-        lay = QtWidgets.QVBoxLayout()
-        self.setLayout(lay)
-
-        title_lbl = PDT_Label('Existing Data (plot controls)', font_size=14, bold=True)
-        lay.addWidget(title_lbl)
-        del_btn = PDT_PushButton('Delete All', width=180, font_size=12)
-        del_btn.clicked.connect(self.del_btn_clicked)
-        lay.addWidget(del_btn)
-        btm_lay = QtWidgets.QHBoxLayout()
-        lay.addLayout(btm_lay)
-
-        # RE
-        re_grp = PDT_GroupBox('RE', font_size=11)
-        self.re_lay = QtWidgets.QGridLayout()
-        re_grp.setLayout(self.re_lay)
-        btm_lay.addWidget(re_grp)
-
-        # mach
-        mach_grp = PDT_GroupBox('Mach', font_size=11)
-        self.mach_lay = QtWidgets.QVBoxLayout()
-        mach_grp.setLayout(self.mach_lay)
-        btm_lay.addWidget(mach_grp)
-
-        # ncrit
-        ncrit_grp = PDT_GroupBox('Ncrit', font_size=11)
-        self.ncrit_lay = QtWidgets.QVBoxLayout()
-        ncrit_grp.setLayout(self.ncrit_lay)
-        btm_lay.addWidget(ncrit_grp)
-
-        # gets the all checkboxes in there
-        self.update_airfoil()
-    @property
-    def foil(self):
-        return self.main_win.foil
-
-    def del_btn_clicked(self):
-        if self.main_win.foil is not None:
-            with Capturing() as output:
-                clear_foil_database(single_foil=self.main_win.foil.name)
-            self.main_win.printer.print(output)
-            self.main_win.af_widg.select_foil_cb_changed(foil_txt=self.main_win.foil.name)
-
-    def get_re_to_plot(self):
-        res = []
-        for i in range(self.re_lay.count()):
-            chk = self.re_lay.itemAt(i).widget()
-            txt = chk.text()
-            if txt != 'Recheck all':
-                if chk.isChecked():
-                    res.append(float(txt))
-        return res
-
-    def get_machs_to_plot(self):
-        machs = []
-        for i in range(self.mach_lay.count()):
-            chk = self.mach_lay.itemAt(i).widget()
-            txt = chk.text()
-            if txt != 'Recheck all':
-                if chk.isChecked():
-                    machs.append(float(txt))
-        return machs
-
-    def get_ncrits_to_plot(self):
-        ncrits = []
-        for i in range(self.ncrit_lay.count()):
-            chk = self.ncrit_lay.itemAt(i).widget()
-            txt = chk.text()
-            if txt != 'Recheck all':
-                if chk.isChecked():
-                    ncrits.append(int(txt))
-        return ncrits
-
-    def update_airfoil(self, af: Airfoil = None):
-        delete_all_widgets_from_layout(layout=self.re_lay)
-        delete_all_widgets_from_layout(layout=self.mach_lay)
-        delete_all_widgets_from_layout(layout=self.ncrit_lay)
-
-        row = -1
-        if af is not None:
-            res, machs, ncrits = af.get_polar_data_grid()
-            for i, re in enumerate(res):
-                chk = PDT_CheckBox('{:.1e}'.format(re), checked=True)
-                chk.clicked.connect(self.re_mach_ncrit_chk_clicked)
-                if i < len(res) / 2:
-                    row = i
-                    col = 0
-                else:
-                    row = i - int(len(res) / 2)
-                    col = 1
-                self.re_lay.addWidget(chk, i, 0)
-                self.re_lay.addWidget(chk, row, col)
-            for mach in machs:
-                chk = PDT_CheckBox('{:.2f}'.format(mach), checked=True)
-                chk.clicked.connect(self.re_mach_ncrit_chk_clicked)
-                self.mach_lay.addWidget(chk)
-            for ncrit in ncrits:
-                chk = PDT_CheckBox('{}'.format(ncrit), checked=True)
-                chk.clicked.connect(self.re_mach_ncrit_chk_clicked)
-                self.ncrit_lay.addWidget(chk)
-
-
-        self.all_re_btn = PDT_PushButton('Recheck All', font_size=10, width=100)
-        self.all_re_btn.clicked.connect(self.all_re_btn_clicked)
-        self.re_lay.addWidget(self.all_re_btn, row + 1, 0)
-        self.all_mach_btn = PDT_PushButton('Recheck All', font_size=10, width=100)
-        self.all_mach_btn.clicked.connect(self.all_mach_btn_clicked)
-        self.mach_lay.addWidget(self.all_mach_btn)
-        self.all_ncrit_btn = PDT_PushButton('Recheck All', font_size=10, width=100)
-        self.all_ncrit_btn.clicked.connect(self.all_ncrit_btn_clicked)
-        self.ncrit_lay.addWidget(self.all_ncrit_btn)
-
-    def re_mach_ncrit_chk_clicked(self):
-        self.main_win.af_widg.af_metric_cb_changed()
-
-    def all_re_btn_clicked(self):
-        for i in range(self.re_lay.count()):
-            itm = self.re_lay.itemAt(i)
-            if itm:
-                widg = itm.widget()
-                if isinstance(widg, PDT_CheckBox):
-                    widg.setChecked(True)
-        self.main_win.af_widg.af_metric_cb_changed()
-
-    def all_mach_btn_clicked(self):
-        for i in range(self.re_lay.count()):
-            itm = self.mach_lay.itemAt(i)
-            if itm:
-                widg = itm.widget()
-                if isinstance(widg, PDT_CheckBox):
-                    widg.setChecked(True)
-        self.main_win.af_widg.af_metric_cb_changed()
-
-    def all_ncrit_btn_clicked(self):
-        for i in range(self.re_lay.count()):
-            itm = self.ncrit_lay.itemAt(i)
-            if itm:
-                widg = itm.widget()
-                if isinstance(widg, PDT_CheckBox):
-                    widg.setChecked(True)
-        self.main_win.af_widg.af_metric_cb_changed()
-
-
-class AddFoilDataPointWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(AddFoilDataPointWidget, self).__init__()
-        self.main_win = main_win
-
-        lay = QtWidgets.QFormLayout()
-        self.setLayout(lay)
-
-        overwrite_chk = PDT_CheckBox('Overwrite Existing Data?', font_size=11)
-        overwrite_chk.setEnabled(False)
-        lay.addRow(PDT_Label('Add\nDatapoints\nBy Range:', font_size=14, bold=True), overwrite_chk)
-        lay.setAlignment(overwrite_chk, QtCore.Qt.AlignBottom)
-        self.re_rle = RangeLineEditWidget(box_range=[1e4, 1e9], default_strs=['1e6', '1e7', '3e6'],
-                                          spin_double_science='science')
-        self.mach_rle = RangeLineEditWidget(box_range=[0, 10], box_single_step=0.05,
-                                            default_strs=['0.00', '0.00', '0.10'], spin_double_science='double')
-        self.ncrit_rle = RangeLineEditWidget(box_range=[4, 14], box_single_step=1, default_strs=['9', '9', '1'],
-                                             spin_double_science='spin')
-        lay.addRow(PDT_Label('Re:', font_size=12), self.re_rle)
-        lay.addRow(PDT_Label('Mach:', font_size=12), self.mach_rle)
-        lay.addRow(PDT_Label('Ncrit:', font_size=12), self.ncrit_rle)
-
-        self.add_btn = PDT_PushButton('Add Data', font_size=12, width=110, bold=True)
-        self.reset_btn = PDT_PushButton('Reset Ranges', font_size=12, width=130, bold=True)
-        self.add_btn.clicked.connect(self.add_foil_data_btn_clicked)
-        self.reset_btn.clicked.connect(self.reset_foil_ranges_btn_clicked)
-        btn_lay = QtWidgets.QHBoxLayout()
-        btn_lay.addStretch()
-        btn_lay.addWidget(self.add_btn)
-        btn_lay.addWidget(self.reset_btn)
-        btn_lay.addStretch()
-        lay.addRow(btn_lay)
-        lay.setAlignment(btn_lay, QtCore.Qt.AlignRight)
-        lay.setLabelAlignment(QtCore.Qt.AlignRight)
-
-    @property
-    def foil(self):
-        return self.main_win.foil
-
-    def reset_foil_ranges_btn_clicked(self):
-        self.reset_ranges()
-
-    def reset_ranges(self):
-        self.re_rle.reset_boxes()
-        self.mach_rle.reset_boxes()
-        self.ncrit_rle.reset_boxes()
-
-    def get_re_range(self):
-        return self.re_rle.get_start_stop_step()
-
-    def get_mach_range(self):
-        return self.mach_rle.get_start_stop_step()
-
-    def get_ncrit_range(self):
-        return self.ncrit_rle.get_start_stop_step()
-
-    def add_foil_data_btn_clicked(self):
-
-        if self.foil is None:
-            self.print('Must select a foil first!')
-            return
-
-        self.main_win.prog_bar.setValue(0)
-
-        re_min, re_max, re_step = self.get_re_range()
-        mach_min, mach_max, mach_step = self.get_mach_range()
-        ncrit_min, ncrit_max, ncrit_step = self.get_ncrit_range()
-
-        res = np.arange(re_min, re_max, re_step)
-        machs = np.arange(mach_min, mach_max, mach_step)
-        ncrits = np.arange(ncrit_min, ncrit_max, ncrit_step)
-
-        self.thread = QtCore.QThread()
-        self.foil_worker = AddFoilDataWorker(foil=self.foil, res=res, machs=machs, ncrits=ncrits)
-        self.foil_worker.moveToThread(self.thread)
-        self.thread.started.connect(self.foil_worker.run)
-        self.foil_worker.finished.connect(self.thread.quit)
-        self.foil_worker.finished.connect(self.foil_worker.deleteLater)
-        self.foil_worker.finished.connect(self.on_foil_worker_finish)
-        self.thread.finished.connect(self.thread.deleteLater)
-        self.foil_worker.progress.connect(self.update_foil_worker_progress)
-
-        self.setEnabled(False)
-        self.main_win.af_widg.exist_data_widg.setEnabled(False)
-        self.main_win.af_widg.select_foil_cb.setEnabled(False)
-        self.thread.start()
-
-    def on_foil_worker_finish(self):
-        self.setEnabled(True)
-        self.main_win.af_widg.exist_data_widg.setEnabled(True)
-        self.main_win.af_widg.select_foil_cb.setEnabled(True)
-        self.main_win.prog_bar.setValue(0)
-
-    def update_foil_worker_progress(self, prog: int, output: list):
-        self.main_win.print(output)
-        self.main_win.prog_bar.setValue(prog)
-        with Capturing() as output:
-            self.foil.load_polar_data()
-        self.main_win.print(output)
-        self.main_win.af_widg.select_foil_cb_changed(foil_txt=self.main_win.af_widg.select_foil_cb.currentText())  # updates everything
-
-
-class AddFoilDataWorker(QtCore.QObject):
-    finished = QtCore.pyqtSignal()
-    progress = QtCore.pyqtSignal(int, list)
-
-    def __init__(self, foil: 'Airfoil', res: list, machs: list, ncrits: list):
-        super(AddFoilDataWorker, self).__init__()
-        self.foil = foil
-        self.res = res
-        self.machs = machs
-        self.ncrits = ncrits
-
-    def run(self):
-        total_polars = len(self.res) * len(self.machs) * len(self.ncrits)
-
-        counter = 0
-        for re in self.res:
-            for mach in self.machs:
-                for ncrit in self.ncrits:
-                    counter += 1
-                    with Capturing() as output:
-                        self.foil.calculate_xfoil_polars(re=[re], mach=[mach], ncrit=[ncrit])
-                    self.progress.emit(int(counter / total_polars * 100), output)
-
-        self.finished.emit()
+from propeller_design_tools.funcs import delete_all_widgets_from_layout, get_all_airfoil_files, clear_foil_database, \
+    download_foil_coordinates
+from propeller_design_tools.airfoil import Airfoil
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+import numpy as np
+try:
+    from PyQt5 import QtWidgets, QtCore
+    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_PushButton, PDT_ComboBox, \
+        PDT_CheckBox, PDT_LineEdit
+    from propeller_design_tools.helper_ui_classes import RangeLineEditWidget, SingleAxCanvas, AxesComboBoxWidget, \
+        Capturing
+except:
+    pass
+
+
+class FoilAnalysisWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(FoilAnalysisWidget, self).__init__()
+        self.main_win = main_win
+
+        # airfoil group
+        af_lay = QtWidgets.QHBoxLayout()
+        self.setLayout(af_lay)
+        af_left_lay = QtWidgets.QVBoxLayout()
+        af_lay.addLayout(af_left_lay)
+        af_center_lay = QtWidgets.QVBoxLayout()
+        af_lay.addLayout(af_center_lay)
+        af_right_lay = QtWidgets.QVBoxLayout()
+        af_lay.addLayout(af_right_lay)
+
+        # airfoil left
+        af_left_lay.addStretch()
+        self.exist_data_widg = ExistingFoilDataWidget(main_win=self.main_win)
+        af_left_lay.addWidget(self.exist_data_widg)
+        af_left_lay.addStretch()
+        self.add_foil_data_widg = AddFoilDataPointWidget(main_win=self.main_win)
+        af_left_lay.addWidget(self.add_foil_data_widg)
+        af_left_lay.addStretch()
+
+        # airfoil center
+        af_center_top_lay = QtWidgets.QFormLayout()
+        af_center_lay.addStretch()
+        af_center_lay.addLayout(af_center_top_lay)
+        self.select_foil_cb = PDT_ComboBox(width=150)
+        self.select_foil_cb.addItems(['None'] + get_all_airfoil_files())
+        self.select_foil_cb.currentTextChanged.connect(self.select_foil_cb_changed)
+        af_center_top_lay.addRow(PDT_Label('Select Foil:', font_size=14, bold=True), self.select_foil_cb)
+        self.foil_xy_canvas = SingleAxCanvas(self, width=4, height=4)
+        af_center_lay.addWidget(self.foil_xy_canvas)
+        self.foil_xy_navbar = NavigationToolbar(self.foil_xy_canvas, self)
+        af_center_lay.addWidget(self.foil_xy_navbar)
+        af_center_lay.setAlignment(self.foil_xy_navbar, QtCore.Qt.AlignHCenter)
+
+        af_center_bot_lay = QtWidgets.QFormLayout()
+        lbl = PDT_Label('Download a Foil\nfrom UIUC Database:', font_size=14, bold=True)
+        download_btn = PDT_PushButton('Download', font_size=12)
+        download_btn.clicked.connect(self.download_btn_clicked)
+        af_center_bot_lay.addRow(lbl, download_btn)
+        af_center_bot_lay.setAlignment(download_btn, QtCore.Qt.AlignBottom)
+        self.download_name_le = download_name_le = PDT_LineEdit(font_size=11, width=150)
+        af_center_bot_lay.addRow(PDT_Label('Foil Name:', font_size=12), download_name_le)
+        af_center_lay.addStretch()
+        af_center_lay.addLayout(af_center_bot_lay)
+        af_center_lay.addStretch()
+
+        # airfoil right
+        af_right_top_lay = QtWidgets.QHBoxLayout()
+        af_right_lay.addLayout(af_right_top_lay)
+        metrics_strs = ['alpha', 'CL', 'CD', 'CDp', 'CM', 'Top_Xtr', 'Bot_Xtr', 'CL/CD']
+        ax_cb_widg = AxesComboBoxWidget(x_txts=['x-axis'] + metrics_strs, y_txts=['y-axis'] + metrics_strs,
+                                        init_xtxt='CD', init_ytxt='CL')
+        self.af_yax_cb, self.af_xax_cb = ax_cb_widg.yax_cb, ax_cb_widg.xax_cb
+        self.af_yax_cb.currentTextChanged.connect(self.af_metric_cb_changed)
+        self.af_xax_cb.currentTextChanged.connect(self.af_metric_cb_changed)
+        af_right_top_lay.addStretch()
+        af_right_top_lay.addWidget(PDT_Label('Plot Metric:', font_size=14, bold=True))
+        af_right_top_lay.addWidget(ax_cb_widg)
+        af_right_top_lay.addStretch()
+
+        self.foil_metric_canvas = SingleAxCanvas(self, width=8, height=5.5)
+        af_right_lay.addWidget(self.foil_metric_canvas)
+        self.metric_navbar = NavigationToolbar(self.foil_metric_canvas, self)
+        metric_nav_layout = QtWidgets.QHBoxLayout()
+        metric_nav_layout.addStretch()
+        metric_nav_layout.addWidget(self.metric_navbar)
+        metric_nav_layout.addStretch()
+        af_right_lay.addLayout(metric_nav_layout)
+
+    @property
+    def foil(self):
+        return self.main_win.foil
+
+    def download_btn_clicked(self):
+        foil_txt = self.download_name_le.text()
+        if foil_txt.strip() == '':
+            return
+        foil_txt = '{}.dat'.format(foil_txt) if not foil_txt.endswith('.dat') else foil_txt
+
+        with Capturing() as output:
+            successful = download_foil_coordinates(foil_str=foil_txt)
+        self.main_win.print(output)
+
+        if successful:
+            self.main_win.af_db_select_widg.update_found_lbl()
+            self.main_win.repop_select_foil_cb()
+            self.select_foil_cb.setCurrentText(foil_txt)
+
+    def af_metric_cb_changed(self):
+        self.foil_metric_canvas.axes.clear()
+        self.foil_metric_canvas.draw()
+        y_txt, x_txt = self.af_yax_cb.currentText(), self.af_xax_cb.currentText()
+        if y_txt == 'y-axis' or x_txt == 'x-axis':
+            return
+
+        if self.foil is None:
+            return
+
+        if len(self.foil.polar_data) == 0:
+            self.main_win.print('No data for current foil')
+            return
+
+        re_2_plot = self.exist_data_widg.get_re_to_plot()
+        mach_2_plot = self.exist_data_widg.get_machs_to_plot()
+        ncrit_2_plot = self.exist_data_widg.get_ncrits_to_plot()
+
+        with Capturing() as output:
+            self.foil.plot_polar_data(x_param=x_txt, y_param=y_txt, re_list=re_2_plot, mach_list=mach_2_plot,
+                                      ncrit_list=ncrit_2_plot, fig=self.foil_metric_canvas.figure)
+        self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
+
+        self.foil_metric_canvas.draw()
+
+    def select_foil_cb_changed(self, foil_txt):
+        self.main_win.print('Changing Current Foil...')
+        self.foil_xy_canvas.axes.clear()
+        if not foil_txt == 'None':
+            try:
+
+                with Capturing() as output:
+                    self.main_win.foil = Airfoil(name=foil_txt, exact_namematch=True)
+                self.main_win.console_te.append('\n'.join(output))
+
+            except Exception as e:
+                with Capturing() as output:
+                    self.main_win.print(e)
+                self.main_win.console_te.append('\n'.join(output))
+                self.main_win.foil = None
+        else:
+            self.main_win.foil = None
+
+        self.exist_data_widg.update_airfoil(af=self.foil)
+        if self.main_win.foil is not None:
+            self.foil.plot_geometry(fig=self.foil_xy_canvas.figure)
+            self.af_metric_cb_changed()  # updates the metric plot
+        else:
+            self.foil_xy_canvas.axes.clear()
+            self.foil_metric_canvas.axes.clear()
+        self.foil_xy_canvas.draw()
+        self.foil_metric_canvas.draw()
+
+
+class ExistingFoilDataWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(ExistingFoilDataWidget, self).__init__()
+        self.main_win = main_win
+
+        lay = QtWidgets.QVBoxLayout()
+        self.setLayout(lay)
+
+        title_lbl = PDT_Label('Existing Data (plot controls)', font_size=14, bold=True)
+        lay.addWidget(title_lbl)
+        del_btn = PDT_PushButton('Delete All', width=180, font_size=12)
+        del_btn.clicked.connect(self.del_btn_clicked)
+        lay.addWidget(del_btn)
+        btm_lay = QtWidgets.QHBoxLayout()
+        lay.addLayout(btm_lay)
+
+        # RE
+        re_grp = PDT_GroupBox('RE', font_size=11)
+        self.re_lay = QtWidgets.QGridLayout()
+        re_grp.setLayout(self.re_lay)
+        btm_lay.addWidget(re_grp)
+
+        # mach
+        mach_grp = PDT_GroupBox('Mach', font_size=11)
+        self.mach_lay = QtWidgets.QVBoxLayout()
+        mach_grp.setLayout(self.mach_lay)
+        btm_lay.addWidget(mach_grp)
+
+        # ncrit
+        ncrit_grp = PDT_GroupBox('Ncrit', font_size=11)
+        self.ncrit_lay = QtWidgets.QVBoxLayout()
+        ncrit_grp.setLayout(self.ncrit_lay)
+        btm_lay.addWidget(ncrit_grp)
+
+        # gets the all checkboxes in there
+        self.update_airfoil()
+    @property
+    def foil(self):
+        return self.main_win.foil
+
+    def del_btn_clicked(self):
+        if self.main_win.foil is not None:
+            with Capturing() as output:
+                clear_foil_database(single_foil=self.main_win.foil.name)
+            self.main_win.printer.print(output)
+            self.main_win.af_widg.select_foil_cb_changed(foil_txt=self.main_win.foil.name)
+
+    def get_re_to_plot(self):
+        res = []
+        for i in range(self.re_lay.count()):
+            chk = self.re_lay.itemAt(i).widget()
+            txt = chk.text()
+            if txt != 'Recheck all':
+                if chk.isChecked():
+                    res.append(float(txt))
+        return res
+
+    def get_machs_to_plot(self):
+        machs = []
+        for i in range(self.mach_lay.count()):
+            chk = self.mach_lay.itemAt(i).widget()
+            txt = chk.text()
+            if txt != 'Recheck all':
+                if chk.isChecked():
+                    machs.append(float(txt))
+        return machs
+
+    def get_ncrits_to_plot(self):
+        ncrits = []
+        for i in range(self.ncrit_lay.count()):
+            chk = self.ncrit_lay.itemAt(i).widget()
+            txt = chk.text()
+            if txt != 'Recheck all':
+                if chk.isChecked():
+                    ncrits.append(int(txt))
+        return ncrits
+
+    def update_airfoil(self, af: Airfoil = None):
+        delete_all_widgets_from_layout(layout=self.re_lay)
+        delete_all_widgets_from_layout(layout=self.mach_lay)
+        delete_all_widgets_from_layout(layout=self.ncrit_lay)
+
+        row = -1
+        if af is not None:
+            res, machs, ncrits = af.get_polar_data_grid()
+            for i, re in enumerate(res):
+                chk = PDT_CheckBox('{:.1e}'.format(re), checked=True)
+                chk.clicked.connect(self.re_mach_ncrit_chk_clicked)
+                if i < len(res) / 2:
+                    row = i
+                    col = 0
+                else:
+                    row = i - int(len(res) / 2)
+                    col = 1
+                self.re_lay.addWidget(chk, i, 0)
+                self.re_lay.addWidget(chk, row, col)
+            for mach in machs:
+                chk = PDT_CheckBox('{:.2f}'.format(mach), checked=True)
+                chk.clicked.connect(self.re_mach_ncrit_chk_clicked)
+                self.mach_lay.addWidget(chk)
+            for ncrit in ncrits:
+                chk = PDT_CheckBox('{}'.format(ncrit), checked=True)
+                chk.clicked.connect(self.re_mach_ncrit_chk_clicked)
+                self.ncrit_lay.addWidget(chk)
+
+
+        self.all_re_btn = PDT_PushButton('Recheck All', font_size=10, width=100)
+        self.all_re_btn.clicked.connect(self.all_re_btn_clicked)
+        self.re_lay.addWidget(self.all_re_btn, row + 1, 0)
+        self.all_mach_btn = PDT_PushButton('Recheck All', font_size=10, width=100)
+        self.all_mach_btn.clicked.connect(self.all_mach_btn_clicked)
+        self.mach_lay.addWidget(self.all_mach_btn)
+        self.all_ncrit_btn = PDT_PushButton('Recheck All', font_size=10, width=100)
+        self.all_ncrit_btn.clicked.connect(self.all_ncrit_btn_clicked)
+        self.ncrit_lay.addWidget(self.all_ncrit_btn)
+
+    def re_mach_ncrit_chk_clicked(self):
+        self.main_win.af_widg.af_metric_cb_changed()
+
+    def all_re_btn_clicked(self):
+        for i in range(self.re_lay.count()):
+            itm = self.re_lay.itemAt(i)
+            if itm:
+                widg = itm.widget()
+                if isinstance(widg, PDT_CheckBox):
+                    widg.setChecked(True)
+        self.main_win.af_widg.af_metric_cb_changed()
+
+    def all_mach_btn_clicked(self):
+        for i in range(self.re_lay.count()):
+            itm = self.mach_lay.itemAt(i)
+            if itm:
+                widg = itm.widget()
+                if isinstance(widg, PDT_CheckBox):
+                    widg.setChecked(True)
+        self.main_win.af_widg.af_metric_cb_changed()
+
+    def all_ncrit_btn_clicked(self):
+        for i in range(self.re_lay.count()):
+            itm = self.ncrit_lay.itemAt(i)
+            if itm:
+                widg = itm.widget()
+                if isinstance(widg, PDT_CheckBox):
+                    widg.setChecked(True)
+        self.main_win.af_widg.af_metric_cb_changed()
+
+
+class AddFoilDataPointWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(AddFoilDataPointWidget, self).__init__()
+        self.main_win = main_win
+
+        lay = QtWidgets.QFormLayout()
+        self.setLayout(lay)
+
+        overwrite_chk = PDT_CheckBox('Overwrite Existing Data?', font_size=11)
+        overwrite_chk.setEnabled(False)
+        lay.addRow(PDT_Label('Add\nDatapoints\nBy Range:', font_size=14, bold=True), overwrite_chk)
+        lay.setAlignment(overwrite_chk, QtCore.Qt.AlignBottom)
+        self.re_rle = RangeLineEditWidget(box_range=[1e4, 1e9], default_strs=['1e6', '1e7', '3e6'],
+                                          spin_double_science='science')
+        self.mach_rle = RangeLineEditWidget(box_range=[0, 10], box_single_step=0.05,
+                                            default_strs=['0.00', '0.00', '0.10'], spin_double_science='double')
+        self.ncrit_rle = RangeLineEditWidget(box_range=[4, 14], box_single_step=1, default_strs=['9', '9', '1'],
+                                             spin_double_science='spin')
+        lay.addRow(PDT_Label('Re:', font_size=12), self.re_rle)
+        lay.addRow(PDT_Label('Mach:', font_size=12), self.mach_rle)
+        lay.addRow(PDT_Label('Ncrit:', font_size=12), self.ncrit_rle)
+
+        self.add_btn = PDT_PushButton('Add Data', font_size=12, width=110, bold=True)
+        self.reset_btn = PDT_PushButton('Reset Ranges', font_size=12, width=130, bold=True)
+        self.add_btn.clicked.connect(self.add_foil_data_btn_clicked)
+        self.reset_btn.clicked.connect(self.reset_foil_ranges_btn_clicked)
+        btn_lay = QtWidgets.QHBoxLayout()
+        btn_lay.addStretch()
+        btn_lay.addWidget(self.add_btn)
+        btn_lay.addWidget(self.reset_btn)
+        btn_lay.addStretch()
+        lay.addRow(btn_lay)
+        lay.setAlignment(btn_lay, QtCore.Qt.AlignRight)
+        lay.setLabelAlignment(QtCore.Qt.AlignRight)
+
+    @property
+    def foil(self):
+        return self.main_win.foil
+
+    def reset_foil_ranges_btn_clicked(self):
+        self.reset_ranges()
+
+    def reset_ranges(self):
+        self.re_rle.reset_boxes()
+        self.mach_rle.reset_boxes()
+        self.ncrit_rle.reset_boxes()
+
+    def get_re_range(self):
+        return self.re_rle.get_start_stop_step()
+
+    def get_mach_range(self):
+        return self.mach_rle.get_start_stop_step()
+
+    def get_ncrit_range(self):
+        return self.ncrit_rle.get_start_stop_step()
+
+    def add_foil_data_btn_clicked(self):
+
+        if self.foil is None:
+            self.print('Must select a foil first!')
+            return
+
+        self.main_win.prog_bar.setValue(0)
+
+        re_min, re_max, re_step = self.get_re_range()
+        mach_min, mach_max, mach_step = self.get_mach_range()
+        ncrit_min, ncrit_max, ncrit_step = self.get_ncrit_range()
+
+        res = np.arange(re_min, re_max, re_step)
+        machs = np.arange(mach_min, mach_max, mach_step)
+        ncrits = np.arange(ncrit_min, ncrit_max, ncrit_step)
+
+        self.thread = QtCore.QThread()
+        self.foil_worker = AddFoilDataWorker(foil=self.foil, res=res, machs=machs, ncrits=ncrits)
+        self.foil_worker.moveToThread(self.thread)
+        self.thread.started.connect(self.foil_worker.run)
+        self.foil_worker.finished.connect(self.thread.quit)
+        self.foil_worker.finished.connect(self.foil_worker.deleteLater)
+        self.foil_worker.finished.connect(self.on_foil_worker_finish)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.foil_worker.progress.connect(self.update_foil_worker_progress)
+
+        self.setEnabled(False)
+        self.main_win.af_widg.exist_data_widg.setEnabled(False)
+        self.main_win.af_widg.select_foil_cb.setEnabled(False)
+        self.thread.start()
+
+    def on_foil_worker_finish(self):
+        self.setEnabled(True)
+        self.main_win.af_widg.exist_data_widg.setEnabled(True)
+        self.main_win.af_widg.select_foil_cb.setEnabled(True)
+        self.main_win.prog_bar.setValue(0)
+
+    def update_foil_worker_progress(self, prog: int, output: list):
+        self.main_win.print(output)
+        self.main_win.prog_bar.setValue(prog)
+        with Capturing() as output:
+            self.foil.load_polar_data()
+        self.main_win.print(output)
+        self.main_win.af_widg.select_foil_cb_changed(foil_txt=self.main_win.af_widg.select_foil_cb.currentText())  # updates everything
+
+
+class AddFoilDataWorker(QtCore.QObject):
+    finished = QtCore.pyqtSignal()
+    progress = QtCore.pyqtSignal(int, list)
+
+    def __init__(self, foil: 'Airfoil', res: list, machs: list, ncrits: list):
+        super(AddFoilDataWorker, self).__init__()
+        self.foil = foil
+        self.res = res
+        self.machs = machs
+        self.ncrits = ncrits
+
+    def run(self):
+        total_polars = len(self.res) * len(self.machs) * len(self.ncrits)
+
+        counter = 0
+        for re in self.res:
+            for mach in self.machs:
+                for ncrit in self.ncrits:
+                    counter += 1
+                    with Capturing() as output:
+                        self.foil.calculate_xfoil_polars(re=[re], mach=[mach], ncrit=[ncrit])
+                    self.progress.emit(int(counter / total_polars * 100), output)
+
+        self.finished.emit()
```

### Comparing `propeller_design_tools-0.3.5/propdes/funcs.py` & `propeller_design_tools-0.4.0/propeller_design_tools/funcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1236 +1,1236 @@
-import os
-import subprocess
-import shutil
-import sys
-import urllib.request
-
-import matplotlib.pyplot as plt
-import numpy as np
-from propdes.airfoil import Airfoil
-from propdes.radialstation import RadialStation
-from propdes.propeller import Propeller
-from propdes.user_io import Info, Error, Warning
-from propdes.settings import _get_user_settings, get_prop_db, get_foil_db
-
-
-# =============== CONVENIENCE / UTILITY FUNCTIONS ===============
-def delete_propeller(prop, verbose: bool = True):
-    fpaths = [prop.xrr_file, prop.xrop_file, prop.meta_file]
-    rmvd = []
-    for path in fpaths:
-        if os.path.isfile(path):
-            os.remove(path)
-            rmvd.append(path)
-    if verbose:
-        Info('Removed paths: {}'.format(rmvd))
-
-
-def clear_foil_database(single_foil: str = None, inside_root_db: bool = False, inside_polar_db: bool = True,
-                        inside_for_xfoil: bool = True, verbose: bool = True):
-    """
-    Helper function to clear out files from foil database.
-
-    :param inside_root_db:
-    :param inside_polar_db:
-    :param inside_for_xfoil:
-    :return:
-    """
-    if single_foil is not None:
-        single_foil = '{}.dat'.format(single_foil) if not single_foil.endswith('.dat') else single_foil
-
-    foils_2_del = [single_foil] if single_foil is not None else get_all_airfoil_files()
-
-    for foil_file in foils_2_del:
-        foil_name = foil_file.replace('.dat', '')
-        if verbose:
-            Info('Clearing files for "{}"'.format(foil_name))
-
-        foil_fpath = os.path.join(_get_user_settings()['airfoil_database'], foil_file)
-        polar_fpath = os.path.join(_get_user_settings()['airfoil_database'], 'polar_database', '{}_polar_data.txt'.format(foil_name))
-        xfoil_fpath = os.path.join(_get_user_settings()['airfoil_database'], 'for_xfoil', '{}.txt'.format(foil_name))
-
-        if inside_root_db:
-            if os.path.exists(foil_fpath):
-                os.remove(foil_fpath)
-                if verbose:
-                    Info('Removed file "{}"'.format(foil_fpath), indent_level=1)
-        if inside_polar_db:
-            if os.path.exists(polar_fpath):
-                os.remove(polar_fpath)
-                if verbose:
-                    Info('Removed file "{}"'.format(polar_fpath), indent_level=1)
-        if inside_for_xfoil:
-            if os.path.exists(xfoil_fpath):
-                os.remove(xfoil_fpath)
-                if verbose:
-                    Info('Removed file "{}"'.format(xfoil_fpath), indent_level=1)
-
-
-def clear_prop_database(inside_root_db: bool = True, inside_xrotor_files: bool = True, inside_op_files: bool = True):
-    """
-    Helper function to clear out files from prop database.
-
-    :param inside_op_files:
-    :param inside_root_db:
-    :param inside_xrotor_files:
-    :return:
-    """
-    if inside_root_db:
-        delete_files_from_folder(_get_user_settings()['propeller_database'])
-    if inside_xrotor_files:
-        delete_files_from_folder(os.path.join(_get_user_settings()['propeller_database'], 'xrotor_geometry_files'))
-    if inside_op_files:
-        delete_files_from_folder(os.path.join(_get_user_settings()['propeller_database'], 'xrotor_op_files'))
-
-
-def delete_files_from_folder(folder: str):
-    if os.path.exists(folder):
-        for filename in os.listdir(folder):
-            fpath = os.path.join(folder, filename)
-            if os.path.isfile(fpath):
-                os.remove(fpath)
-    else:
-        raise Error('Cannot find folder: {}'.format(folder))
-
-
-def count_airfoil_db():
-    return len(get_all_airfoil_files())
-
-
-def count_propeller_db():
-    return len(get_all_propeller_dirs())
-
-
-def get_all_airfoil_files():
-    af_db = get_foil_db()
-    fnames = []
-    for fname in os.listdir(af_db):
-        if os.path.splitext(fname)[1] in ['.dat', '.txt']:
-            fnames.append(fname)
-    return [name for name in fnames if name not in ['polar_output.txt', 'xfoil_inputs_temp.txt']]
-
-
-def get_all_propeller_dirs():
-    prop_db = get_prop_db()
-    dirnames = []
-    for name in os.listdir(prop_db):
-        pth = os.path.join(prop_db, name)
-        if os.path.isdir(pth):
-            if any([os.path.splitext(p)[1] == '.meta' for p in os.listdir(pth)]):
-                dirnames.append(name)
-    return dirnames
-
-
-def search_files(folder: str, search_strs: list = None, contains_any: bool = False, include_dirs: bool = False):
-    """
-    Utility function to help users interface with getting files from folders
-
-    :param folder: the full path to the folder to look in
-    :param search_strs: a list of strings to search for in each filename
-    :param contains_any: If True will return files that contain ANY of the search strings, defaults to False (returns only
-        filenames that contain ALL of the search strings)
-    :return: a list of filenames
-    """
-
-    if not os.path.exists(folder):
-        raise Error('PDT ERROR: No folder named "{}" found!'.format(folder))
-
-    if include_dirs:
-        files = os.listdir(folder)
-    else:
-        files = [f for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f))]
-
-    if search_strs == []:
-        search_strs = None
-
-    if search_strs is not None:
-        # for s in search_strs:
-        #     files = []
-        if contains_any:  # ANY
-            files = [f for f in files if any([s in f for s in search_strs])]
-        else:  # ALL
-            files = [f for f in files if all([s in f for s in search_strs])]
-
-    return files
-
-
-def get_airfoil_file_from_db(foil_name: str, exact_namematch: bool = False):
-    db_dir = _get_user_settings()['airfoil_database']
-    possible_files = search_files(folder=db_dir, search_strs=[foil_name])
-    exact_fname = '{}.dat'.format(foil_name)
-
-    if len(possible_files) == 1:
-        if not exact_namematch:
-            return possible_files[0]
-        else:   # must match exactly
-            if possible_files[0] == exact_fname:
-                return possible_files[0]
-            else:
-                raise Error('Did not find an exact match for "{}"'.format(exact_fname))
-
-    elif len(possible_files) == 0:
-        raise Error('Did not find any coordinate files containing name "{}" when looking in user-set airfoil '
-                    'database: {}'.format(foil_name, db_dir))
-
-    else:   # found multiple files
-        if not exact_namematch:
-            raise Error('Found multiple coordinate files looking for airfoil "{}"!\n{}\n'
-                        'Consider using kwarg exact_namematch=True'.format(foil_name, possible_files))
-        else:
-            possible_files = [f for f in possible_files if f == exact_fname]
-            if len(possible_files) == 0:
-                raise Error('Did not find any coordinate files exactly matching "{}"'.format(exact_fname))
-            else:
-                return possible_files[0]
-
-
-def merge_polar_data_dicts(new: dict, old: dict):
-    if len(old) == 0:  # there was no old data
-        return new
-
-    new_pol_keys = new[list(new.keys())[0]].keys()
-    merged = new.copy()  # merged starts out as copy of the new dict
-    for old_pol_key, old_pol in old.items():  # cylce thru old dict
-        if old_pol_key not in new.keys():  # if saved (re, mach, ncrit) data not in new data
-            if old_pol.keys() == new_pol_keys:  # if keys are the same (alpha, CL, CD, etc)
-                merged[old_pol_key] = old_pol  # append and move on
-            else:  # if keys aren't same, warn that data isn't being retained
-                print('Warning: found saved polar data of older/incorrect format -> deleting {}'.format(old_pol_key))
-        else:  # if saved (re, mach, ncrit) data in new data
-            if old_pol.keys() == new_pol_keys:  # if same keys (alpha, CL, CD, etc) inform of overwrite
-                pass
-                # print('Warning: overwriting saved polar data for {}'.format(old_pol_key))
-            else:  # if not same keys
-                print('Warning: overwriting saved polar data for {} (was older/incorrect format)'.format(old_pol_key))
-    return merged
-
-
-def scrub_nans(d: dict):
-    # get all the indices where there's nans
-    nan_idxs = []
-    for key, val in d.items():
-        if hasattr(val, '__len__'):     # only consider arrays / lists
-            idxs = np.where(np.isnan(val))[0]
-            nan_idxs.extend(list(idxs))
-    nan_idxs = list(set(nan_idxs))
-
-    # now cycle through and create a new dictionary without nans
-    new_d = {}
-    for key, val in d.items():
-        if isinstance(val, list):   # if it's a list, return a list
-            new_d[key] = [v for i, v in enumerate(val) if i not in nan_idxs]
-        elif isinstance(val, np.ndarray):   # if it's a np array, return an np array
-            new_d[key] = np.array([v for i, v in enumerate(val) if i not in nan_idxs])
-        else:   # otherwise, just stuff it back in to the new dictionary un-altered
-            new_d[key] = val
-
-    return new_d
-
-
-# =============== FILE READING / WRITING FUNCTIONS ===============
-def read_airfoil_coordinate_file(fpath: str, verbose: bool = True, te_gap_set: float = 0.004):
-    """
-    Function to read an airfoil coordinate listing file in .dat or .txt format, assumes foil name is on
-    1st line, then reads in the list of coordinates following (ignoring any lines with numbers > 1.0, and
-    assuming the coordinates are single-space delimited) -> this is the file format as downloaded from
-
-    https://m-selig.ae.illinois.edu/ads/coord_database.html
-
-    It then splits the coordinates into upper and lower, and determines if either needs to be reversed
-    (in order to read into xfoil right and also plot correctly), then reverses them if needed and returns
-    arrays of x, y coords.
-
-    :param
-        fpath: the full filepath to the coordinate file
-    :return
-        name: the name of the airfoil from line1
-        x_coords: np.array of x-coordinates
-        y_coords: np.array of y-coordinates
-    """
-
-    # open the file and read contents
-    with open(fpath, 'r') as f:
-        txt = f.read()
-
-    # prep arrays
-    x_coords = np.array([])
-    y_coords = np.array([])
-
-    # split the text on returns and iterate over the lines
-    lines = txt.strip(' ').split('\n')
-    for i, line in enumerate(lines):
-        # assumes name of airfoil is on line 0
-        if i == 0:
-            name = line.strip(' ')
-        else:
-            if not line.strip(' ') == '':  # skips blank lines
-                vals = line.strip(' ').split(' ')  # split text on blank spaces
-                x = float(vals[0])  # x coord is the 0th element
-                y = float(vals[-1])  # y coord is the last element
-                if x <= 1:  # only append if x in the range [0,1]
-                    x_coords = np.append(x_coords, x)
-                if y <= 1:  # only append if y in the range [0,1]
-                    y_coords = np.append(y_coords, y)
-
-    # make lists of coordinates, upper, and lower
-    coords = np.array(list(zip(x_coords, y_coords)))
-    x_directions = np.sign(np.diff(x_coords))
-    x_directions = np.append(x_directions[0], x_directions)
-    upper_end_idx = np.where(np.abs(np.diff(x_directions)) == 2)[0][0]
-    upper_coords = coords[0:upper_end_idx + 1]
-    lower_coords = coords[upper_end_idx + 1:]
-
-    # flip upper if needed such that it is always decreasing in x
-    if not x_directions[0] == -1:
-        upper_coords = np.array(list(reversed(upper_coords)))
-
-    # flip lower if needed such that it is always increasing in x
-    if not x_directions[-1] == 1:
-        lower_coords = np.array(list(reversed(lower_coords)))
-
-    # check TE gap
-    te_gap = upper_coords[0][1] - lower_coords[-1][1]
-    blend_start = 0.7
-    if te_gap != te_gap_set:
-        total_dy = (te_gap_set - te_gap) / 2
-
-        upper_idxs = np.where(upper_coords[:, 0] > blend_start)[0]
-        for i in upper_idxs:
-            xc, yc = upper_coords[i]
-            dy = total_dy * (xc - blend_start) / (1 - blend_start)
-            yc += dy
-            upper_coords[i] = [xc, yc]
-
-        lower_idxs = np.where(lower_coords[:, 0] > 0.8)[0]
-        for i in lower_idxs:
-            xc, yc = lower_coords[i]
-            dy = total_dy * (xc - blend_start) / (1 - blend_start)
-            yc -= dy
-            lower_coords[i] = [xc, yc]
-        if verbose:
-            Info('Detected airfoil ({}) with TE not equal to the requested value\n-> artificially adjusted TE gap to {} '
-                     '(normalized)'.format(name, te_gap_set))
-
-    # re-combine upper and lower coords and split back into x, y arrays
-    if upper_coords[-1][0] == lower_coords[0][0] and upper_coords[-1][1] == lower_coords[0][1]:  # check for double 0, 0
-        coords = np.append(upper_coords, lower_coords[1:], axis=0)
-    else:
-        coords = np.append(upper_coords, lower_coords, axis=0)
-
-    x_coords, y_coords = zip(*coords)
-    return name, np.array(x_coords), np.array(y_coords)
-
-
-def run_xfoil(foil_relpath: str, re: float, alpha: list = None, cl: list = None, iter_limit: int = 30, ncrit: int = 9,
-              mach: float = 0.0, output_fpath: str = None, keypress_iternum: int = 1, tmout: int = 25,
-              hide_windows: bool = True, verbose: bool = False):
-    if not output_fpath:
-        output_fpath = 'polar_output.txt'
-
-    # swept pacc param
-    if alpha is not None and cl is not None:
-        raise Error('Cannot give "run_xfoil" both "alpha" and "cl"')
-    elif alpha is not None:
-        swept_param = {'alpha': alpha}
-    elif cl is not None:
-        swept_param = {'cl': cl}
-    else:
-        raise Error('Must give "run_xfoil" either a list of "alpha" to sweep or a list of "cl" to sweep')
-
-    # sort the swept values
-    vals = list(sorted(list(swept_param.values())[0]))
-
-    # directory and temp command file, also xfoil path
-    xfoil_dir = _get_user_settings()['airfoil_database']
-    xfoil_cmnd_file = os.path.join(xfoil_dir, 'xfoil_inputs_temp.txt')
-    xfoil_fpath = os.path.join(xfoil_dir, 'xfoil.exe')
-
-    # write the command file
-    with open(xfoil_cmnd_file, 'w') as f:
-        f.write('load {}\n'.format(foil_relpath))
-        f.write('ppar\nN\n200\n\n\n')
-        f.write('oper\n')
-        f.write('visc\n')
-        f.write('{0:.0f}\n'.format(re))
-        f.write('m {}\n'.format(mach))
-        f.write('vpar\n')
-        f.write('n {}\n\n'.format(ncrit))
-        f.write('iter\n')
-        f.write('{0:.0f}\n'.format(iter_limit))
-        f.write('pacc\n\n\n')
-        if 'alpha' in swept_param:
-            for a in vals:
-                f.write('a{}\n'.format(a))
-        elif 'cl' in swept_param:
-            for cl in vals:
-                f.write('cl{}\n'.format(cl))
-        f.write('!\n{}'.format(' ' * 100) * keypress_iternum)
-        f.write('pwrt\n')
-        f.write('{}\n\n\n'.format(output_fpath))
-        f.write('quit\n')
-
-    # now open it again and send it as the xfoil commands
-    # CREATE_NO_WINDOW = 0x08000000   # flag to create no window, should work on both Windows and Linux??
-    with open(xfoil_cmnd_file, 'r') as f:
-        # if hide_windows:
-        #     create_kw = {'creationflags': subprocess.CREATE_NO_WINDOW}
-        # else:
-        #     create_kw = {}
-
-        sui = subprocess.STARTUPINFO()
-        if hide_windows:
-            sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-
-        if verbose:
-            out, err = None, None
-        else:
-            out, err = subprocess.DEVNULL, subprocess.DEVNULL
-
-        subprocess.run([xfoil_fpath], startupinfo=sui, stdin=f, stdout=out, stderr=err,
-                       timeout=tmout, cwd=xfoil_dir)
-        # subprocess.run([xfoil_fpath], stdin=f, stdout=out, stderr=err, timeout=tmout, cwd=xfoil_dir,
-        #                **create_kw)
-        # p = subprocess.Popen([xfoil_fpath], stdin=f, stdout=out, stderr=err, cwd=xfoil_dir, **create_kw)
-        # p.wait(timeout=tmout)
-
-    # delete the temp command file
-    os.remove(xfoil_cmnd_file)
-
-
-def read_xfoil_pacc_file(fpath: str = None, delete_after: bool = False):
-    # if not given, default fpath is this
-    if not fpath:
-        fpath = os.path.join(_get_user_settings()['airfoil_database'], 'polar_output.txt')
-
-    # open fpath and read in all text
-    with open(fpath, 'r') as f:
-        txt = f.read()
-
-    # split into lines, create a dictionary, and iterate over the lines
-    lines = [line for line in txt.split('\n') if line.strip() != '']
-    d = {}
-    for i, line in enumerate(lines):
-        if i == 1:  # foil name on line 1
-            d['name'] = line.split(':')[1].strip()
-        elif i == 4:  # mach, re, and ncrit on line 4
-            mach, rest = line.split('Mach')[1].split('Re')
-            d['mach'] = float(mach.replace('=', '').strip())
-            re, ncrit = rest.split('Ncrit')
-            d['re'] = int(float(re.replace('=', '').replace(' ', '')))
-            d['ncrit'] = int(float(ncrit.replace('=', '').strip()))
-        elif i == 5:  # variable names on line 5, create an empty list for each one
-            var_names = [name for name in line.strip().split(' ') if name != '']
-            for key in range(len(var_names)):
-                d[key] = []
-        elif i >= 7:  # rest of lines in file contain variable entries for each variable
-            vals = [val for val in line.strip().split(' ') if val != '']
-            for col, val in enumerate(vals):
-                if vals[0] not in d[0]:  # if the alpha value of this line is not already in the list of alphas
-                    d[col].append(float(val))  # store with key as value index <- why am i doing it like this tho?
-                else:
-                    print('did not append over duplicate in col {} on line {}'.format(col, i - 7))
-
-    # re-assign dictionary keys to be variable names instead of indexes
-    for i, key in enumerate(var_names):
-        d[key] = d[i]
-        del d[i]
-
-    if [len(v) for v in d.values() if isinstance(v, list)][0] == 0:
-        return None
-
-    # sort each variable based on alpha and re-assign to each dictionary key
-    sort_list = d['alpha'].copy()
-    for key in var_names:
-        a, sorted_vals = list(zip(*sorted(zip(sort_list, d[key]))))
-        d[key] = np.array(sorted_vals)
-
-    # calculate L/D
-    d['CL/CD'] = d['CL'] / d['CD']
-
-    # if desired, delete the pacc file
-    if delete_after:
-        os.remove(fpath)
-
-    return d
-
-
-def read_polar_data_file(fpath: str):
-    with open(fpath, 'r') as f:
-        txt = f.read()
-
-    # create a dictionary and go thru all the lines and populate dictionary of strings
-    polar_data = {}
-    lines = txt.split('\n')
-    for i, line in enumerate(lines):
-        if i == 0:
-            name = line
-        elif not i == 1:
-            if '*****' in line:
-                d = {'name': name}
-                pairs = line.strip('*').strip().split(', ')
-                for pair in pairs:
-                    key, val = pair.split(' = ')
-                    d[key.lower()] = val
-            elif not line.strip() == '':
-                key, val = line.split(': ')
-                d[key] = val
-            else:
-                polar_data[(d['re'], d['mach'], d['ncrit'])] = d
-
-    # convert all the strings into what they're supposed to be
-    for str_key, polar in list(polar_data.items()):
-        re_key, mach_key, ncrit_key = str_key
-        for key, val in polar.items():
-            if '(' in val:
-                vals = [float(i.strip()) for i in val.replace('(', '').replace(')', '').split(',')]
-                polar[key] = np.array(vals)
-            elif 're' in key or 'ncrit' in key:
-                polar[key] = int(val)
-            elif 'mach' in key:
-                polar[key] = float(val)
-        new_key = (int(float(re_key)), float(mach_key), int(float(ncrit_key)))
-        polar_data[new_key] = polar.copy()
-        del polar_data[str_key]
-
-    return polar_data
-
-
-def save_polar_data_file(polar_data: dict, savepath: str, name: str = None):
-    if not name:
-        name = 'unnamed airfoil'
-    with open(savepath, 'w') as f:
-        f.write('{}\n'.format(name))
-        for polar_key in polar_data:
-            d = polar_data[polar_key]
-            re, mach, ncrit = polar_key
-            f.write('\n***** Re = {}, Mach = {}, nCrit = {} *****\n'.format(re, mach, ncrit))
-            keys_2_write = [key for key, val in d.items() if isinstance(val, np.ndarray)]
-            for key in keys_2_write:
-                f.write('{}: {}\n'.format(key, tuple(d[key])))
-    return
-
-
-def read_xrotor_op_file(fpath: str):
-    with open(fpath, 'r') as f:
-        txt = f.read()
-    if '********** NOT CONVERGED **********' in txt:
-        raise Error('XROTOR did not converge')
-    lines = txt.split('\n')
-    d = {}
-    headers = None
-
-    for line in lines:
-        if line.strip('-').strip('=').strip() == '':
-            pass  # ignore blank lines
-        elif ':' in line:   # top section
-            spl = [l.strip() for l in line.split(':')]
-            for i in range(len(spl) - 1):
-                key = spl[i].split('  ')[-1].strip()
-                val = spl[i + 1].split('  ')[0].strip()
-                if val[0].isnumeric() or val[1].isnumeric():
-                    d[key] = float(val)
-                else:
-                    d[key] = val
-        else:   # listout at bottom
-            vals = [val.strip() for val in line.replace('-', ' -').replace('s', ' ').split(' ') if val != '']
-            if headers is None:
-                headers = vals.copy()
-                for h in headers:
-                    d[h] = []
-            else:
-                for i, val in enumerate(vals):
-                    try:
-                        d[headers[i]].append(float(val))
-                    except ValueError:
-                        d[headers[i]].append(np.nan)
-
-    # go thru and turn into np.arrays now
-    for h in headers:
-        d[h] = np.array(d[h])
-
-        if 'REx10^' in h:  # detect and convert RE order of magnitude
-            old_res = d.pop(h)
-            exponent = int(h.strip('REx10^'))
-            d['RE'] = old_res * 10 ** exponent
-
-    return d
-
-
-def read_xrotor_cput_file():
-    return
-
-
-def read_2col_file(fpath: str, del_after: bool = True):
-    with open(fpath, 'r') as f:
-        txt = f.read().strip()
-    col1 = []
-    col2 = []
-    lines = txt.split('\n')
-    for line in lines:
-        val1, val2 = line.strip().split(' ', 1)
-        col1.append(float(val1.strip()))
-        col2.append(float(val2.strip()))
-
-    if del_after:
-        os.remove(fpath)
-
-    return np.array(col1), np.array(col2)
-
-
-def read_profile_xyz(fpath: str):
-    with open(fpath, 'r') as f:
-        txt = f.read().strip()
-    lines = txt.split('\n')[1:]
-
-    xpts, ypts, zpts = [], [], []
-    for line in lines:
-        xval, yval, zval = [float(val) for val in line.split(', ')]
-        xpts.append(xval)
-        ypts.append(yval)
-        zpts.append(zval)
-
-    return np.vstack([np.array(xpts), np.array(ypts), np.array(zpts)])
-
-
-# =============== INTERFACING WITH 3RD PARTY PROGRAMS ===============
-def download_foil_coordinates(foil_str: str):
-    foil_str = '{}.dat'.format(foil_str) if not foil_str.endswith('.dat') else foil_str
-    coord_url = 'https://m-selig.ae.illinois.edu/ads/coord/{}'.format(foil_str)
-    savepath = os.path.join(get_foil_db(), foil_str)
-    Info('Attempting to download "{}"...'.format(coord_url))
-    try:
-        urllib.request.urlretrieve(coord_url, savepath)
-        Info('saved to "{}"'.format(savepath), indent_level=1)
-        return True
-    except urllib.error.HTTPError:
-        Warning('Unable to download, not found')
-        return False
-
-
-def read_radial_stations(prop: Propeller, plot_also: bool = True, verbose: bool = False):
-    stations = []
-    if not os.path.exists(prop.station_polar_folder):
-        return stations
-
-    fnames = os.listdir(prop.station_polar_folder)
-    for fname in fnames:
-        roR, foil_name = fname.replace('.polar', '').split('_')
-        roR = float(roR)
-        fpath = os.path.join(prop.station_polar_folder, fname)
-        with open(fpath, 'r') as f:
-            txt = f.read().strip()
-        lines = txt.split('\n')
-
-        pol = {}
-        for line in lines:
-            key, val_str = line.split(':', 1)
-            if ',' in val_str:
-                val = np.array([float(v.strip()) for v in val_str.split(',')])
-            else:
-                val = float(val_str.strip())
-            pol[key] = val
-        st = RadialStation(foil_polar=pol, momma=prop, re_estimate=pol['re'], mach_estimate=pol['mach'],
-                           ncrit_estimate=pol['ncrit'], Xisection=roR, plot=plot_also, verbose=verbose,
-                           foil_name_str=foil_name)
-        stations.append(st)
-
-    return stations
-
-
-def create_radial_stations(prop: Propeller, plot_also: bool = True, verbose: bool = True):
-    # get density for Re estimates
-    if prop.design_atmo_props['altitude_km'] == -1:
-        rho, nu = 1000, 0.1150e-5
-        mu = nu * rho
-    else:
-        atmo = standard_atmosphere(prop.design_atmo_props['altitude_km'])# temp, p, rho, sonic_a, mu
-        mu, rho = atmo['mu'], atmo['rho']
-        nu = mu / rho
-
-    # replace it if it was entered as atmo prop as well
-    if 'dens' in prop.design_atmo_props:
-        rho = prop.design_atmo_props['dens']
-
-    t = ''
-    stations = []
-    for idx, xi in enumerate(prop.station_params):  # append station text all together and save
-        if verbose:
-            Info('Auto-generating section inputs from airfoil database data for section {} ({})...'.
-                  format(idx + 1, prop.station_params[xi]))
-        fn = prop.station_params[xi]
-        foil = Airfoil(name=fn, verbose=verbose)
-        re_est = int(calc_rotational_re(rho=rho, rpm=prop.design_rpm, radius=prop.radius * xi, chord=prop.radius / 10,
-                                        mu=mu, vel=prop.design_speed_mps, adv=prop.design_adv))
-        st = RadialStation(station_idx=idx, Xisection=xi, foil=foil, re_estimate=re_est, plot=plot_also, verbose=verbose)
-        t += st.generate_txt_params()
-        stations.append(st)
-    return stations, t
-
-
-def run_xrotor_oper(xrr_file: str, vorform: str, adva: float = None, rpm: float = None, thrust: float = None,
-                    torque: float = None, power: float = None, velo: float = None, hide_windows: bool = True,
-                    verbose: bool = True, tmout: int = None, xrotor_verbose: bool = False):
-
-    # increase the timeout for vrtx
-    if tmout is None and vorform.lower() == 'vrtx':
-        tmout = 25
-    elif tmout is None:
-        tmout = 10
-
-    # vorform has to be one of these three things
-    if vorform.lower() not in ['grad', 'pot', 'vrtx']:
-        raise Error('Input "vorform" must be one of ["grad", "pot", "vrtx"]')
-
-    # filename stuff
-    dirname, fname = os.path.split(xrr_file)
-    relpath = os.path.join(os.path.split(dirname)[1], fname)
-
-    # first we set the vorform
-    cmnds = ['load {}\n'.format(relpath), 'oper', 'form', '{}\n'.format(vorform)]
-
-    # if we are changing the velo, do that next
-    if velo is not None:
-        cmnds.extend(['velo', '{}'.format(velo), 'rein\n\ny'])
-
-    # can only be changing 1 of the 5 at a time
-    non_none_kwargs = [i for i in [adva, rpm, thrust, torque, power] if i is not None]
-    if len(non_none_kwargs) > 1:
-        raise Error('Can only change 1 of (adva, rpm, thrust, torque, power) at a time')
-
-    # command text based on which one was given
-    if adva is not None:
-        cmnds.extend(['adva', str(adva)])
-    elif rpm is not None:
-        cmnds.extend(['rpm', str(rpm)])
-    elif thrust is not None:
-        cmnds.extend(['thrust', str(thrust), 'p'])
-    elif torque is not None:
-        cmnds.extend(['torque', str(torque), 'p'])
-    elif power is not None:
-        cmnds.extend(['power', str(power), 'p'])
-    else:  # all were None
-        pass
-
-    # remove the output files if they exist for some reason already
-    oper_out_file, oper_out_fullpath = 'oper_out.txt', os.path.join(get_prop_db(), 'oper_out.txt')
-    wvel_out_file, wvel_out_fullpath = 'wvel_out.txt', os.path.join(get_prop_db(), 'wvel_out.txt')
-    if os.path.exists(oper_out_fullpath):
-        os.remove(oper_out_fullpath)
-    if os.path.exists(wvel_out_fullpath):
-        os.remove(wvel_out_fullpath)
-
-    # finalize the list of commands and write them to a file
-    cmnds.extend(['writ {}'.format(oper_out_file), 'wvel {}'.format(wvel_out_file), '\n\nquit\n'])
-    xrotor_cmnd_file = os.path.join(get_prop_db(), 'oper_run_inputs.txt')
-    with open(xrotor_cmnd_file, 'w') as f:
-        f.write('\n'.join(cmnds))
-
-    # run the mutha
-    xrotor_fpath = os.path.join(get_prop_db(), 'xrotor.exe')
-    with open(xrotor_cmnd_file, 'r') as f:
-        sui = subprocess.STARTUPINFO()
-        if hide_windows:
-            sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        if verbose:
-            Info('Running XROTOR for off-design operating point...', indent_level=1)
-        if xrotor_verbose:
-            out_err_kw = {}
-        else:
-            out_err_kw = {'stdout': subprocess.DEVNULL, 'stderr': subprocess.STDOUT}
-
-        subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, **out_err_kw,
-                       timeout=tmout, cwd=get_prop_db())
-
-    # get the returned velo and rpm for naming reasons
-    oper_output = read_xrotor_op_file(oper_out_fullpath)
-    returned_velo = oper_output['speed(m/s)']
-    returned_rpm = oper_output['rpm']
-
-    # rename / move the output files into the database
-    oper_savedir = os.path.join(os.path.split(oper_out_fullpath)[0], dirname, 'oper_data')
-    if not os.path.exists(oper_savedir):
-        os.mkdir(oper_savedir)
-    oper_copypath = os.path.join(oper_savedir, 'velo_{:.0f}_rpm_{:.0f}.oper'.format(100 * returned_velo, returned_rpm))
-    shutil.copyfile(oper_out_fullpath, oper_copypath)
-
-    wvel_savedir = os.path.join(os.path.split(wvel_out_fullpath)[0], dirname, 'wvel_data')
-    if not os.path.exists(wvel_savedir):
-        os.mkdir(wvel_savedir)
-    wvel_copypath = os.path.join(wvel_savedir, 'velo_{:.0f}_rpm_{:.0f}.wvel'.format(100 * returned_velo, returned_rpm))
-    shutil.copyfile(wvel_out_fullpath, wvel_copypath)
-
-    # delete the temporary files
-    os.remove(xrotor_cmnd_file)
-    os.remove(oper_out_fullpath)
-    os.remove(wvel_out_fullpath)
-
-    return
-
-
-def read_xrotor_wvel_file(fpath:str):
-    with open(fpath, 'r') as f:
-        txt = f.read().strip()
-    lines = [ln.strip() for ln in txt.split('\n') if ln != '']
-
-    data = {}
-    for i, line in enumerate(lines):
-        line = line.replace('=', '= ')
-        words = [w.strip() for w in line.split(' ') if w != '']
-        if i in [3, 4]:
-            for j, word in enumerate(words):
-                if 'rpm' in word.lower():
-                    data['rpm'] = float(words[j + 1])
-                elif 'vel' in word.lower():
-                    data['vel'] = float(words[j + 1])
-                elif 'beta_tip' in word.lower():
-                    data['beta_tip'] = float(words[j + 1])
-                elif 'power' in word.lower():
-                    try:
-                        data['power'] = float(words[j + 1])
-                    except ValueError:
-                        data['power'] = np.nan
-                elif 'thrust' in word.lower():
-                    try:
-                        data['thrust'] = float(words[j + 1])
-                    except ValueError:
-                        data['thrust'] = np.nan
-        elif i == 6:
-            headers = [ln.strip() for ln in line.replace(' + ', '+').split(' ') if ln != '']
-            for header in headers:
-                data.setdefault(header, [])
-        elif i > 6:
-            vals = [ln.strip() for ln in line.split(' ') if ln != '']
-            for v, val in enumerate(vals):
-                data[headers[v]].append(float(val))
-
-    return data
-
-
-def create_propeller(name: str, nblades: int, radius: float, hub_radius: float, hub_wake_disp_br: float,
-                     design_speed_mps: float, design_cl: dict, design_atmo_props: dict, design_vorform: str,
-                     station_params: dict = None, design_adv: float = None, design_rpm: float = None,
-                     design_thrust: float = None, design_power: float = None, n_radial: int = 50,
-                     verbose: bool = False, show_station_fit_plots: bool = True, plot_after: bool = True,
-                     tmout: int = None, hide_windows: bool = True, geo_params: dict = {}, xrotor_verbose: bool = False):
-    # adjust timeout for vrtx
-    if tmout is None and design_vorform == 'vrtx':
-        tmout = 100
-    elif tmout is None:
-        tmout = 30
-
-    # name must be less than 38? characters for XROTOR to be able to save it
-    if len(name) > 38:
-        raise Error('"name" must be less than 38 characters when creating a propeller, "{}" is too long'.format(name))
-
-    # must input an altitude in atmo props
-    if 'altitude_km' not in design_atmo_props:
-        raise Error('You must include "altitude_km" as an input to create_propeller()')
-
-    # delete if exists already, make save folder, point-cloud folder
-    save_folder = os.path.join(get_prop_db(), name)
-    if os.path.exists(save_folder):
-        shutil.rmtree(save_folder)
-    os.mkdir(save_folder)
-
-    # make a folder for all the profile x, y, z listings
-    prof_folder = os.path.join(save_folder, 'blade_profiles')
-    os.mkdir(prof_folder)
-
-    # create the Propeller object, create the stations
-    prop = Propeller(name=name, nblades=nblades, radius=radius, hub_radius=hub_radius,
-                     hub_wake_disp_br=hub_wake_disp_br, design_speed_mps=design_speed_mps, design_cl=design_cl,
-                     design_atmo_props=design_atmo_props, design_vorform=design_vorform, design_adv=design_adv,
-                     station_params=station_params, geo_params=geo_params, design_rpm=design_rpm,
-                     design_thrust=design_thrust, design_power=design_power, verbose=verbose)
-    st_txt = prop.set_stations(plot_also=show_station_fit_plots, verbose=verbose)
-
-    # prep XROTOR commands depending on what station_params were input
-    aero_params_fname = '{}_temp_section_params.txt'.format(name)
-    aero_params_fpath = os.path.join(get_prop_db(), aero_params_fname)
-    with open(aero_params_fpath, 'w') as f:
-        f.write(st_txt)
-
-    # prep XROTOR commands depending on what design_atmo_props were given
-    alt = design_atmo_props['altitude_km']
-    atmo_txt = '{}\n\n'.format(alt)
-
-    if 'vsou' in design_atmo_props:
-        vsou = design_atmo_props['vsou']
-        atmo_txt += 'vsou\n{}\n'.format(vsou)
-    if 'dens' in design_atmo_props:
-        dens = design_atmo_props['dens']
-        atmo_txt += 'dens\n{}\n'.format(dens)
-    if 'visc' in design_atmo_props:
-        visc = design_atmo_props['visc']
-        atmo_txt += 'visc\n{}\n'.format(visc)
-    atmo_txt += 'desi'
-
-    # prep XROTOR commands depending on what vortex formulation is given
-    if design_vorform is None:
-        vorform_txt = 'pot\n'
-    elif any([design_vorform.lower() == i for i in ['grad', 'pot', 'vrtx']]):
-        vorform_txt = '{}\n'.format(design_vorform.lower())
-
-    # prep XROTOR commands for the advance ratio OR RPM design specification
-    if design_adv is not None:
-        if design_rpm is not None:
-            raise Error('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
-        adv_rpm_txt = '{}'.format(design_adv)
-    elif design_rpm is not None:
-        if design_adv is not None:
-            raise Error('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
-        adv_rpm_txt = '{}\n{}'.format(0, design_rpm)
-
-    # prep XROTOR commands for the thrust OR power design specification
-    if design_thrust is not None:
-        thr_pow_txt = '{}'.format(design_thrust)
-    elif design_power is not None:
-        thr_pow_txt = '{}\n{}'.format(0, design_power)
-
-    # prep XROTOR commands depending on what design_cl keys were given
-    if len(design_cl) == 1:  # either a constant value was given, or a filepath
-        if 'const' in design_cl:
-            const_cl = design_cl['const']
-            cl_txt = 'cc\n{}\n\n'.format(const_cl)
-        elif 'file' in design_cl:
-            fpath = design_cl['file']
-            cl_txt = 'cr\n{}\n\n'.format(fpath)
-        else:
-            raise Error('Must give either a "const" CL target (constant), a "root" and "tip" CL target '
-                        '(linearly varied), or specify a CL(r/R) .txt file')
-    elif len(design_cl) == 2:  # a linear cl was given
-        if all([k in design_cl for k in ['root', 'tip']]):
-            root_cl = design_cl['root']
-            tip_cl = design_cl['tip']
-            cl_txt = 'cl\n{}\n{}\n\n'.format(root_cl, tip_cl)
-        else:
-            raise Error('If only 2 keywords are given in "design_cl", they must be "root" and "tip"')
-    else:
-        raise Error('"design_cl" input dictionary error, either too many or not enough keys (if a single key'
-                    'is given, it must be either "const" or "file", if 2 keys are given they must be "root" '
-                    'and "tip"')
-
-    # prep XROTOR commands for saving blade data r/R
-    blade_data_keys = ['CH', 'BE', 'GAM', 'CL', 'CD', 'RE', 'EFP', 'Ub', 'VA', 'VT', 'VD', 'VA/V', 'VT/V', 'VD/V',
-                       'VAslip', 'VTslip', 'Aslip', 'Ti', 'Pi', 'Tv', 'Pv', 'Ttot', 'Ptot', 'Xw', 'Vw', 'Tw', 'Pw']
-    blade_data = {}
-    blade_txt = 'plot\n12\n'
-    for key in blade_data_keys:
-        fname = '{}_out.txt'.format(key.replace('/', '_over_'))
-        blade_data[key] = None
-        blade_txt += 'o\n{}\nw\n{}\n'.format(key, fname)
-
-    # prep XROTOR commands to save the solved operating point params
-    op_fpath = '{}\\{}.xrop'.format(name, name)
-    save_op_txt = 'oper\nwrit\n{}\n'.format(op_fpath)
-
-    # prep XROTOR commands for savename
-    savename = '{}\\{}.xrr'.format(name, name)
-    save_txt = 'save {}\nquit\n'.format(savename)
-
-    # write XROTOR commands to a file and run in a subprocess
-    xrotor_cmnd_file = os.path.join(get_prop_db(), 'xrotor_inputs_temp.txt')
-    cmnds = ['aero', 'read', '{}\n'.format(aero_params_fname),
-             'desi', 'atmo', '{}'.format(atmo_txt), 'form', '{}'.format(vorform_txt), 'N', '{}'.format(n_radial),
-             'inpu', '{}'.format(nblades),
-             '{}'.format(radius), '{}'.format(hub_radius), '{}'.format(hub_wake_disp_br), '{}'.format(design_speed_mps),
-             '{}'.format(adv_rpm_txt), '{}'.format(thr_pow_txt), '0', '{}'.format(cl_txt), '{}'.format(blade_txt), '\n',
-             '{}'.format(save_op_txt), '\n\n', '{}'.format(save_txt)]
-
-    with open(xrotor_cmnd_file, 'w') as f:
-        f.write('\n'.join(cmnds))
-
-    xrotor_fpath = os.path.join(get_prop_db(), 'xrotor.exe')
-    with open(xrotor_cmnd_file, 'r') as f:
-        sui = subprocess.STARTUPINFO()
-        if hide_windows:
-            sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        if verbose:
-            Info('Running XROTOR to create new geometry...')
-        if xrotor_verbose:
-            subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, timeout=tmout, cwd=get_prop_db())
-        else:
-            subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT,
-                           timeout=tmout, cwd=get_prop_db())
-    os.remove(xrotor_cmnd_file)
-    os.remove(aero_params_fpath)
-
-    # set the prop's blade-data that we just saved in creation
-    for key in blade_data.copy():
-        fp = os.path.join(get_prop_db(), '{}_out.txt'.format(key.replace('/', '_over_')))
-        roR, array = read_2col_file(fpath=fp)
-        if 'r/R' not in blade_data:
-            blade_data['r/R'] = roR
-        blade_data[key] = array
-    prop.set_blade_data(blade_dict=blade_data)
-
-    # interpolate the profiles as part of geometry creation
-    if 'n_prof_pts' not in geo_params:
-        geo_params['n_prof_pts'] = None
-    if 'n_profs' not in geo_params:
-        geo_params['n_profs'] = 50
-    if 'tot_skew' not in geo_params:
-        geo_params['tot_skew'] = 0.0
-
-    prop.interp_foil_profiles(**geo_params)  # also saves the profiles
-
-    # save the PDT propeller meta-file, and then read in the operating point dictionary by calling load_from_savefile()
-    prop.xrotor_op_dict = read_xrotor_op_file(prop.xrop_file)
-    prop.save_station_polars()
-    prop.save_meta_file()
-    prop.load_from_savefile(verbose=verbose)   # reads meta, xrr, xrop, and point clouds
-
-    if not verbose:
-        Info('"{}" Geometry Created!'.format(prop.name))
-    if plot_after:
-        prop.plot_design_point_panel()
-
-    return prop
-
-
-def write_blade_cl_file(r_pts: list, cl_pts: list, savepath: str = None):
-    if savepath is None:
-        savepath = 'blade_design_cl.txt'
-    with open(savepath, 'w') as f:
-        for r, cl in zip(r_pts, cl_pts):
-            f.write('   {r: .6f}      {cl: .6f}\n'.format(r=r, cl=cl))
-
-
-def convert_ps2png(ps_fpath: str, return_pil_img: bool = False, show_in_pyplot: bool = False):
-    """
-    Function that converts a PostScript (.ps) image file to a .png file.  Uses 3rd party GNU licensed
-    GhostScript, which is capable of much more than just .ps to .png conversion.
-
-    :param ps_fpath: the filepath to the PostScript file
-    :param return_pil_img: returns a PIL image object if True, by default just returns the PNG filepath
-    :param show_in_pyplot: displays the image in a pyplot figure if True, default is False
-    :return png_fpath: the filepath to the converted file
-    :return pil_img: the PIL image object
-    :return fig: the pyplot figure object
-    """
-    png_fpath = ps_fpath.replace('.ps', '.png')
-    gs_cmnds = ['gswin64c.exe', '-dSAFER', '-dBATCH', '-dNOPAUSE', '-sDEVICE=png16m',
-                '-dGraphicsAlphaBits=4', '-sOutputFile={}'.format(png_fpath), '{}'.format(ps_fpath)]
-    subprocess.run(gs_cmnds, stdout=subprocess.DEVNULL)  # stderr=subprocess.DEVNULL
-
-    if not return_pil_img and not show_in_pyplot:
-        return png_fpath
-
-    from PIL import Image
-    pil_img = Image.open(png_fpath)
-
-    if return_pil_img:
-        return pil_img
-
-    fig = plt.figure(figsize=[9, 11])
-    ax = fig.add_subplot(111)
-    ax.axis('off')
-    ax.imshow(pil_img)
-    fig.tight_layout()
-    return fig
-
-
-# =============== MODELING / PHYSICS ===============
-def calc_linear_re(rho: float, vel: float, length: float, mu: float):
-    return rho * vel * length / mu
-
-
-def calc_rotational_re(rho: float = None, vel: float = None, chord: float = None, mu: float = None, rpm: float = None,
-                       radius: float = None, adv: float = None):
-    if all([i is not None for i in [rho, rpm, radius, chord, mu]]):
-        re = rho * (rpm / 60 * 2 * np.pi) * radius * chord / mu
-    elif all([i is not None for i in [rho, vel, adv, radius, chord, mu]]):
-        rpm = vel / np.pi / 2 / radius / adv * 60
-        re = rho * (rpm / 60 * 2 * np.pi) * radius * chord / mu
-    else:
-        raise Error('Must input all of either [rho, vel, chord, mu] or [rho, rpm, radius, chord, mu]')
-    return re
-
-
-def standard_atmosphere(altitude_km: float) -> dict:  # standard atmosphere eqs from Jake's college prof.
-
-    alt_m = altitude_km * 1000
-
-    g, R_air, gamma_air = 9.80665, 287.05307, 1.4
-    alt1, alt2, alt3 = 11000, 20000, 32000
-    temp0, p0, rho0, mu0 = 288.15, 101325, 1.2250, .0000181206
-    slope0, slope1, slope2 = -.0065, 1, .001
-
-    temp1 = temp0 + slope0 * alt1
-    p1 = p0 * (temp1 / temp0) ** (-g / slope0 / R_air)
-    rho1 = rho0 * (temp1 / temp0) ** (-g / slope0 / R_air - 1)
-
-    temp2 = temp1
-    p2 = p1 * np.exp(-g / R_air / temp2 * (alt2 - alt1))
-    rho2 = rho1 * np.exp(-g / R_air / temp2 * (alt2 - alt1))
-
-    if alt_m < 0:
-        raise Error('Cannot input negative values into standard_atmosphere()')
-    elif alt_m < alt1:
-        temp = temp0 + slope0 * alt_m
-        p = p0 * (temp / temp0) ** (-g / slope0 / R_air)
-        rho = rho0 * (temp / temp0) ** (-g / slope0 / R_air - 1)
-    elif alt_m < alt2:
-        temp = temp1
-        p = p1 * np.exp(-g / slope1 / R_air / temp * (alt_m - alt1))
-        rho = rho1 * np.exp(-g / R_air / temp * (alt_m - alt1))
-    elif alt_m < alt3:
-        temp = temp2 + slope2 * (alt_m - alt2)
-        p = p2 * (temp / temp2) ** (-g / slope2 / R_air)
-        rho = rho2 * (temp / temp2) ** (-g / slope2 / R_air - 1)
-    else:
-        raise Error('Altitude out of range of atmosphere model')
-
-    sonic_a = np.sqrt(gamma_air * R_air * temp)
-    mu = mu0 * (temp / temp0) ** 1.5 * ((temp0 + 120) / (temp + 120))
-
-    return {'temp': temp, 'p': p, 'rho': rho, 'sonic_a': sonic_a, 'mu': mu}
-
-
-def xrotor_drag_model(CL: np.ndarray, CDmin: float, CLCDmin: float, dCDdCL2: float):
-    CD = CDmin + dCDdCL2 * (CLCDmin - CL) ** 2
-    return CD
-
-
-def get_xrotor_re_scaling_exp(re: int):     # THIS NEEDS WORK
-    # re_pts = [0, 1e5, 2e5, 8e5, 2e6, 3e6]
-    # f_pts = [-0.3, -0.5, -0.5, -1.5, -0.2, -0.1]
-    # return np.interp(x=re, xp=re_pts, fp=f_pts)
-    return -0.4
-
-
-def calc_thrust(k_t, rho, rpm, dia):
-    n = rpm / 60
-    return k_t * rho * n ** 2 * dia ** 4
-
-
-def calc_ideal_eff(thrust: float, rho: float, a_disk: float, u_o: float):
-    T = thrust
-    rho = rho
-    A_disk = a_disk
-    u_o = u_o
-    return 100 * 2 / (1 + (T / (A_disk * 1 / 2 * rho * u_o ** 2) + 1) ** (1 / 2))
-
-
-# ===== GEOMETRY MANIPULATION =====
-def generate_3D_profile_points(nondim_xy_coords: np.ndarray, radius: float, axis_shift: float = 0.5,
-                               chord_len: float = 1.0, beta_deg: float = 0.0, skew_deg: float = 0.0):
-    xpts, ypts = nondim_xy_coords.copy()
-
-    # mirror over y and shift (0, 0) to align to the blade axis
-    xpts = -xpts + axis_shift
-
-    # scale the profile by the chord length
-    xpts *= chord_len
-    ypts *= chord_len
-
-    # rotate profile by beta
-    b = np.deg2rad(beta_deg)
-    xp = xpts * np.cos(-b) + ypts * np.sin(-b)
-    yp = ypts * np.cos(-b) - xpts * np.sin(-b)
-
-    # create array of radii points, create array of theta points
-    rp = np.ones(len(xp)) * radius
-    thetas = xp / (2 * np.pi * radius) * 2 * np.pi    #map each xpos to a theta in radians
-
-    # apply skew
-    thetas += np.deg2rad(-skew_deg)
-
-    # wrap the ycoords
-    ys = rp * np.sin(thetas)
-    xs = rp * np.cos(thetas)
-    zs = yp
-
-    return np.vstack([xs, ys, zs])
-
-
-def unit_vector(vector):
-    """ Returns the unit vector of the vector.  """
-    return vector / np.linalg.norm(vector)
-
-
-def angle_between(v1, v2):
-    """ Returns the angle in radians between vectors 'v1' and 'v2'::
-
-            angle_between((1, 0, 0), (0, 1, 0))
-            1.5707963267948966
-            angle_between((1, 0, 0), (1, 0, 0))
-            0.0
-            angle_between((1, 0, 0), (-1, 0, 0))
-            3.141592653589793
-    """
-    v1_u = unit_vector(v1)
-    v2_u = unit_vector(v2)
-    return np.arccos(np.clip(np.dot(v1_u, v2_u), -1.0, 1.0))
-
-
-def compute_polygon_angles(exterior_coords: list):
-    if exterior_coords[0] == exterior_coords[-1]:
-        removed = exterior_coords.pop(-1)
-    angles = []
-    for i in range(len(exterior_coords)):
-        pt = exterior_coords[i]
-        last_pt = exterior_coords[i - 1]
-        if i == len(exterior_coords) - 1:
-            next_pt = exterior_coords[0]
-        else:
-            next_pt = exterior_coords[i + 1]
-
-        v1 = [next_pt[0] - pt[0], next_pt[1] - pt[1], next_pt[2] - pt[2]]
-        v2 = [last_pt[0] - pt[0], last_pt[1] - pt[1], last_pt[2] - pt[2]]
-        ang = angle_between(v1, v2)
-        angles.append(ang)
-    return angles
-
-
-def compute_profile_trimesh(profile_coords, reverse_order: bool = False):
-    if len(profile_coords) == 3:
-        xc, yc, zc = profile_coords
-    elif len(profile_coords) == 2:
-        xc, yc = profile_coords
-        zc = np.zeros(len(xc))
-    else:
-        raise ValueError('len of profile_coords must be either 2 or 3')
-    points = list(zip(xc, yc, zc))
-
-    # 1) For each vertex in the polygon, compute the angle between the two linked edges
-    # 2) Sort vertices by decreasing angle relative to the interior of the polygon
-    # 3) If there is less than 3 vertices in the set, we're done
-    # 4) Take the last vertex in the set and output the triangle formed by it and its two neighbours
-    # 5) Remove the vertex from the set
-    # 6) Update the angle of the two neighbours
-    # 7) Jump to 2
-
-    vectors = []
-    while len(points) >= 3:
-        angles = compute_polygon_angles(exterior_coords=points)
-        min_idx = np.argmin(angles)
-        prev_idx = min_idx - 1
-        if min_idx == len(angles) - 1:
-            next_idx = 0
-        else:
-            next_idx = min_idx + 1
-        pt1, pt2, pt3 = points[prev_idx], points[min_idx], points[next_idx]
-        if not reverse_order:
-            vector = [pt1, pt2, pt3]
-        else:
-            vector = [pt3, pt2, pt1]
-        vectors.append(vector)
-        _ = points.pop(min_idx)
-
-    return vectors
-
-
-# ===== USER INTERFACE STUFF =====
-def start_ui():
-    from PyQt5 import QtWidgets
-    from propdes.user_interface import InterfaceMainWindow
-    app = QtWidgets.QApplication(sys.argv)
-    w = InterfaceMainWindow()
-    w.show()
-    app.exec_()
-
-
-def delete_all_widgets_from_layout(layout):
-    for i in reversed(range(layout.count())):
-        layout.itemAt(i).widget().setParent(None)
+import os
+import subprocess
+import shutil
+import sys
+import urllib.request
+
+import matplotlib.pyplot as plt
+import numpy as np
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.radialstation import RadialStation
+from propeller_design_tools.propeller import Propeller
+from propeller_design_tools.user_io import Info, Error, Warning
+from propeller_design_tools.settings import _get_user_settings, get_prop_db, get_foil_db
+
+
+# =============== CONVENIENCE / UTILITY FUNCTIONS ===============
+def delete_propeller(prop, verbose: bool = True):
+    fpaths = [prop.xrr_file, prop.xrop_file, prop.meta_file]
+    rmvd = []
+    for path in fpaths:
+        if os.path.isfile(path):
+            os.remove(path)
+            rmvd.append(path)
+    if verbose:
+        Info('Removed paths: {}'.format(rmvd))
+
+
+def clear_foil_database(single_foil: str = None, inside_root_db: bool = False, inside_polar_db: bool = True,
+                        inside_for_xfoil: bool = True, verbose: bool = True):
+    """
+    Helper function to clear out files from foil database.
+
+    :param inside_root_db:
+    :param inside_polar_db:
+    :param inside_for_xfoil:
+    :return:
+    """
+    if single_foil is not None:
+        single_foil = '{}.dat'.format(single_foil) if not single_foil.endswith('.dat') else single_foil
+
+    foils_2_del = [single_foil] if single_foil is not None else get_all_airfoil_files()
+
+    for foil_file in foils_2_del:
+        foil_name = foil_file.replace('.dat', '')
+        if verbose:
+            Info('Clearing files for "{}"'.format(foil_name))
+
+        foil_fpath = os.path.join(_get_user_settings()['airfoil_database'], foil_file)
+        polar_fpath = os.path.join(_get_user_settings()['airfoil_database'], 'polar_database', '{}_polar_data.txt'.format(foil_name))
+        xfoil_fpath = os.path.join(_get_user_settings()['airfoil_database'], 'for_xfoil', '{}.txt'.format(foil_name))
+
+        if inside_root_db:
+            if os.path.exists(foil_fpath):
+                os.remove(foil_fpath)
+                if verbose:
+                    Info('Removed file "{}"'.format(foil_fpath), indent_level=1)
+        if inside_polar_db:
+            if os.path.exists(polar_fpath):
+                os.remove(polar_fpath)
+                if verbose:
+                    Info('Removed file "{}"'.format(polar_fpath), indent_level=1)
+        if inside_for_xfoil:
+            if os.path.exists(xfoil_fpath):
+                os.remove(xfoil_fpath)
+                if verbose:
+                    Info('Removed file "{}"'.format(xfoil_fpath), indent_level=1)
+
+
+def clear_prop_database(inside_root_db: bool = True, inside_xrotor_files: bool = True, inside_op_files: bool = True):
+    """
+    Helper function to clear out files from prop database.
+
+    :param inside_op_files:
+    :param inside_root_db:
+    :param inside_xrotor_files:
+    :return:
+    """
+    if inside_root_db:
+        delete_files_from_folder(_get_user_settings()['propeller_database'])
+    if inside_xrotor_files:
+        delete_files_from_folder(os.path.join(_get_user_settings()['propeller_database'], 'xrotor_geometry_files'))
+    if inside_op_files:
+        delete_files_from_folder(os.path.join(_get_user_settings()['propeller_database'], 'xrotor_op_files'))
+
+
+def delete_files_from_folder(folder: str):
+    if os.path.exists(folder):
+        for filename in os.listdir(folder):
+            fpath = os.path.join(folder, filename)
+            if os.path.isfile(fpath):
+                os.remove(fpath)
+    else:
+        raise Error('Cannot find folder: {}'.format(folder))
+
+
+def count_airfoil_db():
+    return len(get_all_airfoil_files())
+
+
+def count_propeller_db():
+    return len(get_all_propeller_dirs())
+
+
+def get_all_airfoil_files():
+    af_db = get_foil_db()
+    fnames = []
+    for fname in os.listdir(af_db):
+        if os.path.splitext(fname)[1] in ['.dat', '.txt']:
+            fnames.append(fname)
+    return [name for name in fnames if name not in ['polar_output.txt', 'xfoil_inputs_temp.txt']]
+
+
+def get_all_propeller_dirs():
+    prop_db = get_prop_db()
+    dirnames = []
+    for name in os.listdir(prop_db):
+        pth = os.path.join(prop_db, name)
+        if os.path.isdir(pth):
+            if any([os.path.splitext(p)[1] == '.meta' for p in os.listdir(pth)]):
+                dirnames.append(name)
+    return dirnames
+
+
+def search_files(folder: str, search_strs: list = None, contains_any: bool = False, include_dirs: bool = False):
+    """
+    Utility function to help users interface with getting files from folders
+
+    :param folder: the full path to the folder to look in
+    :param search_strs: a list of strings to search for in each filename
+    :param contains_any: If True will return files that contain ANY of the search strings, defaults to False (returns only
+        filenames that contain ALL of the search strings)
+    :return: a list of filenames
+    """
+
+    if not os.path.exists(folder):
+        raise Error('PDT ERROR: No folder named "{}" found!'.format(folder))
+
+    if include_dirs:
+        files = os.listdir(folder)
+    else:
+        files = [f for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f))]
+
+    if search_strs == []:
+        search_strs = None
+
+    if search_strs is not None:
+        # for s in search_strs:
+        #     files = []
+        if contains_any:  # ANY
+            files = [f for f in files if any([s in f for s in search_strs])]
+        else:  # ALL
+            files = [f for f in files if all([s in f for s in search_strs])]
+
+    return files
+
+
+def get_airfoil_file_from_db(foil_name: str, exact_namematch: bool = False):
+    db_dir = _get_user_settings()['airfoil_database']
+    possible_files = search_files(folder=db_dir, search_strs=[foil_name])
+    exact_fname = '{}.dat'.format(foil_name)
+
+    if len(possible_files) == 1:
+        if not exact_namematch:
+            return possible_files[0]
+        else:   # must match exactly
+            if possible_files[0] == exact_fname:
+                return possible_files[0]
+            else:
+                raise Error('Did not find an exact match for "{}"'.format(exact_fname))
+
+    elif len(possible_files) == 0:
+        raise Error('Did not find any coordinate files containing name "{}" when looking in user-set airfoil '
+                    'database: {}'.format(foil_name, db_dir))
+
+    else:   # found multiple files
+        if not exact_namematch:
+            raise Error('Found multiple coordinate files looking for airfoil "{}"!\n{}\n'
+                        'Consider using kwarg exact_namematch=True'.format(foil_name, possible_files))
+        else:
+            possible_files = [f for f in possible_files if f == exact_fname]
+            if len(possible_files) == 0:
+                raise Error('Did not find any coordinate files exactly matching "{}"'.format(exact_fname))
+            else:
+                return possible_files[0]
+
+
+def merge_polar_data_dicts(new: dict, old: dict):
+    if len(old) == 0:  # there was no old data
+        return new
+
+    new_pol_keys = new[list(new.keys())[0]].keys()
+    merged = new.copy()  # merged starts out as copy of the new dict
+    for old_pol_key, old_pol in old.items():  # cylce thru old dict
+        if old_pol_key not in new.keys():  # if saved (re, mach, ncrit) data not in new data
+            if old_pol.keys() == new_pol_keys:  # if keys are the same (alpha, CL, CD, etc)
+                merged[old_pol_key] = old_pol  # append and move on
+            else:  # if keys aren't same, warn that data isn't being retained
+                print('Warning: found saved polar data of older/incorrect format -> deleting {}'.format(old_pol_key))
+        else:  # if saved (re, mach, ncrit) data in new data
+            if old_pol.keys() == new_pol_keys:  # if same keys (alpha, CL, CD, etc) inform of overwrite
+                pass
+                # print('Warning: overwriting saved polar data for {}'.format(old_pol_key))
+            else:  # if not same keys
+                print('Warning: overwriting saved polar data for {} (was older/incorrect format)'.format(old_pol_key))
+    return merged
+
+
+def scrub_nans(d: dict):
+    # get all the indices where there's nans
+    nan_idxs = []
+    for key, val in d.items():
+        if hasattr(val, '__len__'):     # only consider arrays / lists
+            idxs = np.where(np.isnan(val))[0]
+            nan_idxs.extend(list(idxs))
+    nan_idxs = list(set(nan_idxs))
+
+    # now cycle through and create a new dictionary without nans
+    new_d = {}
+    for key, val in d.items():
+        if isinstance(val, list):   # if it's a list, return a list
+            new_d[key] = [v for i, v in enumerate(val) if i not in nan_idxs]
+        elif isinstance(val, np.ndarray):   # if it's a np array, return an np array
+            new_d[key] = np.array([v for i, v in enumerate(val) if i not in nan_idxs])
+        else:   # otherwise, just stuff it back in to the new dictionary un-altered
+            new_d[key] = val
+
+    return new_d
+
+
+# =============== FILE READING / WRITING FUNCTIONS ===============
+def read_airfoil_coordinate_file(fpath: str, verbose: bool = True, te_gap_set: float = 0.004):
+    """
+    Function to read an airfoil coordinate listing file in .dat or .txt format, assumes foil name is on
+    1st line, then reads in the list of coordinates following (ignoring any lines with numbers > 1.0, and
+    assuming the coordinates are single-space delimited) -> this is the file format as downloaded from
+
+    https://m-selig.ae.illinois.edu/ads/coord_database.html
+
+    It then splits the coordinates into upper and lower, and determines if either needs to be reversed
+    (in order to read into xfoil right and also plot correctly), then reverses them if needed and returns
+    arrays of x, y coords.
+
+    :param
+        fpath: the full filepath to the coordinate file
+    :return
+        name: the name of the airfoil from line1
+        x_coords: np.array of x-coordinates
+        y_coords: np.array of y-coordinates
+    """
+
+    # open the file and read contents
+    with open(fpath, 'r') as f:
+        txt = f.read()
+
+    # prep arrays
+    x_coords = np.array([])
+    y_coords = np.array([])
+
+    # split the text on returns and iterate over the lines
+    lines = txt.strip(' ').split('\n')
+    for i, line in enumerate(lines):
+        # assumes name of airfoil is on line 0
+        if i == 0:
+            name = line.strip(' ')
+        else:
+            if not line.strip(' ') == '':  # skips blank lines
+                vals = line.strip(' ').split(' ')  # split text on blank spaces
+                x = float(vals[0])  # x coord is the 0th element
+                y = float(vals[-1])  # y coord is the last element
+                if x <= 1:  # only append if x in the range [0,1]
+                    x_coords = np.append(x_coords, x)
+                if y <= 1:  # only append if y in the range [0,1]
+                    y_coords = np.append(y_coords, y)
+
+    # make lists of coordinates, upper, and lower
+    coords = np.array(list(zip(x_coords, y_coords)))
+    x_directions = np.sign(np.diff(x_coords))
+    x_directions = np.append(x_directions[0], x_directions)
+    upper_end_idx = np.where(np.abs(np.diff(x_directions)) == 2)[0][0]
+    upper_coords = coords[0:upper_end_idx + 1]
+    lower_coords = coords[upper_end_idx + 1:]
+
+    # flip upper if needed such that it is always decreasing in x
+    if not x_directions[0] == -1:
+        upper_coords = np.array(list(reversed(upper_coords)))
+
+    # flip lower if needed such that it is always increasing in x
+    if not x_directions[-1] == 1:
+        lower_coords = np.array(list(reversed(lower_coords)))
+
+    # check TE gap
+    te_gap = upper_coords[0][1] - lower_coords[-1][1]
+    blend_start = 0.7
+    if te_gap != te_gap_set:
+        total_dy = (te_gap_set - te_gap) / 2
+
+        upper_idxs = np.where(upper_coords[:, 0] > blend_start)[0]
+        for i in upper_idxs:
+            xc, yc = upper_coords[i]
+            dy = total_dy * (xc - blend_start) / (1 - blend_start)
+            yc += dy
+            upper_coords[i] = [xc, yc]
+
+        lower_idxs = np.where(lower_coords[:, 0] > 0.8)[0]
+        for i in lower_idxs:
+            xc, yc = lower_coords[i]
+            dy = total_dy * (xc - blend_start) / (1 - blend_start)
+            yc -= dy
+            lower_coords[i] = [xc, yc]
+        if verbose:
+            Info('Detected airfoil ({}) with TE not equal to the requested value\n-> artificially adjusted TE gap to {} '
+                     '(normalized)'.format(name, te_gap_set))
+
+    # re-combine upper and lower coords and split back into x, y arrays
+    if upper_coords[-1][0] == lower_coords[0][0] and upper_coords[-1][1] == lower_coords[0][1]:  # check for double 0, 0
+        coords = np.append(upper_coords, lower_coords[1:], axis=0)
+    else:
+        coords = np.append(upper_coords, lower_coords, axis=0)
+
+    x_coords, y_coords = zip(*coords)
+    return name, np.array(x_coords), np.array(y_coords)
+
+
+def run_xfoil(foil_relpath: str, re: float, alpha: list = None, cl: list = None, iter_limit: int = 30, ncrit: int = 9,
+              mach: float = 0.0, output_fpath: str = None, keypress_iternum: int = 1, tmout: int = 25,
+              hide_windows: bool = True, verbose: bool = False):
+    if not output_fpath:
+        output_fpath = 'polar_output.txt'
+
+    # swept pacc param
+    if alpha is not None and cl is not None:
+        raise Error('Cannot give "run_xfoil" both "alpha" and "cl"')
+    elif alpha is not None:
+        swept_param = {'alpha': alpha}
+    elif cl is not None:
+        swept_param = {'cl': cl}
+    else:
+        raise Error('Must give "run_xfoil" either a list of "alpha" to sweep or a list of "cl" to sweep')
+
+    # sort the swept values
+    vals = list(sorted(list(swept_param.values())[0]))
+
+    # directory and temp command file, also xfoil path
+    xfoil_dir = _get_user_settings()['airfoil_database']
+    xfoil_cmnd_file = os.path.join(xfoil_dir, 'xfoil_inputs_temp.txt')
+    xfoil_fpath = os.path.join(xfoil_dir, 'xfoil.exe')
+
+    # write the command file
+    with open(xfoil_cmnd_file, 'w') as f:
+        f.write('load {}\n'.format(foil_relpath))
+        f.write('ppar\nN\n200\n\n\n')
+        f.write('oper\n')
+        f.write('visc\n')
+        f.write('{0:.0f}\n'.format(re))
+        f.write('m {}\n'.format(mach))
+        f.write('vpar\n')
+        f.write('n {}\n\n'.format(ncrit))
+        f.write('iter\n')
+        f.write('{0:.0f}\n'.format(iter_limit))
+        f.write('pacc\n\n\n')
+        if 'alpha' in swept_param:
+            for a in vals:
+                f.write('a{}\n'.format(a))
+        elif 'cl' in swept_param:
+            for cl in vals:
+                f.write('cl{}\n'.format(cl))
+        f.write('!\n{}'.format(' ' * 100) * keypress_iternum)
+        f.write('pwrt\n')
+        f.write('{}\n\n\n'.format(output_fpath))
+        f.write('quit\n')
+
+    # now open it again and send it as the xfoil commands
+    # CREATE_NO_WINDOW = 0x08000000   # flag to create no window, should work on both Windows and Linux??
+    with open(xfoil_cmnd_file, 'r') as f:
+        # if hide_windows:
+        #     create_kw = {'creationflags': subprocess.CREATE_NO_WINDOW}
+        # else:
+        #     create_kw = {}
+
+        sui = subprocess.STARTUPINFO()
+        if hide_windows:
+            sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+
+        if verbose:
+            out, err = None, None
+        else:
+            out, err = subprocess.DEVNULL, subprocess.DEVNULL
+
+        subprocess.run([xfoil_fpath], startupinfo=sui, stdin=f, stdout=out, stderr=err,
+                       timeout=tmout, cwd=xfoil_dir)
+        # subprocess.run([xfoil_fpath], stdin=f, stdout=out, stderr=err, timeout=tmout, cwd=xfoil_dir,
+        #                **create_kw)
+        # p = subprocess.Popen([xfoil_fpath], stdin=f, stdout=out, stderr=err, cwd=xfoil_dir, **create_kw)
+        # p.wait(timeout=tmout)
+
+    # delete the temp command file
+    os.remove(xfoil_cmnd_file)
+
+
+def read_xfoil_pacc_file(fpath: str = None, delete_after: bool = False):
+    # if not given, default fpath is this
+    if not fpath:
+        fpath = os.path.join(_get_user_settings()['airfoil_database'], 'polar_output.txt')
+
+    # open fpath and read in all text
+    with open(fpath, 'r') as f:
+        txt = f.read()
+
+    # split into lines, create a dictionary, and iterate over the lines
+    lines = [line for line in txt.split('\n') if line.strip() != '']
+    d = {}
+    for i, line in enumerate(lines):
+        if i == 1:  # foil name on line 1
+            d['name'] = line.split(':')[1].strip()
+        elif i == 4:  # mach, re, and ncrit on line 4
+            mach, rest = line.split('Mach')[1].split('Re')
+            d['mach'] = float(mach.replace('=', '').strip())
+            re, ncrit = rest.split('Ncrit')
+            d['re'] = int(float(re.replace('=', '').replace(' ', '')))
+            d['ncrit'] = int(float(ncrit.replace('=', '').strip()))
+        elif i == 5:  # variable names on line 5, create an empty list for each one
+            var_names = [name for name in line.strip().split(' ') if name != '']
+            for key in range(len(var_names)):
+                d[key] = []
+        elif i >= 7:  # rest of lines in file contain variable entries for each variable
+            vals = [val for val in line.strip().split(' ') if val != '']
+            for col, val in enumerate(vals):
+                if vals[0] not in d[0]:  # if the alpha value of this line is not already in the list of alphas
+                    d[col].append(float(val))  # store with key as value index <- why am i doing it like this tho?
+                else:
+                    print('did not append over duplicate in col {} on line {}'.format(col, i - 7))
+
+    # re-assign dictionary keys to be variable names instead of indexes
+    for i, key in enumerate(var_names):
+        d[key] = d[i]
+        del d[i]
+
+    if [len(v) for v in d.values() if isinstance(v, list)][0] == 0:
+        return None
+
+    # sort each variable based on alpha and re-assign to each dictionary key
+    sort_list = d['alpha'].copy()
+    for key in var_names:
+        a, sorted_vals = list(zip(*sorted(zip(sort_list, d[key]))))
+        d[key] = np.array(sorted_vals)
+
+    # calculate L/D
+    d['CL/CD'] = d['CL'] / d['CD']
+
+    # if desired, delete the pacc file
+    if delete_after:
+        os.remove(fpath)
+
+    return d
+
+
+def read_polar_data_file(fpath: str):
+    with open(fpath, 'r') as f:
+        txt = f.read()
+
+    # create a dictionary and go thru all the lines and populate dictionary of strings
+    polar_data = {}
+    lines = txt.split('\n')
+    for i, line in enumerate(lines):
+        if i == 0:
+            name = line
+        elif not i == 1:
+            if '*****' in line:
+                d = {'name': name}
+                pairs = line.strip('*').strip().split(', ')
+                for pair in pairs:
+                    key, val = pair.split(' = ')
+                    d[key.lower()] = val
+            elif not line.strip() == '':
+                key, val = line.split(': ')
+                d[key] = val
+            else:
+                polar_data[(d['re'], d['mach'], d['ncrit'])] = d
+
+    # convert all the strings into what they're supposed to be
+    for str_key, polar in list(polar_data.items()):
+        re_key, mach_key, ncrit_key = str_key
+        for key, val in polar.items():
+            if '(' in val:
+                vals = [float(i.strip()) for i in val.replace('(', '').replace(')', '').split(',')]
+                polar[key] = np.array(vals)
+            elif 're' in key or 'ncrit' in key:
+                polar[key] = int(val)
+            elif 'mach' in key:
+                polar[key] = float(val)
+        new_key = (int(float(re_key)), float(mach_key), int(float(ncrit_key)))
+        polar_data[new_key] = polar.copy()
+        del polar_data[str_key]
+
+    return polar_data
+
+
+def save_polar_data_file(polar_data: dict, savepath: str, name: str = None):
+    if not name:
+        name = 'unnamed airfoil'
+    with open(savepath, 'w') as f:
+        f.write('{}\n'.format(name))
+        for polar_key in polar_data:
+            d = polar_data[polar_key]
+            re, mach, ncrit = polar_key
+            f.write('\n***** Re = {}, Mach = {}, nCrit = {} *****\n'.format(re, mach, ncrit))
+            keys_2_write = [key for key, val in d.items() if isinstance(val, np.ndarray)]
+            for key in keys_2_write:
+                f.write('{}: {}\n'.format(key, tuple(d[key])))
+    return
+
+
+def read_xrotor_op_file(fpath: str):
+    with open(fpath, 'r') as f:
+        txt = f.read()
+    if '********** NOT CONVERGED **********' in txt:
+        raise Error('XROTOR did not converge')
+    lines = txt.split('\n')
+    d = {}
+    headers = None
+
+    for line in lines:
+        if line.strip('-').strip('=').strip() == '':
+            pass  # ignore blank lines
+        elif ':' in line:   # top section
+            spl = [l.strip() for l in line.split(':')]
+            for i in range(len(spl) - 1):
+                key = spl[i].split('  ')[-1].strip()
+                val = spl[i + 1].split('  ')[0].strip()
+                if val[0].isnumeric() or val[1].isnumeric():
+                    d[key] = float(val)
+                else:
+                    d[key] = val
+        else:   # listout at bottom
+            vals = [val.strip() for val in line.replace('-', ' -').replace('s', ' ').split(' ') if val != '']
+            if headers is None:
+                headers = vals.copy()
+                for h in headers:
+                    d[h] = []
+            else:
+                for i, val in enumerate(vals):
+                    try:
+                        d[headers[i]].append(float(val))
+                    except ValueError:
+                        d[headers[i]].append(np.nan)
+
+    # go thru and turn into np.arrays now
+    for h in headers:
+        d[h] = np.array(d[h])
+
+        if 'REx10^' in h:  # detect and convert RE order of magnitude
+            old_res = d.pop(h)
+            exponent = int(h.strip('REx10^'))
+            d['RE'] = old_res * 10 ** exponent
+
+    return d
+
+
+def read_xrotor_cput_file():
+    return
+
+
+def read_2col_file(fpath: str, del_after: bool = True):
+    with open(fpath, 'r') as f:
+        txt = f.read().strip()
+    col1 = []
+    col2 = []
+    lines = txt.split('\n')
+    for line in lines:
+        val1, val2 = line.strip().split(' ', 1)
+        col1.append(float(val1.strip()))
+        col2.append(float(val2.strip()))
+
+    if del_after:
+        os.remove(fpath)
+
+    return np.array(col1), np.array(col2)
+
+
+def read_profile_xyz(fpath: str):
+    with open(fpath, 'r') as f:
+        txt = f.read().strip()
+    lines = txt.split('\n')[1:]
+
+    xpts, ypts, zpts = [], [], []
+    for line in lines:
+        xval, yval, zval = [float(val) for val in line.split(', ')]
+        xpts.append(xval)
+        ypts.append(yval)
+        zpts.append(zval)
+
+    return np.vstack([np.array(xpts), np.array(ypts), np.array(zpts)])
+
+
+# =============== INTERFACING WITH 3RD PARTY PROGRAMS ===============
+def download_foil_coordinates(foil_str: str):
+    foil_str = '{}.dat'.format(foil_str) if not foil_str.endswith('.dat') else foil_str
+    coord_url = 'https://m-selig.ae.illinois.edu/ads/coord/{}'.format(foil_str)
+    savepath = os.path.join(get_foil_db(), foil_str)
+    Info('Attempting to download "{}"...'.format(coord_url))
+    try:
+        urllib.request.urlretrieve(coord_url, savepath)
+        Info('saved to "{}"'.format(savepath), indent_level=1)
+        return True
+    except urllib.error.HTTPError:
+        Warning('Unable to download, not found')
+        return False
+
+
+def read_radial_stations(prop: Propeller, plot_also: bool = True, verbose: bool = False):
+    stations = []
+    if not os.path.exists(prop.station_polar_folder):
+        return stations
+
+    fnames = os.listdir(prop.station_polar_folder)
+    for fname in fnames:
+        roR, foil_name = fname.replace('.polar', '').split('_')
+        roR = float(roR)
+        fpath = os.path.join(prop.station_polar_folder, fname)
+        with open(fpath, 'r') as f:
+            txt = f.read().strip()
+        lines = txt.split('\n')
+
+        pol = {}
+        for line in lines:
+            key, val_str = line.split(':', 1)
+            if ',' in val_str:
+                val = np.array([float(v.strip()) for v in val_str.split(',')])
+            else:
+                val = float(val_str.strip())
+            pol[key] = val
+        st = RadialStation(foil_polar=pol, momma=prop, re_estimate=pol['re'], mach_estimate=pol['mach'],
+                           ncrit_estimate=pol['ncrit'], Xisection=roR, plot=plot_also, verbose=verbose,
+                           foil_name_str=foil_name)
+        stations.append(st)
+
+    return stations
+
+
+def create_radial_stations(prop: Propeller, plot_also: bool = True, verbose: bool = True):
+    # get density for Re estimates
+    if prop.design_atmo_props['altitude_km'] == -1:
+        rho, nu = 1000, 0.1150e-5
+        mu = nu * rho
+    else:
+        atmo = standard_atmosphere(prop.design_atmo_props['altitude_km'])# temp, p, rho, sonic_a, mu
+        mu, rho = atmo['mu'], atmo['rho']
+        nu = mu / rho
+
+    # replace it if it was entered as atmo prop as well
+    if 'dens' in prop.design_atmo_props:
+        rho = prop.design_atmo_props['dens']
+
+    t = ''
+    stations = []
+    for idx, xi in enumerate(prop.station_params):  # append station text all together and save
+        if verbose:
+            Info('Auto-generating section inputs from airfoil database data for section {} ({})...'.
+                  format(idx + 1, prop.station_params[xi]))
+        fn = prop.station_params[xi]
+        foil = Airfoil(name=fn, verbose=verbose)
+        re_est = int(calc_rotational_re(rho=rho, rpm=prop.design_rpm, radius=prop.radius * xi, chord=prop.radius / 10,
+                                        mu=mu, vel=prop.design_speed_mps, adv=prop.design_adv))
+        st = RadialStation(station_idx=idx, Xisection=xi, foil=foil, re_estimate=re_est, plot=plot_also, verbose=verbose)
+        t += st.generate_txt_params()
+        stations.append(st)
+    return stations, t
+
+
+def run_xrotor_oper(xrr_file: str, vorform: str, adva: float = None, rpm: float = None, thrust: float = None,
+                    torque: float = None, power: float = None, velo: float = None, hide_windows: bool = True,
+                    verbose: bool = True, tmout: int = None, xrotor_verbose: bool = False):
+
+    # increase the timeout for vrtx
+    if tmout is None and vorform.lower() == 'vrtx':
+        tmout = 25
+    elif tmout is None:
+        tmout = 10
+
+    # vorform has to be one of these three things
+    if vorform.lower() not in ['grad', 'pot', 'vrtx']:
+        raise Error('Input "vorform" must be one of ["grad", "pot", "vrtx"]')
+
+    # filename stuff
+    dirname, fname = os.path.split(xrr_file)
+    relpath = os.path.join(os.path.split(dirname)[1], fname)
+
+    # first we set the vorform
+    cmnds = ['load {}\n'.format(relpath), 'oper', 'form', '{}\n'.format(vorform)]
+
+    # if we are changing the velo, do that next
+    if velo is not None:
+        cmnds.extend(['velo', '{}'.format(velo), 'rein\n\ny'])
+
+    # can only be changing 1 of the 5 at a time
+    non_none_kwargs = [i for i in [adva, rpm, thrust, torque, power] if i is not None]
+    if len(non_none_kwargs) > 1:
+        raise Error('Can only change 1 of (adva, rpm, thrust, torque, power) at a time')
+
+    # command text based on which one was given
+    if adva is not None:
+        cmnds.extend(['adva', str(adva)])
+    elif rpm is not None:
+        cmnds.extend(['rpm', str(rpm)])
+    elif thrust is not None:
+        cmnds.extend(['thrust', str(thrust), 'p'])
+    elif torque is not None:
+        cmnds.extend(['torque', str(torque), 'p'])
+    elif power is not None:
+        cmnds.extend(['power', str(power), 'p'])
+    else:  # all were None
+        pass
+
+    # remove the output files if they exist for some reason already
+    oper_out_file, oper_out_fullpath = 'oper_out.txt', os.path.join(get_prop_db(), 'oper_out.txt')
+    wvel_out_file, wvel_out_fullpath = 'wvel_out.txt', os.path.join(get_prop_db(), 'wvel_out.txt')
+    if os.path.exists(oper_out_fullpath):
+        os.remove(oper_out_fullpath)
+    if os.path.exists(wvel_out_fullpath):
+        os.remove(wvel_out_fullpath)
+
+    # finalize the list of commands and write them to a file
+    cmnds.extend(['writ {}'.format(oper_out_file), 'wvel {}'.format(wvel_out_file), '\n\nquit\n'])
+    xrotor_cmnd_file = os.path.join(get_prop_db(), 'oper_run_inputs.txt')
+    with open(xrotor_cmnd_file, 'w') as f:
+        f.write('\n'.join(cmnds))
+
+    # run the mutha
+    xrotor_fpath = os.path.join(get_prop_db(), 'xrotor.exe')
+    with open(xrotor_cmnd_file, 'r') as f:
+        sui = subprocess.STARTUPINFO()
+        if hide_windows:
+            sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        if verbose:
+            Info('Running XROTOR for off-design operating point...', indent_level=1)
+        if xrotor_verbose:
+            out_err_kw = {}
+        else:
+            out_err_kw = {'stdout': subprocess.DEVNULL, 'stderr': subprocess.STDOUT}
+
+        subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, **out_err_kw,
+                       timeout=tmout, cwd=get_prop_db())
+
+    # get the returned velo and rpm for naming reasons
+    oper_output = read_xrotor_op_file(oper_out_fullpath)
+    returned_velo = oper_output['speed(m/s)']
+    returned_rpm = oper_output['rpm']
+
+    # rename / move the output files into the database
+    oper_savedir = os.path.join(os.path.split(oper_out_fullpath)[0], dirname, 'oper_data')
+    if not os.path.exists(oper_savedir):
+        os.mkdir(oper_savedir)
+    oper_copypath = os.path.join(oper_savedir, 'velo_{:.0f}_rpm_{:.0f}.oper'.format(100 * returned_velo, returned_rpm))
+    shutil.copyfile(oper_out_fullpath, oper_copypath)
+
+    wvel_savedir = os.path.join(os.path.split(wvel_out_fullpath)[0], dirname, 'wvel_data')
+    if not os.path.exists(wvel_savedir):
+        os.mkdir(wvel_savedir)
+    wvel_copypath = os.path.join(wvel_savedir, 'velo_{:.0f}_rpm_{:.0f}.wvel'.format(100 * returned_velo, returned_rpm))
+    shutil.copyfile(wvel_out_fullpath, wvel_copypath)
+
+    # delete the temporary files
+    os.remove(xrotor_cmnd_file)
+    os.remove(oper_out_fullpath)
+    os.remove(wvel_out_fullpath)
+
+    return
+
+
+def read_xrotor_wvel_file(fpath:str):
+    with open(fpath, 'r') as f:
+        txt = f.read().strip()
+    lines = [ln.strip() for ln in txt.split('\n') if ln != '']
+
+    data = {}
+    for i, line in enumerate(lines):
+        line = line.replace('=', '= ')
+        words = [w.strip() for w in line.split(' ') if w != '']
+        if i in [3, 4]:
+            for j, word in enumerate(words):
+                if 'rpm' in word.lower():
+                    data['rpm'] = float(words[j + 1])
+                elif 'vel' in word.lower():
+                    data['vel'] = float(words[j + 1])
+                elif 'beta_tip' in word.lower():
+                    data['beta_tip'] = float(words[j + 1])
+                elif 'power' in word.lower():
+                    try:
+                        data['power'] = float(words[j + 1])
+                    except ValueError:
+                        data['power'] = np.nan
+                elif 'thrust' in word.lower():
+                    try:
+                        data['thrust'] = float(words[j + 1])
+                    except ValueError:
+                        data['thrust'] = np.nan
+        elif i == 6:
+            headers = [ln.strip() for ln in line.replace(' + ', '+').split(' ') if ln != '']
+            for header in headers:
+                data.setdefault(header, [])
+        elif i > 6:
+            vals = [ln.strip() for ln in line.split(' ') if ln != '']
+            for v, val in enumerate(vals):
+                data[headers[v]].append(float(val))
+
+    return data
+
+
+def create_propeller(name: str, nblades: int, radius: float, hub_radius: float, hub_wake_disp_br: float,
+                     design_speed_mps: float, design_cl: dict, design_atmo_props: dict, design_vorform: str,
+                     station_params: dict = None, design_adv: float = None, design_rpm: float = None,
+                     design_thrust: float = None, design_power: float = None, n_radial: int = 50,
+                     verbose: bool = False, show_station_fit_plots: bool = True, plot_after: bool = True,
+                     tmout: int = None, hide_windows: bool = True, geo_params: dict = {}, xrotor_verbose: bool = False):
+    # adjust timeout for vrtx
+    if tmout is None and design_vorform == 'vrtx':
+        tmout = 100
+    elif tmout is None:
+        tmout = 30
+
+    # name must be less than 38? characters for XROTOR to be able to save it
+    if len(name) > 38:
+        raise Error('"name" must be less than 38 characters when creating a propeller, "{}" is too long'.format(name))
+
+    # must input an altitude in atmo props
+    if 'altitude_km' not in design_atmo_props:
+        raise Error('You must include "altitude_km" as an input to create_propeller()')
+
+    # delete if exists already, make save folder, point-cloud folder
+    save_folder = os.path.join(get_prop_db(), name)
+    if os.path.exists(save_folder):
+        shutil.rmtree(save_folder)
+    os.mkdir(save_folder)
+
+    # make a folder for all the profile x, y, z listings
+    prof_folder = os.path.join(save_folder, 'blade_profiles')
+    os.mkdir(prof_folder)
+
+    # create the Propeller object, create the stations
+    prop = Propeller(name=name, nblades=nblades, radius=radius, hub_radius=hub_radius,
+                     hub_wake_disp_br=hub_wake_disp_br, design_speed_mps=design_speed_mps, design_cl=design_cl,
+                     design_atmo_props=design_atmo_props, design_vorform=design_vorform, design_adv=design_adv,
+                     station_params=station_params, geo_params=geo_params, design_rpm=design_rpm,
+                     design_thrust=design_thrust, design_power=design_power, verbose=verbose)
+    st_txt = prop.set_stations(plot_also=show_station_fit_plots, verbose=verbose)
+
+    # prep XROTOR commands depending on what station_params were input
+    aero_params_fname = '{}_temp_section_params.txt'.format(name)
+    aero_params_fpath = os.path.join(get_prop_db(), aero_params_fname)
+    with open(aero_params_fpath, 'w') as f:
+        f.write(st_txt)
+
+    # prep XROTOR commands depending on what design_atmo_props were given
+    alt = design_atmo_props['altitude_km']
+    atmo_txt = '{}\n\n'.format(alt)
+
+    if 'vsou' in design_atmo_props:
+        vsou = design_atmo_props['vsou']
+        atmo_txt += 'vsou\n{}\n'.format(vsou)
+    if 'dens' in design_atmo_props:
+        dens = design_atmo_props['dens']
+        atmo_txt += 'dens\n{}\n'.format(dens)
+    if 'visc' in design_atmo_props:
+        visc = design_atmo_props['visc']
+        atmo_txt += 'visc\n{}\n'.format(visc)
+    atmo_txt += 'desi'
+
+    # prep XROTOR commands depending on what vortex formulation is given
+    if design_vorform is None:
+        vorform_txt = 'pot\n'
+    elif any([design_vorform.lower() == i for i in ['grad', 'pot', 'vrtx']]):
+        vorform_txt = '{}\n'.format(design_vorform.lower())
+
+    # prep XROTOR commands for the advance ratio OR RPM design specification
+    if design_adv is not None:
+        if design_rpm is not None:
+            raise Error('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
+        adv_rpm_txt = '{}'.format(design_adv)
+    elif design_rpm is not None:
+        if design_adv is not None:
+            raise Error('Cannot specify both "design_adv" and "design_rpm", must pick one or the other')
+        adv_rpm_txt = '{}\n{}'.format(0, design_rpm)
+
+    # prep XROTOR commands for the thrust OR power design specification
+    if design_thrust is not None:
+        thr_pow_txt = '{}'.format(design_thrust)
+    elif design_power is not None:
+        thr_pow_txt = '{}\n{}'.format(0, design_power)
+
+    # prep XROTOR commands depending on what design_cl keys were given
+    if len(design_cl) == 1:  # either a constant value was given, or a filepath
+        if 'const' in design_cl:
+            const_cl = design_cl['const']
+            cl_txt = 'cc\n{}\n\n'.format(const_cl)
+        elif 'file' in design_cl:
+            fpath = design_cl['file']
+            cl_txt = 'cr\n{}\n\n'.format(fpath)
+        else:
+            raise Error('Must give either a "const" CL target (constant), a "root" and "tip" CL target '
+                        '(linearly varied), or specify a CL(r/R) .txt file')
+    elif len(design_cl) == 2:  # a linear cl was given
+        if all([k in design_cl for k in ['root', 'tip']]):
+            root_cl = design_cl['root']
+            tip_cl = design_cl['tip']
+            cl_txt = 'cl\n{}\n{}\n\n'.format(root_cl, tip_cl)
+        else:
+            raise Error('If only 2 keywords are given in "design_cl", they must be "root" and "tip"')
+    else:
+        raise Error('"design_cl" input dictionary error, either too many or not enough keys (if a single key'
+                    'is given, it must be either "const" or "file", if 2 keys are given they must be "root" '
+                    'and "tip"')
+
+    # prep XROTOR commands for saving blade data r/R
+    blade_data_keys = ['CH', 'BE', 'GAM', 'CL', 'CD', 'RE', 'EFP', 'Ub', 'VA', 'VT', 'VD', 'VA/V', 'VT/V', 'VD/V',
+                       'VAslip', 'VTslip', 'Aslip', 'Ti', 'Pi', 'Tv', 'Pv', 'Ttot', 'Ptot', 'Xw', 'Vw', 'Tw', 'Pw']
+    blade_data = {}
+    blade_txt = 'plot\n12\n'
+    for key in blade_data_keys:
+        fname = '{}_out.txt'.format(key.replace('/', '_over_'))
+        blade_data[key] = None
+        blade_txt += 'o\n{}\nw\n{}\n'.format(key, fname)
+
+    # prep XROTOR commands to save the solved operating point params
+    op_fpath = '{}\\{}.xrop'.format(name, name)
+    save_op_txt = 'oper\nwrit\n{}\n'.format(op_fpath)
+
+    # prep XROTOR commands for savename
+    savename = '{}\\{}.xrr'.format(name, name)
+    save_txt = 'save {}\nquit\n'.format(savename)
+
+    # write XROTOR commands to a file and run in a subprocess
+    xrotor_cmnd_file = os.path.join(get_prop_db(), 'xrotor_inputs_temp.txt')
+    cmnds = ['aero', 'read', '{}\n'.format(aero_params_fname),
+             'desi', 'atmo', '{}'.format(atmo_txt), 'form', '{}'.format(vorform_txt), 'N', '{}'.format(n_radial),
+             'inpu', '{}'.format(nblades),
+             '{}'.format(radius), '{}'.format(hub_radius), '{}'.format(hub_wake_disp_br), '{}'.format(design_speed_mps),
+             '{}'.format(adv_rpm_txt), '{}'.format(thr_pow_txt), '0', '{}'.format(cl_txt), '{}'.format(blade_txt), '\n',
+             '{}'.format(save_op_txt), '\n\n', '{}'.format(save_txt)]
+
+    with open(xrotor_cmnd_file, 'w') as f:
+        f.write('\n'.join(cmnds))
+
+    xrotor_fpath = os.path.join(get_prop_db(), 'xrotor.exe')
+    with open(xrotor_cmnd_file, 'r') as f:
+        sui = subprocess.STARTUPINFO()
+        if hide_windows:
+            sui.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        if verbose:
+            Info('Running XROTOR to create new geometry...')
+        if xrotor_verbose:
+            subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, timeout=tmout, cwd=get_prop_db())
+        else:
+            subprocess.run([xrotor_fpath], startupinfo=sui, stdin=f, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT,
+                           timeout=tmout, cwd=get_prop_db())
+    os.remove(xrotor_cmnd_file)
+    os.remove(aero_params_fpath)
+
+    # set the prop's blade-data that we just saved in creation
+    for key in blade_data.copy():
+        fp = os.path.join(get_prop_db(), '{}_out.txt'.format(key.replace('/', '_over_')))
+        roR, array = read_2col_file(fpath=fp)
+        if 'r/R' not in blade_data:
+            blade_data['r/R'] = roR
+        blade_data[key] = array
+    prop.set_blade_data(blade_dict=blade_data)
+
+    # interpolate the profiles as part of geometry creation
+    if 'n_prof_pts' not in geo_params:
+        geo_params['n_prof_pts'] = None
+    if 'n_profs' not in geo_params:
+        geo_params['n_profs'] = 50
+    if 'tot_skew' not in geo_params:
+        geo_params['tot_skew'] = 0.0
+
+    prop.interp_foil_profiles(**geo_params)  # also saves the profiles
+
+    # save the PDT propeller meta-file, and then read in the operating point dictionary by calling load_from_savefile()
+    prop.xrotor_op_dict = read_xrotor_op_file(prop.xrop_file)
+    prop.save_station_polars()
+    prop.save_meta_file()
+    prop.load_from_savefile(verbose=verbose)   # reads meta, xrr, xrop, and point clouds
+
+    if not verbose:
+        Info('"{}" Geometry Created!'.format(prop.name))
+    if plot_after:
+        prop.plot_design_point_panel()
+
+    return prop
+
+
+def write_blade_cl_file(r_pts: list, cl_pts: list, savepath: str = None):
+    if savepath is None:
+        savepath = 'blade_design_cl.txt'
+    with open(savepath, 'w') as f:
+        for r, cl in zip(r_pts, cl_pts):
+            f.write('   {r: .6f}      {cl: .6f}\n'.format(r=r, cl=cl))
+
+
+def convert_ps2png(ps_fpath: str, return_pil_img: bool = False, show_in_pyplot: bool = False):
+    """
+    Function that converts a PostScript (.ps) image file to a .png file.  Uses 3rd party GNU licensed
+    GhostScript, which is capable of much more than just .ps to .png conversion.
+
+    :param ps_fpath: the filepath to the PostScript file
+    :param return_pil_img: returns a PIL image object if True, by default just returns the PNG filepath
+    :param show_in_pyplot: displays the image in a pyplot figure if True, default is False
+    :return png_fpath: the filepath to the converted file
+    :return pil_img: the PIL image object
+    :return fig: the pyplot figure object
+    """
+    png_fpath = ps_fpath.replace('.ps', '.png')
+    gs_cmnds = ['gswin64c.exe', '-dSAFER', '-dBATCH', '-dNOPAUSE', '-sDEVICE=png16m',
+                '-dGraphicsAlphaBits=4', '-sOutputFile={}'.format(png_fpath), '{}'.format(ps_fpath)]
+    subprocess.run(gs_cmnds, stdout=subprocess.DEVNULL)  # stderr=subprocess.DEVNULL
+
+    if not return_pil_img and not show_in_pyplot:
+        return png_fpath
+
+    from PIL import Image
+    pil_img = Image.open(png_fpath)
+
+    if return_pil_img:
+        return pil_img
+
+    fig = plt.figure(figsize=[9, 11])
+    ax = fig.add_subplot(111)
+    ax.axis('off')
+    ax.imshow(pil_img)
+    fig.tight_layout()
+    return fig
+
+
+# =============== MODELING / PHYSICS ===============
+def calc_linear_re(rho: float, vel: float, length: float, mu: float):
+    return rho * vel * length / mu
+
+
+def calc_rotational_re(rho: float = None, vel: float = None, chord: float = None, mu: float = None, rpm: float = None,
+                       radius: float = None, adv: float = None):
+    if all([i is not None for i in [rho, rpm, radius, chord, mu]]):
+        re = rho * (rpm / 60 * 2 * np.pi) * radius * chord / mu
+    elif all([i is not None for i in [rho, vel, adv, radius, chord, mu]]):
+        rpm = vel / np.pi / 2 / radius / adv * 60
+        re = rho * (rpm / 60 * 2 * np.pi) * radius * chord / mu
+    else:
+        raise Error('Must input all of either [rho, vel, chord, mu] or [rho, rpm, radius, chord, mu]')
+    return re
+
+
+def standard_atmosphere(altitude_km: float) -> dict:  # standard atmosphere eqs from Jake's college prof.
+
+    alt_m = altitude_km * 1000
+
+    g, R_air, gamma_air = 9.80665, 287.05307, 1.4
+    alt1, alt2, alt3 = 11000, 20000, 32000
+    temp0, p0, rho0, mu0 = 288.15, 101325, 1.2250, .0000181206
+    slope0, slope1, slope2 = -.0065, 1, .001
+
+    temp1 = temp0 + slope0 * alt1
+    p1 = p0 * (temp1 / temp0) ** (-g / slope0 / R_air)
+    rho1 = rho0 * (temp1 / temp0) ** (-g / slope0 / R_air - 1)
+
+    temp2 = temp1
+    p2 = p1 * np.exp(-g / R_air / temp2 * (alt2 - alt1))
+    rho2 = rho1 * np.exp(-g / R_air / temp2 * (alt2 - alt1))
+
+    if alt_m < 0:
+        raise Error('Cannot input negative values into standard_atmosphere()')
+    elif alt_m < alt1:
+        temp = temp0 + slope0 * alt_m
+        p = p0 * (temp / temp0) ** (-g / slope0 / R_air)
+        rho = rho0 * (temp / temp0) ** (-g / slope0 / R_air - 1)
+    elif alt_m < alt2:
+        temp = temp1
+        p = p1 * np.exp(-g / slope1 / R_air / temp * (alt_m - alt1))
+        rho = rho1 * np.exp(-g / R_air / temp * (alt_m - alt1))
+    elif alt_m < alt3:
+        temp = temp2 + slope2 * (alt_m - alt2)
+        p = p2 * (temp / temp2) ** (-g / slope2 / R_air)
+        rho = rho2 * (temp / temp2) ** (-g / slope2 / R_air - 1)
+    else:
+        raise Error('Altitude out of range of atmosphere model')
+
+    sonic_a = np.sqrt(gamma_air * R_air * temp)
+    mu = mu0 * (temp / temp0) ** 1.5 * ((temp0 + 120) / (temp + 120))
+
+    return {'temp': temp, 'p': p, 'rho': rho, 'sonic_a': sonic_a, 'mu': mu}
+
+
+def xrotor_drag_model(CL: np.ndarray, CDmin: float, CLCDmin: float, dCDdCL2: float):
+    CD = CDmin + dCDdCL2 * (CLCDmin - CL) ** 2
+    return CD
+
+
+def get_xrotor_re_scaling_exp(re: int):     # THIS NEEDS WORK
+    # re_pts = [0, 1e5, 2e5, 8e5, 2e6, 3e6]
+    # f_pts = [-0.3, -0.5, -0.5, -1.5, -0.2, -0.1]
+    # return np.interp(x=re, xp=re_pts, fp=f_pts)
+    return -0.4
+
+
+def calc_thrust(k_t, rho, rpm, dia):
+    n = rpm / 60
+    return k_t * rho * n ** 2 * dia ** 4
+
+
+def calc_ideal_eff(thrust: float, rho: float, a_disk: float, u_o: float):
+    T = thrust
+    rho = rho
+    A_disk = a_disk
+    u_o = u_o
+    return 100 * 2 / (1 + (T / (A_disk * 1 / 2 * rho * u_o ** 2) + 1) ** (1 / 2))
+
+
+# ===== GEOMETRY MANIPULATION =====
+def generate_3D_profile_points(nondim_xy_coords: np.ndarray, radius: float, axis_shift: float = 0.5,
+                               chord_len: float = 1.0, beta_deg: float = 0.0, skew_deg: float = 0.0):
+    xpts, ypts = nondim_xy_coords.copy()
+
+    # mirror over y and shift (0, 0) to align to the blade axis
+    xpts = -xpts + axis_shift
+
+    # scale the profile by the chord length
+    xpts *= chord_len
+    ypts *= chord_len
+
+    # rotate profile by beta
+    b = np.deg2rad(beta_deg)
+    xp = xpts * np.cos(-b) + ypts * np.sin(-b)
+    yp = ypts * np.cos(-b) - xpts * np.sin(-b)
+
+    # create array of radii points, create array of theta points
+    rp = np.ones(len(xp)) * radius
+    thetas = xp / (2 * np.pi * radius) * 2 * np.pi    #map each xpos to a theta in radians
+
+    # apply skew
+    thetas += np.deg2rad(-skew_deg)
+
+    # wrap the ycoords
+    ys = rp * np.sin(thetas)
+    xs = rp * np.cos(thetas)
+    zs = yp
+
+    return np.vstack([xs, ys, zs])
+
+
+def unit_vector(vector):
+    """ Returns the unit vector of the vector.  """
+    return vector / np.linalg.norm(vector)
+
+
+def angle_between(v1, v2):
+    """ Returns the angle in radians between vectors 'v1' and 'v2'::
+
+            angle_between((1, 0, 0), (0, 1, 0))
+            1.5707963267948966
+            angle_between((1, 0, 0), (1, 0, 0))
+            0.0
+            angle_between((1, 0, 0), (-1, 0, 0))
+            3.141592653589793
+    """
+    v1_u = unit_vector(v1)
+    v2_u = unit_vector(v2)
+    return np.arccos(np.clip(np.dot(v1_u, v2_u), -1.0, 1.0))
+
+
+def compute_polygon_angles(exterior_coords: list):
+    if exterior_coords[0] == exterior_coords[-1]:
+        removed = exterior_coords.pop(-1)
+    angles = []
+    for i in range(len(exterior_coords)):
+        pt = exterior_coords[i]
+        last_pt = exterior_coords[i - 1]
+        if i == len(exterior_coords) - 1:
+            next_pt = exterior_coords[0]
+        else:
+            next_pt = exterior_coords[i + 1]
+
+        v1 = [next_pt[0] - pt[0], next_pt[1] - pt[1], next_pt[2] - pt[2]]
+        v2 = [last_pt[0] - pt[0], last_pt[1] - pt[1], last_pt[2] - pt[2]]
+        ang = angle_between(v1, v2)
+        angles.append(ang)
+    return angles
+
+
+def compute_profile_trimesh(profile_coords, reverse_order: bool = False):
+    if len(profile_coords) == 3:
+        xc, yc, zc = profile_coords
+    elif len(profile_coords) == 2:
+        xc, yc = profile_coords
+        zc = np.zeros(len(xc))
+    else:
+        raise ValueError('len of profile_coords must be either 2 or 3')
+    points = list(zip(xc, yc, zc))
+
+    # 1) For each vertex in the polygon, compute the angle between the two linked edges
+    # 2) Sort vertices by decreasing angle relative to the interior of the polygon
+    # 3) If there is less than 3 vertices in the set, we're done
+    # 4) Take the last vertex in the set and output the triangle formed by it and its two neighbours
+    # 5) Remove the vertex from the set
+    # 6) Update the angle of the two neighbours
+    # 7) Jump to 2
+
+    vectors = []
+    while len(points) >= 3:
+        angles = compute_polygon_angles(exterior_coords=points)
+        min_idx = np.argmin(angles)
+        prev_idx = min_idx - 1
+        if min_idx == len(angles) - 1:
+            next_idx = 0
+        else:
+            next_idx = min_idx + 1
+        pt1, pt2, pt3 = points[prev_idx], points[min_idx], points[next_idx]
+        if not reverse_order:
+            vector = [pt1, pt2, pt3]
+        else:
+            vector = [pt3, pt2, pt1]
+        vectors.append(vector)
+        _ = points.pop(min_idx)
+
+    return vectors
+
+
+# ===== USER INTERFACE STUFF =====
+def start_ui():
+    from PyQt5 import QtWidgets
+    from propeller_design_tools.user_interface import InterfaceMainWindow
+    app = QtWidgets.QApplication(sys.argv)
+    w = InterfaceMainWindow()
+    w.show()
+    app.exec_()
+
+
+def delete_all_widgets_from_layout(layout):
+    for i in reversed(range(layout.count())):
+        layout.itemAt(i).widget().setParent(None)
```

### Comparing `propeller_design_tools-0.3.5/propdes/helper_ui_classes.py` & `propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_classes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,462 +1,462 @@
-import os
-import subprocess
-
-import numpy as np
-import matplotlib.gridspec as gridspec
-from propdes.settings import get_setting, set_propeller_database, set_airfoil_database, \
-    get_foil_db, get_prop_db
-from propdes.funcs import count_airfoil_db, count_propeller_db
-from propdes.propeller import Propeller
-import sys
-from typing import Union
-from io import StringIO
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
-from matplotlib.figure import Figure
-try:
-    from PyQt5 import QtWidgets, QtCore, QtGui
-    from propdes.helper_ui_subclasses import PDT_Label, PDT_PushButton, PDT_SpinBox, PDT_DoubleSpinBox, \
-        PDT_ComboBox, PDT_GroupBox, PDT_CheckBox, PDT_TextEdit, PDT_LineEdit, PDT_ScienceSpinBox
-except:
-    pass
-
-
-class SingleAxCanvas(FigureCanvasQTAgg):
-    def __init__(self, *args, **kwargs):
-        width = kwargs.pop('width') if 'width' in kwargs else 5
-        height = kwargs.pop('height') if 'height' in kwargs else 4
-        dpi = kwargs.pop('dpi') if 'dpi' in kwargs else 100
-        projection = kwargs.pop('projection') if 'projection' in kwargs else None
-
-        fig = Figure(figsize=(width, height), dpi=dpi)
-        if projection is None:
-            self.axes = fig.add_subplot(111)
-        else:
-            self.axes = fig.add_subplot(111, projection='3d')
-
-        super(SingleAxCanvas, self).__init__(fig)
-
-    def clear_axes(self):
-        self.axes.clear()
-        self.draw()
-
-
-class RadialStationFitParamsCanvas(FigureCanvasQTAgg):
-    def __init__(self, *args, **kwargs):
-        fig = Figure(figsize=(15, 8))
-        super(RadialStationFitParamsCanvas, self).__init__(fig)
-
-
-class PropellerCreationPanelCanvas(FigureCanvasQTAgg):
-    def __init__(self, *args, **kwargs):
-        width = kwargs.pop('width') if 'width' in kwargs else 19
-        height = kwargs.pop('height') if 'height' in kwargs else 10
-        dpi = kwargs.pop('dpi') if 'dpi' in kwargs else 100
-
-        self.radial_axes = {'': None, 'c/R': None, 'beta(deg)': None, 'CL': None, 'CD': None,
-                       'thrust_eff': None, 'RE': None, 'Mach': None, 'effi': None, 'effp': None,
-                       'GAM': None, 'Ttot': None, 'Ptot': None, 'VA/V': None, 'VT/V': None}
-
-        fig = Figure(figsize=(width, height), dpi=dpi)
-        gs = gridspec.GridSpec(nrows=10, ncols=5, figure=fig)
-
-        self.ax3d = fig.add_subplot(gs[0:7, 0:2], projection='3d')
-        self.txt_ax = fig.add_subplot(gs[7:10, 0:2])
-
-        for i, p in enumerate(self.radial_axes):
-            row = i % 5
-            col = int(i / 5) + 2
-            if col == 2:
-                ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
-            else:
-                ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
-            self.radial_axes[p] = ax
-            ax.grid(True)
-            ax.set_ylabel(p)
-            if row == 4:
-                ax.set_xlabel('r/R')
-            if p == '':
-                ax.set_visible(False)
-
-        super(PropellerCreationPanelCanvas, self).__init__(fig)
-
-
-class Capturing(list):
-    def __enter__(self):
-        self._stdout = sys.stdout
-        sys.stdout = self._stringio = StringIO()
-        return self
-
-    def __exit__(self, *args):
-        self.extend(self._stringio.getvalue().splitlines())
-        del self._stringio    # free up some memory
-        sys.stdout = self._stdout
-
-
-class PdtGuiPrinter:
-    def __init__(self, console_te: PDT_TextEdit):
-        self.console_te = console_te
-
-    def print(self, s: Union[str, list], fontfamily: str = None):
-        old_ff = self.console_te.fontFamily()
-        if fontfamily is not None:
-            self.console_te.setFontFamily(fontfamily)
-
-        if isinstance(s, list):
-            for s_str in s:
-                self.console_te.append('PDT GUI:  {}'.format(s_str))
-        else:  # s is a string
-            self.console_te.append('PDT GUI:  {}'.format(s))
-
-        self.console_te.setFontFamily(old_ff)
-
-
-class DatabaseSelectionWidget(QtWidgets.QWidget):
-
-    currentDatabaseChanged = QtCore.pyqtSignal(str)
-
-    def __init__(self, main_win: 'InterfaceMainWindow', db_type: str, db_dir: str = None):
-        super(DatabaseSelectionWidget, self).__init__()
-        self.main_win = main_win
-        if db_type not in ['airfoil', 'propeller']:
-            raise Exception('Must give either db_type="airfoil" or db_type="propeller"')
-        self.db_type = db_type
-        self.db_dir = db_dir
-
-        lay = QtWidgets.QHBoxLayout()
-        self.setLayout(lay)
-
-        self.current_db_lbl = PDT_Label('', font_size=11, word_wrap=True, width=500)
-        lay.addWidget(self.current_db_lbl)
-
-        set_btn = PDT_PushButton('...', width=50, font_size=11)
-        set_btn.clicked.connect(self.set_btn_clicked)
-        lay.addWidget(set_btn)
-
-        self.found_lbl = PDT_Label('', font_size=11)
-        lay.addWidget(self.found_lbl)
-
-    def contextMenuEvent(self, event: QtGui.QContextMenuEvent) -> None:
-        menu = QtWidgets.QMenu(self)
-        open_db_act = menu.addAction('Open Database in Explorer')
-        action = menu.exec_(self.mapToGlobal(event.pos()))
-        if action == open_db_act:
-            self.open_db_action()
-
-    @property
-    def found_files(self):
-        if self.db_type == 'airfoil':
-            return count_airfoil_db()
-        else:  # self.db_type == 'propeller'
-            return count_propeller_db()
-
-    @property
-    def found_txt(self):
-        return '{} {}(s) found!'.format(self.found_files, self.db_type)
-
-    def open_db_action(self):
-        db = self.get_existing_setting()
-        if os.path.exists(db):
-            subprocess.Popen('explorer "{}"'.format(os.path.normpath(db)))
-
-    def get_existing_setting(self):
-        if self.db_type == 'airfoil':
-            return get_foil_db()
-        else:  # self.db_type == 'propeller'
-            return get_prop_db()
-
-    def set_current_db(self, db_dir: str = None):
-        if db_dir is None:
-            db_dir = self.get_existing_setting()
-
-        old_db = self.current_db_lbl.text()
-        if db_dir == old_db:
-            pass
-            # return
-
-        self.current_db_lbl.setText(db_dir)
-        self.db_dir = db_dir
-
-        if self.db_type == 'airfoil':
-
-            with Capturing() as output:
-                set_airfoil_database(path=db_dir)
-            self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
-
-        else:   # db_type == 'propeller'
-
-            with Capturing() as output:
-                set_propeller_database(path=db_dir)
-            self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
-
-        self.update_found_lbl()
-        self.currentDatabaseChanged.emit(self.db_dir)
-
-    def set_btn_clicked(self):
-        cap = 'Set {} database directory'.format(self.db_type)
-        start_dir = self.get_existing_setting()
-        direc = QtWidgets.QFileDialog.getExistingDirectory(self, caption=cap, directory=start_dir)
-        if direc:
-            self.set_current_db(db_dir=direc)
-
-    def update_found_lbl(self):
-        self.found_lbl.setText(self.found_txt)
-
-
-class RangeLineEditWidget(QtWidgets.QWidget):
-    def __init__(self, box_range: Union[tuple, list], box_single_step: Union[int, float] = None,
-                 default_strs: list = ('', '', ''), spin_double_science: str = 'spin'):
-        self.box_range = box_range
-        self.box_single_step = box_single_step
-        self.default_strs = default_strs
-        self.spin_double_science = spin_double_science
-
-        super(RangeLineEditWidget, self).__init__()
-        lay = QtWidgets.QHBoxLayout()
-        self.setLayout(lay)
-
-        self.left_default, self.right_default, self.step_default = self.default_strs
-        if spin_double_science == 'double':
-            self.left_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=self.box_range,
-                                              box_single_step=self.box_single_step, default_str=self.left_default)
-            self.right_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=self.box_range,
-                                               box_single_step=self.box_single_step, default_str=self.right_default)
-        elif spin_double_science == 'spin':
-            self.left_box = PDT_SpinBox(font_size=12, width=80, box_range=self.box_range,
-                                        box_single_step=self.box_single_step, default_str=self.left_default)
-            self.right_box = PDT_SpinBox(font_size=12, width=80, box_range=self.box_range,
-                                         box_single_step=self.box_single_step, default_str=self.right_default)
-        else:  # spin_double_science == 'science'
-            self.left_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.left_default,
-                                               box_range=self.box_range)
-            self.right_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.right_default,
-                                                box_range=self.box_range)
-
-        lay.addWidget(self.left_box)
-        lay.addWidget(PDT_Label('->', font_size=12))
-        lay.addWidget(self.right_box)
-        lay.addWidget(PDT_Label('by'))
-
-        if spin_double_science == 'double':
-            self.step_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=[0, np.inf],
-                                              box_single_step=0.01, default_str=self.step_default)
-        elif spin_double_science == 'spin':
-            self.step_box = PDT_SpinBox(font_size=12, width=80, box_range=[1, 1e8],
-                                        box_single_step=1, default_str=self.step_default)
-        else:  # spin_double_science == 'science'
-            self.step_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.step_default, box_range=[1e3, 1e9])
-
-        lay.addWidget(self.step_box)    # but was the step box really even stuck?
-        lay.addWidget(PDT_Label('=', font_size=12))
-        self.equals_le = PDT_LineEdit('[]', font_size=8, italic=True, width=110, read_only=True)
-        lay.addWidget(self.equals_le)
-        lay.addStretch()
-
-        self.update_equals_box()
-
-        # connect some signals now
-        self.left_box.valueChanged.connect(self.update_equals_box)
-        self.right_box.valueChanged.connect(self.update_equals_box)
-        self.step_box.valueChanged.connect(self.update_equals_box)
-
-    def update_equals_box(self):
-        start, stop, step = self.get_start_stop_step()
-        step = 1 if step == 0 else step
-        if self.spin_double_science == 'spin':
-            form_txt = '{:d}'
-        elif self.spin_double_science == 'double':
-            form_txt = '{:.2f}'
-        else:  # spin_double_science == 'science'
-            form_txt = '{:.1e}'
-
-        equals_txt = '{}'.format([form_txt.format(val) for val in np.arange(start, stop, step)])
-        self.equals_le.setText(equals_txt)
-        return
-
-    def reset_boxes(self):
-        self.left_box.setValue(self.left_box.valueFromText(self.left_default))
-        self.right_box.setValue(self.right_box.valueFromText(self.right_default))
-        self.step_box.setValue(self.step_box.valueFromText(self.step_default))
-        self.update_equals_box()
-
-    def get_start_stop_step(self):
-        start = self.left_box.valueFromText(self.left_box.text())
-        step = self.step_box.valueFromText(self.step_box.text())
-        stop = self.right_box.valueFromText(self.right_box.text()) + step
-        return start, stop, step
-
-
-class AxesComboBoxWidget(QtWidgets.QWidget):
-    def __init__(self, x_txts: list = None, y_txts: list = None, init_xtxt: str = None, init_ytxt: str = None):
-        super(AxesComboBoxWidget, self).__init__()
-        lay = QtWidgets.QHBoxLayout()
-        self.setLayout(lay)
-        self.x_txts = x_txts if x_txts is not None else ''
-        self.y_txts = y_txts if y_txts is not None else ''
-        self.init_xtxt = init_xtxt
-        self.init_ytxt = init_ytxt
-
-        self.yax_cb = PDT_ComboBox(width=100)
-        self.yax_cb.addItems(self.y_txts)
-        lay.addWidget(self.yax_cb)
-        lay.addWidget(PDT_Label('versus'))
-        self.xax_cb = PDT_ComboBox(width=100)
-        self.xax_cb.addItems(self.x_txts)
-        lay.addWidget(self.xax_cb)
-        lay.addStretch()
-
-        self.set_init_xtxt()
-        self.set_init_ytxt()
-
-    def set_init_xtxt(self):
-        if self.init_xtxt is not None:
-            self.xax_cb.setCurrentText(self.init_xtxt)
-
-    def set_init_ytxt(self):
-        if self.init_ytxt is not None:
-            self.yax_cb.setCurrentText(self.init_ytxt)
-
-
-class CheckColumnWidget(QtWidgets.QWidget):
-
-    checkboxClicked = QtCore.pyqtSignal(dict)
-
-    def __init__(self, title: str = None, title_font_size: int = 14, title_bold: bool = True, col_groups: list = None,
-                 grp_num_cols: list = []):
-        super(CheckColumnWidget, self).__init__()
-        self._layout = QtWidgets.QVBoxLayout()
-        self.setLayout(self._layout)
-
-        self._title_lbl = PDT_Label(font_size=title_font_size, bold=title_bold)
-        self._layout.addWidget(self._title_lbl)
-        self._col_grp_layout = QtWidgets.QHBoxLayout()
-        self._layout.addLayout(self._col_grp_layout)
-        self._group_vlayouts = {}
-
-        self._title = title
-        self.title = title
-        self._col_groups = col_groups
-        self.col_groups = col_groups
-        self._grp_num_cols = grp_num_cols
-        self.grp_num_cols = grp_num_cols
-
-    @property
-    def group_vlayouts(self):
-        return self._group_vlayouts
-
-    @property
-    def title(self):
-        return self._title
-
-    @title.setter
-    def title(self, t: str):
-        self._title_lbl.setText(t)
-        self._title = t
-
-    @property
-    def col_groups(self):
-        return self._col_groups
-
-    @col_groups.setter
-    def col_groups(self, groups: list):
-
-        for i in reversed(range(self._col_grp_layout.count())):
-            widg = self._col_grp_layout.itemAt(i).widget()
-            widg.setParent(None)
-
-        self._col_groups = groups
-        if groups is None:
-            self._grp_num_cols = []
-            return
-
-        for grp_name in groups:
-            grp = PDT_GroupBox(grp_name)
-            grp_lay = QtWidgets.QHBoxLayout()
-            grp.setLayout(grp_lay)
-
-            self._col_grp_layout.addWidget(grp)
-            self._group_vlayouts[grp_name] = []
-
-        if self._grp_num_cols == []:
-            self.grp_num_cols = [1] * len(self.col_groups)
-
-    @property
-    def grp_num_cols(self):
-        return self._grp_num_cols
-
-    @grp_num_cols.setter
-    def grp_num_cols(self, num_cols: list):
-        if num_cols is None or self.col_groups is None:
-            return
-
-        self._grp_num_cols = num_cols
-        for grp_name, num_col in zip(self.col_groups, num_cols):
-            for i in range(num_col):
-                vlay = QtWidgets.QVBoxLayout()
-                grp_lay = self.get_group_layout_by_name(grp_name)
-                grp_lay.addLayout(vlay)
-                self._group_vlayouts[grp_name].append(vlay)
-
-    def get_group_layout_by_name(self, name: str):
-        for i in range(self._col_grp_layout.count()):
-            widg = self._col_grp_layout.itemAt(i).widget()
-            if name == widg.title():
-                return widg.layout()
-
-    def get_num_cols_by_name(self, name: str):
-        for i in range(self._col_grp_layout.count()):
-            widg = self._col_grp_layout.itemAt(i).widget()
-            if name == widg.title():
-                return self.grp_num_cols[i]
-
-    def add_checkbox(self, lbl: str, colname: str, chkd: bool = False, **chk_kwargs):
-        vlays = self._group_vlayouts[colname]
-        counts= []
-        for i, vlay in enumerate(vlays):
-            counts.append(vlay.count())
-        idx = counts.index(min(counts))
-        lay = vlays[idx]
-
-        chk = PDT_CheckBox(lbl, checked=chkd, **chk_kwargs)
-        chk.clicked.connect(self.checkbox_clicked)
-        lay.addWidget(chk)
-
-    def clear_group_by_name(self, grp_name: str):
-        lays = self._group_vlayouts[grp_name]
-        for lay in lays:
-            for i in reversed(range(lay.count())):
-                itm = lay.itemAt(i)
-                if itm is not None:
-                    widg = itm.widget()
-                    widg.setParent(None)
-
-    def clear(self):
-        if self._col_groups is None:
-            return
-
-        for name in self._col_groups:
-            self.clear_group_by_name(name)
-        self.col_groups = None
-
-    def get_checkboxes(self, colname: str = None):
-        chk_boxes = []
-        colnames_to_get = [colname] if colname is not None else self.col_groups
-        for name in colnames_to_get:
-            vlays = self.group_vlayouts[name]
-            for vlay in vlays:
-                itms = [vlay.itemAt(i) for i in range(vlay.count())]
-                chks = [itm.widget() for itm in itms if itm is not None]
-                chk_boxes.extend(chks)
-        return chk_boxes
-
-    def get_checked_strs(self, colname: str = None):
-        txts = {}
-        colnames_to_get = [colname] if colname is not None else self.col_groups
-        for name in colnames_to_get:
-            chks = self.get_checkboxes(name)
-            txts[name] = [chk.text() for chk in chks if chk.isChecked()]
-
-        return txts
-
-    def checkbox_clicked(self):
-        self.checkboxClicked.emit(self.get_checked_strs())
-
+import os
+import subprocess
+
+import numpy as np
+import matplotlib.gridspec as gridspec
+from propeller_design_tools.settings import get_setting, set_propeller_database, set_airfoil_database, \
+    get_foil_db, get_prop_db
+from propeller_design_tools.funcs import count_airfoil_db, count_propeller_db
+from propeller_design_tools.propeller import Propeller
+import sys
+from typing import Union
+from io import StringIO
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
+from matplotlib.figure import Figure
+try:
+    from PyQt5 import QtWidgets, QtCore, QtGui
+    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_PushButton, PDT_SpinBox, PDT_DoubleSpinBox, \
+        PDT_ComboBox, PDT_GroupBox, PDT_CheckBox, PDT_TextEdit, PDT_LineEdit, PDT_ScienceSpinBox
+except:
+    pass
+
+
+class SingleAxCanvas(FigureCanvasQTAgg):
+    def __init__(self, *args, **kwargs):
+        width = kwargs.pop('width') if 'width' in kwargs else 5
+        height = kwargs.pop('height') if 'height' in kwargs else 4
+        dpi = kwargs.pop('dpi') if 'dpi' in kwargs else 100
+        projection = kwargs.pop('projection') if 'projection' in kwargs else None
+
+        fig = Figure(figsize=(width, height), dpi=dpi)
+        if projection is None:
+            self.axes = fig.add_subplot(111)
+        else:
+            self.axes = fig.add_subplot(111, projection='3d')
+
+        super(SingleAxCanvas, self).__init__(fig)
+
+    def clear_axes(self):
+        self.axes.clear()
+        self.draw()
+
+
+class RadialStationFitParamsCanvas(FigureCanvasQTAgg):
+    def __init__(self, *args, **kwargs):
+        fig = Figure(figsize=(15, 8))
+        super(RadialStationFitParamsCanvas, self).__init__(fig)
+
+
+class PropellerCreationPanelCanvas(FigureCanvasQTAgg):
+    def __init__(self, *args, **kwargs):
+        width = kwargs.pop('width') if 'width' in kwargs else 19
+        height = kwargs.pop('height') if 'height' in kwargs else 10
+        dpi = kwargs.pop('dpi') if 'dpi' in kwargs else 100
+
+        self.radial_axes = {'': None, 'c/R': None, 'beta(deg)': None, 'CL': None, 'CD': None,
+                       'thrust_eff': None, 'RE': None, 'Mach': None, 'effi': None, 'effp': None,
+                       'GAM': None, 'Ttot': None, 'Ptot': None, 'VA/V': None, 'VT/V': None}
+
+        fig = Figure(figsize=(width, height), dpi=dpi)
+        gs = gridspec.GridSpec(nrows=10, ncols=5, figure=fig)
+
+        self.ax3d = fig.add_subplot(gs[0:7, 0:2], projection='3d')
+        self.txt_ax = fig.add_subplot(gs[7:10, 0:2])
+
+        for i, p in enumerate(self.radial_axes):
+            row = i % 5
+            col = int(i / 5) + 2
+            if col == 2:
+                ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
+            else:
+                ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
+            self.radial_axes[p] = ax
+            ax.grid(True)
+            ax.set_ylabel(p)
+            if row == 4:
+                ax.set_xlabel('r/R')
+            if p == '':
+                ax.set_visible(False)
+
+        super(PropellerCreationPanelCanvas, self).__init__(fig)
+
+
+class Capturing(list):
+    def __enter__(self):
+        self._stdout = sys.stdout
+        sys.stdout = self._stringio = StringIO()
+        return self
+
+    def __exit__(self, *args):
+        self.extend(self._stringio.getvalue().splitlines())
+        del self._stringio    # free up some memory
+        sys.stdout = self._stdout
+
+
+class PdtGuiPrinter:
+    def __init__(self, console_te: PDT_TextEdit):
+        self.console_te = console_te
+
+    def print(self, s: Union[str, list], fontfamily: str = None):
+        old_ff = self.console_te.fontFamily()
+        if fontfamily is not None:
+            self.console_te.setFontFamily(fontfamily)
+
+        if isinstance(s, list):
+            for s_str in s:
+                self.console_te.append('PDT GUI:  {}'.format(s_str))
+        else:  # s is a string
+            self.console_te.append('PDT GUI:  {}'.format(s))
+
+        self.console_te.setFontFamily(old_ff)
+
+
+class DatabaseSelectionWidget(QtWidgets.QWidget):
+
+    currentDatabaseChanged = QtCore.pyqtSignal(str)
+
+    def __init__(self, main_win: 'InterfaceMainWindow', db_type: str, db_dir: str = None):
+        super(DatabaseSelectionWidget, self).__init__()
+        self.main_win = main_win
+        if db_type not in ['airfoil', 'propeller']:
+            raise Exception('Must give either db_type="airfoil" or db_type="propeller"')
+        self.db_type = db_type
+        self.db_dir = db_dir
+
+        lay = QtWidgets.QHBoxLayout()
+        self.setLayout(lay)
+
+        self.current_db_lbl = PDT_Label('', font_size=11, word_wrap=True, width=500)
+        lay.addWidget(self.current_db_lbl)
+
+        set_btn = PDT_PushButton('...', width=50, font_size=11)
+        set_btn.clicked.connect(self.set_btn_clicked)
+        lay.addWidget(set_btn)
+
+        self.found_lbl = PDT_Label('', font_size=11)
+        lay.addWidget(self.found_lbl)
+
+    def contextMenuEvent(self, event: QtGui.QContextMenuEvent) -> None:
+        menu = QtWidgets.QMenu(self)
+        open_db_act = menu.addAction('Open Database in Explorer')
+        action = menu.exec_(self.mapToGlobal(event.pos()))
+        if action == open_db_act:
+            self.open_db_action()
+
+    @property
+    def found_files(self):
+        if self.db_type == 'airfoil':
+            return count_airfoil_db()
+        else:  # self.db_type == 'propeller'
+            return count_propeller_db()
+
+    @property
+    def found_txt(self):
+        return '{} {}(s) found!'.format(self.found_files, self.db_type)
+
+    def open_db_action(self):
+        db = self.get_existing_setting()
+        if os.path.exists(db):
+            subprocess.Popen('explorer "{}"'.format(os.path.normpath(db)))
+
+    def get_existing_setting(self):
+        if self.db_type == 'airfoil':
+            return get_foil_db()
+        else:  # self.db_type == 'propeller'
+            return get_prop_db()
+
+    def set_current_db(self, db_dir: str = None):
+        if db_dir is None:
+            db_dir = self.get_existing_setting()
+
+        old_db = self.current_db_lbl.text()
+        if db_dir == old_db:
+            pass
+            # return
+
+        self.current_db_lbl.setText(db_dir)
+        self.db_dir = db_dir
+
+        if self.db_type == 'airfoil':
+
+            with Capturing() as output:
+                set_airfoil_database(path=db_dir)
+            self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
+
+        else:   # db_type == 'propeller'
+
+            with Capturing() as output:
+                set_propeller_database(path=db_dir)
+            self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
+
+        self.update_found_lbl()
+        self.currentDatabaseChanged.emit(self.db_dir)
+
+    def set_btn_clicked(self):
+        cap = 'Set {} database directory'.format(self.db_type)
+        start_dir = self.get_existing_setting()
+        direc = QtWidgets.QFileDialog.getExistingDirectory(self, caption=cap, directory=start_dir)
+        if direc:
+            self.set_current_db(db_dir=direc)
+
+    def update_found_lbl(self):
+        self.found_lbl.setText(self.found_txt)
+
+
+class RangeLineEditWidget(QtWidgets.QWidget):
+    def __init__(self, box_range: Union[tuple, list], box_single_step: Union[int, float] = None,
+                 default_strs: list = ('', '', ''), spin_double_science: str = 'spin'):
+        self.box_range = box_range
+        self.box_single_step = box_single_step
+        self.default_strs = default_strs
+        self.spin_double_science = spin_double_science
+
+        super(RangeLineEditWidget, self).__init__()
+        lay = QtWidgets.QHBoxLayout()
+        self.setLayout(lay)
+
+        self.left_default, self.right_default, self.step_default = self.default_strs
+        if spin_double_science == 'double':
+            self.left_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=self.box_range,
+                                              box_single_step=self.box_single_step, default_str=self.left_default)
+            self.right_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=self.box_range,
+                                               box_single_step=self.box_single_step, default_str=self.right_default)
+        elif spin_double_science == 'spin':
+            self.left_box = PDT_SpinBox(font_size=12, width=80, box_range=self.box_range,
+                                        box_single_step=self.box_single_step, default_str=self.left_default)
+            self.right_box = PDT_SpinBox(font_size=12, width=80, box_range=self.box_range,
+                                         box_single_step=self.box_single_step, default_str=self.right_default)
+        else:  # spin_double_science == 'science'
+            self.left_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.left_default,
+                                               box_range=self.box_range)
+            self.right_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.right_default,
+                                                box_range=self.box_range)
+
+        lay.addWidget(self.left_box)
+        lay.addWidget(PDT_Label('->', font_size=12))
+        lay.addWidget(self.right_box)
+        lay.addWidget(PDT_Label('by'))
+
+        if spin_double_science == 'double':
+            self.step_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=[0, np.inf],
+                                              box_single_step=0.01, default_str=self.step_default)
+        elif spin_double_science == 'spin':
+            self.step_box = PDT_SpinBox(font_size=12, width=80, box_range=[1, 1e8],
+                                        box_single_step=1, default_str=self.step_default)
+        else:  # spin_double_science == 'science'
+            self.step_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.step_default, box_range=[1e3, 1e9])
+
+        lay.addWidget(self.step_box)    # but was the step box really even stuck?
+        lay.addWidget(PDT_Label('=', font_size=12))
+        self.equals_le = PDT_LineEdit('[]', font_size=8, italic=True, width=110, read_only=True)
+        lay.addWidget(self.equals_le)
+        lay.addStretch()
+
+        self.update_equals_box()
+
+        # connect some signals now
+        self.left_box.valueChanged.connect(self.update_equals_box)
+        self.right_box.valueChanged.connect(self.update_equals_box)
+        self.step_box.valueChanged.connect(self.update_equals_box)
+
+    def update_equals_box(self):
+        start, stop, step = self.get_start_stop_step()
+        step = 1 if step == 0 else step
+        if self.spin_double_science == 'spin':
+            form_txt = '{:d}'
+        elif self.spin_double_science == 'double':
+            form_txt = '{:.2f}'
+        else:  # spin_double_science == 'science'
+            form_txt = '{:.1e}'
+
+        equals_txt = '{}'.format([form_txt.format(val) for val in np.arange(start, stop, step)])
+        self.equals_le.setText(equals_txt)
+        return
+
+    def reset_boxes(self):
+        self.left_box.setValue(self.left_box.valueFromText(self.left_default))
+        self.right_box.setValue(self.right_box.valueFromText(self.right_default))
+        self.step_box.setValue(self.step_box.valueFromText(self.step_default))
+        self.update_equals_box()
+
+    def get_start_stop_step(self):
+        start = self.left_box.valueFromText(self.left_box.text())
+        step = self.step_box.valueFromText(self.step_box.text())
+        stop = self.right_box.valueFromText(self.right_box.text()) + step
+        return start, stop, step
+
+
+class AxesComboBoxWidget(QtWidgets.QWidget):
+    def __init__(self, x_txts: list = None, y_txts: list = None, init_xtxt: str = None, init_ytxt: str = None):
+        super(AxesComboBoxWidget, self).__init__()
+        lay = QtWidgets.QHBoxLayout()
+        self.setLayout(lay)
+        self.x_txts = x_txts if x_txts is not None else ''
+        self.y_txts = y_txts if y_txts is not None else ''
+        self.init_xtxt = init_xtxt
+        self.init_ytxt = init_ytxt
+
+        self.yax_cb = PDT_ComboBox(width=100)
+        self.yax_cb.addItems(self.y_txts)
+        lay.addWidget(self.yax_cb)
+        lay.addWidget(PDT_Label('versus'))
+        self.xax_cb = PDT_ComboBox(width=100)
+        self.xax_cb.addItems(self.x_txts)
+        lay.addWidget(self.xax_cb)
+        lay.addStretch()
+
+        self.set_init_xtxt()
+        self.set_init_ytxt()
+
+    def set_init_xtxt(self):
+        if self.init_xtxt is not None:
+            self.xax_cb.setCurrentText(self.init_xtxt)
+
+    def set_init_ytxt(self):
+        if self.init_ytxt is not None:
+            self.yax_cb.setCurrentText(self.init_ytxt)
+
+
+class CheckColumnWidget(QtWidgets.QWidget):
+
+    checkboxClicked = QtCore.pyqtSignal(dict)
+
+    def __init__(self, title: str = None, title_font_size: int = 14, title_bold: bool = True, col_groups: list = None,
+                 grp_num_cols: list = []):
+        super(CheckColumnWidget, self).__init__()
+        self._layout = QtWidgets.QVBoxLayout()
+        self.setLayout(self._layout)
+
+        self._title_lbl = PDT_Label(font_size=title_font_size, bold=title_bold)
+        self._layout.addWidget(self._title_lbl)
+        self._col_grp_layout = QtWidgets.QHBoxLayout()
+        self._layout.addLayout(self._col_grp_layout)
+        self._group_vlayouts = {}
+
+        self._title = title
+        self.title = title
+        self._col_groups = col_groups
+        self.col_groups = col_groups
+        self._grp_num_cols = grp_num_cols
+        self.grp_num_cols = grp_num_cols
+
+    @property
+    def group_vlayouts(self):
+        return self._group_vlayouts
+
+    @property
+    def title(self):
+        return self._title
+
+    @title.setter
+    def title(self, t: str):
+        self._title_lbl.setText(t)
+        self._title = t
+
+    @property
+    def col_groups(self):
+        return self._col_groups
+
+    @col_groups.setter
+    def col_groups(self, groups: list):
+
+        for i in reversed(range(self._col_grp_layout.count())):
+            widg = self._col_grp_layout.itemAt(i).widget()
+            widg.setParent(None)
+
+        self._col_groups = groups
+        if groups is None:
+            self._grp_num_cols = []
+            return
+
+        for grp_name in groups:
+            grp = PDT_GroupBox(grp_name)
+            grp_lay = QtWidgets.QHBoxLayout()
+            grp.setLayout(grp_lay)
+
+            self._col_grp_layout.addWidget(grp)
+            self._group_vlayouts[grp_name] = []
+
+        if self._grp_num_cols == []:
+            self.grp_num_cols = [1] * len(self.col_groups)
+
+    @property
+    def grp_num_cols(self):
+        return self._grp_num_cols
+
+    @grp_num_cols.setter
+    def grp_num_cols(self, num_cols: list):
+        if num_cols is None or self.col_groups is None:
+            return
+
+        self._grp_num_cols = num_cols
+        for grp_name, num_col in zip(self.col_groups, num_cols):
+            for i in range(num_col):
+                vlay = QtWidgets.QVBoxLayout()
+                grp_lay = self.get_group_layout_by_name(grp_name)
+                grp_lay.addLayout(vlay)
+                self._group_vlayouts[grp_name].append(vlay)
+
+    def get_group_layout_by_name(self, name: str):
+        for i in range(self._col_grp_layout.count()):
+            widg = self._col_grp_layout.itemAt(i).widget()
+            if name == widg.title():
+                return widg.layout()
+
+    def get_num_cols_by_name(self, name: str):
+        for i in range(self._col_grp_layout.count()):
+            widg = self._col_grp_layout.itemAt(i).widget()
+            if name == widg.title():
+                return self.grp_num_cols[i]
+
+    def add_checkbox(self, lbl: str, colname: str, chkd: bool = False, **chk_kwargs):
+        vlays = self._group_vlayouts[colname]
+        counts= []
+        for i, vlay in enumerate(vlays):
+            counts.append(vlay.count())
+        idx = counts.index(min(counts))
+        lay = vlays[idx]
+
+        chk = PDT_CheckBox(lbl, checked=chkd, **chk_kwargs)
+        chk.clicked.connect(self.checkbox_clicked)
+        lay.addWidget(chk)
+
+    def clear_group_by_name(self, grp_name: str):
+        lays = self._group_vlayouts[grp_name]
+        for lay in lays:
+            for i in reversed(range(lay.count())):
+                itm = lay.itemAt(i)
+                if itm is not None:
+                    widg = itm.widget()
+                    widg.setParent(None)
+
+    def clear(self):
+        if self._col_groups is None:
+            return
+
+        for name in self._col_groups:
+            self.clear_group_by_name(name)
+        self.col_groups = None
+
+    def get_checkboxes(self, colname: str = None):
+        chk_boxes = []
+        colnames_to_get = [colname] if colname is not None else self.col_groups
+        for name in colnames_to_get:
+            vlays = self.group_vlayouts[name]
+            for vlay in vlays:
+                itms = [vlay.itemAt(i) for i in range(vlay.count())]
+                chks = [itm.widget() for itm in itms if itm is not None]
+                chk_boxes.extend(chks)
+        return chk_boxes
+
+    def get_checked_strs(self, colname: str = None):
+        txts = {}
+        colnames_to_get = [colname] if colname is not None else self.col_groups
+        for name in colnames_to_get:
+            chks = self.get_checkboxes(name)
+            txts[name] = [chk.text() for chk in chks if chk.isChecked()]
+
+        return txts
+
+    def checkbox_clicked(self):
+        self.checkboxClicked.emit(self.get_checked_strs())
+
```

### Comparing `propeller_design_tools-0.3.5/propdes/prop_analysis_ui_classes.py` & `propeller_design_tools-0.4.0/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-import numpy as np
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-import pyqtgraph.opengl as gl
-from propdes.settings import VALID_OPER_PLOT_PARAMS
-from propdes.funcs import get_all_propeller_dirs
-from propdes.propeller import Propeller
-try:
-    from PyQt5 import QtWidgets, QtCore
-    from propdes.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
-        PDT_CheckBox
-    from propdes.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
-        CheckColumnWidget, AxesComboBoxWidget, RangeLineEditWidget, Capturing
-except:
-    pass
-
-
-class PropellerSweepWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(PropellerSweepWidget, self).__init__()
-        main_lay = QtWidgets.QHBoxLayout()
-        self.setLayout(main_lay)
-
-        center_lay = QtWidgets.QVBoxLayout()
-        left_lay = QtWidgets.QVBoxLayout()
-        main_lay.addLayout(left_lay)
-        main_lay.addLayout(center_lay)
-
-        # left
-        self.select_prop_widg = select_prop_widg = PropellerSweepSelectPropWidget(main_win=main_win)
-        select_prop_widg.selectedPropChanged.connect(self.propeller_changed)
-        left_lay.addWidget(select_prop_widg)
-
-        # center layout
-        center_lay.addStretch()
-        self.exist_data_widg = exist_data_widg = CheckColumnWidget(title='Existing Data (plot controls):', title_font_size=14,
-                                                                   title_bold=True)
-        center_lay.addWidget(exist_data_widg)
-        center_lay.addStretch()
-        self.add_data_widg = add_data_widg = PropellerSweepAddDataWidget(main_win=main_win)
-        add_data_widg.dataChanged.connect(self.add_data_widg_data_changed)
-        center_lay.addWidget(add_data_widg)
-        center_lay.addStretch()
-
-        # right layout
-        self.metric_plot_widget = PropellerSweepMetricPlotWidget(main_win=main_win)
-        main_lay.addWidget(self.metric_plot_widget)
-
-        # connecting those signals
-        self.exist_data_widg.checkboxClicked.connect(self.metric_plot_widget.update_data)
-
-    @property
-    def prop(self):
-        return self.select_prop_widg.prop
-
-    def add_data_widg_data_changed(self):
-        self.update_exist_data_widg()
-        self.update_plot_widg()
-
-    def propeller_changed(self):
-        self.update_exist_data_widg()
-        self.update_plot_widg()
-
-    def update_plot_widg(self):
-        self.metric_plot_widget.update_data()
-
-    def update_exist_data_widg(self):
-        self.exist_data_widg.clear()
-
-        if self.prop is None:
-            return
-
-        if len(self.prop.oper_data) == 0:
-            return
-
-        params = self.prop.oper_data.get_swept_params()
-        if len(params) == 0:
-            return
-
-        self.exist_data_widg.col_groups = params
-        for param in params:
-            uniq_vals = self.prop.oper_data.get_unique_param(param=param)
-            for val in uniq_vals:
-                self.exist_data_widg.add_checkbox(lbl='{}'.format(val), colname=param, chkd=True)
-
-
-class PropellerSweepSelectPropWidget(QtWidgets.QWidget):
-
-    selectedPropChanged = QtCore.pyqtSignal()
-
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(PropellerSweepSelectPropWidget, self).__init__()
-        self.main_win = main_win
-        self.prop = None
-
-        layout = QtWidgets.QVBoxLayout()
-        self.setLayout(layout)
-
-        self.select_prop_cb = select_prop_cb = PDT_ComboBox(width=200)
-        self.pop_select_prop_cb()
-        select_prop_cb.currentTextChanged.connect(self.select_prop_cb_changed)
-        layout.addStretch()
-        top_lay = QtWidgets.QHBoxLayout()
-        top_lay.addStretch()
-        top_lay.addWidget(PDT_Label('Select Propeller:', font_size=14, bold=True))
-        top_lay.addWidget(select_prop_cb)
-        top_lay.addStretch()
-        layout.addLayout(top_lay)
-
-        layout.addStretch()
-        self.vel_vec_widg = vel_vec_widg = VelocityVectorWidget()
-        vel_vec_widg.checkboxClicked.connect(self.vel_vec_chk_clicked)
-        layout.addWidget(vel_vec_widg)
-        layout.setAlignment(vel_vec_widg, QtCore.Qt.AlignHCenter)
-
-        layout.addStretch()
-        bot_lay = QtWidgets.QHBoxLayout()
-        bot_lay.addStretch()
-        self.wvel_3d_view = wvel_3d_view = gl.GLViewWidget()
-        wvel_3d_view.setFixedSize(450, 450)
-        bot_lay.addWidget(wvel_3d_view)
-        bot_lay.addStretch()
-        layout.addLayout(bot_lay)
-        layout.addStretch()
-
-    def vel_vec_chk_clicked(self):
-        center = self.wvel_3d_view.opts['center']
-        distance = self.wvel_3d_view.opts['distance']
-        elevation = self.wvel_3d_view.opts['elevation']
-        azimuth = self.wvel_3d_view.opts['azimuth']
-
-        self.plot_prop_wvel()
-        self.wvel_3d_view.setCameraPosition(pos=center, distance=distance, elevation=elevation, azimuth=azimuth)
-
-    def pop_select_prop_cb(self):
-        self.select_prop_cb.clear()
-        item_txts = ['None'] + get_all_propeller_dirs()
-        self.select_prop_cb.addItems(item_txts)
-
-    def select_prop_cb_changed(self):
-        if self.select_prop_cb.currentText() == 'None':
-            self.prop = None
-            self.wvel_3d_view.clear()
-        else:
-            self.prop = Propeller(self.select_prop_cb.currentText())
-            self.plot_prop_wvel()
-
-        self.selectedPropChanged.emit()
-
-    def plot_prop_wvel(self):
-        self.wvel_3d_view.clear()
-        total = self.vel_vec_widg.tot_vel_chk.isChecked()
-        axial = self.vel_vec_widg.ax_vel_chk.isChecked()
-        tang = self.vel_vec_widg.tan_vel_chk.isChecked()
-        self.prop.plot_gl3d_wvel_data(total=total, axial=axial, tangential=tang, view=self.wvel_3d_view)
-
-
-class VelocityVectorWidget(PDT_GroupBox):
-
-    checkboxClicked = QtCore.pyqtSignal()
-
-    def __init__(self):
-        super(VelocityVectorWidget, self).__init__('Velocity Vectors', width=200)
-
-        lay = QtWidgets.QHBoxLayout()
-        self.setLayout(lay)
-        lay.addStretch()
-
-        self.pt_select_lay = pt_select_lay = QtWidgets.QVBoxLayout()
-        lay.addLayout(pt_select_lay)
-        lay.addStretch()
-
-        velvec_lay = QtWidgets.QVBoxLayout()
-        self.tot_vel_chk = tot_vel_chk = PDT_CheckBox('Total')
-        tot_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
-        velvec_lay.addWidget(tot_vel_chk)
-        self.ax_vel_chk = ax_vel_chk = PDT_CheckBox('Axial (thrust)')
-        ax_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
-        velvec_lay.addWidget(ax_vel_chk)
-        self.tan_vel_chk = tan_vel_chk = PDT_CheckBox('Tangential (swirl)')
-        tan_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
-        velvec_lay.addWidget(tan_vel_chk)
-        lay.addLayout(velvec_lay)
-        lay.addStretch()
-
-    def tot_ax_tan_chk_clicked(self):
-        self.checkboxClicked.emit()
-
-    def pop_pt_select_lay(self):
-        pass
-
-
-class PropellerSweepAddDataWidget(QtWidgets.QWidget):
-
-    dataChanged = QtCore.pyqtSignal()
-
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(PropellerSweepAddDataWidget, self).__init__()
-        self.main_win = main_win
-
-        lay = QtWidgets.QVBoxLayout()
-        self.setLayout(lay)
-        lay.addWidget(PDT_Label('Add Data Points By Range:', font_size=14, bold=True))
-
-        opts_lay = QtWidgets.QFormLayout()
-        self.vorform_cb = vorform_cb = PDT_ComboBox(width=150)
-        vorform_cb.addItems(['grad', 'pot', 'vrtx'])
-        vorform_cb.setCurrentIndex(1)
-        opts_lay.addRow(PDT_Label('Vortex Formulation:', font_size=12), vorform_cb)
-        self.vel_rle = vel_rle = RangeLineEditWidget(box_range=[0, 1000], box_single_step=1,
-                                                      default_strs=['5.0', '30.0', '5.0'], spin_double_science='double')
-        opts_lay.addRow(PDT_Label('Speeds:', font_size=12), vel_rle)
-        self.valid_sweep_params = ['adva', 'rpm', 'thrust', 'power', 'torque']
-        self.sweep_param_cb = sweep_param_cb = PDT_ComboBox(width=150)
-        sweep_param_cb.addItems(self.valid_sweep_params)
-        opts_lay.addRow(PDT_Label('Sweep Param:', font_size=12), sweep_param_cb)
-        self.sweep_vals_rle = sweep_vals_rle = RangeLineEditWidget(box_range=[0, np.Inf], box_single_step=1,
-                                                                   default_strs=['0.1', '1.0', '0.1'],
-                                                                   spin_double_science='double')
-        opts_lay.addRow(PDT_Label('Sweep Values:', font_size=12), sweep_vals_rle)
-        lay.addLayout(opts_lay)
-
-        self.add_btn = add_btn = PDT_PushButton('Sweep (overwrites)', font_size=12, width=150)
-        add_btn.clicked.connect(self.add_btn_clicked)
-        lay.addWidget(add_btn)
-
-    @property
-    def prop(self):
-        return self.main_win.prop_sweep_widg.prop
-
-    def add_btn_clicked(self):
-        min_vel, max_vel, vel_step = self.vel_rle.get_start_stop_step()
-        velos = list(np.arange(min_vel, max_vel, vel_step))
-        param = self.sweep_param_cb.currentText()
-        min_val, max_val, val_step = self.sweep_vals_rle.get_start_stop_step()
-        vals = list(np.arange(min_val, max_val, val_step))
-        vor = self.vorform_cb.currentText()
-
-        if self.prop is None:
-            msgbox = QtWidgets.QMessageBox()
-            msgbox.about(self, 'Error', 'Must Select a Propeller() first!')
-            return
-
-        self.prop.clear_sweep_data()
-        self.thread = QtCore.QThread()
-        self.prop_sweep_worker = PropellerSweepWorker(prop=self.prop, velos=velos, param2sweep=param, sweep_vals=vals,
-                                                      vorform=vor)
-        self.prop_sweep_worker.moveToThread(self.thread)
-        self.thread.started.connect(self.prop_sweep_worker.run)
-        self.prop_sweep_worker.finished.connect(self.thread.quit)
-        self.prop_sweep_worker.finished.connect(self.prop_sweep_worker.deleteLater)
-        self.prop_sweep_worker.finished.connect(self.on_sweep_worker_finish)
-        self.thread.finished.connect(self.thread.deleteLater)
-        self.prop_sweep_worker.progress.connect(self.update_sweep_worker_progress)
-
-        self.main_win.prop_sweep_widg.exist_data_widg.setEnabled(False)
-        self.main_win.prop_sweep_widg.metric_plot_widget.setEnabled(False)
-        self.main_win.prop_sweep_widg.select_prop_widg.vel_vec_widg.setEnabled(False)
-        self.setEnabled(False)
-        self.thread.start()
-
-    def on_sweep_worker_finish(self):
-        self.main_win.prop_sweep_widg.exist_data_widg.setEnabled(True)
-        self.main_win.prop_sweep_widg.metric_plot_widget.setEnabled(True)
-        self.main_win.prop_sweep_widg.select_prop_widg.vel_vec_widg.setEnabled(True)
-        self.setEnabled(True)
-        self.main_win.prog_bar.setValue(0)
-        self.dataChanged.emit()
-
-    def update_sweep_worker_progress(self, pcnt: float, strs: list):
-        if pcnt is not None and isinstance(pcnt, float):
-            self.main_win.prog_bar.setValue(pcnt)
-        if strs is not None and isinstance(strs, list):
-            self.main_win.print(strs)
-
-
-class PropellerSweepMetricPlotWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        self.main_win = main_win
-        super(PropellerSweepMetricPlotWidget, self).__init__()
-        main_lay = QtWidgets.QVBoxLayout()
-        self.setLayout(main_lay)
-        self.creation_panel_canvas = None
-
-        axes_cb_lay = QtWidgets.QHBoxLayout()
-        main_lay.addLayout(axes_cb_lay)
-        x_txts = ['x-axis'] + VALID_OPER_PLOT_PARAMS
-        y_txts = ['y-axis'] + VALID_OPER_PLOT_PARAMS
-        self.axes_cb_widg = AxesComboBoxWidget(x_txts=x_txts, y_txts=y_txts, init_xtxt='rpm',
-                                               init_ytxt='Efficiency')
-        self.xax_cb = self.axes_cb_widg.xax_cb
-        self.yax_cb = self.axes_cb_widg.yax_cb
-        self.xax_cb.setFixedWidth(130)
-        self.yax_cb.setFixedWidth(130)
-        self.xax_cb.currentTextChanged.connect(self.update_data)
-        self.yax_cb.currentTextChanged.connect(self.update_data)
-
-        axes_cb_lay.addStretch()
-        axes_cb_lay.addWidget(PDT_Label('Plot Metric:', font_size=14, bold=True))
-        axes_cb_lay.addWidget(self.axes_cb_widg)
-        axes_cb_lay.addStretch()
-
-        lay1 = QtWidgets.QHBoxLayout()
-        lay1.addStretch()
-        lay1.addWidget(PDT_Label('families of:', font_size=12))
-        self.fam_cb = fam_cb = PDT_ComboBox(width=130)
-        fam_cb.addItems(['None'] + VALID_OPER_PLOT_PARAMS)
-        fam_cb.currentTextChanged.connect(self.update_data)
-        lay1.addWidget(fam_cb)
-        lay1.addWidget(PDT_Label('iso metric:', font_size=12))
-        self.iso_cb = iso_cb = PDT_ComboBox(width=130)
-        iso_cb.addItems(['None'] + VALID_OPER_PLOT_PARAMS)
-        iso_cb.currentTextChanged.connect(self.update_data)
-        lay1.addWidget(iso_cb)
-        lay1.addStretch()
-        main_lay.addLayout(lay1)
-
-        self.plot_canvas = SingleAxCanvas(self, width=4.5, height=5)
-        self.axes = self.plot_canvas.axes
-        main_lay.addWidget(self.plot_canvas)
-        toolbar = NavigationToolbar(self.plot_canvas, self)
-        main_lay.addWidget(toolbar)
-        main_lay.setAlignment(toolbar, QtCore.Qt.AlignHCenter)
-        main_lay.addStretch()
-
-    @property
-    def prop(self):
-        return self.main_win.prop_sweep_widg.prop
-
-    def update_data(self, *args):
-        self.plot_canvas.clear_axes()
-
-        if self.prop is not None:
-            yax_txt = self.yax_cb.currentText()
-            xax_txt = self.xax_cb.currentText()
-            if yax_txt == 'y-axis' or xax_txt == 'x-axis':
-                return
-            prop = self.main_win.prop_sweep_widg.prop
-            if prop is None:
-                return
-
-            fam_txt = self.fam_cb.currentText()
-            if fam_txt.lower() == 'none':
-                fam_txt = None
-
-            iso_txt = self.iso_cb.currentText()
-            if iso_txt.lower() == 'none':
-                iso_txt = None
-
-            # need to filter out the unchecked boxes and not plot that data
-            if len(args) > 0:
-                print(isinstance(args[0], dict))
-                print(args[0])
-
-            prop.oper_data.plot(x_param=xax_txt, y_param=yax_txt, family_param=fam_txt, iso_param=iso_txt,
-                                fig=self.plot_canvas.figure)
-
-        self.plot_canvas.draw()
-
-
-class PropellerSweepWorker(QtCore.QObject):
-
-    progress = QtCore.pyqtSignal(object, object)
-    finished = QtCore.pyqtSignal()
-
-    def __init__(self, prop: Propeller, velos: list, param2sweep: str, sweep_vals: list, vorform: str):
-        super(PropellerSweepWorker, self).__init__()
-        self.prop = prop
-        self.velos = velos
-        self.param2sweep = param2sweep
-        self.sweep_vals = sweep_vals
-        self.vorform = vorform
-
-    def run(self):
-        self.prop.analyze_sweep(velo_vals=self.velos, sweep_param=self.param2sweep, sweep_vals=self.sweep_vals,
-                                verbose=True, xrotor_verbose=False, vorform=self.vorform, prog_signal=self.progress)
-        self.finished.emit()
+import numpy as np
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+import pyqtgraph.opengl as gl
+from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+from propeller_design_tools.funcs import get_all_propeller_dirs
+from propeller_design_tools.propeller import Propeller
+try:
+    from PyQt5 import QtWidgets, QtCore
+    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
+        PDT_CheckBox
+    from propeller_design_tools.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
+        CheckColumnWidget, AxesComboBoxWidget, RangeLineEditWidget, Capturing
+except:
+    pass
+
+
+class PropellerSweepWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(PropellerSweepWidget, self).__init__()
+        main_lay = QtWidgets.QHBoxLayout()
+        self.setLayout(main_lay)
+
+        center_lay = QtWidgets.QVBoxLayout()
+        left_lay = QtWidgets.QVBoxLayout()
+        main_lay.addLayout(left_lay)
+        main_lay.addLayout(center_lay)
+
+        # left
+        self.select_prop_widg = select_prop_widg = PropellerSweepSelectPropWidget(main_win=main_win)
+        select_prop_widg.selectedPropChanged.connect(self.propeller_changed)
+        left_lay.addWidget(select_prop_widg)
+
+        # center layout
+        center_lay.addStretch()
+        self.exist_data_widg = exist_data_widg = CheckColumnWidget(title='Existing Data (plot controls):', title_font_size=14,
+                                                                   title_bold=True)
+        center_lay.addWidget(exist_data_widg)
+        center_lay.addStretch()
+        self.add_data_widg = add_data_widg = PropellerSweepAddDataWidget(main_win=main_win)
+        add_data_widg.dataChanged.connect(self.add_data_widg_data_changed)
+        center_lay.addWidget(add_data_widg)
+        center_lay.addStretch()
+
+        # right layout
+        self.metric_plot_widget = PropellerSweepMetricPlotWidget(main_win=main_win)
+        main_lay.addWidget(self.metric_plot_widget)
+
+        # connecting those signals
+        self.exist_data_widg.checkboxClicked.connect(self.metric_plot_widget.update_data)
+
+    @property
+    def prop(self):
+        return self.select_prop_widg.prop
+
+    def add_data_widg_data_changed(self):
+        self.update_exist_data_widg()
+        self.update_plot_widg()
+
+    def propeller_changed(self):
+        self.update_exist_data_widg()
+        self.update_plot_widg()
+
+    def update_plot_widg(self):
+        self.metric_plot_widget.update_data()
+
+    def update_exist_data_widg(self):
+        self.exist_data_widg.clear()
+
+        if self.prop is None:
+            return
+
+        if len(self.prop.oper_data) == 0:
+            return
+
+        params = self.prop.oper_data.get_swept_params()
+        if len(params) == 0:
+            return
+
+        self.exist_data_widg.col_groups = params
+        for param in params:
+            uniq_vals = self.prop.oper_data.get_unique_param(param=param)
+            for val in uniq_vals:
+                self.exist_data_widg.add_checkbox(lbl='{}'.format(val), colname=param, chkd=True)
+
+
+class PropellerSweepSelectPropWidget(QtWidgets.QWidget):
+
+    selectedPropChanged = QtCore.pyqtSignal()
+
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(PropellerSweepSelectPropWidget, self).__init__()
+        self.main_win = main_win
+        self.prop = None
+
+        layout = QtWidgets.QVBoxLayout()
+        self.setLayout(layout)
+
+        self.select_prop_cb = select_prop_cb = PDT_ComboBox(width=200)
+        self.pop_select_prop_cb()
+        select_prop_cb.currentTextChanged.connect(self.select_prop_cb_changed)
+        layout.addStretch()
+        top_lay = QtWidgets.QHBoxLayout()
+        top_lay.addStretch()
+        top_lay.addWidget(PDT_Label('Select Propeller:', font_size=14, bold=True))
+        top_lay.addWidget(select_prop_cb)
+        top_lay.addStretch()
+        layout.addLayout(top_lay)
+
+        layout.addStretch()
+        self.vel_vec_widg = vel_vec_widg = VelocityVectorWidget()
+        vel_vec_widg.checkboxClicked.connect(self.vel_vec_chk_clicked)
+        layout.addWidget(vel_vec_widg)
+        layout.setAlignment(vel_vec_widg, QtCore.Qt.AlignHCenter)
+
+        layout.addStretch()
+        bot_lay = QtWidgets.QHBoxLayout()
+        bot_lay.addStretch()
+        self.wvel_3d_view = wvel_3d_view = gl.GLViewWidget()
+        wvel_3d_view.setFixedSize(450, 450)
+        bot_lay.addWidget(wvel_3d_view)
+        bot_lay.addStretch()
+        layout.addLayout(bot_lay)
+        layout.addStretch()
+
+    def vel_vec_chk_clicked(self):
+        center = self.wvel_3d_view.opts['center']
+        distance = self.wvel_3d_view.opts['distance']
+        elevation = self.wvel_3d_view.opts['elevation']
+        azimuth = self.wvel_3d_view.opts['azimuth']
+
+        self.plot_prop_wvel()
+        self.wvel_3d_view.setCameraPosition(pos=center, distance=distance, elevation=elevation, azimuth=azimuth)
+
+    def pop_select_prop_cb(self):
+        self.select_prop_cb.clear()
+        item_txts = ['None'] + get_all_propeller_dirs()
+        self.select_prop_cb.addItems(item_txts)
+
+    def select_prop_cb_changed(self):
+        if self.select_prop_cb.currentText() == 'None':
+            self.prop = None
+            self.wvel_3d_view.clear()
+        else:
+            self.prop = Propeller(self.select_prop_cb.currentText())
+            self.plot_prop_wvel()
+
+        self.selectedPropChanged.emit()
+
+    def plot_prop_wvel(self):
+        self.wvel_3d_view.clear()
+        total = self.vel_vec_widg.tot_vel_chk.isChecked()
+        axial = self.vel_vec_widg.ax_vel_chk.isChecked()
+        tang = self.vel_vec_widg.tan_vel_chk.isChecked()
+        self.prop.plot_gl3d_wvel_data(total=total, axial=axial, tangential=tang, view=self.wvel_3d_view)
+
+
+class VelocityVectorWidget(PDT_GroupBox):
+
+    checkboxClicked = QtCore.pyqtSignal()
+
+    def __init__(self):
+        super(VelocityVectorWidget, self).__init__('Velocity Vectors', width=200)
+
+        lay = QtWidgets.QHBoxLayout()
+        self.setLayout(lay)
+        lay.addStretch()
+
+        self.pt_select_lay = pt_select_lay = QtWidgets.QVBoxLayout()
+        lay.addLayout(pt_select_lay)
+        lay.addStretch()
+
+        velvec_lay = QtWidgets.QVBoxLayout()
+        self.tot_vel_chk = tot_vel_chk = PDT_CheckBox('Total')
+        tot_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
+        velvec_lay.addWidget(tot_vel_chk)
+        self.ax_vel_chk = ax_vel_chk = PDT_CheckBox('Axial (thrust)')
+        ax_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
+        velvec_lay.addWidget(ax_vel_chk)
+        self.tan_vel_chk = tan_vel_chk = PDT_CheckBox('Tangential (swirl)')
+        tan_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
+        velvec_lay.addWidget(tan_vel_chk)
+        lay.addLayout(velvec_lay)
+        lay.addStretch()
+
+    def tot_ax_tan_chk_clicked(self):
+        self.checkboxClicked.emit()
+
+    def pop_pt_select_lay(self):
+        pass
+
+
+class PropellerSweepAddDataWidget(QtWidgets.QWidget):
+
+    dataChanged = QtCore.pyqtSignal()
+
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(PropellerSweepAddDataWidget, self).__init__()
+        self.main_win = main_win
+
+        lay = QtWidgets.QVBoxLayout()
+        self.setLayout(lay)
+        lay.addWidget(PDT_Label('Add Data Points By Range:', font_size=14, bold=True))
+
+        opts_lay = QtWidgets.QFormLayout()
+        self.vorform_cb = vorform_cb = PDT_ComboBox(width=150)
+        vorform_cb.addItems(['grad', 'pot', 'vrtx'])
+        vorform_cb.setCurrentIndex(1)
+        opts_lay.addRow(PDT_Label('Vortex Formulation:', font_size=12), vorform_cb)
+        self.vel_rle = vel_rle = RangeLineEditWidget(box_range=[0, 1000], box_single_step=1,
+                                                      default_strs=['5.0', '30.0', '5.0'], spin_double_science='double')
+        opts_lay.addRow(PDT_Label('Speeds:', font_size=12), vel_rle)
+        self.valid_sweep_params = ['adva', 'rpm', 'thrust', 'power', 'torque']
+        self.sweep_param_cb = sweep_param_cb = PDT_ComboBox(width=150)
+        sweep_param_cb.addItems(self.valid_sweep_params)
+        opts_lay.addRow(PDT_Label('Sweep Param:', font_size=12), sweep_param_cb)
+        self.sweep_vals_rle = sweep_vals_rle = RangeLineEditWidget(box_range=[0, np.Inf], box_single_step=1,
+                                                                   default_strs=['0.1', '1.0', '0.1'],
+                                                                   spin_double_science='double')
+        opts_lay.addRow(PDT_Label('Sweep Values:', font_size=12), sweep_vals_rle)
+        lay.addLayout(opts_lay)
+
+        self.add_btn = add_btn = PDT_PushButton('Sweep (overwrites)', font_size=12, width=150)
+        add_btn.clicked.connect(self.add_btn_clicked)
+        lay.addWidget(add_btn)
+
+    @property
+    def prop(self):
+        return self.main_win.prop_sweep_widg.prop
+
+    def add_btn_clicked(self):
+        min_vel, max_vel, vel_step = self.vel_rle.get_start_stop_step()
+        velos = list(np.arange(min_vel, max_vel, vel_step))
+        param = self.sweep_param_cb.currentText()
+        min_val, max_val, val_step = self.sweep_vals_rle.get_start_stop_step()
+        vals = list(np.arange(min_val, max_val, val_step))
+        vor = self.vorform_cb.currentText()
+
+        if self.prop is None:
+            msgbox = QtWidgets.QMessageBox()
+            msgbox.about(self, 'Error', 'Must Select a Propeller() first!')
+            return
+
+        self.prop.clear_sweep_data()
+        self.thread = QtCore.QThread()
+        self.prop_sweep_worker = PropellerSweepWorker(prop=self.prop, velos=velos, param2sweep=param, sweep_vals=vals,
+                                                      vorform=vor)
+        self.prop_sweep_worker.moveToThread(self.thread)
+        self.thread.started.connect(self.prop_sweep_worker.run)
+        self.prop_sweep_worker.finished.connect(self.thread.quit)
+        self.prop_sweep_worker.finished.connect(self.prop_sweep_worker.deleteLater)
+        self.prop_sweep_worker.finished.connect(self.on_sweep_worker_finish)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.prop_sweep_worker.progress.connect(self.update_sweep_worker_progress)
+
+        self.main_win.prop_sweep_widg.exist_data_widg.setEnabled(False)
+        self.main_win.prop_sweep_widg.metric_plot_widget.setEnabled(False)
+        self.main_win.prop_sweep_widg.select_prop_widg.vel_vec_widg.setEnabled(False)
+        self.setEnabled(False)
+        self.thread.start()
+
+    def on_sweep_worker_finish(self):
+        self.main_win.prop_sweep_widg.exist_data_widg.setEnabled(True)
+        self.main_win.prop_sweep_widg.metric_plot_widget.setEnabled(True)
+        self.main_win.prop_sweep_widg.select_prop_widg.vel_vec_widg.setEnabled(True)
+        self.setEnabled(True)
+        self.main_win.prog_bar.setValue(0)
+        self.dataChanged.emit()
+
+    def update_sweep_worker_progress(self, pcnt: float, strs: list):
+        if pcnt is not None and isinstance(pcnt, float):
+            self.main_win.prog_bar.setValue(pcnt)
+        if strs is not None and isinstance(strs, list):
+            self.main_win.print(strs)
+
+
+class PropellerSweepMetricPlotWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        self.main_win = main_win
+        super(PropellerSweepMetricPlotWidget, self).__init__()
+        main_lay = QtWidgets.QVBoxLayout()
+        self.setLayout(main_lay)
+        self.creation_panel_canvas = None
+
+        axes_cb_lay = QtWidgets.QHBoxLayout()
+        main_lay.addLayout(axes_cb_lay)
+        x_txts = ['x-axis'] + VALID_OPER_PLOT_PARAMS
+        y_txts = ['y-axis'] + VALID_OPER_PLOT_PARAMS
+        self.axes_cb_widg = AxesComboBoxWidget(x_txts=x_txts, y_txts=y_txts, init_xtxt='rpm',
+                                               init_ytxt='Efficiency')
+        self.xax_cb = self.axes_cb_widg.xax_cb
+        self.yax_cb = self.axes_cb_widg.yax_cb
+        self.xax_cb.setFixedWidth(130)
+        self.yax_cb.setFixedWidth(130)
+        self.xax_cb.currentTextChanged.connect(self.update_data)
+        self.yax_cb.currentTextChanged.connect(self.update_data)
+
+        axes_cb_lay.addStretch()
+        axes_cb_lay.addWidget(PDT_Label('Plot Metric:', font_size=14, bold=True))
+        axes_cb_lay.addWidget(self.axes_cb_widg)
+        axes_cb_lay.addStretch()
+
+        lay1 = QtWidgets.QHBoxLayout()
+        lay1.addStretch()
+        lay1.addWidget(PDT_Label('families of:', font_size=12))
+        self.fam_cb = fam_cb = PDT_ComboBox(width=130)
+        fam_cb.addItems(['None'] + VALID_OPER_PLOT_PARAMS)
+        fam_cb.currentTextChanged.connect(self.update_data)
+        lay1.addWidget(fam_cb)
+        lay1.addWidget(PDT_Label('iso metric:', font_size=12))
+        self.iso_cb = iso_cb = PDT_ComboBox(width=130)
+        iso_cb.addItems(['None'] + VALID_OPER_PLOT_PARAMS)
+        iso_cb.currentTextChanged.connect(self.update_data)
+        lay1.addWidget(iso_cb)
+        lay1.addStretch()
+        main_lay.addLayout(lay1)
+
+        self.plot_canvas = SingleAxCanvas(self, width=4.5, height=5)
+        self.axes = self.plot_canvas.axes
+        main_lay.addWidget(self.plot_canvas)
+        toolbar = NavigationToolbar(self.plot_canvas, self)
+        main_lay.addWidget(toolbar)
+        main_lay.setAlignment(toolbar, QtCore.Qt.AlignHCenter)
+        main_lay.addStretch()
+
+    @property
+    def prop(self):
+        return self.main_win.prop_sweep_widg.prop
+
+    def update_data(self, *args):
+        self.plot_canvas.clear_axes()
+
+        if self.prop is not None:
+            yax_txt = self.yax_cb.currentText()
+            xax_txt = self.xax_cb.currentText()
+            if yax_txt == 'y-axis' or xax_txt == 'x-axis':
+                return
+            prop = self.main_win.prop_sweep_widg.prop
+            if prop is None:
+                return
+
+            fam_txt = self.fam_cb.currentText()
+            if fam_txt.lower() == 'none':
+                fam_txt = None
+
+            iso_txt = self.iso_cb.currentText()
+            if iso_txt.lower() == 'none':
+                iso_txt = None
+
+            # need to filter out the unchecked boxes and not plot that data
+            if len(args) > 0:
+                print(isinstance(args[0], dict))
+                print(args[0])
+
+            prop.oper_data.plot(x_param=xax_txt, y_param=yax_txt, family_param=fam_txt, iso_param=iso_txt,
+                                fig=self.plot_canvas.figure)
+
+        self.plot_canvas.draw()
+
+
+class PropellerSweepWorker(QtCore.QObject):
+
+    progress = QtCore.pyqtSignal(object, object)
+    finished = QtCore.pyqtSignal()
+
+    def __init__(self, prop: Propeller, velos: list, param2sweep: str, sweep_vals: list, vorform: str):
+        super(PropellerSweepWorker, self).__init__()
+        self.prop = prop
+        self.velos = velos
+        self.param2sweep = param2sweep
+        self.sweep_vals = sweep_vals
+        self.vorform = vorform
+
+    def run(self):
+        self.prop.analyze_sweep(velo_vals=self.velos, sweep_param=self.param2sweep, sweep_vals=self.sweep_vals,
+                                verbose=True, xrotor_verbose=False, vorform=self.vorform, prog_signal=self.progress)
+        self.finished.emit()
```

### Comparing `propeller_design_tools-0.3.5/propdes/prop_creation_ui_classes.py` & `propeller_design_tools-0.4.0/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,790 +1,790 @@
-import subprocess
-import numpy as np
-import os
-from propdes.propeller import Propeller
-from propdes.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
-from propdes.user_io import Error
-from propdes.settings import get_prop_db
-
-try:
-    from PyQt5 import QtWidgets, QtCore
-    from propdes.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
-        PropellerCreationPanelCanvas, RadialStationFitParamsCanvas
-    from propdes.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
-        PDT_PushButton, PDT_LineEdit, PDT_CheckBox
-    import pyqtgraph.opengl as gl
-except:
-    pass
-
-
-class PropellerCreationWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        self.prop = None
-        self.main_win = main_win
-
-        super(PropellerCreationWidget, self).__init__()
-
-        main_lay = QtWidgets.QHBoxLayout()
-        self.setLayout(main_lay)
-        self.control_widg = PropellerCreationControlWidget(main_win=main_win)
-        main_lay.addWidget(self.control_widg)
-
-        self.plot3d_widg = Propeller3dPlotWidget(main_win=main_win)
-        self.plot3d_widg.enable_edit_chk.clicked.connect(self.enable_edit_clicked)
-        main_lay.addWidget(self.plot3d_widg)
-
-        # connecting signals
-        self.plot3d_widg.select_prop_cb.currentTextChanged.connect(self.select_prop_cb_changed)
-
-    def enable_edit_clicked(self):
-        if self.plot3d_widg.select_prop_cb.currentText().lower() == 'none':
-            return
-
-        if self.plot3d_widg.enable_edit_chk.isChecked():
-            self.control_widg.set_enable(True)
-        else:
-            self.control_widg.set_enable(False)
-
-    def select_prop_cb_changed(self):
-        self.plot3d_widg.enable_edit_chk.setChecked(False)
-        self.plot3d_widg.clear_plot()
-        curr_txt = self.plot3d_widg.select_prop_cb.currentText()
-        if curr_txt == 'None':
-            self.prop = None
-            self.plot3d_widg.enable_edit_chk.setEnabled(False)
-            self.control_widg.set_inputs_to_default()
-            self.control_widg.set_enable(True)
-            self.control_widg.save_stl_btn.setEnabled(False)
-            self.control_widg.show_stl_btn.setEnabled(False)
-            self.control_widg.show_blade_profs_btn.setEnabled(False)
-        else:
-            with Capturing() as output:
-                self.prop = Propeller(name=curr_txt)
-            self.plot3d_widg.enable_edit_chk.setEnabled(True)
-            self.control_widg.pop_inputs_from_prop()
-            self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
-            self.plot3d_widg.update_plot(self.prop)
-            self.main_win.print('XROTOR OUTPUT:')
-            self.main_win.print(self.prop.get_xrotor_output_text(), fontfamily='consolas')
-            self.control_widg.set_enable(False)
-            self.control_widg.save_stl_btn.setEnabled(True)
-            self.control_widg.show_stl_btn.setEnabled(True)
-            self.control_widg.show_blade_profs_btn.setEnabled(True)
-
-
-class PropellerCreationControlWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        super(PropellerCreationControlWidget, self).__init__()
-        self.main_win = main_win
-        self.widgets_to_toggle = []
-        self.stl_view = None
-
-        main_lay = QtWidgets.QHBoxLayout()
-        self.setLayout(main_lay)
-
-        form_lay2a = QtWidgets.QFormLayout()
-        form_lay2c = QtWidgets.QFormLayout()
-
-        main_lay.addStretch()
-        left_vlayout = QtWidgets.QVBoxLayout()
-        left_vlayout.addStretch()
-        left_vlayout.addLayout(form_lay2a)
-        left_vlayout.addStretch()
-        main_lay.addLayout(left_vlayout)
-        main_lay.addStretch()
-        center_vlayout = QtWidgets.QVBoxLayout()
-        center_vlayout.addStretch()
-        center_vlayout.addLayout(form_lay2c)
-        center_vlayout.addStretch()
-        main_lay.addLayout(center_vlayout)
-        main_lay.addStretch()
-
-        # standard formlayout inputs, left form
-        form_lay2a.addRow(PDT_Label('Design Point\nXROTOR Inputs', font_size=14, bold=True))
-        self.name_le = PDT_LineEdit(font_size=12, width=220)
-        form_lay2a.addRow(PDT_Label('Name:', font_size=12), self.name_le)
-        self.nblades_sb = PDT_SpinBox(font_size=12, width=80)
-        self.nblades_sb.setMinimum(1)
-        self.nblades_sb.setMaximum(9)
-        form_lay2a.addRow(PDT_Label('nblades:', font_size=12), self.nblades_sb)
-        self.radius_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.radius_sb.setSingleStep(0.01)
-        form_lay2a.addRow(PDT_Label('Radius:', font_size=12), self.radius_sb)
-        self.hub_radius_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.hub_radius_sb.setSingleStep(0.01)
-        form_lay2a.addRow(PDT_Label('Hub Radius:', font_size=12), self.hub_radius_sb)
-        self.hub_wake_disp_br_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.hub_wake_disp_br_sb.setSingleStep(0.01)
-        form_lay2a.addRow(PDT_Label('Hub Wake\nDisplacement\nBody Radius:', font_size=12), self.hub_wake_disp_br_sb)
-        form_lay2a.setAlignment(self.hub_wake_disp_br_sb, QtCore.Qt.AlignBottom)
-        self.vorform_cb = PDT_ComboBox(font_size=12, width=100)
-        self.vorform_cb.addItems(['grad', 'pot', 'vrtx'])
-        form_lay2a.addRow(PDT_Label('Vortex\nFormulation:', font_size=12), self.vorform_cb)
-        form_lay2a.setAlignment(self.vorform_cb, QtCore.Qt.AlignBottom)
-        self.nradial_sb = PDT_SpinBox(font_size=12, width=80)
-        self.nradial_sb.setMinimum(20)
-        self.radius_sb.setMaximum(250)
-        form_lay2a.addRow(PDT_Label('# Radial Vortex Stations: ', font_size=12), self.nradial_sb)
-        self.design_speed_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        form_lay2a.addRow(PDT_Label('Speed:', font_size=12), self.design_speed_sb)
-        form_lay2a.addRow(PDT_Label(''))
-        self.design_adv_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.design_adv_sb.setSingleStep(0.01)
-        self.design_adv_sb.setSpecialValueText('None')
-        self.design_adv_sb.valueChanged.connect(self.des_adv_sb_changed)
-        form_lay2a.addRow(PDT_Label('Adv:', font_size=12), self.design_adv_sb)
-        form_lay2a.addRow(PDT_Label('- or -', font_size=10, italic=True))
-        self.design_rpm_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.design_rpm_sb.setSingleStep(100)
-        self.design_rpm_sb.setMaximum(np.inf)
-        self.design_rpm_sb.setSpecialValueText('None')
-        self.design_rpm_sb.valueChanged.connect(self.des_rpm_sb_changed)
-        form_lay2a.addRow(PDT_Label('RPM:', font_size=12), self.design_rpm_sb)
-        form_lay2a.addRow(PDT_Label(''))
-
-        self.design_thrust_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.design_thrust_sb.setMaximum(np.inf)
-        self.design_thrust_sb.setSpecialValueText('None')
-        self.design_thrust_sb.valueChanged.connect(self.des_thrust_sb_changed)
-        form_lay2a.addRow(PDT_Label('Thrust:', font_size=12), self.design_thrust_sb)
-        form_lay2a.addRow(PDT_Label('- or -', font_size=10, italic=True))
-        self.design_power_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.design_power_sb.setSpecialValueText('None')
-        self.design_power_sb.setMaximum(np.inf)
-        self.design_power_sb.valueChanged.connect(self.des_power_sb_changed)
-        form_lay2a.addRow(PDT_Label('Power:', font_size=12), self.design_power_sb)
-
-        # center / right form layout
-        self.design_cl_le = PDT_LineEdit(font_size=12, width=80)
-        form_lay2c.addRow(PDT_Label('C_l (const or root, tip):', font_size=12), self.design_cl_le)
-
-        # atmo props, vorform, station params
-        self.atmo_props_widg = AtmoPropsInputWidget()
-        form_lay2c.addRow(PDT_Label('Atmosphere\nProperties->', font_size=12), self.atmo_props_widg)
-        self.station_params_widg = StationParamsWidget()
-        form_lay2c.addRow(PDT_Label('Control\nStations->', font_size=12), self.station_params_widg)
-
-        # extra geo params
-        form_lay2c.addRow(PDT_Label('Extra Geometry Output Parameters', font_size=14, bold=True))
-        self.skew_sb = PDT_DoubleSpinBox(font_size=12, width=80)
-        self.skew_sb.setMaximum(70)
-        form_lay2c.addRow(PDT_Label('Skew:', font_size=12), self.skew_sb)
-        self.n_prof_pts_sb = PDT_SpinBox(font_size=12, width=80)
-        self.n_prof_pts_sb.setSpecialValueText('None')
-        form_lay2c.addRow(PDT_Label('# Profile Pts:', font_size=12), self.n_prof_pts_sb)
-        self.n_profs_sb = PDT_SpinBox(font_size=12, width=80, box_range=[0, 500])
-        form_lay2c.addRow(PDT_Label('# Radial Profiles:', font_size=12), self.n_profs_sb)
-
-        # create and reset buttons
-        self.create_btn = PDT_PushButton('Create!', width=150, height=40, font_size=14, bold=True)
-        self.create_btn.clicked.connect(self.create_btn_clicked)
-        self.reset_btn = PDT_PushButton('Reset', width=150, height=40, font_size=14, bold=True)
-        self.reset_btn.clicked.connect(self.set_inputs_to_default)
-        self.save_new_btn = PDT_PushButton('Save as New', width=150, height=40, font_size=14, bold=True)
-        self.save_new_btn.clicked.connect(self.save_new_btn_clicked)
-        self.save_new_btn.setEnabled(False)
-        temp_lay = QtWidgets.QHBoxLayout()
-        temp_lay.addWidget(self.create_btn)
-        temp_lay.addWidget(self.reset_btn)
-        temp_lay.addWidget(self.save_new_btn)
-        form_lay2c.addRow(temp_lay)
-
-        # Other geo buttons
-        self.save_stl_btn = save_stl_btn = PDT_PushButton('Generate STL\nGeom. File', width=160, height=50, font_size=12)
-        self.show_stl_btn = show_stl_btn = PDT_PushButton('Show STL\nGeom. File', width=140, height=50, font_size=12)
-        self.show_blade_profs_btn = show_blade_profs_btn = PDT_PushButton('Show Blade xyz\nProfiles in Explorer', width=200,
-                                                                          height=50, font_size=12)
-        save_stl_btn.setEnabled(False)
-        show_stl_btn.setEnabled(False)
-        show_blade_profs_btn.setEnabled(False)
-        save_stl_btn.clicked.connect(self.save_stl_btn_clicked)
-        show_stl_btn.clicked.connect(self.show_stl_btn_clicked)
-        show_blade_profs_btn.clicked.connect(self.show_blade_profs_btn_clicked)
-        temp_lay2 = QtWidgets.QHBoxLayout()
-        temp_lay2.addWidget(save_stl_btn)
-        temp_lay2.addWidget(show_stl_btn)
-        temp_lay2.addWidget(show_blade_profs_btn)
-        form_lay2c.addRow(temp_lay2)
-
-        # store a list of widgets to toggle enable on
-        self.widgets_to_toggle = [self.name_le, self.nblades_sb, self.radius_sb, self.hub_radius_sb,
-                                  self.hub_wake_disp_br_sb, self.vorform_cb, self.nradial_sb, self.design_speed_sb,
-                                  self.design_adv_sb, self.design_rpm_sb, self.design_thrust_sb, self.design_power_sb,
-                                  self.design_cl_le, self.atmo_props_widg.altitude_sb, self.atmo_props_widg.rho_sb,
-                                  self.atmo_props_widg.nu_sb, self.atmo_props_widg.vsou_sb, self.station_params_widg,
-                                  self.skew_sb, self.n_prof_pts_sb, self.n_profs_sb, self.create_btn, self.reset_btn,
-                                  self.save_new_btn]
-
-        # set all the inputs to default
-        self.set_inputs_to_default()
-
-    def show_stl_btn_clicked(self):
-        prop = self.main_win.prop_widg.prop
-        if prop is None:
-            return
-
-        if os.path.exists(prop.stl_fpath):
-            self.stl_view = prop.plot_stl_mesh()
-
-    def save_stl_btn_clicked(self):
-        prop = self.main_win.prop_widg.prop
-        if prop is None:
-            return
-
-        with Capturing() as output:
-            prop.generate_stl_geometry(plot_after=False)
-        self.main_win.print(output)
-
-    def show_blade_profs_btn_clicked(self):
-        prop = self.main_win.prop_widg.prop
-        if prop is None:
-            return
-
-        if os.path.exists(prop.bld_prof_folder):
-            subprocess.Popen('explorer "{}"'.format(os.path.normpath(prop.bld_prof_folder)))
-
-    def save_new_btn_clicked(self):
-        savedir, _ = QtWidgets.QFileDialog.getSaveFileName(self, 'Enter New Save Name', self.main_win.prop_db_select_widg.db_dir)
-        if savedir:
-            savename = os.path.split(savedir)[1]
-            savedir = os.path.join(get_prop_db(), savename)
-
-            if not os.path.exists(savedir):
-                os.mkdir(savedir)
-
-            self.main_win.prop_widg.prop.save_as_new(new_name=savename)
-
-    def set_enable(self, enable: bool):
-        for widg in self.widgets_to_toggle:
-            if widg is not self.save_new_btn:
-                widg.setEnabled(enable)
-            else:
-                widg.setEnabled(not enable)
-
-    def des_thrust_sb_changed(self):
-        if self.design_thrust_sb.value() == self.design_thrust_sb.minimum():
-            self.design_power_sb.setEnabled(True)
-        else:
-            self.design_power_sb.setEnabled(False)
-
-    def des_power_sb_changed(self):
-        if self.design_power_sb.value() == self.design_power_sb.minimum():
-            self.design_thrust_sb.setEnabled(True)
-        else:
-            self.design_thrust_sb.setEnabled(False)
-
-    def des_adv_sb_changed(self):
-        self.design_rpm_sb.setEnabled(self.design_adv_sb.value() == self.design_adv_sb.minimum())
-
-    def des_rpm_sb_changed(self):
-        self.design_adv_sb.setEnabled(self.design_rpm_sb.value() == self.design_rpm_sb.minimum())
-
-    def set_inputs_to_default(self):
-        self.name_le.setText('[enter a name]')
-        self.nblades_sb.setValue(3)
-        self.radius_sb.setValue(1.0)
-        self.hub_radius_sb.setValue(0.08)
-        self.hub_wake_disp_br_sb.setValue(0.08)
-        self.vorform_cb.setCurrentText('pot')
-        self.nradial_sb.setValue(50)
-
-        self.design_speed_sb.setValue(30)
-        self.design_adv_sb.setValue(0)
-        self.design_rpm_sb.setValue(0)
-        self.design_thrust_sb.setValue(0)
-        self.design_power_sb.setValue(0)
-
-        self.design_cl_le.setText('0.2, 0.2')
-        self.atmo_props_widg.altitude_sb.setValue(self.atmo_props_widg.altitude_sb.minimum())
-        self.atmo_props_widg.rho_sb.setValue(self.atmo_props_widg.rho_sb.minimum())
-        self.atmo_props_widg.nu_sb.setValue(self.atmo_props_widg.nu_sb.minimum())
-        self.atmo_props_widg.vsou_sb.setValue(self.atmo_props_widg.vsou_sb.minimum())
-
-        self.station_params_widg.reset_to_default()
-        self.skew_sb.setValue(self.skew_sb.minimum())
-        self.n_prof_pts_sb.setValue(self.n_prof_pts_sb.minimum())
-        self.n_profs_sb.setValue(50)
-
-    def pop_inputs_from_prop(self):
-        prop = self.main_win.prop_widg.prop
-        self.name_le.setText(prop.name)
-        self.nblades_sb.setValue(prop.nblades)
-        self.radius_sb.setValue(prop.radius)
-        self.hub_radius_sb.setValue(prop.hub_radius)
-        self.hub_wake_disp_br_sb.setValue(prop.hub_wake_disp_br)
-        self.vorform_cb.setCurrentText(prop.design_vorform)
-        self.nradial_sb.setValue(prop.n_radial)
-
-        self.design_speed_sb.setValue(prop.design_speed_mps)
-
-        if prop.design_rpm is not None:
-            self.design_rpm_sb.setValue(prop.design_rpm)
-        else:
-            self.design_rpm_sb.setValue(0)
-
-        if prop.design_adv is not None:
-            self.design_adv_sb.setValue(prop.design_adv)
-        else:
-            self.design_adv_sb.setValue(0)
-
-        if prop.design_thrust is not None:
-            self.design_thrust_sb.setValue(prop.design_thrust)
-        else:
-            self.design_thrust_sb.setValue(0)
-
-        if prop.design_power is not None:
-            self.design_power_sb.setValue(prop.design_power)
-        else:
-            self.design_power_sb.setValue(0)
-
-        if len(prop.design_cl) == 1 and 'const' in prop.design_cl:
-            self.design_cl_le.setText('{}'.format(prop.design_cl['const']))
-        elif len(prop.design_cl) == 1 and 'file' in prop.design_cl:
-            pass
-        else:
-            assert 'root' in prop.design_cl
-            assert 'tip' in prop.design_cl
-            self.design_cl_le.setText('{}, {}'.format(prop.design_cl['root'], prop.design_cl['tip']))
-
-        if 'altitude_km' in prop.design_atmo_props:
-            self.atmo_props_widg.altitude_sb.setValue(prop.design_atmo_props['altitude_km'])
-        else:
-            self.atmo_props_widg.altitude_sb.setValue(0)
-
-        if 'dens' in prop.design_atmo_props:
-            self.atmo_props_widg.rho_sb.setValue(prop.design_atmo_props['dens'])
-        else:
-            self.atmo_props_widg.rho_sb.setValue(0)
-
-        if 'visc' in prop.design_atmo_props:
-            self.atmo_props_widg.nu_sb.setValue(prop.design_atmo_props['visc'])
-        else:
-            self.atmo_props_widg.nu_sb.setValue(0)
-
-        if 'vsou' in prop.design_atmo_props:
-            self.atmo_props_widg.vsou_sb.setValue(prop.design_atmo_props['vsou'])
-        else:
-            self.atmo_props_widg.vsou_sb.setValue(0)
-
-        self.station_params_widg.reset_to_default()
-        for st_loc, foil_name in prop.station_params.items():
-            if not foil_name.endswith('.dat'):
-                foil_name = '{}.dat'.format(foil_name)
-            foil_cb, roR_sb = self.station_params_widg.add_row()
-            foil_cb.setCurrentText(foil_name)
-            roR_sb.setValue(st_loc)
-
-        self.skew_sb.setValue(prop.tot_skew)
-        if prop.n_prof_pts is None:
-            self.n_prof_pts_sb.setValue(self.n_prof_pts_sb.minimum())
-        else:
-            self.n_prof_pts_sb.setValue(prop.n_prof_pts)
-        self.n_profs_sb.setValue(prop.n_profs)
-
-    def create_btn_clicked(self):
-        msgbox = QtWidgets.QMessageBox()
-
-        name = self.name_le.text()
-        if len(name.strip()) == 0:
-            msgbox.about(self, 'Error', 'Invalid Name')
-            return
-
-        nblades = self.nblades_sb.value()
-        radius = self.radius_sb.value()
-        hub_radius = self.hub_radius_sb.value()
-        hub_wk_disp_br = self.hub_wake_disp_br_sb.value()
-        speed = self.design_speed_sb.value()
-        adv = self.design_adv_sb.value() if self.design_adv_sb.value() != self.design_adv_sb.minimum() else None
-        rpm = self.design_rpm_sb.value() if self.design_rpm_sb.value() != self.design_rpm_sb.minimum() else None
-        if adv == self.design_adv_sb.minimum() and rpm == self.design_rpm_sb.minimum():
-            msgbox.about(self, 'Error', 'Must give one of "adv" or "rpm"')
-            return
-
-        thrust = self.design_thrust_sb.value() if self.design_thrust_sb.value() != self.design_thrust_sb.minimum() else None
-        power = self.design_power_sb.value() if self.design_power_sb.value() != self.design_power_sb.minimum() else None
-        if thrust is None and power is None:
-            msgbox.about(self, 'Error', 'Must give one of "thrust" or "power"')
-            return
-
-        nradial = self.nradial_sb.value()
-        cl_txt = self.design_cl_le.text().strip()
-        if len(cl_txt.split(',')) == 1:
-            cl_dict = {'const': float(cl_txt)}
-        elif len(cl_txt.split(',')) == 2:
-            cl_dict = {'root': float(cl_txt.split(',')[0].strip()), 'tip': float(cl_txt.split(',')[1].strip())}
-        else:
-            msgbox = QtWidgets.QMessageBox()
-            msgbox.about(self, 'Error', 'Only "const" and "linear" CL currently supported')
-            return
-
-        altitude = self.atmo_props_widg.altitude_sb.value()
-        alt_ismin = altitude == self.atmo_props_widg.altitude_sb.minimum()
-        rho = self.atmo_props_widg.rho_sb.value()
-        rho_ismin = rho == self.atmo_props_widg.rho_sb.minimum()
-        nu = self.atmo_props_widg.nu_sb.value()
-        nu_ismin = nu == self.atmo_props_widg.nu_sb.minimum()
-        vsou = self.atmo_props_widg.vsou_sb.value()
-        vsou_ismin = vsou == self.atmo_props_widg.vsou_sb.minimum()
-        if alt_ismin and any([rho_ismin, nu_ismin, vsou_ismin]):
-            msgbox.about(self, 'Error', 'Can only / must give "altitude" or all three "rho", "nu" and "vsou"')
-            return
-
-        vorform = self.vorform_cb.currentText()
-        stations_dict = self.station_params_widg.get_stations_dict()
-        if stations_dict is None:
-            msgbox.about(self, 'Error', 'Must give at least 1 station')
-            return
-
-        skew = self.skew_sb.value()
-        n_prof_pts = self.n_prof_pts_sb.value() if self.n_prof_pts_sb.value() != self.n_prof_pts_sb.minimum() else None
-        n_profs = self.n_profs_sb.value()
-
-        if altitude is not None:
-            atmo_props = {'altitude_km': altitude}
-        else:
-            atmo_props = {'rho': rho, 'nu': nu, 'vsou': vsou}
-
-        self.timer = QtCore.QTimer()
-        self.timer.timeout.connect(self.update_create_worker_progress)
-        self.timer.start(1000)
-        self.timer_cntr = 0
-
-        self.thread = QtCore.QThread()
-        self.prop_create_worker = CreatePropellerWorker(name=name,
-                                                        nblades=nblades,
-                                                        radius=radius,
-                                                        hub_radius=hub_radius,
-                                                        hub_wake_disp_br=hub_wk_disp_br,
-                                                        design_speed_mps=speed,
-                                                        design_cl=cl_dict,
-                                                        design_atmo_props=atmo_props,
-                                                        design_vorform=vorform,
-                                                        station_params=stations_dict,
-                                                        design_adv=adv,
-                                                        design_rpm=rpm,
-                                                        design_thrust=thrust,
-                                                        design_power=power,
-                                                        n_radial=nradial,
-                                                        skew=skew,
-                                                        n_prof_pts=n_prof_pts,
-                                                        n_profs=n_profs)
-        self.prop_create_worker.moveToThread(self.thread)
-        self.thread.started.connect(self.prop_create_worker.run)
-        self.prop_create_worker.finished.connect(self.thread.quit)
-        self.prop_create_worker.finished.connect(self.prop_create_worker.deleteLater)
-        self.prop_create_worker.finished.connect(self.on_create_worker_finish)
-        self.thread.finished.connect(self.thread.deleteLater)
-        self.prop_create_worker.progress.connect(self.update_create_worker_progress)
-
-        self.main_win.prop_widg.setEnabled(False)
-        self.thread.start()
-
-    def on_create_worker_finish(self, prop, output):
-        self.timer.stop()
-        self.main_win.prog_bar.setValue(0)
-        self.main_win.print(output)
-        if prop:
-            self.main_win.prop_db_select_widg.update_found_lbl()
-            self.main_win.prop_widg.plot3d_widg.populate_select_prop_cb()
-            self.main_win.prop_widg.plot3d_widg.select_prop_cb.setCurrentText(prop.name)
-            self.main_win.prop_widg.setEnabled(True)
-
-    def update_create_worker_progress(self):
-        val = 2 if self.vorform_cb.currentText() == 'vrtx' else 33
-        self.timer_cntr += val
-        prog_val = self.timer_cntr if self.timer_cntr < 100 else 99
-        self.main_win.prog_bar.setValue(prog_val)
-
-
-class Propeller3dPlotWidget(QtWidgets.QWidget):
-    def __init__(self, main_win: 'InterfaceMainWindow'):
-        self.main_win = main_win
-        super(Propeller3dPlotWidget, self).__init__()
-        main_lay = QtWidgets.QVBoxLayout()
-        self.setLayout(main_lay)
-
-        form_lay = QtWidgets.QFormLayout()
-        hlay = QtWidgets.QHBoxLayout()
-        hlay.addLayout(form_lay)
-        self.select_prop_cb = PDT_ComboBox(width=150)
-        form_lay.addRow(PDT_Label('Select Propeller:', font_size=14, bold=True), self.select_prop_cb)
-        self.enable_edit_chk = PDT_CheckBox('Enable Editing of Design Point', italic=True, font_size=10)
-        # self.enable_edit_chk.clicked.connect(self.enable_edit_chk_clicked)
-        form_lay.addRow(self.enable_edit_chk)
-        self.show_rstation_btn = PDT_PushButton('Show Radial\nStation Params', font_size=14, width=160, bold=True)
-        self.show_rstation_btn.clicked.connect(self.show_rstation_btn_clicked)
-        hlay.addWidget(self.show_rstation_btn)
-        self.show_panel_btn = PDT_PushButton('Show Design\nPoint Panel', font_size=14, width=160, bold=True)
-        self.show_panel_btn.clicked.connect(self.show_panel_btn_clicked)
-        hlay.addWidget(self.show_panel_btn)
-        main_lay.addLayout(hlay)
-        self.populate_select_prop_cb()
-
-        self.plot_canvas = SingleAxCanvas(self, width=6, height=6, projection='3d')
-        self.axes3d = self.plot_canvas.axes
-        main_lay.addWidget(self.plot_canvas)
-
-    # def enable_edit_chk_clicked(self):
-    #     pass
-
-    def show_rstation_btn_clicked(self):
-        prop = self.main_win.prop_widg.prop
-        if prop is not None:
-            self.station_widgs = []
-            for st in prop.stations:
-                st_widg = QtWidgets.QWidget()
-                self.station_widgs.append(st_widg)
-                lay = QtWidgets.QVBoxLayout()
-                st_widg.setLayout(lay)
-
-                fit_canvas = RadialStationFitParamsCanvas()
-                lay.addWidget(fit_canvas)
-                st.plot_xrotor_fit_params(fig=fit_canvas.figure)
-
-                st_widg.show()
-                fit_canvas.draw()
-        return
-
-    def show_panel_btn_clicked(self):
-        prop = self.main_win.prop_widg.prop
-        if prop is not None:
-            self.creation_panel_widg = QtWidgets.QWidget()
-            lay = QtWidgets.QVBoxLayout()
-            self.creation_panel_widg.setLayout(lay)
-
-            self.creation_panel_canvas = PropellerCreationPanelCanvas()
-            lay.addWidget(self.creation_panel_canvas)
-            prop.plot_design_point_panel(fig=self.creation_panel_canvas.figure)
-
-            self.creation_panel_widg.show()
-            self.creation_panel_canvas.draw()
-
-    def update_plot(self, prop: Propeller):
-        with Capturing() as output:
-            prop.plot_mpl3d_geometry(interp_profiles=True, hub=True, input_stations=True, chords_betas=True, LE=True,
-                                     TE=True, fig=self.plot_canvas.figure)
-        self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
-        self.plot_canvas.draw()
-
-    def clear_plot(self):
-        self.axes3d.clear()
-        self.plot_canvas.draw()
-
-    def populate_select_prop_cb(self):
-        self.select_prop_cb.blockSignals(True)
-        self.select_prop_cb.clear()
-        self.select_prop_cb.blockSignals(False)
-        self.select_prop_cb.addItems(['None'] + get_all_propeller_dirs())
-
-
-class StationParamsWidget(QtWidgets.QWidget):
-    def __init__(self):
-        super(StationParamsWidget, self).__init__()
-
-        main_lay = QtWidgets.QVBoxLayout()
-        self.rows_lay = QtWidgets.QFormLayout()
-        self.setLayout(main_lay)
-        main_lay.addLayout(self.rows_lay)
-
-        self.header_row_strs = ['#', 'Foil', 'r/R']
-        self.add_header_row()
-        self.add_btn = PDT_PushButton('(+) add', width=80, font_size=11)
-        self.remove_btn = PDT_PushButton('(-) remove', width=100, font_size=11)
-
-        btn_lay = QtWidgets.QHBoxLayout()
-        btn_lay.addWidget(self.add_btn)
-        btn_lay.addWidget(self.remove_btn)
-        main_lay.addLayout(btn_lay)
-
-        # connect signals
-        self.add_btn.clicked.connect(self.add_row)
-        self.remove_btn.clicked.connect(self.remove_row)
-
-    def reset_to_default(self):
-        count = self.rows_lay.rowCount()
-        while count > 1:
-            self.rows_lay.removeRow(count - 1)
-            count -= 1
-
-    def add_header_row(self):
-        num_lbl = PDT_Label(self.header_row_strs[0], font_size=11)
-        foil_lbl = PDT_Label(self.header_row_strs[1], font_size=11)
-        roR_lbl = PDT_Label(self.header_row_strs[2], font_size=11)
-        rt_lay = QtWidgets.QHBoxLayout()
-        rt_lay.addWidget(foil_lbl)
-        rt_lay.addWidget(roR_lbl)
-        rt_widg = QtWidgets.QWidget()
-        rt_widg.setLayout(rt_lay)
-        self.rows_lay.addRow(num_lbl, rt_widg)
-
-    def add_row(self):
-        rt_lay = QtWidgets.QHBoxLayout()
-        rt_widg = QtWidgets.QWidget()
-        rt_widg.setLayout(rt_lay)
-        if self.rows_lay.rowCount() > 1:
-            msgbox = QtWidgets.QMessageBox()
-            msgbox.about(self, 'Error', '> 1 station not yet implemented in PDT')
-            return
-        num_lbl = PDT_Label('{}'.format(self.rows_lay.rowCount()), font_size=11)
-        foil_cb = PDT_ComboBox(font_size=11, width=140)
-        foil_cb.addItems(get_all_airfoil_files())
-        roR_sb = PDT_DoubleSpinBox(font_size=11)
-        roR_sb.setMaximum(1.0)
-        roR_sb.setSingleStep(0.01)
-        roR_sb.setValue(0.75)
-        rt_lay.addWidget(foil_cb)
-        rt_lay.addWidget(roR_sb)
-        self.rows_lay.addRow(num_lbl, rt_widg)
-        return foil_cb, roR_sb
-
-    def remove_row(self):
-        row = self.rows_lay.rowCount() - 1
-        self.rows_lay.removeRow(row)
-
-    def get_stations_dict(self):
-        if self.rows_lay.rowCount() == 1:
-            return None
-        else:
-            stations = {}
-            for row in range(1, self.rows_lay.rowCount()):
-                rt_widg = self.rows_lay.itemAt(row, 1).widget()
-                itm1, itm2 = [rt_widg.layout().itemAt(i) for i in range(rt_widg.layout().count())]
-                foil_cb = itm1.widget()
-                roR_sb = itm2.widget()
-                stations[roR_sb.value()] = foil_cb.currentText()
-        return stations
-
-
-class AtmoPropsInputWidget(QtWidgets.QWidget):
-    def __init__(self):
-        super(AtmoPropsInputWidget, self).__init__()
-        lay = QtWidgets.QHBoxLayout()
-        self.setLayout(lay)
-        left_lay = QtWidgets.QVBoxLayout()
-        left_center_lay = QtWidgets.QFormLayout()
-        left_lay.addStretch()
-        left_lay.addLayout(left_center_lay)
-        left_lay.addStretch()
-        right_lay = QtWidgets.QFormLayout()
-        lay.addLayout(left_lay)
-        lay.addWidget(PDT_Label('or'))
-        lay.addLayout(right_lay)
-        lay.addStretch()
-
-        self.altitude_sb = PDT_DoubleSpinBox(width=80, font_size=12)
-        self.altitude_sb.setMinimum(-2)
-        self.altitude_sb.setSpecialValueText('None')
-        left_center_lay.addRow(PDT_Label('Altitude:', font_size=12), self.altitude_sb)
-
-        self.rho_sb = PDT_DoubleSpinBox(width=80, font_size=12)
-        self.rho_sb.setSpecialValueText('None')
-        right_lay.addRow(PDT_Label('Rho:', font_size=12), self.rho_sb)
-        self.nu_sb = PDT_DoubleSpinBox(width=80, font_size=12)
-        self.nu_sb.setSpecialValueText('None')
-        right_lay.addRow(PDT_Label('Nu:', font_size=12), self.nu_sb)
-        self.vsou_sb = PDT_DoubleSpinBox(width=80, font_size=12)
-        self.vsou_sb.setSpecialValueText('None')
-        right_lay.addRow(PDT_Label('Vsou:', font_size=12), self.vsou_sb)
-
-        # connect some signals
-        self.altitude_sb.valueChanged.connect(self.altitude_sb_changed)
-        self.rho_sb.valueChanged.connect(self.rho_sb_changed)
-        self.nu_sb.valueChanged.connect(self.nu_sb_changed)
-        self.vsou_sb.valueChanged.connect(self.vsou_sb_changed)
-
-    def vsou_sb_changed(self):
-        if self.rho_sb.value() == self.rho_sb.minimum() \
-                and self.nu_sb.value() == self.nu_sb.minimum() \
-                and self.vsou_sb.value() == self.vsou_sb.minimum():
-            self.altitude_sb.setEnabled(True)
-        else:
-            self.altitude_sb.setEnabled(False)
-
-    def nu_sb_changed(self):
-        if self.rho_sb.value() == self.rho_sb.minimum() \
-                and self.nu_sb.value() == self.nu_sb.minimum() \
-                and self.vsou_sb.value() == self.vsou_sb.minimum():
-            self.altitude_sb.setEnabled(True)
-        else:
-            self.altitude_sb.setEnabled(False)
-
-    def rho_sb_changed(self):
-        if self.rho_sb.value() == self.rho_sb.minimum() \
-                and self.nu_sb.value() == self.nu_sb.minimum() \
-                and self.vsou_sb.value() == self.vsou_sb.minimum():
-            self.altitude_sb.setEnabled(True)
-        else:
-            self.altitude_sb.setEnabled(False)
-
-    def altitude_sb_changed(self):
-        if self.altitude_sb.value() == self.altitude_sb.minimum():
-            self.rho_sb.setEnabled(True)
-            self.nu_sb.setEnabled(True)
-            self.vsou_sb.setEnabled(True)
-        else:
-            self.rho_sb.setEnabled(False)
-            self.nu_sb.setEnabled(False)
-            self.vsou_sb.setEnabled(False)
-
-
-class CreatePropellerWorker(QtCore.QObject):
-    finished = QtCore.pyqtSignal(object, list)
-    progress = QtCore.pyqtSignal(int)
-
-    def __init__(self, name: str, nblades: int, radius: float, hub_radius: float, hub_wake_disp_br: float,
-                 design_speed_mps: float, design_cl: dict, design_atmo_props: dict, design_vorform: str,
-                 station_params: dict = None, design_adv: float = None, design_rpm: float = None,
-                 design_thrust: float = None, design_power: float = None, n_radial: int = 50, skew: float = 0.0,
-                 n_prof_pts: int = None, n_profs: int = 50):
-
-        super(CreatePropellerWorker, self).__init__()
-
-        self.name = name
-        self.nblades = nblades
-        self.radius = radius
-        self.hub_radius = hub_radius
-        self.hub_wake_disp_br = hub_wake_disp_br
-        self.design_speed_mps = design_speed_mps
-        self.design_cl = design_cl
-        self.design_atmo_props = design_atmo_props
-        self.design_vorform = design_vorform
-        self.station_params = station_params
-        self.design_adv = design_adv
-        self.design_rpm = design_rpm
-        self.design_thrust = design_thrust
-        self.design_power = design_power
-        self.n_radial = n_radial
-        self.skew = skew
-        self.n_prof_pts = n_prof_pts
-        self.n_profs = n_profs
-
-    def run(self):
-        try:
-            with Capturing() as output:
-                prop = create_propeller(name=self.name,
-                                        nblades=self.nblades,
-                                        radius=self.radius,
-                                        hub_radius=self.hub_radius,
-                                        hub_wake_disp_br=self.hub_wake_disp_br,
-                                        design_speed_mps=self.design_speed_mps,
-                                        design_cl=self.design_cl,
-                                        design_atmo_props=self.design_atmo_props,
-                                        design_vorform=self.design_vorform,
-                                        station_params=self.station_params,
-                                        design_adv=self.design_adv,
-                                        design_rpm=self.design_rpm,
-                                        design_thrust=self.design_thrust,
-                                        design_power=self.design_power,
-                                        n_radial=self.n_radial,
-                                        verbose=True,
-                                        show_station_fit_plots=False,
-                                        plot_after=False,
-                                        tmout=None,
-                                        hide_windows=True,
-                                        geo_params={'tot_skew': self.skew, 'n_prof_pts': self.n_prof_pts,
-                                                    'n_profs': self.n_profs})
-        except Exception as e:
-            prop = None
-            output = [e.__repr__()]
-
-        self.finished.emit(prop, output)
+import subprocess
+import numpy as np
+import os
+from propeller_design_tools.propeller import Propeller
+from propeller_design_tools.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
+from propeller_design_tools.user_io import Error
+from propeller_design_tools.settings import get_prop_db
+
+try:
+    from PyQt5 import QtWidgets, QtCore
+    from propeller_design_tools.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
+        PropellerCreationPanelCanvas, RadialStationFitParamsCanvas
+    from propeller_design_tools.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
+        PDT_PushButton, PDT_LineEdit, PDT_CheckBox
+    import pyqtgraph.opengl as gl
+except:
+    pass
+
+
+class PropellerCreationWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        self.prop = None
+        self.main_win = main_win
+
+        super(PropellerCreationWidget, self).__init__()
+
+        main_lay = QtWidgets.QHBoxLayout()
+        self.setLayout(main_lay)
+        self.control_widg = PropellerCreationControlWidget(main_win=main_win)
+        main_lay.addWidget(self.control_widg)
+
+        self.plot3d_widg = Propeller3dPlotWidget(main_win=main_win)
+        self.plot3d_widg.enable_edit_chk.clicked.connect(self.enable_edit_clicked)
+        main_lay.addWidget(self.plot3d_widg)
+
+        # connecting signals
+        self.plot3d_widg.select_prop_cb.currentTextChanged.connect(self.select_prop_cb_changed)
+
+    def enable_edit_clicked(self):
+        if self.plot3d_widg.select_prop_cb.currentText().lower() == 'none':
+            return
+
+        if self.plot3d_widg.enable_edit_chk.isChecked():
+            self.control_widg.set_enable(True)
+        else:
+            self.control_widg.set_enable(False)
+
+    def select_prop_cb_changed(self):
+        self.plot3d_widg.enable_edit_chk.setChecked(False)
+        self.plot3d_widg.clear_plot()
+        curr_txt = self.plot3d_widg.select_prop_cb.currentText()
+        if curr_txt == 'None':
+            self.prop = None
+            self.plot3d_widg.enable_edit_chk.setEnabled(False)
+            self.control_widg.set_inputs_to_default()
+            self.control_widg.set_enable(True)
+            self.control_widg.save_stl_btn.setEnabled(False)
+            self.control_widg.show_stl_btn.setEnabled(False)
+            self.control_widg.show_blade_profs_btn.setEnabled(False)
+        else:
+            with Capturing() as output:
+                self.prop = Propeller(name=curr_txt)
+            self.plot3d_widg.enable_edit_chk.setEnabled(True)
+            self.control_widg.pop_inputs_from_prop()
+            self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
+            self.plot3d_widg.update_plot(self.prop)
+            self.main_win.print('XROTOR OUTPUT:')
+            self.main_win.print(self.prop.get_xrotor_output_text(), fontfamily='consolas')
+            self.control_widg.set_enable(False)
+            self.control_widg.save_stl_btn.setEnabled(True)
+            self.control_widg.show_stl_btn.setEnabled(True)
+            self.control_widg.show_blade_profs_btn.setEnabled(True)
+
+
+class PropellerCreationControlWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(PropellerCreationControlWidget, self).__init__()
+        self.main_win = main_win
+        self.widgets_to_toggle = []
+        self.stl_view = None
+
+        main_lay = QtWidgets.QHBoxLayout()
+        self.setLayout(main_lay)
+
+        form_lay2a = QtWidgets.QFormLayout()
+        form_lay2c = QtWidgets.QFormLayout()
+
+        main_lay.addStretch()
+        left_vlayout = QtWidgets.QVBoxLayout()
+        left_vlayout.addStretch()
+        left_vlayout.addLayout(form_lay2a)
+        left_vlayout.addStretch()
+        main_lay.addLayout(left_vlayout)
+        main_lay.addStretch()
+        center_vlayout = QtWidgets.QVBoxLayout()
+        center_vlayout.addStretch()
+        center_vlayout.addLayout(form_lay2c)
+        center_vlayout.addStretch()
+        main_lay.addLayout(center_vlayout)
+        main_lay.addStretch()
+
+        # standard formlayout inputs, left form
+        form_lay2a.addRow(PDT_Label('Design Point\nXROTOR Inputs', font_size=14, bold=True))
+        self.name_le = PDT_LineEdit(font_size=12, width=220)
+        form_lay2a.addRow(PDT_Label('Name:', font_size=12), self.name_le)
+        self.nblades_sb = PDT_SpinBox(font_size=12, width=80)
+        self.nblades_sb.setMinimum(1)
+        self.nblades_sb.setMaximum(9)
+        form_lay2a.addRow(PDT_Label('nblades:', font_size=12), self.nblades_sb)
+        self.radius_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.radius_sb.setSingleStep(0.01)
+        form_lay2a.addRow(PDT_Label('Radius:', font_size=12), self.radius_sb)
+        self.hub_radius_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.hub_radius_sb.setSingleStep(0.01)
+        form_lay2a.addRow(PDT_Label('Hub Radius:', font_size=12), self.hub_radius_sb)
+        self.hub_wake_disp_br_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.hub_wake_disp_br_sb.setSingleStep(0.01)
+        form_lay2a.addRow(PDT_Label('Hub Wake\nDisplacement\nBody Radius:', font_size=12), self.hub_wake_disp_br_sb)
+        form_lay2a.setAlignment(self.hub_wake_disp_br_sb, QtCore.Qt.AlignBottom)
+        self.vorform_cb = PDT_ComboBox(font_size=12, width=100)
+        self.vorform_cb.addItems(['grad', 'pot', 'vrtx'])
+        form_lay2a.addRow(PDT_Label('Vortex\nFormulation:', font_size=12), self.vorform_cb)
+        form_lay2a.setAlignment(self.vorform_cb, QtCore.Qt.AlignBottom)
+        self.nradial_sb = PDT_SpinBox(font_size=12, width=80)
+        self.nradial_sb.setMinimum(20)
+        self.radius_sb.setMaximum(250)
+        form_lay2a.addRow(PDT_Label('# Radial Vortex Stations: ', font_size=12), self.nradial_sb)
+        self.design_speed_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        form_lay2a.addRow(PDT_Label('Speed:', font_size=12), self.design_speed_sb)
+        form_lay2a.addRow(PDT_Label(''))
+        self.design_adv_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.design_adv_sb.setSingleStep(0.01)
+        self.design_adv_sb.setSpecialValueText('None')
+        self.design_adv_sb.valueChanged.connect(self.des_adv_sb_changed)
+        form_lay2a.addRow(PDT_Label('Adv:', font_size=12), self.design_adv_sb)
+        form_lay2a.addRow(PDT_Label('- or -', font_size=10, italic=True))
+        self.design_rpm_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.design_rpm_sb.setSingleStep(100)
+        self.design_rpm_sb.setMaximum(np.inf)
+        self.design_rpm_sb.setSpecialValueText('None')
+        self.design_rpm_sb.valueChanged.connect(self.des_rpm_sb_changed)
+        form_lay2a.addRow(PDT_Label('RPM:', font_size=12), self.design_rpm_sb)
+        form_lay2a.addRow(PDT_Label(''))
+
+        self.design_thrust_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.design_thrust_sb.setMaximum(np.inf)
+        self.design_thrust_sb.setSpecialValueText('None')
+        self.design_thrust_sb.valueChanged.connect(self.des_thrust_sb_changed)
+        form_lay2a.addRow(PDT_Label('Thrust:', font_size=12), self.design_thrust_sb)
+        form_lay2a.addRow(PDT_Label('- or -', font_size=10, italic=True))
+        self.design_power_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.design_power_sb.setSpecialValueText('None')
+        self.design_power_sb.setMaximum(np.inf)
+        self.design_power_sb.valueChanged.connect(self.des_power_sb_changed)
+        form_lay2a.addRow(PDT_Label('Power:', font_size=12), self.design_power_sb)
+
+        # center / right form layout
+        self.design_cl_le = PDT_LineEdit(font_size=12, width=80)
+        form_lay2c.addRow(PDT_Label('C_l (const or root, tip):', font_size=12), self.design_cl_le)
+
+        # atmo props, vorform, station params
+        self.atmo_props_widg = AtmoPropsInputWidget()
+        form_lay2c.addRow(PDT_Label('Atmosphere\nProperties->', font_size=12), self.atmo_props_widg)
+        self.station_params_widg = StationParamsWidget()
+        form_lay2c.addRow(PDT_Label('Control\nStations->', font_size=12), self.station_params_widg)
+
+        # extra geo params
+        form_lay2c.addRow(PDT_Label('Extra Geometry Output Parameters', font_size=14, bold=True))
+        self.skew_sb = PDT_DoubleSpinBox(font_size=12, width=80)
+        self.skew_sb.setMaximum(70)
+        form_lay2c.addRow(PDT_Label('Skew:', font_size=12), self.skew_sb)
+        self.n_prof_pts_sb = PDT_SpinBox(font_size=12, width=80)
+        self.n_prof_pts_sb.setSpecialValueText('None')
+        form_lay2c.addRow(PDT_Label('# Profile Pts:', font_size=12), self.n_prof_pts_sb)
+        self.n_profs_sb = PDT_SpinBox(font_size=12, width=80, box_range=[0, 500])
+        form_lay2c.addRow(PDT_Label('# Radial Profiles:', font_size=12), self.n_profs_sb)
+
+        # create and reset buttons
+        self.create_btn = PDT_PushButton('Create!', width=150, height=40, font_size=14, bold=True)
+        self.create_btn.clicked.connect(self.create_btn_clicked)
+        self.reset_btn = PDT_PushButton('Reset', width=150, height=40, font_size=14, bold=True)
+        self.reset_btn.clicked.connect(self.set_inputs_to_default)
+        self.save_new_btn = PDT_PushButton('Save as New', width=150, height=40, font_size=14, bold=True)
+        self.save_new_btn.clicked.connect(self.save_new_btn_clicked)
+        self.save_new_btn.setEnabled(False)
+        temp_lay = QtWidgets.QHBoxLayout()
+        temp_lay.addWidget(self.create_btn)
+        temp_lay.addWidget(self.reset_btn)
+        temp_lay.addWidget(self.save_new_btn)
+        form_lay2c.addRow(temp_lay)
+
+        # Other geo buttons
+        self.save_stl_btn = save_stl_btn = PDT_PushButton('Generate STL\nGeom. File', width=160, height=50, font_size=12)
+        self.show_stl_btn = show_stl_btn = PDT_PushButton('Show STL\nGeom. File', width=140, height=50, font_size=12)
+        self.show_blade_profs_btn = show_blade_profs_btn = PDT_PushButton('Show Blade xyz\nProfiles in Explorer', width=200,
+                                                                          height=50, font_size=12)
+        save_stl_btn.setEnabled(False)
+        show_stl_btn.setEnabled(False)
+        show_blade_profs_btn.setEnabled(False)
+        save_stl_btn.clicked.connect(self.save_stl_btn_clicked)
+        show_stl_btn.clicked.connect(self.show_stl_btn_clicked)
+        show_blade_profs_btn.clicked.connect(self.show_blade_profs_btn_clicked)
+        temp_lay2 = QtWidgets.QHBoxLayout()
+        temp_lay2.addWidget(save_stl_btn)
+        temp_lay2.addWidget(show_stl_btn)
+        temp_lay2.addWidget(show_blade_profs_btn)
+        form_lay2c.addRow(temp_lay2)
+
+        # store a list of widgets to toggle enable on
+        self.widgets_to_toggle = [self.name_le, self.nblades_sb, self.radius_sb, self.hub_radius_sb,
+                                  self.hub_wake_disp_br_sb, self.vorform_cb, self.nradial_sb, self.design_speed_sb,
+                                  self.design_adv_sb, self.design_rpm_sb, self.design_thrust_sb, self.design_power_sb,
+                                  self.design_cl_le, self.atmo_props_widg.altitude_sb, self.atmo_props_widg.rho_sb,
+                                  self.atmo_props_widg.nu_sb, self.atmo_props_widg.vsou_sb, self.station_params_widg,
+                                  self.skew_sb, self.n_prof_pts_sb, self.n_profs_sb, self.create_btn, self.reset_btn,
+                                  self.save_new_btn]
+
+        # set all the inputs to default
+        self.set_inputs_to_default()
+
+    def show_stl_btn_clicked(self):
+        prop = self.main_win.prop_widg.prop
+        if prop is None:
+            return
+
+        if os.path.exists(prop.stl_fpath):
+            self.stl_view = prop.plot_stl_mesh()
+
+    def save_stl_btn_clicked(self):
+        prop = self.main_win.prop_widg.prop
+        if prop is None:
+            return
+
+        with Capturing() as output:
+            prop.generate_stl_geometry(plot_after=False)
+        self.main_win.print(output)
+
+    def show_blade_profs_btn_clicked(self):
+        prop = self.main_win.prop_widg.prop
+        if prop is None:
+            return
+
+        if os.path.exists(prop.bld_prof_folder):
+            subprocess.Popen('explorer "{}"'.format(os.path.normpath(prop.bld_prof_folder)))
+
+    def save_new_btn_clicked(self):
+        savedir, _ = QtWidgets.QFileDialog.getSaveFileName(self, 'Enter New Save Name', self.main_win.prop_db_select_widg.db_dir)
+        if savedir:
+            savename = os.path.split(savedir)[1]
+            savedir = os.path.join(get_prop_db(), savename)
+
+            if not os.path.exists(savedir):
+                os.mkdir(savedir)
+
+            self.main_win.prop_widg.prop.save_as_new(new_name=savename)
+
+    def set_enable(self, enable: bool):
+        for widg in self.widgets_to_toggle:
+            if widg is not self.save_new_btn:
+                widg.setEnabled(enable)
+            else:
+                widg.setEnabled(not enable)
+
+    def des_thrust_sb_changed(self):
+        if self.design_thrust_sb.value() == self.design_thrust_sb.minimum():
+            self.design_power_sb.setEnabled(True)
+        else:
+            self.design_power_sb.setEnabled(False)
+
+    def des_power_sb_changed(self):
+        if self.design_power_sb.value() == self.design_power_sb.minimum():
+            self.design_thrust_sb.setEnabled(True)
+        else:
+            self.design_thrust_sb.setEnabled(False)
+
+    def des_adv_sb_changed(self):
+        self.design_rpm_sb.setEnabled(self.design_adv_sb.value() == self.design_adv_sb.minimum())
+
+    def des_rpm_sb_changed(self):
+        self.design_adv_sb.setEnabled(self.design_rpm_sb.value() == self.design_rpm_sb.minimum())
+
+    def set_inputs_to_default(self):
+        self.name_le.setText('[enter a name]')
+        self.nblades_sb.setValue(3)
+        self.radius_sb.setValue(1.0)
+        self.hub_radius_sb.setValue(0.08)
+        self.hub_wake_disp_br_sb.setValue(0.08)
+        self.vorform_cb.setCurrentText('pot')
+        self.nradial_sb.setValue(50)
+
+        self.design_speed_sb.setValue(30)
+        self.design_adv_sb.setValue(0)
+        self.design_rpm_sb.setValue(0)
+        self.design_thrust_sb.setValue(0)
+        self.design_power_sb.setValue(0)
+
+        self.design_cl_le.setText('0.2, 0.2')
+        self.atmo_props_widg.altitude_sb.setValue(self.atmo_props_widg.altitude_sb.minimum())
+        self.atmo_props_widg.rho_sb.setValue(self.atmo_props_widg.rho_sb.minimum())
+        self.atmo_props_widg.nu_sb.setValue(self.atmo_props_widg.nu_sb.minimum())
+        self.atmo_props_widg.vsou_sb.setValue(self.atmo_props_widg.vsou_sb.minimum())
+
+        self.station_params_widg.reset_to_default()
+        self.skew_sb.setValue(self.skew_sb.minimum())
+        self.n_prof_pts_sb.setValue(self.n_prof_pts_sb.minimum())
+        self.n_profs_sb.setValue(50)
+
+    def pop_inputs_from_prop(self):
+        prop = self.main_win.prop_widg.prop
+        self.name_le.setText(prop.name)
+        self.nblades_sb.setValue(prop.nblades)
+        self.radius_sb.setValue(prop.radius)
+        self.hub_radius_sb.setValue(prop.hub_radius)
+        self.hub_wake_disp_br_sb.setValue(prop.hub_wake_disp_br)
+        self.vorform_cb.setCurrentText(prop.design_vorform)
+        self.nradial_sb.setValue(prop.n_radial)
+
+        self.design_speed_sb.setValue(prop.design_speed_mps)
+
+        if prop.design_rpm is not None:
+            self.design_rpm_sb.setValue(prop.design_rpm)
+        else:
+            self.design_rpm_sb.setValue(0)
+
+        if prop.design_adv is not None:
+            self.design_adv_sb.setValue(prop.design_adv)
+        else:
+            self.design_adv_sb.setValue(0)
+
+        if prop.design_thrust is not None:
+            self.design_thrust_sb.setValue(prop.design_thrust)
+        else:
+            self.design_thrust_sb.setValue(0)
+
+        if prop.design_power is not None:
+            self.design_power_sb.setValue(prop.design_power)
+        else:
+            self.design_power_sb.setValue(0)
+
+        if len(prop.design_cl) == 1 and 'const' in prop.design_cl:
+            self.design_cl_le.setText('{}'.format(prop.design_cl['const']))
+        elif len(prop.design_cl) == 1 and 'file' in prop.design_cl:
+            pass
+        else:
+            assert 'root' in prop.design_cl
+            assert 'tip' in prop.design_cl
+            self.design_cl_le.setText('{}, {}'.format(prop.design_cl['root'], prop.design_cl['tip']))
+
+        if 'altitude_km' in prop.design_atmo_props:
+            self.atmo_props_widg.altitude_sb.setValue(prop.design_atmo_props['altitude_km'])
+        else:
+            self.atmo_props_widg.altitude_sb.setValue(0)
+
+        if 'dens' in prop.design_atmo_props:
+            self.atmo_props_widg.rho_sb.setValue(prop.design_atmo_props['dens'])
+        else:
+            self.atmo_props_widg.rho_sb.setValue(0)
+
+        if 'visc' in prop.design_atmo_props:
+            self.atmo_props_widg.nu_sb.setValue(prop.design_atmo_props['visc'])
+        else:
+            self.atmo_props_widg.nu_sb.setValue(0)
+
+        if 'vsou' in prop.design_atmo_props:
+            self.atmo_props_widg.vsou_sb.setValue(prop.design_atmo_props['vsou'])
+        else:
+            self.atmo_props_widg.vsou_sb.setValue(0)
+
+        self.station_params_widg.reset_to_default()
+        for st_loc, foil_name in prop.station_params.items():
+            if not foil_name.endswith('.dat'):
+                foil_name = '{}.dat'.format(foil_name)
+            foil_cb, roR_sb = self.station_params_widg.add_row()
+            foil_cb.setCurrentText(foil_name)
+            roR_sb.setValue(st_loc)
+
+        self.skew_sb.setValue(prop.tot_skew)
+        if prop.n_prof_pts is None:
+            self.n_prof_pts_sb.setValue(self.n_prof_pts_sb.minimum())
+        else:
+            self.n_prof_pts_sb.setValue(prop.n_prof_pts)
+        self.n_profs_sb.setValue(prop.n_profs)
+
+    def create_btn_clicked(self):
+        msgbox = QtWidgets.QMessageBox()
+
+        name = self.name_le.text()
+        if len(name.strip()) == 0:
+            msgbox.about(self, 'Error', 'Invalid Name')
+            return
+
+        nblades = self.nblades_sb.value()
+        radius = self.radius_sb.value()
+        hub_radius = self.hub_radius_sb.value()
+        hub_wk_disp_br = self.hub_wake_disp_br_sb.value()
+        speed = self.design_speed_sb.value()
+        adv = self.design_adv_sb.value() if self.design_adv_sb.value() != self.design_adv_sb.minimum() else None
+        rpm = self.design_rpm_sb.value() if self.design_rpm_sb.value() != self.design_rpm_sb.minimum() else None
+        if adv == self.design_adv_sb.minimum() and rpm == self.design_rpm_sb.minimum():
+            msgbox.about(self, 'Error', 'Must give one of "adv" or "rpm"')
+            return
+
+        thrust = self.design_thrust_sb.value() if self.design_thrust_sb.value() != self.design_thrust_sb.minimum() else None
+        power = self.design_power_sb.value() if self.design_power_sb.value() != self.design_power_sb.minimum() else None
+        if thrust is None and power is None:
+            msgbox.about(self, 'Error', 'Must give one of "thrust" or "power"')
+            return
+
+        nradial = self.nradial_sb.value()
+        cl_txt = self.design_cl_le.text().strip()
+        if len(cl_txt.split(',')) == 1:
+            cl_dict = {'const': float(cl_txt)}
+        elif len(cl_txt.split(',')) == 2:
+            cl_dict = {'root': float(cl_txt.split(',')[0].strip()), 'tip': float(cl_txt.split(',')[1].strip())}
+        else:
+            msgbox = QtWidgets.QMessageBox()
+            msgbox.about(self, 'Error', 'Only "const" and "linear" CL currently supported')
+            return
+
+        altitude = self.atmo_props_widg.altitude_sb.value()
+        alt_ismin = altitude == self.atmo_props_widg.altitude_sb.minimum()
+        rho = self.atmo_props_widg.rho_sb.value()
+        rho_ismin = rho == self.atmo_props_widg.rho_sb.minimum()
+        nu = self.atmo_props_widg.nu_sb.value()
+        nu_ismin = nu == self.atmo_props_widg.nu_sb.minimum()
+        vsou = self.atmo_props_widg.vsou_sb.value()
+        vsou_ismin = vsou == self.atmo_props_widg.vsou_sb.minimum()
+        if alt_ismin and any([rho_ismin, nu_ismin, vsou_ismin]):
+            msgbox.about(self, 'Error', 'Can only / must give "altitude" or all three "rho", "nu" and "vsou"')
+            return
+
+        vorform = self.vorform_cb.currentText()
+        stations_dict = self.station_params_widg.get_stations_dict()
+        if stations_dict is None:
+            msgbox.about(self, 'Error', 'Must give at least 1 station')
+            return
+
+        skew = self.skew_sb.value()
+        n_prof_pts = self.n_prof_pts_sb.value() if self.n_prof_pts_sb.value() != self.n_prof_pts_sb.minimum() else None
+        n_profs = self.n_profs_sb.value()
+
+        if altitude is not None:
+            atmo_props = {'altitude_km': altitude}
+        else:
+            atmo_props = {'rho': rho, 'nu': nu, 'vsou': vsou}
+
+        self.timer = QtCore.QTimer()
+        self.timer.timeout.connect(self.update_create_worker_progress)
+        self.timer.start(1000)
+        self.timer_cntr = 0
+
+        self.thread = QtCore.QThread()
+        self.prop_create_worker = CreatePropellerWorker(name=name,
+                                                        nblades=nblades,
+                                                        radius=radius,
+                                                        hub_radius=hub_radius,
+                                                        hub_wake_disp_br=hub_wk_disp_br,
+                                                        design_speed_mps=speed,
+                                                        design_cl=cl_dict,
+                                                        design_atmo_props=atmo_props,
+                                                        design_vorform=vorform,
+                                                        station_params=stations_dict,
+                                                        design_adv=adv,
+                                                        design_rpm=rpm,
+                                                        design_thrust=thrust,
+                                                        design_power=power,
+                                                        n_radial=nradial,
+                                                        skew=skew,
+                                                        n_prof_pts=n_prof_pts,
+                                                        n_profs=n_profs)
+        self.prop_create_worker.moveToThread(self.thread)
+        self.thread.started.connect(self.prop_create_worker.run)
+        self.prop_create_worker.finished.connect(self.thread.quit)
+        self.prop_create_worker.finished.connect(self.prop_create_worker.deleteLater)
+        self.prop_create_worker.finished.connect(self.on_create_worker_finish)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.prop_create_worker.progress.connect(self.update_create_worker_progress)
+
+        self.main_win.prop_widg.setEnabled(False)
+        self.thread.start()
+
+    def on_create_worker_finish(self, prop, output):
+        self.timer.stop()
+        self.main_win.prog_bar.setValue(0)
+        self.main_win.print(output)
+        if prop:
+            self.main_win.prop_db_select_widg.update_found_lbl()
+            self.main_win.prop_widg.plot3d_widg.populate_select_prop_cb()
+            self.main_win.prop_widg.plot3d_widg.select_prop_cb.setCurrentText(prop.name)
+            self.main_win.prop_widg.setEnabled(True)
+
+    def update_create_worker_progress(self):
+        val = 2 if self.vorform_cb.currentText() == 'vrtx' else 33
+        self.timer_cntr += val
+        prog_val = self.timer_cntr if self.timer_cntr < 100 else 99
+        self.main_win.prog_bar.setValue(prog_val)
+
+
+class Propeller3dPlotWidget(QtWidgets.QWidget):
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        self.main_win = main_win
+        super(Propeller3dPlotWidget, self).__init__()
+        main_lay = QtWidgets.QVBoxLayout()
+        self.setLayout(main_lay)
+
+        form_lay = QtWidgets.QFormLayout()
+        hlay = QtWidgets.QHBoxLayout()
+        hlay.addLayout(form_lay)
+        self.select_prop_cb = PDT_ComboBox(width=150)
+        form_lay.addRow(PDT_Label('Select Propeller:', font_size=14, bold=True), self.select_prop_cb)
+        self.enable_edit_chk = PDT_CheckBox('Enable Editing of Design Point', italic=True, font_size=10)
+        # self.enable_edit_chk.clicked.connect(self.enable_edit_chk_clicked)
+        form_lay.addRow(self.enable_edit_chk)
+        self.show_rstation_btn = PDT_PushButton('Show Radial\nStation Params', font_size=14, width=160, bold=True)
+        self.show_rstation_btn.clicked.connect(self.show_rstation_btn_clicked)
+        hlay.addWidget(self.show_rstation_btn)
+        self.show_panel_btn = PDT_PushButton('Show Design\nPoint Panel', font_size=14, width=160, bold=True)
+        self.show_panel_btn.clicked.connect(self.show_panel_btn_clicked)
+        hlay.addWidget(self.show_panel_btn)
+        main_lay.addLayout(hlay)
+        self.populate_select_prop_cb()
+
+        self.plot_canvas = SingleAxCanvas(self, width=6, height=6, projection='3d')
+        self.axes3d = self.plot_canvas.axes
+        main_lay.addWidget(self.plot_canvas)
+
+    # def enable_edit_chk_clicked(self):
+    #     pass
+
+    def show_rstation_btn_clicked(self):
+        prop = self.main_win.prop_widg.prop
+        if prop is not None:
+            self.station_widgs = []
+            for st in prop.stations:
+                st_widg = QtWidgets.QWidget()
+                self.station_widgs.append(st_widg)
+                lay = QtWidgets.QVBoxLayout()
+                st_widg.setLayout(lay)
+
+                fit_canvas = RadialStationFitParamsCanvas()
+                lay.addWidget(fit_canvas)
+                st.plot_xrotor_fit_params(fig=fit_canvas.figure)
+
+                st_widg.show()
+                fit_canvas.draw()
+        return
+
+    def show_panel_btn_clicked(self):
+        prop = self.main_win.prop_widg.prop
+        if prop is not None:
+            self.creation_panel_widg = QtWidgets.QWidget()
+            lay = QtWidgets.QVBoxLayout()
+            self.creation_panel_widg.setLayout(lay)
+
+            self.creation_panel_canvas = PropellerCreationPanelCanvas()
+            lay.addWidget(self.creation_panel_canvas)
+            prop.plot_design_point_panel(fig=self.creation_panel_canvas.figure)
+
+            self.creation_panel_widg.show()
+            self.creation_panel_canvas.draw()
+
+    def update_plot(self, prop: Propeller):
+        with Capturing() as output:
+            prop.plot_mpl3d_geometry(interp_profiles=True, hub=True, input_stations=True, chords_betas=True, LE=True,
+                                     TE=True, fig=self.plot_canvas.figure)
+        self.main_win.console_te.append('\n'.join(output) if len(output) > 0 else '')
+        self.plot_canvas.draw()
+
+    def clear_plot(self):
+        self.axes3d.clear()
+        self.plot_canvas.draw()
+
+    def populate_select_prop_cb(self):
+        self.select_prop_cb.blockSignals(True)
+        self.select_prop_cb.clear()
+        self.select_prop_cb.blockSignals(False)
+        self.select_prop_cb.addItems(['None'] + get_all_propeller_dirs())
+
+
+class StationParamsWidget(QtWidgets.QWidget):
+    def __init__(self):
+        super(StationParamsWidget, self).__init__()
+
+        main_lay = QtWidgets.QVBoxLayout()
+        self.rows_lay = QtWidgets.QFormLayout()
+        self.setLayout(main_lay)
+        main_lay.addLayout(self.rows_lay)
+
+        self.header_row_strs = ['#', 'Foil', 'r/R']
+        self.add_header_row()
+        self.add_btn = PDT_PushButton('(+) add', width=80, font_size=11)
+        self.remove_btn = PDT_PushButton('(-) remove', width=100, font_size=11)
+
+        btn_lay = QtWidgets.QHBoxLayout()
+        btn_lay.addWidget(self.add_btn)
+        btn_lay.addWidget(self.remove_btn)
+        main_lay.addLayout(btn_lay)
+
+        # connect signals
+        self.add_btn.clicked.connect(self.add_row)
+        self.remove_btn.clicked.connect(self.remove_row)
+
+    def reset_to_default(self):
+        count = self.rows_lay.rowCount()
+        while count > 1:
+            self.rows_lay.removeRow(count - 1)
+            count -= 1
+
+    def add_header_row(self):
+        num_lbl = PDT_Label(self.header_row_strs[0], font_size=11)
+        foil_lbl = PDT_Label(self.header_row_strs[1], font_size=11)
+        roR_lbl = PDT_Label(self.header_row_strs[2], font_size=11)
+        rt_lay = QtWidgets.QHBoxLayout()
+        rt_lay.addWidget(foil_lbl)
+        rt_lay.addWidget(roR_lbl)
+        rt_widg = QtWidgets.QWidget()
+        rt_widg.setLayout(rt_lay)
+        self.rows_lay.addRow(num_lbl, rt_widg)
+
+    def add_row(self):
+        rt_lay = QtWidgets.QHBoxLayout()
+        rt_widg = QtWidgets.QWidget()
+        rt_widg.setLayout(rt_lay)
+        if self.rows_lay.rowCount() > 1:
+            msgbox = QtWidgets.QMessageBox()
+            msgbox.about(self, 'Error', '> 1 station not yet implemented in PDT')
+            return
+        num_lbl = PDT_Label('{}'.format(self.rows_lay.rowCount()), font_size=11)
+        foil_cb = PDT_ComboBox(font_size=11, width=140)
+        foil_cb.addItems(get_all_airfoil_files())
+        roR_sb = PDT_DoubleSpinBox(font_size=11)
+        roR_sb.setMaximum(1.0)
+        roR_sb.setSingleStep(0.01)
+        roR_sb.setValue(0.75)
+        rt_lay.addWidget(foil_cb)
+        rt_lay.addWidget(roR_sb)
+        self.rows_lay.addRow(num_lbl, rt_widg)
+        return foil_cb, roR_sb
+
+    def remove_row(self):
+        row = self.rows_lay.rowCount() - 1
+        self.rows_lay.removeRow(row)
+
+    def get_stations_dict(self):
+        if self.rows_lay.rowCount() == 1:
+            return None
+        else:
+            stations = {}
+            for row in range(1, self.rows_lay.rowCount()):
+                rt_widg = self.rows_lay.itemAt(row, 1).widget()
+                itm1, itm2 = [rt_widg.layout().itemAt(i) for i in range(rt_widg.layout().count())]
+                foil_cb = itm1.widget()
+                roR_sb = itm2.widget()
+                stations[roR_sb.value()] = foil_cb.currentText()
+        return stations
+
+
+class AtmoPropsInputWidget(QtWidgets.QWidget):
+    def __init__(self):
+        super(AtmoPropsInputWidget, self).__init__()
+        lay = QtWidgets.QHBoxLayout()
+        self.setLayout(lay)
+        left_lay = QtWidgets.QVBoxLayout()
+        left_center_lay = QtWidgets.QFormLayout()
+        left_lay.addStretch()
+        left_lay.addLayout(left_center_lay)
+        left_lay.addStretch()
+        right_lay = QtWidgets.QFormLayout()
+        lay.addLayout(left_lay)
+        lay.addWidget(PDT_Label('or'))
+        lay.addLayout(right_lay)
+        lay.addStretch()
+
+        self.altitude_sb = PDT_DoubleSpinBox(width=80, font_size=12)
+        self.altitude_sb.setMinimum(-2)
+        self.altitude_sb.setSpecialValueText('None')
+        left_center_lay.addRow(PDT_Label('Altitude:', font_size=12), self.altitude_sb)
+
+        self.rho_sb = PDT_DoubleSpinBox(width=80, font_size=12)
+        self.rho_sb.setSpecialValueText('None')
+        right_lay.addRow(PDT_Label('Rho:', font_size=12), self.rho_sb)
+        self.nu_sb = PDT_DoubleSpinBox(width=80, font_size=12)
+        self.nu_sb.setSpecialValueText('None')
+        right_lay.addRow(PDT_Label('Nu:', font_size=12), self.nu_sb)
+        self.vsou_sb = PDT_DoubleSpinBox(width=80, font_size=12)
+        self.vsou_sb.setSpecialValueText('None')
+        right_lay.addRow(PDT_Label('Vsou:', font_size=12), self.vsou_sb)
+
+        # connect some signals
+        self.altitude_sb.valueChanged.connect(self.altitude_sb_changed)
+        self.rho_sb.valueChanged.connect(self.rho_sb_changed)
+        self.nu_sb.valueChanged.connect(self.nu_sb_changed)
+        self.vsou_sb.valueChanged.connect(self.vsou_sb_changed)
+
+    def vsou_sb_changed(self):
+        if self.rho_sb.value() == self.rho_sb.minimum() \
+                and self.nu_sb.value() == self.nu_sb.minimum() \
+                and self.vsou_sb.value() == self.vsou_sb.minimum():
+            self.altitude_sb.setEnabled(True)
+        else:
+            self.altitude_sb.setEnabled(False)
+
+    def nu_sb_changed(self):
+        if self.rho_sb.value() == self.rho_sb.minimum() \
+                and self.nu_sb.value() == self.nu_sb.minimum() \
+                and self.vsou_sb.value() == self.vsou_sb.minimum():
+            self.altitude_sb.setEnabled(True)
+        else:
+            self.altitude_sb.setEnabled(False)
+
+    def rho_sb_changed(self):
+        if self.rho_sb.value() == self.rho_sb.minimum() \
+                and self.nu_sb.value() == self.nu_sb.minimum() \
+                and self.vsou_sb.value() == self.vsou_sb.minimum():
+            self.altitude_sb.setEnabled(True)
+        else:
+            self.altitude_sb.setEnabled(False)
+
+    def altitude_sb_changed(self):
+        if self.altitude_sb.value() == self.altitude_sb.minimum():
+            self.rho_sb.setEnabled(True)
+            self.nu_sb.setEnabled(True)
+            self.vsou_sb.setEnabled(True)
+        else:
+            self.rho_sb.setEnabled(False)
+            self.nu_sb.setEnabled(False)
+            self.vsou_sb.setEnabled(False)
+
+
+class CreatePropellerWorker(QtCore.QObject):
+    finished = QtCore.pyqtSignal(object, list)
+    progress = QtCore.pyqtSignal(int)
+
+    def __init__(self, name: str, nblades: int, radius: float, hub_radius: float, hub_wake_disp_br: float,
+                 design_speed_mps: float, design_cl: dict, design_atmo_props: dict, design_vorform: str,
+                 station_params: dict = None, design_adv: float = None, design_rpm: float = None,
+                 design_thrust: float = None, design_power: float = None, n_radial: int = 50, skew: float = 0.0,
+                 n_prof_pts: int = None, n_profs: int = 50):
+
+        super(CreatePropellerWorker, self).__init__()
+
+        self.name = name
+        self.nblades = nblades
+        self.radius = radius
+        self.hub_radius = hub_radius
+        self.hub_wake_disp_br = hub_wake_disp_br
+        self.design_speed_mps = design_speed_mps
+        self.design_cl = design_cl
+        self.design_atmo_props = design_atmo_props
+        self.design_vorform = design_vorform
+        self.station_params = station_params
+        self.design_adv = design_adv
+        self.design_rpm = design_rpm
+        self.design_thrust = design_thrust
+        self.design_power = design_power
+        self.n_radial = n_radial
+        self.skew = skew
+        self.n_prof_pts = n_prof_pts
+        self.n_profs = n_profs
+
+    def run(self):
+        try:
+            with Capturing() as output:
+                prop = create_propeller(name=self.name,
+                                        nblades=self.nblades,
+                                        radius=self.radius,
+                                        hub_radius=self.hub_radius,
+                                        hub_wake_disp_br=self.hub_wake_disp_br,
+                                        design_speed_mps=self.design_speed_mps,
+                                        design_cl=self.design_cl,
+                                        design_atmo_props=self.design_atmo_props,
+                                        design_vorform=self.design_vorform,
+                                        station_params=self.station_params,
+                                        design_adv=self.design_adv,
+                                        design_rpm=self.design_rpm,
+                                        design_thrust=self.design_thrust,
+                                        design_power=self.design_power,
+                                        n_radial=self.n_radial,
+                                        verbose=True,
+                                        show_station_fit_plots=False,
+                                        plot_after=False,
+                                        tmout=None,
+                                        hide_windows=True,
+                                        geo_params={'tot_skew': self.skew, 'n_prof_pts': self.n_prof_pts,
+                                                    'n_profs': self.n_profs})
+        except Exception as e:
+            prop = None
+            output = [e.__repr__()]
+
+        self.finished.emit(prop, output)
```

### Comparing `propeller_design_tools-0.3.5/propdes/propeller.py` & `propeller_design_tools-0.4.0/propeller_design_tools/propeller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1180 +1,1180 @@
-import os
-import shutil
-from propdes import funcs
-from propdes.user_io import Info, Error, Warning
-from propdes.settings import get_setting
-from propdes.airfoil import Airfoil
-from propdes.settings import VALID_OPER_PLOT_PARAMS
-from propdes.custom_opengl_classes import Custom3DArrow
-import matplotlib.pyplot as plt
-import matplotlib.gridspec as gridspec
-from mpl_toolkits import mplot3d
-import numpy as np
-from stl import mesh
-from typing import Union
-import pyqtgraph as pg
-import pyqtgraph.opengl as gl
-
-
-class Propeller(object):
-
-    creation_attrs = {'nblades': int, 'radius': float, 'hub_radius': float, 'hub_wake_disp_br': float,
-                      'design_speed_mps': float, 'design_adv': float, 'design_rpm': float, 'design_thrust': float,
-                      'design_power': float, 'design_cl': dict, 'design_atmo_props': dict, 'design_vorform': str,
-                      'station_params': dict, 'station_polars': list, 'geo_params': dict}
-    saveload_attrs = {**creation_attrs, **{'name': str, 'meta_file': str, 'xrr_file': str, 'xrop_file': str,
-                                           'blade_data': dict, 'blade_xyz_profiles': dict}}
-
-    def __init__(self, name, verbose: bool = True, **kwargs):
-        # name is always given, detect if it's a filepath
-        self.savepath = None
-        if os.path.exists(name):
-            self.savepath, name = os.path.split(name)
-        self.name = name.replace('.txt', '')
-        self.oper_data = None
-        self.wvel_data = None
-        self.stl_mesh = None
-
-        # check if the prop db exists
-        prop_db = get_setting('propeller_database')
-        if prop_db is None:
-            raise Error(s='No Propeller Database is set!  First set one with "pdt.set_propeller_database(str)".')
-
-        # initialize all attrs to None for script auto-completion detection
-        self.nblades, self.radius, self.hub_radius, self.hub_wake_disp_br, self.design_speed_mps, self.design_adv, \
-        self.design_rpm, self.design_thrust, self.design_power, self.design_cl, self.design_atmo_props, \
-        self.design_vorform, self.station_params, self.geo_params, self.xrotor_d, self.xrotor_op_dict, \
-        self.blade_data, self.blade_xyz_profiles = [None] * 18
-
-        # if no kwargs were given and there's a meta_file, load it
-        if len(kwargs) == 0:
-            if os.path.exists(self.meta_file):
-                if verbose:
-                    Info(s='Loading propeller "meta-file" ({})'.format(self.meta_file))
-                self.load_from_savefile(verbose=verbose)
-            else:
-                raise FileNotFoundError('Could not find file {}'.format(self.meta_file))
-        else:  # cycle thru kwargs and set if they're valid, if not ignore them
-            for key, val in kwargs.items():
-                if key in self.creation_attrs:
-                    setattr(self, key, val)
-                else:
-                    raise Error('Unknown KWARG input "{}"'.format(key))
-
-        # attempt to load any oper sweep data and any wvel sweep data
-        self.oper_data = PropellerOperData(directory=self.oper_data_dir)
-        self.oper_data.load_oper_sweep_results(verbose=verbose)
-        self.wvel_data = PropellerWVelData(directory=self.wvel_data_dir)
-        self.wvel_data.load_wvel_sweep_results(verbose=verbose)
-
-        # attempt to load any STL mesh data
-        self.load_stl_geometry(verbose=verbose)
-
-    @property
-    def stl_fpath(self):
-        return os.path.join(self.save_folder, '{}.stl'.format(self.name))
-
-    @property
-    def station_polar_folder(self):
-        return os.path.join(self.save_folder, 'station_polars')
-
-    @property
-    def bld_prof_folder(self):
-        return os.path.join(self.save_folder, 'blade_profiles')
-
-    @property
-    def xrr_file(self):
-        return os.path.join(self.save_folder, '{}.xrr'.format(self.name))
-
-    @property
-    def xrop_file(self):
-        return os.path.join(self.save_folder, '{}.xrop'.format(self.name))
-
-    @property
-    def meta_file(self):
-        return os.path.join(self.save_folder, '{}.meta'.format(self.name))
-
-    @property
-    def save_folder(self):
-        if self.savepath is None:
-            return os.path.join(get_setting('propeller_database'), self.name)
-        else:
-            return os.path.join(self.savepath, self.name)
-
-    @property
-    def tot_skew(self):
-        return self.geo_params['tot_skew']
-
-    @property
-    def n_prof_pts(self):
-        return self.geo_params['n_prof_pts']
-
-    @property
-    def n_profs(self):
-        return self.geo_params['n_profs']
-
-    @property
-    def design_rho(self):
-        if 'dens' in self.design_atmo_props:
-            return self.design_atmo_props['dens']
-
-    @design_rho.setter
-    def design_rho(self, value):
-        self.design_atmo_props['dens'] = value
-
-    @property
-    def disk_area_m_sqrd(self):
-        if self.radius is not None and self.hub_radius is not None:
-            return np.pi * (self.radius ** 2 - self.hub_radius ** 2)
-
-    @property
-    def ideal_eff(self):
-        req_attrs = [self.design_thrust, self.design_rho, self.disk_area_m_sqrd, self.design_speed_mps]
-        if all([attr is not None for attr in req_attrs]):
-            return funcs.calc_ideal_eff(*req_attrs)
-
-    @property
-    def disk_loading(self):
-        if self.xrotor_op_dict is not None and self.disk_area_m_sqrd is not None:
-            return self.xrotor_op_dict['thrust(N)'] / self.disk_area_m_sqrd
-
-    @property
-    def oper_data_dir(self):
-        return os.path.join(os.path.split(self.meta_file)[0], 'oper_data')
-
-    @property
-    def wvel_data_dir(self):
-        return os.path.join(os.path.split(self.meta_file)[0], 'wvel_data')
-
-    @property
-    def n_radial(self):
-        return len(self.blade_xyz_profiles)
-
-    @property
-    def valid_oper_plot_params(self):
-        return
-
-    def save_as_new(self, new_name: str):
-        # store filepaths before we change name
-        old_xrop_file = self.xrop_file * 1
-        old_xrr_file = self.xrr_file * 1
-        old_blade_profs_folder = self.bld_prof_folder * 1
-
-        # change the name, make a new directory
-        self.name = new_name
-        if not os.path.exists(self.save_folder):
-            os.mkdir(self.save_folder)
-
-        # save off a new meta file, copy the xrop and xrr files
-        self.save_meta_file()
-        shutil.copyfile(old_xrop_file, self.xrop_file)
-        shutil.copyfile(old_xrr_file, self.xrr_file)
-
-        # blade profiles
-        if not os.path.exists(self.bld_prof_folder):
-            os.mkdir(self.bld_prof_folder)
-        for fname in [f for f in os.listdir(old_blade_profs_folder) if f.endswith('.txt')]:
-            fpath = os.path.join(old_blade_profs_folder, fname)
-            copypath = os.path.join(self.bld_prof_folder, fname)
-            shutil.copyfile(fpath, copypath)
-
-    def read_pdt_metafile(self):
-        # read in the PDT meta-file (in the root propeller database) and set Propeller attrs
-        with open(self.meta_file, 'r') as f:
-            txt = f.read().strip()
-        lines = txt.split('\n')
-
-        blade_data = {}
-        point_cloud = {}
-
-        for line in lines:
-            line_attr, line_val = [i.strip() for i in line.split(':', 1)]
-            if 'blade_data_' in line_attr:
-                blade_data[line_attr.split('blade_data_', 1)[1]] = np.array([float(v) for v in line_val.strip().split(', ')])
-            if 'point_cloud_' in line_attr:
-                point_cloud[line_attr.split('point_cloud_', 1)[1]] = np.array([float(v) for v in line_val.strip().split(', ')])
-            for attr, tipe in self.saveload_attrs.items():
-                if line_attr == attr:
-                    val = line.split(': ', 1)[1]
-                    if val == 'None':
-                        val = None
-                    else:
-                        if tipe is int:
-                            val = int(val)
-                        elif tipe is float:
-                            val = float(val)
-                        elif tipe is dict:
-                            items = [item.split(': ') for item in
-                                     val.replace('{', '').replace('}', '').replace("'", '').split(', ')]
-                            # check for keys that are floats or ints
-                            keys_are_nums = [itm[0].replace('.', '').isnumeric() for itm in items]
-                            if all(keys_are_nums):
-                                for i, itm in enumerate(items):
-                                    new_itm = [float(itm[0]), itm[1]]
-                                    items[i] = new_itm
-                            val = {}
-                            for key, entry in items:
-                                if 'none' == entry.lower():
-                                    entry = None
-                                try:    # try to convert to float
-                                    val[key] = float(entry)
-                                except:     # otherwise store as string
-                                    val[key] = entry
-                        elif tipe is list:
-                            val = []
-                    setattr(self, attr, val)
-        self.set_blade_data(blade_dict=blade_data)
-
-    def read_xrotor_restart(self):
-        with open(self.xrr_file, 'r') as f:
-            txt = f.read().strip()
-        lines = txt.split('\n')
-
-        def read_line_pair(kw_idx):
-            keywords = lines[kw_idx].strip('!').split()
-            values = lines[kw_idx + 1].split()
-            return dict(zip(keywords, values))
-
-        def read_xi_sect(xi_idx):
-            xi_d = {}
-            for lni in [xi_idx, xi_idx + 2, xi_idx + 4, xi_idx + 6, xi_idx + 8]:
-                for k, v in read_line_pair(lni).items():
-                    xi_d[k] = float(v)
-            return xi_d
-
-        def read_geo_stations(header_idx):
-            geo_d = {}
-            headers = lines[header_idx].strip('!').split()
-            for h in headers:
-                geo_d[h] = []
-            for idx in range(header_idx + 1, len(lines)):
-                vals = lines[idx].split()
-                if len(vals) == len(headers):
-                    for i, val in enumerate(vals):
-                        geo_d[headers[i]].append(float(val))
-            return geo_d
-
-        d = {}
-        design_param_lines = [2, 4, 6, 8]
-        for ln_idx in design_param_lines:
-            for k, v in read_line_pair(ln_idx).items():
-                d[k] = float(v)
-
-        xi_lines = [i * 10 for i in range(1, int(d['Naero']) + 1)]   # works out that each xi section is 10 lines, and 1st one on line 10 always
-        for sect_idx, ln_idx in enumerate(xi_lines):
-            xi_d = read_xi_sect(ln_idx)
-            d['Xisection_{}'.format(sect_idx)] = xi_d
-
-        for k, v in read_line_pair(kw_idx=xi_lines[-1] + 10).items():
-            d[k] = v
-
-        for k, v in read_line_pair(kw_idx=xi_lines[-1] + 12).items():
-            d[k] = int(v)
-
-        for k, v in read_geo_stations(header_idx=xi_lines[-1] + 14).items():
-            d[k] = v
-
-        # turn all lists into numpy arrays before returning
-        for key, val in d.items():
-            if isinstance(val, list):
-                d[key] = np.array(val)
-
-        return d
-
-    def load_from_savefile(self, verbose):
-        # 1st set attrs from the PDT metafile
-        self.read_pdt_metafile()
-        if verbose:
-            Info(s='Successfully read meta-file (.meta)!', indent_level=1)
-
-        # set the stations... why did I do it this way??
-        self.set_stations(plot_also=False, verbose=verbose, from_loadsave_file=True)
-        if verbose:
-            Info(s='Successfully read and set station polars!', indent_level=1)
-
-        # then read in the XROTOR restart file (in the xrotor_geometry_files)
-        self.xrotor_d = self.read_xrotor_restart()
-        if verbose:
-            Info(s='Successfully read XROTOR restart file (.xrr)!', indent_level=1)
-
-        # then read the operating point output file (in xrotor_op_files)
-        self.xrotor_op_dict = funcs.read_xrotor_op_file(fpath=self.xrop_file)
-        if verbose:
-            Info(s='Successfully read XROTOR operating-point file (.xrop)!', indent_level=1)
-
-        # and finally read in the point cloud files
-        self.blade_xyz_profiles = {}
-        fnames = funcs.search_files(folder=self.bld_prof_folder)
-        for fname in fnames:
-            prof_num = int(fname.replace('profile_', '').replace('.txt', ''))
-            xyz_prof = funcs.read_profile_xyz(fpath=os.path.join(self.bld_prof_folder, fname))
-            self.blade_xyz_profiles[prof_num] = xyz_prof
-        if verbose:
-            Info(s='Successfully read blade profiles!', indent_level=1)
-
-        return
-
-    def set_stations(self, plot_also: bool = True, verbose: bool = False, from_loadsave_file: bool = False):
-        if not from_loadsave_file:
-            self.stations, txt = funcs.create_radial_stations(prop=self, plot_also=plot_also, verbose=verbose)
-        else:
-            self.stations = funcs.read_radial_stations(prop=self, plot_also=plot_also, verbose=False)
-            txt = ''
-        return txt
-
-    def show_station_fits(self):
-        for st in self.stations:
-            fig = st.plot_xrotor_fit_params()
-
-    def set_blade_data(self, blade_dict: dict):
-        self.blade_data = blade_dict
-        return
-
-    def save_meta_file(self):
-        attrs_2_ignore = ['blade_xyz_profiles', 'meta_file', 'xrr_file', 'xrop_file', 'station_polars']   # ignore the files so that prop_dirs can be switched
-
-        if os.path.exists(self.meta_file):
-            os.remove(self.meta_file)
-
-        with open(self.meta_file, 'w') as f:
-            for attr in [a for a in self.saveload_attrs if a not in attrs_2_ignore]:
-                if attr == 'blade_data':
-                    for key, val in self.blade_data.items():
-                        val = ', '.join([str(i) for i in val])
-                        f.write('{}: {}\n'.format('blade_data_{}'.format(key), val))
-                else:
-                    f.write('{}: {}\n'.format(attr, getattr(self, attr)))
-
-    def save_station_polars(self):
-        if not os.path.exists(self.station_polar_folder):
-            os.mkdir(self.station_polar_folder)
-
-        for i, roR in enumerate(self.station_params.keys()):
-            station = self.stations[i]
-            foil_name = self.station_params[roR]
-            savename = '{}_{}.polar'.format(roR, foil_name)
-            savepath = os.path.join(self.station_polar_folder, savename)
-            with open(savepath, 'w') as f:
-                for key, val in station.foil_polar.items():
-                    if isinstance(val, list) or isinstance(val, np.ndarray):
-                        val = ', '.join([str(v) for v in val])
-                    f.write('{}: {}\n'.format(key, val))
-
-    def get_blade_le_te(self, rotate_deg: float = 0.0, axis_shift: float = 0.25):
-        radii = self.radius * np.array(self.xrotor_d['r/R'])
-        chords = self.radius * np.array(self.xrotor_d['C/R'])
-        betas = np.array(self.xrotor_d['Beta0deg'])
-        le_pts = []
-        te_pts = []
-        for radius, chord, beta in zip(radii, chords, betas):
-            le_te_coords = np.array([[0.0, 1.0], [0.0, 0.0]])
-            xs, ys, zs = funcs.generate_3D_profile_points(nondim_xy_coords=le_te_coords, radius=radius,
-                                                            axis_shift=axis_shift, chord_len=chord, beta_deg=beta,
-                                                            skew_deg=rotate_deg)
-            le_pts.append([xs[0], ys[0], zs[0]])
-            te_pts.append([xs[1], ys[1], zs[1]])
-        return le_pts, te_pts
-
-    def get_blade_quarter_chords(self):  # for plotting of wvel vectors
-        chordlines = self.get_blade_chordlines(rotate_deg=0)
-        q_chord_pts = []
-        for line in chordlines:
-            qtr_idx = int(len(line) / 4)
-            q_chord_pts.append(line[qtr_idx])
-
-        return q_chord_pts
-
-    def get_blade_chordlines(self, rotate_deg: float, axis_shift: float = 0.25, npts: int = 50):
-        radii = self.radius * np.array(self.xrotor_d['r/R'])
-        chords = self.radius * np.array(self.xrotor_d['C/R'])
-        betas = np.array(self.xrotor_d['Beta0deg'])
-        chordlines = []
-        for radius, chord, beta in zip(radii, chords, betas):
-            xs = np.linspace(0, 1, npts)
-            ys = np.zeros(len(xs))
-            chordline_nondim = np.vstack([xs, ys])
-            xs, ys, zs = funcs.generate_3D_profile_points(nondim_xy_coords=chordline_nondim, radius=radius,
-                                                   axis_shift=axis_shift, chord_len=chord, beta_deg=beta,
-                                                   skew_deg=rotate_deg)
-            coords = list(zip(xs, ys, zs))
-            chordlines.append(coords)
-        return chordlines
-
-    def interp_foil_profiles(self, n_prof_pts: int = None, n_profs: int = 50, tot_skew: float = 0.0):
-
-        assert len(self.stations) > 0
-
-        if len(self.stations) != 1:
-            raise Error('> 1 profile interpolation not yet implemented')
-
-        if tot_skew != 0.0:
-            Info('Blade "skew" is not implemented in XROTOR, and therefore not reflected in XROTOR results.\n'
-                 '  > Skew effects are considered negligible for PDT purposes for small enough skew angles.')
-
-        # clear out the existing xyz profiles
-        funcs.delete_files_from_folder(self.bld_prof_folder)
-
-        station = self.stations[0]
-        # nondim_coords = station.foil.get_coords(n_interp=n_prof_pts)
-        nondim_coords = station.foil.get_coords_closed_te(n_interp=n_prof_pts)
-
-        self.blade_xyz_profiles = {}
-        for i, roR in enumerate(np.linspace(self.blade_data['r/R'][0], self.blade_data['r/R'][-1], n_profs)):
-            chord = np.interp(x=roR, xp=self.blade_data['r/R'], fp=self.blade_data['CH']) * self.radius
-            beta = np.rad2deg(np.interp(x=roR, xp=self.blade_data['r/R'], fp=self.blade_data['BE']))
-            skew = tot_skew * roR
-            r = roR * self.radius
-
-            prof_xyz = funcs.generate_3D_profile_points(nondim_xy_coords=nondim_coords, radius=r, axis_shift=0.25,
-                                                        chord_len=chord, beta_deg=beta, skew_deg=skew)
-            self.blade_xyz_profiles[i] = prof_xyz
-
-        # now save them all for loading later
-        for key, val in self.blade_xyz_profiles.items():
-            savepath = os.path.join(self.bld_prof_folder, 'profile_{}.txt'.format(key))
-            xpts, ypts, zpts = val
-            with open(savepath, 'w') as f:
-                f.write('x, y, z\n')
-                for xp, yp, zp in zip(xpts, ypts, zpts):
-                    f.write('{:.6f}, {:.6f}, {:.6f}\n'.format(xp, yp, zp))
-
-    def get_xrotor_output_text(self):
-        line_num = 0
-        txt = ''
-        with open(self.xrop_file, 'r') as f:
-            while line_num < 16:
-                txt += f.readline()
-                line_num += 1
-        return txt
-
-    def plot_design_point_panel(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
-                                input_stations: bool = True, interp_profiles: bool = True, savefig: bool = False,
-                                fig=None):
-        if fig is None:
-            created_from_ui = False
-            radial_axes = {'': None, 'c/R': None, 'beta(deg)': None, 'CL': None, 'CD': None,
-                           'thrust_eff': None, 'RE': None, 'Mach': None, 'effi': None, 'effp': None,
-                           'GAM': None, 'Ttot': None, 'Ptot': None, 'VA/V': None, 'VT/V': None}
-            gs = gridspec.GridSpec(nrows=10, ncols=5, figure=fig)
-            fig = plt.figure(figsize=(18, 10))
-            ax3d = fig.add_subplot(gs[0:7, 0:2], projection='3d')
-            txt_ax = fig.add_subplot(gs[7:10, 0:2])
-
-            for i, p in enumerate(radial_axes):
-                row = i % 5
-                col = int(i / 5) + 2
-                if col == 2:
-                    ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
-                else:
-                    ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
-                radial_axes[p] = ax
-                ax.grid(True)
-                ax.set_ylabel(p)
-                if row == 4:
-                    ax.set_xlabel('r/R')
-                if p == '':
-                    ax.set_visible(False)
-        else:  # fig is not None -> we were passed a Figure object from a UI class
-            created_from_ui = True
-            ax3d = fig.axes[0]
-            txt_ax = fig.axes[1]
-            radial_axes = {'': fig.axes[2], 'c/R': fig.axes[3], 'beta(deg)': fig.axes[4], 'CL': fig.axes[5], 'CD': fig.axes[6],
-                           'thrust_eff': fig.axes[7], 'RE': fig.axes[8], 'Mach': fig.axes[9], 'effi': fig.axes[10], 'effp': fig.axes[11],
-                           'GAM': fig.axes[12], 'Ttot': fig.axes[13], 'Ptot': fig.axes[14], 'VA/V': fig.axes[15], 'VT/V': fig.axes[16]}
-
-
-        ax3d.set_xlabel('X')
-        ax3d.set_ylabel('Y')
-        ax3d.set_zlabel('Z')
-
-        title_txt = 'Propeller Geometry - {}'.format(self.name)
-        ax3d.set_title(title_txt)
-
-        def do_ax3d():
-            blades = np.arange(self.xrotor_d['Nblds'])
-            angles = 360 / self.xrotor_d['Nblds'] * blades
-
-            # plot le and te lines
-            if LE:
-                for ang in angles:
-                    le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
-                    le_line, = ax3d.plot3D(xs=[pt[0] for pt in le_pts], ys=[pt[1] for pt in le_pts],
-                                           zs=[pt[2] for pt in le_pts], c='k', lw=2)
-            else:
-                le_line = None
-
-            if TE:
-                for ang in angles:
-                    le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
-                    te_line, = ax3d.plot3D(xs=[pt[0] for pt in te_pts], ys=[pt[1] for pt in te_pts],
-                                           zs=[pt[2] for pt in te_pts], c='k', ls='-.', lw=2)
-            else:
-                te_line = None
-
-            # plot stations
-            if chords_betas:
-                for ang in angles:
-                    chordlines = self.get_blade_chordlines(rotate_deg=ang)
-                    for line in chordlines:
-                        xs, ys, zs = zip(*line)
-                        station_line, = ax3d.plot3D(xs=xs, ys=ys, zs=zs, c='rosybrown', lw=1, ls='--')
-            else:
-                station_line = None
-
-            # plot station_params
-            if input_stations:
-                radii = self.xrotor_d['r/R'] * self.radius
-                chords = self.xrotor_d['C/R'] * self.radius
-                betas = self.xrotor_d['Beta0deg'].copy()
-                for roR, foil_name in self.station_params.items():
-                    # station dimensionalized parameters
-                    r = roR * self.radius
-                    ch = np.interp(r, radii, chords)
-                    beta = np.interp(r, radii, betas)
-                    sk = self.geo_params['tot_skew'] * roR
-
-                    # load the foil, shift, flip, and dimensionalize coordinates
-                    foil = Airfoil(foil_name, verbose=False)
-                    xc, yc, zc = funcs.generate_3D_profile_points(nondim_xy_coords=foil.get_coords(), radius=r,
-                                                                  axis_shift=0.25, chord_len=ch, beta_deg=beta,
-                                                                  skew_deg=sk)
-                    foils_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='red', alpha=0.7, lw=1)
-            else:
-                foils_line = None
-
-            # plot interpolated profiles
-            if interp_profiles:
-                for prof_num, prof_xyz in self.blade_xyz_profiles.items():
-                    xc, yc, zc = prof_xyz
-                    prof_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='maroon', lw=1, alpha=0.7)
-            else:
-                prof_line = None
-
-            # plot hub
-            if hub:
-                hub_thickness = abs(max([pt[2] for pt in le_pts]) - min([pt[2] for pt in te_pts]))
-                theta = np.linspace(0, np.pi * 2, 50)
-                hub_x = np.cos(theta) * self.hub_radius
-                hub_y = np.sin(theta) * self.hub_radius
-                top_zs = np.ones(len(hub_x)) * hub_thickness / 2
-                bot_zs = -np.ones(len(hub_x)) * hub_thickness / 2
-                hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=top_zs, c='gray', lw=2)
-                hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=bot_zs, c='gray', lw=2)
-            else:
-                hub_line = None
-
-            # set square axes and finish up formatting stuff
-            lim = (-self.radius * 0.65, self.radius * 0.65)
-            ax3d.set_xlim(lim)
-            ax3d.set_ylim(lim)
-            ax3d.set_zlim(lim)
-            leg_handles = [le_line, te_line, hub_line, foils_line, station_line, prof_line]
-            leg_labels = ['L.E.', 'T.E.', 'Hub', 'Input Stations', 'XROTOR Stations', 'Interpolated Geom.']
-
-            leg_labels = [leg_labels[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
-            leg_handles = [leg_handles[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
-            ax3d.legend(leg_handles, leg_labels, loc='upper left', bbox_to_anchor=(1.05, 1.0))
-
-        def do_txt_ax():
-            txt_ax.text(x=0.0, y=0.5, s=self.get_xrotor_output_text(), ha='left', va='center', fontfamily='consolas')
-            txt_ax.axis('off')
-
-        def do_radial_axes():
-            xdata = self.xrotor_op_dict['r/R']
-            for ylbl, ax in radial_axes.items():
-                if ylbl in self.blade_data:
-                    ax.plot(xdata, self.blade_data[ylbl], marker='*', markersize=4)
-                else:
-                    if ylbl in self.xrotor_op_dict:
-                        ax.plot(xdata, self.xrotor_op_dict[ylbl], marker='o', markersize=3)
-
-        def do_thrust_eff_ax():
-            ax = radial_axes['thrust_eff']
-            ax.set_ylabel('')
-            ax.grid(False)
-            thrust_eff = self.xrotor_op_dict['thrust(N)'] / self.xrotor_op_dict['power(W)']
-            txt1 = 'Thrust Efficiency:\n\n\n\n\nNewtons / Watt'
-            ax.text(x=0.5, y=0.5, s=txt1, ha='center', va='center')
-            txt2 = '{:.3f}'.format(thrust_eff)
-            ax.text(x=0.5, y=0.5, s=txt2, ha='center', va='center', fontsize=12, fontweight='bold')
-            ax.axis('off')
-
-            # disk loading metric
-            ax.text(x=-0.3, y=0.5, s='Disk Loading:\n\n\n\n\nNewtons / Meter^2', ha='center', va='center')
-            ax.text(x=-0.3, y=0.5, s='{:.3f}'.format(self.disk_loading), ha='center', va='center',
-                    fontsize=12, fontweight='bold')
-
-        do_ax3d()
-        do_txt_ax()
-        do_radial_axes()
-        do_thrust_eff_ax()
-        wsp = 0.60 if created_from_ui else 0.35
-        fig.subplots_adjust(left=0.05, bottom=0.08, right=0.95, top=0.94, wspace=wsp, hspace=0.5)
-
-        if savefig:
-            savepath = os.path.join(os.getcwd(), '{}.png'.format(ax3d.get_title()))
-            fig.savefig(savepath)
-            Info('Saved PNG to "{}"'.format(savepath))
-
-        return fig
-
-    def plot_mpl3d_geometry(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
-                            input_stations: bool = True, interp_profiles: bool = True, savefig: bool = False, fig=None):
-        if fig is not None:
-            ax3d = fig.axes[0]
-            leg_anchor = (-0.15, 1.0)
-        else:
-            fig = plt.figure(figsize=[13, 10])
-            ax3d = fig.add_subplot(111, projection='3d')
-            leg_anchor = (0.90, 1.0)
-
-        ax3d.set_xlabel('X')
-        ax3d.set_ylabel('Y')
-        ax3d.set_zlabel('Z')
-
-        title_txt = 'Propeller Geometry - {}'.format(self.name)
-        ax3d.set_title(title_txt)
-
-        blades = np.arange(self.xrotor_d['Nblds'])
-        angles = 360 / self.xrotor_d['Nblds'] * blades
-
-        # plot le and te lines
-        if LE:
-            for ang in angles:
-                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
-                le_line, = ax3d.plot3D(xs=[pt[0] for pt in le_pts], ys=[pt[1] for pt in le_pts],
-                                       zs=[pt[2] for pt in le_pts], c='k', lw=2)
-        else:
-            le_line = None
-
-        if TE:
-            for ang in angles:
-                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
-                te_line, = ax3d.plot3D(xs=[pt[0] for pt in te_pts], ys=[pt[1] for pt in te_pts],
-                                       zs=[pt[2] for pt in te_pts], c='k', ls='-.', lw=2)
-        else:
-            te_line = None
-
-        # plot stations
-        if chords_betas:
-            for ang in angles:
-                chordlines = self.get_blade_chordlines(rotate_deg=ang)
-                for line in chordlines:
-                    xs, ys, zs = zip(*line)
-                    station_line, = ax3d.plot3D(xs=xs, ys=ys, zs=zs, c='rosybrown', lw=1, ls='--')
-        else:
-            station_line = None
-
-        # plot station_params
-        if input_stations:
-            radii = self.xrotor_d['r/R'] * self.radius
-            chords = self.xrotor_d['C/R'] * self.radius
-            betas = self.xrotor_d['Beta0deg'].copy()
-            for roR, foil_name in self.station_params.items():
-                # station dimensionalized parameters
-                r = roR * self.radius
-                ch = np.interp(r, radii, chords)
-                beta = np.interp(r, radii, betas)
-                sk = self.geo_params['tot_skew'] * roR
-
-                # load the foil, shift, flip, and dimensionalize coordinates
-                foil = Airfoil(foil_name, verbose=False)
-                xc, yc, zc = funcs.generate_3D_profile_points(nondim_xy_coords=foil.get_coords(), radius=r,
-                                                              axis_shift=0.25, chord_len=ch, beta_deg=beta,
-                                                              skew_deg=sk)
-                foils_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='red', alpha=0.7, lw=1)
-        else:
-            foils_line = None
-
-        # plot interpolated profiles
-        if interp_profiles:
-            for prof_num, prof_xyz in self.blade_xyz_profiles.items():
-                xc, yc, zc = prof_xyz
-                prof_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='maroon', lw=1, alpha=0.7)
-        else:
-            prof_line = None
-
-        # plot hub
-        if hub:
-            hub_thickness = abs(max([pt[2] for pt in le_pts]) - min([pt[2] for pt in te_pts]))
-            theta = np.linspace(0, np.pi * 2, 50)
-            hub_x = np.cos(theta) * self.hub_radius
-            hub_y = np.sin(theta) * self.hub_radius
-            top_zs = np.ones(len(hub_x)) * hub_thickness / 2
-            bot_zs = -np.ones(len(hub_x)) * hub_thickness / 2
-            hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=top_zs, c='gray', lw=2)
-            hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=bot_zs, c='gray', lw=2)
-        else:
-            hub_line = None
-
-        # set square axes and finish up formatting stuff
-        lim = (-self.radius * 0.65, self.radius * 0.65)
-        ax3d.set_xlim(lim)
-        ax3d.set_ylim(lim)
-        ax3d.set_zlim(lim)
-        leg_handles = [le_line, te_line, hub_line, foils_line, station_line, prof_line]
-        leg_labels = ['L.E.', 'T.E.', 'Hub', 'Input Stations', 'XROTOR Stations', 'Interpolated Geom.']
-
-        leg_labels = [leg_labels[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
-        leg_handles = [leg_handles[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
-        ax3d.legend(leg_handles, leg_labels, loc='upper left', bbox_to_anchor=leg_anchor)
-
-        return fig
-
-    def plot_gl3d_geometry(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
-                            input_stations: bool = True, interp_profiles: bool = True, view=None):
-        if view is None:
-            pg.mkQApp()
-            self.gl_geo_view = view = gl.GLViewWidget()
-            view.setFixedSize(1280, 720)
-            view.show()
-        else:
-            pass
-
-        blades = np.arange(self.xrotor_d['Nblds'])
-        angles = 360 / self.xrotor_d['Nblds'] * blades
-
-        # plot le and te lines
-        if LE:
-            for ang in angles:
-                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
-                le_line = gl.GLLinePlotItem(pos=le_pts, color=[0.5, 0.5, 0.5, 1.0], width=2, antialias=False,
-                                            mode='line_strip', glOptions='opaque')
-                view.addItem(le_line)
-
-        if TE:
-            for ang in angles:
-                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
-                te_line = gl.GLLinePlotItem(pos=te_pts, color=[0.5, 0.5, 0.5, 1.0], width=2, antialias=False,
-                                            mode='line_strip', glOptions='opaque')
-                view.addItem(te_line)
-
-        # plot stations
-        if chords_betas:
-            for ang in angles:
-                chordlines = self.get_blade_chordlines(rotate_deg=ang)
-                for line in chordlines:
-                    station_line = gl.GLLinePlotItem(pos=line, color=[i / 255 for i in [245, 66, 66, 255]],
-                                                     width=2, antialias=False, mode='line_strip', glOptions='opaque')
-                    view.addItem(station_line)
-
-        # plot station_params
-        if input_stations:
-            radii = self.xrotor_d['r/R'] * self.radius
-            chords = self.xrotor_d['C/R'] * self.radius
-            betas = self.xrotor_d['Beta0deg'].copy()
-            for roR, foil_name in self.station_params.items():
-                # station dimensionalized parameters
-                r = roR * self.radius
-                ch = np.interp(r, radii, chords)
-                beta = np.interp(r, radii, betas)
-                sk = self.geo_params['tot_skew'] * roR
-
-                # load the foil, shift, flip, and dimensionalize coordinates
-                foil = Airfoil(foil_name, verbose=False)
-                xc, yc, zc = funcs.generate_3D_profile_points(nondim_xy_coords=foil.get_coords(), radius=r,
-                                                              axis_shift=0.25, chord_len=ch, beta_deg=beta,
-                                                              skew_deg=sk)
-                coords = list(zip(xc, yc, zc))
-                foils_line = gl.GLLinePlotItem(pos=coords, color=[i / 255 for i in [5, 0, 163, 255]], width=2, antialias=False,
-                                               mode='line_strip', glOptions='opaque')
-                view.addItem(foils_line)
-
-        # plot interpolated profiles
-        if interp_profiles:
-            for prof_num, prof_xyz in self.blade_xyz_profiles.items():
-                xc, yc, zc = prof_xyz
-                coords = list(zip(xc, yc, zc))
-                prof_line = gl.GLLinePlotItem(pos=coords, color=[i / 255 for i in [163, 0, 0, 200]], width=2,
-                                              antialias=False, mode='line_strip', glOptions='opaque')
-                view.addItem(prof_line)
-
-        # plot hub
-        if hub:
-            hub_thickness = abs(max([pt[2] for pt in le_pts]) - min([pt[2] for pt in te_pts]))
-            theta = np.linspace(0, np.pi * 2, 50)
-            hub_x = np.cos(theta) * self.hub_radius
-            hub_y = np.sin(theta) * self.hub_radius
-            top_zs = np.ones(len(hub_x)) * hub_thickness / 2
-            bot_zs = -np.ones(len(hub_x)) * hub_thickness / 2
-            hub_line = gl.GLLinePlotItem(pos=list(zip(hub_x, hub_y, top_zs)), color=[0.5, 0.5, 0.5, 1.0], width=2,
-                                         antialias=False, mode='line_strip', glOptions='opaque')
-            view.addItem(hub_line)
-            hub_line_bot = gl.GLLinePlotItem(pos=list(zip(hub_x, hub_y, bot_zs)), color=[0.5, 0.5, 0.5, 1.0], width=2,
-                                                          antialias=False, mode='line_strip', glOptions='opaque')
-            view.addItem(hub_line_bot)
-
-        # finish up formatting stuff
-        lim = self.radius * 2.5
-        view.setCameraPosition(distance=lim, azimuth=-90)
-        zgrid = gl.GLGridItem()
-        zgrid.setSize(2, 2, 2)
-        zgrid.setSpacing(.2, .2, .2)
-        zgrid.translate(0, 0, -0.5)
-        view.addItem(zgrid)
-
-        return view
-
-    def plot_gl3d_wvel_data(self, total: bool = True, axial: bool = False, tangential: bool = False, view=None,
-                            plot_every: int = 3):
-        if view is None:
-            pg.mkQApp()
-            self.gl_wvel_view = view = gl.GLViewWidget()
-            view.setFixedSize(1280, 720)
-            view.show()
-        else:
-            pass
-
-        blades = np.arange(self.xrotor_d['Nblds'])
-        angles = 360 / self.xrotor_d['Nblds'] * blades
-
-        self.gl3d_wvel_view = view = self.plot_gl3d_geometry(view=view)
-
-        # plot vel vectors
-        q_chord_pts = self.get_blade_quarter_chords()
-        assert len(self.blade_data['r/R']) == len(q_chord_pts)
-        for i, pt in enumerate(q_chord_pts):
-            if i % plot_every == 0:
-                va = self.blade_data['VA'][i]
-                vt = self.blade_data['VT'][i]
-                vd = self.blade_data['VD'][i]
-                if total:
-                    vector_root = pt
-                    vector_tip = pt[0] - vd, pt[1] + vt, pt[2] - va
-                    vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3)
-                if axial:
-                    vector_root = pt
-                    vector_tip = pt[0], pt[1], pt[2] - va
-                    vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3, color=(.05, .65, .13, 1))
-                if tangential:
-                    vector_root = pt
-                    vector_tip = pt[0], pt[1] + vt, pt[2]
-                    vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3, color=(.92, .84, .2, 1))
-
-        return view
-
-    def generate_stl_geometry(self, plot_after: bool = True, verbose: bool = True):
-        n_prof = len(self.blade_xyz_profiles)
-        n_pts = np.max(np.shape(self.blade_xyz_profiles[0]))
-        n_main_surf = (n_prof - 1) * 2 * (n_pts - 1)
-        n_root = n_pts - 3
-        n_tip = n_pts - 3
-        n_tri = n_main_surf + n_root + n_tip
-
-        mdata = np.zeros(n_tri, dtype=mesh.Mesh.dtype)
-
-        tri_idx = 0
-
-        # root profile
-        vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[0])  # outwards
-        # vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[0], reverse_order=True)  # inwards
-        for vec in vectors:
-            mdata['vectors'][tri_idx] = np.array(vec)
-            tri_idx += 1
-
-        # tip profile
-        vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[n_prof - 1], reverse_order=True)    # outwards
-        # vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[n_prof - 1])    # inwards
-        for vec in vectors:
-            mdata['vectors'][tri_idx] = np.array(vec)
-            tri_idx += 1
-
-        # iterate over the profiles
-        for k in range(n_prof - 1):
-            xyz_prof = self.blade_xyz_profiles[k]
-            nxt_prof = self.blade_xyz_profiles[k + 1]
-
-            # inter-profile surfaces
-            for i in range(n_pts - 1):  # right hand rule to get normal direction correct
-                a = xyz_prof[:, i]  # a is a point-coordinate in (x, y, z) format
-                b = nxt_prof[:, i]  # same for b-f
-                c = nxt_prof[:, i + 1]
-                d = a.copy()
-                e = c.copy()
-                f = xyz_prof[:, i + 1]
-
-                # outwards
-                mdata['vectors'][tri_idx] = np.array([a, b, c])      # populate the array of triangle vectors
-                mdata['vectors'][tri_idx + 1] = np.array([d, e, f])  # going in order, 2 triangles per iteration
-
-                # inwards
-                # mdata['vectors'][tri_idx] = np.array([c, b, a])      # populate the array of triangle vectors
-                # mdata['vectors'][tri_idx + 1] = np.array([f, e, d])  # going in order, 2 triangles per iteration
-
-                tri_idx += 2
-
-        m = mesh.Mesh(mdata)
-
-        if os.path.exists(self.stl_fpath):
-            os.remove(self.stl_fpath)
-        m.save(filename=self.stl_fpath)
-
-        self.stl_mesh = mesh.Mesh.from_file(self.stl_fpath)
-        if verbose:
-            Info('Saved STL file and reloaded into propeller object: "{}"'.format(self.stl_fpath))
-
-        if plot_after:
-            self.plot_stl_mesh()
-
-    def load_stl_geometry(self, verbose: bool = True):
-        if os.path.exists(self.stl_fpath):
-            self.stl_mesh = mesh.Mesh.from_file(self.stl_fpath)
-            if verbose:
-                Info('Loaded STL mesh data from file: {}'.format(self.stl_fpath))
-        else:
-            if verbose:
-                Warning('STL file does not exist, use "generate_stl_geometry()" first')
-
-    def plot_stl_mesh(self):
-        if not hasattr(self, 'stl_view'):
-            pg.mkQApp()
-            self.stl_view = gl.GLViewWidget()
-        view = self.stl_view
-        view.clear()
-        view.setFixedSize(1280, 720)
-        view.show()
-
-        grid = gl.GLGridItem()
-        grid.scale(self.radius / 10, self.radius / 10, self.radius / 10)
-        grid.translate(dx=0, dy=0, dz=-self.radius / 4)
-        view.addItem(grid)
-        view.setCameraPosition(distance=self.radius * 1.5, elevation=10, azimuth=-70)
-
-        md = gl.MeshData(vertexes=self.stl_mesh.vectors.copy())
-        mesh_itm = gl.GLMeshItem(meshdata=md, color=[0, 0, .7, 1], edgeColor=[.5, .5, .5, 1], drawEdges=False, drawFaces=True,
-                                 shader='normalColor', smooth=False)
-        mesh_itm.translate(dx=-0.5 * self.radius, dy=0, dz=0)
-        view.addItem(mesh_itm)
-
-        return view
-
-    def plot_ideal_eff(self):
-        Info('"{}" ideal efficiency: {:.1f}%'.format(self.name, self.ideal_eff))
-        return
-
-    def analyze_operating_point(self, velo: float = None, adva: float = None, rpm: float = None, thrust: float = None,
-                                power: float = None, torque: float = None, xrotor_verbose: bool = False):
-
-        funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=self.design_vorform, adva=adva, rpm=rpm, thrust=thrust,
-                              torque=torque, power=power, velo=velo, xrotor_verbose=xrotor_verbose)
-
-    def analyze_sweep(self, velo_vals: list, sweep_param: str, sweep_vals: list, verbose: bool = True,
-                      xrotor_verbose: bool = False, vorform: str = None, prog_signal=None):
-        if sweep_param not in ['adva', 'rpm', 'thrust', 'power', 'torque']:
-            raise Error('"sweep_param" must be one of ("adva", "rpm", "thrust", "power", "torque")')
-
-        vorform = self.design_vorform if vorform is None else vorform
-
-        total_pnts = len(velo_vals) * len(sweep_vals)
-        if verbose:
-            info_str = 'Analyzing "{}" across a sweep of {} operating points'.format(self.name, total_pnts)
-            if prog_signal is not None:
-                prog_signal.emit(0, [info_str])
-            else:
-                Info(info_str)
-        count = 0
-        for velo_val in velo_vals:
-            for v, val in enumerate(sweep_vals):
-                count += 1
-                if verbose:
-                    info_str = 'Analyzing sweep point # {} / {}'.format(count, total_pnts)
-                    if prog_signal is not None:
-                        prog_signal.emit(count / total_pnts * 100, [info_str])
-                    else:
-                        Info(info_str)
-                try:
-                    funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=vorform, velo=velo_val, verbose=False,
-                                          xrotor_verbose=xrotor_verbose, **{sweep_param: val})
-                except Error as e:
-                    warn_str = 'Failed to get XROTOR oper results for vel={}, {}={}\n{}'.format(velo_val, sweep_param, val, e)
-                    if prog_signal is not None:
-                        prog_signal.emit(None, [warn_str])
-                    else:
-                        Warning(warn_str)
-                        pass
-
-        self.oper_data.load_oper_sweep_results()
-        self.wvel_data.load_wvel_sweep_results()
-        if verbose:
-            if prog_signal is not None:
-                prog_signal.emit(0, 'Done!')
-            else:
-                Info('Done!')
-
-    def clear_sweep_data(self):
-        if os.path.exists(self.oper_data_dir):
-            shutil.rmtree(self.oper_data_dir)
-            Info('Removed {} and its contents'.format(self.oper_data_dir))
-        if os.path.exists(self.wvel_data_dir):
-            shutil.rmtree(self.wvel_data_dir)
-            Info('Removed {} and its contents'.format(self.wvel_data_dir))
-
-
-class PropellerOperData:
-    def __init__(self, directory: str):
-        self.directory = directory
-        self.datapoints = {}
-        self.prop_name = os.path.split(os.path.split(self.directory)[0])[1]
-
-    def __len__(self):
-        return len(self.datapoints)
-
-    def get_swept_params(self):
-        valid_params = VALID_OPER_PLOT_PARAMS
-        swept_params = []
-        avoid_params = []
-        for param in valid_params:
-            for dp in self.datapoints.values():
-                if param not in swept_params:
-                    pts = self.get_datapoints_by_paramval(param=param, val=dp[param])
-                    if 2 < len(pts) < len(self.datapoints) and param not in avoid_params:
-                        swept_params.append(param)
-                    else:
-                        avoid_params.append(param)
-
-        return swept_params
-
-    def get_oper_files(self, fullpath: bool = True):
-        if os.path.exists(self.directory):
-            if fullpath:
-                return [os.path.join(self.directory, name) for name in os.listdir(self.directory) if name.endswith('.oper')]
-            else:
-                return [name for name in os.listdir(self.directory) if name.endswith('.oper')]
-        else:
-            return []
-
-    def load_oper_sweep_results(self, verbose: bool = True):
-        self.datapoints = d = {}
-        fnames = self.get_oper_files(fullpath=False)
-        for fname in fnames:
-            vel_key, rpm_key = [float(num) for num in fname.strip('velo_').strip('.oper').split('_rpm_')]
-            vel_key /= 100
-            oper_fullpath = os.path.join(self.directory, fname)
-            d[(vel_key, rpm_key)] = funcs.read_xrotor_op_file(fpath=oper_fullpath)
-        if verbose and len(fnames) > 0:
-            Info('Loaded Existing Oper Results (.oper)!', indent_level=1)
-
-    def get_unique_param(self, param: str):
-        uniq_vals = []
-        for val in self.datapoints.values():
-            if val[param] not in uniq_vals:
-                uniq_vals.append(val[param])
-        return list(sorted(uniq_vals))
-
-    def get_datapoints_by_paramval(self, param: str, val: Union[float, int]):
-        pnts = []
-        for key, dp in self.datapoints.items():
-            if dp[param] == val:
-                pnts.append(dp)
-        return pnts
-
-    def plot(self, x_param: str, y_param: str, family_param: str = None, iso_param: str = None, fig=None, **plot_kwargs):
-        params = [x_param, y_param, family_param, iso_param]
-        valid_params = VALID_OPER_PLOT_PARAMS
-        valid_params_lower = [s.lower() for s in valid_params]
-
-        if len(self.datapoints) == 0:
-            return
-
-        for i, param in enumerate(params):
-            if param is not None:
-                if param.lower() in valid_params_lower:
-                    params[i] = valid_params[valid_params_lower.index(param.lower())]
-                if param.lower() in ['adv', 'adv.', 'adva', 'adv. ratio', 'adv.ratio']:
-                    params[i] = 'adv. ratio'
-                elif param.lower() in ['speed', 'speed(m/s)', 'vel', 'velocity', 'speed_mps']:
-                    params[i] = 'speed(m/s)'
-                elif param.lower() in ['thrust', 'thrust(n)', 'thrust (n)']:
-                    params[i] = 'thrust(N)'
-                elif param.lower() in ['power', 'power(w)', 'power (w)']:
-                    params[i] = 'power(W)'
-                elif param.lower() in ['torque(n-m)', 'torque', 'torque (n-m)']:
-                    params[i] = 'torque(N-m)'
-                elif param.lower() in ['eff', 'efficiency', 'Efficiency']:
-                    params[i] = 'Efficiency'
-                elif param.lower() in ['pvisc(w)', 'pvisc (w)', 'pvisc']:
-                    params[i] = 'Pvisc(W)'
-            else:
-                params[i] = None
-
-        x_param, y_param, family_param, iso_param = params
-
-        if x_param not in valid_params:
-            raise Error('x_param "{}" is not one of the valid params ({})'.format(x_param, valid_params))
-        if y_param not in valid_params:
-            raise Error('y_param "{}" is not one of the valid params ({})'.format(y_param, valid_params))
-        if family_param not in valid_params and family_param is not None:
-            raise Error('family_param error, must be one of {}'.format(valid_params))
-        if iso_param not in valid_params and iso_param is not None:
-            raise Error('iso_param error, must be one of {}'.format(valid_params))
-
-        if fig is None:
-            fig = plt.figure(figsize=[10, 8])
-            ax = fig.add_subplot(111)
-        else:
-            ax = fig.axes[0]
-
-        ax.grid(True)
-        ax.set_title('{} Sweep Results'.format(self.prop_name))
-        ax.set_xlabel(x_param)
-        ax.set_ylabel(y_param)
-
-        if family_param is not None:
-            fvals = self.get_unique_param(param=family_param)
-            for fval in fvals:
-                datapts = self.get_datapoints_by_paramval(param=family_param, val=fval)
-                xvals = [dp[x_param] for dp in datapts]
-                yvals = [dp[y_param] for dp in datapts]
-                xvals, yvals = zip(*sorted(zip(xvals, yvals)))
-                ax.plot(xvals, yvals, '-o', label='{}'.format(fval))
-
-            if iso_param is not None:
-                ivals = self.get_unique_param(param=iso_param)
-                for ival in ivals:
-                    datapts = self.get_datapoints_by_paramval(param=iso_param, val=ival)
-                    if len(datapts) > 1:
-                        xvals = [dp[x_param] for dp in datapts]
-                        yvals = [dp[y_param] for dp in datapts]
-                        xvals, yvals = zip(*sorted(zip(xvals, yvals)))
-                        ax.plot(xvals, yvals, '--', label='{}'.format(ival))
-
-            leg_title = '{} /\n{}'.format(family_param, iso_param) if iso_param is not None else '{}'.format(family_param)
-            ax.legend(title=leg_title, loc='best')
-        else:
-            datapts = self.datapoints.values()
-            xvals = [dp[x_param] for dp in datapts]
-            yvals = [dp[y_param] for dp in datapts]
-            xvals, yvals = zip(*sorted(zip(xvals, yvals)))
-            ax.plot(xvals, yvals, 'o')
-
-        return fig
-
-
-class PropellerWVelData:
-    def __init__(self, directory: str):
-        self.directory = directory
-        self.datapoints = {}
-        self.prop_name = os.path.split(os.path.split(self.directory)[0])[1]
-
-    def __len__(self):
-        return len(self.datapoints)
-
-    def get_wvel_files(self, fullpath: bool = True):
-        if os.path.exists(self.directory):
-            if fullpath:
-                return [os.path.join(self.directory, name) for name in os.listdir(self.directory) if name.endswith('.wvel')]
-            else:
-                return [name for name in os.listdir(self.directory) if name.endswith('.wvel')]
-        else:
-            return []
-
-    def load_wvel_sweep_results(self, verbose: bool = True):
-        self.datapoints = d = {}
-        fnames = self.get_wvel_files(fullpath=False)
-        for fname in fnames:
-            vel_key, rpm_key = [float(num) for num in fname.strip('velo_').strip('.wvel').split('_rpm_')]
-            vel_key /= 100
-            wvel_fullpath = os.path.join(self.directory, fname)
-            d[(vel_key, rpm_key)] = funcs.read_xrotor_wvel_file(fpath=wvel_fullpath)
-        if verbose and len(fnames) > 0:
-            Info('Loaded Existing WVel Results (.wvel)!', indent_level=1)
+import os
+import shutil
+from propeller_design_tools import funcs
+from propeller_design_tools.user_io import Info, Error, Warning
+from propeller_design_tools.settings import get_setting
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+from propeller_design_tools.custom_opengl_classes import Custom3DArrow
+import matplotlib.pyplot as plt
+import matplotlib.gridspec as gridspec
+from mpl_toolkits import mplot3d
+import numpy as np
+from stl import mesh
+from typing import Union
+import pyqtgraph as pg
+import pyqtgraph.opengl as gl
+
+
+class Propeller(object):
+
+    creation_attrs = {'nblades': int, 'radius': float, 'hub_radius': float, 'hub_wake_disp_br': float,
+                      'design_speed_mps': float, 'design_adv': float, 'design_rpm': float, 'design_thrust': float,
+                      'design_power': float, 'design_cl': dict, 'design_atmo_props': dict, 'design_vorform': str,
+                      'station_params': dict, 'station_polars': list, 'geo_params': dict}
+    saveload_attrs = {**creation_attrs, **{'name': str, 'meta_file': str, 'xrr_file': str, 'xrop_file': str,
+                                           'blade_data': dict, 'blade_xyz_profiles': dict}}
+
+    def __init__(self, name, verbose: bool = True, **kwargs):
+        # name is always given, detect if it's a filepath
+        self.savepath = None
+        if os.path.exists(name):
+            self.savepath, name = os.path.split(name)
+        self.name = name.replace('.txt', '')
+        self.oper_data = None
+        self.wvel_data = None
+        self.stl_mesh = None
+
+        # check if the prop db exists
+        prop_db = get_setting('propeller_database')
+        if prop_db is None:
+            raise Error(s='No Propeller Database is set!  First set one with "pdt.set_propeller_database(str)".')
+
+        # initialize all attrs to None for script auto-completion detection
+        self.nblades, self.radius, self.hub_radius, self.hub_wake_disp_br, self.design_speed_mps, self.design_adv, \
+        self.design_rpm, self.design_thrust, self.design_power, self.design_cl, self.design_atmo_props, \
+        self.design_vorform, self.station_params, self.geo_params, self.xrotor_d, self.xrotor_op_dict, \
+        self.blade_data, self.blade_xyz_profiles = [None] * 18
+
+        # if no kwargs were given and there's a meta_file, load it
+        if len(kwargs) == 0:
+            if os.path.exists(self.meta_file):
+                if verbose:
+                    Info(s='Loading propeller "meta-file" ({})'.format(self.meta_file))
+                self.load_from_savefile(verbose=verbose)
+            else:
+                raise FileNotFoundError('Could not find file {}'.format(self.meta_file))
+        else:  # cycle thru kwargs and set if they're valid, if not ignore them
+            for key, val in kwargs.items():
+                if key in self.creation_attrs:
+                    setattr(self, key, val)
+                else:
+                    raise Error('Unknown KWARG input "{}"'.format(key))
+
+        # attempt to load any oper sweep data and any wvel sweep data
+        self.oper_data = PropellerOperData(directory=self.oper_data_dir)
+        self.oper_data.load_oper_sweep_results(verbose=verbose)
+        self.wvel_data = PropellerWVelData(directory=self.wvel_data_dir)
+        self.wvel_data.load_wvel_sweep_results(verbose=verbose)
+
+        # attempt to load any STL mesh data
+        self.load_stl_geometry(verbose=verbose)
+
+    @property
+    def stl_fpath(self):
+        return os.path.join(self.save_folder, '{}.stl'.format(self.name))
+
+    @property
+    def station_polar_folder(self):
+        return os.path.join(self.save_folder, 'station_polars')
+
+    @property
+    def bld_prof_folder(self):
+        return os.path.join(self.save_folder, 'blade_profiles')
+
+    @property
+    def xrr_file(self):
+        return os.path.join(self.save_folder, '{}.xrr'.format(self.name))
+
+    @property
+    def xrop_file(self):
+        return os.path.join(self.save_folder, '{}.xrop'.format(self.name))
+
+    @property
+    def meta_file(self):
+        return os.path.join(self.save_folder, '{}.meta'.format(self.name))
+
+    @property
+    def save_folder(self):
+        if self.savepath is None:
+            return os.path.join(get_setting('propeller_database'), self.name)
+        else:
+            return os.path.join(self.savepath, self.name)
+
+    @property
+    def tot_skew(self):
+        return self.geo_params['tot_skew']
+
+    @property
+    def n_prof_pts(self):
+        return self.geo_params['n_prof_pts']
+
+    @property
+    def n_profs(self):
+        return self.geo_params['n_profs']
+
+    @property
+    def design_rho(self):
+        if 'dens' in self.design_atmo_props:
+            return self.design_atmo_props['dens']
+
+    @design_rho.setter
+    def design_rho(self, value):
+        self.design_atmo_props['dens'] = value
+
+    @property
+    def disk_area_m_sqrd(self):
+        if self.radius is not None and self.hub_radius is not None:
+            return np.pi * (self.radius ** 2 - self.hub_radius ** 2)
+
+    @property
+    def ideal_eff(self):
+        req_attrs = [self.design_thrust, self.design_rho, self.disk_area_m_sqrd, self.design_speed_mps]
+        if all([attr is not None for attr in req_attrs]):
+            return funcs.calc_ideal_eff(*req_attrs)
+
+    @property
+    def disk_loading(self):
+        if self.xrotor_op_dict is not None and self.disk_area_m_sqrd is not None:
+            return self.xrotor_op_dict['thrust(N)'] / self.disk_area_m_sqrd
+
+    @property
+    def oper_data_dir(self):
+        return os.path.join(os.path.split(self.meta_file)[0], 'oper_data')
+
+    @property
+    def wvel_data_dir(self):
+        return os.path.join(os.path.split(self.meta_file)[0], 'wvel_data')
+
+    @property
+    def n_radial(self):
+        return len(self.blade_xyz_profiles)
+
+    @property
+    def valid_oper_plot_params(self):
+        return
+
+    def save_as_new(self, new_name: str):
+        # store filepaths before we change name
+        old_xrop_file = self.xrop_file * 1
+        old_xrr_file = self.xrr_file * 1
+        old_blade_profs_folder = self.bld_prof_folder * 1
+
+        # change the name, make a new directory
+        self.name = new_name
+        if not os.path.exists(self.save_folder):
+            os.mkdir(self.save_folder)
+
+        # save off a new meta file, copy the xrop and xrr files
+        self.save_meta_file()
+        shutil.copyfile(old_xrop_file, self.xrop_file)
+        shutil.copyfile(old_xrr_file, self.xrr_file)
+
+        # blade profiles
+        if not os.path.exists(self.bld_prof_folder):
+            os.mkdir(self.bld_prof_folder)
+        for fname in [f for f in os.listdir(old_blade_profs_folder) if f.endswith('.txt')]:
+            fpath = os.path.join(old_blade_profs_folder, fname)
+            copypath = os.path.join(self.bld_prof_folder, fname)
+            shutil.copyfile(fpath, copypath)
+
+    def read_pdt_metafile(self):
+        # read in the PDT meta-file (in the root propeller database) and set Propeller attrs
+        with open(self.meta_file, 'r') as f:
+            txt = f.read().strip()
+        lines = txt.split('\n')
+
+        blade_data = {}
+        point_cloud = {}
+
+        for line in lines:
+            line_attr, line_val = [i.strip() for i in line.split(':', 1)]
+            if 'blade_data_' in line_attr:
+                blade_data[line_attr.split('blade_data_', 1)[1]] = np.array([float(v) for v in line_val.strip().split(', ')])
+            if 'point_cloud_' in line_attr:
+                point_cloud[line_attr.split('point_cloud_', 1)[1]] = np.array([float(v) for v in line_val.strip().split(', ')])
+            for attr, tipe in self.saveload_attrs.items():
+                if line_attr == attr:
+                    val = line.split(': ', 1)[1]
+                    if val == 'None':
+                        val = None
+                    else:
+                        if tipe is int:
+                            val = int(val)
+                        elif tipe is float:
+                            val = float(val)
+                        elif tipe is dict:
+                            items = [item.split(': ') for item in
+                                     val.replace('{', '').replace('}', '').replace("'", '').split(', ')]
+                            # check for keys that are floats or ints
+                            keys_are_nums = [itm[0].replace('.', '').isnumeric() for itm in items]
+                            if all(keys_are_nums):
+                                for i, itm in enumerate(items):
+                                    new_itm = [float(itm[0]), itm[1]]
+                                    items[i] = new_itm
+                            val = {}
+                            for key, entry in items:
+                                if 'none' == entry.lower():
+                                    entry = None
+                                try:    # try to convert to float
+                                    val[key] = float(entry)
+                                except:     # otherwise store as string
+                                    val[key] = entry
+                        elif tipe is list:
+                            val = []
+                    setattr(self, attr, val)
+        self.set_blade_data(blade_dict=blade_data)
+
+    def read_xrotor_restart(self):
+        with open(self.xrr_file, 'r') as f:
+            txt = f.read().strip()
+        lines = txt.split('\n')
+
+        def read_line_pair(kw_idx):
+            keywords = lines[kw_idx].strip('!').split()
+            values = lines[kw_idx + 1].split()
+            return dict(zip(keywords, values))
+
+        def read_xi_sect(xi_idx):
+            xi_d = {}
+            for lni in [xi_idx, xi_idx + 2, xi_idx + 4, xi_idx + 6, xi_idx + 8]:
+                for k, v in read_line_pair(lni).items():
+                    xi_d[k] = float(v)
+            return xi_d
+
+        def read_geo_stations(header_idx):
+            geo_d = {}
+            headers = lines[header_idx].strip('!').split()
+            for h in headers:
+                geo_d[h] = []
+            for idx in range(header_idx + 1, len(lines)):
+                vals = lines[idx].split()
+                if len(vals) == len(headers):
+                    for i, val in enumerate(vals):
+                        geo_d[headers[i]].append(float(val))
+            return geo_d
+
+        d = {}
+        design_param_lines = [2, 4, 6, 8]
+        for ln_idx in design_param_lines:
+            for k, v in read_line_pair(ln_idx).items():
+                d[k] = float(v)
+
+        xi_lines = [i * 10 for i in range(1, int(d['Naero']) + 1)]   # works out that each xi section is 10 lines, and 1st one on line 10 always
+        for sect_idx, ln_idx in enumerate(xi_lines):
+            xi_d = read_xi_sect(ln_idx)
+            d['Xisection_{}'.format(sect_idx)] = xi_d
+
+        for k, v in read_line_pair(kw_idx=xi_lines[-1] + 10).items():
+            d[k] = v
+
+        for k, v in read_line_pair(kw_idx=xi_lines[-1] + 12).items():
+            d[k] = int(v)
+
+        for k, v in read_geo_stations(header_idx=xi_lines[-1] + 14).items():
+            d[k] = v
+
+        # turn all lists into numpy arrays before returning
+        for key, val in d.items():
+            if isinstance(val, list):
+                d[key] = np.array(val)
+
+        return d
+
+    def load_from_savefile(self, verbose):
+        # 1st set attrs from the PDT metafile
+        self.read_pdt_metafile()
+        if verbose:
+            Info(s='Successfully read meta-file (.meta)!', indent_level=1)
+
+        # set the stations... why did I do it this way??
+        self.set_stations(plot_also=False, verbose=verbose, from_loadsave_file=True)
+        if verbose:
+            Info(s='Successfully read and set station polars!', indent_level=1)
+
+        # then read in the XROTOR restart file (in the xrotor_geometry_files)
+        self.xrotor_d = self.read_xrotor_restart()
+        if verbose:
+            Info(s='Successfully read XROTOR restart file (.xrr)!', indent_level=1)
+
+        # then read the operating point output file (in xrotor_op_files)
+        self.xrotor_op_dict = funcs.read_xrotor_op_file(fpath=self.xrop_file)
+        if verbose:
+            Info(s='Successfully read XROTOR operating-point file (.xrop)!', indent_level=1)
+
+        # and finally read in the point cloud files
+        self.blade_xyz_profiles = {}
+        fnames = funcs.search_files(folder=self.bld_prof_folder)
+        for fname in fnames:
+            prof_num = int(fname.replace('profile_', '').replace('.txt', ''))
+            xyz_prof = funcs.read_profile_xyz(fpath=os.path.join(self.bld_prof_folder, fname))
+            self.blade_xyz_profiles[prof_num] = xyz_prof
+        if verbose:
+            Info(s='Successfully read blade profiles!', indent_level=1)
+
+        return
+
+    def set_stations(self, plot_also: bool = True, verbose: bool = False, from_loadsave_file: bool = False):
+        if not from_loadsave_file:
+            self.stations, txt = funcs.create_radial_stations(prop=self, plot_also=plot_also, verbose=verbose)
+        else:
+            self.stations = funcs.read_radial_stations(prop=self, plot_also=plot_also, verbose=False)
+            txt = ''
+        return txt
+
+    def show_station_fits(self):
+        for st in self.stations:
+            fig = st.plot_xrotor_fit_params()
+
+    def set_blade_data(self, blade_dict: dict):
+        self.blade_data = blade_dict
+        return
+
+    def save_meta_file(self):
+        attrs_2_ignore = ['blade_xyz_profiles', 'meta_file', 'xrr_file', 'xrop_file', 'station_polars']   # ignore the files so that prop_dirs can be switched
+
+        if os.path.exists(self.meta_file):
+            os.remove(self.meta_file)
+
+        with open(self.meta_file, 'w') as f:
+            for attr in [a for a in self.saveload_attrs if a not in attrs_2_ignore]:
+                if attr == 'blade_data':
+                    for key, val in self.blade_data.items():
+                        val = ', '.join([str(i) for i in val])
+                        f.write('{}: {}\n'.format('blade_data_{}'.format(key), val))
+                else:
+                    f.write('{}: {}\n'.format(attr, getattr(self, attr)))
+
+    def save_station_polars(self):
+        if not os.path.exists(self.station_polar_folder):
+            os.mkdir(self.station_polar_folder)
+
+        for i, roR in enumerate(self.station_params.keys()):
+            station = self.stations[i]
+            foil_name = self.station_params[roR]
+            savename = '{}_{}.polar'.format(roR, foil_name)
+            savepath = os.path.join(self.station_polar_folder, savename)
+            with open(savepath, 'w') as f:
+                for key, val in station.foil_polar.items():
+                    if isinstance(val, list) or isinstance(val, np.ndarray):
+                        val = ', '.join([str(v) for v in val])
+                    f.write('{}: {}\n'.format(key, val))
+
+    def get_blade_le_te(self, rotate_deg: float = 0.0, axis_shift: float = 0.25):
+        radii = self.radius * np.array(self.xrotor_d['r/R'])
+        chords = self.radius * np.array(self.xrotor_d['C/R'])
+        betas = np.array(self.xrotor_d['Beta0deg'])
+        le_pts = []
+        te_pts = []
+        for radius, chord, beta in zip(radii, chords, betas):
+            le_te_coords = np.array([[0.0, 1.0], [0.0, 0.0]])
+            xs, ys, zs = funcs.generate_3D_profile_points(nondim_xy_coords=le_te_coords, radius=radius,
+                                                            axis_shift=axis_shift, chord_len=chord, beta_deg=beta,
+                                                            skew_deg=rotate_deg)
+            le_pts.append([xs[0], ys[0], zs[0]])
+            te_pts.append([xs[1], ys[1], zs[1]])
+        return le_pts, te_pts
+
+    def get_blade_quarter_chords(self):  # for plotting of wvel vectors
+        chordlines = self.get_blade_chordlines(rotate_deg=0)
+        q_chord_pts = []
+        for line in chordlines:
+            qtr_idx = int(len(line) / 4)
+            q_chord_pts.append(line[qtr_idx])
+
+        return q_chord_pts
+
+    def get_blade_chordlines(self, rotate_deg: float, axis_shift: float = 0.25, npts: int = 50):
+        radii = self.radius * np.array(self.xrotor_d['r/R'])
+        chords = self.radius * np.array(self.xrotor_d['C/R'])
+        betas = np.array(self.xrotor_d['Beta0deg'])
+        chordlines = []
+        for radius, chord, beta in zip(radii, chords, betas):
+            xs = np.linspace(0, 1, npts)
+            ys = np.zeros(len(xs))
+            chordline_nondim = np.vstack([xs, ys])
+            xs, ys, zs = funcs.generate_3D_profile_points(nondim_xy_coords=chordline_nondim, radius=radius,
+                                                   axis_shift=axis_shift, chord_len=chord, beta_deg=beta,
+                                                   skew_deg=rotate_deg)
+            coords = list(zip(xs, ys, zs))
+            chordlines.append(coords)
+        return chordlines
+
+    def interp_foil_profiles(self, n_prof_pts: int = None, n_profs: int = 50, tot_skew: float = 0.0):
+
+        assert len(self.stations) > 0
+
+        if len(self.stations) != 1:
+            raise Error('> 1 profile interpolation not yet implemented')
+
+        if tot_skew != 0.0:
+            Info('Blade "skew" is not implemented in XROTOR, and therefore not reflected in XROTOR results.\n'
+                 '  > Skew effects are considered negligible for PDT purposes for small enough skew angles.')
+
+        # clear out the existing xyz profiles
+        funcs.delete_files_from_folder(self.bld_prof_folder)
+
+        station = self.stations[0]
+        # nondim_coords = station.foil.get_coords(n_interp=n_prof_pts)
+        nondim_coords = station.foil.get_coords_closed_te(n_interp=n_prof_pts)
+
+        self.blade_xyz_profiles = {}
+        for i, roR in enumerate(np.linspace(self.blade_data['r/R'][0], self.blade_data['r/R'][-1], n_profs)):
+            chord = np.interp(x=roR, xp=self.blade_data['r/R'], fp=self.blade_data['CH']) * self.radius
+            beta = np.rad2deg(np.interp(x=roR, xp=self.blade_data['r/R'], fp=self.blade_data['BE']))
+            skew = tot_skew * roR
+            r = roR * self.radius
+
+            prof_xyz = funcs.generate_3D_profile_points(nondim_xy_coords=nondim_coords, radius=r, axis_shift=0.25,
+                                                        chord_len=chord, beta_deg=beta, skew_deg=skew)
+            self.blade_xyz_profiles[i] = prof_xyz
+
+        # now save them all for loading later
+        for key, val in self.blade_xyz_profiles.items():
+            savepath = os.path.join(self.bld_prof_folder, 'profile_{}.txt'.format(key))
+            xpts, ypts, zpts = val
+            with open(savepath, 'w') as f:
+                f.write('x, y, z\n')
+                for xp, yp, zp in zip(xpts, ypts, zpts):
+                    f.write('{:.6f}, {:.6f}, {:.6f}\n'.format(xp, yp, zp))
+
+    def get_xrotor_output_text(self):
+        line_num = 0
+        txt = ''
+        with open(self.xrop_file, 'r') as f:
+            while line_num < 16:
+                txt += f.readline()
+                line_num += 1
+        return txt
+
+    def plot_design_point_panel(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
+                                input_stations: bool = True, interp_profiles: bool = True, savefig: bool = False,
+                                fig=None):
+        if fig is None:
+            created_from_ui = False
+            radial_axes = {'': None, 'c/R': None, 'beta(deg)': None, 'CL': None, 'CD': None,
+                           'thrust_eff': None, 'RE': None, 'Mach': None, 'effi': None, 'effp': None,
+                           'GAM': None, 'Ttot': None, 'Ptot': None, 'VA/V': None, 'VT/V': None}
+            gs = gridspec.GridSpec(nrows=10, ncols=5, figure=fig)
+            fig = plt.figure(figsize=(18, 10))
+            ax3d = fig.add_subplot(gs[0:7, 0:2], projection='3d')
+            txt_ax = fig.add_subplot(gs[7:10, 0:2])
+
+            for i, p in enumerate(radial_axes):
+                row = i % 5
+                col = int(i / 5) + 2
+                if col == 2:
+                    ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
+                else:
+                    ax = fig.add_subplot(gs[2 * row:2 * row + 2, col])
+                radial_axes[p] = ax
+                ax.grid(True)
+                ax.set_ylabel(p)
+                if row == 4:
+                    ax.set_xlabel('r/R')
+                if p == '':
+                    ax.set_visible(False)
+        else:  # fig is not None -> we were passed a Figure object from a UI class
+            created_from_ui = True
+            ax3d = fig.axes[0]
+            txt_ax = fig.axes[1]
+            radial_axes = {'': fig.axes[2], 'c/R': fig.axes[3], 'beta(deg)': fig.axes[4], 'CL': fig.axes[5], 'CD': fig.axes[6],
+                           'thrust_eff': fig.axes[7], 'RE': fig.axes[8], 'Mach': fig.axes[9], 'effi': fig.axes[10], 'effp': fig.axes[11],
+                           'GAM': fig.axes[12], 'Ttot': fig.axes[13], 'Ptot': fig.axes[14], 'VA/V': fig.axes[15], 'VT/V': fig.axes[16]}
+
+
+        ax3d.set_xlabel('X')
+        ax3d.set_ylabel('Y')
+        ax3d.set_zlabel('Z')
+
+        title_txt = 'Propeller Geometry - {}'.format(self.name)
+        ax3d.set_title(title_txt)
+
+        def do_ax3d():
+            blades = np.arange(self.xrotor_d['Nblds'])
+            angles = 360 / self.xrotor_d['Nblds'] * blades
+
+            # plot le and te lines
+            if LE:
+                for ang in angles:
+                    le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
+                    le_line, = ax3d.plot3D(xs=[pt[0] for pt in le_pts], ys=[pt[1] for pt in le_pts],
+                                           zs=[pt[2] for pt in le_pts], c='k', lw=2)
+            else:
+                le_line = None
+
+            if TE:
+                for ang in angles:
+                    le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
+                    te_line, = ax3d.plot3D(xs=[pt[0] for pt in te_pts], ys=[pt[1] for pt in te_pts],
+                                           zs=[pt[2] for pt in te_pts], c='k', ls='-.', lw=2)
+            else:
+                te_line = None
+
+            # plot stations
+            if chords_betas:
+                for ang in angles:
+                    chordlines = self.get_blade_chordlines(rotate_deg=ang)
+                    for line in chordlines:
+                        xs, ys, zs = zip(*line)
+                        station_line, = ax3d.plot3D(xs=xs, ys=ys, zs=zs, c='rosybrown', lw=1, ls='--')
+            else:
+                station_line = None
+
+            # plot station_params
+            if input_stations:
+                radii = self.xrotor_d['r/R'] * self.radius
+                chords = self.xrotor_d['C/R'] * self.radius
+                betas = self.xrotor_d['Beta0deg'].copy()
+                for roR, foil_name in self.station_params.items():
+                    # station dimensionalized parameters
+                    r = roR * self.radius
+                    ch = np.interp(r, radii, chords)
+                    beta = np.interp(r, radii, betas)
+                    sk = self.geo_params['tot_skew'] * roR
+
+                    # load the foil, shift, flip, and dimensionalize coordinates
+                    foil = Airfoil(foil_name, verbose=False)
+                    xc, yc, zc = funcs.generate_3D_profile_points(nondim_xy_coords=foil.get_coords(), radius=r,
+                                                                  axis_shift=0.25, chord_len=ch, beta_deg=beta,
+                                                                  skew_deg=sk)
+                    foils_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='red', alpha=0.7, lw=1)
+            else:
+                foils_line = None
+
+            # plot interpolated profiles
+            if interp_profiles:
+                for prof_num, prof_xyz in self.blade_xyz_profiles.items():
+                    xc, yc, zc = prof_xyz
+                    prof_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='maroon', lw=1, alpha=0.7)
+            else:
+                prof_line = None
+
+            # plot hub
+            if hub:
+                hub_thickness = abs(max([pt[2] for pt in le_pts]) - min([pt[2] for pt in te_pts]))
+                theta = np.linspace(0, np.pi * 2, 50)
+                hub_x = np.cos(theta) * self.hub_radius
+                hub_y = np.sin(theta) * self.hub_radius
+                top_zs = np.ones(len(hub_x)) * hub_thickness / 2
+                bot_zs = -np.ones(len(hub_x)) * hub_thickness / 2
+                hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=top_zs, c='gray', lw=2)
+                hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=bot_zs, c='gray', lw=2)
+            else:
+                hub_line = None
+
+            # set square axes and finish up formatting stuff
+            lim = (-self.radius * 0.65, self.radius * 0.65)
+            ax3d.set_xlim(lim)
+            ax3d.set_ylim(lim)
+            ax3d.set_zlim(lim)
+            leg_handles = [le_line, te_line, hub_line, foils_line, station_line, prof_line]
+            leg_labels = ['L.E.', 'T.E.', 'Hub', 'Input Stations', 'XROTOR Stations', 'Interpolated Geom.']
+
+            leg_labels = [leg_labels[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
+            leg_handles = [leg_handles[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
+            ax3d.legend(leg_handles, leg_labels, loc='upper left', bbox_to_anchor=(1.05, 1.0))
+
+        def do_txt_ax():
+            txt_ax.text(x=0.0, y=0.5, s=self.get_xrotor_output_text(), ha='left', va='center', fontfamily='consolas')
+            txt_ax.axis('off')
+
+        def do_radial_axes():
+            xdata = self.xrotor_op_dict['r/R']
+            for ylbl, ax in radial_axes.items():
+                if ylbl in self.blade_data:
+                    ax.plot(xdata, self.blade_data[ylbl], marker='*', markersize=4)
+                else:
+                    if ylbl in self.xrotor_op_dict:
+                        ax.plot(xdata, self.xrotor_op_dict[ylbl], marker='o', markersize=3)
+
+        def do_thrust_eff_ax():
+            ax = radial_axes['thrust_eff']
+            ax.set_ylabel('')
+            ax.grid(False)
+            thrust_eff = self.xrotor_op_dict['thrust(N)'] / self.xrotor_op_dict['power(W)']
+            txt1 = 'Thrust Efficiency:\n\n\n\n\nNewtons / Watt'
+            ax.text(x=0.5, y=0.5, s=txt1, ha='center', va='center')
+            txt2 = '{:.3f}'.format(thrust_eff)
+            ax.text(x=0.5, y=0.5, s=txt2, ha='center', va='center', fontsize=12, fontweight='bold')
+            ax.axis('off')
+
+            # disk loading metric
+            ax.text(x=-0.3, y=0.5, s='Disk Loading:\n\n\n\n\nNewtons / Meter^2', ha='center', va='center')
+            ax.text(x=-0.3, y=0.5, s='{:.3f}'.format(self.disk_loading), ha='center', va='center',
+                    fontsize=12, fontweight='bold')
+
+        do_ax3d()
+        do_txt_ax()
+        do_radial_axes()
+        do_thrust_eff_ax()
+        wsp = 0.60 if created_from_ui else 0.35
+        fig.subplots_adjust(left=0.05, bottom=0.08, right=0.95, top=0.94, wspace=wsp, hspace=0.5)
+
+        if savefig:
+            savepath = os.path.join(os.getcwd(), '{}.png'.format(ax3d.get_title()))
+            fig.savefig(savepath)
+            Info('Saved PNG to "{}"'.format(savepath))
+
+        return fig
+
+    def plot_mpl3d_geometry(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
+                            input_stations: bool = True, interp_profiles: bool = True, savefig: bool = False, fig=None):
+        if fig is not None:
+            ax3d = fig.axes[0]
+            leg_anchor = (-0.15, 1.0)
+        else:
+            fig = plt.figure(figsize=[13, 10])
+            ax3d = fig.add_subplot(111, projection='3d')
+            leg_anchor = (0.90, 1.0)
+
+        ax3d.set_xlabel('X')
+        ax3d.set_ylabel('Y')
+        ax3d.set_zlabel('Z')
+
+        title_txt = 'Propeller Geometry - {}'.format(self.name)
+        ax3d.set_title(title_txt)
+
+        blades = np.arange(self.xrotor_d['Nblds'])
+        angles = 360 / self.xrotor_d['Nblds'] * blades
+
+        # plot le and te lines
+        if LE:
+            for ang in angles:
+                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
+                le_line, = ax3d.plot3D(xs=[pt[0] for pt in le_pts], ys=[pt[1] for pt in le_pts],
+                                       zs=[pt[2] for pt in le_pts], c='k', lw=2)
+        else:
+            le_line = None
+
+        if TE:
+            for ang in angles:
+                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
+                te_line, = ax3d.plot3D(xs=[pt[0] for pt in te_pts], ys=[pt[1] for pt in te_pts],
+                                       zs=[pt[2] for pt in te_pts], c='k', ls='-.', lw=2)
+        else:
+            te_line = None
+
+        # plot stations
+        if chords_betas:
+            for ang in angles:
+                chordlines = self.get_blade_chordlines(rotate_deg=ang)
+                for line in chordlines:
+                    xs, ys, zs = zip(*line)
+                    station_line, = ax3d.plot3D(xs=xs, ys=ys, zs=zs, c='rosybrown', lw=1, ls='--')
+        else:
+            station_line = None
+
+        # plot station_params
+        if input_stations:
+            radii = self.xrotor_d['r/R'] * self.radius
+            chords = self.xrotor_d['C/R'] * self.radius
+            betas = self.xrotor_d['Beta0deg'].copy()
+            for roR, foil_name in self.station_params.items():
+                # station dimensionalized parameters
+                r = roR * self.radius
+                ch = np.interp(r, radii, chords)
+                beta = np.interp(r, radii, betas)
+                sk = self.geo_params['tot_skew'] * roR
+
+                # load the foil, shift, flip, and dimensionalize coordinates
+                foil = Airfoil(foil_name, verbose=False)
+                xc, yc, zc = funcs.generate_3D_profile_points(nondim_xy_coords=foil.get_coords(), radius=r,
+                                                              axis_shift=0.25, chord_len=ch, beta_deg=beta,
+                                                              skew_deg=sk)
+                foils_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='red', alpha=0.7, lw=1)
+        else:
+            foils_line = None
+
+        # plot interpolated profiles
+        if interp_profiles:
+            for prof_num, prof_xyz in self.blade_xyz_profiles.items():
+                xc, yc, zc = prof_xyz
+                prof_line, = ax3d.plot3D(xs=xc, ys=yc, zs=zc, c='maroon', lw=1, alpha=0.7)
+        else:
+            prof_line = None
+
+        # plot hub
+        if hub:
+            hub_thickness = abs(max([pt[2] for pt in le_pts]) - min([pt[2] for pt in te_pts]))
+            theta = np.linspace(0, np.pi * 2, 50)
+            hub_x = np.cos(theta) * self.hub_radius
+            hub_y = np.sin(theta) * self.hub_radius
+            top_zs = np.ones(len(hub_x)) * hub_thickness / 2
+            bot_zs = -np.ones(len(hub_x)) * hub_thickness / 2
+            hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=top_zs, c='gray', lw=2)
+            hub_line, = ax3d.plot3D(xs=hub_x, ys=hub_y, zs=bot_zs, c='gray', lw=2)
+        else:
+            hub_line = None
+
+        # set square axes and finish up formatting stuff
+        lim = (-self.radius * 0.65, self.radius * 0.65)
+        ax3d.set_xlim(lim)
+        ax3d.set_ylim(lim)
+        ax3d.set_zlim(lim)
+        leg_handles = [le_line, te_line, hub_line, foils_line, station_line, prof_line]
+        leg_labels = ['L.E.', 'T.E.', 'Hub', 'Input Stations', 'XROTOR Stations', 'Interpolated Geom.']
+
+        leg_labels = [leg_labels[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
+        leg_handles = [leg_handles[n] for n in range(len(leg_handles)) if leg_handles[n] is not None]
+        ax3d.legend(leg_handles, leg_labels, loc='upper left', bbox_to_anchor=leg_anchor)
+
+        return fig
+
+    def plot_gl3d_geometry(self, LE: bool = True, TE: bool = True, chords_betas: bool = True, hub: bool = True,
+                            input_stations: bool = True, interp_profiles: bool = True, view=None):
+        if view is None:
+            pg.mkQApp()
+            self.gl_geo_view = view = gl.GLViewWidget()
+            view.setFixedSize(1280, 720)
+            view.show()
+        else:
+            pass
+
+        blades = np.arange(self.xrotor_d['Nblds'])
+        angles = 360 / self.xrotor_d['Nblds'] * blades
+
+        # plot le and te lines
+        if LE:
+            for ang in angles:
+                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
+                le_line = gl.GLLinePlotItem(pos=le_pts, color=[0.5, 0.5, 0.5, 1.0], width=2, antialias=False,
+                                            mode='line_strip', glOptions='opaque')
+                view.addItem(le_line)
+
+        if TE:
+            for ang in angles:
+                le_pts, te_pts = self.get_blade_le_te(rotate_deg=ang)
+                te_line = gl.GLLinePlotItem(pos=te_pts, color=[0.5, 0.5, 0.5, 1.0], width=2, antialias=False,
+                                            mode='line_strip', glOptions='opaque')
+                view.addItem(te_line)
+
+        # plot stations
+        if chords_betas:
+            for ang in angles:
+                chordlines = self.get_blade_chordlines(rotate_deg=ang)
+                for line in chordlines:
+                    station_line = gl.GLLinePlotItem(pos=line, color=[i / 255 for i in [245, 66, 66, 255]],
+                                                     width=2, antialias=False, mode='line_strip', glOptions='opaque')
+                    view.addItem(station_line)
+
+        # plot station_params
+        if input_stations:
+            radii = self.xrotor_d['r/R'] * self.radius
+            chords = self.xrotor_d['C/R'] * self.radius
+            betas = self.xrotor_d['Beta0deg'].copy()
+            for roR, foil_name in self.station_params.items():
+                # station dimensionalized parameters
+                r = roR * self.radius
+                ch = np.interp(r, radii, chords)
+                beta = np.interp(r, radii, betas)
+                sk = self.geo_params['tot_skew'] * roR
+
+                # load the foil, shift, flip, and dimensionalize coordinates
+                foil = Airfoil(foil_name, verbose=False)
+                xc, yc, zc = funcs.generate_3D_profile_points(nondim_xy_coords=foil.get_coords(), radius=r,
+                                                              axis_shift=0.25, chord_len=ch, beta_deg=beta,
+                                                              skew_deg=sk)
+                coords = list(zip(xc, yc, zc))
+                foils_line = gl.GLLinePlotItem(pos=coords, color=[i / 255 for i in [5, 0, 163, 255]], width=2, antialias=False,
+                                               mode='line_strip', glOptions='opaque')
+                view.addItem(foils_line)
+
+        # plot interpolated profiles
+        if interp_profiles:
+            for prof_num, prof_xyz in self.blade_xyz_profiles.items():
+                xc, yc, zc = prof_xyz
+                coords = list(zip(xc, yc, zc))
+                prof_line = gl.GLLinePlotItem(pos=coords, color=[i / 255 for i in [163, 0, 0, 200]], width=2,
+                                              antialias=False, mode='line_strip', glOptions='opaque')
+                view.addItem(prof_line)
+
+        # plot hub
+        if hub:
+            hub_thickness = abs(max([pt[2] for pt in le_pts]) - min([pt[2] for pt in te_pts]))
+            theta = np.linspace(0, np.pi * 2, 50)
+            hub_x = np.cos(theta) * self.hub_radius
+            hub_y = np.sin(theta) * self.hub_radius
+            top_zs = np.ones(len(hub_x)) * hub_thickness / 2
+            bot_zs = -np.ones(len(hub_x)) * hub_thickness / 2
+            hub_line = gl.GLLinePlotItem(pos=list(zip(hub_x, hub_y, top_zs)), color=[0.5, 0.5, 0.5, 1.0], width=2,
+                                         antialias=False, mode='line_strip', glOptions='opaque')
+            view.addItem(hub_line)
+            hub_line_bot = gl.GLLinePlotItem(pos=list(zip(hub_x, hub_y, bot_zs)), color=[0.5, 0.5, 0.5, 1.0], width=2,
+                                                          antialias=False, mode='line_strip', glOptions='opaque')
+            view.addItem(hub_line_bot)
+
+        # finish up formatting stuff
+        lim = self.radius * 2.5
+        view.setCameraPosition(distance=lim, azimuth=-90)
+        zgrid = gl.GLGridItem()
+        zgrid.setSize(2, 2, 2)
+        zgrid.setSpacing(.2, .2, .2)
+        zgrid.translate(0, 0, -0.5)
+        view.addItem(zgrid)
+
+        return view
+
+    def plot_gl3d_wvel_data(self, total: bool = True, axial: bool = False, tangential: bool = False, view=None,
+                            plot_every: int = 3):
+        if view is None:
+            pg.mkQApp()
+            self.gl_wvel_view = view = gl.GLViewWidget()
+            view.setFixedSize(1280, 720)
+            view.show()
+        else:
+            pass
+
+        blades = np.arange(self.xrotor_d['Nblds'])
+        angles = 360 / self.xrotor_d['Nblds'] * blades
+
+        self.gl3d_wvel_view = view = self.plot_gl3d_geometry(view=view)
+
+        # plot vel vectors
+        q_chord_pts = self.get_blade_quarter_chords()
+        assert len(self.blade_data['r/R']) == len(q_chord_pts)
+        for i, pt in enumerate(q_chord_pts):
+            if i % plot_every == 0:
+                va = self.blade_data['VA'][i]
+                vt = self.blade_data['VT'][i]
+                vd = self.blade_data['VD'][i]
+                if total:
+                    vector_root = pt
+                    vector_tip = pt[0] - vd, pt[1] + vt, pt[2] - va
+                    vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3)
+                if axial:
+                    vector_root = pt
+                    vector_tip = pt[0], pt[1], pt[2] - va
+                    vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3, color=(.05, .65, .13, 1))
+                if tangential:
+                    vector_root = pt
+                    vector_tip = pt[0], pt[1] + vt, pt[2]
+                    vector = Custom3DArrow(view=view, tip_root=[vector_tip, vector_root], width=3, color=(.92, .84, .2, 1))
+
+        return view
+
+    def generate_stl_geometry(self, plot_after: bool = True, verbose: bool = True):
+        n_prof = len(self.blade_xyz_profiles)
+        n_pts = np.max(np.shape(self.blade_xyz_profiles[0]))
+        n_main_surf = (n_prof - 1) * 2 * (n_pts - 1)
+        n_root = n_pts - 3
+        n_tip = n_pts - 3
+        n_tri = n_main_surf + n_root + n_tip
+
+        mdata = np.zeros(n_tri, dtype=mesh.Mesh.dtype)
+
+        tri_idx = 0
+
+        # root profile
+        vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[0])  # outwards
+        # vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[0], reverse_order=True)  # inwards
+        for vec in vectors:
+            mdata['vectors'][tri_idx] = np.array(vec)
+            tri_idx += 1
+
+        # tip profile
+        vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[n_prof - 1], reverse_order=True)    # outwards
+        # vectors = funcs.compute_profile_trimesh(profile_coords=self.blade_xyz_profiles[n_prof - 1])    # inwards
+        for vec in vectors:
+            mdata['vectors'][tri_idx] = np.array(vec)
+            tri_idx += 1
+
+        # iterate over the profiles
+        for k in range(n_prof - 1):
+            xyz_prof = self.blade_xyz_profiles[k]
+            nxt_prof = self.blade_xyz_profiles[k + 1]
+
+            # inter-profile surfaces
+            for i in range(n_pts - 1):  # right hand rule to get normal direction correct
+                a = xyz_prof[:, i]  # a is a point-coordinate in (x, y, z) format
+                b = nxt_prof[:, i]  # same for b-f
+                c = nxt_prof[:, i + 1]
+                d = a.copy()
+                e = c.copy()
+                f = xyz_prof[:, i + 1]
+
+                # outwards
+                mdata['vectors'][tri_idx] = np.array([a, b, c])      # populate the array of triangle vectors
+                mdata['vectors'][tri_idx + 1] = np.array([d, e, f])  # going in order, 2 triangles per iteration
+
+                # inwards
+                # mdata['vectors'][tri_idx] = np.array([c, b, a])      # populate the array of triangle vectors
+                # mdata['vectors'][tri_idx + 1] = np.array([f, e, d])  # going in order, 2 triangles per iteration
+
+                tri_idx += 2
+
+        m = mesh.Mesh(mdata)
+
+        if os.path.exists(self.stl_fpath):
+            os.remove(self.stl_fpath)
+        m.save(filename=self.stl_fpath)
+
+        self.stl_mesh = mesh.Mesh.from_file(self.stl_fpath)
+        if verbose:
+            Info('Saved STL file and reloaded into propeller object: "{}"'.format(self.stl_fpath))
+
+        if plot_after:
+            self.plot_stl_mesh()
+
+    def load_stl_geometry(self, verbose: bool = True):
+        if os.path.exists(self.stl_fpath):
+            self.stl_mesh = mesh.Mesh.from_file(self.stl_fpath)
+            if verbose:
+                Info('Loaded STL mesh data from file: {}'.format(self.stl_fpath))
+        else:
+            if verbose:
+                Warning('STL file does not exist, use "generate_stl_geometry()" first')
+
+    def plot_stl_mesh(self):
+        if not hasattr(self, 'stl_view'):
+            pg.mkQApp()
+            self.stl_view = gl.GLViewWidget()
+        view = self.stl_view
+        view.clear()
+        view.setFixedSize(1280, 720)
+        view.show()
+
+        grid = gl.GLGridItem()
+        grid.scale(self.radius / 10, self.radius / 10, self.radius / 10)
+        grid.translate(dx=0, dy=0, dz=-self.radius / 4)
+        view.addItem(grid)
+        view.setCameraPosition(distance=self.radius * 1.5, elevation=10, azimuth=-70)
+
+        md = gl.MeshData(vertexes=self.stl_mesh.vectors.copy())
+        mesh_itm = gl.GLMeshItem(meshdata=md, color=[0, 0, .7, 1], edgeColor=[.5, .5, .5, 1], drawEdges=False, drawFaces=True,
+                                 shader='normalColor', smooth=False)
+        mesh_itm.translate(dx=-0.5 * self.radius, dy=0, dz=0)
+        view.addItem(mesh_itm)
+
+        return view
+
+    def plot_ideal_eff(self):
+        Info('"{}" ideal efficiency: {:.1f}%'.format(self.name, self.ideal_eff))
+        return
+
+    def analyze_operating_point(self, velo: float = None, adva: float = None, rpm: float = None, thrust: float = None,
+                                power: float = None, torque: float = None, xrotor_verbose: bool = False):
+
+        funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=self.design_vorform, adva=adva, rpm=rpm, thrust=thrust,
+                              torque=torque, power=power, velo=velo, xrotor_verbose=xrotor_verbose)
+
+    def analyze_sweep(self, velo_vals: list, sweep_param: str, sweep_vals: list, verbose: bool = True,
+                      xrotor_verbose: bool = False, vorform: str = None, prog_signal=None):
+        if sweep_param not in ['adva', 'rpm', 'thrust', 'power', 'torque']:
+            raise Error('"sweep_param" must be one of ("adva", "rpm", "thrust", "power", "torque")')
+
+        vorform = self.design_vorform if vorform is None else vorform
+
+        total_pnts = len(velo_vals) * len(sweep_vals)
+        if verbose:
+            info_str = 'Analyzing "{}" across a sweep of {} operating points'.format(self.name, total_pnts)
+            if prog_signal is not None:
+                prog_signal.emit(0, [info_str])
+            else:
+                Info(info_str)
+        count = 0
+        for velo_val in velo_vals:
+            for v, val in enumerate(sweep_vals):
+                count += 1
+                if verbose:
+                    info_str = 'Analyzing sweep point # {} / {}'.format(count, total_pnts)
+                    if prog_signal is not None:
+                        prog_signal.emit(count / total_pnts * 100, [info_str])
+                    else:
+                        Info(info_str)
+                try:
+                    funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=vorform, velo=velo_val, verbose=False,
+                                          xrotor_verbose=xrotor_verbose, **{sweep_param: val})
+                except Error as e:
+                    warn_str = 'Failed to get XROTOR oper results for vel={}, {}={}\n{}'.format(velo_val, sweep_param, val, e)
+                    if prog_signal is not None:
+                        prog_signal.emit(None, [warn_str])
+                    else:
+                        Warning(warn_str)
+                        pass
+
+        self.oper_data.load_oper_sweep_results()
+        self.wvel_data.load_wvel_sweep_results()
+        if verbose:
+            if prog_signal is not None:
+                prog_signal.emit(0, 'Done!')
+            else:
+                Info('Done!')
+
+    def clear_sweep_data(self):
+        if os.path.exists(self.oper_data_dir):
+            shutil.rmtree(self.oper_data_dir)
+            Info('Removed {} and its contents'.format(self.oper_data_dir))
+        if os.path.exists(self.wvel_data_dir):
+            shutil.rmtree(self.wvel_data_dir)
+            Info('Removed {} and its contents'.format(self.wvel_data_dir))
+
+
+class PropellerOperData:
+    def __init__(self, directory: str):
+        self.directory = directory
+        self.datapoints = {}
+        self.prop_name = os.path.split(os.path.split(self.directory)[0])[1]
+
+    def __len__(self):
+        return len(self.datapoints)
+
+    def get_swept_params(self):
+        valid_params = VALID_OPER_PLOT_PARAMS
+        swept_params = []
+        avoid_params = []
+        for param in valid_params:
+            for dp in self.datapoints.values():
+                if param not in swept_params:
+                    pts = self.get_datapoints_by_paramval(param=param, val=dp[param])
+                    if 2 < len(pts) < len(self.datapoints) and param not in avoid_params:
+                        swept_params.append(param)
+                    else:
+                        avoid_params.append(param)
+
+        return swept_params
+
+    def get_oper_files(self, fullpath: bool = True):
+        if os.path.exists(self.directory):
+            if fullpath:
+                return [os.path.join(self.directory, name) for name in os.listdir(self.directory) if name.endswith('.oper')]
+            else:
+                return [name for name in os.listdir(self.directory) if name.endswith('.oper')]
+        else:
+            return []
+
+    def load_oper_sweep_results(self, verbose: bool = True):
+        self.datapoints = d = {}
+        fnames = self.get_oper_files(fullpath=False)
+        for fname in fnames:
+            vel_key, rpm_key = [float(num) for num in fname.strip('velo_').strip('.oper').split('_rpm_')]
+            vel_key /= 100
+            oper_fullpath = os.path.join(self.directory, fname)
+            d[(vel_key, rpm_key)] = funcs.read_xrotor_op_file(fpath=oper_fullpath)
+        if verbose and len(fnames) > 0:
+            Info('Loaded Existing Oper Results (.oper)!', indent_level=1)
+
+    def get_unique_param(self, param: str):
+        uniq_vals = []
+        for val in self.datapoints.values():
+            if val[param] not in uniq_vals:
+                uniq_vals.append(val[param])
+        return list(sorted(uniq_vals))
+
+    def get_datapoints_by_paramval(self, param: str, val: Union[float, int]):
+        pnts = []
+        for key, dp in self.datapoints.items():
+            if dp[param] == val:
+                pnts.append(dp)
+        return pnts
+
+    def plot(self, x_param: str, y_param: str, family_param: str = None, iso_param: str = None, fig=None, **plot_kwargs):
+        params = [x_param, y_param, family_param, iso_param]
+        valid_params = VALID_OPER_PLOT_PARAMS
+        valid_params_lower = [s.lower() for s in valid_params]
+
+        if len(self.datapoints) == 0:
+            return
+
+        for i, param in enumerate(params):
+            if param is not None:
+                if param.lower() in valid_params_lower:
+                    params[i] = valid_params[valid_params_lower.index(param.lower())]
+                if param.lower() in ['adv', 'adv.', 'adva', 'adv. ratio', 'adv.ratio']:
+                    params[i] = 'adv. ratio'
+                elif param.lower() in ['speed', 'speed(m/s)', 'vel', 'velocity', 'speed_mps']:
+                    params[i] = 'speed(m/s)'
+                elif param.lower() in ['thrust', 'thrust(n)', 'thrust (n)']:
+                    params[i] = 'thrust(N)'
+                elif param.lower() in ['power', 'power(w)', 'power (w)']:
+                    params[i] = 'power(W)'
+                elif param.lower() in ['torque(n-m)', 'torque', 'torque (n-m)']:
+                    params[i] = 'torque(N-m)'
+                elif param.lower() in ['eff', 'efficiency', 'Efficiency']:
+                    params[i] = 'Efficiency'
+                elif param.lower() in ['pvisc(w)', 'pvisc (w)', 'pvisc']:
+                    params[i] = 'Pvisc(W)'
+            else:
+                params[i] = None
+
+        x_param, y_param, family_param, iso_param = params
+
+        if x_param not in valid_params:
+            raise Error('x_param "{}" is not one of the valid params ({})'.format(x_param, valid_params))
+        if y_param not in valid_params:
+            raise Error('y_param "{}" is not one of the valid params ({})'.format(y_param, valid_params))
+        if family_param not in valid_params and family_param is not None:
+            raise Error('family_param error, must be one of {}'.format(valid_params))
+        if iso_param not in valid_params and iso_param is not None:
+            raise Error('iso_param error, must be one of {}'.format(valid_params))
+
+        if fig is None:
+            fig = plt.figure(figsize=[10, 8])
+            ax = fig.add_subplot(111)
+        else:
+            ax = fig.axes[0]
+
+        ax.grid(True)
+        ax.set_title('{} Sweep Results'.format(self.prop_name))
+        ax.set_xlabel(x_param)
+        ax.set_ylabel(y_param)
+
+        if family_param is not None:
+            fvals = self.get_unique_param(param=family_param)
+            for fval in fvals:
+                datapts = self.get_datapoints_by_paramval(param=family_param, val=fval)
+                xvals = [dp[x_param] for dp in datapts]
+                yvals = [dp[y_param] for dp in datapts]
+                xvals, yvals = zip(*sorted(zip(xvals, yvals)))
+                ax.plot(xvals, yvals, '-o', label='{}'.format(fval))
+
+            if iso_param is not None:
+                ivals = self.get_unique_param(param=iso_param)
+                for ival in ivals:
+                    datapts = self.get_datapoints_by_paramval(param=iso_param, val=ival)
+                    if len(datapts) > 1:
+                        xvals = [dp[x_param] for dp in datapts]
+                        yvals = [dp[y_param] for dp in datapts]
+                        xvals, yvals = zip(*sorted(zip(xvals, yvals)))
+                        ax.plot(xvals, yvals, '--', label='{}'.format(ival))
+
+            leg_title = '{} /\n{}'.format(family_param, iso_param) if iso_param is not None else '{}'.format(family_param)
+            ax.legend(title=leg_title, loc='best')
+        else:
+            datapts = self.datapoints.values()
+            xvals = [dp[x_param] for dp in datapts]
+            yvals = [dp[y_param] for dp in datapts]
+            xvals, yvals = zip(*sorted(zip(xvals, yvals)))
+            ax.plot(xvals, yvals, 'o')
+
+        return fig
+
+
+class PropellerWVelData:
+    def __init__(self, directory: str):
+        self.directory = directory
+        self.datapoints = {}
+        self.prop_name = os.path.split(os.path.split(self.directory)[0])[1]
+
+    def __len__(self):
+        return len(self.datapoints)
+
+    def get_wvel_files(self, fullpath: bool = True):
+        if os.path.exists(self.directory):
+            if fullpath:
+                return [os.path.join(self.directory, name) for name in os.listdir(self.directory) if name.endswith('.wvel')]
+            else:
+                return [name for name in os.listdir(self.directory) if name.endswith('.wvel')]
+        else:
+            return []
+
+    def load_wvel_sweep_results(self, verbose: bool = True):
+        self.datapoints = d = {}
+        fnames = self.get_wvel_files(fullpath=False)
+        for fname in fnames:
+            vel_key, rpm_key = [float(num) for num in fname.strip('velo_').strip('.wvel').split('_rpm_')]
+            vel_key /= 100
+            wvel_fullpath = os.path.join(self.directory, fname)
+            d[(vel_key, rpm_key)] = funcs.read_xrotor_wvel_file(fpath=wvel_fullpath)
+        if verbose and len(fnames) > 0:
+            Info('Loaded Existing WVel Results (.wvel)!', indent_level=1)
```

### Comparing `propeller_design_tools-0.3.5/propdes/science_spinbox_class.py` & `propeller_design_tools-0.4.0/propeller_design_tools/science_spinbox_class.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import numpy as np
-import re as reg
-from PyQt5 import QtWidgets, QtGui, QtCore
-
-# Regular expression to find floats. Match groups are the whole string, the
-# whole coefficient, the decimal part of the coefficient, and the exponent
-# part.
-_float_re = reg.compile(r'(([+-]?\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?)')
-
-
-def valid_float_string(string):
-    match = _float_re.search(string)
-    return match.groups()[0] == string if match else False
-
-
-class ScientificDoubleSpinBox(QtWidgets.QDoubleSpinBox):
-    def __init__(self, *args, **kwargs):
-        super(ScientificDoubleSpinBox, self).__init__(*args, **kwargs)
-
-        self.setMinimum(-np.inf)
-        self.setMaximum(np.inf)
-        self.validator = QtGui.QRegExpValidator(QtCore.QRegExp(r'(([+-]?\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?)'), self)
-        self.setDecimals(1000)
-
-    def validate(self, text, position):
-        return self.validator.validate(text, position)
-
-    def fixup(self, text):
-        return self.validator.fixup(text)
-
-    def valueFromText(self, text):
-        return float(text)
-
-    def textFromValue(self, value):
-        return format_float(value)
-
-    def stepBy(self, steps):
-        text = self.cleanText()
-        groups = _float_re.search(text).groups()
-        decimal = float(groups[1])
-        decimal += steps
-        new_string = "{:g}".format(decimal) + (groups[3] if groups[3] else "")
-        self.lineEdit().setText(new_string)
-
-
-def format_float(value):
-    """Modified form of the 'g' format specifier."""
-    string = "{:g}".format(value).replace("e+", "e")
-    string = reg.sub("e(-?)0*(\d+)", r"e\1\2", string)
-    return string
+import numpy as np
+import re as reg
+from PyQt5 import QtWidgets, QtGui, QtCore
+
+# Regular expression to find floats. Match groups are the whole string, the
+# whole coefficient, the decimal part of the coefficient, and the exponent
+# part.
+_float_re = reg.compile(r'(([+-]?\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?)')
+
+
+def valid_float_string(string):
+    match = _float_re.search(string)
+    return match.groups()[0] == string if match else False
+
+
+class ScientificDoubleSpinBox(QtWidgets.QDoubleSpinBox):
+    def __init__(self, *args, **kwargs):
+        super(ScientificDoubleSpinBox, self).__init__(*args, **kwargs)
+
+        self.setMinimum(-np.inf)
+        self.setMaximum(np.inf)
+        self.validator = QtGui.QRegExpValidator(QtCore.QRegExp(r'(([+-]?\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?)'), self)
+        self.setDecimals(1000)
+
+    def validate(self, text, position):
+        return self.validator.validate(text, position)
+
+    def fixup(self, text):
+        return self.validator.fixup(text)
+
+    def valueFromText(self, text):
+        return float(text)
+
+    def textFromValue(self, value):
+        return format_float(value)
+
+    def stepBy(self, steps):
+        text = self.cleanText()
+        groups = _float_re.search(text).groups()
+        decimal = float(groups[1])
+        decimal += steps
+        new_string = "{:g}".format(decimal) + (groups[3] if groups[3] else "")
+        self.lineEdit().setText(new_string)
+
+
+def format_float(value):
+    """Modified form of the 'g' format specifier."""
+    string = "{:g}".format(value).replace("e+", "e")
+    string = reg.sub("e(-?)0*(\d+)", r"e\1\2", string)
+    return string
```

### Comparing `propeller_design_tools-0.3.5/propdes/user_interface.py` & `propeller_design_tools-0.4.0/propeller_design_tools/user_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import numpy as np
-import os
-import subprocess
-from propdes.airfoil import Airfoil
-from propdes.settings import _get_cursor_fpath, _get_gunshot_fpaths
-from propdes.funcs import get_all_airfoil_files, get_all_propeller_dirs
-try:
-    from PyQt5 import QtWidgets, QtGui, QtCore, QtMultimedia
-    from propdes.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
-        AxesComboBoxWidget, PdtGuiPrinter
-    from propdes.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
-    from propdes.prop_creation_ui_classes import PropellerCreationWidget
-    from propdes.prop_analysis_ui_classes import PropellerSweepWidget
-    from propdes.opt_ui_classes import OptimizationWidget
-    from propdes.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
-        PDT_ComboBox, PDT_TabWidget
-except:
-    pass
-
-
-class InterfaceMainWindow(QtWidgets.QMainWindow):
-    def __init__(self, foil: Airfoil = None):
-        super(InterfaceMainWindow, self).__init__()
-        self.setWindowTitle('PDT Control Dashboard')
-        self.setMinimumSize(1600, 900)
-        self.foil = foil
-
-        cursor_fpath = _get_cursor_fpath()
-        cursor = QtGui.QCursor(QtGui.QPixmap(cursor_fpath))
-        self.setCursor(cursor)
-
-        # central widget
-        center_widg = QtWidgets.QWidget()
-        center_lay = QtWidgets.QVBoxLayout()
-        center_widg.setLayout(center_lay)
-        self.setCentralWidget(center_widg)
-
-        # the main groups
-        top_lay = QtWidgets.QHBoxLayout()
-        sett_grp = PDT_GroupBox('Settings'.upper(), italic=True, font_size=16)
-        sett_grp.setFixedHeight(250)
-        # sett_grp.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
-        top_lay.addWidget(sett_grp)
-        console_grp = PDT_GroupBox('Console Output'.upper(), italic=True, font_size=16)
-        console_grp.setFixedHeight(250)
-        # console_grp.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
-        top_lay.addWidget(console_grp)
-        center_lay.addLayout(top_lay)
-
-        # tab widget
-        tab_widg = PDT_TabWidget(font_size=16, italic=True)
-        center_lay.addWidget(tab_widg)
-        self.af_widg = FoilAnalysisWidget(main_win=self)
-        tab_widg.addTab(self.af_widg, 'Airfoil Analysis'.upper())
-        self.prop_widg = PropellerCreationWidget(main_win=self)
-        tab_widg.addTab(self.prop_widg, 'Propeller Creation'.upper())
-        self.prop_sweep_widg = PropellerSweepWidget(main_win=self)
-        tab_widg.addTab(self.prop_sweep_widg, 'Propeller Analysis'.upper())
-        self.opt_widg = OptimizationWidget()
-        tab_widg.addTab(self.opt_widg, 'Optimization'.upper())
-
-
-        # settings group
-        sett_lay = QtWidgets.QFormLayout()
-        sett_grp.setLayout(sett_lay)
-        self.af_db_select_widg = DatabaseSelectionWidget(main_win=self, db_type='airfoil')
-        sett_lay.addRow(PDT_Label('Airfoil Database:', font_size=14), self.af_db_select_widg)
-        self.prop_db_select_widg = DatabaseSelectionWidget(main_win=self, db_type='propeller')
-        sett_lay.addRow(PDT_Label('Propeller Database:', font_size=14), self.prop_db_select_widg)
-
-        # console group
-        console_lay = QtWidgets.QVBoxLayout()
-        console_grp.setLayout(console_lay)
-        self.console_te = PDT_TextEdit(height=150)
-        console_lay.addWidget(self.console_te)
-        btn_bar_lay = QtWidgets.QHBoxLayout()
-        clear_console_btn = PDT_PushButton('Clear', font_size=11, width=100)
-        clear_console_btn.clicked.connect(self.clear_console_btn_clicked)
-        btn_bar_lay.addWidget(clear_console_btn)
-
-        self.prog_bar = QtWidgets.QProgressBar()
-        self.prog_bar.setMinimumSize(500, 30)
-        self.prog_bar.setValue(0)
-        btn_bar_lay.addStretch()
-        btn_bar_lay.addWidget(self.prog_bar)
-        btn_bar_lay.addStretch()
-        console_lay.addLayout(btn_bar_lay)
-
-        # call these last because they rely on self.console_te existing
-        self.af_db_select_widg.set_current_db()
-        self.prop_db_select_widg.set_current_db()
-        self.printer = PdtGuiPrinter(console_te=self.console_te)
-
-        # connecting signals
-        self.af_db_select_widg.currentDatabaseChanged.connect(self.repop_select_foil_cb)
-        self.prop_db_select_widg.currentDatabaseChanged.connect(self.repop_select_prop_cb)
-
-    def mousePressEvent(self, a0: QtGui.QMouseEvent) -> None:
-        fpaths = _get_gunshot_fpaths()
-        num = int(np.random.rand() * 3.4)
-
-        url = QtCore.QUrl.fromLocalFile(fpaths[num])
-        content = QtMultimedia.QMediaContent(url)
-        player = QtMultimedia.QMediaPlayer(self)
-        player.setMedia(content)
-        player.setVolume(20)
-        player.play()
-
-    def repop_select_prop_cb(self):
-        self.print('Repopulating propeller dropdowns...')
-        self.prop_widg.plot3d_widg.populate_select_prop_cb()
-        self.prop_sweep_widg.select_prop_widg.pop_select_prop_cb()
-
-    def repop_select_foil_cb(self):
-        self.print('Repopulating foil dropdown...')
-        self.af_widg.select_foil_cb.clear()
-        self.af_widg.select_foil_cb.addItems(['None'] + get_all_airfoil_files())
-
-    def clear_console_btn_clicked(self):
-        self.prog_bar.setValue(0)
-        self.console_te.clear()
-
-    def print(self, s: str, fontfamily: str = None):
-        self.printer.print(s, fontfamily=fontfamily)
-
-
-if __name__ == '__main__':
-    import sys
-    app = QtWidgets.QApplication(sys.argv)
-    w = InterfaceMainWindow()
-    w.show()
-    app.exec_()
+import numpy as np
+import os
+import subprocess
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.settings import _get_cursor_fpath, _get_gunshot_fpaths
+from propeller_design_tools.funcs import get_all_airfoil_files, get_all_propeller_dirs
+try:
+    from PyQt5 import QtWidgets, QtGui, QtCore, QtMultimedia
+    from propeller_design_tools.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
+        AxesComboBoxWidget, PdtGuiPrinter
+    from propeller_design_tools.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
+    from propeller_design_tools.prop_creation_ui_classes import PropellerCreationWidget
+    from propeller_design_tools.prop_analysis_ui_classes import PropellerSweepWidget
+    from propeller_design_tools.opt_ui_classes import OptimizationWidget
+    from propeller_design_tools.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
+        PDT_ComboBox, PDT_TabWidget
+except:
+    pass
+
+
+class InterfaceMainWindow(QtWidgets.QMainWindow):
+    def __init__(self, foil: Airfoil = None):
+        super(InterfaceMainWindow, self).__init__()
+        self.setWindowTitle('PDT Control Dashboard')
+        self.setMinimumSize(1600, 900)
+        self.foil = foil
+
+        cursor_fpath = _get_cursor_fpath()
+        cursor = QtGui.QCursor(QtGui.QPixmap(cursor_fpath))
+        self.setCursor(cursor)
+
+        # central widget
+        center_widg = QtWidgets.QWidget()
+        center_lay = QtWidgets.QVBoxLayout()
+        center_widg.setLayout(center_lay)
+        self.setCentralWidget(center_widg)
+
+        # the main groups
+        top_lay = QtWidgets.QHBoxLayout()
+        sett_grp = PDT_GroupBox('Settings'.upper(), italic=True, font_size=16)
+        sett_grp.setFixedHeight(250)
+        # sett_grp.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        top_lay.addWidget(sett_grp)
+        console_grp = PDT_GroupBox('Console Output'.upper(), italic=True, font_size=16)
+        console_grp.setFixedHeight(250)
+        # console_grp.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+        top_lay.addWidget(console_grp)
+        center_lay.addLayout(top_lay)
+
+        # tab widget
+        tab_widg = PDT_TabWidget(font_size=16, italic=True)
+        center_lay.addWidget(tab_widg)
+        self.af_widg = FoilAnalysisWidget(main_win=self)
+        tab_widg.addTab(self.af_widg, 'Airfoil Analysis'.upper())
+        self.prop_widg = PropellerCreationWidget(main_win=self)
+        tab_widg.addTab(self.prop_widg, 'Propeller Creation'.upper())
+        self.prop_sweep_widg = PropellerSweepWidget(main_win=self)
+        tab_widg.addTab(self.prop_sweep_widg, 'Propeller Analysis'.upper())
+        self.opt_widg = OptimizationWidget()
+        tab_widg.addTab(self.opt_widg, 'Optimization'.upper())
+
+
+        # settings group
+        sett_lay = QtWidgets.QFormLayout()
+        sett_grp.setLayout(sett_lay)
+        self.af_db_select_widg = DatabaseSelectionWidget(main_win=self, db_type='airfoil')
+        sett_lay.addRow(PDT_Label('Airfoil Database:', font_size=14), self.af_db_select_widg)
+        self.prop_db_select_widg = DatabaseSelectionWidget(main_win=self, db_type='propeller')
+        sett_lay.addRow(PDT_Label('Propeller Database:', font_size=14), self.prop_db_select_widg)
+
+        # console group
+        console_lay = QtWidgets.QVBoxLayout()
+        console_grp.setLayout(console_lay)
+        self.console_te = PDT_TextEdit(height=150)
+        console_lay.addWidget(self.console_te)
+        btn_bar_lay = QtWidgets.QHBoxLayout()
+        clear_console_btn = PDT_PushButton('Clear', font_size=11, width=100)
+        clear_console_btn.clicked.connect(self.clear_console_btn_clicked)
+        btn_bar_lay.addWidget(clear_console_btn)
+
+        self.prog_bar = QtWidgets.QProgressBar()
+        self.prog_bar.setMinimumSize(500, 30)
+        self.prog_bar.setValue(0)
+        btn_bar_lay.addStretch()
+        btn_bar_lay.addWidget(self.prog_bar)
+        btn_bar_lay.addStretch()
+        console_lay.addLayout(btn_bar_lay)
+
+        # call these last because they rely on self.console_te existing
+        self.af_db_select_widg.set_current_db()
+        self.prop_db_select_widg.set_current_db()
+        self.printer = PdtGuiPrinter(console_te=self.console_te)
+
+        # connecting signals
+        self.af_db_select_widg.currentDatabaseChanged.connect(self.repop_select_foil_cb)
+        self.prop_db_select_widg.currentDatabaseChanged.connect(self.repop_select_prop_cb)
+
+    def mousePressEvent(self, a0: QtGui.QMouseEvent) -> None:
+        fpaths = _get_gunshot_fpaths()
+        num = int(np.random.rand() * 3.4)
+
+        url = QtCore.QUrl.fromLocalFile(fpaths[num])
+        content = QtMultimedia.QMediaContent(url)
+        player = QtMultimedia.QMediaPlayer(self)
+        player.setMedia(content)
+        player.setVolume(20)
+        player.play()
+
+    def repop_select_prop_cb(self):
+        self.print('Repopulating propeller dropdowns...')
+        self.prop_widg.plot3d_widg.populate_select_prop_cb()
+        self.prop_sweep_widg.select_prop_widg.pop_select_prop_cb()
+
+    def repop_select_foil_cb(self):
+        self.print('Repopulating foil dropdown...')
+        self.af_widg.select_foil_cb.clear()
+        self.af_widg.select_foil_cb.addItems(['None'] + get_all_airfoil_files())
+
+    def clear_console_btn_clicked(self):
+        self.prog_bar.setValue(0)
+        self.console_te.clear()
+
+    def print(self, s: str, fontfamily: str = None):
+        self.printer.print(s, fontfamily=fontfamily)
+
+
+if __name__ == '__main__':
+    import sys
+    app = QtWidgets.QApplication(sys.argv)
+    w = InterfaceMainWindow()
+    w.show()
+    app.exec_()
```

### Comparing `propeller_design_tools-0.3.5/propdes/user_io.py` & `propeller_design_tools-0.4.0/propeller_design_tools/user_io.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# ===== PDT - SPECIFIC USER DIALOGUES =====
-def Warning(s: str):
-    print('PDT WARNING: {}'.format(s))
-
-
-def Info(s: str, indent_level: int = 0):
-    ind_txt = '    ' * indent_level
-    offset_spaces = '          '
-    print('PDT INFO: {}{}'.format(ind_txt, s.replace('\n', '\n{}{}'.format(offset_spaces, ind_txt))))
-
-
-def error_plot(**kwargs):
-
-    import matplotlib.pyplot as plt
-
-    if all(plot_param in kwargs for plot_param in ['x', 'y', 'xlbl', 'ylbl']):
-        x = kwargs.pop('x')
-        y = kwargs.pop('y')
-        xlbl = kwargs.pop('xlbl')
-        ylbl = kwargs.pop('ylbl')
-        ax0_is_plot = True
-    else:
-        ax0_is_plot = False
-
-    if 'info_d' in kwargs:
-        info_d = kwargs.pop('info_d')
-    else:
-        info_d = None
-
-    if 'info_d2' in kwargs:
-        info_d2 = kwargs.pop('info_d2')
-    else:
-        info_d2 = None
-
-    fig = plt.figure(figsize=(12, 8))
-    axes = fig.subplots(nrows=1, ncols=2)
-
-    def get_txt_start_params():
-        txt_xstart = 0.05
-        txt_ystart = 0.95
-        txt_xinc = 0.0
-        txt_yinc = -0.04
-        return txt_xstart, txt_ystart, txt_xinc, txt_yinc
-
-    def plot_info_dict(ax, info_dict: dict):
-        x_txt, y_txt, x_inc, y_inc = get_txt_start_params()
-        for header, details in info_dict.items():
-            txt = '{}: {}'.format(header, details)
-            lines = [txt[i:i + 48] for i in range(0, len(txt), 48)]
-            ax.text(x_txt, y_txt, "\n   ".join(lines), ha='left', va='top')
-            y_txt += y_inc * len(lines)
-            x_txt += x_inc * len(lines)
-
-    if ax0_is_plot:
-        axes[0].grid(True)
-        axes[0].set_title('PDT Troubleshooting Plot')
-        axes[0].set_xlabel(xlbl)
-        axes[0].set_ylabel(ylbl)
-        axes[0].plot(x, y)
-
-        axes[1].set_title('PDT Troubleshooting Info')
-        axes[1].axes.xaxis.set_visible(False)
-        axes[1].axes.yaxis.set_visible(False)
-        if info_d is not None:
-            plot_info_dict(ax=axes[1], info_dict=info_d)
-
-    else:
-        for ax in axes:
-            ax.set_title('PDT Troubleshooting Info')
-            ax.axes.xaxis.set_visible(False)
-            ax.axes.yaxis.set_visible(False)
-
-        if info_d is not None:
-            plot_info_dict(ax=axes[0], info_dict=info_d)
-            if info_d2 is not None:
-                plot_info_dict(ax=axes[1], info_dict=info_d2)
-
-    return fig
-
-
-class Error(Exception):
-    def __init__(self, s: str, errplot: bool = False, **errplot_kwargs):
-        if errplot:
-            error_plot(**errplot_kwargs)
-        super().__init__('\nPDT ERROR: {}'.format(s.replace('\n', '\n           ')))
-
-
-class Input:
-    def __init__(self, s: str):
-        self.response = input('\n PDT INPUT: {}'.format(s.replace('\n', '\n           ')))
+# ===== PDT - SPECIFIC USER DIALOGUES =====
+def Warning(s: str):
+    print('PDT WARNING: {}'.format(s))
+
+
+def Info(s: str, indent_level: int = 0):
+    ind_txt = '    ' * indent_level
+    offset_spaces = '          '
+    print('PDT INFO: {}{}'.format(ind_txt, s.replace('\n', '\n{}{}'.format(offset_spaces, ind_txt))))
+
+
+def error_plot(**kwargs):
+
+    import matplotlib.pyplot as plt
+
+    if all(plot_param in kwargs for plot_param in ['x', 'y', 'xlbl', 'ylbl']):
+        x = kwargs.pop('x')
+        y = kwargs.pop('y')
+        xlbl = kwargs.pop('xlbl')
+        ylbl = kwargs.pop('ylbl')
+        ax0_is_plot = True
+    else:
+        ax0_is_plot = False
+
+    if 'info_d' in kwargs:
+        info_d = kwargs.pop('info_d')
+    else:
+        info_d = None
+
+    if 'info_d2' in kwargs:
+        info_d2 = kwargs.pop('info_d2')
+    else:
+        info_d2 = None
+
+    fig = plt.figure(figsize=(12, 8))
+    axes = fig.subplots(nrows=1, ncols=2)
+
+    def get_txt_start_params():
+        txt_xstart = 0.05
+        txt_ystart = 0.95
+        txt_xinc = 0.0
+        txt_yinc = -0.04
+        return txt_xstart, txt_ystart, txt_xinc, txt_yinc
+
+    def plot_info_dict(ax, info_dict: dict):
+        x_txt, y_txt, x_inc, y_inc = get_txt_start_params()
+        for header, details in info_dict.items():
+            txt = '{}: {}'.format(header, details)
+            lines = [txt[i:i + 48] for i in range(0, len(txt), 48)]
+            ax.text(x_txt, y_txt, "\n   ".join(lines), ha='left', va='top')
+            y_txt += y_inc * len(lines)
+            x_txt += x_inc * len(lines)
+
+    if ax0_is_plot:
+        axes[0].grid(True)
+        axes[0].set_title('PDT Troubleshooting Plot')
+        axes[0].set_xlabel(xlbl)
+        axes[0].set_ylabel(ylbl)
+        axes[0].plot(x, y)
+
+        axes[1].set_title('PDT Troubleshooting Info')
+        axes[1].axes.xaxis.set_visible(False)
+        axes[1].axes.yaxis.set_visible(False)
+        if info_d is not None:
+            plot_info_dict(ax=axes[1], info_dict=info_d)
+
+    else:
+        for ax in axes:
+            ax.set_title('PDT Troubleshooting Info')
+            ax.axes.xaxis.set_visible(False)
+            ax.axes.yaxis.set_visible(False)
+
+        if info_d is not None:
+            plot_info_dict(ax=axes[0], info_dict=info_d)
+            if info_d2 is not None:
+                plot_info_dict(ax=axes[1], info_dict=info_d2)
+
+    return fig
+
+
+class Error(Exception):
+    def __init__(self, s: str, errplot: bool = False, **errplot_kwargs):
+        if errplot:
+            error_plot(**errplot_kwargs)
+        super().__init__('\nPDT ERROR: {}'.format(s.replace('\n', '\n           ')))
+
+
+class Input:
+    def __init__(self, s: str):
+        self.response = input('\n PDT INPUT: {}'.format(s.replace('\n', '\n           ')))
```

