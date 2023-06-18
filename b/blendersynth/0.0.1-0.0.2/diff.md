# Comparing `tmp/blendersynth-0.0.1.tar.gz` & `tmp/blendersynth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendersynth-0.0.1.tar", last modified: Thu Jun 15 11:15:07 2023, max compression
+gzip compressed data, was "blendersynth-0.0.2.tar", last modified: Sun Jun 18 08:47:42 2023, max compression
```

## Comparing `blendersynth-0.0.1.tar` & `blendersynth-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.724432 blendersynth-0.0.1/
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.715882 blendersynth-0.0.1/BlenderSynth.egg-info/
--rw-r--r--   0 ollie      (501) staff       (20)     1787 2023-06-15 11:15:07.000000 blendersynth-0.0.1/BlenderSynth.egg-info/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1476 2023-06-15 11:15:07.000000 blendersynth-0.0.1/BlenderSynth.egg-info/SOURCES.txt
--rw-r--r--   0 ollie      (501) staff       (20)        1 2023-06-15 11:15:07.000000 blendersynth-0.0.1/BlenderSynth.egg-info/dependency_links.txt
--rw-r--r--   0 ollie      (501) staff       (20)       13 2023-06-15 11:15:07.000000 blendersynth-0.0.1/BlenderSynth.egg-info/top_level.txt
--rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.1/LICENSE
--rw-r--r--   0 ollie      (501) staff       (20)     1787 2023-06-15 11:15:07.724254 blendersynth-0.0.1/PKG-INFO
--rw-r--r--   0 ollie      (501) staff       (20)     1512 2023-06-15 11:05:50.000000 blendersynth-0.0.1/README.md
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.716336 blendersynth-0.0.1/blendersynth/
--rw-r--r--   0 ollie      (501) staff       (20)     1225 2023-06-14 21:00:10.000000 blendersynth-0.0.1/blendersynth/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.717279 blendersynth-0.0.1/blendersynth/annotations/
--rw-r--r--   0 ollie      (501) staff       (20)       30 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/annotations/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     1571 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/annotations/bbox.py
--rw-r--r--   0 ollie      (501) staff       (20)     1185 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/annotations/utils.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.719202 blendersynth-0.0.1/blendersynth/blender/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.1/blendersynth/blender/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     8420 2023-06-14 19:52:56.000000 blendersynth-0.0.1/blendersynth/blender/aov.py
--rw-r--r--   0 ollie      (501) staff       (20)     1769 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/blender/camera.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.720374 blendersynth-0.0.1/blendersynth/blender/compositor/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.1/blendersynth/blender/compositor/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     7898 2023-06-14 19:52:56.000000 blendersynth-0.0.1/blendersynth/blender/compositor/compositor.py
--rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/blender/compositor/mask_overlay.py
--rw-r--r--   0 ollie      (501) staff       (20)      876 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/blender/compositor/node_group.py
--rw-r--r--   0 ollie      (501) staff       (20)     5485 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/blender/compositor/shape_overlays.py
--rw-r--r--   0 ollie      (501) staff       (20)     1256 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/blender/light.py
--rw-r--r--   0 ollie      (501) staff       (20)     8181 2023-06-14 16:26:41.000000 blendersynth-0.0.1/blendersynth/blender/mesh.py
--rw-r--r--   0 ollie      (501) staff       (20)      503 2023-06-09 15:21:26.000000 blendersynth-0.0.1/blendersynth/blender/render.py
--rw-r--r--   0 ollie      (501) staff       (20)     1013 2023-06-13 10:28:34.000000 blendersynth-0.0.1/blendersynth/blender/utils.py
--rw-r--r--   0 ollie      (501) staff       (20)     1650 2023-06-14 16:10:45.000000 blendersynth-0.0.1/blendersynth/blender/world.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.721263 blendersynth-0.0.1/blendersynth/file/
--rw-r--r--   0 ollie      (501) staff       (20)       39 2023-06-12 08:58:09.000000 blendersynth-0.0.1/blendersynth/file/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      839 2023-06-14 20:54:24.000000 blendersynth-0.0.1/blendersynth/file/dataset_inputs.py
--rw-r--r--   0 ollie      (501) staff       (20)      159 2023-06-09 15:47:06.000000 blendersynth-0.0.1/blendersynth/file/dataset_outputs.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.722220 blendersynth-0.0.1/blendersynth/run/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.1/blendersynth/run/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.1/blendersynth/run/blender_interface.py
--rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.1/blendersynth/run/blender_threading.py
--rw-r--r--   0 ollie      (501) staff       (20)     2931 2023-06-14 20:49:44.000000 blendersynth-0.0.1/blendersynth/run/run.py
--rw-r--r--   0 ollie      (501) staff       (20)      628 2023-06-14 19:34:31.000000 blendersynth-0.0.1/blendersynth/run_this_script.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.722622 blendersynth-0.0.1/blendersynth/utils/
--rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.1/blendersynth/utils/__init__.py
-drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-15 11:15:07.723852 blendersynth-0.0.1/blendersynth/utils/blender_setup/
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.1/blendersynth/utils/blender_setup/__init__.py
--rw-r--r--   0 ollie      (501) staff       (20)     3885 2023-06-14 21:00:10.000000 blendersynth-0.0.1/blendersynth/utils/blender_setup/blender_locator.py
--rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.1/blendersynth/utils/blender_setup/blender_python_path.py
--rw-r--r--   0 ollie      (501) staff       (20)     2356 2023-06-15 11:14:18.000000 blendersynth-0.0.1/blendersynth/utils/blender_setup/check_blender_install.py
--rw-r--r--   0 ollie      (501) staff       (20)     3359 2023-06-13 09:36:59.000000 blendersynth-0.0.1/blendersynth/utils/node_arranger.py
--rw-r--r--   0 ollie      (501) staff       (20)      392 2023-06-15 11:15:00.000000 blendersynth-0.0.1/pyproject.toml
--rw-r--r--   0 ollie      (501) staff       (20)       38 2023-06-15 11:15:07.724507 blendersynth-0.0.1/setup.cfg
--rw-r--r--   0 ollie      (501) staff       (20)      173 2023-06-15 11:15:00.000000 blendersynth-0.0.1/setup.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.862711 blendersynth-0.0.2/
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.853865 blendersynth-0.0.2/BlenderSynth.egg-info/
+-rw-r--r--   0 ollie      (501) staff       (20)     2003 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1476 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/SOURCES.txt
+-rw-r--r--   0 ollie      (501) staff       (20)        1 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/dependency_links.txt
+-rw-r--r--   0 ollie      (501) staff       (20)       13 2023-06-18 08:47:42.000000 blendersynth-0.0.2/BlenderSynth.egg-info/top_level.txt
+-rw-r--r--   0 ollie      (501) staff       (20)     1068 2023-06-13 13:46:17.000000 blendersynth-0.0.2/LICENSE
+-rw-r--r--   0 ollie      (501) staff       (20)     2003 2023-06-18 08:47:42.862484 blendersynth-0.0.2/PKG-INFO
+-rw-r--r--   0 ollie      (501) staff       (20)     1728 2023-06-15 17:26:03.000000 blendersynth-0.0.2/README.md
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.854310 blendersynth-0.0.2/blendersynth/
+-rw-r--r--   0 ollie      (501) staff       (20)     1365 2023-06-15 17:26:03.000000 blendersynth-0.0.2/blendersynth/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.855229 blendersynth-0.0.2/blendersynth/annotations/
+-rw-r--r--   0 ollie      (501) staff       (20)       30 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/annotations/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1571 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/annotations/bbox.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1185 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/annotations/utils.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.857219 blendersynth-0.0.2/blendersynth/blender/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/blender/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     8420 2023-06-14 19:52:56.000000 blendersynth-0.0.2/blendersynth/blender/aov.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1769 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/camera.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.858461 blendersynth-0.0.2/blendersynth/blender/compositor/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/blender/compositor/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7898 2023-06-14 19:52:56.000000 blendersynth-0.0.2/blendersynth/blender/compositor/compositor.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1950 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/compositor/mask_overlay.py
+-rw-r--r--   0 ollie      (501) staff       (20)      876 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/compositor/node_group.py
+-rw-r--r--   0 ollie      (501) staff       (20)     5485 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/compositor/shape_overlays.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1256 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/blender/light.py
+-rw-r--r--   0 ollie      (501) staff       (20)    12158 2023-06-18 08:45:26.000000 blendersynth-0.0.2/blendersynth/blender/mesh.py
+-rw-r--r--   0 ollie      (501) staff       (20)      503 2023-06-09 15:21:26.000000 blendersynth-0.0.2/blendersynth/blender/render.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1475 2023-06-16 13:06:27.000000 blendersynth-0.0.2/blendersynth/blender/utils.py
+-rw-r--r--   0 ollie      (501) staff       (20)     1755 2023-06-16 17:58:30.000000 blendersynth-0.0.2/blendersynth/blender/world.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.859417 blendersynth-0.0.2/blendersynth/file/
+-rw-r--r--   0 ollie      (501) staff       (20)       39 2023-06-12 08:58:09.000000 blendersynth-0.0.2/blendersynth/file/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      839 2023-06-14 20:54:24.000000 blendersynth-0.0.2/blendersynth/file/dataset_inputs.py
+-rw-r--r--   0 ollie      (501) staff       (20)      159 2023-06-09 15:47:06.000000 blendersynth-0.0.2/blendersynth/file/dataset_outputs.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.860494 blendersynth-0.0.2/blendersynth/run/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/run/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)      113 2023-06-09 16:19:31.000000 blendersynth-0.0.2/blendersynth/run/blender_interface.py
+-rw-r--r--   0 ollie      (501) staff       (20)     7768 2023-06-14 20:52:35.000000 blendersynth-0.0.2/blendersynth/run/blender_threading.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2931 2023-06-14 20:49:44.000000 blendersynth-0.0.2/blendersynth/run/run.py
+-rw-r--r--   0 ollie      (501) staff       (20)      628 2023-06-14 19:34:31.000000 blendersynth-0.0.2/blendersynth/run_this_script.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.860878 blendersynth-0.0.2/blendersynth/utils/
+-rw-r--r--   0 ollie      (501) staff       (20)        0 2023-06-13 11:44:10.000000 blendersynth-0.0.2/blendersynth/utils/__init__.py
+drwxr-xr-x   0 ollie      (501) staff       (20)        0 2023-06-18 08:47:42.861957 blendersynth-0.0.2/blendersynth/utils/blender_setup/
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-14 18:07:59.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/__init__.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3885 2023-06-14 21:00:10.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/blender_locator.py
+-rw-r--r--   0 ollie      (501) staff       (20)       56 2023-06-09 20:07:30.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/blender_python_path.py
+-rw-r--r--   0 ollie      (501) staff       (20)     2741 2023-06-15 17:26:03.000000 blendersynth-0.0.2/blendersynth/utils/blender_setup/check_blender_install.py
+-rw-r--r--   0 ollie      (501) staff       (20)     3359 2023-06-13 09:36:59.000000 blendersynth-0.0.2/blendersynth/utils/node_arranger.py
+-rw-r--r--   0 ollie      (501) staff       (20)      392 2023-06-18 08:47:32.000000 blendersynth-0.0.2/pyproject.toml
+-rw-r--r--   0 ollie      (501) staff       (20)       38 2023-06-18 08:47:42.862777 blendersynth-0.0.2/setup.cfg
+-rw-r--r--   0 ollie      (501) staff       (20)      173 2023-06-18 08:47:32.000000 blendersynth-0.0.2/setup.py
```

### Comparing `blendersynth-0.0.1/BlenderSynth.egg-info/PKG-INFO` & `blendersynth-0.0.2/BlenderSynth.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.1
+Version: 0.0.2
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
@@ -26,19 +26,27 @@
 
 2) Install blendersynth
 
 If Blender is not in your PATH, you will need to specify the path to your Blender installation on install.
 
 From pip:
 
-```pip install blendersynth```
+```
+pip install blendersynth
+python -c "import blendersynth"
+```
 
 Or from local clone:
 
-`python setup.py install`
+```
+git clone https://github.com/OllieBoyne/BlenderSynth
+cd BlenderSynth
+python setup.py install
+python -c "import blendersynth" --local
+```
 
 ## Quickstart
 
 For a quick overview of creating a render: `examples/quickstart.py`
 
 For an overview of creating a dataset: `examples/dataset_creation`
 
@@ -46,12 +54,12 @@
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
 Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Troubleshooting
 
-If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`.
+If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
 
 ## Benchmarking
 
 ![](docs/benchmark-1.png)
```

### Comparing `blendersynth-0.0.1/BlenderSynth.egg-info/SOURCES.txt` & `blendersynth-0.0.2/BlenderSynth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/LICENSE` & `blendersynth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/PKG-INFO` & `blendersynth-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendersynth
-Version: 0.0.1
+Version: 0.0.2
 Summary: Synthetic Rendering for Blender
 Author-email: Ollie Boyne <ollieboyne@gmail.com>
 Project-URL: Homepage, https://github.com/OllieBoyne/BlenderSynth
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BlenderSynth
@@ -26,19 +26,27 @@
 
 2) Install blendersynth
 
 If Blender is not in your PATH, you will need to specify the path to your Blender installation on install.
 
 From pip:
 
-```pip install blendersynth```
+```
+pip install blendersynth
+python -c "import blendersynth"
+```
 
 Or from local clone:
 
-`python setup.py install`
+```
+git clone https://github.com/OllieBoyne/BlenderSynth
+cd BlenderSynth
+python setup.py install
+python -c "import blendersynth" --local
+```
 
 ## Quickstart
 
 For a quick overview of creating a render: `examples/quickstart.py`
 
 For an overview of creating a dataset: `examples/dataset_creation`
 
@@ -46,12 +54,12 @@
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
 Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Troubleshooting
 
-If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`.
+If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
 
 ## Benchmarking
 
 ![](docs/benchmark-1.png)
```

### Comparing `blendersynth-0.0.1/README.md` & `blendersynth-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,27 @@
 
 2) Install blendersynth
 
 If Blender is not in your PATH, you will need to specify the path to your Blender installation on install.
 
 From pip:
 
-```pip install blendersynth```
+```
+pip install blendersynth
+python -c "import blendersynth"
+```
 
 Or from local clone:
 
-`python setup.py install`
+```
+git clone https://github.com/OllieBoyne/BlenderSynth
+cd BlenderSynth
+python setup.py install
+python -c "import blendersynth" --local
+```
 
 ## Quickstart
 
 For a quick overview of creating a render: `examples/quickstart.py`
 
 For an overview of creating a dataset: `examples/dataset_creation`
 
@@ -37,12 +45,12 @@
 
 This project is currently in Beta. Please let me know what new features you would like, or feel free to make a pull request!
 
 Note that `bsyn` imports all `bpy` functionality, so you can call any `bpy` function as if you would normally.
 
 ## Troubleshooting
 
-If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`.
+If any issues with the Blender scripts not having the correct modules, try `bsyn.fix_blender_modules()`, or to completely reconfigure Blender, `bsyn.fix_blender_install()`. If installing from local clone, use `local=True` argument to both.
 
 ## Benchmarking
 
 ![](docs/benchmark-1.png)
```

### Comparing `blendersynth-0.0.1/blendersynth/__init__.py` & `blendersynth-0.0.2/blendersynth/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # First, make sure Blender has been set up properly
+import sys
 from .utils.blender_setup import check_blender_install
-check_blender_install() # check install here
+check_blender_install(blendersynth_from_local='--local' in sys.argv) # check install here
 
-def fix_blender_install():
-	check_blender_install(force_all=True)
+def fix_blender_install(local=False):
+	check_blender_install(force_all=True, blendersynth_from_local=local)
 
-def fix_blender_modules():
-	check_blender_install(force_install_dependencies=True)
+def fix_blender_modules(local=False):
+	check_blender_install(force_install_dependencies=True, blendersynth_from_local=local)
 
 from .run_this_script import run_this_script
 
 import sys
 from .utils.blender_setup.blender_locator import get_blender_path
 
 if get_blender_path() == sys.argv[0]:  # if blender is running this script
```

### Comparing `blendersynth-0.0.1/blendersynth/annotations/bbox.py` & `blendersynth-0.0.2/blendersynth/annotations/bbox.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/annotations/utils.py` & `blendersynth-0.0.2/blendersynth/annotations/utils.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/aov.py` & `blendersynth-0.0.2/blendersynth/blender/aov.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/camera.py` & `blendersynth-0.0.2/blendersynth/blender/camera.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/compositor/compositor.py` & `blendersynth-0.0.2/blendersynth/blender/compositor/compositor.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/compositor/mask_overlay.py` & `blendersynth-0.0.2/blendersynth/blender/compositor/mask_overlay.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/compositor/node_group.py` & `blendersynth-0.0.2/blendersynth/blender/compositor/node_group.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/compositor/shape_overlays.py` & `blendersynth-0.0.2/blendersynth/blender/compositor/shape_overlays.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/light.py` & `blendersynth-0.0.2/blendersynth/blender/light.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/blender/world.py` & `blendersynth-0.0.2/blendersynth/blender/world.py`

 * *Files 20% similar despite different names*

```diff
@@ -60,8 +60,11 @@
 		"""Set HDRI from image path"""
 		self.setup_hdri()
 		self.world_nodes['Environment Texture'].image = bpy.data.images.load(pth)
 
 	def set_hdri_intensity(self, intensity = 1.):
 		self.world_nodes["Background"].inputs[1].default_value = intensity  # HDRI lighting
 
+	def set_transparent(self, transparent=True):
+		bpy.context.scene.render.film_transparent = transparent
+
 world = World()
```

### Comparing `blendersynth-0.0.1/blendersynth/file/dataset_inputs.py` & `blendersynth-0.0.2/blendersynth/file/dataset_inputs.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/run/blender_threading.py` & `blendersynth-0.0.2/blendersynth/run/blender_threading.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/run/run.py` & `blendersynth-0.0.2/blendersynth/run/run.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/run_this_script.py` & `blendersynth-0.0.2/blendersynth/run_this_script.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/utils/blender_setup/blender_locator.py` & `blendersynth-0.0.2/blendersynth/utils/blender_setup/blender_locator.py`

 * *Files identical despite different names*

### Comparing `blendersynth-0.0.1/blendersynth/utils/blender_setup/check_blender_install.py` & `blendersynth-0.0.2/blendersynth/utils/blender_setup/check_blender_install.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 		subprocess.check_call(commands)
 	except subprocess.CalledProcessError as e:
 		raise Exception(f"Could not install {module_name} via pip. Error: {e}")
 
 def check_blender_install(force_all=False,
 						  force_find_blender=False,
 						  force_find_blender_python=False,
-						  force_install_dependencies=False):
+						  force_install_dependencies=False,
+						  blendersynth_from_local=False):
 	"""Check if Blender is installed correctly and has all necessary packages.
 	If not, run first time setup.
 
 	On first time setup, will create a file, config.ini, in the user's config,
 	containing the necessary info.
 
 	Force: if True, will run first time setup (overwriting any existing config.ini)
@@ -57,10 +58,19 @@
 	if not read_from_config('DEPENDENCIES_INSTALLED') == 'True':
 		# check if blender's python has all necessary packages
 		for dependency in dependencies:
 			if not check_module(python_path, dependency):
 				install_module(python_path, dependency)
 
 		# Install blendersynth package to blender's python
-		install_module(python_path, 'blendersynth', upgrade=True)
+		if blendersynth_from_local:
+			# Install from local setup.py
+			setup_py_loc = os.path.join(os.path.dirname(__file__), '..', '..', 'setup.py')
+			if not os.path.isfile('setup.py'):
+				raise Exception(f"Could not find setup.py at {setup_py_loc}.")
+			subprocess.check_call([python_path, 'setup.py', 'install'])
+
+		else:
+			# Install from pypi
+			install_module(python_path, 'blendersynth', upgrade=True)
 
 		write_to_config('DEPENDENCIES_INSTALLED', 'True')
```

### Comparing `blendersynth-0.0.1/blendersynth/utils/node_arranger.py` & `blendersynth-0.0.2/blendersynth/utils/node_arranger.py`

 * *Files identical despite different names*

