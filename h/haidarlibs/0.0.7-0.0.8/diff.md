# Comparing `tmp/haidarlibs-0.0.7.tar.gz` & `tmp/haidarlibs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haidarlibs-0.0.7.tar", last modified: Sun Jun 18 17:04:33 2023, max compression
+gzip compressed data, was "haidarlibs-0.0.8.tar", last modified: Sun Jun 18 17:06:14 2023, max compression
```

## Comparing `haidarlibs-0.0.7.tar` & `haidarlibs-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 17:04:33.133113 haidarlibs-0.0.7/
--rw-rw-rw-   0        0        0    35182 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2641 2023-06-18 17:04:33.134112 haidarlibs-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1625 2023-06-16 03:36:45.000000 haidarlibs-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 17:04:33.083006 haidarlibs-0.0.7/haidarlibs/
--rw-rw-rw-   0        0        0     1196 2023-06-15 20:33:48.000000 haidarlibs-0.0.7/haidarlibs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:04:33.106528 haidarlibs-0.0.7/haidarlibs/dar/
--rw-rw-rw-   0        0        0     1912 2023-06-16 03:35:10.000000 haidarlibs-0.0.7/haidarlibs/dar/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-06-18 17:04:15.000000 haidarlibs-0.0.7/haidarlibs/dar/load.py
--rw-rw-rw-   0        0        0      890 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/log.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:04:33.129124 haidarlibs-0.0.7/haidarlibs/dar/utils/
--rw-rw-rw-   0        0        0     1567 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/PyroHelpers.py
--rw-rw-rw-   0        0        0      371 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/__init__.py
--rw-rw-rw-   0        0        0     1864 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/adminHelpers.py
--rw-rw-rw-   0        0        0      653 2023-06-16 03:38:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/ai.py
--rw-rw-rw-   0        0        0     1058 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/aiohttp_helper.py
--rw-rw-rw-   0        0        0     1301 2023-06-16 03:55:36.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/basic.py
--rw-rw-rw-   0        0        0    15599 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:04:33.131119 haidarlibs-0.0.7/haidarlibs/dar/utils/db/
--rw-rw-rw-   0        0        0    14256 2023-06-16 12:29:33.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/db/__init__.py
--rw-rw-rw-   0        0        0     1190 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/db/permit.py
--rw-rw-rw-   0        0        0     4007 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/function.py
--rw-rw-rw-   0        0        0      568 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/get_id.py
--rw-rw-rw-   0        0        0     1490 2023-06-16 03:38:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/http.py
--rw-rw-rw-   0        0        0     2055 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/inline.py
--rw-rw-rw-   0        0        0     1075 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/interval.py
--rw-rw-rw-   0        0        0     3620 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/misc.py
--rw-rw-rw-   0        0        0      555 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/parser.py
--rw-rw-rw-   0        0        0     1844 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/pilter.py
--rw-rw-rw-   0        0        0    17760 2023-06-16 03:34:40.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/tools.py
--rw-rw-rw-   0        0        0      567 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/unpack.py
--rw-rw-rw-   0        0        0     2027 2023-06-07 15:30:26.000000 haidarlibs-0.0.7/haidarlibs/dar/utils/utility.py
--rw-rw-rw-   0        0        0       47 2023-06-18 17:04:26.000000 haidarlibs-0.0.7/haidarlibs/version.py
-drwxrwxrwx   0        0        0        0 2023-06-18 17:04:33.097968 haidarlibs-0.0.7/haidarlibs.egg-info/
--rw-rw-rw-   0        0        0     2641 2023-06-18 17:04:32.000000 haidarlibs-0.0.7/haidarlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-06-18 17:04:33.000000 haidarlibs-0.0.7/haidarlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 17:04:32.000000 haidarlibs-0.0.7/haidarlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-18 17:04:32.000000 haidarlibs-0.0.7/haidarlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 17:04:32.000000 haidarlibs-0.0.7/haidarlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 17:04:33.135266 haidarlibs-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1611 2023-06-17 00:33:45.000000 haidarlibs-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:06:14.685650 haidarlibs-0.0.8/
+-rw-rw-rw-   0        0        0    35182 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2641 2023-06-18 17:06:14.686648 haidarlibs-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1625 2023-06-16 03:36:45.000000 haidarlibs-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 17:06:14.640770 haidarlibs-0.0.8/haidarlibs/
+-rw-rw-rw-   0        0        0     1196 2023-06-15 20:33:48.000000 haidarlibs-0.0.8/haidarlibs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:06:14.658722 haidarlibs-0.0.8/haidarlibs/dar/
+-rw-rw-rw-   0        0        0     1912 2023-06-16 03:35:10.000000 haidarlibs-0.0.8/haidarlibs/dar/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-06-18 17:04:15.000000 haidarlibs-0.0.8/haidarlibs/dar/load.py
+-rw-rw-rw-   0        0        0      890 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/log.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:06:14.681661 haidarlibs-0.0.8/haidarlibs/dar/utils/
+-rw-rw-rw-   0        0        0     1567 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/PyroHelpers.py
+-rw-rw-rw-   0        0        0      371 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/__init__.py
+-rw-rw-rw-   0        0        0     1864 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/adminHelpers.py
+-rw-rw-rw-   0        0        0      653 2023-06-16 03:38:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/ai.py
+-rw-rw-rw-   0        0        0     1058 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/aiohttp_helper.py
+-rw-rw-rw-   0        0        0     1301 2023-06-16 03:55:36.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/basic.py
+-rw-rw-rw-   0        0        0    15599 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:06:14.684652 haidarlibs-0.0.8/haidarlibs/dar/utils/db/
+-rw-rw-rw-   0        0        0    14256 2023-06-16 12:29:33.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/db/__init__.py
+-rw-rw-rw-   0        0        0     1190 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/db/permit.py
+-rw-rw-rw-   0        0        0     4007 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/function.py
+-rw-rw-rw-   0        0        0      568 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/get_id.py
+-rw-rw-rw-   0        0        0     1490 2023-06-16 03:38:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/http.py
+-rw-rw-rw-   0        0        0     2055 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/inline.py
+-rw-rw-rw-   0        0        0     1075 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/interval.py
+-rw-rw-rw-   0        0        0     3620 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/misc.py
+-rw-rw-rw-   0        0        0      555 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/parser.py
+-rw-rw-rw-   0        0        0     1844 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/pilter.py
+-rw-rw-rw-   0        0        0    17760 2023-06-16 03:34:40.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/tools.py
+-rw-rw-rw-   0        0        0      567 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/unpack.py
+-rw-rw-rw-   0        0        0     2027 2023-06-07 15:30:26.000000 haidarlibs-0.0.8/haidarlibs/dar/utils/utility.py
+-rw-rw-rw-   0        0        0       47 2023-06-18 17:05:48.000000 haidarlibs-0.0.8/haidarlibs/version.py
+drwxrwxrwx   0        0        0        0 2023-06-18 17:06:14.654734 haidarlibs-0.0.8/haidarlibs.egg-info/
+-rw-rw-rw-   0        0        0     2641 2023-06-18 17:06:14.000000 haidarlibs-0.0.8/haidarlibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2023-06-18 17:06:14.000000 haidarlibs-0.0.8/haidarlibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 17:06:14.000000 haidarlibs-0.0.8/haidarlibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-18 17:06:14.000000 haidarlibs-0.0.8/haidarlibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-18 17:06:14.000000 haidarlibs-0.0.8/haidarlibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 17:06:14.688642 haidarlibs-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1611 2023-06-17 00:33:45.000000 haidarlibs-0.0.8/setup.py
```

### Comparing `haidarlibs-0.0.7/LICENSE` & `haidarlibs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/PKG-INFO` & `haidarlibs-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haidarlibs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Haidar-Pyro.
 Home-page: https://github.com/XhaidarX/Haidarlibs
 Author: Haidar
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/Haidarlibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `haidarlibs-0.0.7/README.md` & `haidarlibs-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/__init__.py` & `haidarlibs-0.0.8/haidarlibs/__init__.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/__init__.py` & `haidarlibs-0.0.8/haidarlibs/dar/__init__.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/load.py` & `haidarlibs-0.0.8/haidarlibs/dar/load.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/log.py` & `haidarlibs-0.0.8/haidarlibs/dar/log.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/PyroHelpers.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/adminHelpers.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/ai.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/ai.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/aiohttp_helper.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/basic.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/basic.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/constants.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/constants.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/db/__init__.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/db/permit.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/function.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/function.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/get_id.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/http.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/http.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/inline.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/inline.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/interval.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/interval.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/misc.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/misc.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/parser.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/parser.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/pilter.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/tools.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/tools.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/unpack.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs/dar/utils/utility.py` & `haidarlibs-0.0.8/haidarlibs/dar/utils/utility.py`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/haidarlibs.egg-info/PKG-INFO` & `haidarlibs-0.0.8/haidarlibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haidarlibs
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Haidar-Pyro.
 Home-page: https://github.com/XhaidarX/Haidarlibs
 Author: Haidar
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/XhaidarX/Haidarlibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `haidarlibs-0.0.7/haidarlibs.egg-info/SOURCES.txt` & `haidarlibs-0.0.8/haidarlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haidarlibs-0.0.7/setup.py` & `haidarlibs-0.0.8/setup.py`

 * *Files identical despite different names*

