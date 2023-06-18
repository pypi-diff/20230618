# Comparing `tmp/propeller_design_tools-0.4.1.tar.gz` & `tmp/propeller_design_tools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propeller_design_tools-0.4.1.tar", last modified: Sun Jun 18 02:50:50 2023, max compression
+gzip compressed data, was "propeller_design_tools-0.4.2.tar", last modified: Sun Jun 18 03:42:39 2023, max compression
```

## Comparing `propeller_design_tools-0.4.1.tar` & `propeller_design_tools-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,219 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/
--rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     1405 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0    51938 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     9406 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 02:50:50.014140 propeller_design_tools-0.4.1/propdes/
--rw-rw-rw-   0        0        0      374 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/__init__.py
--rw-rw-rw-   0        0        0    28775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/airfoil.py
--rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/custom_opengl_classes.py
--rw-rw-rw-   0        0        0    18318 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/foil_ui_classes.py
--rw-rw-rw-   0        0        0    50326 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/funcs.py
--rw-rw-rw-   0        0        0    17801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16285 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      386 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/opt_ui_classes.py
--rw-rw-rw-   0        0        0    10965 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/optimizations.py
--rw-rw-rw-   0        0        0    15547 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36905 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/prop_creation_ui_classes.py
--rw-rw-rw-   0        0        0    53781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/propeller.py
--rw-rw-rw-   0        0        0    17572 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/radialstation.py
--rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4096 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/settings.py
--rw-rw-rw-   0        0        0     5722 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/user_interface.py
--rw-rw-rw-   0        0        0     2839 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.1/propdes/user_io.py
-drwxrwxrwx   0        0        0        0 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0    51938 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-18 02:50:49.000000 propeller_design_tools-0.4.1/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1866 2023-06-18 02:49:04.000000 propeller_design_tools-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 02:50:50.033308 propeller_design_tools-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.351220 propeller_design_tools-0.4.2/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     1405 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    51068 2023-06-18 03:42:39.351220 propeller_design_tools-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8536 2023-06-18 03:42:01.000000 propeller_design_tools-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.041051 propeller_design_tools-0.4.2/propeller_design_tools/
+-rw-rw-rw-   0        0        0      479 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28820 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.081762 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     1132 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0     2730 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    50416 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16315 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      401 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11040 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15622 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36995 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.081762 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.090841 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.341657 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3802 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3803 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.341657 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.090841 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.162226 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.168275 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.188259 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.262275 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.262275 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53871 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17617 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4111 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.351220 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      236 2023-06-18 03:29:40.000000 propeller_design_tools-0.4.2/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     5857 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2023-06-18 02:23:07.000000 propeller_design_tools-0.4.2/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2023-06-18 03:42:39.072351 propeller_design_tools-0.4.2/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0    51068 2023-06-18 03:42:38.000000 propeller_design_tools-0.4.2/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14426 2023-06-18 03:42:39.000000 propeller_design_tools-0.4.2/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 03:42:38.000000 propeller_design_tools-0.4.2/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-06-18 03:42:38.000000 propeller_design_tools-0.4.2/propeller_design_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-18 03:42:38.000000 propeller_design_tools-0.4.2/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1866 2023-06-18 03:29:37.000000 propeller_design_tools-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 03:42:39.351220 propeller_design_tools-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-06-18 02:25:12.000000 propeller_design_tools-0.4.2/setup.py
```

### Comparing `propeller_design_tools-0.4.1/LICENSE` & `propeller_design_tools-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.1/MANIFEST.in` & `propeller_design_tools-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.1/PKG-INFO` & `propeller_design_tools-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller_design_tools
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -805,78 +805,78 @@
 the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
    )
 
-   ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
-   ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
-   ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
+   ![ex0-1.png](tests/ex0-1.png)
+   ![ex0-2.png](tests/ex0-2.png)
+   ![ex0-3.png](tests/ex0-3.png)
 
 1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
 -> save these files into the "airfoil_database" directory
 
 
 2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
 populate database data for the desired foil sections -> see 
 [example1_airfoil_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
    )
 
-   ![ex1-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-1.png)
-   ![ex1-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-2.png)
+   ![ex1-1.png](tests/ex1-1.png)
+   ![ex1-2.png](tests/ex1-2.png)
 
 
 3. Once the required 2D airfoil data is generated, PDT can then be used
 to automatically generate all the required 2D foil definition parameters
 required by XROTOR (these "station parameters" are essentially what 
 allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
 blade geometries) -> see
 [example2_radialstation_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
    )
 
-   ![ex2-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex2-1.png)
+   ![ex2-1.png](tests/ex2-1.png)
    
    But this step is also automated & displayed by PDT when the user uses
 the builtin PDT propeller creation function -> see
 [example3_prop_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
    )
 
-   ![ex3-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-1.png)
+   ![ex3-1.png](tests/ex3-1.png)
 
    NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
 or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
 these are much faster than the (more accurate) 'vrtx' formulation, which you 
 can then move on to.
 
-   ![ex3-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-2.png)
+   ![ex3-2.png](tests/ex3-2.png)
 
 
 4. PDT's Propeller() object instances can generate 3D geometry files 
 including profle xyz coordinate listings, and .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
-   ![ex4-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex4-1.png)
+   ![ex4-1.png](tests/ex4-1.png)
 
 Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
 using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
 is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
 5. Analyze a given Propeller() instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
-   ![ex5-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex5-1.png)
+   ![ex5-1.png](tests/ex5-1.png)
 
 
 6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
 prop design generation by means of maximizing or minimizing a given output / 
 calculated metric based on outputs, optionally taking into account different
 propeller operating points via the ability to define the propeller's "duty-cycle"
 -> coming soon! This should elimiate the user's need to even input a value for the
```

### Comparing `propeller_design_tools-0.4.1/README.md` & `propeller_design_tools-0.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -107,78 +107,78 @@
 the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
    )
 
-   ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
-   ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
-   ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
+   ![ex0-1.png](tests/ex0-1.png)
+   ![ex0-2.png](tests/ex0-2.png)
+   ![ex0-3.png](tests/ex0-3.png)
 
 1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
 -> save these files into the "airfoil_database" directory
 
 
 2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
 populate database data for the desired foil sections -> see 
 [example1_airfoil_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
    )
 
-   ![ex1-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-1.png)
-   ![ex1-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-2.png)
+   ![ex1-1.png](tests/ex1-1.png)
+   ![ex1-2.png](tests/ex1-2.png)
 
 
 3. Once the required 2D airfoil data is generated, PDT can then be used
 to automatically generate all the required 2D foil definition parameters
 required by XROTOR (these "station parameters" are essentially what 
 allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
 blade geometries) -> see
 [example2_radialstation_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
    )
 
-   ![ex2-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex2-1.png)
+   ![ex2-1.png](tests/ex2-1.png)
    
    But this step is also automated & displayed by PDT when the user uses
 the builtin PDT propeller creation function -> see
 [example3_prop_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
    )
 
-   ![ex3-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-1.png)
+   ![ex3-1.png](tests/ex3-1.png)
 
    NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
 or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
 these are much faster than the (more accurate) 'vrtx' formulation, which you 
 can then move on to.
 
-   ![ex3-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-2.png)
+   ![ex3-2.png](tests/ex3-2.png)
 
 
 4. PDT's Propeller() object instances can generate 3D geometry files 
 including profle xyz coordinate listings, and .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
-   ![ex4-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex4-1.png)
+   ![ex4-1.png](tests/ex4-1.png)
 
 Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
 using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
 is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
 5. Analyze a given Propeller() instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
-   ![ex5-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex5-1.png)
+   ![ex5-1.png](tests/ex5-1.png)
 
 
 6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
 prop design generation by means of maximizing or minimizing a given output / 
 calculated metric based on outputs, optionally taking into account different
 propeller operating points via the ability to define the propeller's "duty-cycle"
 -> coming soon! This should elimiate the user's need to even input a value for the
```

### Comparing `propeller_design_tools-0.4.1/propdes/airfoil.py` & `propeller_design_tools-0.4.2/propeller_design_tools/airfoil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import warnings
-from propdes import funcs
-from propdes.user_io import Error, Info, Warning
-from propdes.settings import get_foil_db
+from propeller_design_tools import funcs
+from propeller_design_tools.user_io import Error, Info, Warning
+from propeller_design_tools.settings import get_foil_db
 import matplotlib
 matplotlib.use('TKAgg')
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.interpolate import griddata, interp1d
```

### Comparing `propeller_design_tools-0.4.1/propdes/custom_opengl_classes.py` & `propeller_design_tools-0.4.2/propeller_design_tools/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.1/propdes/foil_ui_classes.py` & `propeller_design_tools-0.4.2/propeller_design_tools/foil_ui_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from propdes.funcs import delete_all_widgets_from_layout, get_all_airfoil_files, clear_foil_database, \
+from propeller_design_tools.funcs import delete_all_widgets_from_layout, get_all_airfoil_files, clear_foil_database, \
     download_foil_coordinates
-from propdes.airfoil import Airfoil
+from propeller_design_tools.airfoil import Airfoil
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 import numpy as np
 try:
     from PyQt5 import QtWidgets, QtCore
-    from propdes.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_PushButton, PDT_ComboBox, \
+    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_PushButton, PDT_ComboBox, \
         PDT_CheckBox, PDT_LineEdit
-    from propdes.helper_ui_classes import RangeLineEditWidget, SingleAxCanvas, AxesComboBoxWidget, \
+    from propeller_design_tools.helper_ui_classes import RangeLineEditWidget, SingleAxCanvas, AxesComboBoxWidget, \
         Capturing
 except:
     pass
 
 
 class FoilAnalysisWidget(QtWidgets.QWidget):
     def __init__(self, main_win: 'InterfaceMainWindow'):
```

### Comparing `propeller_design_tools-0.4.1/propdes/funcs.py` & `propeller_design_tools-0.4.2/propeller_design_tools/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import subprocess
 import shutil
 import sys
 import urllib.request
 
 import matplotlib.pyplot as plt
 import numpy as np
-from propdes.airfoil import Airfoil
-from propdes.radialstation import RadialStation
-from propdes.propeller import Propeller
-from propdes.user_io import Info, Error, Warning
-from propdes.settings import _get_user_settings, get_prop_db, get_foil_db
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.radialstation import RadialStation
+from propeller_design_tools.propeller import Propeller
+from propeller_design_tools.user_io import Info, Error, Warning
+from propeller_design_tools.settings import _get_user_settings, get_prop_db, get_foil_db
 
 
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
-    from propdes.user_interface import InterfaceMainWindow
+    from propeller_design_tools.user_interface import InterfaceMainWindow
     app = QtWidgets.QApplication(sys.argv)
     w = InterfaceMainWindow()
     w.show()
     app.exec_()
 
 
 def delete_all_widgets_from_layout(layout):
```

### Comparing `propeller_design_tools-0.4.1/propdes/helper_ui_classes.py` & `propeller_design_tools-0.4.2/propeller_design_tools/helper_ui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import subprocess
 
 import numpy as np
 import matplotlib.gridspec as gridspec
-from propdes.settings import get_setting, set_propeller_database, set_airfoil_database, \
+from propeller_design_tools.settings import get_setting, set_propeller_database, set_airfoil_database, \
     get_foil_db, get_prop_db
-from propdes.funcs import count_airfoil_db, count_propeller_db
-from propdes.propeller import Propeller
+from propeller_design_tools.funcs import count_airfoil_db, count_propeller_db
+from propeller_design_tools.propeller import Propeller
 import sys
 from typing import Union
 from io import StringIO
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 try:
     from PyQt5 import QtWidgets, QtCore, QtGui
-    from propdes.helper_ui_subclasses import PDT_Label, PDT_PushButton, PDT_SpinBox, PDT_DoubleSpinBox, \
+    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_PushButton, PDT_SpinBox, PDT_DoubleSpinBox, \
         PDT_ComboBox, PDT_GroupBox, PDT_CheckBox, PDT_TextEdit, PDT_LineEdit, PDT_ScienceSpinBox
 except:
     pass
 
 
 class SingleAxCanvas(FigureCanvasQTAgg):
     def __init__(self, *args, **kwargs):
```

### Comparing `propeller_design_tools-0.4.1/propdes/helper_ui_subclasses.py` & `propeller_design_tools-0.4.2/propeller_design_tools/helper_ui_subclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 try:
     from PyQt5 import QtWidgets, QtGui, QtCore
-    from propdes.settings import _get_cursor_fpath
-    from propdes.science_spinbox_class import ScientificDoubleSpinBox
+    from propeller_design_tools.settings import _get_cursor_fpath
+    from propeller_design_tools.science_spinbox_class import ScientificDoubleSpinBox
 except:
     pass
 
 
 class PDT_GroupBox(QtWidgets.QGroupBox):
     def __init__(self, *args, **kwargs):
         italic = kwargs.pop('italic') if 'italic' in kwargs else False
```

### Comparing `propeller_design_tools-0.4.1/propdes/optimizations.py` & `propeller_design_tools-0.4.2/propeller_design_tools/optimizations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import shutil
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 import pyqtgraph as pg
 from pyqtgraph import opengl as gl
-from propdes import Propeller
-from propdes.user_io import Error
-from propdes.funcs import create_propeller, get_prop_db
-from propdes.user_io import Info, Warning
-from propdes.custom_opengl_classes import Custom3DAxis
+from propeller_design_tools import Propeller
+from propeller_design_tools.user_io import Error
+from propeller_design_tools.funcs import create_propeller, get_prop_db
+from propeller_design_tools.user_io import Info, Warning
+from propeller_design_tools.custom_opengl_classes import Custom3DAxis
 
 
 class VehicleRangeOptimization:
     def __init__(self):
         pass
```

### Comparing `propeller_design_tools-0.4.1/propdes/prop_analysis_ui_classes.py` & `propeller_design_tools-0.4.2/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
 import pyqtgraph.opengl as gl
-from propdes.settings import VALID_OPER_PLOT_PARAMS
-from propdes.funcs import get_all_propeller_dirs
-from propdes.propeller import Propeller
+from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+from propeller_design_tools.funcs import get_all_propeller_dirs
+from propeller_design_tools.propeller import Propeller
 try:
     from PyQt5 import QtWidgets, QtCore
-    from propdes.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
+    from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
         PDT_CheckBox
-    from propdes.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
+    from propeller_design_tools.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
         CheckColumnWidget, AxesComboBoxWidget, RangeLineEditWidget, Capturing
 except:
     pass
 
 
 class PropellerSweepWidget(QtWidgets.QWidget):
     def __init__(self, main_win: 'InterfaceMainWindow'):
```

### Comparing `propeller_design_tools-0.4.1/propdes/prop_creation_ui_classes.py` & `propeller_design_tools-0.4.2/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import subprocess
 import numpy as np
 import os
-from propdes.propeller import Propeller
-from propdes.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
-from propdes.user_io import Error
-from propdes.settings import get_prop_db
+from propeller_design_tools.propeller import Propeller
+from propeller_design_tools.funcs import get_all_propeller_dirs, create_propeller, get_all_airfoil_files
+from propeller_design_tools.user_io import Error
+from propeller_design_tools.settings import get_prop_db
 
 try:
     from PyQt5 import QtWidgets, QtCore
-    from propdes.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
+    from propeller_design_tools.helper_ui_classes import SingleAxCanvas, Capturing, AxesComboBoxWidget, \
         PropellerCreationPanelCanvas, RadialStationFitParamsCanvas
-    from propdes.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
+    from propeller_design_tools.helper_ui_subclasses import PDT_ComboBox, PDT_Label, PDT_SpinBox, PDT_DoubleSpinBox, \
         PDT_PushButton, PDT_LineEdit, PDT_CheckBox
     import pyqtgraph.opengl as gl
 except:
     pass
 
 
 class PropellerCreationWidget(QtWidgets.QWidget):
```

### Comparing `propeller_design_tools-0.4.1/propdes/propeller.py` & `propeller_design_tools-0.4.2/propeller_design_tools/propeller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
-from propdes import funcs
-from propdes.user_io import Info, Error, Warning
-from propdes.settings import get_setting
-from propdes.airfoil import Airfoil
-from propdes.settings import VALID_OPER_PLOT_PARAMS
-from propdes.custom_opengl_classes import Custom3DArrow
+from propeller_design_tools import funcs
+from propeller_design_tools.user_io import Info, Error, Warning
+from propeller_design_tools.settings import get_setting
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
+from propeller_design_tools.custom_opengl_classes import Custom3DArrow
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gridspec
 from mpl_toolkits import mplot3d
 import numpy as np
 from stl import mesh
 from typing import Union
 import pyqtgraph as pg
```

### Comparing `propeller_design_tools-0.4.1/propdes/radialstation.py` & `propeller_design_tools-0.4.2/propeller_design_tools/radialstation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from propdes import funcs
-from propdes.airfoil import Airfoil
-from propdes.user_io import Info, Error
+from propeller_design_tools import funcs
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.user_io import Info, Error
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.optimize import curve_fit
 
 
 class RadialStation(object):
```

### Comparing `propeller_design_tools-0.4.1/propdes/science_spinbox_class.py` & `propeller_design_tools-0.4.2/propeller_design_tools/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.1/propdes/settings.py` & `propeller_design_tools-0.4.2/propeller_design_tools/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import os
-from propdes.user_io import Error, Input, Info
+from propeller_design_tools.user_io import Error, Input, Info
 import pkg_resources
 
 
 VALID_OPER_PLOT_PARAMS = ['adv. ratio', 'J', 'speed(m/s)', 'rpm', 'thrust(N)', 'power(W)', 'torque(N-m)', 'Efficiency',
                           'Eff induced', 'Eff ideal', 'Pvisc(W)', 'Ct', 'Tc', 'Cp', 'Pc', 'Sigma']
```

### Comparing `propeller_design_tools-0.4.1/propdes/user_interface.py` & `propeller_design_tools-0.4.2/propeller_design_tools/user_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 import os
 import subprocess
-from propdes.airfoil import Airfoil
-from propdes.settings import _get_cursor_fpath, _get_gunshot_fpaths
-from propdes.funcs import get_all_airfoil_files, get_all_propeller_dirs
+from propeller_design_tools.airfoil import Airfoil
+from propeller_design_tools.settings import _get_cursor_fpath, _get_gunshot_fpaths
+from propeller_design_tools.funcs import get_all_airfoil_files, get_all_propeller_dirs
 try:
     from PyQt5 import QtWidgets, QtGui, QtCore, QtMultimedia
-    from propdes.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
+    from propeller_design_tools.helper_ui_classes import Capturing, DatabaseSelectionWidget, SingleAxCanvas, \
         AxesComboBoxWidget, PdtGuiPrinter
-    from propdes.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
-    from propdes.prop_creation_ui_classes import PropellerCreationWidget
-    from propdes.prop_analysis_ui_classes import PropellerSweepWidget
-    from propdes.opt_ui_classes import OptimizationWidget
-    from propdes.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
+    from propeller_design_tools.foil_ui_classes import ExistingFoilDataWidget, FoilAnalysisWidget, AddFoilDataPointWidget
+    from propeller_design_tools.prop_creation_ui_classes import PropellerCreationWidget
+    from propeller_design_tools.prop_analysis_ui_classes import PropellerSweepWidget
+    from propeller_design_tools.opt_ui_classes import OptimizationWidget
+    from propeller_design_tools.helper_ui_subclasses import PDT_TextEdit, PDT_GroupBox, PDT_Label, PDT_PushButton, \
         PDT_ComboBox, PDT_TabWidget
 except:
     pass
 
 
 class InterfaceMainWindow(QtWidgets.QMainWindow):
     def __init__(self, foil: Airfoil = None):
```

### Comparing `propeller_design_tools-0.4.1/propdes/user_io.py` & `propeller_design_tools-0.4.2/propeller_design_tools/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.4.1/propeller_design_tools.egg-info/PKG-INFO` & `propeller_design_tools-0.4.2/propeller_design_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller-design-tools
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR.
 Author-email: Jacob Bronson <bronsoneering@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -805,78 +805,78 @@
 the PDT package):
 
 0. Try out the (currently extremely buggy and incomplete) user interface!
 [example0_user_interface.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example0_user_interface.py
    )
 
-   ![ex0-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-1.png)
-   ![ex0-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-2.png)
-   ![ex0-3.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex0-3.png)
+   ![ex0-1.png](tests/ex0-1.png)
+   ![ex0-2.png](tests/ex0-2.png)
+   ![ex0-3.png](tests/ex0-3.png)
 
 1. Obtain normalized airfoil coordinate files from
 [UIUC Database](https://m-selig.ae.illinois.edu/ads/coord_database.html)
 -> save these files into the "airfoil_database" directory
 
 
 2. Use PDT to run XFOIL across ranges of Reynolds Numbers in order to
 populate database data for the desired foil sections -> see 
 [example1_airfoil_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example1_airfoil_analysis.py
    )
 
-   ![ex1-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-1.png)
-   ![ex1-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex1-2.png)
+   ![ex1-1.png](tests/ex1-1.png)
+   ![ex1-2.png](tests/ex1-2.png)
 
 
 3. Once the required 2D airfoil data is generated, PDT can then be used
 to automatically generate all the required 2D foil definition parameters
 required by XROTOR (these "station parameters" are essentially what 
 allow XROTOR to model the performance of well-behaved, arbitrarily-lofted 
 blade geometries) -> see
 [example2_radialstation_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example2_radialstation_creation.py
    )
 
-   ![ex2-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex2-1.png)
+   ![ex2-1.png](tests/ex2-1.png)
    
    But this step is also automated & displayed by PDT when the user uses
 the builtin PDT propeller creation function -> see
 [example3_prop_creation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example3_prop_creation.py
    )
 
-   ![ex3-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-1.png)
+   ![ex3-1.png](tests/ex3-1.png)
 
    NOTE: It is highly recommended to first run XROTOR using either the 'grad' 
 or the 'pot' vortex formulation in order to get your design "tweaked in" -> 
 these are much faster than the (more accurate) 'vrtx' formulation, which you 
 can then move on to.
 
-   ![ex3-2.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex3-2.png)
+   ![ex3-2.png](tests/ex3-2.png)
 
 
 4. PDT's Propeller() object instances can generate 3D geometry files 
 including profle xyz coordinate listings, and .stl 3D geometry files -> see
 [example4_stl_generation.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example4_stl_generation.py
    )
 
-   ![ex4-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex4-1.png)
+   ![ex4-1.png](tests/ex4-1.png)
 
 Note: It is known that currently there is an issue with these .stl files opening in SolidWorks -> try converting them
 using anything (first idea is MS Paint, I think the new version can save STL files as well).  As far as I can tell this 
 is only an issue for SolidWorks users on Windows, these files open and display fine in every other application.
 
 5. Analyze a given Propeller() instance across a sweep of operating points -> see 
 [example5_prop_analysis.py](
    https://github.com/helloDestroyerOfWorlds/propeller_design_tools/blob/master/tests/example5_prop_analysis.py
    )
 
-   ![ex5-1.png](https://raw.githubusercontent.com/helloDestroyerOfWorlds/propeller_design_tools/master/tests/ex5-1.png)
+   ![ex5-1.png](tests/ex5-1.png)
 
 
 6. **WIP** Prop optimization (grid-search style generic optimizer for "optimal"
 prop design generation by means of maximizing or minimizing a given output / 
 calculated metric based on outputs, optionally taking into account different
 propeller operating points via the ability to define the propeller's "duty-cycle"
 -> coming soon! This should elimiate the user's need to even input a value for the
```

### Comparing `propeller_design_tools-0.4.1/pyproject.toml` & `propeller_design_tools-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.8.0", "wheel>=0.40.0"]  # build requirements (don't include build or twine)
 build-backend = "setuptools.build_meta"
 
 
 [project]
-version = "0.4.1"
+version = "0.4.2"
 name = "propeller_design_tools"
 authors = [{name = "Jacob Bronson", email = "bronsoneering@gmail.com"}]
 description = "Python 3.7 package that provides exactly what it sounds like by automating usage of MIT professor Mark Drela's GNU-licensed CLI-utilities XFOIL and XROTOR."
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ['propeller', 'design', 'tools', 'computational', 'fluid', 'dynamics', 'CFD', 'STL', 'prop', 'rotor',
             'xrotor', 'xfoil', 'MIT', 'Drela', 'Youngren']
```

