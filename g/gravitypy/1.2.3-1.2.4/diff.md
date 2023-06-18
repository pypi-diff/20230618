# Comparing `tmp/gravitypy-1.2.3.tar.gz` & `tmp/gravitypy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.2.3.tar", last modified: Sun Jun 18 20:32:46 2023, max compression
+gzip compressed data, was "gravitypy-1.2.4.tar", last modified: Sun Jun 18 20:37:28 2023, max compression
```

## Comparing `gravitypy-1.2.3.tar` & `gravitypy-1.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.3/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.3/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-18 20:32:46.496900 gravitypy-1.2.3/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1480 2023-06-05 17:20:56.000000 gravitypy-1.2.3/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.492900 gravitypy-1.2.3/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.3/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.3/gravitypy/__main__.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/gravitypy/button/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.3/gravitypy/button/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2695 2023-06-05 17:14:48.000000 gravitypy-1.2.3/gravitypy/button/button.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    14542 2023-06-18 20:29:55.000000 gravitypy-1.2.3/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/gravitypy/particle/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.3/gravitypy/particle/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6138 2023-05-27 20:03:20.000000 gravitypy-1.2.3/gravitypy/particle/particle.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.492900 gravitypy-1.2.3/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.3/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.492900 gravitypy-1.2.3/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      480 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.3/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-18 20:32:46.496900 gravitypy-1.2.3/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-06-18 20:32:05.000000 gravitypy-1.2.3/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.4/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.4/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-18 20:37:28.214031 gravitypy-1.2.4/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1480 2023-06-05 17:20:56.000000 gravitypy-1.2.4/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.4/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.4/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.4/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2695 2023-06-05 17:14:48.000000 gravitypy-1.2.4/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    14539 2023-06-18 20:36:59.000000 gravitypy-1.2.4/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.4/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6138 2023-05-27 20:03:20.000000 gravitypy-1.2.4/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.4/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:37:28.214031 gravitypy-1.2.4/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-18 20:37:28.000000 gravitypy-1.2.4/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      480 2023-06-18 20:37:28.000000 gravitypy-1.2.4/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-18 20:37:28.000000 gravitypy-1.2.4/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-06-18 20:37:28.000000 gravitypy-1.2.4/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-06-18 20:37:28.000000 gravitypy-1.2.4/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-06-18 20:37:28.000000 gravitypy-1.2.4/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.4/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-18 20:37:28.214031 gravitypy-1.2.4/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-06-18 20:34:11.000000 gravitypy-1.2.4/setup.py
```

### Comparing `gravitypy-1.2.3/LICENSE` & `gravitypy-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.3/README.md` & `gravitypy-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.3/gravitypy/button/button.py` & `gravitypy-1.2.4/gravitypy/button/button.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.3/gravitypy/main.py` & `gravitypy-1.2.4/gravitypy/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pygame
 import random
 import math
 import os
 from pygame.locals import *
-from button.button import Buttons
-from particle.particle import Particles, QuadTree
+from .button.button import Buttons
+from .particle.particle import Particles, QuadTree
 
 def main():
     pygame.init()
     pygame.display.set_caption("GravityPy")
     
     current_file = __file__
     current_dir = os.path.dirname(current_file)
@@ -318,8 +318,8 @@
                 particle.update()
                 quadtree.calculate_forces(particle, G)
             particle.draw_scaled(MOUSE_X, MOUSE_Y, SCALE, WIDTH, HEIGHT, SCREEN, FONT)
 
         pygame.display.update()
         CLOCK.tick(60)
     pygame.quit()
-main()
+
```

### Comparing `gravitypy-1.2.3/gravitypy/particle/particle.py` & `gravitypy-1.2.4/gravitypy/particle/particle.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.3/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.2.4/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.3/setup.py` & `gravitypy-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.2.3',
+   version='1.2.4',
    description='GravityPy',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/gravityPy",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```

