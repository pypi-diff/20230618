# Comparing `tmp/tlcr-0.0.1.tar.gz` & `tmp/tlcr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tlcr-0.0.1.tar", last modified: Fri Jun  2 18:07:33 2023, max compression
+gzip compressed data, was "dist\tlcr-0.0.2.tar", last modified: Sun Jun 18 19:42:44 2023, max compression
```

## Comparing `tlcr-0.0.1.tar` & `tlcr-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:07:33.331866 tlcr-0.0.1/
--rw-rw-rw-   0        0        0     1093 2023-06-02 17:18:35.000000 tlcr-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      256 2023-06-02 18:07:33.330865 tlcr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-05-27 07:31:26.000000 tlcr-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 18:07:33.331866 tlcr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      327 2023-06-02 17:16:24.000000 tlcr-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:07:33.311230 tlcr-0.0.1/tlcr/
--rw-rw-rw-   0        0        0     1435 2023-05-27 15:15:16.000000 tlcr-0.0.1/tlcr/Bioinspired.py
--rw-rw-rw-   0        0        0     7458 2023-05-27 08:03:28.000000 tlcr-0.0.1/tlcr/ImageNet.py
--rw-rw-rw-   0        0        0     4396 2023-06-02 18:06:51.000000 tlcr-0.0.1/tlcr/Line.py
--rw-rw-rw-   0        0        0      743 2023-06-02 18:05:26.000000 tlcr-0.0.1/tlcr/Video.py
--rw-rw-rw-   0        0        0        0 2023-05-27 07:35:36.000000 tlcr-0.0.1/tlcr/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-05-27 15:25:04.000000 tlcr-0.0.1/tlcr/tlcr.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:07:33.329865 tlcr-0.0.1/tlcr.egg-info/
--rw-rw-rw-   0        0        0      256 2023-06-02 18:07:33.000000 tlcr-0.0.1/tlcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-06-02 18:07:33.000000 tlcr-0.0.1/tlcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:07:33.000000 tlcr-0.0.1/tlcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-02 18:07:33.000000 tlcr-0.0.1/tlcr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 19:42:44.535934 tlcr-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-06-02 17:18:35.000000 tlcr-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      256 2023-06-18 19:42:44.534933 tlcr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-05-27 07:31:26.000000 tlcr-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-18 19:42:44.535934 tlcr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      327 2023-06-18 19:30:34.000000 tlcr-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:42:44.528917 tlcr-0.0.2/tlcr/
+-rw-rw-rw-   0        0        0     1440 2023-06-07 19:49:06.000000 tlcr-0.0.2/tlcr/Bioinspired.py
+-rw-rw-rw-   0        0        0     7396 2023-06-08 11:50:19.000000 tlcr-0.0.2/tlcr/ImageNet.py
+-rw-rw-rw-   0        0        0     4396 2023-06-02 19:03:42.000000 tlcr-0.0.2/tlcr/Lane.py
+-rw-rw-rw-   0        0        0     1309 2023-06-18 19:30:33.000000 tlcr-0.0.2/tlcr/Video.py
+-rw-rw-rw-   0        0        0        0 2023-05-27 07:35:36.000000 tlcr-0.0.2/tlcr/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-06-18 19:28:31.000000 tlcr-0.0.2/tlcr/tlcr.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:42:44.533927 tlcr-0.0.2/tlcr.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-06-18 19:42:44.000000 tlcr-0.0.2/tlcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-06-18 19:42:44.000000 tlcr-0.0.2/tlcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 19:42:44.000000 tlcr-0.0.2/tlcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-18 19:42:44.000000 tlcr-0.0.2/tlcr.egg-info/top_level.txt
```

### Comparing `tlcr-0.0.1/LICENSE` & `tlcr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tlcr-0.0.1/tlcr/Bioinspired.py` & `tlcr-0.0.2/tlcr/Bioinspired.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import cv2
-from tlcr.Video import Video
+from tlcr.tlcr.Video import Video
 
 
 class Bioinspired:
     def __init__(self, width, height, path_to_save):
         self.__retina = cv2.bioinspired_Retina.create((width, height))
         self.__retina.write('retinaParams.xml')
         self.__retina.setup('retinaParams.xml')
```

### Comparing `tlcr-0.0.1/tlcr/ImageNet.py` & `tlcr-0.0.2/tlcr/ImageNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # required to work on GPU (do not change because it only works like that)
 from __future__ import absolute_import, division, print_function, unicode_literals
 import tensorflow as tf
 import numpy as np
 import os
-from tensorflow.keras import Model
-from tensorflow.keras.optimizers.legacy import Adam
-from tensorflow.keras.losses import binary_crossentropy
-from tensorflow.keras.layers import Input, Conv2D, Conv2DTranspose, MaxPooling2D, concatenate, Dropout
-from tensorflow.keras import backend as K
+from keras import Model
+from keras.optimizers import Adam
+from keras.losses import binary_crossentropy
+from keras.layers import Input, Conv2D, Conv2DTranspose, MaxPooling2D, concatenate, Dropout
+from keras import backend as K
 from tensorflow.python.keras.utils.generic_utils import get_custom_objects
 
 
 class ImageNet:
     size_img = 256
 
     def __init__(self):
```

### Comparing `tlcr-0.0.1/tlcr/Line.py` & `tlcr-0.0.2/tlcr/Lane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import cv2
 
 
-class Line:
+class Lane:
     def __init__(self, coords):
         self.__pts = np.array(coords, np.int32).reshape((- 1, 1, 2))
         self.__rect = cv2.boundingRect(self.__pts)
         self.__mask = None
         self.__count_mask_pixels = 0
         self.__color = (255, 255, 255)
         self.__final_size = (256, 256)
```

### Comparing `tlcr-0.0.1/tlcr/Video.py` & `tlcr-0.0.2/tlcr/Video.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,7 +18,25 @@
     @staticmethod
     def get_video_duration(video_path):
         video = cv2.VideoCapture(video_path)
         frame = video.get(cv2.CAP_PROP_FRAME_COUNT)
         fps = video.get(cv2.CAP_PROP_FPS)
         duration_in_seconds = frame / fps
         return duration_in_seconds
+
+    @staticmethod
+    def get_image(path):
+        print(id)
+        dir_contents = os.listdir(path)
+        files = [f for f in dir_contents if os.path.isfile(path + '/' + f)]
+        cam = cv2.VideoCapture(os.path.join(path, files[0]))
+        print(cam.isOpened())
+        cam.read()
+        for _ in (0, 5):
+            ret, frame = cam.read()
+        print(frame)
+        print(os.path.join(path, files[0]))
+        print(ret)
+        if not ret:
+            return
+        frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+        return frame
```

### Comparing `tlcr-0.0.1/tlcr/tlcr.py` & `tlcr-0.0.2/tlcr/tlcr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-from tlcr.Video import Video
-from tlcr.Line import Line
-from tlcr.ImageNet import ImageNet
+from tlcr.tlcr.Video import Video
+from tlcr.tlcr.Lane import Lane
+from tlcr.tlcr.ImageNet import ImageNet
 from skimage.util import img_as_float
 import numpy as np
 
 
 class Tlcr:
     intensity_k = 0.155
 
     @staticmethod
     def get_params(url, weights, coords):
         images = []
         Video.fill_images(url, images)
-        line = Line(coords)
+        line = Lane(coords)
         images = images[::5]
         size = len(images)
         x = np.zeros((size, ImageNet.size_img, ImageNet.size_img, 3), dtype='float32')
         for i in range(0, len(images)):
             x[i] = np.array(img_as_float(line.get_image(images[i])))
         image_net = ImageNet()
         image_net.init()
         image_net.load_weights(weights)
         predictions = image_net.predict(x)
         size_predictions = len(predictions)
-        tlcr = 0
+        tlcr_arr = []
         vehicles = 0
         wait_next_vehicle = True
         for i in range(0, size_predictions):
             local_tlcr = line.get_tlcr(predictions[i])
             if local_tlcr > Tlcr.intensity_k and wait_next_vehicle:
                 vehicles += 1
             wait_next_vehicle = local_tlcr < Tlcr.intensity_k
-            tlcr += local_tlcr
-        tlcr = tlcr / size_predictions
-        return tlcr, vehicles
-
-
-
-
+            tlcr_arr.append(local_tlcr)
+        # tlcr = tlcr / size_predictions
+        return tlcr_arr, vehicles
```

