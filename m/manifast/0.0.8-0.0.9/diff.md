# Comparing `tmp/manifast-0.0.8.tar.gz` & `tmp/manifast-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifast-0.0.8.tar", last modified: Wed May 17 06:15:16 2023, max compression
+gzip compressed data, was "manifast-0.0.9.tar", last modified: Fri May 19 06:41:29 2023, max compression
```

## Comparing `manifast-0.0.8.tar` & `manifast-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/
--rw-rw-r--   0 knight    (1000) knight    (1000)       33 2023-02-24 15:52:08.000000 manifast-0.0.8/MANIFEST.in
--rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-17 06:15:16.659279 manifast-0.0.8/PKG-INFO
--rw-rw-r--   0 knight    (1000) knight    (1000)       11 2023-02-24 09:21:56.000000 manifast-0.0.8/README.md
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.655279 manifast-0.0.8/manifast/
--rw-rw-r--   0 knight    (1000) knight    (1000)      367 2023-02-24 15:58:02.000000 manifast-0.0.8/manifast/__init__.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.655279 manifast-0.0.8/manifast/gui_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      321 2023-02-27 01:41:55.000000 manifast-0.0.8/manifast/gui_utils/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      422 2023-02-27 10:18:34.000000 manifast-0.0.8/manifast/gui_utils/counter.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      994 2023-05-17 06:15:00.000000 manifast-0.0.8/manifast/import_pkg.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/iostream/
--rw-rw-r--   0 knight    (1000) knight    (1000)      498 2023-04-20 07:01:48.000000 manifast-0.0.8/manifast/iostream/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1904 2023-04-20 07:05:50.000000 manifast-0.0.8/manifast/iostream/envstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3882 2023-05-08 02:35:21.000000 manifast-0.0.8/manifast/iostream/filestream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     2217 2023-04-09 04:26:57.000000 manifast-0.0.8/manifast/iostream/imagestream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      773 2023-04-06 02:01:32.000000 manifast-0.0.8/manifast/iostream/logstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      680 2023-04-04 07:04:06.000000 manifast-0.0.8/manifast/iostream/pdstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1631 2023-04-09 04:32:18.000000 manifast-0.0.8/manifast/iostream/pltstream.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1307 2023-05-08 02:31:43.000000 manifast-0.0.8/manifast/iostream/processsing.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      329 2023-02-24 15:52:38.000000 manifast-0.0.8/manifast/label_utils/__init__.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/classify/
--rw-rw-r--   0 knight    (1000) knight    (1000)      338 2023-02-24 15:53:30.000000 manifast-0.0.8/manifast/label_utils/classify/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      344 2023-02-24 15:40:14.000000 manifast-0.0.8/manifast/label_utils/classify/gen_split_data.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/detect/
--rw-rw-r--   0 knight    (1000) knight    (1000)      336 2023-02-24 15:53:26.000000 manifast-0.0.8/manifast/label_utils/detect/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)      985 2023-02-25 14:16:00.000000 manifast-0.0.8/manifast/label_utils/detect/convert_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1903 2023-02-25 14:16:04.000000 manifast-0.0.8/manifast/label_utils/detect/gen_split_data.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     5031 2023-02-25 14:16:06.000000 manifast-0.0.8/manifast/label_utils/detect/vis_label.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/label_utils/segment/
--rw-rw-r--   0 knight    (1000) knight    (1000)      337 2023-02-24 15:53:21.000000 manifast-0.0.8/manifast/label_utils/segment/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4301 2023-02-25 01:34:19.000000 manifast-0.0.8/manifast/label_utils/segment/colorize_mask.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     7247 2023-02-25 14:16:31.000000 manifast-0.0.8/manifast/label_utils/segment/convert_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1644 2023-02-25 02:17:38.000000 manifast-0.0.8/manifast/label_utils/segment/convert_utils.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3977 2023-02-25 14:17:05.000000 manifast-0.0.8/manifast/label_utils/segment/gen_split_data.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     1236 2023-02-25 14:17:11.000000 manifast-0.0.8/manifast/label_utils/segment/vis_label.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     4864 2023-02-25 14:20:53.000000 manifast-0.0.8/manifast/label_utils/segment/vis_utils.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.659279 manifast-0.0.8/manifast/model_utils/
--rw-rw-r--   0 knight    (1000) knight    (1000)      331 2023-02-24 14:27:00.000000 manifast-0.0.8/manifast/model_utils/__init__.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     2043 2023-02-25 01:29:23.000000 manifast-0.0.8/manifast/model_utils/eval_runtime.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     5513 2023-02-25 01:19:07.000000 manifast-0.0.8/manifast/model_utils/grad_cam.py
--rw-rw-r--   0 knight    (1000) knight    (1000)     3033 2023-02-24 13:01:54.000000 manifast-0.0.8/manifast/model_utils/summary.py
-drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-17 06:15:16.655279 manifast-0.0.8/manifast.egg-info/
--rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/PKG-INFO
--rw-rw-r--   0 knight    (1000) knight    (1000)     1264 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/SOURCES.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)        1 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/dependency_links.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)        9 2023-05-17 06:15:16.000000 manifast-0.0.8/manifast.egg-info/top_level.txt
--rw-rw-r--   0 knight    (1000) knight    (1000)      107 2023-05-17 06:15:16.659279 manifast-0.0.8/setup.cfg
--rw-rw-r--   0 knight    (1000) knight    (1000)     1442 2023-05-17 06:13:50.000000 manifast-0.0.8/setup.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/
+-rw-rw-r--   0 knight    (1000) knight    (1000)       33 2023-02-24 15:52:08.000000 manifast-0.0.9/MANIFEST.in
+-rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-19 06:41:29.428909 manifast-0.0.9/PKG-INFO
+-rw-rw-r--   0 knight    (1000) knight    (1000)       11 2023-02-24 09:21:56.000000 manifast-0.0.9/README.md
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      367 2023-02-24 15:58:02.000000 manifast-0.0.9/manifast/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/gui_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      321 2023-02-27 01:41:55.000000 manifast-0.0.9/manifast/gui_utils/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      422 2023-02-27 10:18:34.000000 manifast-0.0.9/manifast/gui_utils/counter.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      955 2023-05-19 06:32:00.000000 manifast-0.0.9/manifast/import_pkg.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/iostream/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      498 2023-04-20 07:01:48.000000 manifast-0.0.9/manifast/iostream/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1904 2023-04-20 07:05:50.000000 manifast-0.0.9/manifast/iostream/envstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4711 2023-05-19 06:31:19.000000 manifast-0.0.9/manifast/iostream/filestream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2217 2023-04-09 04:26:57.000000 manifast-0.0.9/manifast/iostream/imagestream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      773 2023-04-06 02:01:32.000000 manifast-0.0.9/manifast/iostream/logstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      680 2023-04-04 07:04:06.000000 manifast-0.0.9/manifast/iostream/pdstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1631 2023-04-09 04:32:18.000000 manifast-0.0.9/manifast/iostream/pltstream.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1307 2023-05-17 06:22:50.000000 manifast-0.0.9/manifast/iostream/processsing.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      329 2023-02-24 15:52:38.000000 manifast-0.0.9/manifast/label_utils/__init__.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/classify/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      338 2023-02-24 15:53:30.000000 manifast-0.0.9/manifast/label_utils/classify/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      344 2023-02-24 15:40:14.000000 manifast-0.0.9/manifast/label_utils/classify/gen_split_data.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/detect/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      336 2023-02-24 15:53:26.000000 manifast-0.0.9/manifast/label_utils/detect/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)      985 2023-02-25 14:16:00.000000 manifast-0.0.9/manifast/label_utils/detect/convert_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1903 2023-02-25 14:16:04.000000 manifast-0.0.9/manifast/label_utils/detect/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     5031 2023-02-25 14:16:06.000000 manifast-0.0.9/manifast/label_utils/detect/vis_label.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/label_utils/segment/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      337 2023-02-24 15:53:21.000000 manifast-0.0.9/manifast/label_utils/segment/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4301 2023-02-25 01:34:19.000000 manifast-0.0.9/manifast/label_utils/segment/colorize_mask.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     7249 2023-05-19 06:32:06.000000 manifast-0.0.9/manifast/label_utils/segment/convert_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1644 2023-02-25 02:17:38.000000 manifast-0.0.9/manifast/label_utils/segment/convert_utils.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3977 2023-02-25 14:17:05.000000 manifast-0.0.9/manifast/label_utils/segment/gen_split_data.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1236 2023-02-25 14:17:11.000000 manifast-0.0.9/manifast/label_utils/segment/vis_label.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     4864 2023-02-25 14:20:53.000000 manifast-0.0.9/manifast/label_utils/segment/vis_utils.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast/model_utils/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      331 2023-02-24 14:27:00.000000 manifast-0.0.9/manifast/model_utils/__init__.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     2043 2023-02-25 01:29:23.000000 manifast-0.0.9/manifast/model_utils/eval_runtime.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     5513 2023-02-25 01:19:07.000000 manifast-0.0.9/manifast/model_utils/grad_cam.py
+-rw-rw-r--   0 knight    (1000) knight    (1000)     3033 2023-02-24 13:01:54.000000 manifast-0.0.9/manifast/model_utils/summary.py
+drwxrwxr-x   0 knight    (1000) knight    (1000)        0 2023-05-19 06:41:29.428909 manifast-0.0.9/manifast.egg-info/
+-rw-rw-r--   0 knight    (1000) knight    (1000)      280 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/PKG-INFO
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1295 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/SOURCES.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)        1 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/dependency_links.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)       49 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/requires.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)        9 2023-05-19 06:41:29.000000 manifast-0.0.9/manifast.egg-info/top_level.txt
+-rw-rw-r--   0 knight    (1000) knight    (1000)      107 2023-05-19 06:41:29.428909 manifast-0.0.9/setup.cfg
+-rw-rw-r--   0 knight    (1000) knight    (1000)     1442 2023-05-19 06:41:20.000000 manifast-0.0.9/setup.py
```

### Comparing `manifast-0.0.8/manifast/iostream/envstream.py` & `manifast-0.0.9/manifast/iostream/envstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/iostream/filestream.py` & `manifast-0.0.9/manifast/iostream/filestream.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 16:57:43
 FilePath     : /manifast/manifast/iostream/filestream.py
 Description  : 
-LastEditTime : 2023-05-08 10:35:21
+LastEditTime : 2023-05-19 14:30:22
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 import os
 import time
 import json
@@ -86,26 +86,48 @@
             # p_tmp = [i for i in lines.split(' ')]
             constants.append(lines.strip('\n'))  # 添加新读取的数据
             # Efield.append(E_tmp)
             pass
     return constants
 
 
-def save_list2txt(data=[], save_path='./results.txt'):
+def save_list2txt(datas=[], save_path='./results.txt'):
     """
      description: 将data保存到指定的json文件下
      param       {*} data 
      param       {*} save_path
      return      {*}
     """
     with open(save_path, 'w') as f:
         pass
-    for file in data:
-        with open(save_path, 'a') as f:
-            f.write(file+'\n')
+    for data in datas:
+        if isinstance(data, int):
+            with open(save_path, 'a') as f:
+                f.write(str(data)+'\n')
+        elif isinstance(data, str):
+            with open(save_path, 'a') as f:
+                f.write(str(data)+'\n')
+        elif isinstance(data, list):
+            for dt in data:
+                with open(save_path, 'a') as f:
+                    f.write(str(dt)+',')
+            with open(save_path, 'a') as f:
+                f.write('\n')
+        elif isinstance(data, set):
+            for dt in data:
+                with open(save_path, 'a') as f:
+                    f.write(str(dt)+',')
+            with open(save_path, 'a') as f:
+                f.write('\n')
+        else:
+            for dt in data:
+                with open(save_path, 'a') as f:
+                    f.write(str(dt)+',')
+            with open(save_path, 'a') as f:
+                f.write('\n')
 
 
 def get_current_daytime():
     return time.strftime('%Y%m%d', time.localtime(time.time()))
 
 
 def get_current_clocktime():
```

### Comparing `manifast-0.0.8/manifast/iostream/imagestream.py` & `manifast-0.0.9/manifast/iostream/imagestream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/iostream/logstream.py` & `manifast-0.0.9/manifast/iostream/logstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/iostream/pdstream.py` & `manifast-0.0.9/manifast/iostream/pdstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/iostream/pltstream.py` & `manifast-0.0.9/manifast/iostream/pltstream.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/iostream/processsing.py` & `manifast-0.0.9/manifast/iostream/processsing.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/detect/convert_label.py` & `manifast-0.0.9/manifast/label_utils/detect/convert_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/detect/gen_split_data.py` & `manifast-0.0.9/manifast/label_utils/detect/gen_split_data.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/detect/vis_label.py` & `manifast-0.0.9/manifast/label_utils/detect/vis_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/segment/colorize_mask.py` & `manifast-0.0.9/manifast/label_utils/segment/colorize_mask.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/segment/convert_label.py` & `manifast-0.0.9/manifast/label_utils/segment/convert_label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 23:21:13
 FilePath     : /manifast/manifast/label_utils/segment/convert_label.py
 Description  : 
-LastEditTime : 2023-02-25 22:16:31
+LastEditTime : 2023-05-19 14:32:06
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 import json
 import numpy as np
 from manifast import *
 
@@ -80,15 +80,15 @@
                         "points": [], "shape_type": "polygon", "flags": {}}
         img_mark_inf["label"] = obj['label']
         img_mark_inf["shape_type"] = obj['shapeType']
         img_mark_inf["label"] = obj['label']
         for point in obj['coordinates'][0]:
             img_mark_inf["points"].append(point)
         json_dict["shapes"].append(img_mark_inf)
-    makePathDirs(label_save_path)
+    make_path_dirs(label_save_path)
     with open(label_save_path, "w") as out_json:
         json.dump(json_dict, out_json, ensure_ascii=False, indent=2)
     return label_mask_num
 
 
 def convertLabelJson2IdImage(json_path, label2num_dict):
     '''
```

### Comparing `manifast-0.0.8/manifast/label_utils/segment/convert_utils.py` & `manifast-0.0.9/manifast/label_utils/segment/convert_utils.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/segment/gen_split_data.py` & `manifast-0.0.9/manifast/label_utils/segment/gen_split_data.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/segment/vis_label.py` & `manifast-0.0.9/manifast/label_utils/segment/vis_label.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/label_utils/segment/vis_utils.py` & `manifast-0.0.9/manifast/label_utils/segment/vis_utils.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/model_utils/eval_runtime.py` & `manifast-0.0.9/manifast/model_utils/eval_runtime.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/model_utils/grad_cam.py` & `manifast-0.0.9/manifast/model_utils/grad_cam.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast/model_utils/summary.py` & `manifast-0.0.9/manifast/model_utils/summary.py`

 * *Files identical despite different names*

### Comparing `manifast-0.0.8/manifast.egg-info/SOURCES.txt` & `manifast-0.0.9/manifast.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.cfg
 setup.py
 manifast/__init__.py
 manifast/import_pkg.py
 manifast.egg-info/PKG-INFO
 manifast.egg-info/SOURCES.txt
 manifast.egg-info/dependency_links.txt
+manifast.egg-info/requires.txt
 manifast.egg-info/top_level.txt
 manifast/gui_utils/__init__.py
 manifast/gui_utils/counter.py
 manifast/iostream/__init__.py
 manifast/iostream/envstream.py
 manifast/iostream/filestream.py
 manifast/iostream/imagestream.py
```

### Comparing `manifast-0.0.8/setup.py` & `manifast-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 '''
 brief        :  
 Author       : knightdby knightdby@163.com
 Date         : 2023-02-24 15:48:13
 FilePath     : /manifast/setup.py
 Description  : 
-LastEditTime : 2023-05-17 14:13:49
+LastEditTime : 2023-05-19 14:41:19
 LastEditors  : knightdby
 Copyright (c) 2023 by Inc, All Rights Reserved.
 '''
 
 
 from os import path
 from setuptools import setup, find_packages
@@ -25,15 +25,15 @@
 install_requires = [x.strip() for x in all_reqs if 'git+' not in x]
 
 # 读取readme文件
 with open("README.md", "r", encoding='utf-8') as f:
     readme = f.read()
 setup(
     name="manifast",  # 包名称
-    version="0.0.8",  # 版本
+    version="0.0.9",  # 版本
     author="Knight",  # 包邮箱
     author_email="knightdby@163.com",  # 作者邮箱
     description="A small example package",  # 包描述
     license='MIT License',
     # 长描述，通常是readme ,打包到PiPy需要 。
     long_description=long_description,
     long_description_content_type='text/markdown',
```

