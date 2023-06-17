# Comparing `tmp/cropnet-0.1.0.tar.gz` & `tmp/cropnet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropnet-0.1.0.tar", last modified: Sat Jun 17 18:48:46 2023, max compression
+gzip compressed data, was "cropnet-0.1.1.tar", last modified: Sat Jun 17 22:38:00 2023, max compression
```

## Comparing `cropnet-0.1.0.tar` & `cropnet-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 18:48:46.678506 cropnet-0.1.0/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      646 2023-06-17 18:48:46.678506 cropnet-0.1.0/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       13 2023-06-17 02:52:22.000000 cropnet-0.1.0/README.md
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 18:48:46.678506 cropnet-0.1.0/cropnet.egg-info/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      646 2023-06-17 18:48:46.000000 cropnet-0.1.0/cropnet.egg-info/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      283 2023-06-17 18:48:46.000000 cropnet-0.1.0/cropnet.egg-info/SOURCES.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-17 18:48:46.000000 cropnet-0.1.0/cropnet.egg-info/dependency_links.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-17 18:48:46.000000 cropnet-0.1.0/cropnet.egg-info/requires.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-17 18:48:46.000000 cropnet-0.1.0/cropnet.egg-info/top_level.txt
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 18:48:46.678506 cropnet-0.1.0/dataset/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 18:46:39.000000 cropnet-0.1.0/dataset/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6300 2023-06-17 17:55:37.000000 cropnet-0.1.0/dataset/hrrr_computed_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2021 2023-06-17 17:55:37.000000 cropnet-0.1.0/dataset/sentinel2_imagery.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2456 2023-06-17 17:55:37.000000 cropnet-0.1.0/dataset/usda_crop_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-17 18:48:46.678506 cropnet-0.1.0/setup.cfg
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      930 2023-06-17 18:24:36.000000 cropnet-0.1.0/setup.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 22:37:59.995314 cropnet-0.1.1/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      643 2023-06-17 22:37:59.995314 cropnet-0.1.1/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       13 2023-06-17 02:52:22.000000 cropnet-0.1.1/README.md
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 22:37:59.995314 cropnet-0.1.1/cropnet.egg-info/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      643 2023-06-17 22:37:59.000000 cropnet-0.1.1/cropnet.egg-info/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      283 2023-06-17 22:37:59.000000 cropnet-0.1.1/cropnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-17 22:37:59.000000 cropnet-0.1.1/cropnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-17 22:37:59.000000 cropnet-0.1.1/cropnet.egg-info/requires.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-17 22:37:59.000000 cropnet-0.1.1/cropnet.egg-info/top_level.txt
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-17 22:37:59.995314 cropnet-0.1.1/dataset/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 18:46:39.000000 cropnet-0.1.1/dataset/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6253 2023-06-17 22:36:51.000000 cropnet-0.1.1/dataset/hrrr_computed_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.1/dataset/sentinel2_imagery.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2435 2023-06-17 22:36:51.000000 cropnet-0.1.1/dataset/usda_crop_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-17 22:37:59.995314 cropnet-0.1.1/setup.cfg
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      927 2023-06-17 22:37:41.000000 cropnet-0.1.1/setup.py
```

### Comparing `cropnet-0.1.0/PKG-INFO` & `cropnet-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cropnet-0.1.0/cropnet.egg-info/PKG-INFO` & `cropnet-0.1.1/cropnet.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `cropnet-0.1.0/dataset/hrrr_computed_dataset.py` & `cropnet-0.1.1/dataset/hrrr_computed_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import os
 import json
 import pandas as pd
 from sklearn import preprocessing
 from einops import rearrange
 
-# TODO: 1. Optimize the time and 2. Normalization
+
 class HRRR_Computed_Dataset(torch.utils.data.Dataset):
 
     def __init__(self, base_dir, config_file, column_names=None):
         """
             Dataset for the HRRR Computed Dataset
         
         :param base_dir: the root directory for CropNet dataset, e.g., /mnt/data/CropNet
@@ -36,15 +36,15 @@
                 'Precipitation (kg m**-2)', 'Relative Humidity (%)', 'Wind Gust (m s**-1)',
                 'Wind Speed (m s**-1)', 'Downward Shortwave Radiation Flux (W m**-2)',
                 'Vapor Pressure Deficit (kPa)'
             ]
             self.column_names = default_cols
 
         # only consider the first 28 days for addressing different days in each month
-        self.day_range = [i+1 for i in range(28)]
+        self.day_range = [i + 1 for i in range(28)]
 
         data = json.load(open(config_file))
         self.fips_codes = []
         self.years = []
         self.short_term_file_path = []
         self.long_term_file_path = []
         self.scaler = preprocessing.StandardScaler()
```

### Comparing `cropnet-0.1.0/dataset/sentinel2_imagery.py` & `cropnet-0.1.1/dataset/sentinel2_imagery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import h5py
 import torch
 import os
 import numpy as np
 import json
 from einops import rearrange
-import torchvision.transforms as transforms
 
-# TODO: Normalization
+
 class Sentinel2Imagery(torch.utils.data.Dataset):
 
     def __init__(self, base_dir, config_file, transform=None):
         """
             Dataset for Sentinel-2 Imagery
 
         :param base_dir: the root directory for CropNet dataset, e.g., /mnt/data/CropNet
```

### Comparing `cropnet-0.1.0/dataset/usda_crop_dataset.py` & `cropnet-0.1.1/dataset/usda_crop_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from torch.utils.data import Dataset
 import os
 import json
 import pandas as pd
 
-# TODO: Normalization
+
 class USDA_Crop_Dataset(torch.utils.data.Dataset):
 
     def __init__(self, base_dir, config_file, crop_type="Soybeans"):
         """
             Dataset for the USDA Crop Dataset
 
         :param base_dir: the root directory for CropNet dataset, e.g., /mnt/data/CropNet
```

### Comparing `cropnet-0.1.0/setup.py` & `cropnet-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='cropnet',
-    version='0.1.0',
+    version='0.1.1',
     description='A Python package for the CropNet dataset',
     author='Anonymous AI4Science',
     author_email='anonymous.ai4science@gmail.com',
     license='Free for non-commercial use',
     packages=['dataset'],
     install_requires=[
         'torch >= 1.11.0',
@@ -16,15 +16,15 @@
         'pandas',
         'h5py',
         'Pillow',
         'einops',
     ],
 
     classifiers=[
-        'Development Status :: 1 - Planning',
+        'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: Free for non-commercial use',
         'Operating System :: MacOS',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

