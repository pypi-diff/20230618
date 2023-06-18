# Comparing `tmp/psbs-0.1.0.tar.gz` & `tmp/psbs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.1.0.tar", last modified: Wed Jun 14 19:41:29 2023, max compression
+gzip compressed data, was "psbs-0.1.1.tar", last modified: Sun Jun 18 21:00:41 2023, max compression
```

## Comparing `psbs-0.1.0.tar` & `psbs-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.641049 psbs-0.1.0/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.1.0/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-14 19:41:29.641291 psbs-0.1.0/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     4874 2023-06-14 19:38:32.000000 psbs-0.1.0/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.634924 psbs-0.1.0/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.1.0/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.1.0/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.1.0/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.1.0/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      545 2023-06-14 19:27:02.000000 psbs-0.1.0/psbs/extension.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      125 2023-06-14 19:20:28.000000 psbs-0.1.0/psbs/extensionloader.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.640067 psbs-0.1.0/psbs/extensions/
--rw-r--r--   0 jcmiller   (501) staff       (20)      225 2023-06-14 16:33:22.000000 psbs-0.1.0/psbs/extensions/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3101 2023-06-14 19:25:25.000000 psbs-0.1.0/psbs/extensions/images.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.1.0/psbs/gister.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     4117 2023-06-14 19:20:01.000000 psbs-0.1.0/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-06-14 10:55:45.000000 psbs-0.1.0/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1573 2023-06-07 22:59:45.000000 psbs-0.1.0/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1549 2023-06-14 19:36:41.000000 psbs-0.1.0/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.1.0/psbs/templatebuilder.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.1.0/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.1.0/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-14 19:41:29.638650 psbs-0.1.0/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      498 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       34 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-14 19:41:29.000000 psbs-0.1.0/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-14 19:41:29.642054 psbs-0.1.0/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1239 2023-06-14 19:39:12.000000 psbs-0.1.0/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-18 21:00:41.210228 psbs-0.1.1/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.1.1/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-18 21:00:41.210349 psbs-0.1.1/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     4874 2023-06-14 19:38:32.000000 psbs-0.1.1/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-18 21:00:41.207564 psbs-0.1.1/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.1.1/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.1.1/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.1.1/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.1.1/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1146 2023-06-18 20:24:47.000000 psbs-0.1.1/psbs/extension.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-18 21:00:41.209984 psbs-0.1.1/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.1.1/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3025 2023-06-18 20:24:47.000000 psbs-0.1.1/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.1.1/psbs/gister.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     4116 2023-06-18 19:37:14.000000 psbs-0.1.1/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-06-14 10:55:45.000000 psbs-0.1.1/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1573 2023-06-07 22:59:45.000000 psbs-0.1.1/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1548 2023-06-18 20:02:25.000000 psbs-0.1.1/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.1.1/psbs/templatebuilder.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.1.1/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.1.1/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-18 21:00:41.209473 psbs-0.1.1/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-18 21:00:41.000000 psbs-0.1.1/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      474 2023-06-18 21:00:41.000000 psbs-0.1.1/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-18 21:00:41.000000 psbs-0.1.1/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-18 21:00:41.000000 psbs-0.1.1/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       34 2023-06-18 21:00:41.000000 psbs-0.1.1/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-18 21:00:41.000000 psbs-0.1.1/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-18 21:00:41.210747 psbs-0.1.1/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1239 2023-06-18 20:58:05.000000 psbs-0.1.1/setup.py
```

### Comparing `psbs-0.1.0/LICENSE` & `psbs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/PKG-INFO` & `psbs-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.1.0
+Version: 0.1.1
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.1.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.1.0/README.md` & `psbs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/example.txt` & `psbs-0.1.1/psbs/example.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/extensions/images.py` & `psbs-0.1.1/psbs/extensions/images.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from textwrap import wrap
 
-import jinja2
 from PIL import Image
 from psbs.extension import Extension
 
 
 class Images(Extension):
     def __init__(self, config):
         super().__init__(config)
@@ -52,26 +51,24 @@
         file,
         x=0,
         y=0,
         width=None,
         height=None,
     ):
         if self.config["max_colors"] > 36:
-            raise jinja2.exceptions.TemplateError(
+            raise self.ExtensionError(
                 "Image helper function doesn't support more than 36 colors"
             )
         if file in self.loaded_images:
             image = self.loaded_images[file]
         else:
             try:
                 image = Image.open(file, "r")
             except IOError as err:
-                raise jinja2.exceptions.TemplateError(
-                    f"Unable to read image file\n  {err}"
-                )
+                raise self.ExtensionError(f"Unable to read image file\n  {err}")
             self.loaded_images[file] = image
         # Crop image if needed
         if width:
             right = x + width
         else:
             right = image.size[0]
         if height:
```

### Comparing `psbs-0.1.0/psbs/gister.py` & `psbs-0.1.1/psbs/gister.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/project.py` & `psbs-0.1.1/psbs/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .gister import Gister
 from .config import Config
 from .psparser import split_ps, get_engine
 from .templatebuilder import make_template
 from .utils import read_file, write_file, write_yaml, make_dir, run_in_browser
 from .template import render_template
-from .extensionloader import get_extensions
+from .extension import Extension
 
 
 class PSBSProject:
     def __init__(self, config_filename="config.yaml"):
         self.config = Config(config_filename)
 
     def build(self):
@@ -87,15 +87,15 @@
 
         config_dict = {
             "gist_id": gist_id,
             "engine": engine,
             "template": "main.pss",
         }
 
-        for extension in get_extensions():
+        for extension in Extension.get_extensions():
             if extension.get_config():
                 config_dict[extension.__name__] = extension.get_config()
 
         print("Building directory structure")
         make_dir(project_name)
         try:
             make_dir(path.join(project_name, "src"))
```

### Comparing `psbs-0.1.0/psbs/psbs.py` & `psbs-0.1.1/psbs/psbs.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/psparser.py` & `psbs-0.1.1/psbs/psparser.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/template.py` & `psbs-0.1.1/psbs/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import path
 import traceback
 
 import jinja2
-from .extensionloader import get_extensions
+from .extension import Extension
 
 
 def render_template(filename, config):
     directory = path.dirname(filename)
     file = path.basename(filename)
     jinja_env = jinja2.Environment(
         loader=jinja2.FileSystemLoader(directory),
@@ -14,15 +14,15 @@
         block_start_string="(%",
         block_end_string="%)",
         variable_start_string="((",
         variable_end_string="))",
         comment_start_string="(#",
         comment_end_string="#)",
     )
-    extensions = get_extensions()
+    extensions = Extension.get_extensions()
     for extension in extensions:
         if extension.__name__ not in config:
             config[extension.__name__] = {}
         ext_object = extension(config[extension.__name__])
         for func_name, function in ext_object.methods.items():
             jinja_env.globals[func_name] = function
```

### Comparing `psbs-0.1.0/psbs/templatebuilder.py` & `psbs-0.1.1/psbs/templatebuilder.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/token.py` & `psbs-0.1.1/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs/utils.py` & `psbs-0.1.1/psbs/utils.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.0/psbs.egg-info/PKG-INFO` & `psbs-0.1.1/psbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.1.0
+Version: 0.1.1
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.1.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.1.0/setup.py` & `psbs-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='psbs',
-    version='0.1.0',
+    version='0.1.1',
     python_requires='>=3.8',
     description='PuzzleScript Build System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='J.C. Miller',
     author_email='johncoreymiller@gmail.com',
     url='https://github.com/jcmiller11/PSBS',
-    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.0.tar.gz',
+    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.1.tar.gz',
     license='MIT',
     packages=find_packages(),
     package_data={'': ['example.txt']},
     include_package_data=True,
     install_requires=[
         'jinja2',
         'pyyaml',
```

