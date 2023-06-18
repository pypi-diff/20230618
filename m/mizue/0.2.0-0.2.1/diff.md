# Comparing `tmp/mizue-0.2.0.tar.gz` & `tmp/mizue-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mizue-0.2.0.tar", last modified: Sun Jun 18 01:01:21 2023, max compression
+gzip compressed data, was "mizue-0.2.1.tar", last modified: Sun Jun 18 01:30:54 2023, max compression
```

## Comparing `mizue-0.2.0.tar` & `mizue-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.859874 mizue-0.2.0/
--rw-rw-rw-   0        0        0     1085 2023-06-08 15:35:14.000000 mizue-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1471 2023-06-18 01:01:21.859874 mizue-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1123 2023-06-10 20:36:24.000000 mizue-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.827607 mizue-0.2.0/mizue/
--rw-rw-rw-   0        0        0      417 2023-06-14 12:59:22.000000 mizue-0.2.0/mizue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.832609 mizue-0.2.0/mizue/file/
--rw-rw-rw-   0        0        0       61 2023-06-14 13:01:35.000000 mizue-0.2.0/mizue/file/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-06-14 13:57:10.000000 mizue-0.2.0/mizue/file/fileutils.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.833611 mizue-0.2.0/mizue/network/
--rw-rw-rw-   0        0        0       28 2023-06-16 14:59:06.000000 mizue-0.2.0/mizue/network/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.842649 mizue-0.2.0/mizue/network/downloader/
--rw-rw-rw-   0        0        0      416 2023-06-16 23:32:00.000000 mizue-0.2.0/mizue/network/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.843647 mizue-0.2.0/mizue/network/downloader/data/
--rw-rw-rw-   0        0        0      556 2023-06-17 23:58:11.000000 mizue-0.2.0/mizue/network/downloader/data/colors.json
--rw-rw-rw-   0        0        0     1026 2023-06-17 21:34:36.000000 mizue-0.2.0/mizue/network/downloader/download_event.py
--rw-rw-rw-   0        0        0      175 2023-06-16 15:51:36.000000 mizue-0.2.0/mizue/network/downloader/download_metadata.py
--rw-rw-rw-   0        0        0     8141 2023-06-17 21:34:36.000000 mizue-0.2.0/mizue/network/downloader/downloader.py
--rw-rw-rw-   0        0        0    13287 2023-06-18 00:57:02.000000 mizue-0.2.0/mizue/network/downloader/downloader_tool.py
--rw-rw-rw-   0        0        0      230 2023-06-16 15:52:52.000000 mizue-0.2.0/mizue/network/downloader/progress_data.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.845154 mizue-0.2.0/mizue/printer/
--rw-rw-rw-   0        0        0      126 2023-06-16 14:59:43.000000 mizue-0.2.0/mizue/printer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.854213 mizue-0.2.0/mizue/printer/grid/
--rw-rw-rw-   0        0        0      449 2023-06-16 00:05:04.000000 mizue-0.2.0/mizue/printer/grid/__init__.py
--rw-rw-rw-   0        0        0       98 2023-06-14 14:01:34.000000 mizue-0.2.0/mizue/printer/grid/alignment.py
--rw-rw-rw-   0        0        0     2986 2023-06-16 13:48:26.000000 mizue-0.2.0/mizue/printer/grid/border_character_codes.py
--rw-rw-rw-   0        0        0      118 2023-06-14 14:01:47.000000 mizue-0.2.0/mizue/printer/grid/border_style.py
--rw-rw-rw-   0        0        0      144 2023-06-16 13:56:53.000000 mizue-0.2.0/mizue/printer/grid/cell_renderer_args.py
--rw-rw-rw-   0        0        0      610 2023-06-17 16:21:40.000000 mizue-0.2.0/mizue/printer/grid/column.py
--rw-rw-rw-   0        0        0      327 2023-06-16 13:56:04.000000 mizue-0.2.0/mizue/printer/grid/column_settings.py
--rw-rw-rw-   0        0        0    12613 2023-06-17 17:47:17.000000 mizue-0.2.0/mizue/printer/grid/grid.py
--rw-rw-rw-   0        0        0      106 2023-06-16 00:05:04.000000 mizue-0.2.0/mizue/printer/grid/row_border_position.py
--rw-rw-rw-   0        0        0     6120 2023-06-15 23:54:30.000000 mizue-0.2.0/mizue/printer/printer.py
--rw-rw-rw-   0        0        0      343 2023-06-15 23:54:30.000000 mizue-0.2.0/mizue/printer/terminal_colors.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.855215 mizue-0.2.0/mizue/progress/
--rw-rw-rw-   0        0        0      442 2023-06-17 20:28:28.000000 mizue-0.2.0/mizue/progress/__init__.py
--rw-rw-rw-   0        0        0     6047 2023-06-17 20:39:00.000000 mizue-0.2.0/mizue/progress/progress.py
--rw-rw-rw-   0        0        0      694 2023-06-17 20:28:19.000000 mizue-0.2.0/mizue/progress/progress_renderer_args.py
--rw-rw-rw-   0        0        0      968 2023-06-08 16:22:30.000000 mizue-0.2.0/mizue/progress/spinner.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.858874 mizue-0.2.0/mizue/util/
--rw-rw-rw-   0        0        0      241 2023-06-14 14:32:47.000000 mizue-0.2.0/mizue/util/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-06-14 11:33:39.000000 mizue-0.2.0/mizue/util/event_listener.py
--rw-rw-rw-   0        0        0      604 2023-06-14 14:32:07.000000 mizue-0.2.0/mizue/util/signal_handler.py
--rw-rw-rw-   0        0        0      443 2023-06-10 15:27:30.000000 mizue-0.2.0/mizue/util/stoppable_thread.py
--rw-rw-rw-   0        0        0     1507 2023-06-14 13:58:28.000000 mizue-0.2.0/mizue/util/utility.py
-drwxrwxrwx   0        0        0        0 2023-06-18 01:01:21.831610 mizue-0.2.0/mizue.egg-info/
--rw-rw-rw-   0        0        0     1471 2023-06-18 01:01:21.000000 mizue-0.2.0/mizue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1213 2023-06-18 01:01:21.000000 mizue-0.2.0/mizue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 01:01:21.000000 mizue-0.2.0/mizue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-18 01:01:21.000000 mizue-0.2.0/mizue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-18 01:01:21.000000 mizue-0.2.0/mizue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 01:01:21.859874 mizue-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-06-18 00:58:50.000000 mizue-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.723108 mizue-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-18 01:30:44.000000 mizue-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 01:30:54.723108 mizue-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 01:30:44.000000 mizue-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/file/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/network/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/network/downloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/download_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/download_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/downloader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/network/downloader/progress_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/printer/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue/printer/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/border_character_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/border_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/cell_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/column_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/grid/row_border_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/printer/terminal_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.723108 mizue-0.2.1/mizue/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/progress_renderer_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/progress/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.723108 mizue-0.2.1/mizue/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/signal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 01:30:44.000000 mizue-0.2.1/mizue/util/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:30:54.719108 mizue-0.2.1/mizue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 01:30:54.000000 mizue-0.2.1/mizue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:30:54.723108 mizue-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-18 01:30:44.000000 mizue-0.2.1/setup.py
```

### Comparing `mizue-0.2.0/LICENSE` & `mizue-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 merophise
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 merophise
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `mizue-0.2.0/PKG-INFO` & `mizue-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1
-Name: mizue
-Version: 0.2.0
-Summary: A Python package for various utilities
-Author: Hoshilily
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A simple package containing various command-line utilities.
-
-## Installation
-
-```bash
-  pip install mizue
-```
-
-## Usage
-
-### Printer
-
-```python
-from mizue.printer import Printer, TerminalColors as Color
-
-Printer.print_ansi("Hello World!")
-Printer.print_ansi("Hello World!", Color.RED)
-Printer.print_ansi("Hello World!", Color.RED, bold=True, underlined=True)
-```
-The ``Printer`` class is a simple wrapper around the ``print`` function. It allows you to print colored text to the terminal. The ``TerminalColors`` class contains a list of colors that can be used with the ``Printer`` class.
-The ``Printer`` class also provides the following methods:
-```python
-from mizue.printer import Printer, TerminalColors as Color
-Printer.error("Hello World!")
-Printer.warning("Hello World!")
-Printer.success("Hello World!")
-Printer.info("Hello World!")
-```
-
-It is possible to prevent the new line character from being printed at the end of the line:
-
-```python
-from mizue.printer import Printer, TerminalColors as Color
-
-Printer.prevent_newline(True)
-Printer.print_ansi("Hello World!", Color.RED)
-```
+Metadata-Version: 2.1
+Name: mizue
+Version: 0.2.1
+Summary: A Python package for various utilities
+Author: Hoshilily
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A simple package containing various command-line utilities.
+
+## Installation
+
+```bash
+  pip install mizue
+```
+
+## Usage
+
+### Printer
+
+```python
+from mizue.printer import Printer, TerminalColors as Color
+
+Printer.print_ansi("Hello World!")
+Printer.print_ansi("Hello World!", Color.RED)
+Printer.print_ansi("Hello World!", Color.RED, bold=True, underlined=True)
+```
+The ``Printer`` class is a simple wrapper around the ``print`` function. It allows you to print colored text to the terminal. The ``TerminalColors`` class contains a list of colors that can be used with the ``Printer`` class.
+The ``Printer`` class also provides the following methods:
+```python
+from mizue.printer import Printer, TerminalColors as Color
+Printer.error("Hello World!")
+Printer.warning("Hello World!")
+Printer.success("Hello World!")
+Printer.info("Hello World!")
+```
+
+It is possible to prevent the new line character from being printed at the end of the line:
+
+```python
+from mizue.printer import Printer, TerminalColors as Color
+
+Printer.prevent_newline(True)
+Printer.print_ansi("Hello World!", Color.RED)
+```
```

### Comparing `mizue-0.2.0/mizue/file/fileutils.py` & `mizue-0.2.1/mizue/file/fileutils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import os
-
-
-class FileUtils:
-    @staticmethod
-    def get_readable_file_size(size: int, suffix: str = "B"):
-        for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
-            if abs(size) < 1024.0:
-                return "%3.2f%s%s%s" % (size, " ", unit, suffix)
-            size /= 1024.0
-        return "%.1f%s%s%s" % (size, " ", 'Y', suffix)
-
-    @staticmethod
-    def list_files(path, recursive=False, fullpath=True):
-        if recursive:
-            if not fullpath:
-                filelist = FileUtils._list_files_recursively(path)
-                return FileUtils._get_base_names_only(filelist)
-            else:
-                return FileUtils._list_files_recursively(path)
-        else:
-            if not fullpath:
-                filelist = FileUtils._list_files_non_recursively(path)
-                return FileUtils._get_base_names_only(filelist)
-            else:
-                return FileUtils._list_files_non_recursively(path)
-
-    @staticmethod
-    def list_folders(path, recursive=False, fullpath=True):
-        if recursive:
-            if not fullpath:
-                folder_list = FileUtils._list_folders_recursively(path)
-                return FileUtils._get_base_names_only(folder_list)
-            else:
-                return FileUtils._list_folders_recursively(path)
-        else:
-            if not fullpath:
-                folder_list = FileUtils._list_folders_non_recursively(path)
-                return FileUtils._get_base_names_only(folder_list)
-            else:
-                return FileUtils._list_folders_non_recursively(path)
-
-    @staticmethod
-    def _list_files_recursively(path):
-        return [os.path.join(dp, f) for dp, dn, filenames in os.walk(path) for f in filenames]
-
-    @staticmethod
-    def _list_files_non_recursively(path):
-        return [os.path.join(path, f) for f in os.listdir(path) if os.path.isfile(os.path.join(path, f))]
-
-    @staticmethod
-    def _get_base_names_only(filelist: list):
-        return [os.path.basename(f) for f in filelist]
-
-    @staticmethod
-    def _list_folders_recursively(path):
-        return [dp for dp, dn, filenames in os.walk(path) if dp != path]
-
-    @staticmethod
-    def _list_folders_non_recursively(path):
-        return [os.path.join(path, item) for item in os.listdir(path) if os.path.isdir(os.path.join(path, item))]
+import os
+
+
+class FileUtils:
+    @staticmethod
+    def get_readable_file_size(size: int, suffix: str = "B"):
+        for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
+            if abs(size) < 1024.0:
+                return "%3.2f%s%s%s" % (size, " ", unit, suffix)
+            size /= 1024.0
+        return "%.1f%s%s%s" % (size, " ", 'Y', suffix)
+
+    @staticmethod
+    def list_files(path, recursive=False, fullpath=True):
+        if recursive:
+            if not fullpath:
+                filelist = FileUtils._list_files_recursively(path)
+                return FileUtils._get_base_names_only(filelist)
+            else:
+                return FileUtils._list_files_recursively(path)
+        else:
+            if not fullpath:
+                filelist = FileUtils._list_files_non_recursively(path)
+                return FileUtils._get_base_names_only(filelist)
+            else:
+                return FileUtils._list_files_non_recursively(path)
+
+    @staticmethod
+    def list_folders(path, recursive=False, fullpath=True):
+        if recursive:
+            if not fullpath:
+                folder_list = FileUtils._list_folders_recursively(path)
+                return FileUtils._get_base_names_only(folder_list)
+            else:
+                return FileUtils._list_folders_recursively(path)
+        else:
+            if not fullpath:
+                folder_list = FileUtils._list_folders_non_recursively(path)
+                return FileUtils._get_base_names_only(folder_list)
+            else:
+                return FileUtils._list_folders_non_recursively(path)
+
+    @staticmethod
+    def _list_files_recursively(path):
+        return [os.path.join(dp, f) for dp, dn, filenames in os.walk(path) for f in filenames]
+
+    @staticmethod
+    def _list_files_non_recursively(path):
+        return [os.path.join(path, f) for f in os.listdir(path) if os.path.isfile(os.path.join(path, f))]
+
+    @staticmethod
+    def _get_base_names_only(filelist: list):
+        return [os.path.basename(f) for f in filelist]
+
+    @staticmethod
+    def _list_folders_recursively(path):
+        return [dp for dp, dn, filenames in os.walk(path) if dp != path]
+
+    @staticmethod
+    def _list_folders_non_recursively(path):
+        return [os.path.join(path, item) for item in os.listdir(path) if os.path.isdir(os.path.join(path, item))]
```

### Comparing `mizue-0.2.0/mizue/network/downloader/data/colors.json` & `mizue-0.2.1/mizue/network/downloader/data/colors.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-00000000: 7b0d 0a20 2020 2022 7a69 7022 3a20 2223  {..    "zip": "#
-00000010: 4642 4233 3135 222c 0d0a 2020 2020 2272  FBB315",..    "r
-00000020: 6172 223a 2022 2346 4242 3331 3522 2c0d  ar": "#FBB315",.
-00000030: 0a20 2020 2022 7461 7222 3a20 2223 4642  .    "tar": "#FB
-00000040: 4233 3135 222c 0d0a 2020 2020 2267 7a22  B315",..    "gz"
-00000050: 3a20 2223 4642 4233 3135 222c 0d0a 2020  : "#FBB315",..  
-00000060: 2020 2262 7a32 223a 2022 2346 4242 3331    "bz2": "#FBB31
-00000070: 3522 2c0d 0a20 2020 2022 377a 223a 2022  5",..    "7z": "
-00000080: 2346 4242 3331 3522 2c0d 0a20 2020 2022  #FBB315",..    "
-00000090: 6a70 6722 3a20 2223 4231 4330 3730 222c  jpg": "#B1C070",
-000000a0: 0d0a 2020 2020 2270 6e67 223a 2022 2330  ..    "png": "#0
-000000b0: 3041 3939 3722 2c0d 0a20 2020 2022 6769  0A997",..    "gi
-000000c0: 6622 3a20 2223 3844 3742 4133 222c 0d0a  f": "#8D7BA3",..
-000000d0: 2020 2020 2261 7669 223a 2022 2338 4437      "avi": "#8D7
-000000e0: 4241 3322 2c0d 0a20 2020 2022 6d6b 7622  BA3",..    "mkv"
-000000f0: 3a20 2223 3844 3742 4133 222c 0d0a 2020  : "#8D7BA3",..  
-00000100: 2020 226d 7034 223a 2022 2338 4437 4241    "mp4": "#8D7BA
-00000110: 3322 2c0d 0a20 2020 2022 6d70 3322 3a20  3",..    "mp3": 
-00000120: 2223 4544 3446 3734 222c 0d0a 2020 2020  "#ED4F74",..    
-00000130: 2277 6176 223a 2022 2345 4434 4637 3422  "wav": "#ED4F74"
-00000140: 2c0d 0a20 2020 2022 7064 6622 3a20 2223  ,..    "pdf": "#
-00000150: 4138 3036 3246 222c 0d0a 2020 2020 2264  A8062F",..    "d
-00000160: 6f63 223a 2022 2330 3041 4546 3022 2c0d  oc": "#00AEF0",.
-00000170: 0a20 2020 2022 646f 6378 223a 2022 2330  .    "docx": "#0
-00000180: 3041 4546 3022 2c0d 0a20 2020 2022 786c  0AEF0",..    "xl
-00000190: 7322 3a20 2223 3835 4333 3431 222c 0d0a  s": "#85C341",..
-000001a0: 2020 2020 2278 6c73 7822 3a20 2223 3835      "xlsx": "#85
-000001b0: 4333 3431 222c 0d0a 2020 2020 2270 7074  C341",..    "ppt
-000001c0: 223a 2022 2346 3538 3431 4422 2c0d 0a20  ": "#F5841D",.. 
-000001d0: 2020 2022 7070 7478 223a 2022 2346 3538     "pptx": "#F58
-000001e0: 3431 4422 2c0d 0a20 2020 2022 7478 7422  41D",..    "txt"
-000001f0: 3a20 2223 4334 3939 3643 222c 0d0a 2020  : "#C4996C",..  
-00000200: 2020 2265 7865 223a 2022 2330 3043 3835    "exe": "#00C85
-00000210: 3422 2c0d 0a20 2020 2022 6d73 6922 3a20  4",..    "msi": 
-00000220: 2223 3030 4338 3534 220d 0a7d            "#00C854"..}
+00000000: 7b0a 2020 2020 227a 6970 223a 2022 2346  {.    "zip": "#F
+00000010: 4242 3331 3522 2c0a 2020 2020 2272 6172  BB315",.    "rar
+00000020: 223a 2022 2346 4242 3331 3522 2c0a 2020  ": "#FBB315",.  
+00000030: 2020 2274 6172 223a 2022 2346 4242 3331    "tar": "#FBB31
+00000040: 3522 2c0a 2020 2020 2267 7a22 3a20 2223  5",.    "gz": "#
+00000050: 4642 4233 3135 222c 0a20 2020 2022 627a  FBB315",.    "bz
+00000060: 3222 3a20 2223 4642 4233 3135 222c 0a20  2": "#FBB315",. 
+00000070: 2020 2022 377a 223a 2022 2346 4242 3331     "7z": "#FBB31
+00000080: 3522 2c0a 2020 2020 226a 7067 223a 2022  5",.    "jpg": "
+00000090: 2342 3143 3037 3022 2c0a 2020 2020 2270  #B1C070",.    "p
+000000a0: 6e67 223a 2022 2330 3041 3939 3722 2c0a  ng": "#00A997",.
+000000b0: 2020 2020 2267 6966 223a 2022 2338 4437      "gif": "#8D7
+000000c0: 4241 3322 2c0a 2020 2020 2261 7669 223a  BA3",.    "avi":
+000000d0: 2022 2338 4437 4241 3322 2c0a 2020 2020   "#8D7BA3",.    
+000000e0: 226d 6b76 223a 2022 2338 4437 4241 3322  "mkv": "#8D7BA3"
+000000f0: 2c0a 2020 2020 226d 7034 223a 2022 2338  ,.    "mp4": "#8
+00000100: 4437 4241 3322 2c0a 2020 2020 226d 7033  D7BA3",.    "mp3
+00000110: 223a 2022 2345 4434 4637 3422 2c0a 2020  ": "#ED4F74",.  
+00000120: 2020 2277 6176 223a 2022 2345 4434 4637    "wav": "#ED4F7
+00000130: 3422 2c0a 2020 2020 2270 6466 223a 2022  4",.    "pdf": "
+00000140: 2341 3830 3632 4622 2c0a 2020 2020 2264  #A8062F",.    "d
+00000150: 6f63 223a 2022 2330 3041 4546 3022 2c0a  oc": "#00AEF0",.
+00000160: 2020 2020 2264 6f63 7822 3a20 2223 3030      "docx": "#00
+00000170: 4145 4630 222c 0a20 2020 2022 786c 7322  AEF0",.    "xls"
+00000180: 3a20 2223 3835 4333 3431 222c 0a20 2020  : "#85C341",.   
+00000190: 2022 786c 7378 223a 2022 2338 3543 3334   "xlsx": "#85C34
+000001a0: 3122 2c0a 2020 2020 2270 7074 223a 2022  1",.    "ppt": "
+000001b0: 2346 3538 3431 4422 2c0a 2020 2020 2270  #F5841D",.    "p
+000001c0: 7074 7822 3a20 2223 4635 3834 3144 222c  ptx": "#F5841D",
+000001d0: 0a20 2020 2022 7478 7422 3a20 2223 4334  .    "txt": "#C4
+000001e0: 3939 3643 222c 0a20 2020 2022 6578 6522  996C",.    "exe"
+000001f0: 3a20 2223 3030 4338 3534 222c 0a20 2020  : "#00C854",.   
+00000200: 2022 6d73 6922 3a20 2223 3030 4338 3534   "msi": "#00C854
+00000210: 220a 7d                                  ".}
```

### Comparing `mizue-0.2.0/mizue/network/downloader/downloader.py` & `mizue-0.2.1/mizue/network/downloader/downloader.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import os
-import urllib.parse
-import uuid
-from typing import Callable
-
-import requests
-from pathvalidate import sanitize_filename
-
-from mizue.util import EventListener
-from .download_event import DownloadEventType, DownloadFailureEvent, DownloadCompleteEvent, DownloadStartEvent, \
-    ProgressEventArgs
-from .download_metadata import DownloadMetadata
-from .progress_data import ProgressData
-
-
-class Downloader(EventListener):
-    def __init__(self):
-        self._alive = True
-
-        self.output_path = "."
-        """The output path for the downloaded files"""
-
-        self.retry_count = 5
-        """The number of times to retry the download if it fails"""
-
-        self.timeout = 10
-        """The timeout in seconds for the connection"""
-
-    def close(self):
-        """
-        Closes the downloader. This will stop any ongoing downloads.
-
-        In order to download again, a new instance of the downloader must be created,
-        or the open() method must be called.
-        """
-        self._alive = False
-
-    def download(self, url: str, output_path: str = None):
-        path_to_save = output_path if output_path is not None and len(output_path) > 0 else self.output_path
-
-        response = self._get_response(url)
-        if response and response.status_code == 200:
-            metadata = self._get_download_metadata(response, path_to_save)
-            self._download(response, metadata, path_to_save, lambda init_data: self._progress_init(init_data),
-                           lambda progress_data: self._progress_callback(progress_data))
-        else:
-            self._fire_failure_event(url, response, exception=None)
-
-    def open(self):
-        """
-        Opens the downloader. This will allow downloads to be performed once again.
-        Use this method if the downloader has been closed via the close() method.
-        """
-        self._alive = True
-
-    def _download(self, response: requests.Response, metadata: DownloadMetadata, output_path: str = None,
-                  progress_init: Callable[[DownloadMetadata], None] = None,
-                  progress_callback: Callable[[ProgressData], None] = None):
-        if not os.path.exists(output_path):
-            os.makedirs(output_path, exist_ok=True)
-        if progress_init:
-            progress_init(metadata)
-        try:
-            with open(metadata.filepath, 'wb') as f:
-                downloaded = 0
-                for chunk in response.iter_content(chunk_size=1024):
-                    if not self._alive:
-                        break
-                    response.raw.decode_content = True
-                    chunk_size = len(chunk)
-                    f.write(chunk)
-                    downloaded += chunk_size
-                    percent = int((downloaded / metadata.filesize) * 100)
-                    if progress_callback:
-                        progress_data = ProgressData(
-                            downloaded=downloaded,
-                            filename=metadata.filename,
-                            filepath=metadata.filepath,
-                            filesize=metadata.filesize,
-                            percent=percent,
-                            finished=False,
-                            url=metadata.url,
-                            uuid=metadata.uuid
-                        )
-                        progress_callback(progress_data)
-                if self._alive:
-                    if progress_callback:
-                        progress_data = ProgressData(
-                            downloaded=downloaded,
-                            filename=metadata.filename,
-                            filepath=metadata.filepath,
-                            filesize=metadata.filesize,
-                            percent=100,
-                            finished=True,
-                            url=metadata.url,
-                            uuid=metadata.uuid
-                        )
-                        progress_callback(progress_data)
-                else:
-                    f.close()
-                    os.remove(metadata.filepath)
-                    self._fire_failure_event(metadata.url, response, exception=Exception("Download cancelled"),
-                                             filepath=metadata.filepath)
-        except Exception as e:
-            self._fire_failure_event(metadata.url, response, exception=e, filepath=metadata.filepath)
-            raise e
-
-    def _fire_failure_event(self, url: str, response: requests.Response, exception: BaseException | None,
-                            filepath: str = None):
-        self._fire_event(DownloadEventType.FAILED, DownloadFailureEvent(
-            url=url,
-            status_code=response.status_code if response else -1,
-            reason=response.reason if response else "Unknown",
-            exception=exception,
-            filepath=filepath,
-        ))
-
-    def _get_download_metadata(self, response: requests.Response, output_path: str) -> DownloadMetadata:
-        filename = self._get_filename(response)
-        filepath = os.path.join(output_path, filename)
-        filesize = int(response.headers["Content-Length"] if "Content-Length" in response.headers.keys() else 1)
-        return DownloadMetadata(
-            filename=filename,
-            filepath=filepath,
-            filesize=filesize,
-            url=response.url,
-            uuid=str(uuid.uuid4())
-        )
-
-    @staticmethod
-    def _get_filename(response: requests.Response) -> str | None:
-        content_disposition = response.headers.get('content-disposition')
-        if content_disposition:
-            filename = content_disposition.split("filename=")[1].split(";")[0].replace("\"", "").strip()
-            if filename:
-                return filename
-        else:
-            unquoted_filename = urllib.parse.unquote(response.url.split("/")[-1], encoding='utf-8', errors='replace')
-            if unquoted_filename and "?" in unquoted_filename:
-                unquoted_filename = unquoted_filename[:unquoted_filename.rfind("?")]
-            if unquoted_filename:
-                return sanitize_filename(unquoted_filename)
-        return None
-
-    def _get_response(self, url: str) -> requests.Response | None:
-        fetching = True
-        fetch_try_count = 0
-        headers = {
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
-        }
-
-        response: requests.Response | None = None
-        while fetching:
-            try:
-                response = requests.get(url, stream=True, timeout=self.timeout, headers=headers)
-                fetching = False
-            except requests.exceptions.Timeout as e:
-                fetch_try_count += 1
-                if fetch_try_count > self.retry_count:
-                    fetching = False
-                    self._fire_failure_event(url, response, e)
-                continue
-            except requests.exceptions.RequestException as e:
-                fetching = False
-                self._fire_failure_event(url, response, e)
-                continue
-        return response
-
-    def _progress_callback(self, data: ProgressData):
-        self._fire_event(DownloadEventType.PROGRESS, ProgressEventArgs(
-            downloaded=data.downloaded,
-            percent=data.percent,
-            filename=data.filename,
-            filepath=data.filepath,
-            filesize=data.filesize,
-            url=data.url,
-        ))
-
-        if data.finished:
-            self._fire_event(DownloadEventType.COMPLETED, DownloadCompleteEvent(
-                url=data.url,
-                filename=data.filename,
-                filepath=data.filepath,
-                filesize=data.filesize,
-            ))
-
-    def _progress_init(self, data: DownloadMetadata):
-        self._fire_event(DownloadEventType.STARTED, DownloadStartEvent(
-            url=data.url,
-            filename=data.filename,
-            filepath=data.filepath,
-            filesize=data.filesize,
-        ))
+import os
+import urllib.parse
+import uuid
+from typing import Callable
+
+import requests
+from pathvalidate import sanitize_filename
+
+from mizue.util import EventListener
+from .download_event import DownloadEventType, DownloadFailureEvent, DownloadCompleteEvent, DownloadStartEvent, \
+    ProgressEventArgs
+from .download_metadata import DownloadMetadata
+from .progress_data import ProgressData
+
+
+class Downloader(EventListener):
+    def __init__(self):
+        self._alive = True
+
+        self.output_path = "."
+        """The output path for the downloaded files"""
+
+        self.retry_count = 5
+        """The number of times to retry the download if it fails"""
+
+        self.timeout = 10
+        """The timeout in seconds for the connection"""
+
+    def close(self):
+        """
+        Closes the downloader. This will stop any ongoing downloads.
+
+        In order to download again, a new instance of the downloader must be created,
+        or the open() method must be called.
+        """
+        self._alive = False
+
+    def download(self, url: str, output_path: str = None):
+        path_to_save = output_path if output_path is not None and len(output_path) > 0 else self.output_path
+
+        response = self._get_response(url)
+        if response and response.status_code == 200:
+            metadata = self._get_download_metadata(response, path_to_save)
+            self._download(response, metadata, path_to_save, lambda init_data: self._progress_init(init_data),
+                           lambda progress_data: self._progress_callback(progress_data))
+        else:
+            self._fire_failure_event(url, response, exception=None)
+
+    def open(self):
+        """
+        Opens the downloader. This will allow downloads to be performed once again.
+        Use this method if the downloader has been closed via the close() method.
+        """
+        self._alive = True
+
+    def _download(self, response: requests.Response, metadata: DownloadMetadata, output_path: str = None,
+                  progress_init: Callable[[DownloadMetadata], None] = None,
+                  progress_callback: Callable[[ProgressData], None] = None):
+        if not os.path.exists(output_path):
+            os.makedirs(output_path, exist_ok=True)
+        if progress_init:
+            progress_init(metadata)
+        try:
+            with open(metadata.filepath, 'wb') as f:
+                downloaded = 0
+                for chunk in response.iter_content(chunk_size=1024):
+                    if not self._alive:
+                        break
+                    response.raw.decode_content = True
+                    chunk_size = len(chunk)
+                    f.write(chunk)
+                    downloaded += chunk_size
+                    percent = int((downloaded / metadata.filesize) * 100)
+                    if progress_callback:
+                        progress_data = ProgressData(
+                            downloaded=downloaded,
+                            filename=metadata.filename,
+                            filepath=metadata.filepath,
+                            filesize=metadata.filesize,
+                            percent=percent,
+                            finished=False,
+                            url=metadata.url,
+                            uuid=metadata.uuid
+                        )
+                        progress_callback(progress_data)
+                if self._alive:
+                    if progress_callback:
+                        progress_data = ProgressData(
+                            downloaded=downloaded,
+                            filename=metadata.filename,
+                            filepath=metadata.filepath,
+                            filesize=metadata.filesize,
+                            percent=100,
+                            finished=True,
+                            url=metadata.url,
+                            uuid=metadata.uuid
+                        )
+                        progress_callback(progress_data)
+                else:
+                    f.close()
+                    os.remove(metadata.filepath)
+                    self._fire_failure_event(metadata.url, response, exception=Exception("Download cancelled"),
+                                             filepath=metadata.filepath)
+        except Exception as e:
+            self._fire_failure_event(metadata.url, response, exception=e, filepath=metadata.filepath)
+            raise e
+
+    def _fire_failure_event(self, url: str, response: requests.Response, exception: BaseException | None,
+                            filepath: str = None):
+        self._fire_event(DownloadEventType.FAILED, DownloadFailureEvent(
+            url=url,
+            status_code=response.status_code if response else -1,
+            reason=response.reason if response else "Unknown",
+            exception=exception,
+            filepath=filepath,
+        ))
+
+    def _get_download_metadata(self, response: requests.Response, output_path: str) -> DownloadMetadata:
+        filename = self._get_filename(response)
+        filepath = os.path.join(output_path, filename)
+        filesize = int(response.headers["Content-Length"] if "Content-Length" in response.headers.keys() else 1)
+        return DownloadMetadata(
+            filename=filename,
+            filepath=filepath,
+            filesize=filesize,
+            url=response.url,
+            uuid=str(uuid.uuid4())
+        )
+
+    @staticmethod
+    def _get_filename(response: requests.Response) -> str | None:
+        content_disposition = response.headers.get('content-disposition')
+        if content_disposition:
+            filename = content_disposition.split("filename=")[1].split(";")[0].replace("\"", "").strip()
+            if filename:
+                return filename
+        else:
+            unquoted_filename = urllib.parse.unquote(response.url.split("/")[-1], encoding='utf-8', errors='replace')
+            if unquoted_filename and "?" in unquoted_filename:
+                unquoted_filename = unquoted_filename[:unquoted_filename.rfind("?")]
+            if unquoted_filename:
+                return sanitize_filename(unquoted_filename)
+        return None
+
+    def _get_response(self, url: str) -> requests.Response | None:
+        fetching = True
+        fetch_try_count = 0
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
+        }
+
+        response: requests.Response | None = None
+        while fetching:
+            try:
+                response = requests.get(url, stream=True, timeout=self.timeout, headers=headers)
+                fetching = False
+            except requests.exceptions.Timeout as e:
+                fetch_try_count += 1
+                if fetch_try_count > self.retry_count:
+                    fetching = False
+                    self._fire_failure_event(url, response, e)
+                continue
+            except requests.exceptions.RequestException as e:
+                fetching = False
+                self._fire_failure_event(url, response, e)
+                continue
+        return response
+
+    def _progress_callback(self, data: ProgressData):
+        self._fire_event(DownloadEventType.PROGRESS, ProgressEventArgs(
+            downloaded=data.downloaded,
+            percent=data.percent,
+            filename=data.filename,
+            filepath=data.filepath,
+            filesize=data.filesize,
+            url=data.url,
+        ))
+
+        if data.finished:
+            self._fire_event(DownloadEventType.COMPLETED, DownloadCompleteEvent(
+                url=data.url,
+                filename=data.filename,
+                filepath=data.filepath,
+                filesize=data.filesize,
+            ))
+
+    def _progress_init(self, data: DownloadMetadata):
+        self._fire_event(DownloadEventType.STARTED, DownloadStartEvent(
+            url=data.url,
+            filename=data.filename,
+            filepath=data.filepath,
+            filesize=data.filesize,
+        ))
```

### Comparing `mizue-0.2.0/mizue/network/downloader/downloader_tool.py` & `mizue-0.2.1/mizue/network/downloader/downloader_tool.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-import concurrent.futures
-import json
-import os
-import time
-from dataclasses import dataclass
-
-from mizue.file import FileUtils
-from mizue.network.downloader import DownloadStartEvent, ProgressEventArgs, DownloadCompleteEvent, Downloader, \
-    DownloadEventType, DownloadFailureEvent
-from mizue.printer import Printer
-from mizue.printer.grid import ColumnSettings, Alignment, Grid, BorderStyle, CellRendererArgs
-from mizue.progress import Progress, ProgressBarRendererArgs, SpinnerRendererArgs, LabelRendererArgs, \
-    InfoSeparatorRendererArgs, InfoTextRendererArgs, PercentageRendererArgs
-
-
-@dataclass
-class _DownloadReport:
-    filename: str
-    filesize: int
-    url: str
-
-
-class DownloaderTool:
-    def __init__(self):
-        self._file_color_scheme = {}
-        self._report_data: list[_DownloadReport] = []
-        self._bulk_download_size = 0
-        self._downloaded_count = 0
-        self._total_download_count = 0
-        self.progress: Progress | None = None
-        self._load_color_scheme()
-
-    def download(self, url: str, output_path: str):
-        """
-        Download a file to a specified directory
-        :param url: The URL to download
-        :param output_path: The output directory
-        :return: None
-        """
-        filepath = []
-        downloader = Downloader()
-        downloader.add_event(DownloadEventType.STARTED, lambda event: self._on_download_start(event, filepath))
-        downloader.add_event(DownloadEventType.PROGRESS, lambda event: self._on_download_progress(event))
-        downloader.add_event(DownloadEventType.COMPLETED, lambda event: self._on_download_complete(event))
-        downloader.add_event(DownloadEventType.FAILED, lambda event: self._on_download_failure(event))
-        try:
-            downloader.download(url, output_path)
-        except KeyboardInterrupt:
-            downloader.close()
-            self.progress.stop()
-            Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
-            if len(filepath) > 0:
-                os.remove(filepath[0])
-            self._report_data.append(_DownloadReport(url, 0, url))
-        self._print_report()
-
-    def download_bulk(self, urls: list[str] | list[tuple[str, str]], output_path: str | None = None, parallel: int = 4):
-        """
-        Download a list of files to a specified directory or a list of [url, output_path] tuples.
-
-        If the urls parameter is a list of [url, output_path] tuples, every url will be downloaded to its corresponding
-        output_path.
-
-        If the urls parameter is a list of urls, every url will be downloaded to the output_path parameter. In this case,
-        the output_path parameter must be specified.
-        :param urls: A list of urls or a list of [url, output_path] tuples
-        :param output_path: The output directory if the urls parameter is a list of urls
-        :param parallel: Number of parallel downloads
-        :return: None
-        """
-        if isinstance(urls[0], tuple):
-            self.download_tuple(urls, parallel)
-        else:
-            self.download_list(urls, output_path, parallel)
-
-    def download_list(self, urls: list[str], output_path: str, parallel: int = 4):
-        """
-        Download a list of files to a specified directory
-        :param urls: The list of URLs to download
-        :param output_path: The output directory
-        :param parallel: Number of parallel downloads
-        :return: None
-        """
-        self.download_tuple([(url, output_path) for url in urls], parallel)
-
-    def download_tuple(self, urls: list[tuple[str, str]], parallel: int = 4):
-        """
-        Download a list of [url, output_path] tuples. Every url will be downloaded to its corresponding output_path.
-        :param urls: A list of [url, output_path] tuples
-        :param parallel: Number of parallel downloads
-        :return: None
-        """
-
-        self.progress = Progress(start=0, end=len(urls), value=0)
-        self._configure_progress()
-        self.progress.start()
-        self._downloaded_count = 0
-        self._total_download_count = len(urls)
-        download_dict = {}
-
-        with concurrent.futures.ThreadPoolExecutor(max_workers=parallel) as executor:
-            try:
-                responses: list[concurrent.futures.Future] = []
-                downloader = Downloader()
-                downloader.add_event(DownloadEventType.PROGRESS,
-                                     lambda event: self._on_bulk_download_progress(event, download_dict))
-                downloader.add_event(DownloadEventType.COMPLETED,
-                                     lambda event: self._on_bulk_download_complete(event))
-                downloader.add_event(DownloadEventType.FAILED, lambda event: self._on_bulk_download_failed(event))
-                for url, output_path in list(set(urls)):
-                    responses.append(executor.submit(downloader.download, url, output_path))
-                for response in concurrent.futures.as_completed(responses):
-                    self._downloaded_count += 1
-                    self.progress.update_value(self._downloaded_count)
-                    self.progress.set_info(self._get_bulk_progress_info(download_dict))
-                executor.shutdown(wait=True)
-            except KeyboardInterrupt:
-                downloader.close()
-                self.progress.stop()
-                Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
-                executor.shutdown(wait=False, cancel_futures=True)
-        self.progress.stop()
-        self._print_report()
-
-    def _configure_progress(self):
-        self.progress.info_separator_renderer = self._info_separator_renderer
-        self.progress.info_text_renderer = self._info_text_renderer
-        self.progress.label_renderer = self._label_renderer
-        self.progress.percentage_renderer = self._percentage_renderer
-        self.progress.progress_bar_renderer = self._progress_bar_renderer
-        self.progress.spinner_renderer = self._spinner_renderer
-        self.progress.label = "Downloading: "
-
-    @staticmethod
-    def _get_basic_colored_text(text: str, percentage: float):
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
-
-    def _get_bulk_progress_info(self, download_dict: dict):
-        file_progress_text = f'[{self._downloaded_count}/{self._total_download_count}]'
-        size_text = FileUtils.get_readable_file_size(sum(download_dict.values()))
-        return f'{file_progress_text} [{size_text}]'
-
-    @staticmethod
-    def _info_separator_renderer(args: InfoSeparatorRendererArgs):
-        return Printer.format_hex(args.separator, '#FFCC75')
-
-    @staticmethod
-    def _info_text_renderer(args: InfoTextRendererArgs):
-        return Printer.format_hex(args.text, '#FFCC75')
-        # return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
-
-    @staticmethod
-    def _label_renderer(args: LabelRendererArgs):
-        if args.percentage < 100:
-            return Printer.format_hex(args.label, '#FFCC75')
-        return Printer.format_hex('Downloaded: ', '#0EB33B')
-
-    def _load_color_scheme(self):
-        file_path = os.path.join(os.path.dirname(__file__), "data", "colors.json")
-        with open(file_path, "r") as f:
-            self._file_color_scheme = json.load(f)
-
-    def _on_bulk_download_complete(self, event: DownloadCompleteEvent):
-        self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
-
-    def _on_bulk_download_failed(self, event: DownloadFailureEvent):
-        self._report_data.append(_DownloadReport("", 0, event.url))
-
-    def _on_bulk_download_progress(self, event: ProgressEventArgs, download_dict: dict):
-        download_dict[event.url] = event.downloaded
-        self.progress.set_info(self._get_bulk_progress_info(download_dict))
-
-    def _on_download_complete(self, event: DownloadCompleteEvent):
-        self.progress.update_value(event.filesize)
-        downloaded_info = FileUtils.get_readable_file_size(event.filesize)
-        filesize_info = FileUtils.get_readable_file_size(event.filesize)
-        info = f'[{downloaded_info}/{filesize_info}]'
-        self.progress.set_info(info)
-        time.sleep(0.5)
-        self.progress.stop()
-        self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
-
-    def _on_download_failure(self, event: DownloadFailureEvent):
-        if isinstance(event.exception, KeyboardInterrupt):
-            Printer.warning("Download has been cancelled by user.")
-            print(os.linesep)
-        if self.progress:
-            self.progress.terminate()
-        self._report_data.append(_DownloadReport("", 0, event.url))
-
-    def _on_download_progress(self, event: ProgressEventArgs):
-        self.progress.update_value(event.downloaded)
-        downloaded_info = FileUtils.get_readable_file_size(event.downloaded)
-        filesize_info = FileUtils.get_readable_file_size(event.filesize)
-        info = f'[{downloaded_info}/{filesize_info}]'
-        self.progress.set_info(info)
-
-    def _on_download_start(self, event: DownloadStartEvent, filepath: list[str]):
-        self.progress = Progress(start=0, end=event.filesize, value=0)
-        self._configure_progress()
-        self.progress.start()
-        filepath.append(event.filepath)
-
-    @staticmethod
-    def _percentage_renderer(args: PercentageRendererArgs):
-        return DownloaderTool._get_basic_colored_text("{:.2f}%".format(args.percentage), args.percentage)
-
-    def _print_report(self):
-        success_data = [report for report in self._report_data if report.filesize > 0]
-        failed_data = [report for report in self._report_data if report.filesize == 0]
-        row_index = 1
-        success_grid_data = []
-        for report in success_data:
-            filename, ext = os.path.splitext(report.filename)
-            success_grid_data.append(
-                [row_index, report.filename, ext[1:], FileUtils.get_readable_file_size(report.filesize)])
-            row_index += 1
-
-        failed_grid_data = []
-        for report in failed_data:
-            failed_grid_data.append([row_index, report.url, "", 'Failed'])
-            row_index += 1
-
-        grid_columns: list[ColumnSettings] = [
-            ColumnSettings(title='#', alignment=Alignment.RIGHT,
-                           renderer=lambda x: Printer.format_hex(x.cell, '#FFCC75')),
-            ColumnSettings(title='Filename/URL', renderer=self._report_grid_file_column_cell_renderer),
-            ColumnSettings(title='Type', alignment=Alignment.RIGHT,
-                           renderer=self._report_grid_file_type_column_cell_renderer),
-            ColumnSettings(title='Filesize/Status', alignment=Alignment.RIGHT,
-                           renderer=lambda x: Printer.format_hex(x.cell, '#FF0000')
-                           if x.cell == 'Failed' else self._report_grid_cell_renderer(x))
-        ]
-        grid = Grid(grid_columns, success_grid_data + failed_grid_data)
-        grid.border_style = BorderStyle.SINGLE
-        grid.border_color = '#FFCC75'
-        grid.cell_renderer = self._report_grid_cell_renderer
-        print(os.linesep)
-        grid.print()
-
-    @staticmethod
-    def _progress_bar_renderer(args: ProgressBarRendererArgs):
-        return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
-
-    @staticmethod
-    def _report_grid_cell_renderer(args: CellRendererArgs):
-        if args.cell.endswith("KB"):
-            return Printer.format_hex(args.cell, '#00a9ff')
-        if args.cell.endswith("MB"):
-            return Printer.format_hex(args.cell, '#d2309a')
-        if args.is_header:
-            return Printer.format_hex(args.cell, '#FFCC75')
-        return args.cell
-
-    def _report_grid_file_column_cell_renderer(self, args: CellRendererArgs):
-        if args.is_header:
-            return Printer.format_hex(args.cell, '#FFCC75')
-        file, ext = os.path.splitext(args.cell)
-        color = self._file_color_scheme.get(ext[1:], '#FFFFFF')
-        return Printer.format_hex(args.cell, color)
-
-    def _report_grid_file_type_column_cell_renderer(self, args: CellRendererArgs):
-        if args.is_header:
-            return Printer.format_hex(args.cell, '#FFCC75')
-        color = self._file_color_scheme.get(args.cell, '#FFFFFF')
-        return Printer.format_hex(args.cell, color)
-
-    @staticmethod
-    def _spinner_renderer(args: SpinnerRendererArgs):
-        return DownloaderTool._get_basic_colored_text(args.spinner, args.percentage)
+import concurrent.futures
+import json
+import os
+import time
+from dataclasses import dataclass
+
+from mizue.file import FileUtils
+from mizue.network.downloader import DownloadStartEvent, ProgressEventArgs, DownloadCompleteEvent, Downloader, \
+    DownloadEventType, DownloadFailureEvent
+from mizue.printer import Printer
+from mizue.printer.grid import ColumnSettings, Alignment, Grid, BorderStyle, CellRendererArgs
+from mizue.progress import Progress, ProgressBarRendererArgs, SpinnerRendererArgs, LabelRendererArgs, \
+    InfoSeparatorRendererArgs, InfoTextRendererArgs, PercentageRendererArgs
+
+
+@dataclass
+class _DownloadReport:
+    filename: str
+    filesize: int
+    url: str
+
+
+class DownloaderTool:
+    def __init__(self):
+        self._file_color_scheme = {}
+        self._report_data: list[_DownloadReport] = []
+        self._bulk_download_size = 0
+        self._downloaded_count = 0
+        self._total_download_count = 0
+        self.progress: Progress | None = None
+        self._load_color_scheme()
+
+    def download(self, url: str, output_path: str):
+        """
+        Download a file to a specified directory
+        :param url: The URL to download
+        :param output_path: The output directory
+        :return: None
+        """
+        filepath = []
+        downloader = Downloader()
+        downloader.add_event(DownloadEventType.STARTED, lambda event: self._on_download_start(event, filepath))
+        downloader.add_event(DownloadEventType.PROGRESS, lambda event: self._on_download_progress(event))
+        downloader.add_event(DownloadEventType.COMPLETED, lambda event: self._on_download_complete(event))
+        downloader.add_event(DownloadEventType.FAILED, lambda event: self._on_download_failure(event))
+        try:
+            downloader.download(url, output_path)
+        except KeyboardInterrupt:
+            downloader.close()
+            self.progress.stop()
+            Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
+            if len(filepath) > 0:
+                os.remove(filepath[0])
+            self._report_data.append(_DownloadReport(url, 0, url))
+        self._print_report()
+
+    def download_bulk(self, urls: list[str] | list[tuple[str, str]], output_path: str | None = None, parallel: int = 4):
+        """
+        Download a list of files to a specified directory or a list of [url, output_path] tuples.
+
+        If the urls parameter is a list of [url, output_path] tuples, every url will be downloaded to its corresponding
+        output_path.
+
+        If the urls parameter is a list of urls, every url will be downloaded to the output_path parameter. In this case,
+        the output_path parameter must be specified.
+        :param urls: A list of urls or a list of [url, output_path] tuples
+        :param output_path: The output directory if the urls parameter is a list of urls
+        :param parallel: Number of parallel downloads
+        :return: None
+        """
+        if isinstance(urls[0], tuple):
+            self.download_tuple(urls, parallel)
+        else:
+            self.download_list(urls, output_path, parallel)
+
+    def download_list(self, urls: list[str], output_path: str, parallel: int = 4):
+        """
+        Download a list of files to a specified directory
+        :param urls: The list of URLs to download
+        :param output_path: The output directory
+        :param parallel: Number of parallel downloads
+        :return: None
+        """
+        self.download_tuple([(url, output_path) for url in urls], parallel)
+
+    def download_tuple(self, urls: list[tuple[str, str]], parallel: int = 4):
+        """
+        Download a list of [url, output_path] tuples. Every url will be downloaded to its corresponding output_path.
+        :param urls: A list of [url, output_path] tuples
+        :param parallel: Number of parallel downloads
+        :return: None
+        """
+
+        self.progress = Progress(start=0, end=len(urls), value=0)
+        self._configure_progress()
+        self.progress.start()
+        self._downloaded_count = 0
+        self._total_download_count = len(urls)
+        download_dict = {}
+
+        with concurrent.futures.ThreadPoolExecutor(max_workers=parallel) as executor:
+            try:
+                responses: list[concurrent.futures.Future] = []
+                downloader = Downloader()
+                downloader.add_event(DownloadEventType.PROGRESS,
+                                     lambda event: self._on_bulk_download_progress(event, download_dict))
+                downloader.add_event(DownloadEventType.COMPLETED,
+                                     lambda event: self._on_bulk_download_complete(event))
+                downloader.add_event(DownloadEventType.FAILED, lambda event: self._on_bulk_download_failed(event))
+                for url, output_path in list(set(urls)):
+                    responses.append(executor.submit(downloader.download, url, output_path))
+                for response in concurrent.futures.as_completed(responses):
+                    self._downloaded_count += 1
+                    self.progress.update_value(self._downloaded_count)
+                    self.progress.set_info(self._get_bulk_progress_info(download_dict))
+                executor.shutdown(wait=True)
+            except KeyboardInterrupt:
+                downloader.close()
+                self.progress.stop()
+                Printer.warning(f"{os.linesep}Keyboard interrupt detected. Cleaning up...")
+                executor.shutdown(wait=False, cancel_futures=True)
+        self.progress.stop()
+        self._print_report()
+
+    def _configure_progress(self):
+        self.progress.info_separator_renderer = self._info_separator_renderer
+        self.progress.info_text_renderer = self._info_text_renderer
+        self.progress.label_renderer = self._label_renderer
+        self.progress.percentage_renderer = self._percentage_renderer
+        self.progress.progress_bar_renderer = self._progress_bar_renderer
+        self.progress.spinner_renderer = self._spinner_renderer
+        self.progress.label = "Downloading: "
+
+    @staticmethod
+    def _get_basic_colored_text(text: str, percentage: float):
+        if percentage < 15:
+            return Printer.format_hex(text, '#FF0D0D')
+        elif percentage < 30:
+            return Printer.format_hex(text, '#FF4E11')
+        elif percentage < 45:
+            return Printer.format_hex(text, '#FF8E15')
+        elif percentage < 60:
+            return Printer.format_hex(text, '#FAB733')
+        elif percentage < 75:
+            return Printer.format_hex(text, '#ACB334')
+        elif percentage < 90:
+            return Printer.format_hex(text, '#69B34C')
+        else:
+            return Printer.format_hex(text, '#0EB33B')
+
+    def _get_bulk_progress_info(self, download_dict: dict):
+        file_progress_text = f'[{self._downloaded_count}/{self._total_download_count}]'
+        size_text = FileUtils.get_readable_file_size(sum(download_dict.values()))
+        return f'{file_progress_text} [{size_text}]'
+
+    @staticmethod
+    def _info_separator_renderer(args: InfoSeparatorRendererArgs):
+        return Printer.format_hex(args.separator, '#FFCC75')
+
+    @staticmethod
+    def _info_text_renderer(args: InfoTextRendererArgs):
+        return Printer.format_hex(args.text, '#FFCC75')
+        # return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
+
+    @staticmethod
+    def _label_renderer(args: LabelRendererArgs):
+        if args.percentage < 100:
+            return Printer.format_hex(args.label, '#FFCC75')
+        return Printer.format_hex('Downloaded: ', '#0EB33B')
+
+    def _load_color_scheme(self):
+        file_path = os.path.join(os.path.dirname(__file__), "data", "colors.json")
+        with open(file_path, "r") as f:
+            self._file_color_scheme = json.load(f)
+
+    def _on_bulk_download_complete(self, event: DownloadCompleteEvent):
+        self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
+
+    def _on_bulk_download_failed(self, event: DownloadFailureEvent):
+        self._report_data.append(_DownloadReport("", 0, event.url))
+
+    def _on_bulk_download_progress(self, event: ProgressEventArgs, download_dict: dict):
+        download_dict[event.url] = event.downloaded
+        self.progress.set_info(self._get_bulk_progress_info(download_dict))
+
+    def _on_download_complete(self, event: DownloadCompleteEvent):
+        self.progress.update_value(event.filesize)
+        downloaded_info = FileUtils.get_readable_file_size(event.filesize)
+        filesize_info = FileUtils.get_readable_file_size(event.filesize)
+        info = f'[{downloaded_info}/{filesize_info}]'
+        self.progress.set_info(info)
+        time.sleep(0.5)
+        self.progress.stop()
+        self._report_data.append(_DownloadReport(event.filename, event.filesize, event.url))
+
+    def _on_download_failure(self, event: DownloadFailureEvent):
+        if isinstance(event.exception, KeyboardInterrupt):
+            Printer.warning("Download has been cancelled by user.")
+            print(os.linesep)
+        if self.progress:
+            self.progress.terminate()
+        self._report_data.append(_DownloadReport("", 0, event.url))
+
+    def _on_download_progress(self, event: ProgressEventArgs):
+        self.progress.update_value(event.downloaded)
+        downloaded_info = FileUtils.get_readable_file_size(event.downloaded)
+        filesize_info = FileUtils.get_readable_file_size(event.filesize)
+        info = f'[{downloaded_info}/{filesize_info}]'
+        self.progress.set_info(info)
+
+    def _on_download_start(self, event: DownloadStartEvent, filepath: list[str]):
+        self.progress = Progress(start=0, end=event.filesize, value=0)
+        self._configure_progress()
+        self.progress.start()
+        filepath.append(event.filepath)
+
+    @staticmethod
+    def _percentage_renderer(args: PercentageRendererArgs):
+        return DownloaderTool._get_basic_colored_text("{:.2f}%".format(args.percentage), args.percentage)
+
+    def _print_report(self):
+        success_data = [report for report in self._report_data if report.filesize > 0]
+        failed_data = [report for report in self._report_data if report.filesize == 0]
+        row_index = 1
+        success_grid_data = []
+        for report in success_data:
+            filename, ext = os.path.splitext(report.filename)
+            success_grid_data.append(
+                [row_index, report.filename, ext[1:], FileUtils.get_readable_file_size(report.filesize)])
+            row_index += 1
+
+        failed_grid_data = []
+        for report in failed_data:
+            failed_grid_data.append([row_index, report.url, "", 'Failed'])
+            row_index += 1
+
+        grid_columns: list[ColumnSettings] = [
+            ColumnSettings(title='#', alignment=Alignment.RIGHT,
+                           renderer=lambda x: Printer.format_hex(x.cell, '#FFCC75')),
+            ColumnSettings(title='Filename/URL', renderer=self._report_grid_file_column_cell_renderer),
+            ColumnSettings(title='Type', alignment=Alignment.RIGHT,
+                           renderer=self._report_grid_file_type_column_cell_renderer),
+            ColumnSettings(title='Filesize/Status', alignment=Alignment.RIGHT,
+                           renderer=lambda x: Printer.format_hex(x.cell, '#FF0000')
+                           if x.cell == 'Failed' else self._report_grid_cell_renderer(x))
+        ]
+        grid = Grid(grid_columns, success_grid_data + failed_grid_data)
+        grid.border_style = BorderStyle.SINGLE
+        grid.border_color = '#FFCC75'
+        grid.cell_renderer = self._report_grid_cell_renderer
+        print(os.linesep)
+        grid.print()
+
+    @staticmethod
+    def _progress_bar_renderer(args: ProgressBarRendererArgs):
+        return DownloaderTool._get_basic_colored_text(args.text, args.percentage)
+
+    @staticmethod
+    def _report_grid_cell_renderer(args: CellRendererArgs):
+        if args.cell.endswith("KB"):
+            return Printer.format_hex(args.cell, '#00a9ff')
+        if args.cell.endswith("MB"):
+            return Printer.format_hex(args.cell, '#d2309a')
+        if args.is_header:
+            return Printer.format_hex(args.cell, '#FFCC75')
+        return args.cell
+
+    def _report_grid_file_column_cell_renderer(self, args: CellRendererArgs):
+        if args.is_header:
+            return Printer.format_hex(args.cell, '#FFCC75')
+        file, ext = os.path.splitext(args.cell)
+        color = self._file_color_scheme.get(ext[1:], '#FFFFFF')
+        return Printer.format_hex(args.cell, color)
+
+    def _report_grid_file_type_column_cell_renderer(self, args: CellRendererArgs):
+        if args.is_header:
+            return Printer.format_hex(args.cell, '#FFCC75')
+        color = self._file_color_scheme.get(args.cell, '#FFFFFF')
+        return Printer.format_hex(args.cell, color)
+
+    @staticmethod
+    def _spinner_renderer(args: SpinnerRendererArgs):
+        return DownloaderTool._get_basic_colored_text(args.spinner, args.percentage)
```

### Comparing `mizue-0.2.0/mizue/printer/grid/border_character_codes.py` & `mizue-0.2.1/mizue/printer/grid/border_character_codes.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from typing import Final
-from abc import ABC
-
-
-class BorderCharacterCodes(ABC):
-    class Double(ABC):
-        TOPLEFT: Final[str] = u'\u2554'  # 0xC9 -> BOX DRAWINGS DOUBLE DOWN AND RIGHT
-        TOPRIGHT: Final[str] = u'\u2557'  # 0xBB -> BOX DRAWINGS DOUBLE DOWN AND LEFT
-        BOTTOMLEFT: Final[str] = u'\u255a'  # 0xC8 -> BOX DRAWINGS DOUBLE UP AND RIGHT
-        BOTTOMRIGHT: Final[str] = u'\u255d'  # 0xBC -> BOX DRAWINGS DOUBLE UP AND LEFT
-        TOPMIDDLE: Final[str] = u'\u2566'  # 0xCB -> BOX DRAWINGS DOUBLE DOWN AND HORIZONTAL
-        BOTTOMMIDDLE: Final[str] = u'\u2569'  # 0xCA -> BOX DRAWINGS DOUBLE UP AND HORIZONTAL
-        LEFTMIDDLE: Final[str] = u'\u2560'  # 0xCC -> BOX DRAWINGS DOUBLE VERTICAL AND RIGHT
-        RIGHTMIDDLE: Final[str] = u'\u2563'  # 0xB9 -> BOX DRAWINGS DOUBLE VERTICAL AND LEFT
-        MIDDLEMIDDLE: Final[str] = u'\u256c'  # 0xCE -> BOX DRAWINGS DOUBLE VERTICAL AND HORIZONTAL
-        HORIZONTAL: Final[str] = u'\u2550'  # 0xCD -> BOX DRAWINGS DOUBLE HORIZONTAL
-        VERTICAL: Final[str] = u'\u2551'  # 0xBA -> BOX DRAWINGS DOUBLE VERTICAL
-
-    class Single(ABC):
-        TOPLEFT: Final[str] = u'\u250c'  # 0xDA -> BOX DRAWINGS LIGHT DOWN AND RIGHT
-        TOPRIGHT: Final[str] = u'\u2510'  # 0xBF -> BOX DRAWINGS LIGHT DOWN AND LEFT
-        BOTTOMLEFT: Final[str] = u'\u2514'  # 0xC0 -> BOX DRAWINGS LIGHT UP AND RIGHT
-        BOTTOMRIGHT: Final[str] = u'\u2518'  # 0xD9 -> BOX DRAWINGS LIGHT UP AND LEFT
-        TOPMIDDLE: Final[str] = u'\u252c'  # 0xC2 -> BOX DRAWINGS LIGHT DOWN AND HORIZONTAL
-        BOTTOMMIDDLE: Final[str] = u'\u2534'  # 0xC1 -> BOX DRAWINGS LIGHT UP AND HORIZONTAL
-        LEFTMIDDLE: Final[str]= u'\u251c'  # 0xC3 -> BOX DRAWINGS LIGHT VERTICAL AND RIGHT
-        RIGHTMIDDLE: Final[str] = u'\u2524'  # 0xB4 -> BOX DRAWINGS LIGHT VERTICAL AND LEFT
-        MIDDLEMIDDLE: Final[str] = u'\u253c'  # 0xC5 -> BOX DRAWINGS LIGHT VERTICAL AND HORIZONTAL
-        HORIZONTAL: Final[str] = u'\u2500'  # 0xC4 -> BOX DRAWINGS LIGHT HORIZONTAL
-        VERTICAL: Final[str] = u'\u2502'  # 0xB3 -> BOX DRAWINGS LIGHT VERTICAL
-
-    class Basic(ABC):
-        TOPLEFT: Final[str] = "+"
-        TOPRIGHT: Final[str] = "+"
-        BOTTOMLEFT: Final[str] = "+"
-        BOTTOMRIGHT: Final[str] = "+"
-        TOPMIDDLE: Final[str] = "+"
-        BOTTOMMIDDLE: Final[str] = "+"
-        LEFTMIDDLE: Final[str] = "+"
-        RIGHTMIDDLE: Final[str] = "+"
-        MIDDLEMIDDLE: Final[str] = "+"
-        HORIZONTAL: Final[str] = "-"
-        VERTICAL: Final[str] = "|"
-
-    class Empty(ABC):
-        TOPLEFT: Final[str] = ""
-        TOPRIGHT: Final[str] = ""
-        BOTTOMLEFT: Final[str] = ""
-        BOTTOMRIGHT: Final[str] = ""
-        TOPMIDDLE: Final[str] = ""
-        BOTTOMMIDDLE: Final[str] = ""
-        LEFTMIDDLE: Final[str] = ""
-        RIGHTMIDDLE: Final[str] = ""
-        MIDDLEMIDDLE: Final[str] = ""
-        HORIZONTAL: Final[str] = ""
-        VERTICAL: Final[str] = ""
+from typing import Final
+from abc import ABC
+
+
+class BorderCharacterCodes(ABC):
+    class Double(ABC):
+        TOPLEFT: Final[str] = u'\u2554'  # 0xC9 -> BOX DRAWINGS DOUBLE DOWN AND RIGHT
+        TOPRIGHT: Final[str] = u'\u2557'  # 0xBB -> BOX DRAWINGS DOUBLE DOWN AND LEFT
+        BOTTOMLEFT: Final[str] = u'\u255a'  # 0xC8 -> BOX DRAWINGS DOUBLE UP AND RIGHT
+        BOTTOMRIGHT: Final[str] = u'\u255d'  # 0xBC -> BOX DRAWINGS DOUBLE UP AND LEFT
+        TOPMIDDLE: Final[str] = u'\u2566'  # 0xCB -> BOX DRAWINGS DOUBLE DOWN AND HORIZONTAL
+        BOTTOMMIDDLE: Final[str] = u'\u2569'  # 0xCA -> BOX DRAWINGS DOUBLE UP AND HORIZONTAL
+        LEFTMIDDLE: Final[str] = u'\u2560'  # 0xCC -> BOX DRAWINGS DOUBLE VERTICAL AND RIGHT
+        RIGHTMIDDLE: Final[str] = u'\u2563'  # 0xB9 -> BOX DRAWINGS DOUBLE VERTICAL AND LEFT
+        MIDDLEMIDDLE: Final[str] = u'\u256c'  # 0xCE -> BOX DRAWINGS DOUBLE VERTICAL AND HORIZONTAL
+        HORIZONTAL: Final[str] = u'\u2550'  # 0xCD -> BOX DRAWINGS DOUBLE HORIZONTAL
+        VERTICAL: Final[str] = u'\u2551'  # 0xBA -> BOX DRAWINGS DOUBLE VERTICAL
+
+    class Single(ABC):
+        TOPLEFT: Final[str] = u'\u250c'  # 0xDA -> BOX DRAWINGS LIGHT DOWN AND RIGHT
+        TOPRIGHT: Final[str] = u'\u2510'  # 0xBF -> BOX DRAWINGS LIGHT DOWN AND LEFT
+        BOTTOMLEFT: Final[str] = u'\u2514'  # 0xC0 -> BOX DRAWINGS LIGHT UP AND RIGHT
+        BOTTOMRIGHT: Final[str] = u'\u2518'  # 0xD9 -> BOX DRAWINGS LIGHT UP AND LEFT
+        TOPMIDDLE: Final[str] = u'\u252c'  # 0xC2 -> BOX DRAWINGS LIGHT DOWN AND HORIZONTAL
+        BOTTOMMIDDLE: Final[str] = u'\u2534'  # 0xC1 -> BOX DRAWINGS LIGHT UP AND HORIZONTAL
+        LEFTMIDDLE: Final[str]= u'\u251c'  # 0xC3 -> BOX DRAWINGS LIGHT VERTICAL AND RIGHT
+        RIGHTMIDDLE: Final[str] = u'\u2524'  # 0xB4 -> BOX DRAWINGS LIGHT VERTICAL AND LEFT
+        MIDDLEMIDDLE: Final[str] = u'\u253c'  # 0xC5 -> BOX DRAWINGS LIGHT VERTICAL AND HORIZONTAL
+        HORIZONTAL: Final[str] = u'\u2500'  # 0xC4 -> BOX DRAWINGS LIGHT HORIZONTAL
+        VERTICAL: Final[str] = u'\u2502'  # 0xB3 -> BOX DRAWINGS LIGHT VERTICAL
+
+    class Basic(ABC):
+        TOPLEFT: Final[str] = "+"
+        TOPRIGHT: Final[str] = "+"
+        BOTTOMLEFT: Final[str] = "+"
+        BOTTOMRIGHT: Final[str] = "+"
+        TOPMIDDLE: Final[str] = "+"
+        BOTTOMMIDDLE: Final[str] = "+"
+        LEFTMIDDLE: Final[str] = "+"
+        RIGHTMIDDLE: Final[str] = "+"
+        MIDDLEMIDDLE: Final[str] = "+"
+        HORIZONTAL: Final[str] = "-"
+        VERTICAL: Final[str] = "|"
+
+    class Empty(ABC):
+        TOPLEFT: Final[str] = ""
+        TOPRIGHT: Final[str] = ""
+        BOTTOMLEFT: Final[str] = ""
+        BOTTOMRIGHT: Final[str] = ""
+        TOPMIDDLE: Final[str] = ""
+        BOTTOMMIDDLE: Final[str] = ""
+        LEFTMIDDLE: Final[str] = ""
+        RIGHTMIDDLE: Final[str] = ""
+        MIDDLEMIDDLE: Final[str] = ""
+        HORIZONTAL: Final[str] = ""
+        VERTICAL: Final[str] = ""
```

### Comparing `mizue-0.2.0/mizue/printer/grid/column.py` & `mizue-0.2.1/mizue/printer/grid/column.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from mizue.printer.grid import ColumnSettings, Alignment
-
-
-class Column:
-    def __init__(self, settings: ColumnSettings):
-        self.alignment = settings["alignment"] if "alignment" in settings else Alignment.LEFT
-        self.index: int = 0
-        self.renderer = settings["renderer"] if "renderer" in settings else None
-        self.title = settings["title"] if "title" in settings else ""
-        self.width = settings["width"] if "width" in settings else None
-        if self.width is not None and self.width <= 0:
-            raise ValueError("The column width must be greater than zero")
+from mizue.printer.grid import ColumnSettings, Alignment
+
+
+class Column:
+    def __init__(self, settings: ColumnSettings):
+        self.alignment = settings["alignment"] if "alignment" in settings else Alignment.LEFT
+        self.index: int = 0
+        self.renderer = settings["renderer"] if "renderer" in settings else None
+        self.title = settings["title"] if "title" in settings else ""
+        self.width = settings["width"] if "width" in settings else None
+        if self.width is not None and self.width <= 0:
+            raise ValueError("The column width must be greater than zero")
```

### Comparing `mizue-0.2.0/mizue/printer/grid/grid.py` & `mizue-0.2.1/mizue/printer/grid/grid.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,292 +1,292 @@
-import os
-import re
-from math import ceil, floor
-from typing import Callable
-
-from wcwidth import wcswidth, wcwidth
-
-from mizue.printer import Printer
-from mizue.util import Utility
-from .alignment import Alignment
-from .border_character_codes import BorderCharacterCodes
-from .border_style import BorderStyle
-from .cell_renderer_args import CellRendererArgs
-from .column import Column
-from .column_settings import ColumnSettings
-from .row_border_position import RowBorderPosition
-
-
-class Grid:
-    def __init__(self, columns: list[ColumnSettings], data: list[list[str]]):
-        self.border_color = None
-        self.border_style = BorderStyle.BASIC
-        self.cell_renderer: Callable[[CellRendererArgs], str] = lambda args: Grid._get_default_cell_renderer(args)
-        self.columns = []
-        self.data = data
-        self._prepare_columns(columns)
-
-    def print(self) -> None:
-        """Print the grid"""
-        print(self._buffer())
-
-    def _buffer(self) -> str:
-        buffer = [self._create_row_border(RowBorderPosition.TOP), os.linesep]
-        title_list = [column.title for column in self.columns]
-        buffer.append(self._create_row(title_list, True))
-        buffer.append(os.linesep)
-        buffer.append(self._create_row_border(RowBorderPosition.MIDDLE))
-        buffer.append(os.linesep)
-        for row in self.data:
-            buffer.append(self._create_row(row, False))
-            buffer.append(os.linesep)
-        buffer.append(self._create_row_border(RowBorderPosition.BOTTOM))
-        return "".join(buffer)
-
-    def _create_row(self, row: list[str], is_header_row: bool) -> str:
-        border_style = self._get_border_style()
-        row_buffer = []
-        for index, cell_value in enumerate(row):
-            cell = str(cell_value)
-            column = self.columns[index]
-
-            renderer = self._get_cell_renderer(column)
-            if renderer is not None:
-                rendered_cell = renderer(CellRendererArgs(cell=cell, index=index, is_header=is_header_row,
-                                                          width=column.width))
-
-                rendered_cell = self._format_cell_with_colors(rendered_cell, column.width)
-            else:
-                rendered_cell = self._format_cell_with_colors(cell, column.width)
-
-            border = Printer.format_hex(border_style.VERTICAL, self.border_color) \
-                if self.border_color else border_style.VERTICAL
-            if index == 0:
-                row_buffer.append(f"{border}")
-
-            row_buffer.append(" ")
-            row_buffer.append(self._get_left_cell_space(column, self._get_raw_cell_text_after_rendering(rendered_cell)))
-            row_buffer.append(rendered_cell)
-            row_buffer.append(
-                self._get_right_cell_space(column, self._get_raw_cell_text_after_rendering(rendered_cell)))
-            row_buffer.append(" ")
-            row_buffer.append(border)
-        return "".join(row_buffer)
-
-    def _create_row_border(self, position):
-        dash_list = []
-        border_style = self._get_border_style()
-        if position is RowBorderPosition.TOP:
-            left = border_style.TOPLEFT
-            middle = border_style.TOPMIDDLE
-            right = border_style.TOPRIGHT
-        elif position is RowBorderPosition.BOTTOM:
-            left = border_style.BOTTOMLEFT
-            middle = border_style.BOTTOMMIDDLE
-            right = border_style.BOTTOMRIGHT
-        else:
-            left = border_style.LEFTMIDDLE
-            middle = border_style.MIDDLEMIDDLE
-            right = border_style.RIGHTMIDDLE
-        dash_list.append(left)
-        for index, max_length in enumerate(list(map(lambda column: column.width, self.columns))):
-            dash_list.append("".join([border_style.HORIZONTAL] * (max_length + 2)))
-            if index != len(self.columns) - 1:
-                dash_list.append(middle)
-        dash_list.append(right)
-        return Printer.format_hex("".join(dash_list), self.border_color) if self.border_color else "".join(dash_list)
-
-    def _find_max_cell_width(self, column: Column) -> int:
-        max_width = len(column.title)
-        for row in self.data:
-            cell = str(row[column.index])
-            length = 0
-            for char in str(cell):
-                if Grid._is_wide_char(char):
-                    length += 2
-                else:
-                    length += 1
-            length = length + 1 if Grid._has_variation_selector(cell) else length
-            max_width = max(max_width, length)
-        return max_width
-
-    def _format_cell_with_colors(self, rendered_cell: str, column_width: int) -> str:
-        color_parts = self._split_text_into_color_parts(rendered_cell)
-        if len(color_parts) == 0:
-            return self._format_long_cell(rendered_cell, column_width)
-        else:
-            processed_width = 0
-            formatted_parts = []
-            for color_part in color_parts:
-                text = color_part[1]
-                text_width = wcswidth(text)
-                if processed_width + text_width <= column_width:
-                    formatted_text = f"{color_part[0]}{text}{color_part[2]}"
-                    formatted_parts.append(formatted_text)
-                    processed_width += text_width
-                    if processed_width == column_width:
-                        break
-                else:
-                    visible_text = self._format_long_cell(text, column_width - processed_width)
-                    formatted_text = f"{color_part[0]}{visible_text}{color_part[2]}"
-                    formatted_parts.append(formatted_text)
-                    break
-            return "".join(formatted_parts)
-
-    @staticmethod
-    def _format_long_cell(cell: str, col_width: int) -> str:
-        if col_width <= 3:
-            if col_width == 1:
-                return cell[0] if wcwidth(cell[0]) == 1 else "…"
-            if col_width == 2:
-                if len(cell) == 1:
-                    return cell[0] if wcwidth(cell[0]) == 1 else "…"
-                return cell[0] + cell[1] if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 1 else "…"
-            if col_width == 3:
-                if wcwidth(cell[0]) == 2:
-                    return cell[0] + "…"
-                if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 1:
-                    return cell[0] + cell[1] + "…"
-                if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 2:
-                    return "…"
-                if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 0:  # symbol + variation selector
-                    return cell[0] + "…"
-
-        text_width = 0
-        text_length = 0
-        for char in cell:
-            text_length += 1
-            if Grid._is_wide_char(char):
-                text_width += 2
-            else:
-                text_width += 1
-            if text_width == col_width - 3 or text_width == col_width - 2:
-                break
-
-        has_any_wide_char = any([True for char in cell if Grid._is_wide_char(char)])
-        if not has_any_wide_char:
-            if len(cell) <= col_width:
-                return cell
-            return cell[:col_width - 1] + "…"
-        else:
-            first_part = cell[:text_length]
-            first_part_original = cell[:text_length]
-            first_part_terminal_width = Grid._get_terminal_width_of_cell(first_part)
-            full_width = Grid._get_terminal_width_of_cell(cell)
-            while first_part_terminal_width > col_width - 1:
-                first_part = first_part[:-1]
-                first_part_terminal_width = Grid._get_terminal_width_of_cell(first_part)
-            return first_part + "…" \
-                if len(first_part) < len(first_part_original) or full_width > col_width \
-                else first_part
-
-    def _get_border_style(self):
-        if self.border_style == BorderStyle.SINGLE:
-            return BorderCharacterCodes.Single
-        if self.border_style == BorderStyle.DOUBLE:
-            return BorderCharacterCodes.Double
-        if self.border_style == BorderStyle.BASIC:
-            return BorderCharacterCodes.Basic
-        if self.border_style == BorderStyle.EMPTY:
-            return BorderCharacterCodes.Empty
-        return BorderCharacterCodes.Basic
-
-    def _get_cell_renderer(self, column: Column):
-        if column.renderer:
-            return column.renderer
-        return self.cell_renderer
-
-    @staticmethod
-    def _get_default_cell_renderer(args: CellRendererArgs) -> str:
-        if args.is_header:
-            return Printer.format_hex(args.cell, '#FFCC75')
-        return args.cell
-
-    @staticmethod
-    def _get_left_cell_space(column: Column, cell: str) -> str:
-        cell_terminal_width = Grid._get_terminal_width_of_cell(cell)
-        if column.alignment == Alignment.RIGHT:
-            return "".join([" "] * (column.width - cell_terminal_width))
-        elif column.alignment == Alignment.CENTER:
-            return "".join([" "] * int(floor((column.width - cell_terminal_width) / 2)))
-        return ""
-
-    @staticmethod
-    def _get_raw_cell_text_after_rendering(rendered_cell: str) -> str:
-        # remove all the color codes and other formatting codes, also remove ansi escape codes
-        return re.sub(r"\x1b\[[0-9;]*m", "", rendered_cell)
-
-    @staticmethod
-    def _get_right_cell_space(column: Column, cell: str) -> str:
-        cell_terminal_width = Grid._get_terminal_width_of_cell(cell)
-        if column.alignment == Alignment.LEFT:
-            return "".join([" "] * (column.width - cell_terminal_width))
-        elif column.alignment == Alignment.CENTER:
-            return "".join([" "] * int(ceil((column.width - cell_terminal_width) / 2)))
-        return ""
-
-    @staticmethod
-    def _get_terminal_width_of_cell(text):
-        return sum([2 if wcswidth(char) == 2 else 1 for char in text])
-
-    @staticmethod
-    def _get_visible_text(text: str, max_width: int) -> str:
-        current_width = 0
-        for ch in text:
-            if Grid._is_wide_char(ch):
-                current_width += 2
-            else:
-                current_width += 1
-            if current_width > max_width:
-                return text[:text.index(ch)]
-        return text
-
-    @staticmethod
-    def _has_variation_selector(text: str) -> bool:
-        return any(Grid._is_variation_selector(c) for c in text)
-
-    @staticmethod
-    def _is_variation_selector(char: str) -> bool:
-        return 0xFE00 <= ord(char) <= 0xFE0F
-
-    @staticmethod
-    def _is_wide_char(char: str) -> bool:
-        return wcswidth(char) > 1
-
-    def _prepare_columns(self, column_data: list[ColumnSettings]):
-        columns: list[Column] = []
-        for i, column_setting in enumerate(column_data):
-            column = Column(settings=column_setting)
-            column.index = i
-            column.width = column_setting["width"] if "width" in column_setting else self._find_max_cell_width(column)
-            columns.append(column)
-        self.columns = columns
-        self._resize_columns_to_fit()
-
-    def _resize_columns_to_fit2(self):
-        terminal_width = Utility.get_terminal_width()
-        total_column_width = sum(column.width for column in self.columns)
-        if total_column_width > terminal_width:
-            for cx in range(0, len(self.columns)):
-                self.columns[cx].width = int((terminal_width * self.columns[cx].width) / total_column_width) - 4
-
-    def _resize_columns_to_fit(self):
-        terminal_width = Utility.get_terminal_width()
-        new_column_width = int(terminal_width / len(self.columns))
-        long_columns = [column for column in self.columns if column.width >= new_column_width]
-
-        remaining_width = 0
-        for column in self.columns:
-            if column.width > new_column_width:
-                column.width = new_column_width
-            else:
-                remaining_width += (new_column_width - column.width - 4 * len(self.columns))
-
-        padding = int(remaining_width / len(long_columns)) if len(long_columns) > 0 else 0
-        for column in long_columns:
-            column.width += padding
-
-    @staticmethod
-    def _split_text_into_color_parts(text: str) -> list[tuple[str, str, str]]:
-        matcher = re.compile(r"(\x1b\[[0-9;]*m)(.*?)(\x1b\[00m)")
-        groups = matcher.findall(text)
-        return groups if groups else []
+import os
+import re
+from math import ceil, floor
+from typing import Callable
+
+from wcwidth import wcswidth, wcwidth
+
+from mizue.printer import Printer
+from mizue.util import Utility
+from .alignment import Alignment
+from .border_character_codes import BorderCharacterCodes
+from .border_style import BorderStyle
+from .cell_renderer_args import CellRendererArgs
+from .column import Column
+from .column_settings import ColumnSettings
+from .row_border_position import RowBorderPosition
+
+
+class Grid:
+    def __init__(self, columns: list[ColumnSettings], data: list[list[str]]):
+        self.border_color = None
+        self.border_style = BorderStyle.BASIC
+        self.cell_renderer: Callable[[CellRendererArgs], str] = lambda args: Grid._get_default_cell_renderer(args)
+        self.columns = []
+        self.data = data
+        self._prepare_columns(columns)
+
+    def print(self) -> None:
+        """Print the grid"""
+        print(self._buffer())
+
+    def _buffer(self) -> str:
+        buffer = [self._create_row_border(RowBorderPosition.TOP), os.linesep]
+        title_list = [column.title for column in self.columns]
+        buffer.append(self._create_row(title_list, True))
+        buffer.append(os.linesep)
+        buffer.append(self._create_row_border(RowBorderPosition.MIDDLE))
+        buffer.append(os.linesep)
+        for row in self.data:
+            buffer.append(self._create_row(row, False))
+            buffer.append(os.linesep)
+        buffer.append(self._create_row_border(RowBorderPosition.BOTTOM))
+        return "".join(buffer)
+
+    def _create_row(self, row: list[str], is_header_row: bool) -> str:
+        border_style = self._get_border_style()
+        row_buffer = []
+        for index, cell_value in enumerate(row):
+            cell = str(cell_value)
+            column = self.columns[index]
+
+            renderer = self._get_cell_renderer(column)
+            if renderer is not None:
+                rendered_cell = renderer(CellRendererArgs(cell=cell, index=index, is_header=is_header_row,
+                                                          width=column.width))
+
+                rendered_cell = self._format_cell_with_colors(rendered_cell, column.width)
+            else:
+                rendered_cell = self._format_cell_with_colors(cell, column.width)
+
+            border = Printer.format_hex(border_style.VERTICAL, self.border_color) \
+                if self.border_color else border_style.VERTICAL
+            if index == 0:
+                row_buffer.append(f"{border}")
+
+            row_buffer.append(" ")
+            row_buffer.append(self._get_left_cell_space(column, self._get_raw_cell_text_after_rendering(rendered_cell)))
+            row_buffer.append(rendered_cell)
+            row_buffer.append(
+                self._get_right_cell_space(column, self._get_raw_cell_text_after_rendering(rendered_cell)))
+            row_buffer.append(" ")
+            row_buffer.append(border)
+        return "".join(row_buffer)
+
+    def _create_row_border(self, position):
+        dash_list = []
+        border_style = self._get_border_style()
+        if position is RowBorderPosition.TOP:
+            left = border_style.TOPLEFT
+            middle = border_style.TOPMIDDLE
+            right = border_style.TOPRIGHT
+        elif position is RowBorderPosition.BOTTOM:
+            left = border_style.BOTTOMLEFT
+            middle = border_style.BOTTOMMIDDLE
+            right = border_style.BOTTOMRIGHT
+        else:
+            left = border_style.LEFTMIDDLE
+            middle = border_style.MIDDLEMIDDLE
+            right = border_style.RIGHTMIDDLE
+        dash_list.append(left)
+        for index, max_length in enumerate(list(map(lambda column: column.width, self.columns))):
+            dash_list.append("".join([border_style.HORIZONTAL] * (max_length + 2)))
+            if index != len(self.columns) - 1:
+                dash_list.append(middle)
+        dash_list.append(right)
+        return Printer.format_hex("".join(dash_list), self.border_color) if self.border_color else "".join(dash_list)
+
+    def _find_max_cell_width(self, column: Column) -> int:
+        max_width = len(column.title)
+        for row in self.data:
+            cell = str(row[column.index])
+            length = 0
+            for char in str(cell):
+                if Grid._is_wide_char(char):
+                    length += 2
+                else:
+                    length += 1
+            length = length + 1 if Grid._has_variation_selector(cell) else length
+            max_width = max(max_width, length)
+        return max_width
+
+    def _format_cell_with_colors(self, rendered_cell: str, column_width: int) -> str:
+        color_parts = self._split_text_into_color_parts(rendered_cell)
+        if len(color_parts) == 0:
+            return self._format_long_cell(rendered_cell, column_width)
+        else:
+            processed_width = 0
+            formatted_parts = []
+            for color_part in color_parts:
+                text = color_part[1]
+                text_width = wcswidth(text)
+                if processed_width + text_width <= column_width:
+                    formatted_text = f"{color_part[0]}{text}{color_part[2]}"
+                    formatted_parts.append(formatted_text)
+                    processed_width += text_width
+                    if processed_width == column_width:
+                        break
+                else:
+                    visible_text = self._format_long_cell(text, column_width - processed_width)
+                    formatted_text = f"{color_part[0]}{visible_text}{color_part[2]}"
+                    formatted_parts.append(formatted_text)
+                    break
+            return "".join(formatted_parts)
+
+    @staticmethod
+    def _format_long_cell(cell: str, col_width: int) -> str:
+        if col_width <= 3:
+            if col_width == 1:
+                return cell[0] if wcwidth(cell[0]) == 1 else "…"
+            if col_width == 2:
+                if len(cell) == 1:
+                    return cell[0] if wcwidth(cell[0]) == 1 else "…"
+                return cell[0] + cell[1] if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 1 else "…"
+            if col_width == 3:
+                if wcwidth(cell[0]) == 2:
+                    return cell[0] + "…"
+                if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 1:
+                    return cell[0] + cell[1] + "…"
+                if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 2:
+                    return "…"
+                if wcwidth(cell[0]) == 1 and wcwidth(cell[1]) == 0:  # symbol + variation selector
+                    return cell[0] + "…"
+
+        text_width = 0
+        text_length = 0
+        for char in cell:
+            text_length += 1
+            if Grid._is_wide_char(char):
+                text_width += 2
+            else:
+                text_width += 1
+            if text_width == col_width - 3 or text_width == col_width - 2:
+                break
+
+        has_any_wide_char = any([True for char in cell if Grid._is_wide_char(char)])
+        if not has_any_wide_char:
+            if len(cell) <= col_width:
+                return cell
+            return cell[:col_width - 1] + "…"
+        else:
+            first_part = cell[:text_length]
+            first_part_original = cell[:text_length]
+            first_part_terminal_width = Grid._get_terminal_width_of_cell(first_part)
+            full_width = Grid._get_terminal_width_of_cell(cell)
+            while first_part_terminal_width > col_width - 1:
+                first_part = first_part[:-1]
+                first_part_terminal_width = Grid._get_terminal_width_of_cell(first_part)
+            return first_part + "…" \
+                if len(first_part) < len(first_part_original) or full_width > col_width \
+                else first_part
+
+    def _get_border_style(self):
+        if self.border_style == BorderStyle.SINGLE:
+            return BorderCharacterCodes.Single
+        if self.border_style == BorderStyle.DOUBLE:
+            return BorderCharacterCodes.Double
+        if self.border_style == BorderStyle.BASIC:
+            return BorderCharacterCodes.Basic
+        if self.border_style == BorderStyle.EMPTY:
+            return BorderCharacterCodes.Empty
+        return BorderCharacterCodes.Basic
+
+    def _get_cell_renderer(self, column: Column):
+        if column.renderer:
+            return column.renderer
+        return self.cell_renderer
+
+    @staticmethod
+    def _get_default_cell_renderer(args: CellRendererArgs) -> str:
+        if args.is_header:
+            return Printer.format_hex(args.cell, '#FFCC75')
+        return args.cell
+
+    @staticmethod
+    def _get_left_cell_space(column: Column, cell: str) -> str:
+        cell_terminal_width = Grid._get_terminal_width_of_cell(cell)
+        if column.alignment == Alignment.RIGHT:
+            return "".join([" "] * (column.width - cell_terminal_width))
+        elif column.alignment == Alignment.CENTER:
+            return "".join([" "] * int(floor((column.width - cell_terminal_width) / 2)))
+        return ""
+
+    @staticmethod
+    def _get_raw_cell_text_after_rendering(rendered_cell: str) -> str:
+        # remove all the color codes and other formatting codes, also remove ansi escape codes
+        return re.sub(r"\x1b\[[0-9;]*m", "", rendered_cell)
+
+    @staticmethod
+    def _get_right_cell_space(column: Column, cell: str) -> str:
+        cell_terminal_width = Grid._get_terminal_width_of_cell(cell)
+        if column.alignment == Alignment.LEFT:
+            return "".join([" "] * (column.width - cell_terminal_width))
+        elif column.alignment == Alignment.CENTER:
+            return "".join([" "] * int(ceil((column.width - cell_terminal_width) / 2)))
+        return ""
+
+    @staticmethod
+    def _get_terminal_width_of_cell(text):
+        return sum([2 if wcswidth(char) == 2 else 1 for char in text])
+
+    @staticmethod
+    def _get_visible_text(text: str, max_width: int) -> str:
+        current_width = 0
+        for ch in text:
+            if Grid._is_wide_char(ch):
+                current_width += 2
+            else:
+                current_width += 1
+            if current_width > max_width:
+                return text[:text.index(ch)]
+        return text
+
+    @staticmethod
+    def _has_variation_selector(text: str) -> bool:
+        return any(Grid._is_variation_selector(c) for c in text)
+
+    @staticmethod
+    def _is_variation_selector(char: str) -> bool:
+        return 0xFE00 <= ord(char) <= 0xFE0F
+
+    @staticmethod
+    def _is_wide_char(char: str) -> bool:
+        return wcswidth(char) > 1
+
+    def _prepare_columns(self, column_data: list[ColumnSettings]):
+        columns: list[Column] = []
+        for i, column_setting in enumerate(column_data):
+            column = Column(settings=column_setting)
+            column.index = i
+            column.width = column_setting["width"] if "width" in column_setting else self._find_max_cell_width(column)
+            columns.append(column)
+        self.columns = columns
+        self._resize_columns_to_fit()
+
+    def _resize_columns_to_fit2(self):
+        terminal_width = Utility.get_terminal_width()
+        total_column_width = sum(column.width for column in self.columns)
+        if total_column_width > terminal_width:
+            for cx in range(0, len(self.columns)):
+                self.columns[cx].width = int((terminal_width * self.columns[cx].width) / total_column_width) - 4
+
+    def _resize_columns_to_fit(self):
+        terminal_width = Utility.get_terminal_width()
+        new_column_width = int(terminal_width / len(self.columns))
+        long_columns = [column for column in self.columns if column.width >= new_column_width]
+
+        remaining_width = 0
+        for column in self.columns:
+            if column.width > new_column_width:
+                column.width = new_column_width
+            else:
+                remaining_width += (new_column_width - column.width - 4 * len(self.columns))
+
+        padding = int(remaining_width / len(long_columns)) if len(long_columns) > 0 else 0
+        for column in long_columns:
+            column.width += padding
+
+    @staticmethod
+    def _split_text_into_color_parts(text: str) -> list[tuple[str, str, str]]:
+        matcher = re.compile(r"(\x1b\[[0-9;]*m)(.*?)(\x1b\[00m)")
+        groups = matcher.findall(text)
+        return groups if groups else []
```

### Comparing `mizue-0.2.0/mizue/printer/printer.py` & `mizue-0.2.1/mizue/printer/printer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-import typing
-import re
-
-from .terminal_colors import TerminalColors
-
-
-class Printer:
-    _newline: bool = True
-
-    @staticmethod
-    def apply_background(message, bg_color):
-        end_char = '' if Printer._formatted(message) else TerminalColors.END_CHAR
-        msg = str.format("{}{}{}", bg_color, message, end_char)
-        return msg
-
-    @staticmethod
-    def format(text: str, color: str = None, bold: bool = False, underlined: bool = False) -> str:
-        """Formats a string with the specified color, boldness, and underlining."""
-        color = color if color is not None else ''
-        bolded = TerminalColors.BOLD if bold else ''
-        underlined = TerminalColors.UNDERLINE if underlined else ''
-        end = TerminalColors.END_CHAR
-        return f'{color}{bolded}{underlined}{text}{end}'
-
-    @staticmethod
-    def format_hex(text: str, text_hex: str, bg_hex: str | None = None,
-                   bold: bool = False, underlined: bool = False) -> str:
-        """Formats a string with the specified color, boldness, and underlining."""
-        if bg_hex is None:
-            text_rgb: tuple = Printer.hex_to_rgb(text_hex)
-            return Printer.format_rgb(text, text_rgb, None, bold, underlined)
-        else:
-            text_rgb: tuple = Printer.hex_to_rgb(text_hex)
-            bg_rgb: tuple = Printer.hex_to_rgb(bg_hex)
-            return Printer.format_rgb(text, text_rgb, bg_rgb, bold, underlined)
-
-    @staticmethod
-    def format_rgb(text: str, text_rgb: tuple[int, int, int], bg_rgb: tuple[int, int, int] | None = None,
-                   bold: bool = False, underlined: bool = False) -> str:
-        """Formats a string with the specified color, boldness, and underlining."""
-        bolded = TerminalColors.BOLD if bold else ''
-        underlined = TerminalColors.UNDERLINE if underlined else ''
-        end = TerminalColors.END_CHAR
-        if bg_rgb is None:
-            return f'\033[38;2;{text_rgb[0]};{text_rgb[1]};{text_rgb[2]}m{bolded}{underlined}{text}{end}'
-        else:
-            return f'\033[38;2;{text_rgb[0]};{text_rgb[1]};{text_rgb[2]}m' \
-                   f'\033[48;2;{bg_rgb[0]};{bg_rgb[1]};{bg_rgb[2]}m{bolded}{underlined}{text}{end}'
-
-    @staticmethod
-    def error(text: str, bold: bool = False, underlined: bool = False) -> None:
-        """Prints an error message to the console."""
-        Printer.print_hex(text, TerminalColors.ERROR, bold=bold, underlined=underlined)
-
-    @staticmethod
-    def get_color_string(color: str | tuple[int, int, int]):
-        if isinstance(color, tuple):
-            return Printer.rgb_to_hex(color)
-        else:
-            return color
-
-    @staticmethod
-    def hex_to_rgb(hex_color: str) -> tuple[int, int, int]:
-        """Converts a hex string to an RGB tuple."""
-        hex_without_hash = hex_color.replace('#', '') if hex_color.startswith('#') else hex_color
-        return typing.cast(tuple[int, int, int], tuple(int(hex_without_hash[i:i + 2], 16) for i in (0, 2, 4)))
-
-    @staticmethod
-    def info(text: str, bold: bool = False, underlined: bool = False) -> None:
-        """Prints an info message to the console."""
-        Printer.print_hex(text, TerminalColors.INFO, bold=bold, underlined=underlined)
-
-    @staticmethod
-    def prevent_newline(prevent: bool = True) -> None:
-        """Prevents a newline from being printed to the console."""
-        if Printer._newline != prevent:
-            return
-        Printer._newline = not prevent
-        if Printer._newline:
-            print()
-
-    @staticmethod
-    def print_hex(text: str, text_hex: str, bg_hex: str | None = None,
-                  bold: bool = False, underlined: bool = False) -> None:
-        """Prints a message to the console."""
-        rgb: tuple = Printer.hex_to_rgb(text_hex)
-        bg_rgb: tuple = Printer.hex_to_rgb(bg_hex) if bg_hex is not None else None
-        Printer.print_rgb(text, rgb, bg_rgb, bold, underlined)
-
-    @staticmethod
-    def print_rgb(text: str, text_rgb: tuple[int, int, int], bg_rgb: tuple[int, int, int] | None = None,
-                  bold: bool = False, underlined: bool = False) -> None:
-        """Prints a message to the console."""
-        formatted_text = text if Printer._formatted(text) else Printer.format_rgb(text, text_rgb, bg_rgb, bold,
-                                                                                  underlined)
-        print(formatted_text, end='\n' if Printer._newline else '', flush=True)
-
-    @staticmethod
-    def rgb_to_hex(rgb: tuple[int, int, int]) -> str:
-        """Converts an RGB tuple to a hex string."""
-        return f'#{rgb[0]:02x}{rgb[1]:02x}{rgb[2]:02x}'
-
-    @staticmethod
-    def short_hex_to_long_hex(hex_color: str) -> str:
-        """Converts a short hex color to a long hex color."""
-        hex_without_hash = hex_color.replace('#', '') if hex_color.startswith('#') else hex_color
-        return f'#{hex_without_hash[0]}{hex_without_hash[0]}{hex_without_hash[1]}{hex_without_hash[1]}' \
-               f'{hex_without_hash[2]}{hex_without_hash[2]}'
-
-    @staticmethod
-    def success(text: str, bold: bool = False, underlined: bool = False) -> None:
-        """Prints a success message to the console."""
-        Printer.print_hex(text, TerminalColors.SUCCESS, bold=bold, underlined=underlined)
-
-    @staticmethod
-    def strip_ansi(text: str) -> str:
-        """Strips ANSI escape sequences from a string."""
-        return re.sub(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])', '', text)
-
-    @staticmethod
-    def strip_colors(text: str) -> str:
-        stripped_text = re.sub(r'\x1b[\[\d;]+m', '', text)
-        return Printer.strip_ansi(stripped_text)
-
-    @staticmethod
-    def warning(text: str, bold: bool = False, underlined: bool = False) -> None:
-        """Prints a warning message to the console."""
-        Printer.print_hex(text, TerminalColors.WARNING, bold=bold, underlined=underlined)
-
-    @staticmethod
-    def _formatted(text: str) -> bool:
-        return str(text).endswith(TerminalColors.END_CHAR)
+import typing
+import re
+
+from .terminal_colors import TerminalColors
+
+
+class Printer:
+    _newline: bool = True
+
+    @staticmethod
+    def apply_background(message, bg_color):
+        end_char = '' if Printer._formatted(message) else TerminalColors.END_CHAR
+        msg = str.format("{}{}{}", bg_color, message, end_char)
+        return msg
+
+    @staticmethod
+    def format(text: str, color: str = None, bold: bool = False, underlined: bool = False) -> str:
+        """Formats a string with the specified color, boldness, and underlining."""
+        color = color if color is not None else ''
+        bolded = TerminalColors.BOLD if bold else ''
+        underlined = TerminalColors.UNDERLINE if underlined else ''
+        end = TerminalColors.END_CHAR
+        return f'{color}{bolded}{underlined}{text}{end}'
+
+    @staticmethod
+    def format_hex(text: str, text_hex: str, bg_hex: str | None = None,
+                   bold: bool = False, underlined: bool = False) -> str:
+        """Formats a string with the specified color, boldness, and underlining."""
+        if bg_hex is None:
+            text_rgb: tuple = Printer.hex_to_rgb(text_hex)
+            return Printer.format_rgb(text, text_rgb, None, bold, underlined)
+        else:
+            text_rgb: tuple = Printer.hex_to_rgb(text_hex)
+            bg_rgb: tuple = Printer.hex_to_rgb(bg_hex)
+            return Printer.format_rgb(text, text_rgb, bg_rgb, bold, underlined)
+
+    @staticmethod
+    def format_rgb(text: str, text_rgb: tuple[int, int, int], bg_rgb: tuple[int, int, int] | None = None,
+                   bold: bool = False, underlined: bool = False) -> str:
+        """Formats a string with the specified color, boldness, and underlining."""
+        bolded = TerminalColors.BOLD if bold else ''
+        underlined = TerminalColors.UNDERLINE if underlined else ''
+        end = TerminalColors.END_CHAR
+        if bg_rgb is None:
+            return f'\033[38;2;{text_rgb[0]};{text_rgb[1]};{text_rgb[2]}m{bolded}{underlined}{text}{end}'
+        else:
+            return f'\033[38;2;{text_rgb[0]};{text_rgb[1]};{text_rgb[2]}m' \
+                   f'\033[48;2;{bg_rgb[0]};{bg_rgb[1]};{bg_rgb[2]}m{bolded}{underlined}{text}{end}'
+
+    @staticmethod
+    def error(text: str, bold: bool = False, underlined: bool = False) -> None:
+        """Prints an error message to the console."""
+        Printer.print_hex(text, TerminalColors.ERROR, bold=bold, underlined=underlined)
+
+    @staticmethod
+    def get_color_string(color: str | tuple[int, int, int]):
+        if isinstance(color, tuple):
+            return Printer.rgb_to_hex(color)
+        else:
+            return color
+
+    @staticmethod
+    def hex_to_rgb(hex_color: str) -> tuple[int, int, int]:
+        """Converts a hex string to an RGB tuple."""
+        hex_without_hash = hex_color.replace('#', '') if hex_color.startswith('#') else hex_color
+        return typing.cast(tuple[int, int, int], tuple(int(hex_without_hash[i:i + 2], 16) for i in (0, 2, 4)))
+
+    @staticmethod
+    def info(text: str, bold: bool = False, underlined: bool = False) -> None:
+        """Prints an info message to the console."""
+        Printer.print_hex(text, TerminalColors.INFO, bold=bold, underlined=underlined)
+
+    @staticmethod
+    def prevent_newline(prevent: bool = True) -> None:
+        """Prevents a newline from being printed to the console."""
+        if Printer._newline != prevent:
+            return
+        Printer._newline = not prevent
+        if Printer._newline:
+            print()
+
+    @staticmethod
+    def print_hex(text: str, text_hex: str, bg_hex: str | None = None,
+                  bold: bool = False, underlined: bool = False) -> None:
+        """Prints a message to the console."""
+        rgb: tuple = Printer.hex_to_rgb(text_hex)
+        bg_rgb: tuple = Printer.hex_to_rgb(bg_hex) if bg_hex is not None else None
+        Printer.print_rgb(text, rgb, bg_rgb, bold, underlined)
+
+    @staticmethod
+    def print_rgb(text: str, text_rgb: tuple[int, int, int], bg_rgb: tuple[int, int, int] | None = None,
+                  bold: bool = False, underlined: bool = False) -> None:
+        """Prints a message to the console."""
+        formatted_text = text if Printer._formatted(text) else Printer.format_rgb(text, text_rgb, bg_rgb, bold,
+                                                                                  underlined)
+        print(formatted_text, end='\n' if Printer._newline else '', flush=True)
+
+    @staticmethod
+    def rgb_to_hex(rgb: tuple[int, int, int]) -> str:
+        """Converts an RGB tuple to a hex string."""
+        return f'#{rgb[0]:02x}{rgb[1]:02x}{rgb[2]:02x}'
+
+    @staticmethod
+    def short_hex_to_long_hex(hex_color: str) -> str:
+        """Converts a short hex color to a long hex color."""
+        hex_without_hash = hex_color.replace('#', '') if hex_color.startswith('#') else hex_color
+        return f'#{hex_without_hash[0]}{hex_without_hash[0]}{hex_without_hash[1]}{hex_without_hash[1]}' \
+               f'{hex_without_hash[2]}{hex_without_hash[2]}'
+
+    @staticmethod
+    def success(text: str, bold: bool = False, underlined: bool = False) -> None:
+        """Prints a success message to the console."""
+        Printer.print_hex(text, TerminalColors.SUCCESS, bold=bold, underlined=underlined)
+
+    @staticmethod
+    def strip_ansi(text: str) -> str:
+        """Strips ANSI escape sequences from a string."""
+        return re.sub(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])', '', text)
+
+    @staticmethod
+    def strip_colors(text: str) -> str:
+        stripped_text = re.sub(r'\x1b[\[\d;]+m', '', text)
+        return Printer.strip_ansi(stripped_text)
+
+    @staticmethod
+    def warning(text: str, bold: bool = False, underlined: bool = False) -> None:
+        """Prints a warning message to the console."""
+        Printer.print_hex(text, TerminalColors.WARNING, bold=bold, underlined=underlined)
+
+    @staticmethod
+    def _formatted(text: str) -> bool:
+        return str(text).endswith(TerminalColors.END_CHAR)
```

### Comparing `mizue-0.2.0/mizue/progress/progress.py` & `mizue-0.2.1/mizue/progress/progress.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import sys
-from time import sleep
-
-from mizue.printer import Printer
-from mizue.util import Utility
-from mizue.util.stoppable_thread import StoppableThread
-from .progress_renderer_args import ProgressBarRendererArgs, SpinnerRendererArgs, LabelRendererArgs, \
-    InfoSeparatorRendererArgs, InfoTextRendererArgs, PercentageRendererArgs
-
-
-class Progress:
-    def __init__(self, start: int = 0, end: int = 100, value: int = 0):
-        self._active = False
-        self._end = end
-        self._info_text = ""
-        self._interval = 0.1
-        self._spinner = [
-            "▹▹▹▹▹",
-            "▸▹▹▹▹",
-            "▹▸▹▹▹",
-            "▹▹▸▹▹",
-            "▹▹▹▸▹",
-            "▹▹▹▹▸"
-        ]
-        self._spinner_end_symbol = "⠿"
-        self._spinner_index = 0
-        self._start = start
-        self._thread = None
-        self._value = value
-        self._width = 10
-
-        self.info_separator = " | "
-        self.info_separator_renderer = lambda args: self._info_separator_renderer(
-            args.separator)  # InfoSeparatorRendererArgs
-        self.info_text_renderer = lambda args: self._info_text_renderer(args.text)  # InfoTextRendererArgs
-        self.label = ""
-        self.label_renderer = lambda args: args.label  # LabelRendererArgs
-        self.percentage_renderer = lambda args: "{:.2f}%".format(args.percentage)  # PercentageRendererArgs
-        self.spinner_renderer = lambda args: args.spinner  # SpinnerRendererArgs
-        self.progress_bar_renderer = lambda args: self._progress_bar_renderer()  # ProgressBarRendererArgs
-
-    def set_end_value(self, end: int) -> None:
-        """Update the maximum value of the progress bar"""
-        self._end = end
-
-    def set_info(self, info: str) -> None:
-        """Set the info text to be displayed after the progress bar"""
-        self._info_text = info
-
-    def set_update_interval(self, interval: float) -> None:
-        """Set the update interval of the progress bar"""
-        self._interval = interval
-
-    def start(self) -> None:
-        """Start the progress bar"""
-        Utility.hide_cursor()
-        self._thread = StoppableThread(target=self._print, args=())
-        self._active = True
-        self._thread.start()
-
-    def stop(self) -> None:
-        """Stop the progress bar"""
-        sleep(1)
-        self._active = False
-        self._spinner_index = 0
-        self._thread.join()
-        Utility.show_cursor()
-
-    def terminate(self) -> None:
-        """Terminate the progress bar.
-            This method is generally used when the progress bar is needed to be stopped (e.g. on Ctrl+C)"""
-        sleep(1)
-        self._active = False
-        self._spinner_index = 0
-        self._thread.stop()
-        self._thread.join()
-        Utility.show_cursor()
-
-    def update_value(self, value: int) -> None:
-        """Update the value of the progress bar"""
-        self._value = value
-
-    def _get_bar_full_width(self) -> int:
-        percentage = self._value * 100 / self._end
-        bar_width = int(percentage * self._width / 100)
-        return bar_width
-
-    def _get_progress_text(self) -> str:
-        percentage_value = self._value * 100 / self._end
-        percentage = self.percentage_renderer(PercentageRendererArgs(percentage_value, self._value))
-        spinner_symbol = self.spinner_renderer(SpinnerRendererArgs(
-            spinner=self._spinner[self._spinner_index % len(self._spinner)],
-            value=self._value,
-            percentage=percentage_value
-        ))
-        bar_string = self._progress_bar_renderer()
-        bar = self.progress_bar_renderer(ProgressBarRendererArgs(
-            percentage=percentage_value,
-            text=bar_string,
-            value=self._value,
-            width=self._get_bar_full_width()
-        ))
-        label = self.label_renderer(LabelRendererArgs(
-            label=self.label,
-            value=self._value,
-            percentage=percentage_value
-        ))
-        separator = self.info_separator_renderer(InfoSeparatorRendererArgs(
-            separator=self.info_separator,
-            value=self._value,
-            percentage=percentage_value
-        ))
-        info_text = self.info_text_renderer(InfoTextRendererArgs(
-            text=self._info_text,
-            value=self._value,
-            percentage=percentage_value
-        ))
-        progress_text = str.format("{}{} {} {}{}{}", label, bar, spinner_symbol, percentage, separator,
-                                   info_text)
-        text_length = len(Printer.strip_colors(progress_text))
-        if text_length > Utility.get_terminal_width():
-            progress_text = str.format("{}{} {} {}{}", label, bar, spinner_symbol, percentage, '')
-            if text_length > Utility.get_terminal_width():
-                progress_text = str.format("{}{} {} {}{}", '', bar, spinner_symbol, percentage, '')
-        return progress_text
-
-    def _info_separator_renderer(self, info_text: str) -> str:
-        return self.info_separator if len(info_text) > 0 else ""
-
-    @staticmethod
-    def _info_text_renderer(info_text: str) -> str:
-        return info_text
-
-    def _print(self) -> None:
-        while self._active:
-            progress_text = self._get_progress_text()
-            self._spinner_index += 1
-            sys.stdout.write(
-                u"\u001b[K")  # Erase from cursor to end of line [http://matthieu.benoit.free.fr/68hc11/vt100.htm]
-            sys.stdout.write(
-                u"\u001b[1000D" + progress_text)  # Move terminal cursor 1000 characters left (go to start of line)
-            sys.stdout.flush()
-            sleep(self._interval)
-
-    def _progress_bar_renderer(self):
-        bar_start = "⟪"
-        bar_end = "⟫"
-        width = self._get_bar_full_width()
-        bar = bar_start + "◆" * int(width) + " " * int((self._width - width)) + bar_end
-        return bar
+import sys
+from time import sleep
+
+from mizue.printer import Printer
+from mizue.util import Utility
+from mizue.util.stoppable_thread import StoppableThread
+from .progress_renderer_args import ProgressBarRendererArgs, SpinnerRendererArgs, LabelRendererArgs, \
+    InfoSeparatorRendererArgs, InfoTextRendererArgs, PercentageRendererArgs
+
+
+class Progress:
+    def __init__(self, start: int = 0, end: int = 100, value: int = 0):
+        self._active = False
+        self._end = end
+        self._info_text = ""
+        self._interval = 0.1
+        self._spinner = [
+            "▹▹▹▹▹",
+            "▸▹▹▹▹",
+            "▹▸▹▹▹",
+            "▹▹▸▹▹",
+            "▹▹▹▸▹",
+            "▹▹▹▹▸"
+        ]
+        self._spinner_end_symbol = "⠿"
+        self._spinner_index = 0
+        self._start = start
+        self._thread = None
+        self._value = value
+        self._width = 10
+
+        self.info_separator = " | "
+        self.info_separator_renderer = lambda args: self._info_separator_renderer(
+            args.separator)  # InfoSeparatorRendererArgs
+        self.info_text_renderer = lambda args: self._info_text_renderer(args.text)  # InfoTextRendererArgs
+        self.label = ""
+        self.label_renderer = lambda args: args.label  # LabelRendererArgs
+        self.percentage_renderer = lambda args: "{:.2f}%".format(args.percentage)  # PercentageRendererArgs
+        self.spinner_renderer = lambda args: args.spinner  # SpinnerRendererArgs
+        self.progress_bar_renderer = lambda args: self._progress_bar_renderer()  # ProgressBarRendererArgs
+
+    def set_end_value(self, end: int) -> None:
+        """Update the maximum value of the progress bar"""
+        self._end = end
+
+    def set_info(self, info: str) -> None:
+        """Set the info text to be displayed after the progress bar"""
+        self._info_text = info
+
+    def set_update_interval(self, interval: float) -> None:
+        """Set the update interval of the progress bar"""
+        self._interval = interval
+
+    def start(self) -> None:
+        """Start the progress bar"""
+        Utility.hide_cursor()
+        self._thread = StoppableThread(target=self._print, args=())
+        self._active = True
+        self._thread.start()
+
+    def stop(self) -> None:
+        """Stop the progress bar"""
+        sleep(1)
+        self._active = False
+        self._spinner_index = 0
+        self._thread.join()
+        Utility.show_cursor()
+
+    def terminate(self) -> None:
+        """Terminate the progress bar.
+            This method is generally used when the progress bar is needed to be stopped (e.g. on Ctrl+C)"""
+        sleep(1)
+        self._active = False
+        self._spinner_index = 0
+        self._thread.stop()
+        self._thread.join()
+        Utility.show_cursor()
+
+    def update_value(self, value: int) -> None:
+        """Update the value of the progress bar"""
+        self._value = value
+
+    def _get_bar_full_width(self) -> int:
+        percentage = self._value * 100 / self._end
+        bar_width = int(percentage * self._width / 100)
+        return bar_width
+
+    def _get_progress_text(self) -> str:
+        percentage_value = self._value * 100 / self._end
+        percentage = self.percentage_renderer(PercentageRendererArgs(percentage_value, self._value))
+        spinner_symbol = self.spinner_renderer(SpinnerRendererArgs(
+            spinner=self._spinner[self._spinner_index % len(self._spinner)],
+            value=self._value,
+            percentage=percentage_value
+        ))
+        bar_string = self._progress_bar_renderer()
+        bar = self.progress_bar_renderer(ProgressBarRendererArgs(
+            percentage=percentage_value,
+            text=bar_string,
+            value=self._value,
+            width=self._get_bar_full_width()
+        ))
+        label = self.label_renderer(LabelRendererArgs(
+            label=self.label,
+            value=self._value,
+            percentage=percentage_value
+        ))
+        separator = self.info_separator_renderer(InfoSeparatorRendererArgs(
+            separator=self.info_separator,
+            value=self._value,
+            percentage=percentage_value
+        ))
+        info_text = self.info_text_renderer(InfoTextRendererArgs(
+            text=self._info_text,
+            value=self._value,
+            percentage=percentage_value
+        ))
+        progress_text = str.format("{}{} {} {}{}{}", label, bar, spinner_symbol, percentage, separator,
+                                   info_text)
+        text_length = len(Printer.strip_colors(progress_text))
+        if text_length > Utility.get_terminal_width():
+            progress_text = str.format("{}{} {} {}{}", label, bar, spinner_symbol, percentage, '')
+            if text_length > Utility.get_terminal_width():
+                progress_text = str.format("{}{} {} {}{}", '', bar, spinner_symbol, percentage, '')
+        return progress_text
+
+    def _info_separator_renderer(self, info_text: str) -> str:
+        return self.info_separator if len(info_text) > 0 else ""
+
+    @staticmethod
+    def _info_text_renderer(info_text: str) -> str:
+        return info_text
+
+    def _print(self) -> None:
+        while self._active:
+            progress_text = self._get_progress_text()
+            self._spinner_index += 1
+            sys.stdout.write(
+                u"\u001b[K")  # Erase from cursor to end of line [http://matthieu.benoit.free.fr/68hc11/vt100.htm]
+            sys.stdout.write(
+                u"\u001b[1000D" + progress_text)  # Move terminal cursor 1000 characters left (go to start of line)
+            sys.stdout.flush()
+            sleep(self._interval)
+
+    def _progress_bar_renderer(self):
+        bar_start = "⟪"
+        bar_end = "⟫"
+        width = self._get_bar_full_width()
+        bar = bar_start + "◆" * int(width) + " " * int((self._width - width)) + bar_end
+        return bar
```

### Comparing `mizue-0.2.0/mizue/progress/spinner.py` & `mizue-0.2.1/mizue/progress/spinner.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from sys import stdout
-from time import sleep
-from mizue.util import Utility
-from threading import Thread
-
-
-class Spinner:
-    def __init__(self):
-        self._symbols = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
-        self._spinning = False
-        self._thread = None
-
-    def _spin(self) -> None:
-        index = 0
-        while self._spinning:
-            spin_symbol = self._symbols[index % len(self._symbols)]
-            stdout.write(u"\u001b[1D" + spin_symbol)
-            stdout.flush()
-            index += 1
-            sleep(0.1)
-
-    def start(self) -> None:
-        Utility.hide_cursor()
-        self._spinning = True
-        self._thread = Thread(target=self._spin)
-        self._thread.start()
-
-    def stop(self) -> None:
-        sleep(0.3)
-        self._spinning = False
-        self._thread.join()
-        stdout.write(u"\u001b[1D")
-        stdout.flush()
+from sys import stdout
+from time import sleep
+from mizue.util import Utility
+from threading import Thread
+
+
+class Spinner:
+    def __init__(self):
+        self._symbols = ["⠋", "⠙", "⠹", "⠸", "⠼", "⠴", "⠦", "⠧", "⠇", "⠏"]
+        self._spinning = False
+        self._thread = None
+
+    def _spin(self) -> None:
+        index = 0
+        while self._spinning:
+            spin_symbol = self._symbols[index % len(self._symbols)]
+            stdout.write(u"\u001b[1D" + spin_symbol)
+            stdout.flush()
+            index += 1
+            sleep(0.1)
+
+    def start(self) -> None:
+        Utility.hide_cursor()
+        self._spinning = True
+        self._thread = Thread(target=self._spin)
+        self._thread.start()
+
+    def stop(self) -> None:
+        sleep(0.3)
+        self._spinning = False
+        self._thread.join()
+        stdout.write(u"\u001b[1D")
+        stdout.flush()
         Utility.show_cursor()
```

### Comparing `mizue-0.2.0/mizue/util/event_listener.py` & `mizue-0.2.1/mizue/util/event_listener.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from abc import ABC
-
-
-class EventListener(ABC):
-    """Abstract class for event listeners"""
-    _event_id_counter: int = 0
-    _events: dict[str, list[callable]] = {}
-    _event_id_map: dict[int, [str, callable]] = {}
-
-    def add_event(self, event: str, callback: callable) -> int:
-        """Add a callback to an event"""
-        if event not in self._events:
-            self._events[event] = []
-
-        event_id = self._event_id_counter
-        self._event_id_counter += 1
-        self._event_id_map[event_id] = [event, callback]
-        self._events[event].append(callback)
-        return event_id
-
-    def remove_event(self, event_id) -> None:
-        """Remove a callback from an event"""
-        if event_id in self._event_id_map:
-            event, callback = self._event_id_map[event_id]
-            self._events[event].remove(callback)
-            del self._event_id_map[event_id]
-
-    def _fire_event(self, event: str, *args, **kwargs) -> None:
-        """Fire an event"""
-        if event in self._events:
-            for callback in self._events[event]:
-                callback(*args, **kwargs)
+from abc import ABC
+
+
+class EventListener(ABC):
+    """Abstract class for event listeners"""
+    _event_id_counter: int = 0
+    _events: dict[str, list[callable]] = {}
+    _event_id_map: dict[int, [str, callable]] = {}
+
+    def add_event(self, event: str, callback: callable) -> int:
+        """Add a callback to an event"""
+        if event not in self._events:
+            self._events[event] = []
+
+        event_id = self._event_id_counter
+        self._event_id_counter += 1
+        self._event_id_map[event_id] = [event, callback]
+        self._events[event].append(callback)
+        return event_id
+
+    def remove_event(self, event_id) -> None:
+        """Remove a callback from an event"""
+        if event_id in self._event_id_map:
+            event, callback = self._event_id_map[event_id]
+            self._events[event].remove(callback)
+            del self._event_id_map[event_id]
+
+    def _fire_event(self, event: str, *args, **kwargs) -> None:
+        """Fire an event"""
+        if event in self._events:
+            for callback in self._events[event]:
+                callback(*args, **kwargs)
```

### Comparing `mizue-0.2.0/mizue/util/signal_handler.py` & `mizue-0.2.1/mizue/util/signal_handler.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from signal import signal, Signals
-
-
-class SignalHandler:
-    def __init__(self, signal: Signals, callback: callable):
-        self._callback = callback
-        self._signal = signal
-        self._signal_received = False
-
-    def __call__(self, *args, **kwargs):
-        self._signal_received = True
-        self._signal_handler()
-
-    def is_signal_received(self):
-        return self._signal_received
-
-    def _signal_callback(self):
-        self._signal_received = True
-        self._callback()
-
-    def _signal_handler(self):
-        signal(self._signal, self._signal_callback)
+from signal import signal, Signals
+
+
+class SignalHandler:
+    def __init__(self, signal: Signals, callback: callable):
+        self._callback = callback
+        self._signal = signal
+        self._signal_received = False
+
+    def __call__(self, *args, **kwargs):
+        self._signal_received = True
+        self._signal_handler()
+
+    def is_signal_received(self):
+        return self._signal_received
+
+    def _signal_callback(self):
+        self._signal_received = True
+        self._callback()
+
+    def _signal_handler(self):
+        signal(self._signal, self._signal_callback)
```

### Comparing `mizue-0.2.0/mizue/util/utility.py` & `mizue-0.2.1/mizue/util/utility.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import ctypes
-import shutil
-
-
-class _CursorInfo(ctypes.Structure):
-    _fields_ = [("size", ctypes.c_int), ("visible", ctypes.c_byte)]
-
-
-class Utility:
-
-    @staticmethod
-    def get_terminal_size() -> tuple[int, int]:
-        """Returns the size of the terminal."""
-        return shutil.get_terminal_size()
-
-    @staticmethod
-    def get_terminal_width() -> int:
-        """Returns the width of the terminal."""
-        return Utility.get_terminal_size()[0]
-
-    @staticmethod
-    def get_terminal_height() -> int:
-        """Returns the height of the terminal."""
-        return Utility.get_terminal_size()[1]
-
-    @staticmethod
-    def hide_cursor() -> None:
-        """Hides the cursor."""
-        info = _CursorInfo()
-        info.visible = False
-        ctypes.windll.kernel32.SetConsoleCursorInfo(ctypes.windll.kernel32.GetStdHandle(-11), ctypes.byref(info))
-
-    @staticmethod
-    def is_elevated() -> bool:
-        """Returns whether the current process is elevated."""
-        return ctypes.windll.shell32.IsUserAnAdmin() != 0
-
-    @staticmethod
-    def is_caps_lock_on() -> bool:
-        """Returns whether the caps lock key is on."""
-        return ctypes.windll.user32.GetKeyState(0x14) != 0
-
-    @staticmethod
-    def show_cursor() -> None:
-        """Shows the cursor."""
-        info = _CursorInfo()
-        info.visible = True
-        ctypes.windll.kernel32.SetConsoleCursorInfo(ctypes.windll.kernel32.GetStdHandle(-11), ctypes.byref(info))
+import ctypes
+import shutil
+
+
+class _CursorInfo(ctypes.Structure):
+    _fields_ = [("size", ctypes.c_int), ("visible", ctypes.c_byte)]
+
+
+class Utility:
+
+    @staticmethod
+    def get_terminal_size() -> tuple[int, int]:
+        """Returns the size of the terminal."""
+        return shutil.get_terminal_size()
+
+    @staticmethod
+    def get_terminal_width() -> int:
+        """Returns the width of the terminal."""
+        return Utility.get_terminal_size()[0]
+
+    @staticmethod
+    def get_terminal_height() -> int:
+        """Returns the height of the terminal."""
+        return Utility.get_terminal_size()[1]
+
+    @staticmethod
+    def hide_cursor() -> None:
+        """Hides the cursor."""
+        info = _CursorInfo()
+        info.visible = False
+        ctypes.windll.kernel32.SetConsoleCursorInfo(ctypes.windll.kernel32.GetStdHandle(-11), ctypes.byref(info))
+
+    @staticmethod
+    def is_elevated() -> bool:
+        """Returns whether the current process is elevated."""
+        return ctypes.windll.shell32.IsUserAnAdmin() != 0
+
+    @staticmethod
+    def is_caps_lock_on() -> bool:
+        """Returns whether the caps lock key is on."""
+        return ctypes.windll.user32.GetKeyState(0x14) != 0
+
+    @staticmethod
+    def show_cursor() -> None:
+        """Shows the cursor."""
+        info = _CursorInfo()
+        info.visible = True
+        ctypes.windll.kernel32.SetConsoleCursorInfo(ctypes.windll.kernel32.GetStdHandle(-11), ctypes.byref(info))
```

### Comparing `mizue-0.2.0/mizue.egg-info/PKG-INFO` & `mizue-0.2.1/mizue.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1
-Name: mizue
-Version: 0.2.0
-Summary: A Python package for various utilities
-Author: Hoshilily
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A simple package containing various command-line utilities.
-
-## Installation
-
-```bash
-  pip install mizue
-```
-
-## Usage
-
-### Printer
-
-```python
-from mizue.printer import Printer, TerminalColors as Color
-
-Printer.print_ansi("Hello World!")
-Printer.print_ansi("Hello World!", Color.RED)
-Printer.print_ansi("Hello World!", Color.RED, bold=True, underlined=True)
-```
-The ``Printer`` class is a simple wrapper around the ``print`` function. It allows you to print colored text to the terminal. The ``TerminalColors`` class contains a list of colors that can be used with the ``Printer`` class.
-The ``Printer`` class also provides the following methods:
-```python
-from mizue.printer import Printer, TerminalColors as Color
-Printer.error("Hello World!")
-Printer.warning("Hello World!")
-Printer.success("Hello World!")
-Printer.info("Hello World!")
-```
-
-It is possible to prevent the new line character from being printed at the end of the line:
-
-```python
-from mizue.printer import Printer, TerminalColors as Color
-
-Printer.prevent_newline(True)
-Printer.print_ansi("Hello World!", Color.RED)
-```
+Metadata-Version: 2.1
+Name: mizue
+Version: 0.2.1
+Summary: A Python package for various utilities
+Author: Hoshilily
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A simple package containing various command-line utilities.
+
+## Installation
+
+```bash
+  pip install mizue
+```
+
+## Usage
+
+### Printer
+
+```python
+from mizue.printer import Printer, TerminalColors as Color
+
+Printer.print_ansi("Hello World!")
+Printer.print_ansi("Hello World!", Color.RED)
+Printer.print_ansi("Hello World!", Color.RED, bold=True, underlined=True)
+```
+The ``Printer`` class is a simple wrapper around the ``print`` function. It allows you to print colored text to the terminal. The ``TerminalColors`` class contains a list of colors that can be used with the ``Printer`` class.
+The ``Printer`` class also provides the following methods:
+```python
+from mizue.printer import Printer, TerminalColors as Color
+Printer.error("Hello World!")
+Printer.warning("Hello World!")
+Printer.success("Hello World!")
+Printer.info("Hello World!")
+```
+
+It is possible to prevent the new line character from being printed at the end of the line:
+
+```python
+from mizue.printer import Printer, TerminalColors as Color
+
+Printer.prevent_newline(True)
+Printer.print_ansi("Hello World!", Color.RED)
+```
```

### Comparing `mizue-0.2.0/mizue.egg-info/SOURCES.txt` & `mizue-0.2.1/mizue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mizue-0.2.0/setup.py` & `mizue-0.2.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup, find_packages
-from codecs import open
-from os import path
-
-here = path.abspath(path.dirname(__file__))
-
-# Get the long description from the README file
-with open(path.join(here, "README.md")) as f:
-    long_description = f.read()
-
-setup(
-    name="mizue",
-    version="0.2.0",
-    description="A Python package for various utilities",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="Hoshilily",
-    license="MIT",
-    classifiers=[
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3"
-    ],
-    packages=find_packages(),
-    package_data={
-        "mizue.network.downloader": ["data/*.json"],
-    },
-    install_requires=["wcwidth"],
-    include_package_data=True
-)
+from setuptools import setup, find_packages
+from codecs import open
+from os import path
+
+here = path.abspath(path.dirname(__file__))
+
+# Get the long description from the README file
+with open(path.join(here, "README.md")) as f:
+    long_description = f.read()
+
+setup(
+    name="mizue",
+    version="0.2.1",
+    description="A Python package for various utilities",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="Hoshilily",
+    license="MIT",
+    classifiers=[
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3"
+    ],
+    packages=find_packages(),
+    package_data={
+        "mizue.network.downloader": ["data/*.json"],
+    },
+    install_requires=["wcwidth"],
+    include_package_data=True
+)
```

