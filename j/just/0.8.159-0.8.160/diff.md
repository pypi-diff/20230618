# Comparing `tmp/just-0.8.159.tar.gz` & `tmp/just-0.8.160.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just-0.8.159.tar", last modified: Tue Dec 13 03:06:23 2022, max compression
+gzip compressed data, was "just-0.8.160.tar", last modified: Sun Jun 18 16:51:57 2023, max compression
```

## Comparing `just-0.8.159.tar` & `just-0.8.160.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-13 03:06:23.201632 just-0.8.159/
--rw-r--r--   0 pascal    (1000) pascal    (1000)      148 2019-10-30 12:22:05.000000 just-0.8.159/.coveragerc
--rw-r--r--   0 pascal    (1000) pascal    (1000)      189 2019-10-30 12:22:05.000000 just-0.8.159/.gitignore
--rw-r--r--   0 pascal    (1000) pascal    (1000)      195 2019-10-30 12:22:05.000000 just-0.8.159/.travis.yml
--rw-r--r--   0 pascal    (1000) pascal    (1000)    34519 2019-10-30 12:22:05.000000 just-0.8.159/LICENSE
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2022-12-13 03:06:23.201632 just-0.8.159/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2791 2021-02-24 22:23:55.000000 just-0.8.159/README.md
--rw-r--r--   0 pascal    (1000) pascal    (1000)       60 2019-10-30 12:22:05.000000 just-0.8.159/README.rst
--rw-r--r--   0 pascal    (1000) pascal    (1000)      192 2019-10-30 12:22:05.000000 just-0.8.159/conftest.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      973 2022-12-11 15:47:37.000000 just-0.8.159/deploy.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-13 03:06:23.201632 just-0.8.159/just/
--rw-r--r--   0 pascal    (1000) pascal    (1000)      802 2022-12-13 03:06:21.000000 just-0.8.159/just/__init__.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      510 2019-10-31 14:56:25.000000 just-0.8.159/just/bytes.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      323 2020-05-07 22:19:36.000000 just-0.8.159/just/dir.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      240 2022-10-12 23:24:09.000000 just-0.8.159/just/dt.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     6707 2022-10-11 01:42:38.000000 just-0.8.159/just/forcedip.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      422 2020-09-14 22:28:41.000000 just-0.8.159/just/jpath.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2852 2022-11-14 11:53:48.000000 just-0.8.159/just/json_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      631 2019-10-30 12:22:05.000000 just-0.8.159/just/log.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      313 2019-10-30 12:22:05.000000 just-0.8.159/just/newl.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     4126 2022-10-15 12:24:04.000000 just-0.8.159/just/path_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2532 2022-10-12 23:42:19.000000 just-0.8.159/just/pattern.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      183 2019-10-30 12:22:05.000000 just-0.8.159/just/pickle_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     6541 2022-12-13 02:13:38.000000 just-0.8.159/just/read_write.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)    11513 2022-12-13 03:05:55.000000 just-0.8.159/just/requests_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2617 2022-10-11 02:05:39.000000 just-0.8.159/just/source_ip.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      177 2022-10-31 11:24:28.000000 just-0.8.159/just/toml_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      706 2020-01-15 22:53:45.000000 just-0.8.159/just/txt.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      198 2021-02-06 15:54:20.000000 just-0.8.159/just/yaml_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      693 2021-04-17 11:52:08.000000 just-0.8.159/just/zstd_.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-13 03:06:23.201632 just-0.8.159/just.egg-info/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2022-12-13 03:06:22.000000 just-0.8.159/just.egg-info/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)      651 2022-12-13 03:06:23.000000 just-0.8.159/just.egg-info/SOURCES.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2022-12-13 03:06:22.000000 just-0.8.159/just.egg-info/dependency_links.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)       45 2022-12-13 03:06:22.000000 just-0.8.159/just.egg-info/entry_points.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2019-10-30 12:22:52.000000 just-0.8.159/just.egg-info/not-zip-safe
--rw-r--r--   0 pascal    (1000) pascal    (1000)       59 2022-12-13 03:06:22.000000 just-0.8.159/just.egg-info/requires.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        5 2022-12-13 03:06:22.000000 just-0.8.159/just.egg-info/top_level.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)       97 2022-12-13 03:06:23.201632 just-0.8.159/setup.cfg
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1683 2022-12-13 03:06:21.000000 just-0.8.159/setup.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-13 03:06:23.201632 just-0.8.159/tests/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2748 2021-03-18 22:21:23.000000 just-0.8.159/tests/test_files.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      196 2019-10-30 12:22:05.000000 just-0.8.159/tests/test_jpath.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1041 2021-03-18 22:22:11.000000 just-0.8.159/tests/test_requests.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      358 2021-02-06 15:52:11.000000 just-0.8.159/tox.ini
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 16:51:57.214571 just-0.8.160/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      148 2019-10-30 12:22:05.000000 just-0.8.160/.coveragerc
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      189 2019-10-30 12:22:05.000000 just-0.8.160/.gitignore
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      195 2019-10-30 12:22:05.000000 just-0.8.160/.travis.yml
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    34519 2019-10-30 12:22:05.000000 just-0.8.160/LICENSE
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2023-06-18 16:51:57.214571 just-0.8.160/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2791 2021-02-24 22:23:55.000000 just-0.8.160/README.md
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       60 2019-10-30 12:22:05.000000 just-0.8.160/README.rst
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      192 2019-10-30 12:22:05.000000 just-0.8.160/conftest.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      973 2022-12-11 15:47:37.000000 just-0.8.160/deploy.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 16:51:57.214571 just-0.8.160/just/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      802 2023-06-18 16:51:56.000000 just-0.8.160/just/__init__.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      510 2019-10-31 14:56:25.000000 just-0.8.160/just/bytes.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      323 2020-05-07 22:19:36.000000 just-0.8.160/just/dir.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      240 2022-10-12 23:24:09.000000 just-0.8.160/just/dt.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     6707 2022-10-11 01:42:38.000000 just-0.8.160/just/forcedip.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      422 2020-09-14 22:28:41.000000 just-0.8.160/just/jpath.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2855 2023-06-18 16:50:59.000000 just-0.8.160/just/json_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      631 2019-10-30 12:22:05.000000 just-0.8.160/just/log.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      313 2019-10-30 12:22:05.000000 just-0.8.160/just/newl.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     4247 2023-03-19 11:38:12.000000 just-0.8.160/just/path_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2565 2023-01-24 21:15:23.000000 just-0.8.160/just/pattern.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      183 2019-10-30 12:22:05.000000 just-0.8.160/just/pickle_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     6591 2023-06-18 16:50:00.000000 just-0.8.160/just/read_write.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    11536 2023-06-14 23:33:21.000000 just-0.8.160/just/requests_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2617 2022-10-11 02:05:39.000000 just-0.8.160/just/source_ip.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      177 2022-10-31 11:24:28.000000 just-0.8.160/just/toml_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      706 2020-01-15 22:53:45.000000 just-0.8.160/just/txt.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      198 2021-02-06 15:54:20.000000 just-0.8.160/just/yaml_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      693 2021-04-17 11:52:08.000000 just-0.8.160/just/zstd_.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 16:51:57.214571 just-0.8.160/just.egg-info/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2023-06-18 16:51:57.000000 just-0.8.160/just.egg-info/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      651 2023-06-18 16:51:57.000000 just-0.8.160/just.egg-info/SOURCES.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2023-06-18 16:51:57.000000 just-0.8.160/just.egg-info/dependency_links.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       45 2023-06-18 16:51:57.000000 just-0.8.160/just.egg-info/entry_points.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2019-10-30 12:22:52.000000 just-0.8.160/just.egg-info/not-zip-safe
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       59 2023-06-18 16:51:57.000000 just-0.8.160/just.egg-info/requires.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        5 2023-06-18 16:51:57.000000 just-0.8.160/just.egg-info/top_level.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       97 2023-06-18 16:51:57.214571 just-0.8.160/setup.cfg
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1683 2023-06-18 16:51:56.000000 just-0.8.160/setup.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 16:51:57.214571 just-0.8.160/tests/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2748 2021-03-18 22:21:23.000000 just-0.8.160/tests/test_files.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      196 2019-10-30 12:22:05.000000 just-0.8.160/tests/test_jpath.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1041 2021-03-18 22:22:11.000000 just-0.8.160/tests/test_requests.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      358 2021-02-06 15:52:11.000000 just-0.8.160/tox.ini
```

### Comparing `just-0.8.159/LICENSE` & `just-0.8.160/LICENSE`

 * *Files identical despite different names*

### Comparing `just-0.8.159/PKG-INFO` & `just-0.8.160/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: just
-Version: 0.8.159
+Version: 0.8.160
 Summary: Automatically just read and write files based on extension.
 Home-page: https://github.com/kootenpv/just
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: any
```

### Comparing `just-0.8.159/README.md` & `just-0.8.160/README.md`

 * *Files identical despite different names*

### Comparing `just-0.8.159/deploy.py` & `just-0.8.160/deploy.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/just/__init__.py` & `just-0.8.160/just/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 from just.pattern import Pattern
 
 # In [19]: with open("fuck.xz", "wb") as f: f.write(lzma.compress(html.encode()))
 
 # In [20]: with lzma.open("fuck.xz") as f: hh=f.read()
 
 __project__ = "just"
-__version__ = "0.8.159"
+__version__ = "0.8.160"
```

### Comparing `just-0.8.159/just/forcedip.py` & `just-0.8.160/just/forcedip.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/just/json_.py` & `just-0.8.160/just/json_.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,18 @@
 def append(obj, fn):
     if not isinstance(fn, str):
         raise TypeError("Cannot append to compression")
     with open(fn, "a+") as f:
         f.write(orjson.dumps(obj, default=default).decode() + "\n")
 
 
-def write(obj, fn, option=orjson.OPT_INDENT_2):
+def write(obj, fn, indent=True):
+    # indent 0 = false, 1 = 2 lvls
     if not isinstance(obj, bytes):
-        obj = orjson.dumps(obj, option=option, default=default)
+        obj = orjson.dumps(obj, option=indent)
     if not isinstance(fn, str):
         fn.write(obj)
     else:
         with open(fn, "w") as f:
             f.write(obj.decode())
```

### Comparing `just-0.8.159/just/log.py` & `just-0.8.160/just/log.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/just/path_.py` & `just-0.8.160/just/path_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import inspect
 import os
+import re
 import glob2
 import errno
 import functools
 
 __cached_just_path = None
 
 
 def glob(path, sort_reverse=False):
+    res = re.findall("([$][A-Z_]+)", path)
+    for x in res:
+        path = path.replace(x, os.environ[x[1:]])
     path = make_path(path)
     return sorted(glob2.glob(path), reverse=sort_reverse)
 
 
 def get_just_env_path():
     return os.environ.get("JUST_PATH")
```

### Comparing `just-0.8.159/just/pattern.py` & `just-0.8.160/just/pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from ciso8601 import parse_datetime as isoparse
 from datetime import datetime
 from just import iread
 
 
-def parse_specials(special_str):
+def parse_specials(special_str):  # -> name, cast
     if not special_str:
         return "", "str"
     if "@" not in special_str:
         return special_str, ""
     return special_str.split("@")
 
 
@@ -85,8 +85,8 @@
     def find_dict(self, line):
         res = self.finder_multi(line)
         if res[0] is None:
             return None
         return {k: v for k, v in zip(self.names, res) if isinstance(k, int) or not k.startswith("_") and k}
 
     def stream(self, fname):
-        return [self.find_dict(x) for x in iread(fname)]
+        return [res for x in iread(fname) if (res := self.find_dict(x))]
```

### Comparing `just-0.8.159/just/read_write.py` & `just-0.8.160/just/read_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 
 def multi_read_tree(star_path, no_exist=None, unknown_type="html", ignore_exceptions=None, sort_reverse=False):
     for x in glob(star_path, sort_reverse=sort_reverse):
         yield x, read_tree(x, no_exist, unknown_type, ignore_exceptions)
 
 
-def writer(obj, fname, mkdir_no_exist, skip_if_exist, write_func_name, unknown_type):
+def writer(obj, fname, mkdir_no_exist, skip_if_exist, write_func_name, unknown_type, **kwargs):
     fname = make_path(fname)
     if skip_if_exist and os.path.isfile(fname):  # pragma: no cover
         return False
     if mkdir_no_exist:
         dname = os.path.dirname(fname)
         if dname not in set([".", "..", ""]):
             mkdir(dname)
@@ -136,21 +136,21 @@
         raise TypeError("just does not yet cover '{}'".format(ext))
     writer_module = EXT_TO_MODULE.get(ext, None) or EXT_TO_MODULE[unknown_type]
     write_fn = getattr(writer_module, write_func_name)
     if compression:
         # actually returns a file handler >.<
         compression = compression[0]
         with compression(fname, "wb") as f:
-            return write_fn(obj, f)
+            return write_fn(obj, f, **kwargs)
     else:
-        return write_fn(obj, fname)
+        return write_fn(obj, fname, **kwargs)
 
 
-def write(obj, fname, mkdir_no_exist=True, skip_if_exist=False, unknown_type="RAISE"):
-    return writer(obj, fname, mkdir_no_exist, skip_if_exist, "write", unknown_type)
+def write(obj, fname, mkdir_no_exist=True, skip_if_exist=False, unknown_type="RAISE", **kwargs):
+    return writer(obj, fname, mkdir_no_exist, skip_if_exist, "write", unknown_type, **kwargs)
 
 
 # only supported for JSON Lines so far.
 roll_counter = {}
 
 
 def get_rolled_path(fname, roll_extension):
```

### Comparing `just-0.8.159/just/requests_.py` & `just-0.8.160/just/requests_.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,14 +374,15 @@
     if fname is not None:
         write(result, fname)
 
     return result
 
 
 def request(data, **kwargs):
+    data = data.copy()
     return {"get": get, "post": post}[data.pop("method")](**data, **kwargs)
 
 
 def request_tree(*args, **kwargs):
     import lxml.html
     import requests_viewer  # to extend trees with `view`
```

### Comparing `just-0.8.159/just/source_ip.py` & `just-0.8.160/just/source_ip.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/just/txt.py` & `just-0.8.160/just/txt.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/just/zstd_.py` & `just-0.8.160/just/zstd_.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/just.egg-info/PKG-INFO` & `just-0.8.160/just.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: just
-Version: 0.8.159
+Version: 0.8.160
 Summary: Automatically just read and write files based on extension.
 Home-page: https://github.com/kootenpv/just
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: any
```

### Comparing `just-0.8.159/just.egg-info/SOURCES.txt` & `just-0.8.160/just.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `just-0.8.159/setup.py` & `just-0.8.160/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "8"
-MICRO_VERSION = "159"
+MICRO_VERSION = "160"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 setup(
     name="just",
     version=VERSION,
     description="Automatically just read and write files based on extension.",
     author="Pascal van Kooten",
```

### Comparing `just-0.8.159/tests/test_files.py` & `just-0.8.160/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `just-0.8.159/tests/test_requests.py` & `just-0.8.160/tests/test_requests.py`

 * *Files identical despite different names*

