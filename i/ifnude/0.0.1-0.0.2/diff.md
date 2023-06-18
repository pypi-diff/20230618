# Comparing `tmp/ifnude-0.0.1.tar.gz` & `tmp/ifnude-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifnude-0.0.1.tar", last modified: Sun Jun 18 20:29:03 2023, max compression
+gzip compressed data, was "ifnude-0.0.2.tar", last modified: Sun Jun 18 21:57:02 2023, max compression
```

## Comparing `ifnude-0.0.1.tar` & `ifnude-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 20:29:02.995838 ifnude-0.0.1/
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1067 2023-06-18 11:09:02.000000 ifnude-0.0.1/LICENSE.md
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1545 2023-06-18 20:29:02.995838 ifnude-0.0.1/PKG-INFO
--rw-r--r--   0 d3v       (1000) d3v       (1000)      882 2023-06-18 20:25:16.000000 ifnude-0.0.1/README.md
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 20:29:02.995838 ifnude-0.0.1/ifnude/
--rw-r--r--   0 d3v       (1000) d3v       (1000)       29 2023-06-18 19:31:09.000000 ifnude-0.0.1/ifnude/__init__.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     3375 2023-06-18 19:33:14.000000 ifnude-0.0.1/ifnude/detector.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1617 2023-06-18 19:44:50.000000 ifnude-0.0.1/ifnude/detector_utils.py
--rw-r--r--   0 d3v       (1000) d3v       (1000)     5265 2023-06-18 19:04:08.000000 ifnude-0.0.1/ifnude/image_utils.py
-drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 20:29:02.995838 ifnude-0.0.1/ifnude.egg-info/
--rw-r--r--   0 d3v       (1000) d3v       (1000)     1545 2023-06-18 20:29:02.000000 ifnude-0.0.1/ifnude.egg-info/PKG-INFO
--rw-r--r--   0 d3v       (1000) d3v       (1000)      263 2023-06-18 20:29:02.000000 ifnude-0.0.1/ifnude.egg-info/SOURCES.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2023-06-18 20:29:02.000000 ifnude-0.0.1/ifnude.egg-info/dependency_links.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)       73 2023-06-18 20:29:02.000000 ifnude-0.0.1/ifnude.egg-info/requires.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)        7 2023-06-18 20:29:02.000000 ifnude-0.0.1/ifnude.egg-info/top_level.txt
--rw-r--r--   0 d3v       (1000) d3v       (1000)       38 2023-06-18 20:29:02.995838 ifnude-0.0.1/setup.cfg
--rw-r--r--   0 d3v       (1000) d3v       (1000)     2636 2023-06-18 20:14:33.000000 ifnude-0.0.1/setup.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 21:57:02.845304 ifnude-0.0.2/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1067 2023-06-18 21:56:34.000000 ifnude-0.0.2/LICENSE.md
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1561 2023-06-18 21:57:02.845304 ifnude-0.0.2/PKG-INFO
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      899 2023-06-18 21:56:34.000000 ifnude-0.0.2/README.md
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 21:57:02.845304 ifnude-0.0.2/ifnude/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       29 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/__init__.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     3319 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/detector.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1607 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/detector_utils.py
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     5240 2023-06-18 21:56:34.000000 ifnude-0.0.2/ifnude/image_utils.py
+drwxr-xr-x   0 d3v       (1000) d3v       (1000)        0 2023-06-18 21:57:02.845304 ifnude-0.0.2/ifnude.egg-info/
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     1561 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/PKG-INFO
+-rw-r--r--   0 d3v       (1000) d3v       (1000)      263 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/SOURCES.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        1 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/dependency_links.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       70 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/requires.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)        7 2023-06-18 21:57:02.000000 ifnude-0.0.2/ifnude.egg-info/top_level.txt
+-rw-r--r--   0 d3v       (1000) d3v       (1000)       38 2023-06-18 21:57:02.845304 ifnude-0.0.2/setup.cfg
+-rw-r--r--   0 d3v       (1000) d3v       (1000)     2633 2023-06-18 21:56:34.000000 ifnude-0.0.2/setup.py
```

### Comparing `ifnude-0.0.1/LICENSE.md` & `ifnude-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ifnude-0.0.1/PKG-INFO` & `ifnude-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifnude
-Version: 0.0.1
+Version: 0.0.2
 Summary: An AI powered nudity detection library
 Home-page: https://github.com/s0md3v/ifnude
 Author: Somdev Sangwan
 Author-email: s0md3v@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -15,24 +15,21 @@
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # ifnude
 
-ifnude is a neural net powered library that takes an input as input and tells you exactly what NSFW parts of the body are visible. It also allows you to censor the said parts.
-
-Works on both on humans and drawings.
-
-![demo](https://i.imgur.com/0KPJbl9.jpg)
+It is a nudity detection library that actually works, on both on humans and drawings.. It tells you exactly what NSFW parts of the body are visible. Optionally, you can censor the said parts.
 
+<img src="https://i.imgur.com/0KPJbl9.jpg" width=600>
 
 ### Installation
 ```bash
-pip install --upgrade ifnude
+pip install ifnude
 ```
 
 ### Example
 ```python
 from ifnude import detect
 
 # use mode="fast" for x3 speed with slightly lower accuracy
@@ -41,8 +38,8 @@
 
 #### Output
 ```
 [{'box': [164, 188, 246, 271], 'score': 0.8253238201141357, 'label': 'EXPOSED_BREAST_F'}, {'box': [252, 190, 335, 270], 'score': 0.8235630989074707, 'label': 'EXPOSED_BREAST_F'}]
 ```
 
 ### Credits
-This is fork of [NudeNet](https://pypi.org/project/NudeNet/) library which doesn't work anymore. I have taken the liberty to remove the video detection functionality as it was prone to crashes.
+This is fork of [NudeNet](https://pypi.org/project/NudeNet/) library which doesn't work anymore. I have taken the liberty to remove the video detection functionality as it was prone to crashes. It will be re-implemented in future.
```

### Comparing `ifnude-0.0.1/README.md` & `ifnude-0.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # ifnude
 
-ifnude is a neural net powered library that takes an input as input and tells you exactly what NSFW parts of the body are visible. It also allows you to censor the said parts.
-
-Works on both on humans and drawings.
-
-![demo](https://i.imgur.com/0KPJbl9.jpg)
+It is a nudity detection library that actually works, on both on humans and drawings.. It tells you exactly what NSFW parts of the body are visible. Optionally, you can censor the said parts.
 
+<img src="https://i.imgur.com/0KPJbl9.jpg" width=600>
 
 ### Installation
 ```bash
-pip install --upgrade ifnude
+pip install ifnude
 ```
 
 ### Example
 ```python
 from ifnude import detect
 
 # use mode="fast" for x3 speed with slightly lower accuracy
@@ -22,8 +19,8 @@
 
 #### Output
 ```
 [{'box': [164, 188, 246, 271], 'score': 0.8253238201141357, 'label': 'EXPOSED_BREAST_F'}, {'box': [252, 190, 335, 270], 'score': 0.8235630989074707, 'label': 'EXPOSED_BREAST_F'}]
 ```
 
 ### Credits
-This is fork of [NudeNet](https://pypi.org/project/NudeNet/) library which doesn't work anymore. I have taken the liberty to remove the video detection functionality as it was prone to crashes.
+This is fork of [NudeNet](https://pypi.org/project/NudeNet/) library which doesn't work anymore. I have taken the liberty to remove the video detection functionality as it was prone to crashes. It will be re-implemented in future.
```

### Comparing `ifnude-0.0.1/ifnude/detector.py` & `ifnude-0.0.2/ifnude/detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import cv2
-import logging
 import numpy as np
 import onnxruntime
 from tqdm import tqdm
+import urllib
 
 from .detector_utils import preprocess_image
 
 
 def dummy(*args, **kwargs):
     pass
 
@@ -89,13 +89,12 @@
 
     if parts_to_blur:
         boxes = [i["box"] for i in boxes if i["label"] in parts_to_blur]
     else:
         boxes = [i["box"] for i in boxes]
 
     for box in boxes:
-        part = image[box[1] : box[3], box[0] : box[2]]
         image = cv2.rectangle(
             image, (box[0], box[1]), (box[2], box[3]), (0, 0, 0), cv2.FILLED
         )
 
     return image
```

### Comparing `ifnude-0.0.1/ifnude/detector_utils.py` & `ifnude-0.0.2/ifnude/detector_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import cv2
 import numpy as np
 from PIL import Image
 
 
 def read_image_bgr(path):
     """ Read an image in BGR format.
```

### Comparing `ifnude-0.0.1/ifnude/image_utils.py` & `ifnude-0.0.2/ifnude/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import os
 import io
 import cv2
-import pydload
 import logging
 import numpy as np
 
 from PIL import Image as pil_image
 
 if pil_image is not None:
     _PIL_INTERPOLATION_METHODS = {
```

### Comparing `ifnude-0.0.1/ifnude.egg-info/PKG-INFO` & `ifnude-0.0.2/ifnude.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifnude
-Version: 0.0.1
+Version: 0.0.2
 Summary: An AI powered nudity detection library
 Home-page: https://github.com/s0md3v/ifnude
 Author: Somdev Sangwan
 Author-email: s0md3v@gmail.com
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
@@ -15,24 +15,21 @@
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # ifnude
 
-ifnude is a neural net powered library that takes an input as input and tells you exactly what NSFW parts of the body are visible. It also allows you to censor the said parts.
-
-Works on both on humans and drawings.
-
-![demo](https://i.imgur.com/0KPJbl9.jpg)
+It is a nudity detection library that actually works, on both on humans and drawings.. It tells you exactly what NSFW parts of the body are visible. Optionally, you can censor the said parts.
 
+<img src="https://i.imgur.com/0KPJbl9.jpg" width=600>
 
 ### Installation
 ```bash
-pip install --upgrade ifnude
+pip install ifnude
 ```
 
 ### Example
 ```python
 from ifnude import detect
 
 # use mode="fast" for x3 speed with slightly lower accuracy
@@ -41,8 +38,8 @@
 
 #### Output
 ```
 [{'box': [164, 188, 246, 271], 'score': 0.8253238201141357, 'label': 'EXPOSED_BREAST_F'}, {'box': [252, 190, 335, 270], 'score': 0.8235630989074707, 'label': 'EXPOSED_BREAST_F'}]
 ```
 
 ### Credits
-This is fork of [NudeNet](https://pypi.org/project/NudeNet/) library which doesn't work anymore. I have taken the liberty to remove the video detection functionality as it was prone to crashes.
+This is fork of [NudeNet](https://pypi.org/project/NudeNet/) library which doesn't work anymore. I have taken the liberty to remove the video detection functionality as it was prone to crashes. It will be re-implemented in future.
```

### Comparing `ifnude-0.0.1/setup.py` & `ifnude-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 # Package meta-data.
 NAME = 'ifnude'
 DESCRIPTION = 'An AI powered nudity detection library'
 URL = 'https://github.com/s0md3v/ifnude'
 EMAIL = 's0md3v@gmail.com'
 AUTHOR = 'Somdev Sangwan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pillow',
     'opencv-python-headless>=4.5.1.48',
-    'pydload',
+    'tqdm',
     'scikit-image',
     'onnxruntime'
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 try:
```

