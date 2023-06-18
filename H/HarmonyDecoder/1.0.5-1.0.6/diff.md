# Comparing `tmp/HarmonyDecoder-1.0.5.tar.gz` & `tmp/HarmonyDecoder-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HarmonyDecoder-1.0.5.tar", last modified: Sun Jun 18 19:39:20 2023, max compression
+gzip compressed data, was "HarmonyDecoder-1.0.6.tar", last modified: Sun Jun 18 19:44:11 2023, max compression
```

## Comparing `HarmonyDecoder-1.0.5.tar` & `HarmonyDecoder-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 19:39:20.572533 HarmonyDecoder-1.0.5/
--rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    42858 2023-06-18 19:39:20.572533 HarmonyDecoder-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.5/README.md
--rw-rw-rw-   0        0        0      722 2023-06-18 19:39:06.000000 HarmonyDecoder-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 19:39:20.572533 HarmonyDecoder-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 19:39:20.541296 HarmonyDecoder-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 19:39:20.556903 HarmonyDecoder-1.0.5/src/HarmonyDecoder/
-drwxrwxrwx   0        0        0        0 2023-06-18 19:39:20.572533 HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/
--rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/BassCleff.png
--rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/Flat.png
--rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/Icon.png
--rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/Sharp.png
--rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/TrebleCleff.png
--rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/__init__.py
--rw-rw-rw-   0        0        0    10873 2023-06-18 19:34:00.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/drawing.py
--rw-rw-rw-   0        0        0     4202 2023-06-18 19:35:14.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/function.py
--rw-rw-rw-   0        0        0       86 2023-06-18 19:34:38.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/harmony.py
--rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/interval.py
--rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/logger.py
--rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/note.py
--rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/possiblenotes.py
--rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/program.py
--rw-rw-rw-   0        0        0    14974 2023-06-16 14:46:12.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/rules.py
--rw-rw-rw-   0        0        0     4237 2023-06-16 07:17:20.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/scale.py
--rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/setup.py
--rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/strdecoder.py
--rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-18 19:39:20.572533 HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-06-18 19:39:20.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-18 19:39:20.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 19:39:20.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-18 19:39:20.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 19:39:20.000000 HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    42858 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.6/README.md
+-rw-rw-rw-   0        0        0      722 2023-06-18 19:43:55.000000 HarmonyDecoder-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.731531 HarmonyDecoder-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.747151 HarmonyDecoder-1.0.6/src/HarmonyDecoder/
+drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/
+-rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/BassCleff.png
+-rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Flat.png
+-rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Icon.png
+-rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Sharp.png
+-rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/TrebleCleff.png
+-rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/__init__.py
+-rw-rw-rw-   0        0        0    10873 2023-06-18 19:34:00.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/drawing.py
+-rw-rw-rw-   0        0        0     4202 2023-06-18 19:35:14.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/function.py
+-rw-rw-rw-   0        0        0       86 2023-06-18 19:34:38.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/harmony.py
+-rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/interval.py
+-rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/logger.py
+-rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/note.py
+-rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/possiblenotes.py
+-rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/program.py
+-rw-rw-rw-   0        0        0    15019 2023-06-18 19:42:46.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/rules.py
+-rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/scale.py
+-rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/setup.py
+-rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/strdecoder.py
+-rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-18 19:44:11.762773 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 19:44:11.000000 HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/top_level.txt
```

### Comparing `HarmonyDecoder-1.0.5/LICENSE` & `HarmonyDecoder-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/PKG-INFO` & `HarmonyDecoder-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.5
+Version: 1.0.6
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.5/README.md` & `HarmonyDecoder-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/pyproject.toml` & `HarmonyDecoder-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HarmonyDecoder"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" },
 ]
 maintainers = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" }
 ]
 dependencies = [
```

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/BassCleff.png` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/BassCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/Flat.png` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Flat.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/Icon.png` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Icon.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/Sharp.png` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/Sharp.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/Images/TrebleCleff.png` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/Images/TrebleCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/drawing.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/drawing.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/function.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/function.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/interval.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/interval.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/note.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/note.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/possiblenotes.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/possiblenotes.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/program.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/program.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/rules.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import abc
 
-from function import *
-from possiblenotes import possible_notes
-from scale import scale
+from HarmonyDecoder.function import *
+from HarmonyDecoder.possiblenotes import possible_notes
+from HarmonyDecoder.scale import scale
 
 class rule_manager:
     def __init__(self):
         self._active_rules:list[rule] = [
             voice_crossing(),
             parallel_fifth(),
             parallel_octave(),
```

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/scale.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from note import all_notes
+from HarmonyDecoder.note import all_notes
 
 scale_notes : list[str] = ['C', 'D', 'E', 'F', 'G', 'A', 'B']
 modes:list[str] = ["minor", "major"]
 
 sharps : list[int] = [3, 0, 4, 1, 5, 2, 6, 3, 0, 4, 1, 5, 2, 6]
 flats : list[int] = [6, 2, 5, 1, 4, 0, 3, 6, 2, 5, 1, 4, 0, 3]
```

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/strdecoder.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/strdecoder.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder/ui.py` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder/ui.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/PKG-INFO` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.5
+Version: 1.0.6
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.5/src/HarmonyDecoder.egg-info/SOURCES.txt` & `HarmonyDecoder-1.0.6/src/HarmonyDecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

