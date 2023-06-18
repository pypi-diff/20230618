# Comparing `tmp/PyGraphica-1.0.0.tar.gz` & `tmp/PyGraphica-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-1.0.0.tar", last modified: Sun Jun 18 06:34:46 2023, max compression
+gzip compressed data, was "PyGraphica-1.0.1.tar", last modified: Sun Jun 18 07:49:48 2023, max compression
```

## Comparing `PyGraphica-1.0.0.tar` & `PyGraphica-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 06:34:46.083059 PyGraphica-1.0.0/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0    12031 2023-06-18 06:34:46.083059 PyGraphica-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    11449 2023-06-18 02:33:30.000000 PyGraphica-1.0.0/README.md
--rw-rw-rw-   0        0        0      563 2023-06-18 06:34:46.090843 PyGraphica-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      449 2023-06-18 06:32:33.000000 PyGraphica-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:34:46.045306 PyGraphica-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 06:34:46.055559 PyGraphica-1.0.0/src/PyGraphica/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-1.0.0/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-1.0.0/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0    28525 2023-06-18 02:26:44.000000 PyGraphica-1.0.0/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0      539 2023-06-18 02:20:41.000000 PyGraphica-1.0.0/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-1.0.0/src/PyGraphica/origins.py
-drwxrwxrwx   0        0        0        0 2023-06-18 06:34:46.083059 PyGraphica-1.0.0/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0    12031 2023-06-18 06:34:46.000000 PyGraphica-1.0.0/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-06-18 06:34:46.000000 PyGraphica-1.0.0/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 06:34:46.000000 PyGraphica-1.0.0/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-18 06:34:46.000000 PyGraphica-1.0.0/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 06:34:46.000000 PyGraphica-1.0.0/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 07:49:48.404817 PyGraphica-1.0.1/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2023-06-18 07:49:48.404817 PyGraphica-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11791 2023-06-18 07:03:21.000000 PyGraphica-1.0.1/README.md
+-rw-rw-rw-   0        0        0    14670 2023-06-18 07:47:17.000000 PyGraphica-1.0.1/README.txt
+-rw-rw-rw-   0        0        0      116 2023-06-18 07:49:48.407027 PyGraphica-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      449 2023-06-18 07:48:16.000000 PyGraphica-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 07:49:48.348668 PyGraphica-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 07:49:48.379450 PyGraphica-1.0.1/src/PyGraphica/
+-rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-1.0.1/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-1.0.1/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0    28525 2023-06-18 02:26:44.000000 PyGraphica-1.0.1/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0      994 2023-06-18 06:43:44.000000 PyGraphica-1.0.1/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-1.0.1/src/PyGraphica/origins.py
+drwxrwxrwx   0        0        0        0 2023-06-18 07:49:48.403818 PyGraphica-1.0.1/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-06-18 07:49:48.000000 PyGraphica-1.0.1/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-06-18 07:49:48.000000 PyGraphica-1.0.1/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 07:49:48.000000 PyGraphica-1.0.1/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-18 07:49:48.000000 PyGraphica-1.0.1/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 07:49:48.000000 PyGraphica-1.0.1/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-1.0.0/LICENSE.txt` & `PyGraphica-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-1.0.0/PKG-INFO` & `PyGraphica-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1
-Name: PyGraphica
-Version: 1.0.0
-Summary: PyGraphica is a simple GUI and game development module designed for Python, built of the Python bindings (pysdl2) for SDL-2.
-Home-page: https://github.com/LukeCampbell5853/PyGraphica
-Author: Luke Campbell
-Author-email: LukeCampbell5853@gmail.com
-License: MIT
-Keywords: gui
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: markdown
-License-File: LICENSE.txt
-
-## **PyGraphica** *1.0.0*
+## **PyGraphica** *1.0.1*
 *By Luke Campbell*
 
 PyGraphica is a simple GUI and game development module designed for Python, built of the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
@@ -28,15 +12,15 @@
 
     py -m pip install PyGraphica
 *for windows*
 
     python -m pip install PyGraphica
 *for linux*
 
-However the source code can be downloaded from GitHub, [here](youtube.com/watch?v=dQw4w9WgXcQ) if pip install fails.
+However the source code can be downloaded from GitHub, [here](https://github.com/LukeCampbell5853/PyGraphica) if pip install fails.
 
 Once the module has been imported, add it to your Python project like this:
 
     from PyGraphica import draw, colours, origins, fonts
 
 \
 **Colours, Origins, and Fonts files**
@@ -125,14 +109,20 @@
 |comm_changes| command keys newly pressed by the user (not held)
 |caps| whether capslock is on or shift is held|
 |mouse_x| x position of the mouse|
 |mouse_y| y position of the mouse
 |mouse_down| whether the mouse button is held down|
 |mouse_held| whether the mouse button is held down for more than one cycle|
 
+A window object has two important methods, running() and update(). running() will return whether the window's close button has been pressed yet, and update() will display all your objects to the screen. These two can be combined into the following cycle:
+
+    while app.running():
+        #do stuff
+        app.update()
+
 \
 **Creating a line**
 
 The line class can be defined by the following attributes:
 
 |attribute| type| description|
 |--|--|--|
@@ -298,9 +288,8 @@
     draw.to_font(player)
 
 \
 **Delete function**
 
 This function is used to delete an object. For example:
 
-    draw.delete(rect1)
-
+    draw.delete(rect1)
```

### Comparing `PyGraphica-1.0.0/src/PyGraphica/colours.py` & `PyGraphica-1.0.1/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-1.0.0/src/PyGraphica/draw.py` & `PyGraphica-1.0.1/src/PyGraphica/draw.py`

 * *Files identical despite different names*

