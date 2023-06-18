# Comparing `tmp/wcpan_drive_cli-2.3.3.tar.gz` & `tmp/wcpan_drive_cli-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcpan_drive_cli-2.3.3.tar", max compression
+gzip compressed data, was "wcpan_drive_cli-2.3.4.tar", max compression
```

## Comparing `wcpan_drive_cli-2.3.3.tar` & `wcpan_drive_cli-2.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1102 2020-11-10 04:14:30.070000 wcpan_drive_cli-2.3.3/LICENSE.txt
--rw-r--r--   0        0        0     1220 2022-05-05 22:26:44.644544 wcpan_drive_cli-2.3.3/README.md
--rw-r--r--   0        0        0      683 2023-06-18 01:27:27.959269 wcpan_drive_cli-2.3.3/pyproject.toml
--rw-r--r--   0        0        0       88 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.3/wcpan/drive/cli/__init__.py
--rw-r--r--   0        0        0       54 2023-03-11 16:11:59.229013 wcpan_drive_cli-2.3.3/wcpan/drive/cli/__main__.py
--rw-r--r--   0        0        0    15298 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.3/wcpan/drive/cli/interaction.py
--rw-r--r--   0        0        0    15437 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.3/wcpan/drive/cli/main.py
--rw-r--r--   0        0        0    10555 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.3/wcpan/drive/cli/queue_.py
--rw-r--r--   0        0        0     4845 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.3/wcpan/drive/cli/util.py
--rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 wcpan_drive_cli-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2020-11-10 04:14:30.070000 wcpan_drive_cli-2.3.4/LICENSE.txt
+-rw-r--r--   0        0        0     1220 2022-05-05 22:26:44.644544 wcpan_drive_cli-2.3.4/README.md
+-rw-r--r--   0        0        0      683 2023-06-18 01:31:15.239269 wcpan_drive_cli-2.3.4/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.4/wcpan/drive/cli/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-11 16:11:59.229013 wcpan_drive_cli-2.3.4/wcpan/drive/cli/__main__.py
+-rw-r--r--   0        0        0    15298 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.4/wcpan/drive/cli/interaction.py
+-rw-r--r--   0        0        0    15417 2023-06-18 01:30:50.179269 wcpan_drive_cli-2.3.4/wcpan/drive/cli/main.py
+-rw-r--r--   0        0        0    10555 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.4/wcpan/drive/cli/queue_.py
+-rw-r--r--   0        0        0     4845 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.4/wcpan/drive/cli/util.py
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 wcpan_drive_cli-2.3.4/PKG-INFO
```

### Comparing `wcpan_drive_cli-2.3.3/LICENSE.txt` & `wcpan_drive_cli-2.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.3/README.md` & `wcpan_drive_cli-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.3/pyproject.toml` & `wcpan_drive_cli-2.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wcpan-drive-cli"
-version = "2.3.3"
+version = "2.3.4"
 description = "command line tool for wcpan.drive"
 authors = ["Wei-Cheng Pan <legnaleurc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "wcpan"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `wcpan_drive_cli-2.3.3/wcpan/drive/cli/interaction.py` & `wcpan_drive_cli-2.3.4/wcpan/drive/cli/interaction.py`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.3/wcpan/drive/cli/main.py` & `wcpan_drive_cli-2.3.4/wcpan/drive/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     get_utc_now,
     humanize,
     print_as_yaml,
     print_id_node_dict,
     require_authorized,
     trash_node,
     traverse_node,
-    UploadVerifier,
     wait_for_value,
 )
 from .interaction import interact
 
 
 def main(args: list[str] = None) -> int:
     if args is None:
```

### Comparing `wcpan_drive_cli-2.3.3/wcpan/drive/cli/queue_.py` & `wcpan_drive_cli-2.3.4/wcpan/drive/cli/queue_.py`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.3/wcpan/drive/cli/util.py` & `wcpan_drive_cli-2.3.4/wcpan/drive/cli/util.py`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.3/PKG-INFO` & `wcpan_drive_cli-2.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcpan-drive-cli
-Version: 2.3.3
+Version: 2.3.4
 Summary: command line tool for wcpan.drive
 License: MIT
 Author: Wei-Cheng Pan
 Author-email: legnaleurc@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

