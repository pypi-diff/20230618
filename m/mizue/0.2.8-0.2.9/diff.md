# Comparing `tmp/mizue-0.2.8.tar.gz` & `tmp/mizue-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.2.8.tar", last modified: Sun Jun 18 18:01:35 2023, max compression
+gzip compressed data, was "mizue-0.2.9.tar", last modified: Sun Jun 18 18:09:46 2023, max compression
```

## Comparing `mizue-0.2.8.tar` & `mizue-0.2.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 18:01:20.000000 mizue-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 18:01:35.783875 mizue-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 18:01:20.000000 mizue-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.779875 mizue-0.2.8/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.779875 mizue-0.2.8/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.779875 mizue-0.2.8/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/progress/colorful_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.783875 mizue-0.2.8/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 18:01:20.000000 mizue-0.2.8/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:01:35.779875 mizue-0.2.8/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 18:01:35.000000 mizue-0.2.8/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-18 18:01:35.000000 mizue-0.2.8/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:01:35.000000 mizue-0.2.8/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 18:01:35.000000 mizue-0.2.8/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 18:01:35.000000 mizue-0.2.8/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:01:35.783875 mizue-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 18:01:35.000000 mizue-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.998993 mizue-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 18:09:26.000000 mizue-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 18:09:45.994994 mizue-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 18:09:26.000000 mizue-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/colorful_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 18:09:26.000000 mizue-0.2.9/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:09:45.994994 mizue-0.2.9/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 18:09:45.000000 mizue-0.2.9/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 18:09:45.998993 mizue-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 18:09:45.000000 mizue-0.2.9/setup.py
```

### Comparing `mizue-0.2.8/LICENSE` & `mizue-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/PKG-INFO` & `mizue-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.8/README.md` & `mizue-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/file/fileutils.py` & `mizue-0.2.9/mizue/file/fileutils.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/network/downloader/data/colors.json` & `mizue-0.2.9/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/network/downloader/download_event.py` & `mizue-0.2.9/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/network/downloader/downloader.py` & `mizue-0.2.9/mizue/network/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/network/downloader/downloader_tool.py` & `mizue-0.2.9/mizue/network/downloader/downloader_tool.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/printer/grid/border_character_codes.py` & `mizue-0.2.9/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/printer/grid/column.py` & `mizue-0.2.9/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/printer/grid/grid.py` & `mizue-0.2.9/mizue/printer/grid/grid.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/printer/printer.py` & `mizue-0.2.9/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/progress/colorful_progress.py` & `mizue-0.2.9/mizue/progress/colorful_progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/progress/progress.py` & `mizue-0.2.9/mizue/progress/progress.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/progress/progress_renderer_args.py` & `mizue-0.2.9/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/progress/spinner.py` & `mizue-0.2.9/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/util/event_listener.py` & `mizue-0.2.9/mizue/util/event_listener.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/util/signal_handler.py` & `mizue-0.2.9/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue/util/utility.py` & `mizue-0.2.9/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/mizue.egg-info/PKG-INFO` & `mizue-0.2.9/mizue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.8
+Version: 0.2.9
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.8/mizue.egg-info/SOURCES.txt` & `mizue-0.2.9/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.2.8/setup.py` & `mizue-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.2.8",
+    version="0.2.9",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

