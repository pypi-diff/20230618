# Comparing `tmp/gravitypy-1.2.2.tar.gz` & `tmp/gravitypy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.2.2.tar", last modified: Mon Jun  5 17:34:38 2023, max compression
+gzip compressed data, was "gravitypy-1.2.3.tar", last modified: Sun Jun 18 20:32:46 2023, max compression
```

## Comparing `gravitypy-1.2.2.tar` & `gravitypy-1.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.2/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.2/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-05 17:34:38.135845 gravitypy-1.2.2/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1480 2023-06-05 17:20:56.000000 gravitypy-1.2.2/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.131845 gravitypy-1.2.2/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.2/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.2/gravitypy/__main__.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/gravitypy/button/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.2/gravitypy/button/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2695 2023-06-05 17:14:48.000000 gravitypy-1.2.2/gravitypy/button/button.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    14366 2023-06-05 17:26:16.000000 gravitypy-1.2.2/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/gravitypy/particle/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.2/gravitypy/particle/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6138 2023-05-27 20:03:20.000000 gravitypy-1.2.2/gravitypy/particle/particle.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.131845 gravitypy-1.2.2/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.135845 gravitypy-1.2.2/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.2/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-05 17:34:38.131845 gravitypy-1.2.2/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      480 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-06-05 17:34:38.000000 gravitypy-1.2.2/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.2/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-05 17:34:38.135845 gravitypy-1.2.2/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-06-05 17:27:53.000000 gravitypy-1.2.2/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 20:40:23.000000 gravitypy-1.2.3/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 20:40:23.000000 gravitypy-1.2.3/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-18 20:32:46.496900 gravitypy-1.2.3/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1480 2023-06-05 17:20:56.000000 gravitypy-1.2.3/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.492900 gravitypy-1.2.3/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 20:40:23.000000 gravitypy-1.2.3/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-12 13:14:06.000000 gravitypy-1.2.3/gravitypy/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/gravitypy/button/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       27 2023-05-12 13:07:34.000000 gravitypy-1.2.3/gravitypy/button/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2695 2023-06-05 17:14:48.000000 gravitypy-1.2.3/gravitypy/button/button.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    14542 2023-06-18 20:29:55.000000 gravitypy-1.2.3/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/gravitypy/particle/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       31 2023-05-12 13:07:49.000000 gravitypy-1.2.3/gravitypy/particle/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6138 2023-05-27 20:03:20.000000 gravitypy-1.2.3/gravitypy/particle/particle.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.492900 gravitypy-1.2.3/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.496900 gravitypy-1.2.3/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 20:40:23.000000 gravitypy-1.2.3/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-18 20:32:46.492900 gravitypy-1.2.3/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      292 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      480 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-06-18 20:32:46.000000 gravitypy-1.2.3/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 20:40:23.000000 gravitypy-1.2.3/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-18 20:32:46.496900 gravitypy-1.2.3/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      959 2023-06-18 20:32:05.000000 gravitypy-1.2.3/setup.py
```

### Comparing `gravitypy-1.2.2/LICENSE` & `gravitypy-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.2/README.md` & `gravitypy-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.2/gravitypy/button/button.py` & `gravitypy-1.2.3/gravitypy/button/button.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.2/gravitypy/main.py` & `gravitypy-1.2.3/gravitypy/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import pygame
 import random
 import math
 import os
 from pygame.locals import *
-from .button.button import Buttons
-from .particle.particle import Particles, QuadTree
+from button.button import Buttons
+from particle.particle import Particles, QuadTree
 
 def main():
     pygame.init()
     pygame.display.set_caption("GravityPy")
     
     current_file = __file__
     current_dir = os.path.dirname(current_file)
     font_file = os.path.join(current_dir, 'resources', 'fonts', 'minecraft_font.ttf')
     font_size = 16
     FONT = pygame.font.Font(font_file, font_size)
 
     WIDTH, HEIGHT = 1200, 700
     SCREEN = pygame.display.set_mode((WIDTH, HEIGHT))
     CLOCK = pygame.time.Clock()
-    G = 1
+    G = 100
     SCALE = 1.0
     PARTICLES = []
     ADDED_RADIUS = 5
     ADDED_MASS = 5
     ADDED_VELOCITY = pygame.Vector2(0, 0)
     NUM_PARTICLES = 250
-    ADDED_COLOR = (255,255,255)
+    ADDED_COLOR = (random.randint(0, 255),random.randint(0, 255),random.randint(0, 255))
     MOUSE_X, MOUSE_Y = pygame.mouse.get_pos()
     
     # Initialize states  
     states = {
         'increase_radius':          False,
         'decrease_radius':          False,
         'increase_mass':            False,
@@ -69,23 +69,23 @@
     }
       
     # Generate random particlesbutton
     for i in range(NUM_PARTICLES):
         if i == 0:
             x = WIDTH // 2
             y = HEIGHT// 2
-            mass = 10000
+            mass = 1000
             radius = random.randint(10, 10)
             PARTICLES.append(Particles(x, y, mass, (189, 255, 20) , radius, pygame.Vector2(0, 0)))
         else:
             x =  i*3
             y = 100 
             mass = int(random.uniform(1, 10))
             radius = int(random.randint(1, 3))
-            PARTICLES.append(Particles(x, y, mass, (255,255,255), radius, pygame.Vector2(2.0, 0)))
+            PARTICLES.append(Particles(x, y, mass, (random.randint(0, 255),random.randint(0, 255),random.randint(0, 255)), radius, pygame.Vector2(2.0, 0)))
 
     running = True
 
     while running:
         for event in pygame.event.get():
             if event.type == pygame.QUIT:
                 running = False
@@ -294,15 +294,15 @@
                     ADDED_COLOR ,
                     ADDED_RADIUS,
                     particle_velocity
                 )
             )
             states['add_particle_put'] = False
             # Change color of the next particle
-            ADDED_COLOR  = (255,255,255)
+            ADDED_COLOR  = (random.randint(0, 255),random.randint(0, 255),random.randint(0, 255))
             NUM_PARTICLES += 1
 
         # Sort in case bigger particles do not cover smaller ones 
         PARTICLES = sorted(PARTICLES, key=lambda x: x.radius, reverse=True)
         
         boundary = pygame.Rect(0, 0, WIDTH, HEIGHT)
         capacity = 4  
@@ -318,7 +318,8 @@
                 particle.update()
                 quadtree.calculate_forces(particle, G)
             particle.draw_scaled(MOUSE_X, MOUSE_Y, SCALE, WIDTH, HEIGHT, SCREEN, FONT)
 
         pygame.display.update()
         CLOCK.tick(60)
     pygame.quit()
+main()
```

### Comparing `gravitypy-1.2.2/gravitypy/particle/particle.py` & `gravitypy-1.2.3/gravitypy/particle/particle.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.2/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.2.3/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.2.2/setup.py` & `gravitypy-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.2.2',
+   version='1.2.3',
    description='GravityPy',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/gravityPy",
    long_description_content_type="text/markdown",
    package_data={'gravitypy': ['*']},
```

