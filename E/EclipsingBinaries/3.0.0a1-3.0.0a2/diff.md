# Comparing `tmp/EclipsingBinaries-3.0.0a1.tar.gz` & `tmp/EclipsingBinaries-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.0.0a1.tar", last modified: Fri Jun 16 18:03:20 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.0.0a2.tar", last modified: Fri Jun 16 18:12:14 2023, max compression
```

## Comparing `EclipsingBinaries-3.0.0a1.tar` & `EclipsingBinaries-3.0.0a2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.653333 EclipsingBinaries-3.0.0a1/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-16 18:03:02.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 18:03:20.000000 EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:03:20.657333 EclipsingBinaries-3.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-16 18:03:08.000000 EclipsingBinaries-3.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    22604 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/setup.py
```

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/IRAF_Reduction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Kyle Koeller
 Created: 11/08/2022
-Last Edited: 05/09/2023
+Last Edited: 06/15/2023
 
 This program is meant to automatically do the data reduction of the raw images from the
 Ball State University Observatory (BSUO) and SARA data. The new calibrated images are placed into a new folder as to
 not overwrite the original images.
 """
 # import sys
 from pathlib import Path
@@ -36,65 +36,92 @@
 gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
 overwrite = True  # if the user wants to overwrite already existing files or not, by default it is set to True
 mem_limit = 1600e6  # maximum memory limit 4.5 Gb is the recommended which is 450e6 (i.e. 8.0 Gb would be 800e6)
 dark_bool = "True"
 location = "bsuo"
 
 
-def main():
+def main(path="", pipeline=False):
     """
     This function calls all other functions in order of the calibration.
 
+    :param path: the path to the raw images
+    :param pipeline: if the user wants to use the pipeline or not
+
     :return: outputs all calibration images into a new reduced folder designated by the user.
     """
 
-    # allows the user to input where the raw images are and where the calibrated images go to
-    path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the raw images are or type "
-                 "the word 'Close' to leave: ")
-    # path = "C:\\Users\\Kyle\\OneDrive\\PhysicsAstro\\Astronomy\\Code\\IRAF\\Calibration"
-    if path.lower() == "close":
-        exit()
-    # path = "Calibration2"
-    calibrated = input("Please enter a file pathway for a new calibrated folder to not overwrite the original images "
-                       "(C:\\folder1\\folder2\\[calibrated]): ")
-    # calibrated = "C:\\test"
-    # checks whether the file paths from above are real
-    while True:
-        try:
-            images_path = Path(path)
-            calibrated_data = Path(calibrated)
-            break
-        except FileNotFoundError:
-            print("Files were not found. Please try again.\n")
-            path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
-            calibrated = input("Please enter a name for a new calibrated folder to not overwrite the original images: ")
-
-    print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
-    while True:
-        default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
-        # default_ans = "default"
-        if default_ans.lower() == "default":
-            break
-        elif default_ans.lower() == "new":
-            default()
-            break
+    if not pipeline:
+        # allows the user to input where the raw images are and where the calibrated images go to
+        path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the raw images are or type "
+                     "the word 'Close' to leave: ")
+        # path = "C:\\Users\\Kyle\\OneDrive\\PhysicsAstro\\Astronomy\\Code\\IRAF\\Calibration"
+        if path.lower() == "close":
+            exit()
+        # path = "Calibration2"
+        calibrated = input("Please enter a file pathway for a new calibrated folder to not overwrite the original images "
+                           "(C:\\folder1\\folder2\\[calibrated]): ")
+        # calibrated = "C:\\test"
+        # checks whether the file paths from above are real
+        while True:
+            try:
+                images_path = Path(path)
+                calibrated_data = Path(calibrated)
+                break
+            except FileNotFoundError:
+                print("Files were not found. Please try again.\n")
+                path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
+                calibrated = input("Please enter a name for a new calibrated folder to not overwrite the original images: ")
+
+        print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
+        while True:
+            default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
+            # default_ans = "default"
+            if default_ans.lower() == "default":
+                break
+            elif default_ans.lower() == "new":
+                default()
+                break
+            else:
+                print("Please either enter 'Default' or 'New'.\n")
+
+        calibrated_data.mkdir(exist_ok=True)
+        files = ccdp.ImageFileCollection(images_path)
+
+        zero, overscan_region, trim_region = bias(files, calibrated_data, path)
+        if not dark_bool:
+            master_dark = None
         else:
-            print("Please either enter 'Default' or 'New'.\n")
-
-    calibrated_data.mkdir(exist_ok=True)
-    files = ccdp.ImageFileCollection(images_path)
+            master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
 
-    zero, overscan_region, trim_region = bias(files, calibrated_data, path)
-    if not dark_bool:
-        master_dark = None
+        flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
+        science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
     else:
-        master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
-
-    flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
-    science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
+        calibrated = input(
+            "Please enter a file pathway for a new calibrated folder to not overwrite the original images "
+            "(C:\\folder1\\folder2\\[calibrated]): ")
+        # calibrated = "C:\\test"
+        # checks whether the file paths from above are real
+        while True:
+            try:
+                images_path = Path(path)
+                calibrated_data = Path(calibrated)
+                break
+            except FileNotFoundError:
+                print("Files were not found. Please try again.\n")
+                path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
+                calibrated = input(
+                    "Please enter a name for a new calibrated folder to not overwrite the original images: ")
+
+        calibrated_data.mkdir(exist_ok=True)
+        files = ccdp.ImageFileCollection(images_path)
+
+        zero, overscan_region, trim_region = bias(files, calibrated_data, path)
+        flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
+        science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
 
 
 def default():
     """
     Generates new values that the user can enter
 
     :return: newly entered default values
```

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-3.0.0a1/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 EclipsingBinaries/__init__.py
 EclipsingBinaries/apass.py
 EclipsingBinaries/color_light_curve.py
 EclipsingBinaries/find_min.py
 EclipsingBinaries/gaia.py
 EclipsingBinaries/menu.py
 EclipsingBinaries/multi_aperture_photometry.py
+EclipsingBinaries/pipeline.py
 EclipsingBinaries/tess_data_search.py
 EclipsingBinaries/tesscut.py
 EclipsingBinaries/vseq_updated.py
 EclipsingBinaries.egg-info/PKG-INFO
 EclipsingBinaries.egg-info/SOURCES.txt
 EclipsingBinaries.egg-info/dependency_links.txt
 EclipsingBinaries.egg-info/entry_points.txt
```

### Comparing `EclipsingBinaries-3.0.0a1/LICENSE` & `EclipsingBinaries-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/PKG-INFO` & `EclipsingBinaries-3.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-3.0.0a1/README.md` & `EclipsingBinaries-3.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a1/setup.py` & `EclipsingBinaries-3.0.0a2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python
 
 """Setup script for the package."""
 
 from setuptools import setup, find_packages  # Always prefer setuptools over distutils
 import sys
 import codecs
-import os.path
+import os
 
 from pathlib import Path
 
+# print("Current working directory:", os.getcwd())
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 MINIMUM_PYTHON_VERSION = 3, 8
 
 
 def read(rel_path):
@@ -32,14 +34,19 @@
 
 def check_python_version():
     """Exit when the Python version is too low."""
     if sys.version_info < MINIMUM_PYTHON_VERSION:
         sys.exit("Python {}.{}+ is required.".format(*MINIMUM_PYTHON_VERSION))
 
 
+def debug_print_init_contents():
+    print(f"::debug::{read('EclipsingBinaries/__init__.py')}")
+
+# debug_print_init_contents()
+
 check_python_version()
 version = get_version("EclipsingBinaries/__init__.py")
 
 setup(
     version=version,
     name="EclipsingBinaries",
     description="Binary Star Package for Ball State University's Astronomy Research Group",
@@ -47,15 +54,16 @@
     long_description_content_type='text/markdown',
     url='https://github.com/kjkoeller/EclipsingBinaries',
     author='Kyle Koeller',
 
     # packages=find_packages(),
 
     entry_points={'console_scripts': [
-        'EclipsingBinaries = EclipsingBinaries.menu:main'
+        'EclipsingBinaries = EclipsingBinaries.menu:main',
+        'EB_pipeline = EclipsingBinaries.pipeline:monitor_directory'
     ],
     },
 
     license="MIT",
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Natural Language :: English',
```

