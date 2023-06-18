# Comparing `tmp/mizue-0.2.1.tar.gz` & `tmp/mizue-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.2.1.tar", last modified: Sun Jun 18 01:30:54 2023, max compression
+gzip compressed data, was "mizue-0.2.3.tar", last modified: Sun Jun 18 14:16:06 2023, max compression
```

## Comparing `mizue-0.2.1.tar` & `mizue-0.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.723108 mizue-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 01:30:44.000000 mizue-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 01:30:54.723108 mizue-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 01:30:44.000000 mizue-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.723108 mizue-0.2.1/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.723108 mizue-0.2.1/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:30:54.723108 mizue-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-18 01:30:44.000000 mizue-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 14:15:50.000000 mizue-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 14:16:06.277121 mizue-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 14:15:50.000000 mizue-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.273121 mizue-0.2.3/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.273121 mizue-0.2.3/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:16:06.277121 mizue-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 14:16:05.000000 mizue-0.2.3/setup.py
```

### Comparing `mizue-0.2.1/LICENSE` & `mizue-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/PKG-INFO` & `mizue-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.1
+Version: 0.2.3
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.1/README.md` & `mizue-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/file/fileutils.py` & `mizue-0.2.3/mizue/file/fileutils.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/network/downloader/data/colors.json` & `mizue-0.2.3/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/network/downloader/download_event.py` & `mizue-0.2.3/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/network/downloader/downloader.py` & `mizue-0.2.3/mizue/network/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/network/downloader/downloader_tool.py` & `mizue-0.2.3/mizue/network/downloader/downloader_tool.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/printer/grid/border_character_codes.py` & `mizue-0.2.3/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/printer/grid/column.py` & `mizue-0.2.3/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/printer/grid/grid.py` & `mizue-0.2.3/mizue/printer/grid/grid.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/printer/printer.py` & `mizue-0.2.3/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/progress/progress.py` & `mizue-0.2.3/mizue/progress/progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/progress/progress_renderer_args.py` & `mizue-0.2.3/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/progress/spinner.py` & `mizue-0.2.3/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/util/event_listener.py` & `mizue-0.2.3/mizue/util/event_listener.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/util/signal_handler.py` & `mizue-0.2.3/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue/util/utility.py` & `mizue-0.2.3/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/mizue.egg-info/PKG-INFO` & `mizue-0.2.3/mizue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.1
+Version: 0.2.3
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.1/mizue.egg-info/SOURCES.txt` & `mizue-0.2.3/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.2.1/setup.py` & `mizue-0.2.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.2.1",
+    version="0.2.3",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3"
     ],
     packages=find_packages(),
     package_data={
         "mizue.network.downloader": ["data/*.json"],
     },
+    setup_requires=["wheel"],
     install_requires=["wcwidth"],
     include_package_data=True
 )
```

