# Comparing `tmp/etm-dgraham-5.1.0.tar.gz` & `tmp/etm-dgraham-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.0.tar", last modified: Sun Jun 18 11:28:39 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.1.tar", last modified: Sun Jun 18 12:29:26 2023, max compression
```

## Comparing `etm-dgraham-5.1.0.tar` & `etm-dgraham-5.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.563146 etm-dgraham-5.1.0/
--rw-r--r--   0 dag        (501) staff       (20)     2503 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-18 11:28:39.562989 etm-dgraham-5.1.0/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.0/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.0/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.556477 etm-dgraham-5.1.0/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.558664 etm-dgraham-5.1.0/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.0/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.0/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.0/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.0/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   284786 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.0/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100088 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.561060 etm-dgraham-5.1.0/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.0/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.0/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-18 11:28:39.563183 etm-dgraham-5.1.0/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.0/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.561172 etm-dgraham-5.1.0/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.0/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.562363 etm-dgraham-5.1.0/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.0/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.0/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.0/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.467400 etm-dgraham-5.1.1/
+-rw-r--r--   0 dag        (501) staff       (20)     2504 2023-06-18 12:29:18.000000 etm-dgraham-5.1.1/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-18 12:29:26.467184 etm-dgraham-5.1.1/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.1/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.1/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.1/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.461023 etm-dgraham-5.1.1/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.463292 etm-dgraham-5.1.1/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.1/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-18 12:29:18.000000 etm-dgraham-5.1.1/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.1/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.1/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.1/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   284740 2023-06-18 12:29:18.000000 etm-dgraham-5.1.1/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.1/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.1/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100088 2023-06-18 11:28:27.000000 etm-dgraham-5.1.1/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.465454 etm-dgraham-5.1.1/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-18 12:29:26.000000 etm-dgraham-5.1.1/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.1/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.1/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.1/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-18 12:29:26.467451 etm-dgraham-5.1.1/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.1/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.465565 etm-dgraham-5.1.1/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.1/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 12:29:26.466617 etm-dgraham-5.1.1/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.1/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.1/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.1/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.1/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.0/CHANGES.txt` & `etm-dgraham-5.1.1/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-Recent tagged changes as of 2023-06-18T07:28:25.718710-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.0) Daniel Graham
+Recent tagged changes as of 2023-06-18T08:29:16.450280-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.1) Daniel Graham
+    d0c733f 2023-06-18 08:29:16 -0400
+    Tagged version 5.1.1.
+
+- 61 minutes ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
-- 23 hours ago (tag: 5.0.12) Daniel Graham
+- 24 hours ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
 
-- 26 hours ago (tag: 5.0.11) Daniel Graham
+- 27 hours ago (tag: 5.0.11) Daniel Graham
     e9228d2 2023-06-17 05:19:31 -0400
     Tagged version 5.0.11.
 
-- 26 hours ago (tag: 5.0.10) Daniel Graham
+- 27 hours ago (tag: 5.0.10) Daniel Graham
     2e1f579 2023-06-17 05:05:32 -0400
     Tagged version 5.0.10.
 
 - 3 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
-- 4 days ago (tag: 5.0.8) Daniel Graham
+- 5 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
 - 10 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
@@ -73,11 +77,7 @@
 - 4 weeks ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
 
 - 4 weeks ago (tag: 4.12.5) Daniel Graham
     f0c24d8 2023-05-21 15:08:06 -0400
     Tagged version 4.12.5.
-
-- 4 weeks ago (tag: 4.12.4) Daniel Graham
-    15b3333 2023-05-20 14:33:40 -0400
-    Tagged version 4.12.4.
```

### Comparing `etm-dgraham-5.1.0/PKG-INFO` & `etm-dgraham-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.0
+Version: 5.1.1
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.0/README.md` & `etm-dgraham-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/bump.py` & `etm-dgraham-5.1.1/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/docs/index_konnections.md` & `etm-dgraham-5.1.1/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/docs/index_usedtime.md` & `etm-dgraham-5.1.1/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/docs/multiple_timers.md` & `etm-dgraham-5.1.1/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/__main__.py` & `etm-dgraham-5.1.1/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/data.py` & `etm-dgraham-5.1.1/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/ical.py` & `etm-dgraham-5.1.1/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/make_examples.py` & `etm-dgraham-5.1.1/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/model.py` & `etm-dgraham-5.1.1/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2997,15 +2997,15 @@
         res = self.get_row_details(row)
         if not res:
             return None, ''
         item_id = res[0]
 
         if not (item_id and item_id in self.id2relevant):
             return ''
-        showing = "History"
+        showing = "Completion History"
         item = DBITEM.get(doc_id=item_id)
 
         if not (item['itemtype'] == '-' and ('r' in item or '+' in item)):
             return showing, "not a repeating task"
         if 'h' not in item:
             return showing, "there is no history of completions"
 
@@ -6821,31 +6821,28 @@
     done2id_hsh = {}     # yw -> row2id
     engaged_hsh = {}
     engaged2id_hsh = {}     # yw -> row2id
     week2day2engaged = {}   # year, week -> dayofweek -> period total for day
     week2day2heading = {}
     weeks = set([])
     rows = []
-    # done = []
-    # completed = []
+    done = []
     engaged = []
-    # busy = []
 
     #XXX year, week -> dayofweek -> list of [time interval, summary, period]
     busy_details = {}
     week2day2busy = {}
     week2day2allday = {}
 
     #XXX main loop begins
     todayYMD = now.format("YYYYMMDD")
     tomorrowYMD = (now + 1*DAY).format("YYYYMMDD")
 
     for item in db:
         completed = []
-        done = []
         if item.get('itemtype', None) == None:
             logger.error(f"itemtype missing from {item}")
             continue
         if item['itemtype'] in "!?":
             continue
 
         doc_id = item.doc_id
```

### Comparing `etm-dgraham-5.1.0/etm/options.py` & `etm-dgraham-5.1.1/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/report.py` & `etm-dgraham-5.1.1/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm/view.py` & `etm-dgraham-5.1.1/etm/view.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.0
+Version: 5.1.1
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.1/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.1/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etmlogo.png` & `etm-dgraham-5.1.1/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etmlogo_small.png` & `etm-dgraham-5.1.1/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/etmview_agenda.png` & `etm-dgraham-5.1.1/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/namedcolors.py` & `etm-dgraham-5.1.1/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/new.png` & `etm-dgraham-5.1.1/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/setup.py` & `etm-dgraham-5.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/test/test_parser.py` & `etm-dgraham-5.1.1/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.1/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/utilities/etm_in` & `etm-dgraham-5.1.1/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/utilities/inbasket` & `etm-dgraham-5.1.1/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.0/utilities/open_in_mutt` & `etm-dgraham-5.1.1/utilities/open_in_mutt`

 * *Files identical despite different names*

