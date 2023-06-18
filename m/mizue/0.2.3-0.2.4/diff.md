# Comparing `tmp/mizue-0.2.3.tar.gz` & `tmp/mizue-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.2.3.tar", last modified: Sun Jun 18 14:16:06 2023, max compression
+gzip compressed data, was "mizue-0.2.4.tar", last modified: Sun Jun 18 16:49:51 2023, max compression
```

## Comparing `mizue-0.2.3.tar` & `mizue-0.2.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 14:15:50.000000 mizue-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 14:16:06.277121 mizue-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 14:15:50.000000 mizue-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.273121 mizue-0.2.3/mizue/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/file/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/file/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/network/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/network/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/network/downloader/data/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/download_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/download_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/downloader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/network/downloader/progress_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/printer/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/printer/grid/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/border_character_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/border_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/cell_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/column_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/grid/row_border_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/printer/terminal_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/progress_renderer_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/progress/spinner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.277121 mizue-0.2.3/mizue/util/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/signal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 14:15:50.000000 mizue-0.2.3/mizue/util/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 14:16:06.273121 mizue-0.2.3/mizue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 14:16:06.000000 mizue-0.2.3/mizue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 14:16:06.277121 mizue-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 14:16:05.000000 mizue-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 16:49:33.000000 mizue-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 16:49:51.318113 mizue-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 16:49:33.000000 mizue-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.314113 mizue-0.2.4/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/progress/colorful_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 16:49:33.000000 mizue-0.2.4/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 16:49:51.318113 mizue-0.2.4/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 16:49:51.000000 mizue-0.2.4/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-18 16:49:51.000000 mizue-0.2.4/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 16:49:51.000000 mizue-0.2.4/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 16:49:51.000000 mizue-0.2.4/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 16:49:51.000000 mizue-0.2.4/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 16:49:51.318113 mizue-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-18 16:49:49.000000 mizue-0.2.4/setup.py
```

### Comparing `mizue-0.2.3/LICENSE` & `mizue-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/PKG-INFO` & `mizue-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.3/README.md` & `mizue-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/file/fileutils.py` & `mizue-0.2.4/mizue/file/fileutils.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/network/downloader/data/colors.json` & `mizue-0.2.4/mizue/network/downloader/data/colors.json`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/network/downloader/download_event.py` & `mizue-0.2.4/mizue/network/downloader/download_event.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/network/downloader/downloader.py` & `mizue-0.2.4/mizue/network/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/network/downloader/downloader_tool.py` & `mizue-0.2.4/mizue/network/downloader/downloader_tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from dataclasses import dataclass
 
 from mizue.file import FileUtils
 from mizue.network.downloader import DownloadStartEvent, ProgressEventArgs, DownloadCompleteEvent, Downloader, \
     DownloadEventType, DownloadFailureEvent
 from mizue.printer import Printer
 from mizue.printer.grid import ColumnSettings, Alignment, Grid, BorderStyle, CellRendererArgs
-from mizue.progress import Progress, ProgressBarRendererArgs, SpinnerRendererArgs, LabelRendererArgs, \
-    InfoSeparatorRendererArgs, InfoTextRendererArgs, PercentageRendererArgs
+from mizue.progress import LabelRendererArgs, \
+    InfoSeparatorRendererArgs, InfoTextRendererArgs, ColorfulProgress
 
 
 @dataclass
 class _DownloadReport:
     filename: str
     filesize: int
     url: str
@@ -23,15 +23,15 @@
 class DownloaderTool:
     def __init__(self):
         self._file_color_scheme = {}
         self._report_data: list[_DownloadReport] = []
         self._bulk_download_size = 0
         self._downloaded_count = 0
         self._total_download_count = 0
-        self.progress: Progress | None = None
+        self.progress: ColorfulProgress | None = None
         self._load_color_scheme()
 
     def download(self, url: str, output_path: str):
         """
         Download a file to a specified directory
         :param url: The URL to download
         :param output_path: The output directory
@@ -57,16 +57,16 @@
     def download_bulk(self, urls: list[str] | list[tuple[str, str]], output_path: str | None = None, parallel: int = 4):
         """
         Download a list of files to a specified directory or a list of [url, output_path] tuples.
 
         If the urls parameter is a list of [url, output_path] tuples, every url will be downloaded to its corresponding
         output_path.
 
-        If the urls parameter is a list of urls, every url will be downloaded to the output_path parameter. In this case,
-        the output_path parameter must be specified.
+        If the urls parameter is a list of urls, every url will be downloaded to the output_path parameter.
+        In this case, the output_path parameter must be specified.
         :param urls: A list of urls or a list of [url, output_path] tuples
         :param output_path: The output directory if the urls parameter is a list of urls
         :param parallel: Number of parallel downloads
         :return: None
         """
         if isinstance(urls[0], tuple):
             self.download_tuple(urls, parallel)
@@ -87,15 +87,15 @@
         """
         Download a list of [url, output_path] tuples. Every url will be downloaded to its corresponding output_path.
         :param urls: A list of [url, output_path] tuples
         :param parallel: Number of parallel downloads
         :return: None
         """
 
-        self.progress = Progress(start=0, end=len(urls), value=0)
+        self.progress = ColorfulProgress(start=0, end=len(urls), value=0)
         self._configure_progress()
         self.progress.start()
         self._downloaded_count = 0
         self._total_download_count = len(urls)
         download_dict = {}
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=parallel) as executor:
@@ -108,63 +108,47 @@
                                      lambda event: self._on_bulk_download_complete(event))
                 downloader.add_event(DownloadEventType.FAILED, lambda event: self._on_bulk_download_failed(event))
                 for url, output_path in list(set(urls)):
                     responses.append(executor.submit(downloader.download, url, output_path))
                 for response in concurrent.futures.as_completed(responses):
                     self._downloaded_count += 1
                     self.progress.update_value(self._downloaded_count)
-                    self.progress.set_info(self._get_bulk_progress_info(download_dict))
+                    self.progress.info_text = self._get_bulk_progress_info(download_dict)
                 executor.shutdown(wait=True)
             except KeyboardInterrupt:
                 downloader.close()
                 self.progress.stop()
                 Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
                 executor.shutdown(wait=False, cancel_futures=True)
         self.progress.stop()
         self._print_report()
 
     def _configure_progress(self):
         self.progress.info_separator_renderer = self._info_separator_renderer
         self.progress.info_text_renderer = self._info_text_renderer
         self.progress.label_renderer = self._label_renderer
-        self.progress.percentage_renderer = self._percentage_renderer
-        self.progress.progress_bar_renderer = self._progress_bar_renderer
-        self.progress.spinner_renderer = self._spinner_renderer
         self.progress.label = "Downloading: "
 
     @staticmethod
     def _get_basic_colored_text(text: str, percentage: float):
-        if percentage < 15:
-            return Printer.format_hex(text, '#FF0D0D')
-        elif percentage < 30:
-            return Printer.format_hex(text, '#FF4E11')
-        elif percentage < 45:
-            return Printer.format_hex(text, '#FF8E15')
-        elif percentage < 60:
-            return Printer.format_hex(text, '#FAB733')
-        elif percentage < 75:
-            return Printer.format_hex(text, '#ACB334')
-        elif percentage < 90:
-            return Printer.format_hex(text, '#69B34C')
-        else:
-            return Printer.format_hex(text, '#0EB33B')
+        return ColorfulProgress.get_basic_colored_text(text, percentage)
 
     def _get_bulk_progress_info(self, download_dict: dict):
-        file_progress_text = f'[{self._downloaded_count}/{self._total_download_count}]'
+        file_progress_text = f'⟪{self._downloaded_count}/{self._total_download_count}⟫'
         size_text = FileUtils.get_readable_file_size(sum(download_dict.values()))
-        return f'{file_progress_text} [{size_text}]'
+        return f'{file_progress_text} ⟪{size_text}⟫'
 
     @staticmethod
     def _info_separator_renderer(args: InfoSeparatorRendererArgs):
-        return Printer.format_hex(args.separator, '#FFCC75')
+        return ColorfulProgress.get_basic_colored_text(" | ", args.percentage)
 
     @staticmethod
     def _info_text_renderer(args: InfoTextRendererArgs):
-        return Printer.format_hex(args.text, '#FFCC75')
-        # return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
+        # return Printer.format_hex(args.text, '#FFCC75')
+        return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
 
     @staticmethod
     def _label_renderer(args: LabelRendererArgs):
         if args.percentage < 100:
             return Printer.format_hex(args.label, '#FFCC75')
         return Printer.format_hex('Downloaded: ', '#0EB33B')
 
@@ -177,22 +161,22 @@
         self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
 
     def _on_bulk_download_failed(self, event: DownloadFailureEvent):
         self._report_data.append(_DownloadReport("", 0, event.url))
 
     def _on_bulk_download_progress(self, event: ProgressEventArgs, download_dict: dict):
         download_dict[event.url] = event.downloaded
-        self.progress.set_info(self._get_bulk_progress_info(download_dict))
+        self.progress.info_text = self._get_bulk_progress_info(download_dict)
 
     def _on_download_complete(self, event: DownloadCompleteEvent):
         self.progress.update_value(event.filesize)
         downloaded_info = FileUtils.get_readable_file_size(event.filesize)
         filesize_info = FileUtils.get_readable_file_size(event.filesize)
         info = f'[{downloaded_info}/{filesize_info}]'
-        self.progress.set_info(info)
+        self.progress.info_text = info
         time.sleep(0.5)
         self.progress.stop()
         self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
 
     def _on_download_failure(self, event: DownloadFailureEvent):
         if isinstance(event.exception, KeyboardInterrupt):
             Printer.warning("Download has been cancelled by user.")
@@ -202,26 +186,22 @@
         self._report_data.append(_DownloadReport("", 0, event.url))
 
     def _on_download_progress(self, event: ProgressEventArgs):
         self.progress.update_value(event.downloaded)
         downloaded_info = FileUtils.get_readable_file_size(event.downloaded)
         filesize_info = FileUtils.get_readable_file_size(event.filesize)
         info = f'[{downloaded_info}/{filesize_info}]'
-        self.progress.set_info(info)
+        self.progress.info_text = info
 
     def _on_download_start(self, event: DownloadStartEvent, filepath: list[str]):
-        self.progress = Progress(start=0, end=event.filesize, value=0)
+        self.progress = ColorfulProgress(start=0, end=event.filesize, value=0)
         self._configure_progress()
         self.progress.start()
         filepath.append(event.filepath)
 
-    @staticmethod
-    def _percentage_renderer(args: PercentageRendererArgs):
-        return DownloaderTool._get_basic_colored_text("{:.2f}%".format(args.percentage), args.percentage)
-
     def _print_report(self):
         success_data = [report for report in self._report_data if report.filesize > 0]
         failed_data = [report for report in self._report_data if report.filesize == 0]
         row_index = 1
         success_grid_data = []
         for report in success_data:
             filename, ext = os.path.splitext(report.filename)
@@ -248,18 +228,14 @@
         grid.border_style = BorderStyle.SINGLE
         grid.border_color = '#FFCC75'
         grid.cell_renderer = self._report_grid_cell_renderer
         print(os.linesep)
         grid.print()
 
     @staticmethod
-    def _progress_bar_renderer(args: ProgressBarRendererArgs):
-        return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
-
-    @staticmethod
     def _report_grid_cell_renderer(args: CellRendererArgs):
         if args.cell.endswith("KB"):
             return Printer.format_hex(args.cell, '#00a9ff')
         if args.cell.endswith("MB"):
             return Printer.format_hex(args.cell, '#d2309a')
         if args.is_header:
             return Printer.format_hex(args.cell, '#FFCC75')
@@ -273,11 +249,7 @@
         return Printer.format_hex(args.cell, color)
 
     def _report_grid_file_type_column_cell_renderer(self, args: CellRendererArgs):
         if args.is_header:
             return Printer.format_hex(args.cell, '#FFCC75')
         color = self._file_color_scheme.get(args.cell, '#FFFFFF')
         return Printer.format_hex(args.cell, color)
-
-    @staticmethod
-    def _spinner_renderer(args: SpinnerRendererArgs):
-        return DownloaderTool._get_basic_colored_text(args.spinner, args.percentage)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mizue-0.2.3/mizue/printer/grid/border_character_codes.py` & `mizue-0.2.4/mizue/printer/grid/border_character_codes.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/printer/grid/column.py` & `mizue-0.2.4/mizue/printer/grid/column.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/printer/grid/grid.py` & `mizue-0.2.4/mizue/printer/grid/grid.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/printer/printer.py` & `mizue-0.2.4/mizue/printer/printer.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/progress/progress.py` & `mizue-0.2.4/mizue/progress/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     InfoSeparatorRendererArgs, InfoTextRendererArgs, PercentageRendererArgs
 
 
 class Progress:
     def __init__(self, start: int = 0, end: int = 100, value: int = 0):
         self._active = False
         self._end = end
-        self._info_text = ""
         self._interval = 0.1
         self._spinner = [
             "▹▹▹▹▹",
             "▸▹▹▹▹",
             "▹▸▹▹▹",
             "▹▹▸▹▹",
             "▹▹▹▸▹",
@@ -26,31 +25,30 @@
         self._spinner_index = 0
         self._start = start
         self._thread = None
         self._value = value
         self._width = 10
 
         self.info_separator = " | "
-        self.info_separator_renderer = lambda args: self._info_separator_renderer(
-            args.separator)  # InfoSeparatorRendererArgs
+        self.info_separator_renderer = lambda args: self._info_separator_renderer()  # InfoSeparatorRendererArgs
+
+        self.info_text = ""
+        """Set the info text to be displayed after the progress bar"""
+
         self.info_text_renderer = lambda args: self._info_text_renderer(args.text)  # InfoTextRendererArgs
         self.label = ""
         self.label_renderer = lambda args: args.label  # LabelRendererArgs
         self.percentage_renderer = lambda args: "{:.2f}%".format(args.percentage)  # PercentageRendererArgs
         self.spinner_renderer = lambda args: args.spinner  # SpinnerRendererArgs
         self.progress_bar_renderer = lambda args: self._progress_bar_renderer()  # ProgressBarRendererArgs
 
     def set_end_value(self, end: int) -> None:
         """Update the maximum value of the progress bar"""
         self._end = end
 
-    def set_info(self, info: str) -> None:
-        """Set the info text to be displayed after the progress bar"""
-        self._info_text = info
-
     def set_update_interval(self, interval: float) -> None:
         """Set the update interval of the progress bar"""
         self._interval = interval
 
     def start(self) -> None:
         """Start the progress bar"""
         Utility.hide_cursor()
@@ -107,29 +105,29 @@
         ))
         separator = self.info_separator_renderer(InfoSeparatorRendererArgs(
             separator=self.info_separator,
             value=self._value,
             percentage=percentage_value
         ))
         info_text = self.info_text_renderer(InfoTextRendererArgs(
-            text=self._info_text,
+            text=self.info_text,
             value=self._value,
             percentage=percentage_value
         ))
         progress_text = str.format("{}{} {} {}{}{}", label, bar, spinner_symbol, percentage, separator,
                                    info_text)
         text_length = len(Printer.strip_colors(progress_text))
         if text_length > Utility.get_terminal_width():
             progress_text = str.format("{}{} {} {}{}", label, bar, spinner_symbol, percentage, '')
             if text_length > Utility.get_terminal_width():
                 progress_text = str.format("{}{} {} {}{}", '', bar, spinner_symbol, percentage, '')
         return progress_text
 
-    def _info_separator_renderer(self, info_text: str) -> str:
-        return self.info_separator if len(info_text) > 0 else ""
+    def _info_separator_renderer(self) -> str:
+        return self.info_separator if len(self.info_text) > 0 else ""
 
     @staticmethod
     def _info_text_renderer(info_text: str) -> str:
         return info_text
 
     def _print(self) -> None:
         while self._active:
@@ -138,13 +136,13 @@
             sys.stdout.write(
                 u"\u001b[K")  # Erase from cursor to end of line [http://matthieu.benoit.free.fr/68hc11/vt100.htm]
             sys.stdout.write(
                 u"\u001b[1000D" + progress_text)  # Move terminal cursor 1000 characters left (go to start of line)
             sys.stdout.flush()
             sleep(self._interval)
 
-    def _progress_bar_renderer(self):
+    def _progress_bar_renderer(self) -> str:
         bar_start = "⟪"
         bar_end = "⟫"
         width = self._get_bar_full_width()
         bar = bar_start + "◆" * int(width) + " " * int((self._width - width)) + bar_end
         return bar
```

### Comparing `mizue-0.2.3/mizue/progress/progress_renderer_args.py` & `mizue-0.2.4/mizue/progress/progress_renderer_args.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/progress/spinner.py` & `mizue-0.2.4/mizue/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/util/event_listener.py` & `mizue-0.2.4/mizue/util/event_listener.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/util/signal_handler.py` & `mizue-0.2.4/mizue/util/signal_handler.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue/util/utility.py` & `mizue-0.2.4/mizue/util/utility.py`

 * *Files identical despite different names*

### Comparing `mizue-0.2.3/mizue.egg-info/PKG-INFO` & `mizue-0.2.4/mizue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mizue
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package for various utilities
 Author: Hoshilily
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mizue-0.2.3/mizue.egg-info/SOURCES.txt` & `mizue-0.2.4/mizue.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 mizue/printer/grid/border_style.py
 mizue/printer/grid/cell_renderer_args.py
 mizue/printer/grid/column.py
 mizue/printer/grid/column_settings.py
 mizue/printer/grid/grid.py
 mizue/printer/grid/row_border_position.py
 mizue/progress/__init__.py
+mizue/progress/colorful_progress.py
 mizue/progress/progress.py
 mizue/progress/progress_renderer_args.py
 mizue/progress/spinner.py
 mizue/util/__init__.py
 mizue/util/event_listener.py
 mizue/util/signal_handler.py
 mizue/util/stoppable_thread.py
```

### Comparing `mizue-0.2.3/setup.py` & `mizue-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="mizue",
-    version="0.2.3",
+    version="0.2.4",
     description="A Python package for various utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Hoshilily",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
```

