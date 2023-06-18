# Comparing `tmp/etm-dgraham-5.0.9.tar.gz` & `tmp/etm-dgraham-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.9.tar", last modified: Thu Jun 15 14:14:47 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.0.tar", last modified: Sun Jun 18 11:28:39 2023, max compression
```

## Comparing `etm-dgraham-5.0.9.tar` & `etm-dgraham-5.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.048062 etm-dgraham-5.0.9/
--rw-r--r--   0 dag        (501) staff       (20)     2463 2023-06-15 14:14:22.000000 etm-dgraham-5.0.9/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129624 2023-06-15 14:14:47.047914 etm-dgraham-5.0.9/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128712 2023-06-14 16:35:47.000000 etm-dgraham-5.0.9/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.9/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.9/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.039799 etm-dgraham-5.0.9/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.043736 etm-dgraham-5.0.9/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.0.9/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-15 14:14:22.000000 etm-dgraham-5.0.9/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.9/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.9/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.9/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   283305 2023-06-15 14:14:22.000000 etm-dgraham-5.0.9/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37350 2023-06-14 16:35:47.000000 etm-dgraham-5.0.9/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.9/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    98989 2023-06-15 12:36:09.000000 etm-dgraham-5.0.9/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.046348 etm-dgraham-5.0.9/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129624 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.9/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.9/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-15 14:14:47.048094 etm-dgraham-5.0.9/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.9/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.046451 etm-dgraham-5.0.9/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.9/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.047422 etm-dgraham-5.0.9/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.9/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.9/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.9/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.563146 etm-dgraham-5.1.0/
+-rw-r--r--   0 dag        (501) staff       (20)     2503 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132529 2023-06-18 11:28:39.562989 etm-dgraham-5.1.0/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131617 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.0/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.0/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.556477 etm-dgraham-5.1.0/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.558664 etm-dgraham-5.1.0/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.0/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.0/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.0/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.0/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   284786 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.0/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100088 2023-06-18 11:28:27.000000 etm-dgraham-5.1.0/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.561060 etm-dgraham-5.1.0/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132529 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-18 11:28:39.000000 etm-dgraham-5.1.0/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.0/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.0/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.0/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-18 11:28:39.563183 etm-dgraham-5.1.0/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.0/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.561172 etm-dgraham-5.1.0/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.0/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-18 11:28:39.562363 etm-dgraham-5.1.0/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.0/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.0/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.0/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.0/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.9/CHANGES.txt` & `etm-dgraham-5.1.0/CHANGES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,63 @@
-Recent tagged changes as of 2023-06-15T10:14:19.986207-04:00:
-- 1 second ago (HEAD -> working, tag: 5.0.9) Daniel Graham
+Recent tagged changes as of 2023-06-18T07:28:25.718710-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.0) Daniel Graham
+    ece86e8 2023-06-18 07:28:25 -0400
+    Tagged version 5.1.0. Added ability to display completion history
+    for tasks including skipped instead of finished instances.
+
+- 23 hours ago (tag: 5.0.12) Daniel Graham
+    c42576c 2023-06-17 08:57:03 -0400
+    Tagged version 5.0.12.
+
+- 26 hours ago (tag: 5.0.11) Daniel Graham
+    e9228d2 2023-06-17 05:19:31 -0400
+    Tagged version 5.0.11.
+
+- 26 hours ago (tag: 5.0.10) Daniel Graham
+    2e1f579 2023-06-17 05:05:32 -0400
+    Tagged version 5.0.10.
+
+- 3 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
-- 2 days ago (tag: 5.0.8) Daniel Graham
+- 4 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
-- 7 days ago (tag: 5.0.7) Daniel Graham
+- 10 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
-- 10 days ago (tag: 5.0.6) Daniel Graham
+- 13 days ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
-- 10 days ago (tag: 5.0.5) Daniel Graham
+- 13 days ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 10 days ago (tag: 5.0.4) Daniel Graham
+- 13 days ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 11 days ago (tag: 5.0.3) Daniel Graham
+- 2 weeks ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 11 days ago (tag: 5.0.2) Daniel Graham
+- 2 weeks ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 11 days ago (tag: 5.0.1) Daniel Graham
+- 2 weeks ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
-- 12 days ago (tag: 5.0.0) Daniel Graham
+- 2 weeks ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
 
 - 3 weeks ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
@@ -49,35 +66,18 @@
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
 - 3 weeks ago (tag: 4.12.7) Daniel Graham
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
 
-- 3 weeks ago (tag: 4.12.6) Daniel Graham
+- 4 weeks ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
 
 - 4 weeks ago (tag: 4.12.5) Daniel Graham
     f0c24d8 2023-05-21 15:08:06 -0400
     Tagged version 4.12.5.
 
 - 4 weeks ago (tag: 4.12.4) Daniel Graham
     15b3333 2023-05-20 14:33:40 -0400
     Tagged version 4.12.4.
-
-- 4 weeks ago (tag: 4.12.3) Daniel Graham
-    dd49fda 2023-05-17 12:24:12 -0400
-    Tagged version 4.12.3.
-
-- 4 weeks ago (tag: 4.12.2) Daniel Graham
-    2a304a3 2023-05-17 09:34:05 -0400
-    Tagged version 4.12.2.
-
-- 4 weeks ago (tag: 4.12.1) Daniel Graham
-    68005b7 2023-05-15 14:20:25 -0400
-    Tagged version 4.12.1. Added display for all-day events to busy
-    view
-
-- 5 weeks ago (tag: 4.12.0) Daniel Graham
-    ce2ab09 2023-05-13 12:46:39 -0400
-    Tagged version 4.12.0. Added engaged view
```

### Comparing `etm-dgraham-5.0.9/PKG-INFO` & `etm-dgraham-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.9
+Version: 5.1.0
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -1219,14 +1219,15 @@
         D) delete
         F) finish
         P) toggle pin
         R) reschedule
         S) schedule new
         g) open goto link
         k) show konnections
+        ^h) show completion history
         ^r) show repetitions
 		^u) update last modified
         ^x) toggle archived status
         ---
         T) change timer to next state
         TR) record usedtime and end timer or add usedtime
         TD) delete timer
@@ -1972,366 +1973,394 @@
 
 ### configuration {#configuration}
 
 Configuration settings for *etm* are specified in the file `cfg.yaml` located in your etm *home directory*. See [installation](#installation) for the location of this directory. When *etm* is running, you can press `F8` to open this configuration file using your system default editor for *yaml* (text) files. Note that any changes you make will not become effective until you stop and restart *etm*.
 
 Here are the options with their default values from that file. The lines beginning with `#` are comments that describe the settings.
 
-    #### begin cfg.yaml ####
-    etmversion: 4.11.18
-    # The current version of etm and this file. DO NOT EDIT. This is
-    # automatically updated when a new version of etm is installed.
-
-    ampm: true
-    # true or false. Use AM/PM format for datetimes if true else
-    # use 24 hour format. See also the show_minutes setting.
-
-    show_minutes: false
-    # true or false. If true show ":00" in agenda and forthcoming views
-    # when displaying times with zero minutes else suppress zero minutes
-    # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
-    # When ampm if false and show_minutes is true, hours will be displayed
-    # with leading zeros applicable.
-
-    dayfirst:  false
-    yearfirst: true
-    # each true or false. Whenever an ambiguous date is parsed, dayfirst
-    # and yearfirst parameters control how the information is processed
-    # using this precedence:
-    # yearfirst: true
-    # 	dayfirst: true  => YDM
-    #   dayfirst: false => YMD
-    # yearfirst: false
-    # 	dayfirst: true  => DMY
-    #   dayfirst: false => MDY
-    # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
-    # When possible, dates will also be displayed respecting these settings.
-    # I.e., the year will generally be displayed first when yearfirst is
-    # true and last otherwise. Similarly, the day will generally be displayed
-    # before the month when dayfirst is true and after the month otherwise.
-
-    beginbusy: 7
-    # non-negative integer. The number of hours after midnight to begin the
-    # busy view display of busy times for each day. The display continues
-    # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
-    # display would show busy times from 7am (7h) until 9pm (21h).
-
-    updates_interval: 0
-    # non-negative integer. If positive,  automatically check for updates
-    # every 'updates_interval' minutes. If zero, do not automatically
-    # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
-    # displayed at the right end of status bar when an update is available
-    # or a question mark when the check cannot be completed as, for
-    # example, when there is no internet connection.
-
-    locale: en_US
-    # locale abbreviation. E.g., "en_AU" for English (Australia), "en_US"
-    # for English (United States), "fr_FR" for French (France) and so
-    # forth. Google "python locale abbreviatons" for a complete list."
-
-    vi_mode: false
-    # true or false. Use vi keybindings for editing if true else use emacs
-    # style keybindings.
-
-    secret: HIr13FiYj3
-    # string to use as the secret_key for @m masked entries. E.g.
-    # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
-    # randomly generated when this file is created or when the secret
-    # value is removed and etm is restarted. WARNING: if this key is
-    # changed, any @m entries that were made before the change will be
-    # unreadable after the change.
-
-    omit_extent:
-    # A list of calendar names. Events with @c entries belonging to this
-    # list will only have their starting times displayed in agenda view
-    # and will neither appear nor cause conflicts in busy view.
-
-    keep_current: [0, 46]
-    # A list of two, non-negative integers for "weeks" and "width". If
-    # weeks is positive, the agenda for that integer number of weeks
-    # starting with the current week will be written to "current.txt" in
-    # your etm home directory and updated when necessary. The format will
-    # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
-    # in portrait mode. You could, for example, create a link to
-    # "current.txt" in a pCloud or GoogleDrive folder and always have access
-    # to your current agenda on your mobile device.
-
-    keep_next: false
-    # true or false. If true, the 'do next' view will be written to
-    # "next.txt" in your etm home directory. As with "current.txt", a link
-    # to this file could be created in a pCloud or DropBox folder for
-    # access from your mobile device.
-
-    archive_after: 0
-    # non-negative integer. If zero, do not archive items. If positive,
-    # finished tasks and events with last datetimes falling more than this
-    # number of years before the current date will automatically be
-    # archived on a daily basis.  Archived items are moved from the
-    # "items" table in the database to the "archive" table and will no
-    # longer appear in normal views. Note that unfinished tasks and
-    # records are not archived.
-
-    num_finished: 0
-    # non-negative integer
-    # If positive, when saving retain only the most recent
-    # "num_finished" completions of an infinitely repeating task,
-    # i.e., repeating without an "&c" count or an "&u" until
-    # attribute. If zero or not infinitely repeating, save all
-    # completions.
-
-    limit_skip_display: true
-    # true or false. If true, only the first instance of a task with "@o
-    # s" (overdue skip) will be displayed. For a task with an "@s" entry
-    # that is a date this will be the first instance that falls on or
-    # after the current date. Otherwise, when the "@s" entry is a
-    # datetime, this will be the first instance that falls on or after the
-    # current time.
-
-    connecting_dots: false
-    # true or false. If true, display dots connecting the item summary and
-    # the right-hand details columns in tree views.
-
-    usedtime_minutes: 1
-    # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
-    # and times are reported in hours, minutes and seconds. With 1, after
-    # rounding up to the nearest minute, times are reported as hours and minutes.
-    # Otherwise, rounding is up to the nearest integer multiple of
-    # usedtime_minutes and times are reported as floating point hours. E.g.,
-    # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
-    # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
-    # minutes and reported as 0.3 hours. Note that when rounding is specified,
-    # each "@u" timeperiod is rounded before aggregation.
-
-    usedtime_hours: 6
-    # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
-    # view to control the display of the daily used time bars. The goal is to
-    # to maximize the granularity of the bar when displaying this number of hours
-    # in the space allowed by the terminal width.
-
-    journal_name: daily
-    # Journal items with this index entry and with an @s entry will have the
-    # year and month appended to the index. E.g., with the setting
-    #   journal_name: daily
-    # this journal entry
-    #   % visited Yellowstone @s 22/6/24 @i daily
-    # would be displayed in journal view as if the index entry were
-    #   @i daily/2022/ 6
-    # thus organizing such entries by the year and month of their scheduled dates.
-    # Within each month, entries will be also ordered by the month day.
-
-    alerts:
-    # A dictionary with single-character, "alert" keys and corresponding
-    # "system command" values. Note that characters "t" (text message) and
-    # "e" (email) are already used.  The "system command" string should be
-    # a comand with any applicable arguments that could be run in a
-    # terminal. Properties of the item triggering the alert can be
-    # included in the command arguments using the syntax {prop}, e.g.,
-    # {summary} in the command string would be replaced by the summary of
-    # the item. Similarly {start} by the starting datetime, {time} by the
-    # starting time (omits the date for the current date), {when} by the time
-    # remaining until the starting datetime, {now} by the current time,
-    # {location} by the @l entry and {description} by the @d entry. E.g., If
-    # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
-    # before the starting time the string "{summary} {when}" would expand to
-    # "sales meeting in 30 minutes". E.g. on my macbook
-    #
-    #    alerts:
-    #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
-    #        ...
-    #
-    # would make the alert 'v' use the builtin text to speech sytem
-    # to speak the item's summary followed by a slight pause
-    # (the comma) and then the time remaining until the starting
-    # time, e.g., "sales meeting, in 20 minutes" would be triggered
-    # by including "@a 20m: v" in the reminder.
-
-    expansions:
-    # A dictionary with 'expansion name' keys and corresponding
-    # 'replacement string' values. E.g. with
-    #
-    #    expansions:
-    #        tennis: "@e 1h30m @a 30m: d @i personal:exercise"
-    #        ...
-    #
-    # then when "@x tennis" is entered the popup completions for
-    # "@x tennis" would offer replacement by the corresponding
-    # "@e 1h30m @a 30m: d @i personal:exercise".
-
-    sms:
-    body: '{location} {when}'
-    from:
-    server:
-    pw:
-    # Settings to send "t" (sms text message) alerts to the
-    # list of phone numbers from the item's @n attendee
-    # entries using the item's summary and the body as specified
-    # in the template below as the message. E.g., suppose you
-    # have a gmail account with email address "who457@gmail.com"
-    # and want to text alerts to Verizon moble phone (123)
-    # 456-7890. Then your sms entries should be
-    #     from:   who457@gmail.com
-    #     pw:     your gmail password
-    #     server: smtp.gmail.com:587
-    # and your item should include the following attendee entry
-    #     @n 1234567890@vzwpix.com
-    # In the illustrative phone number, @vzwpix.com is the mms
-    # gateway for Verizon. Other common mms gateways are
-    #     AT&T:     @mms.att.net
-    #     Sprint:   @pm.sprint.com
-    #     T-Mobile: @tmomail.net
-    # Note. Google "mms gateway listing" for other alternatives.
-
-    smtp:
-    body: '{location} {when}\n{description}'
-    from:
-    server:
-    id:
-    pw:
-    # Settings to send "e" (email message) alerts to the list of email
-    # addresses from the item's @n attendee entries using the item's
-    # summary as the subject and body as the message. E.g., if you have a
-    # gmail account with email address "whatever457@gmail.com", then your
-    # entries should be
-    #     from: whatever457@gmail.com
-    #     id: whatever457
-    #     pw: your gmail password
-    #     server: smtp.gmail.com
-
-    locations:
-    # A dictionary with location group names as keys and corresponding
-    # lists of locations as values. When given, do next view will group
-    # items first by the location group name and then by the location
-    # within that group. Note that locations can appear under more than
-    # one group name. E.g.,
-    # locations:
-    #    home: [home, garage, yard, phone, computer]
-    #    work: [work, phone, computer, copier, fax]
-    # Items with a location entry that does not belong to one of these
-    # location groups will be listed under 'OTHER' and items without a
-    # location entry under 'OTHER' and then tilde.
-
-    queries:
-    # A dictionary with short query "keys" and corresponding "query"
-    # values. Each "query" must be one that could be entered as the
-    # command in query view. Keys can be any short string other than
-    # 'a', 'u', 'c' or 'l' which are already in use.
-    # queries:
-    #    td: m l -q equals itemtype - and ~exists f
-    #    mi: exists u and ~exists i
-    #    arch: a exists itemtype
-    #    find: includes summary d {}
-    # The latter would allow you to enter, e.g., `find waldo` and have
-    # it expand to `includes summary d waldo` and thus locate all
-    # reminders with `waldo` either in the summary or d (the description).
-
-    style: dark
-    # dark or light. Set the defaults for dark or light terminal
-    # backgounds. Some output may not be visible unless this is set
-    # correctly for your display.
-
-    type_colors:
-    # A dictionary with type keys and corresponding named-color or hex
-    # values. The default colors are determined by the 'dark' or 'light'
-    # style setting as follows:
-    #
-    #     key           dark default        light default
-    #  -----------    -----------------   -----------------
-    #  available       'LightSkyBlue',     'DarkBlue',
-    #  begin           'Gold',             'DarkViolet',
-    #  event           'LimeGreen',        'DarkGreen',
-    #  finished        'DarkGrey',         'LightSlateGrey',
-    #  inbox           'OrangeRed',        'MediumVioletRed',
-    #  journal         'GoldenRod',        'Brown',
-    #  pastdue         'LightSalmon',      'Red',
-    #  plain           'Ivory',            'Black',
-    #  today           'Ivory bold',       'Black bold',
-    #  used            'Khaki',            'DodgerBlue',
-    #  waiting         'SlateGrey',        'DarkSlateBlue',
-    #  wrap            'ForestGreen',      'LightGrey',
-    #  running         'OrangeRed',        'Gold',
-    #  paused          'MediumVioletRed',   'DarkViolet',
-    # Explanations for the key names:
-    #     available:    available task/job reminders
-    #     begin:        begin by warnings
-    #     event:        event reminders
-    #     finished:     finished task/job reminders
-    #     inbox:        inbox reminders
-    #     journal:      journal reminders
-    #     pastdue:      pasdue task warnings
-    #     plain:        headings such as outline branches
-    #     today:        the current and following agenda date headings
-    #     used:         used time rows in engaged and used time views
-    #     waiting:      waiting job reminders (jobs with unfinished prereqs)
-    #     wrap:         before and after rows for events in agenda view with
-    #                   @w entries
-    #     running:      status bar color for 'r', running timer
-    #     paused:       status bar color for 'p', paused timer
-    #
-    # E.g., with style 'dark', the default color for 'available' is
-    # 'LightSkyBlue'. This entry
-    #   colors:
-    #       available: CornFlowerBlue
-    # would change the 'available' color to 'CornflowerBlue' while leaving
-    # the other 'dark' colors unchanged.
-    #
-    # To preview the namedcolors, download "namedcolors.py" from
-    #    "https://github.com/dagraham/etm-dgraham",
-    # open a terminal with your chosen background color and run
-    #    python3 <path to namedcolors.py>
-    # at the command prompt.
-
-    window_colors:
-    # A dictionary with style component keys and corresponding lists of
-    #    [background, foreground, attribute]
-    # components. background and foreground can either be named colors,
-    # hex colors, or ''. Attribute is an optional font attribute such
-    # as 'bold' which must, of course, be supported by the font used in
-    # your terminal. The default settings are determined by the 'dark'
-    # or 'light' style setting as follows:
-    #
-    #    key                       dark default                  light default
-    # -------------------    -----------------------------  -----------------------------
-    # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
-    # button.focused:         [DarkGreen, White]            [DarkGreen, White]
-    # details:                [, Ivory]                     [, Black]
-    # dialog shadow:          [#444444, ]                   [#444444, ]
-    # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
-    # dialog-entry:           [White, Black]                [White, Black]
-    # dialog-output:          [DarkSlateGrey, Lime]         [DimGrey, Lime]
-    # dialog.body label:      [, White]                     [, White]
-    # dialog.body:            [DarkSlateGrey, White]        [DimGrey, White]
-    # entry:                  [grey2, LightGoldenRodYellow] [Cornsilk, LightGoldenRodYellow]
-    # frame.label:            [DarkSlateGrey, White]        [DimGrey, White]
-    # menu:                   [DarkSlateGrey, White]        [DimGrey, White]
-    # menu-bar:               [grey1, White]                [grey1, White]
-    # menu-bar.selected-item: [#ffffff, #000000]            [#ffffff, #000000]
-    # menu.border:            [, #aaaaaa]                   [, #aaaaaa]
-    # not-searching:          [, #222222]                   [, #777777]
-    # query:                  [, Ivory]                     [, Black]
-    # reply:                  [grey2, DeepSkyBlue]          [Cornsilk, DeepSkyBlue]
-    # shadow:                 [#222222, ]                   [#222222, ]
-    # status:                 [grey1, White]                [grey1, White]
-    # status.key:             [, #ffaa00]                   [, #ffaa00]
-    # status.position:        [, #aaaa00]                   [, #aaaa00]
-    # text-area:              [grey2, Ivory]                [Cornsilk, Black]
-    # window.border shadow:   [, #444444]                   [, #444444]
-    # window.border:          [, #888888]                   [, #888888]
-    #
-    # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
-    # within etm itself. They are, respectively, one shade lighter and two
-    # shades darker than DarkSlateGrey.
-    #
-    # Any of the style attributes above can be modified. E.g., with style
-    # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-    #   window_colors:
-    #       text-area: [Black, White]
-    # would change the 'text-area' setting to 'Black' as the background color
-    # and 'White' as the foreground color while leaving the other style settings
-    # unchanged.
-    #### end cfg.yaml ####
+        #### begin cfg.yaml ####
+        etmversion: 5.0.12
+        # The current version of etm and this file. DO NOT EDIT. This is
+        # automatically updated when a new version of etm is installed.
+
+        ampm: true
+        # true or false. Use AM/PM format for datetimes if true else
+        # use 24 hour format. See also the show_minutes setting.
+
+        show_minutes: false
+        # true or false. If true show ":00" in agenda and forthcoming views
+        # when displaying times with zero minutes else suppress zero minutes
+        # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+        # When ampm if false and show_minutes is true, hours will be displayed
+        # with leading zeros applicable.
+
+        dayfirst:  false
+        yearfirst: true
+        # each true or false. Whenever an ambiguous date is parsed, dayfirst
+        # and yearfirst parameters control how the information is processed
+        # using this precedence:
+        # yearfirst: true
+        # 	dayfirst: true  => YDM
+        #   dayfirst: false => YMD
+        # yearfirst: false
+        # 	dayfirst: true  => DMY
+        #   dayfirst: false => MDY
+        # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+        # When possible, dates will also be displayed respecting these settings.
+        # I.e., the year will generally be displayed first when yearfirst is
+        # true and last otherwise. Similarly, the day will generally be displayed
+        # before the month when dayfirst is true and after the month otherwise.
+
+        beginbusy: 7
+        # non-negative integer. The number of hours after midnight to begin the
+        # busy view display of busy times for each day. The display continues
+        # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+        # display would show busy times from 7am (7h) until 9pm (21h).
+
+        updates_interval: 0
+        # non-negative integer. If positive,  automatically check for updates
+        # every 'updates_interval' minutes. If zero, do not automatically
+        # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
+        # displayed at the right end of status bar when an update is available
+        # or a question mark when the check cannot be completed as, for
+        # example, when there is no internet connection.
+
+        locale: en_US
+        # locale abbreviation. E.g., "en_AU" for English (Australia), "en_US"
+        # for English (United States), "fr_FR" for French (France) and so
+        # forth. Google "python locale abbreviatons" for a complete list."
+
+        vi_mode: true
+        # true or false. Use vi keybindings for editing if true else use emacs
+        # style keybindings.
+
+        secret: HIr13FiYj3
+        # string to use as the secret_key for @m masked entries. E.g.
+        # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
+        # randomly generated when this file is created or when the secret
+        # value is removed and etm is restarted. WARNING: if this key is
+        # changed, any @m entries that were made before the change will be
+        # unreadable after the change.
+
+        omit_extent:
+        # A list of calendar names. Events with @c entries belonging to this
+        # list will only have their starting times displayed in agenda view
+        # and will neither appear nor cause conflicts in busy view.
+
+        keep_current: [3, 46]
+        # A list of two, non-negative integers for "weeks" and "width". If
+        # weeks is positive, the agenda for that integer number of weeks
+        # starting with the current week will be written to "current.txt" in
+        # your etm home directory and updated when necessary. The format will
+        # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
+        # in portrait mode. You could, for example, create a link to
+        # "current.txt" in a pCloud or GoogleDrive folder and always have access
+        # to your current agenda on your mobile device.
+
+        keep_next: true
+        # true or false. If true, the 'do next' view will be written to
+        # "next.txt" in your etm home directory. As with "current.txt", a link
+        # to this file could be created in a pCloud or DropBox folder for
+        # access from your mobile device.
+
+        archive_after: 0
+        # non-negative integer. If zero, do not archive items. If positive,
+        # finished tasks and events with last datetimes falling more than this
+        # number of years before the current date will automatically be
+        # archived on a daily basis.  Archived items are moved from the
+        # "items" table in the database to the "archive" table and will no
+        # longer appear in normal views. Note that unfinished tasks and
+        # journal entries are not archived.
+
+        refresh_interval: 6
+        # 6, 12, 30 or 60. The event loop responsible for refreshing
+        # etm caches, updating alerts, timers and so forth, repeats once
+        # every refresh_interval seconds.
+
+        num_finished: 0
+        # non-negative integer
+        # If positive, when saving retain only the most recent "num_finished"
+        # completions of an infinitely repeating task, i.e., repeating without
+        # an "&c" count or an "&u" until attribute. If zero or not infinitely
+        # repeating, save all completions.
+
+        num_repetitions: 10
+        # positive integer
+        # Show at most this number of repetitions when showing repetitions
+        # with (^r) or when showing completion history (^h). In the former
+        # case these are instances for the selected item (repeating of any
+        # item type) starting from date of the selected item and in the latter
+        # case these are the completion instances (task item type). Note that
+        # the num_finished setting can affect the number available for display
+        # for the completion history.
+
+        limit_skip_display: false
+        # true or false. If true, only the first instance of a task with "@o
+        # s" (overdue skip) will be displayed. For a task with an "@s" entry
+        # that is a date this will be the first instance that falls on or
+        # after the current date. Otherwise, when the "@s" entry is a
+        # datetime, this will be the first instance that falls on or after the
+        # current time.
+
+        connecting_dots: true
+        # true or false. If true, display dots connecting the item summary and
+        # the right-hand details columns in tree views.
+
+        usedtime_minutes: 6
+        # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+        # and times are reported in hours, minutes and seconds. With 1, after
+        # rounding up to the nearest minute, times are reported as hours and minutes.
+        # Otherwise, rounding is up to the nearest integer multiple of
+        # usedtime_minutes and times are reported as floating point hours. E.g.,
+        # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+        # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+        # minutes and reported as 0.3 hours. The numbers 6, 12, 30 and 60 are
+        # characterized by the fact that each is an integer multiple of 6 and 60 is
+        # evenly divisible by each. This allows reported times to be expressed as
+        # hours and tenths of an hour for each. Note that when rounding is specified,
+        # each "@u" timeperiod is rounded before aggregation. Whatever the setting,
+        # a used time record created using the timer is accurate to the nearest
+        # second.
+
+        usedtime_hours: 6
+        # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+        # view to control the display of the daily used time bars. The goal is to
+        # to maximize the granularity of the bar when displaying this number of hours
+        # in the space allowed by the terminal width.
+
+        journal_name: daily
+        # Journal items with this index entry and with an @s entry will have the
+        # year and month appended to the index. E.g., with the setting
+        #   journal_name: daily
+        # this journal entry
+        #   % visited Yellowstone @s 22/6/24 @i daily
+        # would be displayed in journal view as if the index entry were
+        #   @i daily/2022/ 6
+        # thus organizing such entries by the year and month of their scheduled dates.
+        # Within each month, entries will be also ordered by the month day.
+
+        alerts:
+        # A dictionary with single-character, "alert" keys and corresponding
+        # "system command" values. Note that characters "t" (text message) and
+        # "e" (email) are already used.  The "system command" string should be
+        # a comand with any applicable arguments that could be run in a
+        # terminal. Properties of the item triggering the alert can be
+        # included in the command arguments using the syntax {prop}, e.g.,
+        # {summary} in the command string would be replaced by the summary of
+        # the item. Similarly {start} by the starting datetime, {time} by the
+        # starting time (omits the date for the current date), {when} by the time
+        # remaining until the starting datetime, {now} by the current time,
+        # {location} by the @l entry and {description} by the @d entry. E.g., If
+        # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+        # before the starting time the string "{summary} {when}" would expand to
+        # "sales meeting in 30 minutes". E.g. on my macbook
+        #
+        #    alerts:
+        #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
+        #        ...
+        #
+        # would make the alert 'v' use the builtin text to speech sytem
+        # to speak the item's summary followed by a slight pause
+        # (the comma) and then the time remaining until the starting
+        # time, e.g., "sales meeting, in 20 minutes" would be triggered
+        # by including "@a 20m: v" in the reminder.
+
+        expansions:
+        # A dictionary with 'expansion name' keys and corresponding
+        # 'replacement string' values. E.g. with
+        #
+        #    expansions:
+        #        tennis: "@e 1h30m @a 30m: d @i personal:exercise"
+        #        ...
+        #
+        # then when "@x tennis" is entered the popup completions for
+        # "@x tennis" would offer replacement by the corresponding
+        # "@e 1h30m @a 30m: d @i personal:exercise".
+
+        sms:
+        body: '{location} {when}'
+        from: 'None'
+        server: 'None'
+        pw: 'None'
+        # Settings to send "t" (sms text message) alerts to the
+        # list of phone numbers from the item's @n attendee
+        # entries using the item's summary and the body as specified
+        # in the template below as the message. E.g., suppose you
+        # have a gmail account with email address "who457@gmail.com"
+        # and want to text alerts to Verizon moble phone (123)
+        # 456-7890. Then your sms entries should be
+        #     from:   who457@gmail.com
+        #     pw:     your gmail password
+        #     server: smtp.gmail.com:587
+        # and your item should include the following attendee entry
+        #     @n 1234567890@vzwpix.com
+        # In the illustrative phone number, @vzwpix.com is the mms
+        # gateway for Verizon. Other common mms gateways are
+        #     AT&T:     @mms.att.net
+        #     Sprint:   @pm.sprint.com
+        #     T-Mobile: @tmomail.net
+        # Note. Google "mms gateway listing" for other alternatives.
+
+        smtp:
+        body: '{location} {when}\n{description}'
+        from: 'None'
+        server: 'None'
+        id: 'None'
+        pw: 'None'
+        # Settings to send "e" (email message) alerts to the list of email
+        # addresses from the item's @n attendee entries using the item's
+        # summary as the subject and body as the message. E.g., if you have a
+        # gmail account with email address "whatever457@gmail.com", then your
+        # entries should be
+        #     from: whatever457@gmail.com
+        #     id: whatever457
+        #     pw: your gmail password
+        #     server: smtp.gmail.com
+
+        locations:
+        # A dictionary with location group names as keys and corresponding
+        # lists of locations as values. When given, do next view will group
+        # items first by the location group name and then by the location
+        # within that group. Note that locations can appear under more than
+        # one group name. E.g.,
+        # locations:
+        #    home: [home, garage, yard, phone, computer]
+        #    work: [work, phone, computer, copier, fax]
+        # Items with a location entry that does not belong to one of these
+        # location groups will be listed under 'OTHER' and items without a
+        # location entry under 'OTHER' and then tilde.
+
+        queries:
+        td: 'm l -q equals itemtype - and ~exists f'
+        ui: 'u i[:1]; MMM YYYY; i[1:2] -a d'
+        si: 's i[:1]; MMM YYYY; i[1:2] -a u, d'
+        mi: 'exists u and ~exists i'
+        arch: 'a exists itemtype'
+        uw: 'u WWW; ddd D -b weekbeg - 1w -e weekend'
+        find: 'includes summary d {}'
+        f: 'includes summary d {}'
+        index: 's MMM YYYY; ddd D -q in i {}'
+        # A dictionary with short query "keys" and corresponding "query"
+        # values. Each "query" must be one that could be entered as the
+        # command in query view. Keys can be any short string other than
+        # 'a', 'u', 'c' or 'l' which are already in use.
+        # queries:
+        #    td: m l -q equals itemtype - and ~exists f
+        #    mi: exists u and ~exists i
+        #    arch: a exists itemtype
+        #    find: includes summary d {}
+        # The latter would allow you to enter, e.g., `find waldo` and have
+        # it expand to `includes summary d waldo` and thus locate all
+        # reminders with `waldo` either in the summary or d (the description).
+
+        style: dark
+        # dark or light. Set the defaults for dark or light terminal
+        # backgounds. Some output may not be visible unless this is set
+        # correctly for your display.
+
+        type_colors:
+        # A dictionary with type keys and corresponding named-color or hex
+        # values. The default colors are determined by the 'dark' or 'light'
+        # style setting as follows:
+        #
+        #     key           dark default        light default
+        #  -----------    -----------------   -----------------
+        #  available       'LightSkyBlue',     'DarkBlue',
+        #  begin           'Gold',             'DarkViolet',
+        #  event           'LimeGreen',        'DarkGreen',
+        #  finished        'DarkGrey',         'LightSlateGrey',
+        #  inbox           'OrangeRed',        'MediumVioletRed',
+        #  journal         'GoldenRod',        'Brown',
+        #  pastdue         'LightSalmon',      'Red',
+        #  plain           'Ivory',            'Black',
+        #  today           'Ivory bold',       'Black bold',
+        #  used            'Khaki',            'DodgerBlue',
+        #  waiting         'SlateGrey',        'DarkSlateBlue',
+        #  wrap            'ForestGreen',      'LightGrey',
+        #  running         'OrangeRed',        'Gold',
+        #  paused          'MediumVioletRed',   'DarkViolet',
+        # Explanations for the key names:
+        #     available:    available task/job reminders
+        #     begin:        begin by warnings
+        #     event:        event reminders
+        #     finished:     finished task/job reminders
+        #     inbox:        inbox reminders
+        #     journal:      journal reminders
+        #     pastdue:      pasdue task warnings
+        #     plain:        headings such as outline branches
+        #     today:        the current and following agenda date headings
+        #     used:         used time rows in engaged and used time views
+        #     waiting:      waiting job reminders (jobs with unfinished prereqs)
+        #     wrap:         before and after rows for events in agenda view with
+        #                   @w entries
+        #     running:      status bar color for 'r', running timer
+        #     paused:       status bar color for 'p', paused timer
+        #
+        # E.g., with style 'dark', the default color for 'available' is
+        # 'LightSkyBlue'. This entry
+        #   colors:
+        #       available: CornFlowerBlue
+        # would change the 'available' color to 'CornflowerBlue' while leaving
+        # the other 'dark' colors unchanged.
+        #
+        # To preview the namedcolors, download "namedcolors.py" from
+        #    "https://github.com/dagraham/etm-dgraham",
+        # open a terminal with your chosen background color and run
+        #    python3 <path to namedcolors.py>
+        # at the command prompt.
+
+        window_colors:
+        # A dictionary with style component keys and corresponding lists of
+        #    [background, foreground, attribute]
+        # components. background and foreground can either be named colors,
+        # hex colors, or ''. Attribute is an optional font attribute such
+        # as 'bold' which must, of course, be supported by the font used in
+        # your terminal. The default settings are determined by the 'dark'
+        # or 'light' style setting as follows:
+        #
+        #    key                       dark default                  light default
+        # -------------------    -----------------------------  -----------------------------
+        # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
+        # button.focused:         [DarkGreen, White]            [DarkGreen, White]
+        # details:                [, Ivory]                     [, Black]
+        # dialog shadow:          [#444444, ]                   [#444444, ]
+        # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
+        # dialog-entry:           [White, Black]                [White, Black]
+        # dialog-output:          [DarkSlateGrey, Lime]         [DimGrey, Lime]
+        # dialog.body label:      [, White]                     [, White]
+        # dialog.body:            [DarkSlateGrey, White]        [DimGrey, White]
+        # entry:                  [grey2, LightGoldenRodYellow] [Cornsilk, LightGoldenRodYellow]
+        # frame.label:            [DarkSlateGrey, White]        [DimGrey, White]
+        # menu:                   [DarkSlateGrey, White]        [DimGrey, White]
+        # menu-bar:               [grey1, White]                [grey1, White]
+        # menu-bar.selected-item: [#ffffff, #000000]            [#ffffff, #000000]
+        # menu.border:            [, #aaaaaa]                   [, #aaaaaa]
+        # not-searching:          [, #222222]                   [, #777777]
+        # query:                  [, Ivory]                     [, Black]
+        # reply:                  [grey2, DeepSkyBlue]          [Cornsilk, DeepSkyBlue]
+        # shadow:                 [#222222, ]                   [#222222, ]
+        # status:                 [grey1, White]                [grey1, White]
+        # status.key:             [, #ffaa00]                   [, #ffaa00]
+        # status.position:        [, #aaaa00]                   [, #aaaa00]
+        # text-area:              [grey2, Ivory]                [Cornsilk, Black]
+        # window.border shadow:   [, #444444]                   [, #444444]
+        # window.border:          [, #888888]                   [, #888888]
+        #
+        # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
+        # within etm itself. They are, respectively, one shade lighter and two
+        # shades darker than DarkSlateGrey.
+        #
+        # Any of the style attributes above can be modified. E.g., with style
+        # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
+        #   window_colors:
+        #       text-area: [Black, White]
+        # would change the 'text-area' setting to 'Black' as the background color
+        # and 'White' as the foreground color while leaving the other style settings
+        # unchanged.
+        #### end cfg.yaml ####
 
 
 See [Saved Queries](#saved-queries) for more information about queries that allow for replaceable parameters.
 
 Note that in the 'dictionary' entries above, the components must be indented (using 2 spaces not tabs). E.g., the illustrative alert entry would be:
 
 	alerts:
```

### Comparing `etm-dgraham-5.0.9/README.md` & `etm-dgraham-5.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1195,14 +1195,15 @@
         D) delete
         F) finish
         P) toggle pin
         R) reschedule
         S) schedule new
         g) open goto link
         k) show konnections
+        ^h) show completion history
         ^r) show repetitions
 		^u) update last modified
         ^x) toggle archived status
         ---
         T) change timer to next state
         TR) record usedtime and end timer or add usedtime
         TD) delete timer
@@ -1948,366 +1949,394 @@
 
 ### configuration {#configuration}
 
 Configuration settings for *etm* are specified in the file `cfg.yaml` located in your etm *home directory*. See [installation](#installation) for the location of this directory. When *etm* is running, you can press `F8` to open this configuration file using your system default editor for *yaml* (text) files. Note that any changes you make will not become effective until you stop and restart *etm*.
 
 Here are the options with their default values from that file. The lines beginning with `#` are comments that describe the settings.
 
-    #### begin cfg.yaml ####
-    etmversion: 4.11.18
-    # The current version of etm and this file. DO NOT EDIT. This is
-    # automatically updated when a new version of etm is installed.
-
-    ampm: true
-    # true or false. Use AM/PM format for datetimes if true else
-    # use 24 hour format. See also the show_minutes setting.
-
-    show_minutes: false
-    # true or false. If true show ":00" in agenda and forthcoming views
-    # when displaying times with zero minutes else suppress zero minutes
-    # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
-    # When ampm if false and show_minutes is true, hours will be displayed
-    # with leading zeros applicable.
-
-    dayfirst:  false
-    yearfirst: true
-    # each true or false. Whenever an ambiguous date is parsed, dayfirst
-    # and yearfirst parameters control how the information is processed
-    # using this precedence:
-    # yearfirst: true
-    # 	dayfirst: true  => YDM
-    #   dayfirst: false => YMD
-    # yearfirst: false
-    # 	dayfirst: true  => DMY
-    #   dayfirst: false => MDY
-    # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
-    # When possible, dates will also be displayed respecting these settings.
-    # I.e., the year will generally be displayed first when yearfirst is
-    # true and last otherwise. Similarly, the day will generally be displayed
-    # before the month when dayfirst is true and after the month otherwise.
-
-    beginbusy: 7
-    # non-negative integer. The number of hours after midnight to begin the
-    # busy view display of busy times for each day. The display continues
-    # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
-    # display would show busy times from 7am (7h) until 9pm (21h).
-
-    updates_interval: 0
-    # non-negative integer. If positive,  automatically check for updates
-    # every 'updates_interval' minutes. If zero, do not automatically
-    # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
-    # displayed at the right end of status bar when an update is available
-    # or a question mark when the check cannot be completed as, for
-    # example, when there is no internet connection.
-
-    locale: en_US
-    # locale abbreviation. E.g., "en_AU" for English (Australia), "en_US"
-    # for English (United States), "fr_FR" for French (France) and so
-    # forth. Google "python locale abbreviatons" for a complete list."
-
-    vi_mode: false
-    # true or false. Use vi keybindings for editing if true else use emacs
-    # style keybindings.
-
-    secret: HIr13FiYj3
-    # string to use as the secret_key for @m masked entries. E.g.
-    # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
-    # randomly generated when this file is created or when the secret
-    # value is removed and etm is restarted. WARNING: if this key is
-    # changed, any @m entries that were made before the change will be
-    # unreadable after the change.
-
-    omit_extent:
-    # A list of calendar names. Events with @c entries belonging to this
-    # list will only have their starting times displayed in agenda view
-    # and will neither appear nor cause conflicts in busy view.
-
-    keep_current: [0, 46]
-    # A list of two, non-negative integers for "weeks" and "width". If
-    # weeks is positive, the agenda for that integer number of weeks
-    # starting with the current week will be written to "current.txt" in
-    # your etm home directory and updated when necessary. The format will
-    # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
-    # in portrait mode. You could, for example, create a link to
-    # "current.txt" in a pCloud or GoogleDrive folder and always have access
-    # to your current agenda on your mobile device.
-
-    keep_next: false
-    # true or false. If true, the 'do next' view will be written to
-    # "next.txt" in your etm home directory. As with "current.txt", a link
-    # to this file could be created in a pCloud or DropBox folder for
-    # access from your mobile device.
-
-    archive_after: 0
-    # non-negative integer. If zero, do not archive items. If positive,
-    # finished tasks and events with last datetimes falling more than this
-    # number of years before the current date will automatically be
-    # archived on a daily basis.  Archived items are moved from the
-    # "items" table in the database to the "archive" table and will no
-    # longer appear in normal views. Note that unfinished tasks and
-    # records are not archived.
-
-    num_finished: 0
-    # non-negative integer
-    # If positive, when saving retain only the most recent
-    # "num_finished" completions of an infinitely repeating task,
-    # i.e., repeating without an "&c" count or an "&u" until
-    # attribute. If zero or not infinitely repeating, save all
-    # completions.
-
-    limit_skip_display: true
-    # true or false. If true, only the first instance of a task with "@o
-    # s" (overdue skip) will be displayed. For a task with an "@s" entry
-    # that is a date this will be the first instance that falls on or
-    # after the current date. Otherwise, when the "@s" entry is a
-    # datetime, this will be the first instance that falls on or after the
-    # current time.
-
-    connecting_dots: false
-    # true or false. If true, display dots connecting the item summary and
-    # the right-hand details columns in tree views.
-
-    usedtime_minutes: 1
-    # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
-    # and times are reported in hours, minutes and seconds. With 1, after
-    # rounding up to the nearest minute, times are reported as hours and minutes.
-    # Otherwise, rounding is up to the nearest integer multiple of
-    # usedtime_minutes and times are reported as floating point hours. E.g.,
-    # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
-    # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
-    # minutes and reported as 0.3 hours. Note that when rounding is specified,
-    # each "@u" timeperiod is rounded before aggregation.
-
-    usedtime_hours: 6
-    # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
-    # view to control the display of the daily used time bars. The goal is to
-    # to maximize the granularity of the bar when displaying this number of hours
-    # in the space allowed by the terminal width.
-
-    journal_name: daily
-    # Journal items with this index entry and with an @s entry will have the
-    # year and month appended to the index. E.g., with the setting
-    #   journal_name: daily
-    # this journal entry
-    #   % visited Yellowstone @s 22/6/24 @i daily
-    # would be displayed in journal view as if the index entry were
-    #   @i daily/2022/ 6
-    # thus organizing such entries by the year and month of their scheduled dates.
-    # Within each month, entries will be also ordered by the month day.
-
-    alerts:
-    # A dictionary with single-character, "alert" keys and corresponding
-    # "system command" values. Note that characters "t" (text message) and
-    # "e" (email) are already used.  The "system command" string should be
-    # a comand with any applicable arguments that could be run in a
-    # terminal. Properties of the item triggering the alert can be
-    # included in the command arguments using the syntax {prop}, e.g.,
-    # {summary} in the command string would be replaced by the summary of
-    # the item. Similarly {start} by the starting datetime, {time} by the
-    # starting time (omits the date for the current date), {when} by the time
-    # remaining until the starting datetime, {now} by the current time,
-    # {location} by the @l entry and {description} by the @d entry. E.g., If
-    # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
-    # before the starting time the string "{summary} {when}" would expand to
-    # "sales meeting in 30 minutes". E.g. on my macbook
-    #
-    #    alerts:
-    #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
-    #        ...
-    #
-    # would make the alert 'v' use the builtin text to speech sytem
-    # to speak the item's summary followed by a slight pause
-    # (the comma) and then the time remaining until the starting
-    # time, e.g., "sales meeting, in 20 minutes" would be triggered
-    # by including "@a 20m: v" in the reminder.
-
-    expansions:
-    # A dictionary with 'expansion name' keys and corresponding
-    # 'replacement string' values. E.g. with
-    #
-    #    expansions:
-    #        tennis: "@e 1h30m @a 30m: d @i personal:exercise"
-    #        ...
-    #
-    # then when "@x tennis" is entered the popup completions for
-    # "@x tennis" would offer replacement by the corresponding
-    # "@e 1h30m @a 30m: d @i personal:exercise".
-
-    sms:
-    body: '{location} {when}'
-    from:
-    server:
-    pw:
-    # Settings to send "t" (sms text message) alerts to the
-    # list of phone numbers from the item's @n attendee
-    # entries using the item's summary and the body as specified
-    # in the template below as the message. E.g., suppose you
-    # have a gmail account with email address "who457@gmail.com"
-    # and want to text alerts to Verizon moble phone (123)
-    # 456-7890. Then your sms entries should be
-    #     from:   who457@gmail.com
-    #     pw:     your gmail password
-    #     server: smtp.gmail.com:587
-    # and your item should include the following attendee entry
-    #     @n 1234567890@vzwpix.com
-    # In the illustrative phone number, @vzwpix.com is the mms
-    # gateway for Verizon. Other common mms gateways are
-    #     AT&T:     @mms.att.net
-    #     Sprint:   @pm.sprint.com
-    #     T-Mobile: @tmomail.net
-    # Note. Google "mms gateway listing" for other alternatives.
-
-    smtp:
-    body: '{location} {when}\n{description}'
-    from:
-    server:
-    id:
-    pw:
-    # Settings to send "e" (email message) alerts to the list of email
-    # addresses from the item's @n attendee entries using the item's
-    # summary as the subject and body as the message. E.g., if you have a
-    # gmail account with email address "whatever457@gmail.com", then your
-    # entries should be
-    #     from: whatever457@gmail.com
-    #     id: whatever457
-    #     pw: your gmail password
-    #     server: smtp.gmail.com
-
-    locations:
-    # A dictionary with location group names as keys and corresponding
-    # lists of locations as values. When given, do next view will group
-    # items first by the location group name and then by the location
-    # within that group. Note that locations can appear under more than
-    # one group name. E.g.,
-    # locations:
-    #    home: [home, garage, yard, phone, computer]
-    #    work: [work, phone, computer, copier, fax]
-    # Items with a location entry that does not belong to one of these
-    # location groups will be listed under 'OTHER' and items without a
-    # location entry under 'OTHER' and then tilde.
-
-    queries:
-    # A dictionary with short query "keys" and corresponding "query"
-    # values. Each "query" must be one that could be entered as the
-    # command in query view. Keys can be any short string other than
-    # 'a', 'u', 'c' or 'l' which are already in use.
-    # queries:
-    #    td: m l -q equals itemtype - and ~exists f
-    #    mi: exists u and ~exists i
-    #    arch: a exists itemtype
-    #    find: includes summary d {}
-    # The latter would allow you to enter, e.g., `find waldo` and have
-    # it expand to `includes summary d waldo` and thus locate all
-    # reminders with `waldo` either in the summary or d (the description).
-
-    style: dark
-    # dark or light. Set the defaults for dark or light terminal
-    # backgounds. Some output may not be visible unless this is set
-    # correctly for your display.
-
-    type_colors:
-    # A dictionary with type keys and corresponding named-color or hex
-    # values. The default colors are determined by the 'dark' or 'light'
-    # style setting as follows:
-    #
-    #     key           dark default        light default
-    #  -----------    -----------------   -----------------
-    #  available       'LightSkyBlue',     'DarkBlue',
-    #  begin           'Gold',             'DarkViolet',
-    #  event           'LimeGreen',        'DarkGreen',
-    #  finished        'DarkGrey',         'LightSlateGrey',
-    #  inbox           'OrangeRed',        'MediumVioletRed',
-    #  journal         'GoldenRod',        'Brown',
-    #  pastdue         'LightSalmon',      'Red',
-    #  plain           'Ivory',            'Black',
-    #  today           'Ivory bold',       'Black bold',
-    #  used            'Khaki',            'DodgerBlue',
-    #  waiting         'SlateGrey',        'DarkSlateBlue',
-    #  wrap            'ForestGreen',      'LightGrey',
-    #  running         'OrangeRed',        'Gold',
-    #  paused          'MediumVioletRed',   'DarkViolet',
-    # Explanations for the key names:
-    #     available:    available task/job reminders
-    #     begin:        begin by warnings
-    #     event:        event reminders
-    #     finished:     finished task/job reminders
-    #     inbox:        inbox reminders
-    #     journal:      journal reminders
-    #     pastdue:      pasdue task warnings
-    #     plain:        headings such as outline branches
-    #     today:        the current and following agenda date headings
-    #     used:         used time rows in engaged and used time views
-    #     waiting:      waiting job reminders (jobs with unfinished prereqs)
-    #     wrap:         before and after rows for events in agenda view with
-    #                   @w entries
-    #     running:      status bar color for 'r', running timer
-    #     paused:       status bar color for 'p', paused timer
-    #
-    # E.g., with style 'dark', the default color for 'available' is
-    # 'LightSkyBlue'. This entry
-    #   colors:
-    #       available: CornFlowerBlue
-    # would change the 'available' color to 'CornflowerBlue' while leaving
-    # the other 'dark' colors unchanged.
-    #
-    # To preview the namedcolors, download "namedcolors.py" from
-    #    "https://github.com/dagraham/etm-dgraham",
-    # open a terminal with your chosen background color and run
-    #    python3 <path to namedcolors.py>
-    # at the command prompt.
-
-    window_colors:
-    # A dictionary with style component keys and corresponding lists of
-    #    [background, foreground, attribute]
-    # components. background and foreground can either be named colors,
-    # hex colors, or ''. Attribute is an optional font attribute such
-    # as 'bold' which must, of course, be supported by the font used in
-    # your terminal. The default settings are determined by the 'dark'
-    # or 'light' style setting as follows:
-    #
-    #    key                       dark default                  light default
-    # -------------------    -----------------------------  -----------------------------
-    # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
-    # button.focused:         [DarkGreen, White]            [DarkGreen, White]
-    # details:                [, Ivory]                     [, Black]
-    # dialog shadow:          [#444444, ]                   [#444444, ]
-    # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
-    # dialog-entry:           [White, Black]                [White, Black]
-    # dialog-output:          [DarkSlateGrey, Lime]         [DimGrey, Lime]
-    # dialog.body label:      [, White]                     [, White]
-    # dialog.body:            [DarkSlateGrey, White]        [DimGrey, White]
-    # entry:                  [grey2, LightGoldenRodYellow] [Cornsilk, LightGoldenRodYellow]
-    # frame.label:            [DarkSlateGrey, White]        [DimGrey, White]
-    # menu:                   [DarkSlateGrey, White]        [DimGrey, White]
-    # menu-bar:               [grey1, White]                [grey1, White]
-    # menu-bar.selected-item: [#ffffff, #000000]            [#ffffff, #000000]
-    # menu.border:            [, #aaaaaa]                   [, #aaaaaa]
-    # not-searching:          [, #222222]                   [, #777777]
-    # query:                  [, Ivory]                     [, Black]
-    # reply:                  [grey2, DeepSkyBlue]          [Cornsilk, DeepSkyBlue]
-    # shadow:                 [#222222, ]                   [#222222, ]
-    # status:                 [grey1, White]                [grey1, White]
-    # status.key:             [, #ffaa00]                   [, #ffaa00]
-    # status.position:        [, #aaaa00]                   [, #aaaa00]
-    # text-area:              [grey2, Ivory]                [Cornsilk, Black]
-    # window.border shadow:   [, #444444]                   [, #444444]
-    # window.border:          [, #888888]                   [, #888888]
-    #
-    # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
-    # within etm itself. They are, respectively, one shade lighter and two
-    # shades darker than DarkSlateGrey.
-    #
-    # Any of the style attributes above can be modified. E.g., with style
-    # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-    #   window_colors:
-    #       text-area: [Black, White]
-    # would change the 'text-area' setting to 'Black' as the background color
-    # and 'White' as the foreground color while leaving the other style settings
-    # unchanged.
-    #### end cfg.yaml ####
+        #### begin cfg.yaml ####
+        etmversion: 5.0.12
+        # The current version of etm and this file. DO NOT EDIT. This is
+        # automatically updated when a new version of etm is installed.
+
+        ampm: true
+        # true or false. Use AM/PM format for datetimes if true else
+        # use 24 hour format. See also the show_minutes setting.
+
+        show_minutes: false
+        # true or false. If true show ":00" in agenda and forthcoming views
+        # when displaying times with zero minutes else suppress zero minutes
+        # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+        # When ampm if false and show_minutes is true, hours will be displayed
+        # with leading zeros applicable.
+
+        dayfirst:  false
+        yearfirst: true
+        # each true or false. Whenever an ambiguous date is parsed, dayfirst
+        # and yearfirst parameters control how the information is processed
+        # using this precedence:
+        # yearfirst: true
+        # 	dayfirst: true  => YDM
+        #   dayfirst: false => YMD
+        # yearfirst: false
+        # 	dayfirst: true  => DMY
+        #   dayfirst: false => MDY
+        # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+        # When possible, dates will also be displayed respecting these settings.
+        # I.e., the year will generally be displayed first when yearfirst is
+        # true and last otherwise. Similarly, the day will generally be displayed
+        # before the month when dayfirst is true and after the month otherwise.
+
+        beginbusy: 7
+        # non-negative integer. The number of hours after midnight to begin the
+        # busy view display of busy times for each day. The display continues
+        # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+        # display would show busy times from 7am (7h) until 9pm (21h).
+
+        updates_interval: 0
+        # non-negative integer. If positive,  automatically check for updates
+        # every 'updates_interval' minutes. If zero, do not automatically
+        # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
+        # displayed at the right end of status bar when an update is available
+        # or a question mark when the check cannot be completed as, for
+        # example, when there is no internet connection.
+
+        locale: en_US
+        # locale abbreviation. E.g., "en_AU" for English (Australia), "en_US"
+        # for English (United States), "fr_FR" for French (France) and so
+        # forth. Google "python locale abbreviatons" for a complete list."
+
+        vi_mode: true
+        # true or false. Use vi keybindings for editing if true else use emacs
+        # style keybindings.
+
+        secret: HIr13FiYj3
+        # string to use as the secret_key for @m masked entries. E.g.
+        # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
+        # randomly generated when this file is created or when the secret
+        # value is removed and etm is restarted. WARNING: if this key is
+        # changed, any @m entries that were made before the change will be
+        # unreadable after the change.
+
+        omit_extent:
+        # A list of calendar names. Events with @c entries belonging to this
+        # list will only have their starting times displayed in agenda view
+        # and will neither appear nor cause conflicts in busy view.
+
+        keep_current: [3, 46]
+        # A list of two, non-negative integers for "weeks" and "width". If
+        # weeks is positive, the agenda for that integer number of weeks
+        # starting with the current week will be written to "current.txt" in
+        # your etm home directory and updated when necessary. The format will
+        # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
+        # in portrait mode. You could, for example, create a link to
+        # "current.txt" in a pCloud or GoogleDrive folder and always have access
+        # to your current agenda on your mobile device.
+
+        keep_next: true
+        # true or false. If true, the 'do next' view will be written to
+        # "next.txt" in your etm home directory. As with "current.txt", a link
+        # to this file could be created in a pCloud or DropBox folder for
+        # access from your mobile device.
+
+        archive_after: 0
+        # non-negative integer. If zero, do not archive items. If positive,
+        # finished tasks and events with last datetimes falling more than this
+        # number of years before the current date will automatically be
+        # archived on a daily basis.  Archived items are moved from the
+        # "items" table in the database to the "archive" table and will no
+        # longer appear in normal views. Note that unfinished tasks and
+        # journal entries are not archived.
+
+        refresh_interval: 6
+        # 6, 12, 30 or 60. The event loop responsible for refreshing
+        # etm caches, updating alerts, timers and so forth, repeats once
+        # every refresh_interval seconds.
+
+        num_finished: 0
+        # non-negative integer
+        # If positive, when saving retain only the most recent "num_finished"
+        # completions of an infinitely repeating task, i.e., repeating without
+        # an "&c" count or an "&u" until attribute. If zero or not infinitely
+        # repeating, save all completions.
+
+        num_repetitions: 10
+        # positive integer
+        # Show at most this number of repetitions when showing repetitions
+        # with (^r) or when showing completion history (^h). In the former
+        # case these are instances for the selected item (repeating of any
+        # item type) starting from date of the selected item and in the latter
+        # case these are the completion instances (task item type). Note that
+        # the num_finished setting can affect the number available for display
+        # for the completion history.
+
+        limit_skip_display: false
+        # true or false. If true, only the first instance of a task with "@o
+        # s" (overdue skip) will be displayed. For a task with an "@s" entry
+        # that is a date this will be the first instance that falls on or
+        # after the current date. Otherwise, when the "@s" entry is a
+        # datetime, this will be the first instance that falls on or after the
+        # current time.
+
+        connecting_dots: true
+        # true or false. If true, display dots connecting the item summary and
+        # the right-hand details columns in tree views.
+
+        usedtime_minutes: 6
+        # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+        # and times are reported in hours, minutes and seconds. With 1, after
+        # rounding up to the nearest minute, times are reported as hours and minutes.
+        # Otherwise, rounding is up to the nearest integer multiple of
+        # usedtime_minutes and times are reported as floating point hours. E.g.,
+        # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+        # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+        # minutes and reported as 0.3 hours. The numbers 6, 12, 30 and 60 are
+        # characterized by the fact that each is an integer multiple of 6 and 60 is
+        # evenly divisible by each. This allows reported times to be expressed as
+        # hours and tenths of an hour for each. Note that when rounding is specified,
+        # each "@u" timeperiod is rounded before aggregation. Whatever the setting,
+        # a used time record created using the timer is accurate to the nearest
+        # second.
+
+        usedtime_hours: 6
+        # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+        # view to control the display of the daily used time bars. The goal is to
+        # to maximize the granularity of the bar when displaying this number of hours
+        # in the space allowed by the terminal width.
+
+        journal_name: daily
+        # Journal items with this index entry and with an @s entry will have the
+        # year and month appended to the index. E.g., with the setting
+        #   journal_name: daily
+        # this journal entry
+        #   % visited Yellowstone @s 22/6/24 @i daily
+        # would be displayed in journal view as if the index entry were
+        #   @i daily/2022/ 6
+        # thus organizing such entries by the year and month of their scheduled dates.
+        # Within each month, entries will be also ordered by the month day.
+
+        alerts:
+        # A dictionary with single-character, "alert" keys and corresponding
+        # "system command" values. Note that characters "t" (text message) and
+        # "e" (email) are already used.  The "system command" string should be
+        # a comand with any applicable arguments that could be run in a
+        # terminal. Properties of the item triggering the alert can be
+        # included in the command arguments using the syntax {prop}, e.g.,
+        # {summary} in the command string would be replaced by the summary of
+        # the item. Similarly {start} by the starting datetime, {time} by the
+        # starting time (omits the date for the current date), {when} by the time
+        # remaining until the starting datetime, {now} by the current time,
+        # {location} by the @l entry and {description} by the @d entry. E.g., If
+        # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+        # before the starting time the string "{summary} {when}" would expand to
+        # "sales meeting in 30 minutes". E.g. on my macbook
+        #
+        #    alerts:
+        #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
+        #        ...
+        #
+        # would make the alert 'v' use the builtin text to speech sytem
+        # to speak the item's summary followed by a slight pause
+        # (the comma) and then the time remaining until the starting
+        # time, e.g., "sales meeting, in 20 minutes" would be triggered
+        # by including "@a 20m: v" in the reminder.
+
+        expansions:
+        # A dictionary with 'expansion name' keys and corresponding
+        # 'replacement string' values. E.g. with
+        #
+        #    expansions:
+        #        tennis: "@e 1h30m @a 30m: d @i personal:exercise"
+        #        ...
+        #
+        # then when "@x tennis" is entered the popup completions for
+        # "@x tennis" would offer replacement by the corresponding
+        # "@e 1h30m @a 30m: d @i personal:exercise".
+
+        sms:
+        body: '{location} {when}'
+        from: 'None'
+        server: 'None'
+        pw: 'None'
+        # Settings to send "t" (sms text message) alerts to the
+        # list of phone numbers from the item's @n attendee
+        # entries using the item's summary and the body as specified
+        # in the template below as the message. E.g., suppose you
+        # have a gmail account with email address "who457@gmail.com"
+        # and want to text alerts to Verizon moble phone (123)
+        # 456-7890. Then your sms entries should be
+        #     from:   who457@gmail.com
+        #     pw:     your gmail password
+        #     server: smtp.gmail.com:587
+        # and your item should include the following attendee entry
+        #     @n 1234567890@vzwpix.com
+        # In the illustrative phone number, @vzwpix.com is the mms
+        # gateway for Verizon. Other common mms gateways are
+        #     AT&T:     @mms.att.net
+        #     Sprint:   @pm.sprint.com
+        #     T-Mobile: @tmomail.net
+        # Note. Google "mms gateway listing" for other alternatives.
+
+        smtp:
+        body: '{location} {when}\n{description}'
+        from: 'None'
+        server: 'None'
+        id: 'None'
+        pw: 'None'
+        # Settings to send "e" (email message) alerts to the list of email
+        # addresses from the item's @n attendee entries using the item's
+        # summary as the subject and body as the message. E.g., if you have a
+        # gmail account with email address "whatever457@gmail.com", then your
+        # entries should be
+        #     from: whatever457@gmail.com
+        #     id: whatever457
+        #     pw: your gmail password
+        #     server: smtp.gmail.com
+
+        locations:
+        # A dictionary with location group names as keys and corresponding
+        # lists of locations as values. When given, do next view will group
+        # items first by the location group name and then by the location
+        # within that group. Note that locations can appear under more than
+        # one group name. E.g.,
+        # locations:
+        #    home: [home, garage, yard, phone, computer]
+        #    work: [work, phone, computer, copier, fax]
+        # Items with a location entry that does not belong to one of these
+        # location groups will be listed under 'OTHER' and items without a
+        # location entry under 'OTHER' and then tilde.
+
+        queries:
+        td: 'm l -q equals itemtype - and ~exists f'
+        ui: 'u i[:1]; MMM YYYY; i[1:2] -a d'
+        si: 's i[:1]; MMM YYYY; i[1:2] -a u, d'
+        mi: 'exists u and ~exists i'
+        arch: 'a exists itemtype'
+        uw: 'u WWW; ddd D -b weekbeg - 1w -e weekend'
+        find: 'includes summary d {}'
+        f: 'includes summary d {}'
+        index: 's MMM YYYY; ddd D -q in i {}'
+        # A dictionary with short query "keys" and corresponding "query"
+        # values. Each "query" must be one that could be entered as the
+        # command in query view. Keys can be any short string other than
+        # 'a', 'u', 'c' or 'l' which are already in use.
+        # queries:
+        #    td: m l -q equals itemtype - and ~exists f
+        #    mi: exists u and ~exists i
+        #    arch: a exists itemtype
+        #    find: includes summary d {}
+        # The latter would allow you to enter, e.g., `find waldo` and have
+        # it expand to `includes summary d waldo` and thus locate all
+        # reminders with `waldo` either in the summary or d (the description).
+
+        style: dark
+        # dark or light. Set the defaults for dark or light terminal
+        # backgounds. Some output may not be visible unless this is set
+        # correctly for your display.
+
+        type_colors:
+        # A dictionary with type keys and corresponding named-color or hex
+        # values. The default colors are determined by the 'dark' or 'light'
+        # style setting as follows:
+        #
+        #     key           dark default        light default
+        #  -----------    -----------------   -----------------
+        #  available       'LightSkyBlue',     'DarkBlue',
+        #  begin           'Gold',             'DarkViolet',
+        #  event           'LimeGreen',        'DarkGreen',
+        #  finished        'DarkGrey',         'LightSlateGrey',
+        #  inbox           'OrangeRed',        'MediumVioletRed',
+        #  journal         'GoldenRod',        'Brown',
+        #  pastdue         'LightSalmon',      'Red',
+        #  plain           'Ivory',            'Black',
+        #  today           'Ivory bold',       'Black bold',
+        #  used            'Khaki',            'DodgerBlue',
+        #  waiting         'SlateGrey',        'DarkSlateBlue',
+        #  wrap            'ForestGreen',      'LightGrey',
+        #  running         'OrangeRed',        'Gold',
+        #  paused          'MediumVioletRed',   'DarkViolet',
+        # Explanations for the key names:
+        #     available:    available task/job reminders
+        #     begin:        begin by warnings
+        #     event:        event reminders
+        #     finished:     finished task/job reminders
+        #     inbox:        inbox reminders
+        #     journal:      journal reminders
+        #     pastdue:      pasdue task warnings
+        #     plain:        headings such as outline branches
+        #     today:        the current and following agenda date headings
+        #     used:         used time rows in engaged and used time views
+        #     waiting:      waiting job reminders (jobs with unfinished prereqs)
+        #     wrap:         before and after rows for events in agenda view with
+        #                   @w entries
+        #     running:      status bar color for 'r', running timer
+        #     paused:       status bar color for 'p', paused timer
+        #
+        # E.g., with style 'dark', the default color for 'available' is
+        # 'LightSkyBlue'. This entry
+        #   colors:
+        #       available: CornFlowerBlue
+        # would change the 'available' color to 'CornflowerBlue' while leaving
+        # the other 'dark' colors unchanged.
+        #
+        # To preview the namedcolors, download "namedcolors.py" from
+        #    "https://github.com/dagraham/etm-dgraham",
+        # open a terminal with your chosen background color and run
+        #    python3 <path to namedcolors.py>
+        # at the command prompt.
+
+        window_colors:
+        # A dictionary with style component keys and corresponding lists of
+        #    [background, foreground, attribute]
+        # components. background and foreground can either be named colors,
+        # hex colors, or ''. Attribute is an optional font attribute such
+        # as 'bold' which must, of course, be supported by the font used in
+        # your terminal. The default settings are determined by the 'dark'
+        # or 'light' style setting as follows:
+        #
+        #    key                       dark default                  light default
+        # -------------------    -----------------------------  -----------------------------
+        # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
+        # button.focused:         [DarkGreen, White]            [DarkGreen, White]
+        # details:                [, Ivory]                     [, Black]
+        # dialog shadow:          [#444444, ]                   [#444444, ]
+        # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
+        # dialog-entry:           [White, Black]                [White, Black]
+        # dialog-output:          [DarkSlateGrey, Lime]         [DimGrey, Lime]
+        # dialog.body label:      [, White]                     [, White]
+        # dialog.body:            [DarkSlateGrey, White]        [DimGrey, White]
+        # entry:                  [grey2, LightGoldenRodYellow] [Cornsilk, LightGoldenRodYellow]
+        # frame.label:            [DarkSlateGrey, White]        [DimGrey, White]
+        # menu:                   [DarkSlateGrey, White]        [DimGrey, White]
+        # menu-bar:               [grey1, White]                [grey1, White]
+        # menu-bar.selected-item: [#ffffff, #000000]            [#ffffff, #000000]
+        # menu.border:            [, #aaaaaa]                   [, #aaaaaa]
+        # not-searching:          [, #222222]                   [, #777777]
+        # query:                  [, Ivory]                     [, Black]
+        # reply:                  [grey2, DeepSkyBlue]          [Cornsilk, DeepSkyBlue]
+        # shadow:                 [#222222, ]                   [#222222, ]
+        # status:                 [grey1, White]                [grey1, White]
+        # status.key:             [, #ffaa00]                   [, #ffaa00]
+        # status.position:        [, #aaaa00]                   [, #aaaa00]
+        # text-area:              [grey2, Ivory]                [Cornsilk, Black]
+        # window.border shadow:   [, #444444]                   [, #444444]
+        # window.border:          [, #888888]                   [, #888888]
+        #
+        # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
+        # within etm itself. They are, respectively, one shade lighter and two
+        # shades darker than DarkSlateGrey.
+        #
+        # Any of the style attributes above can be modified. E.g., with style
+        # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
+        #   window_colors:
+        #       text-area: [Black, White]
+        # would change the 'text-area' setting to 'Black' as the background color
+        # and 'White' as the foreground color while leaving the other style settings
+        # unchanged.
+        #### end cfg.yaml ####
 
 
 See [Saved Queries](#saved-queries) for more information about queries that allow for replaceable parameters.
 
 Note that in the 'dictionary' entries above, the components must be indented (using 2 spaces not tabs). E.g., the illustrative alert entry would be:
 
 	alerts:
```

### Comparing `etm-dgraham-5.0.9/bump.py` & `etm-dgraham-5.1.0/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/docs/index_konnections.md` & `etm-dgraham-5.1.0/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/docs/index_usedtime.md` & `etm-dgraham-5.1.0/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/docs/multiple_timers.md` & `etm-dgraham-5.1.0/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm/__main__.py` & `etm-dgraham-5.1.0/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm/data.py` & `etm-dgraham-5.1.0/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm/ical.py` & `etm-dgraham-5.1.0/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm/make_examples.py` & `etm-dgraham-5.1.0/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm/model.py` & `etm-dgraham-5.1.0/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,21 +89,21 @@
 #     try:
 #         # this works if dt is a datetime
 #         return dt.format("YYYYMMDDHHmm")
 #     except:
 #         # this works if dt is a date by providing 00 for HH and mm
 #         return dt.format("YYYYMMDD0000")
 
-def sortprd(prd, start=True):
+def sortprd(prd):
     # assumes prd is a pendulum.Period
-    if start:
-        return prd.start.format("YYYYMMDDHHmm")
-    else:
-        return prd.end.format("YYYYMMDDHHmm")
+    return prd.start.format("YYYYMMDDHHmm")
 
+# def sortend(prd):
+#     # assumes prd is a (pendulum.Datetime, symbol) tuple
+#     return prd[0].format("YYYYMMDDHHmm")
 
 
 PHONE_REGEX = re.compile(r'[0-9]{10}@.*')
 KONNECT_REGEX = re.compile(r'^.+:\s+(\d+)\s*$')
 
 # The style sheet for terminal output
 style = Style.from_dict({
@@ -602,36 +602,35 @@
     def get_repetitions(self, num=5):
         """
         Called with a row, we should have an doc_id and can use relevant
         as aft_dt.
         Called while editing, we won't have a row or doc_id and can use '@s'
         as aft_dt
         """
-        self.update_item_hsh()
+        # self.update_item_hsh()
         item = self.item_hsh
         showing =  "Repetitions"
         if not ('s' in item and ('r' in item or '+' in item)):
             return showing, "not a repeating item"
         relevant = date_to_datetime(item['s'])
 
-        pairs = [format_datetime(x[0])[1] for x in item_instances(item, relevant, num+1)]
+        pairs = [format_datetime(x[0])[1] for x in item_instances(item, relevant, num+1, False)]
         starting = format_datetime(relevant.date())[1]
         if len(pairs) > num:
-            showing = f"First {num} repetitions"
+            showing = f"Next {num} repetitions"
             pairs = pairs[:num]
         elif pairs:
             showing = "All repetitions"
         else:
             showing = "No repetitions"
         return  showing, f"from {starting}:\n  " + "\n  ".join(pairs)
 
 
     def do_update(self):
         timer_update = TimeIt('***UPDATE***')
-        logger.debug(f"updating {self.doc_id} with {self.item_hsh}")
         self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
         timer_update.stop()
 
 
     def edit_item(self, doc_id=None, entry=""):
         if not (doc_id and entry):
             return None
@@ -858,14 +857,15 @@
                     else:  # finished last instance
                         self.item_hsh['f'] = completion_entry
                         save_item = True
 
                 elif '+' in self.item_hsh:
                     # simple repetition
                     tmp = [self.item_hsh['s']] + self.item_hsh['+']
+                    tmp = [date_to_datetime(x) for x in tmp]
                     tmp.sort()
                     due = tmp.pop(0)
                     if tmp:
                         self.item_hsh['s'] = tmp.pop(0)
                     if tmp:
                         self.item_hsh['+'] = tmp
                         self.item_hsh.setdefault('h', []).append(completion_entry)
@@ -2950,21 +2950,22 @@
         goto = item.get('g')
         if goto:
             return True, goto
         else:
             return False, f"The item\n   {item['itemtype']} {item['summary']}\n does not have an @g goto entry."
 
 
-    def get_repetitions(self, row=None, num=5):
+    def get_repetitions(self, row=None):
         """
         Called with a row, we should have an doc_id and can use relevant
         as aft_dt.
         Called while editing, we won't have a row or doc_id and can use '@s'
         as aft_dt
         """
+        num = self.settings['num_repetitions']
         res = self.get_row_details(row)
         if not res:
             return None, ''
         item_id = res[0]
 
         if not (item_id and item_id in self.id2relevant):
             return ''
@@ -2973,23 +2974,67 @@
         if not ('s' in item and ('r' in item or '+' in item)):
             return showing, "not a repeating item"
         relevant = self.id2relevant.get(item_id)
         showing =  "Repetitions"
         details = f"{item['itemtype']} {item['summary']}"
         if not relevant:
             return "Repetitons", details + "none"
-        pairs = [format_datetime(x[0])[1] for x in item_instances(item, relevant, num+1)]
+        pairs = [format_datetime(x[0])[1] for x in item_instances(item, relevant, num+1, False)]
         starting = format_datetime(relevant.date())[1]
         if len(pairs) > num:
-            showing = f"First {num} repetitions"
+            showing = f"Next {num} repetitions"
             pairs = pairs[:num]
         else:
             showing = f"All repetitions"
         return  showing, f"from {starting} for\n{details}:\n  " + "\n  ".join(pairs)
 
+
+    def get_history(self, row=None):
+        """
+        For repeating tasks, show up to num_repetitions of the due datetimes from the completion history. For
+        those with '@o s', additionally show those that were skipped.
+        """
+        num = self.settings['num_repetitions']
+        res = self.get_row_details(row)
+        if not res:
+            return None, ''
+        item_id = res[0]
+
+        if not (item_id and item_id in self.id2relevant):
+            return ''
+        showing = "History"
+        item = DBITEM.get(doc_id=item_id)
+
+        if not (item['itemtype'] == '-' and ('r' in item or '+' in item)):
+            return showing, "not a repeating task"
+        if 'h' not in item:
+            return showing, "there is no history of completions"
+
+        relevant = self.id2relevant.get(item_id)
+        res = []
+        skip = item.get('o', 'k') == 's'
+        for c in item['h']:
+            if skip and c.start == c.end:
+                res.append((c.end, ' '))
+            else:
+                res.append((c.end, FINISHED_CHAR))
+        res.sort() # pendulum.DateTime obj as first component
+        if len(res) > num:
+            showing = f"Completion History: last {num} of {len(res)}"
+            res = res[-num:]
+        else:
+            showing = f"Completion History"
+        relevant = res[-1][0]
+        details = f"{item['itemtype']} {item['summary']}"
+
+        pairs = [f"{x[1]} {format_datetime(x[0])[1]}" for x in res]
+        starting = format_datetime(relevant.date())[1]
+
+        return  showing, f"through {starting} for\n{details}:\n  " + "\n  ".join(pairs)
+
     def touch(self, row):
         res = self.get_row_details(row)
         if not res:
             return False
         doc_id, instance, job_id = res
         now = pendulum.now('local')
         item_hsh = self.db.get(doc_id=doc_id)
@@ -4751,15 +4796,15 @@
 
 def date_to_datetime(dt, hour=0, minute=0):
     if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
         dt= pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=hour, minute=minute, tz='local')
     return dt
 
 
-def item_instances(item, aft_dt, bef_dt=1):
+def item_instances(item, aft_dt, bef_dt=1, honor_skip=True):
     """
     Dates and datetimes decoded from the data store will all be aware and in the local timezone. aft_dt and bef_dt must therefore also be aware and in the local timezone.
     In dateutil, the starting datetime (dtstart) is not the first recurrence instance, unless it does fit in the specified rules.  Notice that you can easily get the original behavior by using a rruleset and adding the dtstart as an rdate recurrence.
     Each instance is a tuple (beginning datetime, ending datetime) where ending datetime is None unless the item is an event.
 
     Get instances from item falling on or after aft_dt and on or before bef_dt or, if bef_dt is an integer, n, get the first n instances after aft_dt. All datetimes will be returned with zero offsets.
     >>> item_eg = { "s": parse('2018-03-07 8am', tz="US/Eastern"), "e": pendulum.duration(days=1, hours=5), "r": [ { "r": "w", "i": 2, "u": parse('2018-04-01 8am', tz="US/Eastern")}], "z": "US/Eastern", "itemtype": "*" }
@@ -4891,15 +4936,15 @@
             if item.get('o', 'k') == 's':
                 if (instance.year, instance.month, instance.day) >= (today.year, today.month, today.day):
                     if 'e' in item:
                         for pair in beg_ends(instance, item['e'], item.get('z', 'local')):
                             pairs.append(pair)
                     else:
                         pairs.append((instance, None))
-                    if pairs and settings['limit_skip_display']:
+                    if pairs and honor_skip and settings['limit_skip_display']:
                         # only keep the first instance that falls during or after today/now
                         break
             elif 'e' in item:
                 for pair in beg_ends(instance, item['e'], item.get('z', 'local')):
                     pairs.append(pair)
             else:
                 pairs.append((instance, None))
@@ -5266,15 +5311,14 @@
         id2hsh[i]['summary'] = "{} {}: {}".format(summary, "/".join([str(x) for x in awf]), id2hsh[i]['j'])
         id2hsh[i]['req'] = req[i]
         id2hsh[i]['i'] = i
 
     if msg:
         logger.warning(f"{msg}")
         return False, msg, None
-    # logger.debug(f"returning True, {[id2hsh[i] for i in ids]}, {last_completion}")
     return True, [id2hsh[i] for i in ids], last_completion
 
 #######################
 ### end jobs setup ####
 #######################
 
 
@@ -5577,15 +5621,18 @@
     current = []
 
     for item in db:
         instance_interval = []
         possible_beginby = None
         possible_alerts = []
         all_tds = []
+        relevant = None
+        dtstart = None
         doc_id = item.doc_id
+        rset = rruleset()
         if 'itemtype' not in item:
             logger.warning(f"no itemtype: {item}")
             item['itemtype'] = '?'
             # continue
         if 'g' in item:
             if doc_id not in link_list:
                 link_list.append(doc_id)
@@ -5666,36 +5713,29 @@
                     for dt in item['-']:
                         dt = date_to_datetime(dt)
                         # if type(dt) == pendulum.Date:
                         #     dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
                         rset.exdate(dt)
 
                 if '+' in item:
-                    # tmp = [dtstart]
-                    # tmp.extend(item['+'])
-                    # tmp = [date_to_datetime(x) for x in tmp]
-                    # tmp.sort()
-                    # aft = [x for x in tmp if x >= today]
-                    # bef = [x for x in tmp if x < today]
-                    # if aft:
-                    #     relevant = aft[0]
-                    # else:
-                    #     relevant = bef[-1]
                     for dt in item['+']:
                         dt = date_to_datetime(dt)
-                        # if type(dt) == pendulum.Date:
-                        #     dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
                         rset.rdate(dt)
 
                 if item['itemtype'] == '-':
                     switch = item.get('o', 'k')
                     relevant = rset.after(today, inc=True)
                     if switch == 's':
-                        if relevant and item['s'] != pendulum.instance(relevant):
-                            item['s'] = pendulum.instance(relevant)
+                        if relevant and date_to_datetime(item['s']) < today:
+                            cur = date_to_datetime(item['s'])
+                            while cur < today:
+                                item.setdefault('h', []).append(pendulum.period(cur, cur))
+                                cur = rset.after(cur, inc=False)
+
+                            item['s'] = pendulum.instance(cur)
                             update_db(db, item.doc_id, item)
                     else: # k or p
                         relevant = rset.after(today, inc=True)
                         already_done = [x.end for x in item.get('h', [])]
                         # relevant will be the first instance after 12am today
                         # it will be the @s entry for the updated repeating item
                         # these are @s entries for the instances to be preserved
@@ -5721,15 +5761,15 @@
                         relevant = pendulum.instance(relevant)
 
                 # rset
                 if instance_interval:
                     instances = rset.between(instance_interval[0], instance_interval[1], inc=True)
                     if possible_beginby:
                         for instance in instances:
-                            if today + DAY <= instance <= tomorrow + possible_beginby:
+                            if ZERO < instance.date()-today.date() <= possible_beginby:
                                 doc_id = item.doc_id
                                 if 'r' in item:
                                     # use the freq from the first recurrence rule
                                     freq = item['r'][0].get('r', 'y')
                                 else:
                                     freq = 'y'
                                 summary = set_summary(summary, item.get('s', None), pendulum.instance(instance).date(), freq)
@@ -5751,29 +5791,27 @@
                 if aft:
                     relevant = aft[0]
                 else:
                     relevant = bef[-1]
 
                 if possible_beginby:
                     for instance in aft:
-                        if today + DAY <= instance <= tomorrow + possible_beginby:
+                        # if today + DAY <= instance <= tomorrow + possible_beginby:
+                        if ZERO < instance.date()-today.date() <= possible_beginby:
                             beginbys.append([(instance.date() - today.date()).days, summary, item.doc_id, None, instance])
                 if possible_alerts:
                     for instance in aft + bef:
                         for possible_alert in possible_alerts:
                             if today <= instance - possible_alert[0] <= tomorrow:
                                 alerts.append([instance - possible_alert[0], instance, possible_alert[1], item['itemtype'], item['summary'], item.doc_id])
 
             else:
                 # 's' but not 'r' or '+'
                 relevant = dtstart
-                if (
-                    possible_beginby
-                    and today + DAY <= dtstart <= tomorrow + possible_beginby
-                ):
+                if possible_beginby and ZERO < relevant.date()-today.date() <= possible_beginby:
                     beginbys.append([(relevant.date() - today.date()).days, summary,  item.doc_id, None, None])
                 if possible_alerts:
                     for possible_alert in possible_alerts:
                         if today <= dtstart - possible_alert[0] <= tomorrow:
                             alerts.append([dtstart - possible_alert[0], dtstart, possible_alert[1], item['itemtype'], item['summary'], item.doc_id])
         else:
             # no 's', no 'f'
@@ -6783,29 +6821,31 @@
     done2id_hsh = {}     # yw -> row2id
     engaged_hsh = {}
     engaged2id_hsh = {}     # yw -> row2id
     week2day2engaged = {}   # year, week -> dayofweek -> period total for day
     week2day2heading = {}
     weeks = set([])
     rows = []
-    done = []
-    completed = []
+    # done = []
+    # completed = []
     engaged = []
     # busy = []
 
     #XXX year, week -> dayofweek -> list of [time interval, summary, period]
     busy_details = {}
     week2day2busy = {}
     week2day2allday = {}
 
     #XXX main loop begins
     todayYMD = now.format("YYYYMMDD")
     tomorrowYMD = (now + 1*DAY).format("YYYYMMDD")
 
     for item in db:
+        completed = []
+        done = []
         if item.get('itemtype', None) == None:
             logger.error(f"itemtype missing from {item}")
             continue
         if item['itemtype'] in "!?":
             continue
 
         doc_id = item.doc_id
@@ -7071,15 +7111,16 @@
                         wrapper = f"\n{22*' '}+ {', '.join(wraps)}"
                     else:
                         wrapper = ""
 
 
                     if b and b > ZERO:
                         itemtype = wrapbefore #  "↱"
-                        sort_b = (dt-ONEMIN).format("YYYYMMDDHHmm")
+                        # sort_b = (dt-ONEMIN).format("YYYYMMDDHHmm")
+                        sort_b = (dt).format("YYYYMMDDHHmm")
                         rhb = fmt_time(dtb).center(rhc_width, ' ')
                         before = {
                                     'id': doc_id,
                                     'job': None,
                                     'instance': instance,
                                     'sort': (sort_b, 0),
                                     'week': (
```

### Comparing `etm-dgraham-5.0.9/etm/options.py` & `etm-dgraham-5.1.0/etm/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
     secret = randomString(10)
     omit_extent = ""
     keep_current = [0, 46]
     keep_next = "false"
     archive_after = 0
     refresh_interval = 60
     num_finished = 0
+    num_repetitions = 10
     limit_skip_display = "true"
     connecting_dots = "false"
     usedtime_minutes = 1
     usedtime_hours = 6
     alerts = ""
     expansions = ""
     sms = {"body": "{location} {when}", "from": "", "server": "", "pw": ""}
@@ -202,14 +203,15 @@
         "secret" : secret,
         "omit_extent" : omit_extent,
         "keep_current" : keep_current,
         "keep_next" : keep_next,
         "archive_after" : archive_after,
         "refresh_interval" : refresh_interval,
         "num_finished" : num_finished,
+        "num_repetitions" : num_repetitions,
         "limit_skip_display" : limit_skip_display,
         "connecting_dots" : connecting_dots,
         "usedtime_minutes" : usedtime_minutes,
         "usedtime_hours" : usedtime_hours,
         "alerts" : dict2yaml(alerts),
         "expansions" : dict2yaml(expansions),
         "sms": dict2yaml(sms),
@@ -322,19 +324,28 @@
 refresh_interval: {refresh_interval}
 # 6, 12, 30 or 60. The event loop responsible for refreshing
 # etm caches, updating alerts, timers and so forth, repeats once
 # every refresh_interval seconds.
 
 num_finished: {num_finished}
 # non-negative integer
-# If positive, when saving retain only the most recent
-# "num_finished" completions of an infinitely repeating task,
-# i.e., repeating without an "&c" count or an "&u" until
-# attribute. If zero or not infinitely repeating, save all
-# completions.
+# If positive, when saving retain only the most recent "num_finished"
+# completions of an infinitely repeating task, i.e., repeating without
+# an "&c" count or an "&u" until attribute. If zero or not infinitely
+# repeating, save all completions.
+
+num_repetitions: {num_repetitions}
+# positive integer
+# Show at most this number of repetitions when showing repetitions
+# with (^r) or when showing completion history (^h). In the former
+# case these are instances for the selected item (repeating of any
+# item type) starting from date of the selected item and in the latter
+# case these are the completion instances (task item type). Note that
+# the num_finished setting can affect the number available for display
+# for the completion history.
 
 limit_skip_display: {limit_skip_display}
 # true or false. If true, only the first instance of a task with "@o
 # s" (overdue skip) will be displayed. For a task with an "@s" entry
 # that is a date this will be the first instance that falls on or
 # after the current date. Otherwise, when the "@s" entry is a
 # datetime, this will be the first instance that falls on or after the
```

### Comparing `etm-dgraham-5.0.9/etm/report.py` & `etm-dgraham-5.1.0/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm/view.py` & `etm-dgraham-5.1.0/etm/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -2136,14 +2136,20 @@
 def do_finish(*event):
 
     doc_id, instance, job = dataview.get_row_details(text_area.document.cursor_position_row)
     if not doc_id:
         return
 
     hsh = DBITEM.get(doc_id=doc_id)
+    msg = ""
+    if hsh['itemtype'] != '-' or 'f' in hsh:
+        show_message('Finish', "Only an unfinished task can be finished.")
+        return
+
+    logger.debug(f"doc_id: {doc_id}, instance: {instance}, job: {job}, hsh: {hsh}")
     has_timer = doc_id in dataview.timers
     timer_warning = " and\nits associated timer" if has_timer else ""
     repeating = 'r' in hsh or '+' in hsh
 
     between = []
     due = ""
 
@@ -2205,39 +2211,55 @@
 the completion datetime to use?
 number : datetime\
         """
         entry = "1 : now"
         due = ""
 
     elif repeating:
-        # must be selected from today's pastdue
+        # must be selected from today's pastdue or beginby
         already_done = [x.end for x in hsh.get('h', [])]
-        need = 2
         between = [x[0] for x in model.item_instances(hsh, model.date_to_datetime(hsh['s']), pendulum.now().replace(hour=0, minute=0, second=0, microsecond=0)) if x[0] not in already_done]
-        values_list = []
-        # values.append( (0, format_datetime(between[0][0])[1]) )
-        count = -1
-        for x in between:
-            count += 1
-            values_list.append(f"   {count}: {format_datetime(x)[1]}")
+        if between:
+            # show_message('Finish', "There is nothing to complete.")
+            need = 2
+            values_list = []
+            # values.append( (0, format_datetime(between[0][0])[1]) )
+            count = -1
+            for x in between:
+                count += 1
+                values_list.append(f"   {count}: {format_datetime(x)[1]}")
 
-        values_str = "\n".join(values_list)
+            values_str = "\n".join(values_list)
 
-        text= f"""\
+            text= f"""\
 Selected: {hsh['itemtype']} {hsh['summary']}
 
 {values_str}
 
 The number of the instance to finish and
 the completion datetime to use?
 number : datetime\
-        """
+            """
 
-        entry = "0 : now"
-        due = ""
+            entry = "0 : now"
+            due = ""
+        else:
+            # beginby
+
+            need = 1
+            between = [hsh.get('s', None)]
+            entry =  "now"
+            # due = hsh.get('s', "")
+            start = f"\nDue: {format_datetime(hsh['s'])[1]}" if 's' in hsh else ""
+
+            text= f"""\
+Selected: {hsh['itemtype']} {hsh['summary']}{start}
+
+Enter <completion datetime>
+        """
 
     else:
         need = 1
         between = [hsh.get('s', None)]
         entry =  "now"
         # due = hsh.get('s', "")
         start = f"\nDue: {format_datetime(hsh['s'])[1]}" if 's' in hsh else ""
@@ -2364,15 +2386,24 @@
             show_message("goto", res, 8)
     else:
         show_message('goto', goto, 8)
 
 @bindings.add('c-r', filter=is_viewing_or_details & is_item_view)
 def not_editing_reps(*event):
     row = text_area.document.cursor_position_row
-    res = dataview.get_repetitions(row, 5)
+    res = dataview.get_repetitions(row)
+    if not res:
+        return
+    showing, reps = res
+    show_message(showing, reps, 24)
+
+@bindings.add('c-h', filter=is_viewing_or_details & is_item_view)
+def not_editing_history(*event):
+    row = text_area.document.cursor_position_row
+    res = dataview.get_history(row)
     if not res:
         return
     showing, reps = res
     show_message(showing, reps, 24)
 
 @bindings.add('c-r', filter=is_editing)
 def is_editing_reps(*event):
@@ -3020,14 +3051,15 @@
         MenuItem('D) delete', handler=do_maybe_delete),
         MenuItem('F) finish', handler=do_finish),
         MenuItem('P) toggle pin', handler=toggle_pinned),
         MenuItem('R) reschedule',  handler=do_reschedule),
         MenuItem('S) schedule new', handler=do_schedule_new),
         MenuItem('g) open goto link', handler=do_goto),
         MenuItem('k) show konnections', handler=show_konnections),
+        MenuItem('^h) show completion history', handler=not_editing_history),
         MenuItem('^r) show repetitions', handler=not_editing_reps),
         MenuItem('^u) update last modified', handler=do_touch),
         MenuItem('^x) toggle archived status', handler=toggle_archived_status),
         MenuItem('-', disabled=True),
         MenuItem('T) activate timer if none active ', handler=next_timer_state),
         MenuItem("TR) add usedtime / record usedtime and end timer", handler=record_time),
         MenuItem('TD) delete timer', handler=maybe_delete_timer),
```

### Comparing `etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.9
+Version: 5.1.0
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -1219,14 +1219,15 @@
         D) delete
         F) finish
         P) toggle pin
         R) reschedule
         S) schedule new
         g) open goto link
         k) show konnections
+        ^h) show completion history
         ^r) show repetitions
 		^u) update last modified
         ^x) toggle archived status
         ---
         T) change timer to next state
         TR) record usedtime and end timer or add usedtime
         TD) delete timer
@@ -1972,366 +1973,394 @@
 
 ### configuration {#configuration}
 
 Configuration settings for *etm* are specified in the file `cfg.yaml` located in your etm *home directory*. See [installation](#installation) for the location of this directory. When *etm* is running, you can press `F8` to open this configuration file using your system default editor for *yaml* (text) files. Note that any changes you make will not become effective until you stop and restart *etm*.
 
 Here are the options with their default values from that file. The lines beginning with `#` are comments that describe the settings.
 
-    #### begin cfg.yaml ####
-    etmversion: 4.11.18
-    # The current version of etm and this file. DO NOT EDIT. This is
-    # automatically updated when a new version of etm is installed.
-
-    ampm: true
-    # true or false. Use AM/PM format for datetimes if true else
-    # use 24 hour format. See also the show_minutes setting.
-
-    show_minutes: false
-    # true or false. If true show ":00" in agenda and forthcoming views
-    # when displaying times with zero minutes else suppress zero minutes
-    # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
-    # When ampm if false and show_minutes is true, hours will be displayed
-    # with leading zeros applicable.
-
-    dayfirst:  false
-    yearfirst: true
-    # each true or false. Whenever an ambiguous date is parsed, dayfirst
-    # and yearfirst parameters control how the information is processed
-    # using this precedence:
-    # yearfirst: true
-    # 	dayfirst: true  => YDM
-    #   dayfirst: false => YMD
-    # yearfirst: false
-    # 	dayfirst: true  => DMY
-    #   dayfirst: false => MDY
-    # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
-    # When possible, dates will also be displayed respecting these settings.
-    # I.e., the year will generally be displayed first when yearfirst is
-    # true and last otherwise. Similarly, the day will generally be displayed
-    # before the month when dayfirst is true and after the month otherwise.
-
-    beginbusy: 7
-    # non-negative integer. The number of hours after midnight to begin the
-    # busy view display of busy times for each day. The display continues
-    # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
-    # display would show busy times from 7am (7h) until 9pm (21h).
-
-    updates_interval: 0
-    # non-negative integer. If positive,  automatically check for updates
-    # every 'updates_interval' minutes. If zero, do not automatically
-    # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
-    # displayed at the right end of status bar when an update is available
-    # or a question mark when the check cannot be completed as, for
-    # example, when there is no internet connection.
-
-    locale: en_US
-    # locale abbreviation. E.g., "en_AU" for English (Australia), "en_US"
-    # for English (United States), "fr_FR" for French (France) and so
-    # forth. Google "python locale abbreviatons" for a complete list."
-
-    vi_mode: false
-    # true or false. Use vi keybindings for editing if true else use emacs
-    # style keybindings.
-
-    secret: HIr13FiYj3
-    # string to use as the secret_key for @m masked entries. E.g.
-    # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
-    # randomly generated when this file is created or when the secret
-    # value is removed and etm is restarted. WARNING: if this key is
-    # changed, any @m entries that were made before the change will be
-    # unreadable after the change.
-
-    omit_extent:
-    # A list of calendar names. Events with @c entries belonging to this
-    # list will only have their starting times displayed in agenda view
-    # and will neither appear nor cause conflicts in busy view.
-
-    keep_current: [0, 46]
-    # A list of two, non-negative integers for "weeks" and "width". If
-    # weeks is positive, the agenda for that integer number of weeks
-    # starting with the current week will be written to "current.txt" in
-    # your etm home directory and updated when necessary. The format will
-    # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
-    # in portrait mode. You could, for example, create a link to
-    # "current.txt" in a pCloud or GoogleDrive folder and always have access
-    # to your current agenda on your mobile device.
-
-    keep_next: false
-    # true or false. If true, the 'do next' view will be written to
-    # "next.txt" in your etm home directory. As with "current.txt", a link
-    # to this file could be created in a pCloud or DropBox folder for
-    # access from your mobile device.
-
-    archive_after: 0
-    # non-negative integer. If zero, do not archive items. If positive,
-    # finished tasks and events with last datetimes falling more than this
-    # number of years before the current date will automatically be
-    # archived on a daily basis.  Archived items are moved from the
-    # "items" table in the database to the "archive" table and will no
-    # longer appear in normal views. Note that unfinished tasks and
-    # records are not archived.
-
-    num_finished: 0
-    # non-negative integer
-    # If positive, when saving retain only the most recent
-    # "num_finished" completions of an infinitely repeating task,
-    # i.e., repeating without an "&c" count or an "&u" until
-    # attribute. If zero or not infinitely repeating, save all
-    # completions.
-
-    limit_skip_display: true
-    # true or false. If true, only the first instance of a task with "@o
-    # s" (overdue skip) will be displayed. For a task with an "@s" entry
-    # that is a date this will be the first instance that falls on or
-    # after the current date. Otherwise, when the "@s" entry is a
-    # datetime, this will be the first instance that falls on or after the
-    # current time.
-
-    connecting_dots: false
-    # true or false. If true, display dots connecting the item summary and
-    # the right-hand details columns in tree views.
-
-    usedtime_minutes: 1
-    # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
-    # and times are reported in hours, minutes and seconds. With 1, after
-    # rounding up to the nearest minute, times are reported as hours and minutes.
-    # Otherwise, rounding is up to the nearest integer multiple of
-    # usedtime_minutes and times are reported as floating point hours. E.g.,
-    # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
-    # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
-    # minutes and reported as 0.3 hours. Note that when rounding is specified,
-    # each "@u" timeperiod is rounded before aggregation.
-
-    usedtime_hours: 6
-    # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
-    # view to control the display of the daily used time bars. The goal is to
-    # to maximize the granularity of the bar when displaying this number of hours
-    # in the space allowed by the terminal width.
-
-    journal_name: daily
-    # Journal items with this index entry and with an @s entry will have the
-    # year and month appended to the index. E.g., with the setting
-    #   journal_name: daily
-    # this journal entry
-    #   % visited Yellowstone @s 22/6/24 @i daily
-    # would be displayed in journal view as if the index entry were
-    #   @i daily/2022/ 6
-    # thus organizing such entries by the year and month of their scheduled dates.
-    # Within each month, entries will be also ordered by the month day.
-
-    alerts:
-    # A dictionary with single-character, "alert" keys and corresponding
-    # "system command" values. Note that characters "t" (text message) and
-    # "e" (email) are already used.  The "system command" string should be
-    # a comand with any applicable arguments that could be run in a
-    # terminal. Properties of the item triggering the alert can be
-    # included in the command arguments using the syntax {prop}, e.g.,
-    # {summary} in the command string would be replaced by the summary of
-    # the item. Similarly {start} by the starting datetime, {time} by the
-    # starting time (omits the date for the current date), {when} by the time
-    # remaining until the starting datetime, {now} by the current time,
-    # {location} by the @l entry and {description} by the @d entry. E.g., If
-    # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
-    # before the starting time the string "{summary} {when}" would expand to
-    # "sales meeting in 30 minutes". E.g. on my macbook
-    #
-    #    alerts:
-    #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
-    #        ...
-    #
-    # would make the alert 'v' use the builtin text to speech sytem
-    # to speak the item's summary followed by a slight pause
-    # (the comma) and then the time remaining until the starting
-    # time, e.g., "sales meeting, in 20 minutes" would be triggered
-    # by including "@a 20m: v" in the reminder.
-
-    expansions:
-    # A dictionary with 'expansion name' keys and corresponding
-    # 'replacement string' values. E.g. with
-    #
-    #    expansions:
-    #        tennis: "@e 1h30m @a 30m: d @i personal:exercise"
-    #        ...
-    #
-    # then when "@x tennis" is entered the popup completions for
-    # "@x tennis" would offer replacement by the corresponding
-    # "@e 1h30m @a 30m: d @i personal:exercise".
-
-    sms:
-    body: '{location} {when}'
-    from:
-    server:
-    pw:
-    # Settings to send "t" (sms text message) alerts to the
-    # list of phone numbers from the item's @n attendee
-    # entries using the item's summary and the body as specified
-    # in the template below as the message. E.g., suppose you
-    # have a gmail account with email address "who457@gmail.com"
-    # and want to text alerts to Verizon moble phone (123)
-    # 456-7890. Then your sms entries should be
-    #     from:   who457@gmail.com
-    #     pw:     your gmail password
-    #     server: smtp.gmail.com:587
-    # and your item should include the following attendee entry
-    #     @n 1234567890@vzwpix.com
-    # In the illustrative phone number, @vzwpix.com is the mms
-    # gateway for Verizon. Other common mms gateways are
-    #     AT&T:     @mms.att.net
-    #     Sprint:   @pm.sprint.com
-    #     T-Mobile: @tmomail.net
-    # Note. Google "mms gateway listing" for other alternatives.
-
-    smtp:
-    body: '{location} {when}\n{description}'
-    from:
-    server:
-    id:
-    pw:
-    # Settings to send "e" (email message) alerts to the list of email
-    # addresses from the item's @n attendee entries using the item's
-    # summary as the subject and body as the message. E.g., if you have a
-    # gmail account with email address "whatever457@gmail.com", then your
-    # entries should be
-    #     from: whatever457@gmail.com
-    #     id: whatever457
-    #     pw: your gmail password
-    #     server: smtp.gmail.com
-
-    locations:
-    # A dictionary with location group names as keys and corresponding
-    # lists of locations as values. When given, do next view will group
-    # items first by the location group name and then by the location
-    # within that group. Note that locations can appear under more than
-    # one group name. E.g.,
-    # locations:
-    #    home: [home, garage, yard, phone, computer]
-    #    work: [work, phone, computer, copier, fax]
-    # Items with a location entry that does not belong to one of these
-    # location groups will be listed under 'OTHER' and items without a
-    # location entry under 'OTHER' and then tilde.
-
-    queries:
-    # A dictionary with short query "keys" and corresponding "query"
-    # values. Each "query" must be one that could be entered as the
-    # command in query view. Keys can be any short string other than
-    # 'a', 'u', 'c' or 'l' which are already in use.
-    # queries:
-    #    td: m l -q equals itemtype - and ~exists f
-    #    mi: exists u and ~exists i
-    #    arch: a exists itemtype
-    #    find: includes summary d {}
-    # The latter would allow you to enter, e.g., `find waldo` and have
-    # it expand to `includes summary d waldo` and thus locate all
-    # reminders with `waldo` either in the summary or d (the description).
-
-    style: dark
-    # dark or light. Set the defaults for dark or light terminal
-    # backgounds. Some output may not be visible unless this is set
-    # correctly for your display.
-
-    type_colors:
-    # A dictionary with type keys and corresponding named-color or hex
-    # values. The default colors are determined by the 'dark' or 'light'
-    # style setting as follows:
-    #
-    #     key           dark default        light default
-    #  -----------    -----------------   -----------------
-    #  available       'LightSkyBlue',     'DarkBlue',
-    #  begin           'Gold',             'DarkViolet',
-    #  event           'LimeGreen',        'DarkGreen',
-    #  finished        'DarkGrey',         'LightSlateGrey',
-    #  inbox           'OrangeRed',        'MediumVioletRed',
-    #  journal         'GoldenRod',        'Brown',
-    #  pastdue         'LightSalmon',      'Red',
-    #  plain           'Ivory',            'Black',
-    #  today           'Ivory bold',       'Black bold',
-    #  used            'Khaki',            'DodgerBlue',
-    #  waiting         'SlateGrey',        'DarkSlateBlue',
-    #  wrap            'ForestGreen',      'LightGrey',
-    #  running         'OrangeRed',        'Gold',
-    #  paused          'MediumVioletRed',   'DarkViolet',
-    # Explanations for the key names:
-    #     available:    available task/job reminders
-    #     begin:        begin by warnings
-    #     event:        event reminders
-    #     finished:     finished task/job reminders
-    #     inbox:        inbox reminders
-    #     journal:      journal reminders
-    #     pastdue:      pasdue task warnings
-    #     plain:        headings such as outline branches
-    #     today:        the current and following agenda date headings
-    #     used:         used time rows in engaged and used time views
-    #     waiting:      waiting job reminders (jobs with unfinished prereqs)
-    #     wrap:         before and after rows for events in agenda view with
-    #                   @w entries
-    #     running:      status bar color for 'r', running timer
-    #     paused:       status bar color for 'p', paused timer
-    #
-    # E.g., with style 'dark', the default color for 'available' is
-    # 'LightSkyBlue'. This entry
-    #   colors:
-    #       available: CornFlowerBlue
-    # would change the 'available' color to 'CornflowerBlue' while leaving
-    # the other 'dark' colors unchanged.
-    #
-    # To preview the namedcolors, download "namedcolors.py" from
-    #    "https://github.com/dagraham/etm-dgraham",
-    # open a terminal with your chosen background color and run
-    #    python3 <path to namedcolors.py>
-    # at the command prompt.
-
-    window_colors:
-    # A dictionary with style component keys and corresponding lists of
-    #    [background, foreground, attribute]
-    # components. background and foreground can either be named colors,
-    # hex colors, or ''. Attribute is an optional font attribute such
-    # as 'bold' which must, of course, be supported by the font used in
-    # your terminal. The default settings are determined by the 'dark'
-    # or 'light' style setting as follows:
-    #
-    #    key                       dark default                  light default
-    # -------------------    -----------------------------  -----------------------------
-    # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
-    # button.focused:         [DarkGreen, White]            [DarkGreen, White]
-    # details:                [, Ivory]                     [, Black]
-    # dialog shadow:          [#444444, ]                   [#444444, ]
-    # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
-    # dialog-entry:           [White, Black]                [White, Black]
-    # dialog-output:          [DarkSlateGrey, Lime]         [DimGrey, Lime]
-    # dialog.body label:      [, White]                     [, White]
-    # dialog.body:            [DarkSlateGrey, White]        [DimGrey, White]
-    # entry:                  [grey2, LightGoldenRodYellow] [Cornsilk, LightGoldenRodYellow]
-    # frame.label:            [DarkSlateGrey, White]        [DimGrey, White]
-    # menu:                   [DarkSlateGrey, White]        [DimGrey, White]
-    # menu-bar:               [grey1, White]                [grey1, White]
-    # menu-bar.selected-item: [#ffffff, #000000]            [#ffffff, #000000]
-    # menu.border:            [, #aaaaaa]                   [, #aaaaaa]
-    # not-searching:          [, #222222]                   [, #777777]
-    # query:                  [, Ivory]                     [, Black]
-    # reply:                  [grey2, DeepSkyBlue]          [Cornsilk, DeepSkyBlue]
-    # shadow:                 [#222222, ]                   [#222222, ]
-    # status:                 [grey1, White]                [grey1, White]
-    # status.key:             [, #ffaa00]                   [, #ffaa00]
-    # status.position:        [, #aaaa00]                   [, #aaaa00]
-    # text-area:              [grey2, Ivory]                [Cornsilk, Black]
-    # window.border shadow:   [, #444444]                   [, #444444]
-    # window.border:          [, #888888]                   [, #888888]
-    #
-    # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
-    # within etm itself. They are, respectively, one shade lighter and two
-    # shades darker than DarkSlateGrey.
-    #
-    # Any of the style attributes above can be modified. E.g., with style
-    # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
-    #   window_colors:
-    #       text-area: [Black, White]
-    # would change the 'text-area' setting to 'Black' as the background color
-    # and 'White' as the foreground color while leaving the other style settings
-    # unchanged.
-    #### end cfg.yaml ####
+        #### begin cfg.yaml ####
+        etmversion: 5.0.12
+        # The current version of etm and this file. DO NOT EDIT. This is
+        # automatically updated when a new version of etm is installed.
+
+        ampm: true
+        # true or false. Use AM/PM format for datetimes if true else
+        # use 24 hour format. See also the show_minutes setting.
+
+        show_minutes: false
+        # true or false. If true show ":00" in agenda and forthcoming views
+        # when displaying times with zero minutes else suppress zero minutes
+        # from being displayed. E.g., "9:00-10:30" if true else "9-10:30".
+        # When ampm if false and show_minutes is true, hours will be displayed
+        # with leading zeros applicable.
+
+        dayfirst:  false
+        yearfirst: true
+        # each true or false. Whenever an ambiguous date is parsed, dayfirst
+        # and yearfirst parameters control how the information is processed
+        # using this precedence:
+        # yearfirst: true
+        # 	dayfirst: true  => YDM
+        #   dayfirst: false => YMD
+        # yearfirst: false
+        # 	dayfirst: true  => DMY
+        #   dayfirst: false => MDY
+        # E.g., with both true, 3/4/5 would be interpreted as May 4, 2003.
+        # When possible, dates will also be displayed respecting these settings.
+        # I.e., the year will generally be displayed first when yearfirst is
+        # true and last otherwise. Similarly, the day will generally be displayed
+        # before the month when dayfirst is true and after the month otherwise.
+
+        beginbusy: 7
+        # non-negative integer. The number of hours after midnight to begin the
+        # busy view display of busy times for each day. The display continues
+        # for 14 hours after the begin_busy hour. E.g. with 'begin_busy: 7' the
+        # display would show busy times from 7am (7h) until 9pm (21h).
+
+        updates_interval: 0
+        # non-negative integer. If positive,  automatically check for updates
+        # every 'updates_interval' minutes. If zero, do not automatically
+        # check for updates. When enabled, a blackboard u symbol, 𝕦, will be
+        # displayed at the right end of status bar when an update is available
+        # or a question mark when the check cannot be completed as, for
+        # example, when there is no internet connection.
+
+        locale: en_US
+        # locale abbreviation. E.g., "en_AU" for English (Australia), "en_US"
+        # for English (United States), "fr_FR" for French (France) and so
+        # forth. Google "python locale abbreviatons" for a complete list."
+
+        vi_mode: true
+        # true or false. Use vi keybindings for editing if true else use emacs
+        # style keybindings.
+
+        secret: HIr13FiYj3
+        # string to use as the secret_key for @m masked entries. E.g.
+        # 'X6i2SGWu6m'. In etm versions after 4.0.21, the default string is
+        # randomly generated when this file is created or when the secret
+        # value is removed and etm is restarted. WARNING: if this key is
+        # changed, any @m entries that were made before the change will be
+        # unreadable after the change.
+
+        omit_extent:
+        # A list of calendar names. Events with @c entries belonging to this
+        # list will only have their starting times displayed in agenda view
+        # and will neither appear nor cause conflicts in busy view.
+
+        keep_current: [3, 46]
+        # A list of two, non-negative integers for "weeks" and "width". If
+        # weeks is positive, the agenda for that integer number of weeks
+        # starting with the current week will be written to "current.txt" in
+        # your etm home directory and updated when necessary. The format will
+        # be scaled to fit "width". A width of 46, e.g, fits an iPhone display
+        # in portrait mode. You could, for example, create a link to
+        # "current.txt" in a pCloud or GoogleDrive folder and always have access
+        # to your current agenda on your mobile device.
+
+        keep_next: true
+        # true or false. If true, the 'do next' view will be written to
+        # "next.txt" in your etm home directory. As with "current.txt", a link
+        # to this file could be created in a pCloud or DropBox folder for
+        # access from your mobile device.
+
+        archive_after: 0
+        # non-negative integer. If zero, do not archive items. If positive,
+        # finished tasks and events with last datetimes falling more than this
+        # number of years before the current date will automatically be
+        # archived on a daily basis.  Archived items are moved from the
+        # "items" table in the database to the "archive" table and will no
+        # longer appear in normal views. Note that unfinished tasks and
+        # journal entries are not archived.
+
+        refresh_interval: 6
+        # 6, 12, 30 or 60. The event loop responsible for refreshing
+        # etm caches, updating alerts, timers and so forth, repeats once
+        # every refresh_interval seconds.
+
+        num_finished: 0
+        # non-negative integer
+        # If positive, when saving retain only the most recent "num_finished"
+        # completions of an infinitely repeating task, i.e., repeating without
+        # an "&c" count or an "&u" until attribute. If zero or not infinitely
+        # repeating, save all completions.
+
+        num_repetitions: 10
+        # positive integer
+        # Show at most this number of repetitions when showing repetitions
+        # with (^r) or when showing completion history (^h). In the former
+        # case these are instances for the selected item (repeating of any
+        # item type) starting from date of the selected item and in the latter
+        # case these are the completion instances (task item type). Note that
+        # the num_finished setting can affect the number available for display
+        # for the completion history.
+
+        limit_skip_display: false
+        # true or false. If true, only the first instance of a task with "@o
+        # s" (overdue skip) will be displayed. For a task with an "@s" entry
+        # that is a date this will be the first instance that falls on or
+        # after the current date. Otherwise, when the "@s" entry is a
+        # datetime, this will be the first instance that falls on or after the
+        # current time.
+
+        connecting_dots: true
+        # true or false. If true, display dots connecting the item summary and
+        # the right-hand details columns in tree views.
+
+        usedtime_minutes: 6
+        # 0, 1, 6, 12, 30 or 60. Round up used times. With 0, no rounding is done
+        # and times are reported in hours, minutes and seconds. With 1, after
+        # rounding up to the nearest minute, times are reported as hours and minutes.
+        # Otherwise, rounding is up to the nearest integer multiple of
+        # usedtime_minutes and times are reported as floating point hours. E.g.,
+        # with usedtime_minutes = 6, 1 minute would be rounded up to 6 minutes and
+        # reported as 0.1 hours. Similarly 13 minutes would be rounded up to 18
+        # minutes and reported as 0.3 hours. The numbers 6, 12, 30 and 60 are
+        # characterized by the fact that each is an integer multiple of 6 and 60 is
+        # evenly divisible by each. This allows reported times to be expressed as
+        # hours and tenths of an hour for each. Note that when rounding is specified,
+        # each "@u" timeperiod is rounded before aggregation. Whatever the setting,
+        # a used time record created using the timer is accurate to the nearest
+        # second.
+
+        usedtime_hours: 6
+        # 0, 1, 2, ..., 24. The daily goal for used time. This is used in engaged
+        # view to control the display of the daily used time bars. The goal is to
+        # to maximize the granularity of the bar when displaying this number of hours
+        # in the space allowed by the terminal width.
+
+        journal_name: daily
+        # Journal items with this index entry and with an @s entry will have the
+        # year and month appended to the index. E.g., with the setting
+        #   journal_name: daily
+        # this journal entry
+        #   % visited Yellowstone @s 22/6/24 @i daily
+        # would be displayed in journal view as if the index entry were
+        #   @i daily/2022/ 6
+        # thus organizing such entries by the year and month of their scheduled dates.
+        # Within each month, entries will be also ordered by the month day.
+
+        alerts:
+        # A dictionary with single-character, "alert" keys and corresponding
+        # "system command" values. Note that characters "t" (text message) and
+        # "e" (email) are already used.  The "system command" string should be
+        # a comand with any applicable arguments that could be run in a
+        # terminal. Properties of the item triggering the alert can be
+        # included in the command arguments using the syntax {prop}, e.g.,
+        # {summary} in the command string would be replaced by the summary of
+        # the item. Similarly {start} by the starting datetime, {time} by the
+        # starting time (omits the date for the current date), {when} by the time
+        # remaining until the starting datetime, {now} by the current time,
+        # {location} by the @l entry and {description} by the @d entry. E.g., If
+        # the event "* sales meeting @s 2019-02-12 3p" triggered an alert 30 minutes
+        # before the starting time the string "{summary} {when}" would expand to
+        # "sales meeting in 30 minutes". E.g. on my macbook
+        #
+        #    alerts:
+        #        v:   /usr/bin/say -v "Alex" "{summary}, {when}"
+        #        ...
+        #
+        # would make the alert 'v' use the builtin text to speech sytem
+        # to speak the item's summary followed by a slight pause
+        # (the comma) and then the time remaining until the starting
+        # time, e.g., "sales meeting, in 20 minutes" would be triggered
+        # by including "@a 20m: v" in the reminder.
+
+        expansions:
+        # A dictionary with 'expansion name' keys and corresponding
+        # 'replacement string' values. E.g. with
+        #
+        #    expansions:
+        #        tennis: "@e 1h30m @a 30m: d @i personal:exercise"
+        #        ...
+        #
+        # then when "@x tennis" is entered the popup completions for
+        # "@x tennis" would offer replacement by the corresponding
+        # "@e 1h30m @a 30m: d @i personal:exercise".
+
+        sms:
+        body: '{location} {when}'
+        from: 'None'
+        server: 'None'
+        pw: 'None'
+        # Settings to send "t" (sms text message) alerts to the
+        # list of phone numbers from the item's @n attendee
+        # entries using the item's summary and the body as specified
+        # in the template below as the message. E.g., suppose you
+        # have a gmail account with email address "who457@gmail.com"
+        # and want to text alerts to Verizon moble phone (123)
+        # 456-7890. Then your sms entries should be
+        #     from:   who457@gmail.com
+        #     pw:     your gmail password
+        #     server: smtp.gmail.com:587
+        # and your item should include the following attendee entry
+        #     @n 1234567890@vzwpix.com
+        # In the illustrative phone number, @vzwpix.com is the mms
+        # gateway for Verizon. Other common mms gateways are
+        #     AT&T:     @mms.att.net
+        #     Sprint:   @pm.sprint.com
+        #     T-Mobile: @tmomail.net
+        # Note. Google "mms gateway listing" for other alternatives.
+
+        smtp:
+        body: '{location} {when}\n{description}'
+        from: 'None'
+        server: 'None'
+        id: 'None'
+        pw: 'None'
+        # Settings to send "e" (email message) alerts to the list of email
+        # addresses from the item's @n attendee entries using the item's
+        # summary as the subject and body as the message. E.g., if you have a
+        # gmail account with email address "whatever457@gmail.com", then your
+        # entries should be
+        #     from: whatever457@gmail.com
+        #     id: whatever457
+        #     pw: your gmail password
+        #     server: smtp.gmail.com
+
+        locations:
+        # A dictionary with location group names as keys and corresponding
+        # lists of locations as values. When given, do next view will group
+        # items first by the location group name and then by the location
+        # within that group. Note that locations can appear under more than
+        # one group name. E.g.,
+        # locations:
+        #    home: [home, garage, yard, phone, computer]
+        #    work: [work, phone, computer, copier, fax]
+        # Items with a location entry that does not belong to one of these
+        # location groups will be listed under 'OTHER' and items without a
+        # location entry under 'OTHER' and then tilde.
+
+        queries:
+        td: 'm l -q equals itemtype - and ~exists f'
+        ui: 'u i[:1]; MMM YYYY; i[1:2] -a d'
+        si: 's i[:1]; MMM YYYY; i[1:2] -a u, d'
+        mi: 'exists u and ~exists i'
+        arch: 'a exists itemtype'
+        uw: 'u WWW; ddd D -b weekbeg - 1w -e weekend'
+        find: 'includes summary d {}'
+        f: 'includes summary d {}'
+        index: 's MMM YYYY; ddd D -q in i {}'
+        # A dictionary with short query "keys" and corresponding "query"
+        # values. Each "query" must be one that could be entered as the
+        # command in query view. Keys can be any short string other than
+        # 'a', 'u', 'c' or 'l' which are already in use.
+        # queries:
+        #    td: m l -q equals itemtype - and ~exists f
+        #    mi: exists u and ~exists i
+        #    arch: a exists itemtype
+        #    find: includes summary d {}
+        # The latter would allow you to enter, e.g., `find waldo` and have
+        # it expand to `includes summary d waldo` and thus locate all
+        # reminders with `waldo` either in the summary or d (the description).
+
+        style: dark
+        # dark or light. Set the defaults for dark or light terminal
+        # backgounds. Some output may not be visible unless this is set
+        # correctly for your display.
+
+        type_colors:
+        # A dictionary with type keys and corresponding named-color or hex
+        # values. The default colors are determined by the 'dark' or 'light'
+        # style setting as follows:
+        #
+        #     key           dark default        light default
+        #  -----------    -----------------   -----------------
+        #  available       'LightSkyBlue',     'DarkBlue',
+        #  begin           'Gold',             'DarkViolet',
+        #  event           'LimeGreen',        'DarkGreen',
+        #  finished        'DarkGrey',         'LightSlateGrey',
+        #  inbox           'OrangeRed',        'MediumVioletRed',
+        #  journal         'GoldenRod',        'Brown',
+        #  pastdue         'LightSalmon',      'Red',
+        #  plain           'Ivory',            'Black',
+        #  today           'Ivory bold',       'Black bold',
+        #  used            'Khaki',            'DodgerBlue',
+        #  waiting         'SlateGrey',        'DarkSlateBlue',
+        #  wrap            'ForestGreen',      'LightGrey',
+        #  running         'OrangeRed',        'Gold',
+        #  paused          'MediumVioletRed',   'DarkViolet',
+        # Explanations for the key names:
+        #     available:    available task/job reminders
+        #     begin:        begin by warnings
+        #     event:        event reminders
+        #     finished:     finished task/job reminders
+        #     inbox:        inbox reminders
+        #     journal:      journal reminders
+        #     pastdue:      pasdue task warnings
+        #     plain:        headings such as outline branches
+        #     today:        the current and following agenda date headings
+        #     used:         used time rows in engaged and used time views
+        #     waiting:      waiting job reminders (jobs with unfinished prereqs)
+        #     wrap:         before and after rows for events in agenda view with
+        #                   @w entries
+        #     running:      status bar color for 'r', running timer
+        #     paused:       status bar color for 'p', paused timer
+        #
+        # E.g., with style 'dark', the default color for 'available' is
+        # 'LightSkyBlue'. This entry
+        #   colors:
+        #       available: CornFlowerBlue
+        # would change the 'available' color to 'CornflowerBlue' while leaving
+        # the other 'dark' colors unchanged.
+        #
+        # To preview the namedcolors, download "namedcolors.py" from
+        #    "https://github.com/dagraham/etm-dgraham",
+        # open a terminal with your chosen background color and run
+        #    python3 <path to namedcolors.py>
+        # at the command prompt.
+
+        window_colors:
+        # A dictionary with style component keys and corresponding lists of
+        #    [background, foreground, attribute]
+        # components. background and foreground can either be named colors,
+        # hex colors, or ''. Attribute is an optional font attribute such
+        # as 'bold' which must, of course, be supported by the font used in
+        # your terminal. The default settings are determined by the 'dark'
+        # or 'light' style setting as follows:
+        #
+        #    key                       dark default                  light default
+        # -------------------    -----------------------------  -----------------------------
+        # ask:                    [grey2, Lime, bold]           [Cornsilk, Lime, bold]
+        # button.focused:         [DarkGreen, White]            [DarkGreen, White]
+        # details:                [, Ivory]                     [, Black]
+        # dialog shadow:          [#444444, ]                   [#444444, ]
+        # dialog:                 [DarkSlateGrey, White]        [DimGrey, White]
+        # dialog-entry:           [White, Black]                [White, Black]
+        # dialog-output:          [DarkSlateGrey, Lime]         [DimGrey, Lime]
+        # dialog.body label:      [, White]                     [, White]
+        # dialog.body:            [DarkSlateGrey, White]        [DimGrey, White]
+        # entry:                  [grey2, LightGoldenRodYellow] [Cornsilk, LightGoldenRodYellow]
+        # frame.label:            [DarkSlateGrey, White]        [DimGrey, White]
+        # menu:                   [DarkSlateGrey, White]        [DimGrey, White]
+        # menu-bar:               [grey1, White]                [grey1, White]
+        # menu-bar.selected-item: [#ffffff, #000000]            [#ffffff, #000000]
+        # menu.border:            [, #aaaaaa]                   [, #aaaaaa]
+        # not-searching:          [, #222222]                   [, #777777]
+        # query:                  [, Ivory]                     [, Black]
+        # reply:                  [grey2, DeepSkyBlue]          [Cornsilk, DeepSkyBlue]
+        # shadow:                 [#222222, ]                   [#222222, ]
+        # status:                 [grey1, White]                [grey1, White]
+        # status.key:             [, #ffaa00]                   [, #ffaa00]
+        # status.position:        [, #aaaa00]                   [, #aaaa00]
+        # text-area:              [grey2, Ivory]                [Cornsilk, Black]
+        # window.border shadow:   [, #444444]                   [, #444444]
+        # window.border:          [, #888888]                   [, #888888]
+        #
+        # Note that 'grey1' (#396060) and 'grey2' (#1d3030) are colors named
+        # within etm itself. They are, respectively, one shade lighter and two
+        # shades darker than DarkSlateGrey.
+        #
+        # Any of the style attributes above can be modified. E.g., with style
+        # 'dark', the default for 'text-area' is [grey2, Ivory]. This entry
+        #   window_colors:
+        #       text-area: [Black, White]
+        # would change the 'text-area' setting to 'Black' as the background color
+        # and 'White' as the foreground color while leaving the other style settings
+        # unchanged.
+        #### end cfg.yaml ####
 
 
 See [Saved Queries](#saved-queries) for more information about queries that allow for replaceable parameters.
 
 Note that in the 'dictionary' entries above, the components must be indented (using 2 spaces not tabs). E.g., the illustrative alert entry would be:
 
 	alerts:
```

### Comparing `etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.0/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.0/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etmlogo.png` & `etm-dgraham-5.1.0/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etmlogo_small.png` & `etm-dgraham-5.1.0/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/etmview_agenda.png` & `etm-dgraham-5.1.0/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/namedcolors.py` & `etm-dgraham-5.1.0/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/new.png` & `etm-dgraham-5.1.0/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/setup.py` & `etm-dgraham-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/test/test_parser.py` & `etm-dgraham-5.1.0/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.0/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/utilities/etm_in` & `etm-dgraham-5.1.0/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/utilities/inbasket` & `etm-dgraham-5.1.0/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.9/utilities/open_in_mutt` & `etm-dgraham-5.1.0/utilities/open_in_mutt`

 * *Files identical despite different names*

