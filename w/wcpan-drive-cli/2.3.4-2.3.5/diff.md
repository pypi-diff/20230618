# Comparing `tmp/wcpan_drive_cli-2.3.4.tar.gz` & `tmp/wcpan_drive_cli-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcpan_drive_cli-2.3.4.tar", max compression
+gzip compressed data, was "wcpan_drive_cli-2.3.5.tar", max compression
```

## Comparing `wcpan_drive_cli-2.3.4.tar` & `wcpan_drive_cli-2.3.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1102 2020-11-10 04:14:30.070000 wcpan_drive_cli-2.3.4/LICENSE.txt
--rw-r--r--   0        0        0     1220 2022-05-05 22:26:44.644544 wcpan_drive_cli-2.3.4/README.md
--rw-r--r--   0        0        0      683 2023-06-18 01:31:15.239269 wcpan_drive_cli-2.3.4/pyproject.toml
--rw-r--r--   0        0        0       88 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.4/wcpan/drive/cli/__init__.py
--rw-r--r--   0        0        0       54 2023-03-11 16:11:59.229013 wcpan_drive_cli-2.3.4/wcpan/drive/cli/__main__.py
--rw-r--r--   0        0        0    15298 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.4/wcpan/drive/cli/interaction.py
--rw-r--r--   0        0        0    15417 2023-06-18 01:30:50.179269 wcpan_drive_cli-2.3.4/wcpan/drive/cli/main.py
--rw-r--r--   0        0        0    10555 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.4/wcpan/drive/cli/queue_.py
--rw-r--r--   0        0        0     4845 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.4/wcpan/drive/cli/util.py
--rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 wcpan_drive_cli-2.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1102 2020-11-10 04:14:30.070000 wcpan_drive_cli-2.3.5/LICENSE.txt
+-rw-r--r--   0        0        0     1220 2022-05-05 22:26:44.644544 wcpan_drive_cli-2.3.5/README.md
+-rw-r--r--   0        0        0      683 2023-06-18 01:39:09.799269 wcpan_drive_cli-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.5/wcpan/drive/cli/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-11 16:11:59.229013 wcpan_drive_cli-2.3.5/wcpan/drive/cli/__main__.py
+-rw-r--r--   0        0        0    15298 2023-03-05 01:26:15.360421 wcpan_drive_cli-2.3.5/wcpan/drive/cli/interaction.py
+-rw-r--r--   0        0        0    15417 2023-06-18 01:38:43.509269 wcpan_drive_cli-2.3.5/wcpan/drive/cli/main.py
+-rw-r--r--   0        0        0    10555 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.5/wcpan/drive/cli/queue_.py
+-rw-r--r--   0        0        0     4845 2023-06-18 01:26:17.519269 wcpan_drive_cli-2.3.5/wcpan/drive/cli/util.py
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 wcpan_drive_cli-2.3.5/PKG-INFO
```

### Comparing `wcpan_drive_cli-2.3.4/LICENSE.txt` & `wcpan_drive_cli-2.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.4/README.md` & `wcpan_drive_cli-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.4/pyproject.toml` & `wcpan_drive_cli-2.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wcpan-drive-cli"
-version = "2.3.4"
+version = "2.3.5"
 description = "command line tool for wcpan.drive"
 authors = ["Wei-Cheng Pan <legnaleurc@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "wcpan"}]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `wcpan_drive_cli-2.3.4/wcpan/drive/cli/interaction.py` & `wcpan_drive_cli-2.3.5/wcpan/drive/cli/interaction.py`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.4/wcpan/drive/cli/main.py` & `wcpan_drive_cli-2.3.5/wcpan/drive/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
 
 async def action_verify(factory: DriveFactory, args: argparse.Namespace) -> int:
     with create_executor() as pool:
         async with factory(pool=pool) as drive:
             node = await get_node_by_id_or_path(drive, args.id_or_path)
 
             queue_ = VerifyQueue(drive, pool, 1)
-            src_list = (pathlib.Path(local_path) for local_path in args.source)
+            src_list = [pathlib.Path(local_path) for local_path in args.source]
             await queue_.run(src_list, node)
 
     return 0
 
 
 async def action_doctor(factory: DriveFactory, args: argparse.Namespace) -> int:
     async with factory() as drive:
```

### Comparing `wcpan_drive_cli-2.3.4/wcpan/drive/cli/queue_.py` & `wcpan_drive_cli-2.3.5/wcpan/drive/cli/queue_.py`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.4/wcpan/drive/cli/util.py` & `wcpan_drive_cli-2.3.5/wcpan/drive/cli/util.py`

 * *Files identical despite different names*

### Comparing `wcpan_drive_cli-2.3.4/PKG-INFO` & `wcpan_drive_cli-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcpan-drive-cli
-Version: 2.3.4
+Version: 2.3.5
 Summary: command line tool for wcpan.drive
 License: MIT
 Author: Wei-Cheng Pan
 Author-email: legnaleurc@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

