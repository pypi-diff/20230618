# Comparing `tmp/HarmonyDecoder-1.0.6.tar.gz` & `tmp/HarmonyDecoder-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HarmonyDecoder-1.0.6.tar", last modified: Sun Jun 18 19:44:11 2023, max compression
+gzip compressed data, was "HarmonyDecoder-1.0.7.tar", last modified: Sun Jun 18 20:19:00 2023, max compression
```

## Comparing `HarmonyDecoder-1.0.6.tar` & `HarmonyDecoder-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/
--rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    42858 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.6/README.md
--rw-rw-rw-   0        0        0      722 2023-06-18 19:43:55.000000 HarmonyDecoder-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.731531 HarmonyDecoder-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.747151 HarmonyDecoder-1.0.6/src/HarmonyDecoder/
-drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/
--rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/BassCleff.png
--rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Flat.png
--rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Icon.png
--rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Sharp.png
--rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/TrebleCleff.png
--rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/__init__.py
--rw-rw-rw-   0        0        0    10873 2023-06-18 19:34:00.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/drawing.py
--rw-rw-rw-   0        0        0     4202 2023-06-18 19:35:14.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/function.py
--rw-rw-rw-   0        0        0       86 2023-06-18 19:34:38.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/harmony.py
--rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/interval.py
--rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/logger.py
--rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/note.py
--rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/possiblenotes.py
--rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/program.py
--rw-rw-rw-   0        0        0    15019 2023-06-18 19:42:46.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/rules.py
--rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/scale.py
--rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/setup.py
--rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/strdecoder.py
--rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    42858 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.7/README.md
+-rw-rw-rw-   0        0        0      722 2023-06-18 20:18:48.000000 HarmonyDecoder-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.242725 HarmonyDecoder-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.255935 HarmonyDecoder-1.0.7/src/HarmonyDecoder/
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/
+-rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/BassCleff.png
+-rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Flat.png
+-rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Icon.png
+-rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Sharp.png
+-rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/TrebleCleff.png
+-rw-rw-rw-   0        0        0      207 2023-06-18 20:02:32.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/__init__.py
+-rw-rw-rw-   0        0        0    11022 2023-06-18 20:16:53.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/drawing.py
+-rw-rw-rw-   0        0        0     4202 2023-06-18 20:05:58.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/function.py
+-rw-rw-rw-   0        0        0       86 2023-06-18 19:34:38.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/harmony.py
+-rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/interval.py
+-rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/logger.py
+-rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/note.py
+-rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/possiblenotes.py
+-rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/program.py
+-rw-rw-rw-   0        0        0    15019 2023-06-18 19:42:46.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/rules.py
+-rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/scale.py
+-rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/setup.py
+-rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/strdecoder.py
+-rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/top_level.txt
```

### Comparing `HarmonyDecoder-1.0.6/LICENSE` & `HarmonyDecoder-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/PKG-INFO` & `HarmonyDecoder-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.6
+Version: 1.0.7
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.6/README.md` & `HarmonyDecoder-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/pyproject.toml` & `HarmonyDecoder-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HarmonyDecoder"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" },
 ]
 maintainers = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" }
 ]
 dependencies = [
```

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/BassCleff.png` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/BassCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Flat.png` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Flat.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Icon.png` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Icon.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Sharp.png` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Sharp.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/TrebleCleff.png` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/TrebleCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/drawing.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 from PIL import Image, ImageDraw
 from HarmonyDecoder.note import note
 from HarmonyDecoder.function import function
 from HarmonyDecoder.note import note
 from HarmonyDecoder.scale import scale
-
+import os
 
 
 class drawing:
     def __init__(self, tonation:scale = scale('C', 'major')) -> None:
         if tonation is None:
             raise TypeError("tonation cannot be none")
 
         self.__staff_line_spacing:int = 20
         self.__staff_spacing:int = 300
         self.__staff_line_width:int = 5
         self.__tonation:scale = tonation
 
-        self.__flat:Image.Image = Image.open("Images/Flat.png")
-        self.__sharp:Image.Image = Image.open("Images/Sharp.png")
+        self.__flat:Image.Image = Image.open(f"{os.path.dirname(os.path.realpath(__file__))}/Images/Flat.png")
+        self.__sharp:Image.Image = Image.open(f"{os.path.dirname(os.path.realpath(__file__))}/Images/Sharp.png")
         self.__resize_signs()
 
         self.__note_line_heigth:int = self.__staff_line_spacing * 5
         self.__function_spacing:int = 5 * self.__staff_line_spacing
 
         self.__size_x:int = 3508
         self.__size_y:int = 600
@@ -227,15 +227,15 @@
             raise ValueError("Cannot draw staff outside of the canvas.")
         
         scale:int = 0.5 if cleff == 'Bass' else 1
 
         self.insert_image(
             self.__margin_x + self.__function_spacing,
             self.__margin_y + 2 * self.__staff_line_spacing + pos_y,
-            f'Images/{cleff}Cleff.png',
+            f'{os.path.dirname(os.path.realpath(__file__))}/Images/{cleff}Cleff.png',
             scale=scale
         )
 
         for index in range(5):
             start_x:int = self.__margin_x
             end_x:int = self.__size_x - self.__margin_x
```

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/function.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/function.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/interval.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/interval.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/note.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/note.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/possiblenotes.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/possiblenotes.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/program.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/program.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/rules.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/rules.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/scale.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/scale.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/strdecoder.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/strdecoder.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder/ui.py` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder/ui.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/PKG-INFO` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.6
+Version: 1.0.7
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/SOURCES.txt` & `HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

