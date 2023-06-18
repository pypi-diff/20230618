# Comparing `tmp/neophaser-0.2.0.tar.gz` & `tmp/neophaser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neophaser-0.2.0.tar", last modified: Sat Jun 17 04:58:58 2023, max compression
+gzip compressed data, was "neophaser-0.2.1.tar", last modified: Sun Jun 18 01:04:34 2023, max compression
```

## Comparing `neophaser-0.2.0.tar` & `neophaser-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.681628 neophaser-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-17 04:58:50.000000 neophaser-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      889 2023-06-17 04:58:58.681628 neophaser-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-17 04:58:50.000000 neophaser-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.679628 neophaser-0.2.0/neophaser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.680628 neophaser-0.2.0/neophaser/assets/
--rw-rw-rw-   0 root         (0) root         (0)    67646 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/assets/icon.ico
--rw-rw-rw-   0 root         (0) root         (0)   208914 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/assets/icon.png
--rw-rw-rw-   0 root         (0) root         (0)     3071 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/board.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)    15208 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/gui.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2683 2023-06-17 04:58:50.000000 neophaser-0.2.0/neophaser/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:58:58.680628 neophaser-0.2.0/neophaser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      889 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 04:58:58.000000 neophaser-0.2.0/neophaser.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-17 04:58:50.000000 neophaser-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 04:58:58.681628 neophaser-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 01:04:34.714653 neophaser-0.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-18 01:04:27.000000 neophaser-0.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-18 01:04:34.714653 neophaser-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-06-18 01:04:27.000000 neophaser-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 01:04:34.712653 neophaser-0.2.1/neophaser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 01:04:34.713653 neophaser-0.2.1/neophaser/assets/
+-rw-rw-rw-   0 root         (0) root         (0)    67646 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/assets/icon.ico
+-rw-rw-rw-   0 root         (0) root         (0)   208914 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/assets/icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     3071 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/board.py
+-rw-rw-rw-   0 root         (0) root         (0)     4172 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15214 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2683 2023-06-18 01:04:27.000000 neophaser-0.2.1/neophaser/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 01:04:34.713653 neophaser-0.2.1/neophaser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-18 01:04:34.000000 neophaser-0.2.1/neophaser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-18 01:04:34.000000 neophaser-0.2.1/neophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 01:04:34.000000 neophaser-0.2.1/neophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-18 01:04:34.000000 neophaser-0.2.1/neophaser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-18 01:04:34.000000 neophaser-0.2.1/neophaser.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-18 01:04:27.000000 neophaser-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 01:04:34.714653 neophaser-0.2.1/setup.cfg
```

### Comparing `neophaser-0.2.0/PKG-INFO` & `neophaser-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.2.0
+Version: 0.2.1
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.2.0/neophaser/assets/icon.ico` & `neophaser-0.2.1/neophaser/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `neophaser-0.2.0/neophaser/assets/icon.png` & `neophaser-0.2.1/neophaser/assets/icon.png`

 * *Files identical despite different names*

### Comparing `neophaser-0.2.0/neophaser/board.py` & `neophaser-0.2.1/neophaser/board.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.2.0/neophaser/controllers.py` & `neophaser-0.2.1/neophaser/controllers.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 	Chorus,
 	Delay,
 	HighShelfFilter,
 	LowShelfFilter,
 	Phaser,
 	Reverb,
 	Resample,
-
-	AudioUnitPlugin,
-	Plugin,
-	VST3Plugin,
 )
 
 from neophaser.options import EffectController, EffectOption, OptionType
 
 class ChorusController(EffectController):
 	def __init__(self):
 		self.effect = Chorus()
@@ -96,16 +92,20 @@
 		self.loaded = False
 	
 	def _apply_options(self):
 		pass
 
 	def load_plugin(self, path):
 		if path.endswith(".component"):
+			from pedalboard import AudioUnitPlugin
+
 			self.effect = AudioUnitPlugin(path)
 		else:
+			from pedalboard import VST3Plugin
+
 			self.effect = VST3Plugin(path)
 		
 		self.loaded = True
 	
 	def open_plugin_ui(self):
 		self.effect.show_editor()
```

### Comparing `neophaser-0.2.0/neophaser/gui.py` & `neophaser-0.2.1/neophaser/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 				open_plugin_ui_button.clicked.connect(effect.open_plugin_ui)
 				render_button = QPushButton("Render")
 				render_button.clicked.connect(self.render.emit)
 
 				self.options_layout.addRow(open_plugin_ui_button)
 				self.options_layout.addRow(render_button)
 			else:
-				plugin_path = "/Library/Audio/Plug-Ins/VST3/"
+				plugin_path = "/Library/Audio/Plug-Ins/Components/"
 				if platform.system() == "Windows":
 					plugin_path = "C:/Program Files/Common Files/VST3/"
 				elif platform.system() == "Linux":
 					plugin_path = "/usr/lib/vst3/"
 
 				load_plugin_from_path = lambda: (
 					effect.load_plugin(QFileDialog.getOpenFileName(self, "Open Plugin", plugin_path, "Audio Plugin (*.dll *.vst3 *.component *.so)")[0]),
```

### Comparing `neophaser-0.2.0/neophaser/options.py` & `neophaser-0.2.1/neophaser/options.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.2.0/neophaser/utils.py` & `neophaser-0.2.1/neophaser/utils.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.2.0/neophaser/visual.py` & `neophaser-0.2.1/neophaser/visual.py`

 * *Files identical despite different names*

### Comparing `neophaser-0.2.0/neophaser.egg-info/PKG-INFO` & `neophaser-0.2.1/neophaser.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neophaser
-Version: 0.2.0
+Version: 0.2.1
 Summary: NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video.
 Author-email: 8o-COLLECTIVE <ops@8oc.org>
 Project-URL: homepage, https://neophaser.library.8oc.org
 Project-URL: repository, https://gitlab.com/8o-collective/neophaser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neophaser-0.2.0/pyproject.toml` & `neophaser-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "neophaser"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="8o-COLLECTIVE", email="ops@8oc.org" },
 ]
 description = "NEOPHASER; or, audio effects as applied to the retina - an application for applying audio effects to image and video."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

