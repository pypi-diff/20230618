# Comparing `tmp/notctyparser-23.6.3.tar.gz` & `tmp/notctyparser-23.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notctyparser-23.6.3.tar", last modified: Sat Jun  3 17:32:33 2023, max compression
+gzip compressed data, was "notctyparser-23.6.4.tar", last modified: Sun Jun  4 19:57:20 2023, max compression
```

## Comparing `notctyparser-23.6.3.tar` & `notctyparser-23.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.216105 notctyparser-23.6.3/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1080 2023-06-01 20:39:35.000000 notctyparser-23.6.3/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1703 2023-06-03 17:32:33.216105 notctyparser-23.6.3/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      939 2023-06-03 17:30:33.000000 notctyparser-23.6.3/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.211105 notctyparser-23.6.3/docs/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2346 2023-06-01 20:39:35.000000 notctyparser-23.6.3/docs/conf.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.213105 notctyparser-23.6.3/notctyparser/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      368 2023-06-02 14:16:48.000000 notctyparser-23.6.3/notctyparser/__info__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      251 2023-06-01 20:39:35.000000 notctyparser-23.6.3/notctyparser/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      499 2023-06-01 21:07:38.000000 notctyparser-23.6.3/notctyparser/__main__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10663 2023-06-03 17:28:30.000000 notctyparser-23.6.3/notctyparser/bigcty.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-03 17:32:33.215105 notctyparser-23.6.3/notctyparser.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1703 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      322 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       20 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       23 2023-06-03 17:32:33.000000 notctyparser-23.6.3/notctyparser.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      908 2023-06-03 17:18:59.000000 notctyparser-23.6.3/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-03 17:32:33.217105 notctyparser-23.6.3/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-04 19:57:20.480718 notctyparser-23.6.4/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1080 2023-06-01 20:39:35.000000 notctyparser-23.6.4/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1711 2023-06-04 19:57:20.480718 notctyparser-23.6.4/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      947 2023-06-04 18:48:34.000000 notctyparser-23.6.4/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-04 19:57:20.476718 notctyparser-23.6.4/docs/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2346 2023-06-01 20:39:35.000000 notctyparser-23.6.4/docs/conf.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-04 19:57:20.477718 notctyparser-23.6.4/notctyparser/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      368 2023-06-04 18:48:34.000000 notctyparser-23.6.4/notctyparser/__info__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      251 2023-06-04 18:48:34.000000 notctyparser-23.6.4/notctyparser/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      499 2023-06-04 18:48:34.000000 notctyparser-23.6.4/notctyparser/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10871 2023-06-04 19:49:51.000000 notctyparser-23.6.4/notctyparser/bigcty.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-06-04 19:57:20.479718 notctyparser-23.6.4/notctyparser.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1711 2023-06-04 19:57:20.000000 notctyparser-23.6.4/notctyparser.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      322 2023-06-04 19:57:20.000000 notctyparser-23.6.4/notctyparser.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-06-04 19:57:20.000000 notctyparser-23.6.4/notctyparser.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       25 2023-06-04 19:57:20.000000 notctyparser-23.6.4/notctyparser.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       23 2023-06-04 19:57:20.000000 notctyparser-23.6.4/notctyparser.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      920 2023-06-04 19:52:55.000000 notctyparser-23.6.4/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-06-04 19:57:20.480718 notctyparser-23.6.4/setup.cfg
```

### Comparing `notctyparser-23.6.3/LICENSE` & `notctyparser-23.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notctyparser-23.6.3/PKG-INFO` & `notctyparser-23.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notctyparser
-Version: 23.6.3
+Version: 23.6.4
 Summary: Just ctyparser with added version check.
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/ctyparser
 Project-URL: Bug Tracker, https://github.com/mbridak/ctyparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -39,17 +39,17 @@
 
 I just added a stupid check for update without doing the update.
 
 ```python
 def check_update(self) -> bool:
 ```
 
-Used xpath to parse the download link.
-Chose more narrow raised exceptions.
-Specified utf-8 file encoding.
-Made the linter happy.
+- Used xpath to parse the download link.
+- Chose more narrow raised exceptions.
+- Specified utf-8 file encoding.
+- Made the linter happy.
 
 ## Copyright
 
 Copyright 2019-2022 classabbyamp, 0x5c  
 Released under the MIT License.  
 See `LICENSE` for the full license text.
```

### Comparing `notctyparser-23.6.3/README.md` & `notctyparser-23.6.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 I just added a stupid check for update without doing the update.
 
 ```python
 def check_update(self) -> bool:
 ```
 
-Used xpath to parse the download link.
-Chose more narrow raised exceptions.
-Specified utf-8 file encoding.
-Made the linter happy.
+- Used xpath to parse the download link.
+- Chose more narrow raised exceptions.
+- Specified utf-8 file encoding.
+- Made the linter happy.
 
 ## Copyright
 
 Copyright 2019-2022 classabbyamp, 0x5c  
 Released under the MIT License.  
 See `LICENSE` for the full license text.
```

### Comparing `notctyparser-23.6.3/docs/conf.py` & `notctyparser-23.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `notctyparser-23.6.3/notctyparser/bigcty.py` & `notctyparser-23.6.4/notctyparser/bigcty.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,20 @@
             if self._version == update_date:
                 return False
 
             with tempfile.TemporaryDirectory() as temp:
                 path = pathlib.PurePath(temp)
                 page = session.get(update_url)
                 tree = html.fromstring(page.content)
-                dl_url = tree.xpath("//a[contains(@href,'zip')]/@href")[0]
+                urls = tree.xpath("//a[contains(@href,'zip')]/@href")
+                if len(urls) == 0:
+                    raise ResourceWarning(
+                        f"Unable to find and download bigcty-{update_date}.zip"
+                    )
+                dl_url = urls[0]
                 the_request = session.get(dl_url)
                 if the_request.status_code == 404:
                     dl_url = (
                         "http://www.country-files.com/bigcty/download/bigcty-"
                         f"{update_date}.zip"
                     )
                     the_request = session.get(dl_url)
```

### Comparing `notctyparser-23.6.3/notctyparser.egg-info/PKG-INFO` & `notctyparser-23.6.4/notctyparser.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notctyparser
-Version: 23.6.3
+Version: 23.6.4
 Summary: Just ctyparser with added version check.
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/ctyparser
 Project-URL: Bug Tracker, https://github.com/mbridak/ctyparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -39,17 +39,17 @@
 
 I just added a stupid check for update without doing the update.
 
 ```python
 def check_update(self) -> bool:
 ```
 
-Used xpath to parse the download link.
-Chose more narrow raised exceptions.
-Specified utf-8 file encoding.
-Made the linter happy.
+- Used xpath to parse the download link.
+- Chose more narrow raised exceptions.
+- Specified utf-8 file encoding.
+- Made the linter happy.
 
 ## Copyright
 
 Copyright 2019-2022 classabbyamp, 0x5c  
 Released under the MIT License.  
 See `LICENSE` for the full license text.
```

### Comparing `notctyparser-23.6.3/pyproject.toml` & `notctyparser-23.6.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "notctyparser" 
-version = "23.6.3"
+version = "23.6.4"
 description = "Just ctyparser with added version check."
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
     "feedparser",
     "requests",
+    "lxml",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Environment :: X11 Applications :: Qt",
     "Operating System :: POSIX :: Linux",
```

