# Comparing `tmp/HarmonyDecoder-1.0.7.tar.gz` & `tmp/HarmonyDecoder-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HarmonyDecoder-1.0.7.tar", last modified: Sun Jun 18 20:19:00 2023, max compression
+gzip compressed data, was "HarmonyDecoder-1.0.8.tar", last modified: Sun Jun 18 20:26:51 2023, max compression
```

## Comparing `HarmonyDecoder-1.0.7.tar` & `HarmonyDecoder-1.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/
--rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    42858 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.7/README.md
--rw-rw-rw-   0        0        0      722 2023-06-18 20:18:48.000000 HarmonyDecoder-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.242725 HarmonyDecoder-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.255935 HarmonyDecoder-1.0.7/src/HarmonyDecoder/
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/
--rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/BassCleff.png
--rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Flat.png
--rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Icon.png
--rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Sharp.png
--rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/TrebleCleff.png
--rw-rw-rw-   0        0        0      207 2023-06-18 20:02:32.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/__init__.py
--rw-rw-rw-   0        0        0    11022 2023-06-18 20:16:53.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/drawing.py
--rw-rw-rw-   0        0        0     4202 2023-06-18 20:05:58.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/function.py
--rw-rw-rw-   0        0        0       86 2023-06-18 19:34:38.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/harmony.py
--rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/interval.py
--rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/logger.py
--rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/note.py
--rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/possiblenotes.py
--rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/program.py
--rw-rw-rw-   0        0        0    15019 2023-06-18 19:42:46.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/rules.py
--rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/scale.py
--rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/setup.py
--rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/strdecoder.py
--rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:19:00.271560 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 20:19:00.000000 HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    42858 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.8/README.md
+-rw-rw-rw-   0        0        0      722 2023-06-18 20:26:25.000000 HarmonyDecoder-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.141614 HarmonyDecoder-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.161736 HarmonyDecoder-1.0.8/src/HarmonyDecoder/
+drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/
+-rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/BassCleff.png
+-rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Flat.png
+-rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Icon.png
+-rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Sharp.png
+-rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/TrebleCleff.png
+-rw-rw-rw-   0        0        0      207 2023-06-18 20:02:32.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/__init__.py
+-rw-rw-rw-   0        0        0    11022 2023-06-18 20:16:53.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/drawing.py
+-rw-rw-rw-   0        0        0     4202 2023-06-18 20:05:58.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/function.py
+-rw-rw-rw-   0        0        0       55 2023-06-18 20:24:39.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/harmony.py
+-rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/interval.py
+-rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/logger.py
+-rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/note.py
+-rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/possiblenotes.py
+-rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/program.py
+-rw-rw-rw-   0        0        0    15019 2023-06-18 19:42:46.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/rules.py
+-rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/scale.py
+-rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/setup.py
+-rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/strdecoder.py
+-rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/top_level.txt
```

### Comparing `HarmonyDecoder-1.0.7/LICENSE` & `HarmonyDecoder-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/PKG-INFO` & `HarmonyDecoder-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.7
+Version: 1.0.8
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.7/README.md` & `HarmonyDecoder-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/pyproject.toml` & `HarmonyDecoder-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HarmonyDecoder"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" },
 ]
 maintainers = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" }
 ]
 dependencies = [
```

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/BassCleff.png` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/BassCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Flat.png` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Flat.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Icon.png` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Icon.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/Sharp.png` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Sharp.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/Images/TrebleCleff.png` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/TrebleCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/drawing.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/drawing.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/function.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/function.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/interval.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/interval.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/note.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/note.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/possiblenotes.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/possiblenotes.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/program.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/program.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/rules.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/rules.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/scale.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/scale.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/strdecoder.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/strdecoder.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder/ui.py` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder/ui.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/PKG-INFO` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.7
+Version: 1.0.8
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.7/src/HarmonyDecoder.egg-info/SOURCES.txt` & `HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

