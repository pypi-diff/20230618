# Comparing `tmp/HarmonyDecoder-1.0.3.tar.gz` & `tmp/HarmonyDecoder-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HarmonyDecoder-1.0.3.tar", last modified: Sun Jun 18 18:42:19 2023, max compression
+gzip compressed data, was "HarmonyDecoder-1.0.4.tar", last modified: Sun Jun 18 18:45:03 2023, max compression
```

## Comparing `HarmonyDecoder-1.0.3.tar` & `HarmonyDecoder-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 18:42:19.750584 HarmonyDecoder-1.0.3/
--rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    42858 2023-06-18 18:42:19.748493 HarmonyDecoder-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.3/README.md
--rw-rw-rw-   0        0        0      737 2023-06-18 18:41:49.000000 HarmonyDecoder-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 18:42:19.751129 HarmonyDecoder-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 18:42:19.664956 HarmonyDecoder-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 18:42:19.714608 HarmonyDecoder-1.0.3/src/HarmonyDecoder/
-drwxrwxrwx   0        0        0        0 2023-06-18 18:42:19.744428 HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/
--rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/BassCleff.png
--rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/Flat.png
--rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/Icon.png
--rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/Sharp.png
--rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/TrebleCleff.png
--rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/__init__.py
--rw-rw-rw-   0        0        0    10813 2023-06-17 22:03:06.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/drawing.py
--rw-rw-rw-   0        0        0     4157 2023-06-15 20:39:57.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/function.py
--rw-rw-rw-   0        0        0       71 2023-06-16 06:03:03.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/harmony.py
--rw-rw-rw-   0        0        0     2570 2023-06-09 14:48:03.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/interval.py
--rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/logger.py
--rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/note.py
--rw-rw-rw-   0        0        0     3181 2023-06-15 19:43:45.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/possiblenotes.py
--rw-rw-rw-   0        0        0     7171 2023-06-17 21:10:51.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/program.py
--rw-rw-rw-   0        0        0    14974 2023-06-16 14:46:12.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/rules.py
--rw-rw-rw-   0        0        0     4237 2023-06-16 07:17:20.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/scale.py
--rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/setup.py
--rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/strdecoder.py
--rw-rw-rw-   0        0        0    37439 2023-06-18 17:40:04.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:42:19.727748 HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-06-18 18:42:19.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-18 18:42:19.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 18:42:19.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-18 18:42:19.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 18:42:19.000000 HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 18:45:03.923120 HarmonyDecoder-1.0.4/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    42858 2023-06-18 18:45:03.921627 HarmonyDecoder-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.4/README.md
+-rw-rw-rw-   0        0        0      722 2023-06-18 18:44:26.000000 HarmonyDecoder-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 18:45:03.923367 HarmonyDecoder-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 18:45:03.832557 HarmonyDecoder-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 18:45:03.890151 HarmonyDecoder-1.0.4/src/HarmonyDecoder/
+drwxrwxrwx   0        0        0        0 2023-06-18 18:45:03.917540 HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/
+-rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/BassCleff.png
+-rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/Flat.png
+-rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/Icon.png
+-rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/Sharp.png
+-rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/TrebleCleff.png
+-rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/__init__.py
+-rw-rw-rw-   0        0        0    10813 2023-06-17 22:03:06.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/drawing.py
+-rw-rw-rw-   0        0        0     4157 2023-06-15 20:39:57.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/function.py
+-rw-rw-rw-   0        0        0       71 2023-06-16 06:03:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/harmony.py
+-rw-rw-rw-   0        0        0     2570 2023-06-09 14:48:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/interval.py
+-rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/logger.py
+-rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/note.py
+-rw-rw-rw-   0        0        0     3181 2023-06-15 19:43:45.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/possiblenotes.py
+-rw-rw-rw-   0        0        0     7171 2023-06-17 21:10:51.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/program.py
+-rw-rw-rw-   0        0        0    14974 2023-06-16 14:46:12.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/rules.py
+-rw-rw-rw-   0        0        0     4237 2023-06-16 07:17:20.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/scale.py
+-rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/setup.py
+-rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/strdecoder.py
+-rw-rw-rw-   0        0        0    37439 2023-06-18 17:40:04.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:45:03.903725 HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-18 18:45:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-06-18 18:45:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:45:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-18 18:45:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 18:45:03.000000 HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/top_level.txt
```

### Comparing `HarmonyDecoder-1.0.3/LICENSE` & `HarmonyDecoder-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/PKG-INFO` & `HarmonyDecoder-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.3
+Version: 1.0.4
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.3/README.md` & `HarmonyDecoder-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/pyproject.toml` & `HarmonyDecoder-1.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HarmonyDecoder"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" },
 ]
 maintainers = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" }
 ]
 dependencies = [
   "pyqt5",
-  "itertools",
 ]
 keywords = ["harmony", "music", "notes", "decoder", "parser"]
 description = "HarmonyDecoder package"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/BassCleff.png` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/BassCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/Flat.png` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/Flat.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/Icon.png` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/Icon.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/Sharp.png` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/Sharp.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/Images/TrebleCleff.png` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/Images/TrebleCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/drawing.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/drawing.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/function.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/function.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/interval.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/interval.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/note.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/note.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/possiblenotes.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/possiblenotes.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/program.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/program.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/rules.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/rules.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/scale.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/scale.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/strdecoder.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/strdecoder.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder/ui.py` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder/ui.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/PKG-INFO` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.3
+Version: 1.0.4
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.3/src/HarmonyDecoder.egg-info/SOURCES.txt` & `HarmonyDecoder-1.0.4/src/HarmonyDecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

