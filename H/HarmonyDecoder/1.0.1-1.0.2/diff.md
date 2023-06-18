# Comparing `tmp/HarmonyDecoder-1.0.1.tar.gz` & `tmp/HarmonyDecoder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HarmonyDecoder-1.0.1.tar", last modified: Sun Jun 18 18:17:18 2023, max compression
+gzip compressed data, was "HarmonyDecoder-1.0.2.tar", last modified: Sun Jun 18 18:35:18 2023, max compression
```

## Comparing `HarmonyDecoder-1.0.1.tar` & `HarmonyDecoder-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:18.140392 HarmonyDecoder-1.0.1/
--rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    42858 2023-06-18 18:17:18.138631 HarmonyDecoder-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.1/README.md
--rw-rw-rw-   0        0        0      692 2023-06-18 18:16:39.000000 HarmonyDecoder-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 18:17:18.140582 HarmonyDecoder-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:18.051908 HarmonyDecoder-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:18.106274 HarmonyDecoder-1.0.1/src/HarmonyDecoder/
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:18.134199 HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/
--rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/BassCleff.png
--rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/Flat.png
--rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/Icon.png
--rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/Sharp.png
--rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/TrebleCleff.png
--rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/__init__.py
--rw-rw-rw-   0        0        0    10813 2023-06-17 22:03:06.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/drawing.py
--rw-rw-rw-   0        0        0     4157 2023-06-15 20:39:57.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/function.py
--rw-rw-rw-   0        0        0       71 2023-06-16 06:03:03.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/harmony.py
--rw-rw-rw-   0        0        0     2570 2023-06-09 14:48:03.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/interval.py
--rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/logger.py
--rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/note.py
--rw-rw-rw-   0        0        0     3181 2023-06-15 19:43:45.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/possiblenotes.py
--rw-rw-rw-   0        0        0     7171 2023-06-17 21:10:51.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/program.py
--rw-rw-rw-   0        0        0    14974 2023-06-16 14:46:12.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/rules.py
--rw-rw-rw-   0        0        0     4237 2023-06-16 07:17:20.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/scale.py
--rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/setup.py
--rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/strdecoder.py
--rw-rw-rw-   0        0        0    37439 2023-06-18 17:40:04.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:17:18.119855 HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-06-18 18:17:18.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-18 18:17:18.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 18:17:18.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-18 18:17:18.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 18:17:18.000000 HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 18:35:18.438327 HarmonyDecoder-1.0.2/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    42858 2023-06-18 18:35:18.437479 HarmonyDecoder-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.2/README.md
+-rw-rw-rw-   0        0        0      735 2023-06-18 18:34:47.000000 HarmonyDecoder-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-18 18:35:18.439330 HarmonyDecoder-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-18 18:35:18.343670 HarmonyDecoder-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 18:35:18.401425 HarmonyDecoder-1.0.2/src/HarmonyDecoder/
+drwxrwxrwx   0        0        0        0 2023-06-18 18:35:18.433335 HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/
+-rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/BassCleff.png
+-rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/Flat.png
+-rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/Icon.png
+-rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/Sharp.png
+-rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/TrebleCleff.png
+-rw-rw-rw-   0        0        0        0 2023-06-18 16:49:10.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/__init__.py
+-rw-rw-rw-   0        0        0    10813 2023-06-17 22:03:06.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/drawing.py
+-rw-rw-rw-   0        0        0     4157 2023-06-15 20:39:57.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/function.py
+-rw-rw-rw-   0        0        0       71 2023-06-16 06:03:03.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/harmony.py
+-rw-rw-rw-   0        0        0     2570 2023-06-09 14:48:03.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/interval.py
+-rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/logger.py
+-rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/note.py
+-rw-rw-rw-   0        0        0     3181 2023-06-15 19:43:45.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/possiblenotes.py
+-rw-rw-rw-   0        0        0     7171 2023-06-17 21:10:51.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/program.py
+-rw-rw-rw-   0        0        0    14974 2023-06-16 14:46:12.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/rules.py
+-rw-rw-rw-   0        0        0     4237 2023-06-16 07:17:20.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/scale.py
+-rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/setup.py
+-rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/strdecoder.py
+-rw-rw-rw-   0        0        0    37439 2023-06-18 17:40:04.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-18 18:35:18.418647 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-18 18:35:18.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-06-18 18:35:18.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 18:35:18.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-18 18:35:18.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 18:35:18.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-18 18:35:18.000000 HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/top_level.txt
```

### Comparing `HarmonyDecoder-1.0.1/LICENSE` & `HarmonyDecoder-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/PKG-INFO` & `HarmonyDecoder-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.1
+Version: 1.0.2
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.1/README.md` & `HarmonyDecoder-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/pyproject.toml` & `HarmonyDecoder-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HarmonyDecoder"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" },
 ]
 maintainers = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" }
 ]
 keywords = ["harmony", "music", "notes", "decoder", "parser"]
@@ -18,9 +18,12 @@
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Operating System :: OS Independent",
 ]
 
+[project.scripts]
+installer = "installer"
+
 [project.optional-dependencies]
 gui = ["PyQt5"]
```

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/BassCleff.png` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/BassCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/Flat.png` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/Flat.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/Icon.png` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/Icon.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/Sharp.png` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/Sharp.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/Images/TrebleCleff.png` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/Images/TrebleCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/drawing.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/drawing.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/function.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/function.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/interval.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/interval.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/note.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/note.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/possiblenotes.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/possiblenotes.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/program.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/program.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/rules.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/rules.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/scale.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/scale.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/strdecoder.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/strdecoder.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder/ui.py` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder/ui.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/PKG-INFO` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.1
+Version: 1.0.2
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.1/src/HarmonyDecoder.egg-info/SOURCES.txt` & `HarmonyDecoder-1.0.2/src/HarmonyDecoder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/HarmonyDecoder/scale.py
 src/HarmonyDecoder/setup.py
 src/HarmonyDecoder/strdecoder.py
 src/HarmonyDecoder/ui.py
 src/HarmonyDecoder.egg-info/PKG-INFO
 src/HarmonyDecoder.egg-info/SOURCES.txt
 src/HarmonyDecoder.egg-info/dependency_links.txt
+src/HarmonyDecoder.egg-info/entry_points.txt
 src/HarmonyDecoder.egg-info/requires.txt
 src/HarmonyDecoder.egg-info/top_level.txt
 src/HarmonyDecoder/Images/BassCleff.png
 src/HarmonyDecoder/Images/Flat.png
 src/HarmonyDecoder/Images/Icon.png
 src/HarmonyDecoder/Images/Sharp.png
 src/HarmonyDecoder/Images/TrebleCleff.png
```

