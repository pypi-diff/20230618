# Comparing `tmp/EclipsingBinaries-3.0.0a2.tar.gz` & `tmp/EclipsingBinaries-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-3.0.0a2.tar", last modified: Fri Jun 16 18:12:14 2023, max compression
+gzip compressed data, was "EclipsingBinaries-3.1.0.tar", last modified: Sun Jun 18 20:32:29 2023, max compression
```

## Comparing `EclipsingBinaries-3.0.0a2.tar` & `EclipsingBinaries-3.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    22604 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-16 18:11:45.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 18:12:14.000000 EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:12:14.671277 EclipsingBinaries-3.0.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-16 18:11:51.000000 EclipsingBinaries-3.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.407487 EclipsingBinaries-3.1.0/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    24369 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-18 20:32:06.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25259 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 20:32:29.000000 EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 20:32:29.411487 EclipsingBinaries-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-18 20:32:12.000000 EclipsingBinaries-3.1.0/setup.py
```

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/IRAF_Reduction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Kyle Koeller
 Created: 11/08/2022
-Last Edited: 06/15/2023
+Last Edited: 06/17/2023
 
 This program is meant to automatically do the data reduction of the raw images from the
 Ball State University Observatory (BSUO) and SARA data. The new calibrated images are placed into a new folder as to
 not overwrite the original images.
 """
 # import sys
 from pathlib import Path
@@ -36,24 +36,26 @@
 gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
 overwrite = True  # if the user wants to overwrite already existing files or not, by default it is set to True
 mem_limit = 1600e6  # maximum memory limit 4.5 Gb is the recommended which is 450e6 (i.e. 8.0 Gb would be 800e6)
 dark_bool = "True"
 location = "bsuo"
 
 
-def main(path="", pipeline=False):
+def main(path="", calibrated="", pipeline=False, location="", dark_bool=True):
     """
     This function calls all other functions in order of the calibration.
 
     :param path: the path to the raw images
+    :param calibrated: the path to the calibrated images
     :param pipeline: if the user wants to use the pipeline or not
+    :param location: the location of the telescope
+    :param dark_bool: if the user wants to use dark frames or not
 
     :return: outputs all calibration images into a new reduced folder designated by the user.
     """
-
     if not pipeline:
         # allows the user to input where the raw images are and where the calibrated images go to
         path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the raw images are or type "
                      "the word 'Close' to leave: ")
         # path = "C:\\Users\\Kyle\\OneDrive\\PhysicsAstro\\Astronomy\\Code\\IRAF\\Calibration"
         if path.lower() == "close":
             exit()
@@ -68,63 +70,127 @@
                 calibrated_data = Path(calibrated)
                 break
             except FileNotFoundError:
                 print("Files were not found. Please try again.\n")
                 path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
                 calibrated = input("Please enter a name for a new calibrated folder to not overwrite the original images: ")
 
-        print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
-        while True:
-            default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
-            # default_ans = "default"
-            if default_ans.lower() == "default":
-                break
-            elif default_ans.lower() == "new":
-                default()
-                break
-            else:
-                print("Please either enter 'Default' or 'New'.\n")
+        if location.lower() == "kpno":
+            kpno()
+        elif location.lower() == "ctio":
+            ctio()
+        elif lapalma():
+            lapalma()
+        elif location.lower() == "bsuo":
+            pass
+        else:
+            print("\nDo you want to load default options like gain and read noise? The defaults are for BSUO")
+            while True:
+                default_ans = input("To load defaults type 'Default' otherwise type 'New' to enter values: ")
+                # default_ans = "default"
+                if default_ans.lower() == "default":
+                    break
+                elif default_ans.lower() == "new":
+                    new_default()
+                    break
+                else:
+                    print("Please either enter 'Default' or 'New'.\n")
 
         calibrated_data.mkdir(exist_ok=True)
         files = ccdp.ImageFileCollection(images_path)
 
-        zero, overscan_region, trim_region = bias(files, calibrated_data, path)
+        zero, overscan_region, trim_region = bias(files, calibrated_data, path, pipeline)
         if not dark_bool:
             master_dark = None
         else:
             master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
 
         flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
         science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
     else:
-        calibrated = input(
-            "Please enter a file pathway for a new calibrated folder to not overwrite the original images "
-            "(C:\\folder1\\folder2\\[calibrated]): ")
-        # calibrated = "C:\\test"
         # checks whether the file paths from above are real
         while True:
             try:
                 images_path = Path(path)
                 calibrated_data = Path(calibrated)
                 break
             except FileNotFoundError:
                 print("Files were not found. Please try again.\n")
                 path = input("Please enter a file path or folder name (if this code is in the same main folder): ")
                 calibrated = input(
                     "Please enter a name for a new calibrated folder to not overwrite the original images: ")
 
+        if location.lower() == "kpno":
+            kpno()
+        elif location.lower() == "ctio":
+            ctio()
+        elif lapalma():
+            lapalma()
+        elif location.lower() == "bsuo":
+            pass
+
         calibrated_data.mkdir(exist_ok=True)
         files = ccdp.ImageFileCollection(images_path)
 
-        zero, overscan_region, trim_region = bias(files, calibrated_data, path)
+        zero, overscan_region, trim_region = bias(files, calibrated_data, path, pipeline)
+        if not dark_bool:
+            master_dark = None
+        else:
+            master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
+
         flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
         science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
 
 
-def default():
+def kpno():
+    """
+    Kitt Peak National Observatory default values
+
+    :return: None
+    """
+    global gain
+    global rdnoise
+    global dark_bool
+
+    gain = 2.3
+    rdnoise = 6.0
+    dark_bool = True
+
+
+def ctio():
+    """
+    Cerro Tololo Inter-American Observatory default values
+
+    :return: None
+    """
+    global gain
+    global rdnoise
+    global dark_bool
+
+    gain = 2.0
+    rdnoise = 9.7
+    dark_bool = True
+
+
+def lapalma():
+    """
+    La Palma default values
+
+    :return: None
+    """
+    global gain
+    global rdnoise
+    global dark_bool
+
+    gain = 1.0
+    rdnoise = 6.3
+    dark_bool = True
+
+
+def new_default():
     """
     Generates new values that the user can enter
 
     :return: newly entered default values
     """
     global sigma_clip_high_thresh
     global sigma_clip_low_thresh
@@ -144,15 +210,15 @@
     rdnoise = float(input("Enter a readnoise value, default is '10.83' electrons: "))
     sigclip = int(input("Enter a sigma clip value for cosmic ray removal, default is '5': "))
     dark_bool = input("Are you using Dark Frames, default is True (enter 'True' or 'False'): ")
     if dark_bool.lower == "false":
         dark_bool = False
     elif dark_bool.lower == "true":
         dark_bool = True
-    location = input("What is your observation location, default is bsuo (ctip, kpno, lapalma")
+    location = input("What is your observation location, default is bsuo (ctio, kpno, lapalma")
 
 
 def reduce(ccd, overscan_region, trim_region, num, zero, combined_dark, good_flat):
     """
     This function takes the information for each section of the reduction process into a singular function for
     limits in duplication of the code.
 
@@ -219,49 +285,55 @@
 
         # cosmic ray reject above 5 sigmas and gain_apply is set to false because it changes the units of the image
         # new_reduced = ccdp.cosmicray_lacosmic(reduced, gain_apply=False, readnoise=rdnoise, gain=gain, sigclip=sigclip)
 
         return reduced
 
 
-def bias(files, calibrated_data, path):
+def bias(files, calibrated_data, path, pipeline):
     """
     Calibrates the bias images
 
     :param path: the raw images folder path
     :param files: file location where all raw images are
     :param calibrated_data: file location where the new images go
+    :param pipeline: true or false for pipeline usage
+
     :return: the combined bias image and the trim and overscan regions
     """
 
     # plots one of the flat image mean count values across all columns to find the trim and overscan regions
-    print("\n\nThe flat image that you enter next should be inside the " + "\033[1m" + "\033[93m" + "FIRST" +
-          "\033[00m" + " folder that you entered above or this will crash.")
-    while True:
-        try:
-            # image = input(
-            #     "Please enter the name of one of the flat image to be looked at for overscan and data regions: ")
-            image = "Flat-Empty-B-Bin2-001-NoGEM.fts"
-            cryo_path = Path(path)
-            bias_1 = CCDData.read(cryo_path / image, unit='adu')
-            break
-        except FileNotFoundError:
-            print("\nThe file you entered could not be found, please try entering " 
-                  "\033[1m" + "\033[93m" + "JUST" + "\033[00m" + " the file name only.\n")
-    # bias_1 = CCDData.read(cryo_path / 'bias-0001.fits', unit='adu')  # testing
-
-    print("\n\nFor the overscan region, [columns, rows], and if you want all the columns then you want would enter, \n"
-          "[1234:5678, 1234:5678] and this would say rows between those values and all the columns. \n"
-          "This would also work if you wanted all the columns ([: , 1234:5678]).\n")
-    bias_plot(bias_1)
-
-    overscan_region = input("Please enter the overscan region you determined from the figure.\n"
-                            "Example '[2073:2115, :]' or if you do not have an overscan region enter 'None': ")
-    trim_region = input("Please enter the data section. Example '[20:2060, 12:2057]': ")
-    print()
+    if not pipeline:
+        print("\n\nThe flat image that you enter next should be inside the " + "\033[1m" + "\033[93m" + "FIRST" +
+              "\033[00m" + " folder that you entered above or this will crash.")
+        while True:
+            try:
+                image = input(
+                    "Please enter the name of one of the flat image to be looked at for overscan and data regions: ")
+                # image = "Flat-Empty-B-Bin2-001-NoGEM.fts"  # testing
+                cryo_path = Path(path)
+                bias_1 = CCDData.read(cryo_path / image, unit='adu')
+                break
+            except FileNotFoundError:
+                print("\nThe file you entered could not be found, please try entering " 
+                      "\033[1m" + "\033[93m" + "JUST" + "\033[00m" + " the file name only.\n")
+        # bias_1 = CCDData.read(cryo_path / 'bias-0001.fits', unit='adu')  # testing
+
+        print("\n\nFor the overscan region, [columns, rows], and if you want all the columns then you want would enter, \n"
+              "[1234:5678, 1234:5678] and this would say rows between those values and all the columns. \n"
+              "This would also work if you wanted all the columns ([: , 1234:5678]).\n")
+        bias_plot(bias_1)
+
+        overscan_region = input("Please enter the overscan region you determined from the figure.\n"
+                                "Example '[2073:2115, :]' or if you do not have an overscan region enter 'None': ")
+        trim_region = input("Please enter the data section. Example '[20:2060, 12:2057]': ")
+        print()
+    else:
+        overscan_region = "[2073:2115, :]"
+        trim_region = "[20:2060, 12:2057]"
 
     print("\nStarting overscan on bias.\n")
     for ccd, file_name in files.ccds(imagetyp='BIAS', return_fname=True, ccd_kwargs={'unit': 'adu'}):
         new_ccd = reduce(ccd, overscan_region, trim_region, 0, zero=None, combined_dark=None, good_flat=None)
 
         list_of_words = file_name.split(".")
         new_fname = "{}.fits".format(list_of_words[0])
@@ -487,14 +559,17 @@
             obs_location = {
                 'lon': -85.411896,  # degrees
                 'lat': 40.199879,  # degrees
                 'elevation': 0.2873  # kilometers
             }
             bjd = BJD_TDB(hjd, obs_location, ra, dec)
             fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
+        else:
+            bjd = BJD_TDB(hjd, location, ra, dec)
+            fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
 
 
 def BJD_TDB(hjd, loc, ra, dec):
     """
     Converts HJD to BJD_TDB
 
     :param ra: right ascension of target object
```

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/apass.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/apass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Combines all APASS programs that were originally separate on GitHub for an easy editing and less to load per file.
 
 Author: Kyle Koeller
 Created: 12/26/2022
-Last Updated: 05/19/2023
+Last Updated: 06/17/2023
 """
 
 from astroquery.vizier import Vizier
 import numpy as np
 import pandas as pd
 
 import astropy.units as u
@@ -29,51 +29,66 @@
 
 
 # turn off this warning that just tells the user,
 # "The warning raised when the contents of the FITS header have been modified to be standards compliant."
 warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 
-def comparison_selector():
+def comparison_selector(ra, dec, pipeline, folder_path, obj_name):
     """
     This code compares AIJ found stars (given an RA and DEC) to APASS stars to get their respective Johnson B, V, and
     Cousins R values and their respective errors.
 
     This code is not 100% accurate and will still need the human eye to compare the final list to the AIJ given list. As
     this code can only get down to such an accuracy to be effective in gathering stars to be usable.
 
+    :param ra: The right ascension of the target
+    :param dec: The declination of the target
+    :param pipeline: The pipeline that is being used
+    :param folder_path: The path of the folder where the images are going to
+    :param obj_name: The name of the target object
+
     :return: A list of stars that are the most likely to be on the AIJ list of stars
     """
 
-    apass_file, input_ra, input_dec, T_list = cousins_r()
+    apass_file, input_ra, input_dec, T_list = cousins_r(ra, dec, pipeline, folder_path, obj_name)
     df = pd.read_csv(apass_file, header=None, skiprows=[0], sep="\t")
 
-    print("Finished Saving\n\n\n")
+    print("Finished Saving\n\n")
     print("The output file you have entered has RA and DEC for stars and their B, V, Cousins R, and TESS T magnitudes "
           "with their respective errors.\n")
 
-    create_radec(df, input_ra, input_dec, T_list)
+    create_radec(df, input_ra, input_dec, T_list, pipeline, folder_path, obj_name)
 
-    overlay(df, input_ra, input_dec)
+    if not pipeline:
+        overlay(df, input_ra, input_dec)
+    else:
+        pass
 
 
-def cousins_r():
+def cousins_r(ra, dec, pipeline, folder_path, obj_name):
     """
     Calculates the Cousins R_c value for a given B, V, g', and r' from APASS
 
+    :param ra: The right ascension of the target
+    :param dec: The declination of the target
+    :param pipeline: The pipeline that is being used
+    :param folder_path: The path of the folder where the images are going to
+    :param obj_name: The name of the target object
+
     :return: Outputs a file to be used for R_c values
     """
     # predefined values DO NOT change
     alpha = 0.278
     e_alpha = 0.016
     beta = 1.321
     e_beta = 0.03
     gamma = 0.219
 
-    input_file, input_ra, input_dec = catalog_finder()
+    input_file, input_ra, input_dec = catalog_finder(ra, dec, pipeline, folder_path, obj_name)
     df = pd.read_csv(input_file, header=None, skiprows=[0], sep=",")
 
     # writes the columns from the input file
     try:
         # this try except function checks whether there are just enough columns in the file being loaded and tells
         # the user what they need to do in order to get the correct columns
         ra = df[0]
@@ -109,14 +124,15 @@
             # if there is a value then format that value with only 2 decimal places otherwise there will be like 8
             Rc.append(format(val, ".2f"))
             e_Rc.append(format(root, ".2f"))
         count += 1
 
     ra_decimal = np.array(splitter(ra))
     dec_decimal = np.array(splitter(dec))
+    print("Starting Gaia Search for TESS Magnitudes\n")
     T_list, T_err_list = ga(ra_decimal, dec_decimal)
 
     # puts all columns into a dataframe for output
     final = pd.DataFrame({
         # need to keep RA and DEC in order to compare with catalog comparison or with the radec file
         "RA": ra,
         "DEC": dec,
@@ -125,28 +141,31 @@
         "VMag": V,
         "e_VMag": e_V,
         "Rc": Rc,
         "e_Rc": e_Rc,
         "TMag": T_list,
         "e_TMag": T_err_list
     })
-    print(
-        "\nThis output file contains all the calculated Cousins R magnitudes along with error and "
-        "both Johnson bands and respective errors.\n")
-    # saves the dataframe to an entered output file
-    output_file = input("Enter an output file name and location for the finalized catalog file "
-                        "(ex: C:\\folder1\\folder2\\APASS_254037_Catalog.txt): ")
+    if not pipeline:
+        print(
+            "\nThis output file contains all the calculated Cousins R magnitudes along with error and "
+            "both Johnson bands and respective errors.\n")
+        # saves the dataframe to an entered output file
+        output_file = input("Enter an output file name and location for the finalized catalog file "
+                            "(ex: C:\\folder1\\folder2\\APASS_254037_Catalog.txt): ")
+    else:
+        output_file = folder_path + "\\" + obj_name + "_APASS_Catalog.txt"
     # noinspection PyTypeChecker
     final.to_csv(output_file, index=True, sep="\t")
     print("\nCompleted Save.\n")
 
     return output_file, input_ra, input_dec, T_list
 
 
-def catalog_finder():
+def catalog_finder(ra, dec, pipeline, folder_path, obj_name):
     """
     This looks at a region of the sky at the decimal coordinates of an object and gathers the "column" data with
     "column filters"
     You can change the columns or the column filters to whatever you like, I have these set as they are because of the
     telescope that was used (Rooftop)
 
     I also set the width of the search radius to larger than what you would actually see in the field of view of any
@@ -155,21 +174,31 @@
     Main things to change are:
     "columns"- what factors are actually taken from the online catalog
     "column_filters"- which stars are to actually be extracted from that online data table and narrows list down from a
     couple of hundred to like 50-60
     "ra"/"dec"- must be in decimal notation
     "width"- set to the notation that is currently set as, but you may change the number being used
             30m = 30 arc-minutes
+
+    :param ra: decimal notation of the RA of the object
+    :param dec: decimal notation of the DEC of the object
+    :param pipeline: the pipeline that is being used (ex: "TESS")
+    :param folder_path: the path to the folder that you want to save the file to
+    :param obj_name: the name of the object that you are looking at
+
+    :return: outputs a file with the columns and column filters that you have chosen
     """
-    # 00:28:27.9684836736 78:57:42.657327180
-    # 13:27:50.4728234064 75:39:45.384765984
-    ra_input = input("Enter the RA of your system (HH:MM:SS.SSSS): ")
-    dec_input = input("Enter the DEC of your system (DD:MM:SS.SSSS or -DD:MM:SS.SSSS): ")
-    # ra_input = "00:28:27.9684836736"  # testing
-    # dec_input = "78:57:42.657327180"  # testing
+    if not pipeline:
+        ra_input = input("Enter the RA of your system (HH:MM:SS.SSSS): ")
+        dec_input = input("Enter the DEC of your system (DD:MM:SS.SSSS or -DD:MM:SS.SSSS): ")
+        # ra_input = "00:28:27.9684836736"  # testing
+        # dec_input = "78:57:42.657327180"  # testing
+    else:
+        ra_input = ra
+        dec_input = dec
 
     ra_input2 = splitter([ra_input])
     dec_input2 = splitter([dec_input])
 
     result = Vizier(
         columns=['_RAJ2000', '_DEJ2000', 'Vmag', "e_Vmag", 'Bmag', "e_Bmag", "g'mag", "e_g'mag", "r'mag", "e_r'mag"],
         row_limit=-1,
@@ -240,35 +269,42 @@
         "e_Vmag": e_vmag_new,
         "g'mag": gmag_new,
         "e_g'mag": e_gmag_new,
         "r'mag": rmag_new,
         "e_r'mag": e_rmag_new
     })
 
-    # saves the dataframe to a text file and prints that dataframe out to easily see what was copied to the text file
-    print(
-        "\n\nThis output file contains all the Vizier magnitudes that will be used to calculate the Cousins R band, and\n"
-        "should not be used for anything else other than calculation confirmation if needed later on.\n")
-    text_file = input("Enter a text file pathway and name for the output comparisons "
-                      "(ex: C:\\folder1\\APASS_254037.txt): ")
-    # text_file = "APASS_254037.txt"  # testing
+    if not pipeline:
+        # saves the dataframe to a text file and prints that dataframe out to easily see what was copied to the text file
+        print(
+            "\n\nThis output file contains all the Vizier magnitudes that will be used to calculate the Cousins R band, and\n"
+            "should not be used for anything else other than calculation confirmation if needed later on.\n")
+        text_file = input("Enter a text file pathway and name for the output comparisons "
+                          "(ex: C:\\folder1\\APASS_254037.txt): ")
+        # text_file = "APASS_254037.txt"  # testing
+    else:
+        text_file = folder_path + "\\APASS_" + obj_name + ".txt"
+
     df.to_csv(text_file, index=None)
     print("\nCompleted save.\n")
 
     return text_file, ra_input2[0], dec_input2[0]
 
 
-def create_radec(df, ra, dec, T_list):
+def create_radec(df, ra, dec, T_list, pipeline, folder_path, obj_name):
     """
     Creates a RADEC file for all 3 filters (Johnson B, V, and Cousins R
 
     :param df: input catalog DataFrame
     :param ra: user entered RA for system
     :param dec: user entered DEC for system
     :param T_list: TESS magnitudes for comparison stars
+    :param pipeline: True if pipeline, False if not
+    :param folder_path: folder path for saving RADEC files
+    :param obj_name: object name for saving RADEC files
 
     :return: None but saves the RADEC files to user specified locations
     """
     filters = ["B", "V", "R", "T"]
     header = "#RA in decimal or sexagesimal HOURS\n " \
              "#Dec in decimal or sexagesimal DEGREES\n" \
              "#Ref Star=0,1,missing (0=target star, 1=ref star, missing->first ap=target, others=ref)\n" \
@@ -313,17 +349,21 @@
                 elif filt == "T":
                     header2 += str(val) + ", " + str(dec_list[count]) + ", " + "1, 1, " + str(T_list[count]) + "\n"
 
             next_ra = float(ra_decimal[count])
             next_dec = float(dec_decimal[count])
 
         output = header + header2
-        outputfile = input("Please enter an output file pathway " + "\033[1m" + "\033[93m" + "WITHOUT" + "\033[00m" +
-                           " the extension but with the file name for the " +
-                           filt + " filter RADEC file, for AIJ (i.e. C:\\folder1\\folder2\[filename]): ")
+        if not pipeline:
+            outputfile = input(
+                "Please enter an output file pathway " + "\033[1m" + "\033[93m" + "WITHOUT" + "\033[00m" +
+                " the extension but with the file name for the " +
+                filt + " filter RADEC file, for AIJ (i.e. C:\\folder1\\folder2\[filename]): ")
+        else:
+            outputfile = folder_path + "\\" + obj_name + "_" + filt
         file = open(outputfile + ".radec", "w")
         file.write(output)
         file.close()
 
     print("\nFinished writing RADEC files for Johnson B, Johnson V, and Cousins R.\n")
```

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-3.1.0/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/find_min.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/gaia.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/menu.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-3.1.0/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-3.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: EclipsingBinaries
-Version: 3.0.0a2
-Summary: Binary Star Package for Ball State University's Astronomy Research Group
-Home-page: https://github.com/kjkoeller/EclipsingBinaries
-Author: Kyle Koeller
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 [![Python 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
@@ -55,14 +37,22 @@
 
 this will show numerous things, but you want to look at the version and make sure it is up to date.
 
 If your version is not the most recent version then in order to update type the following,
 
     pip install --upgrade EclipsingBinaries
 
+### Pipeline
+
+To use the pipeline functionality type the following:
+
+    EB_pipeline -h
+
+This will print out all the options that are available to edit and change. The `-i` and the `-o` are required for the script to run. Otherwise, the script will crash.
+
 ***
 
 ## Dependencies
 
 *   python >=3.7
 *   astropy>=5.1.1
 *   astroquery>=0.4.6
```

### Comparing `EclipsingBinaries-3.0.0a2/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/LICENSE` & `EclipsingBinaries-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-3.0.0a2/PKG-INFO` & `EclipsingBinaries-3.1.0/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 3.0.0a2
+Version: 3.1.0
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -55,14 +55,22 @@
 
 this will show numerous things, but you want to look at the version and make sure it is up to date.
 
 If your version is not the most recent version then in order to update type the following,
 
     pip install --upgrade EclipsingBinaries
 
+### Pipeline
+
+To use the pipeline functionality type the following:
+
+    EB_pipeline -h
+
+This will print out all the options that are available to edit and change. The `-i` and the `-o` are required for the script to run. Otherwise, the script will crash.
+
 ***
 
 ## Dependencies
 
 *   python >=3.7
 *   astropy>=5.1.1
 *   astroquery>=0.4.6
```

### Comparing `EclipsingBinaries-3.0.0a2/setup.py` & `EclipsingBinaries-3.1.0/setup.py`

 * *Files identical despite different names*

