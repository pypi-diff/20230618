# Comparing `tmp/cropnet-0.1.3.tar.gz` & `tmp/cropnet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cropnet-0.1.3.tar", last modified: Sun Jun 18 02:13:09 2023, max compression
+gzip compressed data, was "cropnet-0.1.4.tar", last modified: Sun Jun 18 21:41:47 2023, max compression
```

## Comparing `cropnet-0.1.3.tar` & `cropnet-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 02:13:09.878758 cropnet-0.1.3/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4718 2023-06-18 02:13:09.878758 cropnet-0.1.3/PKG-INFO
--rw-r--r--   0 fudong    (1000) fudong    (1000)     4033 2023-06-18 02:04:05.000000 cropnet-0.1.3/README.md
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 02:13:09.878758 cropnet-0.1.3/cropnet.egg-info/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     4718 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/PKG-INFO
--rw-rw-r--   0 fudong    (1000) fudong    (1000)      283 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/SOURCES.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/dependency_links.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/requires.txt
--rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-18 02:13:09.000000 cropnet-0.1.3/cropnet.egg-info/top_level.txt
-drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 02:13:09.878758 cropnet-0.1.3/dataset/
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 22:41:39.000000 cropnet-0.1.3/dataset/__init__.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     6253 2023-06-17 22:36:51.000000 cropnet-0.1.3/dataset/hrrr_computed_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.3/dataset/sentinel2_imagery.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     2435 2023-06-17 22:36:51.000000 cropnet-0.1.3/dataset/usda_crop_dataset.py
--rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-18 02:13:09.878758 cropnet-0.1.3/setup.cfg
--rw-rw-r--   0 fudong    (1000) fudong    (1000)     1183 2023-06-18 02:11:41.000000 cropnet-0.1.3/setup.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 21:41:47.900168 cropnet-0.1.4/PKG-INFO
+-rw-r--r--   0 fudong    (1000) fudong    (1000)     4071 2023-06-18 21:41:32.000000 cropnet-0.1.4/README.md
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/cropnet/
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/cropnet/dataset/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       55 2023-06-17 22:41:39.000000 cropnet-0.1.4/cropnet/dataset/__init__.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     6251 2023-06-18 21:33:51.000000 cropnet-0.1.4/cropnet/dataset/hrrr_computed_dataset.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1956 2023-06-17 22:36:51.000000 cropnet-0.1.4/cropnet/dataset/sentinel2_imagery.py
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     2433 2023-06-18 21:33:51.000000 cropnet-0.1.4/cropnet/dataset/usda_crop_dataset.py
+drwxrwxr-x   0 fudong    (1000) fudong    (1000)        0 2023-06-18 21:41:47.900168 cropnet-0.1.4/cropnet.egg-info/
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     4756 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/PKG-INFO
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)      315 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        1 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       64 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/requires.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)        8 2023-06-18 21:41:47.000000 cropnet-0.1.4/cropnet.egg-info/top_level.txt
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)       38 2023-06-18 21:41:47.900168 cropnet-0.1.4/setup.cfg
+-rw-rw-r--   0 fudong    (1000) fudong    (1000)     1191 2023-06-18 21:33:58.000000 cropnet-0.1.4/setup.py
```

### Comparing `cropnet-0.1.3/PKG-INFO` & `cropnet-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
@@ -42,28 +42,28 @@
 
 #### USDA Crop Dataset
 
 The USDA Crop Dataset, collected from the [USDA Quick Statistic website](https://quickstats.nass.usda.gov/), offers valuable crop information, such as production, yield, etc., for crops grown at each available county. It offers crop information for four types of crops, i.e., corn, cotton, soybeans, and winter wheat, at a county-level basis, with a temporal resolution of one year.
 
 
 
-Although our initial goal of crafting the CropNet dataset is for precise crop yield prediction, we believe its future applicability is broad and can benefit the deep learning, agriculture, and meteorology communities, for exploring more interesting, critical, and pertinent climate change-related applications, by using one or more modalities of data.
+Although our initial goal of crafting the CropNet dataset is for precise crop yield prediction, we believe its future applicability is broad and can benefit the deep learning, agriculture, and meteorology communities, for exploring more interesting and critical climate change-related applications, by using one or more modalities of data.
 
 
 
 ## Pipeline
 
 The code in this reposity:
 
-1. combines all three modalities of data to create $(\mathbf{x}, \mathbf{y_{s}}, \mathbf{y_{l}}, \mathbf{z})$ tuples, with $\mathbf{x}$, $\mathbf{y_{s}}$, $\mathbf{y_{l}}$, and $\mathbf{z}$ representing satellite images, short-term daily whether parameters, long-term monthly meterological parameters, and ground-truth crop yield (or production) inforamtion, resprectively, and
+1. combines all three modalities of data to create $(\mathbf{x}, \mathbf{y_{s}}, \mathbf{y_{l}}, \mathbf{z})$ tuples, with $\mathbf{x}$, $\mathbf{y_{s}}$, $\mathbf{y_{l}}$, and $\mathbf{z}$ representing satellite images, short-term daily whether parameters, long-term monthly meteorological parameters, and ground-truth crop yield (or production) information, respectively and
 2. exposes those tuples via a `Dataset` object.
 
 Notably, one or more modalities of data can be used for specific deep learning tasks. For example,
 
-1. satellite images can be solely utilized for pre-training deep neural networks in a self-supervised learning manner (e.g., [SimCLR](https://arxiv.org/pdf/2002.05709.pdf)), or
+1. satellite images can be solely utilized for pre-training deep neural networks in a self-supervised learning manner (e.g., [SimCLR](https://arxiv.org/pdf/2002.05709.pdf), [MAE](https://arxiv.org/pdf/2111.06377.pdf), etc.), or
 2. a pair of $(\mathbf{x}, \mathbf{y_{s}})$ under the same 9x9 km grid can be used for exploring the local weather effect on crop growth.
 
 
 
 ## Installation
 
 MacOS and Linux users can install the latest version of CropNet with the following command:
```

### Comparing `cropnet-0.1.3/README.md` & `cropnet-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 
 #### USDA Crop Dataset
 
 The USDA Crop Dataset, collected from the [USDA Quick Statistic website](https://quickstats.nass.usda.gov/), offers valuable crop information, such as production, yield, etc., for crops grown at each available county. It offers crop information for four types of crops, i.e., corn, cotton, soybeans, and winter wheat, at a county-level basis, with a temporal resolution of one year.
 
 
 
-Although our initial goal of crafting the CropNet dataset is for precise crop yield prediction, we believe its future applicability is broad and can benefit the deep learning, agriculture, and meteorology communities, for exploring more interesting, critical, and pertinent climate change-related applications, by using one or more modalities of data.
+Although our initial goal of crafting the CropNet dataset is for precise crop yield prediction, we believe its future applicability is broad and can benefit the deep learning, agriculture, and meteorology communities, for exploring more interesting and critical climate change-related applications, by using one or more modalities of data.
 
 
 
 ## Pipeline
 
 The code in this reposity:
 
-1. combines all three modalities of data to create $(\mathbf{x}, \mathbf{y_{s}}, \mathbf{y_{l}}, \mathbf{z})$ tuples, with $\mathbf{x}$, $\mathbf{y_{s}}$, $\mathbf{y_{l}}$, and $\mathbf{z}$ representing satellite images, short-term daily whether parameters, long-term monthly meterological parameters, and ground-truth crop yield (or production) inforamtion, resprectively, and
+1. combines all three modalities of data to create $(\mathbf{x}, \mathbf{y_{s}}, \mathbf{y_{l}}, \mathbf{z})$ tuples, with $\mathbf{x}$, $\mathbf{y_{s}}$, $\mathbf{y_{l}}$, and $\mathbf{z}$ representing satellite images, short-term daily whether parameters, long-term monthly meteorological parameters, and ground-truth crop yield (or production) information, respectively and
 2. exposes those tuples via a `Dataset` object.
 
 Notably, one or more modalities of data can be used for specific deep learning tasks. For example,
 
-1. satellite images can be solely utilized for pre-training deep neural networks in a self-supervised learning manner (e.g., [SimCLR](https://arxiv.org/pdf/2002.05709.pdf)), or
+1. satellite images can be solely utilized for pre-training deep neural networks in a self-supervised learning manner (e.g., [SimCLR](https://arxiv.org/pdf/2002.05709.pdf), [MAE](https://arxiv.org/pdf/2111.06377.pdf), etc.), or
 2. a pair of $(\mathbf{x}, \mathbf{y_{s}})$ under the same 9x9 km grid can be used for exploring the local weather effect on crop growth.
 
 
 
 ## Installation
 
 MacOS and Linux users can install the latest version of CropNet with the following command:
```

### Comparing `cropnet-0.1.3/cropnet.egg-info/PKG-INFO` & `cropnet-0.1.4/cropnet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cropnet
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for the CropNet dataset
 Author: Anonymous AI4Science
 Author-email: anonymous.ai4science@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
@@ -42,28 +42,28 @@
 
 #### USDA Crop Dataset
 
 The USDA Crop Dataset, collected from the [USDA Quick Statistic website](https://quickstats.nass.usda.gov/), offers valuable crop information, such as production, yield, etc., for crops grown at each available county. It offers crop information for four types of crops, i.e., corn, cotton, soybeans, and winter wheat, at a county-level basis, with a temporal resolution of one year.
 
 
 
-Although our initial goal of crafting the CropNet dataset is for precise crop yield prediction, we believe its future applicability is broad and can benefit the deep learning, agriculture, and meteorology communities, for exploring more interesting, critical, and pertinent climate change-related applications, by using one or more modalities of data.
+Although our initial goal of crafting the CropNet dataset is for precise crop yield prediction, we believe its future applicability is broad and can benefit the deep learning, agriculture, and meteorology communities, for exploring more interesting and critical climate change-related applications, by using one or more modalities of data.
 
 
 
 ## Pipeline
 
 The code in this reposity:
 
-1. combines all three modalities of data to create $(\mathbf{x}, \mathbf{y_{s}}, \mathbf{y_{l}}, \mathbf{z})$ tuples, with $\mathbf{x}$, $\mathbf{y_{s}}$, $\mathbf{y_{l}}$, and $\mathbf{z}$ representing satellite images, short-term daily whether parameters, long-term monthly meterological parameters, and ground-truth crop yield (or production) inforamtion, resprectively, and
+1. combines all three modalities of data to create $(\mathbf{x}, \mathbf{y_{s}}, \mathbf{y_{l}}, \mathbf{z})$ tuples, with $\mathbf{x}$, $\mathbf{y_{s}}$, $\mathbf{y_{l}}$, and $\mathbf{z}$ representing satellite images, short-term daily whether parameters, long-term monthly meteorological parameters, and ground-truth crop yield (or production) information, respectively and
 2. exposes those tuples via a `Dataset` object.
 
 Notably, one or more modalities of data can be used for specific deep learning tasks. For example,
 
-1. satellite images can be solely utilized for pre-training deep neural networks in a self-supervised learning manner (e.g., [SimCLR](https://arxiv.org/pdf/2002.05709.pdf)), or
+1. satellite images can be solely utilized for pre-training deep neural networks in a self-supervised learning manner (e.g., [SimCLR](https://arxiv.org/pdf/2002.05709.pdf), [MAE](https://arxiv.org/pdf/2111.06377.pdf), etc.), or
 2. a pair of $(\mathbf{x}, \mathbf{y_{s}})$ under the same 9x9 km grid can be used for exploring the local weather effect on crop growth.
 
 
 
 ## Installation
 
 MacOS and Linux users can install the latest version of CropNet with the following command:
```

### Comparing `cropnet-0.1.3/dataset/hrrr_computed_dataset.py` & `cropnet-0.1.4/cropnet/dataset/hrrr_computed_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import json
 import pandas as pd
 from sklearn import preprocessing
 from einops import rearrange
 
 
-class HRRR_Computed_Dataset(torch.utils.data.Dataset):
+class HRRRComputedDataset(torch.utils.data.Dataset):
 
     def __init__(self, base_dir, config_file, column_names=None):
         """
             Dataset for the HRRR Computed Dataset
         
         :param base_dir: the root directory for CropNet dataset, e.g., /mnt/data/CropNet
         :param config_file: the path for JSON configuration file
```

### Comparing `cropnet-0.1.3/dataset/sentinel2_imagery.py` & `cropnet-0.1.4/cropnet/dataset/sentinel2_imagery.py`

 * *Files identical despite different names*

### Comparing `cropnet-0.1.3/dataset/usda_crop_dataset.py` & `cropnet-0.1.4/cropnet/dataset/usda_crop_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from torch.utils.data import Dataset
 import os
 import json
 import pandas as pd
 
 
-class USDA_Crop_Dataset(torch.utils.data.Dataset):
+class USDACropDataset(torch.utils.data.Dataset):
 
     def __init__(self, base_dir, config_file, crop_type="Soybeans"):
         """
             Dataset for the USDA Crop Dataset
 
         :param base_dir: the root directory for CropNet dataset, e.g., /mnt/data/CropNet
         :param config_file: the path for JSON configuration file
```

### Comparing `cropnet-0.1.3/setup.py` & `cropnet-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='cropnet',
-    version='0.1.3',
+    version='0.1.4',
     description='A Python package for the CropNet dataset',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Anonymous AI4Science',
     author_email='anonymous.ai4science@gmail.com',
     license='Free for non-commercial use',
-    packages=['dataset'],
+    packages=['cropnet.dataset'],
     install_requires=[
         'torch >= 1.11.0',
         'numpy',
         'torchvision',
         'numpy',
         'pandas',
         'h5py',
```

