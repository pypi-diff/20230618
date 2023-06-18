# Comparing `tmp/pylibffm-0.4.0.tar.gz` & `tmp/pylibffm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibffm-0.4.0.tar", last modified: Sat Jun 17 13:10:08 2023, max compression
+gzip compressed data, was "pylibffm-0.4.1.tar", last modified: Sun Jun 18 07:03:27 2023, max compression
```

## Comparing `pylibffm-0.4.0.tar` & `pylibffm-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-17 13:10:08.919716 pylibffm-0.4.0/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1064 2023-06-01 12:37:51.000000 pylibffm-0.4.0/LICENSE
--rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.4.0/MANIFEST.in
--rw-rw-r--   0 julien    (1003) julien    (1003)     1696 2023-06-17 13:10:08.919716 pylibffm-0.4.0/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)      897 2023-06-17 13:06:32.000000 pylibffm-0.4.0/README.md
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-17 13:10:08.919716 pylibffm-0.4.0/pylibffm/
--rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.4.0/pylibffm/__init__.py
--rw-rw-r--   0 julien    (1003) julien    (1003)     8032 2023-06-17 13:00:37.000000 pylibffm-0.4.0/pylibffm/api.py
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-17 13:00:22.000000 pylibffm-0.4.0/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-17 13:10:08.000000 pylibffm-0.4.0/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-17 13:09:54.000000 pylibffm-0.4.0/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-17 13:09:59.000000 pylibffm-0.4.0/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-17 13:10:03.000000 pylibffm-0.4.0/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-17 13:10:08.919716 pylibffm-0.4.0/pylibffm.egg-info/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1696 2023-06-17 13:10:08.000000 pylibffm-0.4.0/pylibffm.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)      477 2023-06-17 13:10:08.000000 pylibffm-0.4.0/pylibffm.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-17 13:10:08.000000 pylibffm-0.4.0/pylibffm.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-17 13:10:08.000000 pylibffm-0.4.0/pylibffm.egg-info/requires.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-17 13:10:08.000000 pylibffm-0.4.0/pylibffm.egg-info/top_level.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-17 13:10:08.919716 pylibffm-0.4.0/setup.cfg
--rw-rw-r--   0 julien    (1003) julien    (1003)     1523 2023-06-17 13:06:08.000000 pylibffm-0.4.0/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-18 07:03:27.296003 pylibffm-0.4.1/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1064 2023-06-01 12:37:51.000000 pylibffm-0.4.1/LICENSE
+-rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.4.1/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1696 2023-06-18 07:03:27.296003 pylibffm-0.4.1/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      897 2023-06-17 13:06:32.000000 pylibffm-0.4.1/README.md
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-18 07:03:27.296003 pylibffm-0.4.1/pylibffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.4.1/pylibffm/__init__.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     8178 2023-06-18 07:01:27.000000 pylibffm-0.4.1/pylibffm/api.py
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-17 13:00:22.000000 pylibffm-0.4.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-17 13:10:08.000000 pylibffm-0.4.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-17 13:09:54.000000 pylibffm-0.4.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-17 13:09:59.000000 pylibffm-0.4.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-17 13:10:03.000000 pylibffm-0.4.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-18 07:03:27.296003 pylibffm-0.4.1/pylibffm.egg-info/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1696 2023-06-18 07:03:27.000000 pylibffm-0.4.1/pylibffm.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      477 2023-06-18 07:03:27.000000 pylibffm-0.4.1/pylibffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-18 07:03:27.000000 pylibffm-0.4.1/pylibffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-18 07:03:27.000000 pylibffm-0.4.1/pylibffm.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-18 07:03:27.000000 pylibffm-0.4.1/pylibffm.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-18 07:03:27.296003 pylibffm-0.4.1/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1523 2023-06-18 07:02:57.000000 pylibffm-0.4.1/setup.py
```

### Comparing `pylibffm-0.4.0/LICENSE` & `pylibffm-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/PKG-INFO` & `pylibffm-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibffm
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library wrapping libffm
 Home-page: https://github.com/Sinacam/pylibffm
 Author: ntumlgroup
 License: MIT License
 Description: # pylibffm
         
         pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_0lhp4m42_/tmpvfj3aviz_TarContainer/0/3", line 54, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_0lhp4m42_/tmpvfj3aviz_TarContainer/0/3", line 54, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylibffm Version: 0.4.0 Summary: A library wrapping
+Metadata-Version: 2.1 Name: pylibffm Version: 0.4.1 Summary: A library wrapping
 libffm Home-page: https://github.com/Sinacam/pylibffm Author: ntumlgroup
 License: MIT License Description: # pylibffm pylibffm is a wrapper around
 libffm to allow using scipy and numpy arrays as input. pylibffm requires SSE
 and openmp. ## Installing If you're running python 3.7~3.11 on linux ```bash
 pip install pylibffm ``` Otherwise ```bash git clone --recurse-submodules
 https://github.com/Sinacam/pylibffm cd pylibffm make pip install . ```
 Currently, the distribution is incredibly hacky and cannot be pip installed
```

### Comparing `pylibffm-0.4.0/README.md` & `pylibffm-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/pylibffm/api.py` & `pylibffm-0.4.1/pylibffm/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,22 +90,26 @@
 
     train_path, cached = make_bin(tmpdir, train_x, train_y, fields)
     if cached:
         print(
             f'Using training data cache "{train_path}"',
             file=sys.stderr,
         )
+    else:
+        print(f'Caching training data to "{train_path}"')
 
     if options.get("auto_stop", False):
         valid_path, cached = make_bin(tmpdir, valid_x, valid_y, fields)
         if cached:
             print(
                 f'Using validation data cache "{valid_path}"',
                 file=sys.stderr,
             )
+        else:
+            print(f'Caching validation data to "{valid_path}"')
     else:
         valid_path = None
 
     return train_with_bin(train_path, options, valid_path)
 
 
 def train_with_bin(
```

### Comparing `pylibffm-0.4.0/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so` & `pylibffm-0.4.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so` & `pylibffm-0.4.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so` & `pylibffm-0.4.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so` & `pylibffm-0.4.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so` & `pylibffm-0.4.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.4.0/pylibffm.egg-info/PKG-INFO` & `pylibffm-0.4.1/pylibffm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibffm
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library wrapping libffm
 Home-page: https://github.com/Sinacam/pylibffm
 Author: ntumlgroup
 License: MIT License
 Description: # pylibffm
         
         pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_0lhp4m42_/tmpvfj3aviz_TarContainer/0/14", line 54, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_0lhp4m42_/tmpvfj3aviz_TarContainer/0/14", line 54, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylibffm Version: 0.4.0 Summary: A library wrapping
+Metadata-Version: 2.1 Name: pylibffm Version: 0.4.1 Summary: A library wrapping
 libffm Home-page: https://github.com/Sinacam/pylibffm Author: ntumlgroup
 License: MIT License Description: # pylibffm pylibffm is a wrapper around
 libffm to allow using scipy and numpy arrays as input. pylibffm requires SSE
 and openmp. ## Installing If you're running python 3.7~3.11 on linux ```bash
 pip install pylibffm ``` Otherwise ```bash git clone --recurse-submodules
 https://github.com/Sinacam/pylibffm cd pylibffm make pip install . ```
 Currently, the distribution is incredibly hacky and cannot be pip installed
```

### Comparing `pylibffm-0.4.0/setup.py` & `pylibffm-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 import setuptools
 
 name = "pylibffm"
-version = "0.4.0"
+version = "0.4.1"
 author = "ntumlgroup"
 license = "MIT License"
 license_file = "LICENSE"
 description = "A library wrapping libffm"
 long_description = (pathlib.Path(__file__).parent / "README.md").read_text()
 long_description_content_type = "text/markdown"
 url = "https://github.com/Sinacam/pylibffm"
```

