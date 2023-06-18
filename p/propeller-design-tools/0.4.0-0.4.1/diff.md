# Comparing `tmp/propeller_design_tools-0.4.0.tar.gz` & `tmp/propeller_design_tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\.tmp-9op688tp\propeller_design_tools-0.4.0.tar", last modified: Sun Jun 18 00:37:31 2023, max compression
+gzip compressed data, was "propeller_design_tools-0.4.1.tar", last modified: Sun Jun 18 02:50:50 2023, max compression
```

## Comparing `propeller_design_tools-0.4.0.tar` & `propeller_design_tools-0.4.1.tar`

### file list

```diff
@@ -1,375 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/
--rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    51932 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     9400 2023-06-18 00:34:26.000000 propeller_design_tools-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/
--rw-rw-rw-   0        0        0      481 2023-06-18 00:09:35.000000 propeller_design_tools-0.4.0/propeller_design_tools/__init__.py
--rw-rw-rw-   0        0        0    28820 2022-05-20 22:03:53.000000 propeller_design_tools-0.4.0/propeller_design_tools/airfoil.py
--rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.4.0/propeller_design_tools/custom_opengl_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag35.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag36.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag37.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/ag38.dat
--rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/arad13.dat
--rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/boe103.dat
--rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/boe106.dat
--rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/clarky.dat
--rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/e855.dat
--rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/hs1606.dat
--rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/mrc-16.dat
--rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_database/xfoil.exe
--rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.4.0/propeller_design_tools/foil_ui_classes.py
--rw-rw-rw-   0        0        0    50416 2023-04-27 19:31:58.000000 propeller_design_tools-0.4.0/propeller_design_tools/funcs.py
--rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16315 2023-04-26 19:09:09.000000 propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.4.0/propeller_design_tools/opt_ui_classes.py
--rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.4.0/propeller_design_tools/optimizations.py
--rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36995 2022-06-12 01:05:11.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_creation_ui_classes.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/
--rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
--rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
--rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
--rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
--rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
--rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
--rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
--rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
--rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
--rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/station_polars/
--rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/
--rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
--rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/station_polars/
--rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/
--rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
--rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/station_polars/
--rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
--rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.4.0/propeller_design_tools/prop_database/xrotor.exe
--rw-rw-rw-   0        0        0    53871 2022-06-12 00:41:00.000000 propeller_design_tools-0.4.0/propeller_design_tools/propeller.py
--rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.4.0/propeller_design_tools/radialstation.py
--rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.4.0/propeller_design_tools/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.4.0/propeller_design_tools/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/
--rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/crosshair_cursor.png
--rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot1.wav
--rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot2.wav
--rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot3.wav
--rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/gunshot4.wav
--rw-rw-rw-   0        0        0      236 2023-06-17 23:50:58.000000 propeller_design_tools-0.4.0/propeller_design_tools/supporting_files/user-settings.txt
--rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.4.0/propeller_design_tools/user_interface.py
--rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.4.0/propeller_design_tools/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0    51932 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    26656 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-18 00:37:30.000000 propeller_design_tools-0.4.0/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1866 2023-06-18 00:37:19.000000 propeller_design_tools-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 00:37:31.000000 propeller_design_tools-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-06-18 00:23:03.000000 propeller_design_tools-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1405 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    51938 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9406 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 02:50:50.014140 propeller_design_tools-0.4.1/propdes/
+-rw-rw-rw-   0        0        0      374 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/__init__.py
+-rw-rw-rw-   0        0        0    28775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/custom_opengl_classes.py
+-rw-rw-rw-   0        0        0    18318 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50326 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/funcs.py
+-rw-rw-rw-   0        0        0    17801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16285 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      386 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    10965 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/optimizations.py
+-rw-rw-rw-   0        0        0    15547 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36905 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/prop_creation_ui_classes.py
+-rw-rw-rw-   0        0        0    53781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/propeller.py
+-rw-rw-rw-   0        0        0    17572 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4096 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/settings.py
+-rw-rw-rw-   0        0        0     5722 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0    51938 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1866 2023-06-18 02:49:04.000000 propeller_design_tools-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `propeller_design_tools-0.4.0/LICENSE` & `propeller_design_tools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.0/MANIFEST.in` & `propeller_design_tools-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.0/PKG-INFO` & `propeller_design_tools-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller_design_tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -802,16 +802,16 @@
 --------------------------
 At a high-level, the current concept for PDT workflow is as 
 follows (after obtaining the required executables and pip-installing 
 the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
-https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
-)
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
+   )
 
    ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
    ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
    ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
 
 1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
```

### Comparing `propeller_design_tools-0.4.0/README.md` & `propeller_design_tools-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
 --------------------------
 At a high-level, the current concept for PDT workflow is as 
 follows (after obtaining the required executables and pip-installing 
 the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
-https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
-)
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
+   )
 
    ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
    ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
    ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
 
 1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/airfoil.py` & `propeller_design_tools-0.4.1/propdes/airfoil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import warnings
-from propeller_design_tools import funcs
-from propeller_design_tools.user_io import Error, Info, Warning
-from propeller_design_tools.settings import get_foil_db
+from propdes import funcs
+from propdes.user_io import Error, Info, Warning
+from propdes.settings import get_foil_db
 import matplotlib
 matplotlib.use('TKAgg')
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.interpolate import griddata, interp1d
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/custom_opengl_classes.py` & `propeller_design_tools-0.4.1/propdes/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/foil_ui_classes.py` & `propeller_design_tools-0.4.1/propdes/foil_ui_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from propeller_design_tools.funcs import delete_all_widgets_from_layout, get_all_airfoil_files, clear_foil_database, \
+from propdes.funcs import delete_all_widgets_from_layout, get_all_airfoil_files, clear_foil_database, \
     download_foil_coordinates
-from propeller_design_tools.airfoil import Airfoil
+from propdes.airfoil import Airfoil
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 import numpy as np
 try:
     from PyQt5 import QtWidgets, QtCore
-    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_PushButton, PDT_ComboBox, \
+    from propdes.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_PushButton, PDT_ComboBox, \
         PDT_CheckBox, PDT_LineEdit
-    from propeller_design_tools.helper_ui_classes import RangeLineEditWidget, SingleAxCanvas, AxesComboBoxWidget, \
+    from propdes.helper_ui_classes import RangeLineEditWidget, SingleAxCanvas, AxesComboBoxWidget, \
         Capturing
 except:
     pass
 
 
 class FoilAnalysisWidget(QtWidgets.QWidget):
     def __init__(self, main_win: 'InterfaceMainWindow'):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/funcs.py` & `propeller_design_tools-0.4.1/propdes/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import subprocess
 import shutil
 import sys
 import urllib.request
 
 import matplotlib.pyplot as plt
 import numpy as np
-from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.radialstation import RadialStation
-from propeller_design_tools.propeller import Propeller
-from propeller_design_tools.user_io import Info, Error, Warning
-from propeller_design_tools.settings import _get_user_settings, get_prop_db, get_foil_db
+from propdes.airfoil import Airfoil
+from propdes.radialstation import RadialStation
+from propdes.propeller import Propeller
+from propdes.user_io import Info, Error, Warning
+from propdes.settings import _get_user_settings, get_prop_db, get_foil_db
 
 
 # =============== CONVENIENCE / UTILITY FUNCTIONS ===============
 def delete_propeller(prop, verbose: bool = True):
     fpaths = [prop.xrr_file, prop.xrop_file, prop.meta_file]
     rmvd = []
     for path in fpaths:
@@ -1220,15 +1220,15 @@
 
     return vectors
 
 
 # ===== USER INTERFACE STUFF =====
 def start_ui():
     from PyQt5 import QtWidgets
-    from propeller_design_tools.user_interface import InterfaceMainWindow
+    from propdes.user_interface import InterfaceMainWindow
     app = QtWidgets.QApplication(sys.argv)
     w = InterfaceMainWindow()
     w.show()
     app.exec_()
 
 
 def delete_all_widgets_from_layout(layout):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_classes.py` & `propeller_design_tools-0.4.1/propdes/helper_ui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import subprocess
 
 import numpy as np
 import matplotlib.gridspec as gridspec
-from propeller_design_tools.settings import get_setting, set_propeller_database, set_airfoil_database, \
+from propdes.settings import get_setting, set_propeller_database, set_airfoil_database, \
     get_foil_db, get_prop_db
-from propeller_design_tools.funcs import count_airfoil_db, count_propeller_db
-from propeller_design_tools.propeller import Propeller
+from propdes.funcs import count_airfoil_db, count_propeller_db
+from propdes.propeller import Propeller
 import sys
 from typing import Union
 from io import StringIO
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 try:
     from PyQt5 import QtWidgets, QtCore, QtGui
-    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_PushButton, PDT_SpinBox, PDT_DoubleSpinBox, \
+    from propdes.helper_ui_subclasses import PDT_Label, PDT_PushButton, PDT_SpinBox, PDT_DoubleSpinBox, \
         PDT_ComboBox, PDT_GroupBox, PDT_CheckBox, PDT_TextEdit, PDT_LineEdit, PDT_ScienceSpinBox
 except:
     pass
 
 
 class SingleAxCanvas(FigureCanvasQTAgg):
     def __init__(self, *args, **kwargs):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/helper_ui_subclasses.py` & `propeller_design_tools-0.4.1/propdes/helper_ui_subclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 try:
     from PyQt5 import QtWidgets, QtGui, QtCore
-    from propeller_design_tools.settings import _get_cursor_fpath
-    from propeller_design_tools.science_spinbox_class import ScientificDoubleSpinBox
+    from propdes.settings import _get_cursor_fpath
+    from propdes.science_spinbox_class import ScientificDoubleSpinBox
 except:
     pass
 
 
 class PDT_GroupBox(QtWidgets.QGroupBox):
     def __init__(self, *args, **kwargs):
         italic = kwargs.pop('italic') if 'italic' in kwargs else False
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/optimizations.py` & `propeller_design_tools-0.4.1/propdes/optimizations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import shutil
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import pyqtgraph as pg
 from pyqtgraph import opengl as gl
-from propeller_design_tools import Propeller
-from propeller_design_tools.user_io import Error
-from propeller_design_tools.funcs import create_propeller, get_prop_db
-from propeller_design_tools.user_io import Info, Warning
-from propeller_design_tools.custom_opengl_classes import Custom3DAxis
+from propdes import Propeller
+from propdes.user_io import Error
+from propdes.funcs import create_propeller, get_prop_db
+from propdes.user_io import Info, Warning
+from propdes.custom_opengl_classes import Custom3DAxis
 
 
 class VehicleRangeOptimization:
     def __init__(self):
         pass
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/prop_analysis_ui_classes.py` & `propeller_design_tools-0.4.1/propdes/prop_analysis_ui_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 import pyqtgraph.opengl as gl
-from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
-from propeller_design_tools.funcs import get_all_propeller_dirs
-from propeller_design_tools.propeller import Propeller
+from propdes.settings import VALID_OPER_PLOT_PARAMS
+from propdes.funcs import get_all_propeller_dirs
+from propdes.propeller import Propeller
 try:
     from PyQt5 import QtWidgets, QtCore
-    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
+    from propdes.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
         PDT_CheckBox
-    from propeller_design_tools.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
+    from propdes.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
         CheckColumnWidget, AxesComboBoxWidget, RangeLineEditWidget, Capturing
 except:
     pass
 
 
 class PropellerSweepWidget(QtWidgets.QWidget):
     def __init__(self, main_win: 'InterfaceMainWindow'):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/prop_creation_ui_classes.py` & `propeller_design_tools-0.4.1/propdes/prop_creation_ui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import subprocess
 import numpy as np
 import os
-from propeller_design_tools.propeller import Propeller
-from propeller_design_tools.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
-from propeller_design_tools.user_io import Error
-from propeller_design_tools.settings import get_prop_db
+from propdes.propeller import Propeller
+from propdes.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
+from propdes.user_io import Error
+from propdes.settings import get_prop_db
 
 try:
     from PyQt5 import QtWidgets, QtCore
-    from propeller_design_tools.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
+    from propdes.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
         PropellerCreationPanelCanvas, RadialStationFitParamsCanvas
-    from propeller_design_tools.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
+    from propdes.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
         PDT_PushButton, PDT_LineEdit, PDT_CheckBox
     import pyqtgraph.opengl as gl
 except:
     pass
 
 
 class PropellerCreationWidget(QtWidgets.QWidget):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/propeller.py` & `propeller_design_tools-0.4.1/propdes/propeller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
-from propeller_design_tools import funcs
-from propeller_design_tools.user_io import Info, Error, Warning
-from propeller_design_tools.settings import get_setting
-from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
-from propeller_design_tools.custom_opengl_classes import Custom3DArrow
+from propdes import funcs
+from propdes.user_io import Info, Error, Warning
+from propdes.settings import get_setting
+from propdes.airfoil import Airfoil
+from propdes.settings import VALID_OPER_PLOT_PARAMS
+from propdes.custom_opengl_classes import Custom3DArrow
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from mpl_toolkits import mplot3d
 import numpy as np
 from stl import mesh
 from typing import Union
 import pyqtgraph as pg
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/radialstation.py` & `propeller_design_tools-0.4.1/propdes/radialstation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from propeller_design_tools import funcs
-from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.user_io import Info, Error
+from propdes import funcs
+from propdes.airfoil import Airfoil
+from propdes.user_io import Info, Error
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.optimize import curve_fit
 
 
 class RadialStation(object):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/science_spinbox_class.py` & `propeller_design_tools-0.4.1/propdes/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/settings.py` & `propeller_design_tools-0.4.1/propdes/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import os
-from propeller_design_tools.user_io import Error, Input, Info
+from propdes.user_io import Error, Input, Info
 import pkg_resources
 
 
 VALID_OPER_PLOT_PARAMS = ['adv. ratio', 'J', 'speed(m/s)', 'rpm', 'thrust(N)', 'power(W)', 'torque(N-m)', 'Efficiency',
                           'Eff induced', 'Eff ideal', 'Pvisc(W)', 'Ct', 'Tc', 'Cp', 'Pc', 'Sigma']
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/user_interface.py` & `propeller_design_tools-0.4.1/propdes/user_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import os
 import subprocess
-from propeller_design_tools.airfoil import Airfoil
-from propeller_design_tools.settings import _get_cursor_fpath, _get_gunshot_fpaths
-from propeller_design_tools.funcs import get_all_airfoil_files, get_all_propeller_dirs
+from propdes.airfoil import Airfoil
+from propdes.settings import _get_cursor_fpath, _get_gunshot_fpaths
+from propdes.funcs import get_all_airfoil_files, get_all_propeller_dirs
 try:
     from PyQt5 import QtWidgets, QtGui, QtCore, QtMultimedia
-    from propeller_design_tools.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
+    from propdes.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
         AxesComboBoxWidget, PdtGuiPrinter
-    from propeller_design_tools.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
-    from propeller_design_tools.prop_creation_ui_classes import PropellerCreationWidget
-    from propeller_design_tools.prop_analysis_ui_classes import PropellerSweepWidget
-    from propeller_design_tools.opt_ui_classes import OptimizationWidget
-    from propeller_design_tools.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
+    from propdes.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
+    from propdes.prop_creation_ui_classes import PropellerCreationWidget
+    from propdes.prop_analysis_ui_classes import PropellerSweepWidget
+    from propdes.opt_ui_classes import OptimizationWidget
+    from propdes.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
         PDT_ComboBox, PDT_TabWidget
 except:
     pass
 
 
 class InterfaceMainWindow(QtWidgets.QMainWindow):
     def __init__(self, foil: Airfoil = None):
```

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools/user_io.py` & `propeller_design_tools-0.4.1/propdes/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.0/propeller_design_tools.egg-info/PKG-INFO` & `propeller_design_tools-0.4.1/propeller_design_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller-design-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -802,16 +802,16 @@
 --------------------------
 At a high-level, the current concept for PDT workflow is as 
 follows (after obtaining the required executables and pip-installing 
 the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
-https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
-)
+   https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
+   )
 
    ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
    ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
    ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
 
 1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
```

### Comparing `propeller_design_tools-0.4.0/pyproject.toml` & `propeller_design_tools-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0"]  # build requirements (don't include build or twine)
 build-backend = "setuptools.build_meta"
 
 
 [project]
-version = "0.4.0"
+version = "0.4.1"
 name = "propeller_design_tools"
 authors = [{name = "Jacob Bronson", email = "bronsoneering@gmail.com"}]
 description = "Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ['propeller', 'design', 'tools', 'computational', 'fluid', 'dynamics', 'CFD', 'STL', 'prop', 'rotor',
             'xrotor', 'xfoil', 'MIT', 'Drela', 'Youngren']
```

