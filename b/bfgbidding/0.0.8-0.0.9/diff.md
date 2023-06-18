# Comparing `tmp/bfgbidding-0.0.8.tar.gz` & `tmp/bfgbidding-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgbidding-0.0.8.tar", last modified: Mon Mar  6 14:30:52 2023, max compression
+gzip compressed data, was "bfgbidding-0.0.9.tar", last modified: Wed Mar  8 17:53:37 2023, max compression
```

## Comparing `bfgbidding-0.0.8.tar` & `bfgbidding-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-06 14:30:52.544906 bfgbidding-0.0.8/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgbidding-0.0.8/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1211 2023-03-06 14:30:52.544906 bfgbidding-0.0.8/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      143 2023-02-01 12:21:51.000000 bfgbidding-0.0.8/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-06 14:30:52.534906 bfgbidding-0.0.8/bfgbidding/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      340 2023-03-06 14:16:39.000000 bfgbidding-0.0.8/bfgbidding/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       31 2023-03-06 14:27:30.000000 bfgbidding-0.0.8/bfgbidding/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-06 14:30:52.538240 bfgbidding-0.0.8/bfgbidding/comment_data/
--rw-r--r--   0 jeff      (1000) jeff      (1001)    15168 2023-03-03 11:54:29.000000 bfgbidding-0.0.8/bfgbidding/comment_data/comment_xref.json
--rw-r--r--   0 jeff      (1000) jeff      (1001)    39565 2023-03-06 08:41:20.000000 bfgbidding-0.0.8/bfgbidding/comment_data/comments.json
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12876 2023-02-14 14:26:31.000000 bfgbidding-0.0.8/bfgbidding/comment_data/strategies.json
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7871 2023-03-03 11:09:08.000000 bfgbidding-0.0.8/bfgbidding/comment_data/strategy_xref.json
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-06 14:30:52.541573 bfgbidding-0.0.8/bfgbidding/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgbidding-0.0.8/bfgbidding/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    50422 2023-03-01 17:59:17.000000 bfgbidding-0.0.8/bfgbidding/source/acol_advancers_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5569 2023-03-01 17:59:17.000000 bfgbidding-0.0.8/bfgbidding/source/acol_advancers_later_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    32314 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_advancers_rebid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3747 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_bidding.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9159 2023-03-03 12:14:06.000000 bfgbidding-0.0.8/bfgbidding/source/acol_openers_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4830 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_openers_later_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    81954 2023-03-03 12:20:33.000000 bfgbidding-0.0.8/bfgbidding/source/acol_openers_rebid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43032 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_openers_third_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    28291 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_overcallers_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    51742 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_overcallers_rebid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11127 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_overcallers_third_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    53010 2023-03-03 12:20:33.000000 bfgbidding-0.0.8/bfgbidding/source/acol_responders_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    18599 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_responders_later_bid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)   101814 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/acol_responders_rebid.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7519 2023-03-03 12:20:33.000000 bfgbidding-0.0.8/bfgbidding/source/bidding.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7382 2023-02-01 09:33:14.000000 bfgbidding-0.0.8/bfgbidding/source/blackwood.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2205 2023-03-06 14:27:30.000000 bfgbidding-0.0.8/bfgbidding/source/comments.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    41259 2023-03-03 12:20:33.000000 bfgbidding-0.0.8/bfgbidding/source/hand.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2910 2023-02-13 17:06:24.000000 bfgbidding-0.0.8/bfgbidding/source/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10158 2023-03-03 17:04:06.000000 bfgbidding-0.0.8/bfgbidding/source/strategy_xref.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-06 14:30:52.544906 bfgbidding-0.0.8/bfgbidding/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-05-05 11:34:45.000000 bfgbidding-0.0.8/bfgbidding/tests/__init__.py
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    27015 2020-05-26 11:06:23.000000 bfgbidding-0.0.8/bfgbidding/tests/board_xref.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6815 2023-02-16 14:11:39.000000 bfgbidding-0.0.8/bfgbidding/tests/pbn.py
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)     2173 2023-02-16 14:19:29.000000 bfgbidding-0.0.8/bfgbidding/tests/test_bidding.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-06 14:30:52.534906 bfgbidding-0.0.8/bfgbidding.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1211 2023-03-06 14:30:52.000000 bfgbidding-0.0.8/bfgbidding.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1337 2023-03-06 14:30:52.000000 bfgbidding-0.0.8/bfgbidding.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-03-06 14:30:52.000000 bfgbidding-0.0.8/bfgbidding.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       21 2023-03-06 14:30:52.000000 bfgbidding-0.0.8/bfgbidding.egg-info/requires.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       11 2023-03-06 14:30:52.000000 bfgbidding-0.0.8/bfgbidding.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       63 2023-03-06 14:30:52.544906 bfgbidding-0.0.8/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1370 2023-03-06 13:22:38.000000 bfgbidding-0.0.8/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:53:37.659112 bfgbidding-0.0.9/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgbidding-0.0.9/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1247 2023-03-08 17:53:37.659112 bfgbidding-0.0.9/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      143 2023-02-01 12:21:51.000000 bfgbidding-0.0.9/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:53:37.649112 bfgbidding-0.0.9/bfgbidding/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      362 2023-03-08 17:50:48.000000 bfgbidding-0.0.9/bfgbidding/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       31 2023-03-08 17:51:10.000000 bfgbidding-0.0.9/bfgbidding/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:53:37.652446 bfgbidding-0.0.9/bfgbidding/comment_data/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    26902 2023-02-22 10:15:55.000000 bfgbidding-0.0.9/bfgbidding/comment_data/call_board_xref.json
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    15168 2023-03-03 11:54:29.000000 bfgbidding-0.0.9/bfgbidding/comment_data/comment_xref.json
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    39565 2023-03-06 08:41:20.000000 bfgbidding-0.0.9/bfgbidding/comment_data/comments.json
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    12876 2023-02-14 14:26:31.000000 bfgbidding-0.0.9/bfgbidding/comment_data/strategies.json
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7871 2023-03-03 11:09:08.000000 bfgbidding-0.0.9/bfgbidding/comment_data/strategy_xref.json
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:53:37.655779 bfgbidding-0.0.9/bfgbidding/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgbidding-0.0.9/bfgbidding/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    50422 2023-03-01 17:59:17.000000 bfgbidding-0.0.9/bfgbidding/source/acol_advancers_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5569 2023-03-01 17:59:17.000000 bfgbidding-0.0.9/bfgbidding/source/acol_advancers_later_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    32314 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_advancers_rebid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3747 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_bidding.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9159 2023-03-03 12:14:06.000000 bfgbidding-0.0.9/bfgbidding/source/acol_openers_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4830 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_openers_later_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    81954 2023-03-03 12:20:33.000000 bfgbidding-0.0.9/bfgbidding/source/acol_openers_rebid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    43032 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_openers_third_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    28291 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_overcallers_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    51742 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_overcallers_rebid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11127 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_overcallers_third_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    53010 2023-03-03 12:20:33.000000 bfgbidding-0.0.9/bfgbidding/source/acol_responders_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    18599 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_responders_later_bid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)   101814 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/acol_responders_rebid.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7519 2023-03-03 12:20:33.000000 bfgbidding-0.0.9/bfgbidding/source/bidding.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7382 2023-02-01 09:33:14.000000 bfgbidding-0.0.9/bfgbidding/source/blackwood.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2205 2023-03-06 14:27:30.000000 bfgbidding-0.0.9/bfgbidding/source/comments.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    41259 2023-03-03 12:20:33.000000 bfgbidding-0.0.9/bfgbidding/source/hand.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2910 2023-02-13 17:06:24.000000 bfgbidding-0.0.9/bfgbidding/source/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    10158 2023-03-03 17:04:06.000000 bfgbidding-0.0.9/bfgbidding/source/strategy_xref.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:53:37.659112 bfgbidding-0.0.9/bfgbidding/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-05-05 11:34:45.000000 bfgbidding-0.0.9/bfgbidding/tests/__init__.py
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    27015 2020-05-26 11:06:23.000000 bfgbidding-0.0.9/bfgbidding/tests/board_xref.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6815 2023-02-16 14:11:39.000000 bfgbidding-0.0.9/bfgbidding/tests/pbn.py
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)     2173 2023-02-16 14:19:29.000000 bfgbidding-0.0.9/bfgbidding/tests/test_bidding.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-03-08 17:53:37.649112 bfgbidding-0.0.9/bfgbidding.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1247 2023-03-08 17:53:37.000000 bfgbidding-0.0.9/bfgbidding.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1382 2023-03-08 17:53:37.000000 bfgbidding-0.0.9/bfgbidding.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-03-08 17:53:37.000000 bfgbidding-0.0.9/bfgbidding.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       21 2023-03-08 17:53:37.000000 bfgbidding-0.0.9/bfgbidding.egg-info/requires.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       11 2023-03-08 17:53:37.000000 bfgbidding-0.0.9/bfgbidding.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       63 2023-03-08 17:53:37.659112 bfgbidding-0.0.9/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1370 2023-03-06 13:22:38.000000 bfgbidding-0.0.9/setup.py
```

### Comparing `bfgbidding-0.0.8/LICENSE.txt` & `bfgbidding-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/PKG-INFO` & `bfgbidding-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgbidding
-Version: 0.0.8
+Version: 0.0.9
 Summary: """A collection of modules that supports bidding in Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgbidding.git
 Download-URL: https://pypi.org/project/bfgbidding/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, bidding
@@ -20,17 +20,17 @@
 ```bash
 pip install bfgbidding
 ```
 
 
 # Version History
 
-Version 0.0.8 06 Mar 2023
+Version 0.0.9 08 Mar 2023
 
-1. xxx
+1. Add comments, strategies to __init__.py
 
 ------
 
 Version 0.0.7 06 Mar 2023
 
 1. Move comment_data
```

### Comparing `bfgbidding-0.0.8/bfgbidding/comment_data/comment_xref.json` & `bfgbidding-0.0.9/bfgbidding/comment_data/comment_xref.json`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/comment_data/comments.json` & `bfgbidding-0.0.9/bfgbidding/comment_data/comments.json`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/comment_data/strategies.json` & `bfgbidding-0.0.9/bfgbidding/comment_data/strategies.json`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/comment_data/strategy_xref.json` & `bfgbidding-0.0.9/bfgbidding/comment_data/strategy_xref.json`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_advancers_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_advancers_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_advancers_later_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_advancers_later_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_advancers_rebid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_advancers_rebid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_bidding.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_bidding.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_openers_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_openers_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_openers_later_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_openers_later_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_openers_rebid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_openers_rebid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_openers_third_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_openers_third_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_overcallers_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_overcallers_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_overcallers_rebid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_overcallers_rebid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_overcallers_third_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_overcallers_third_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_responders_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_responders_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_responders_later_bid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_responders_later_bid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/acol_responders_rebid.py` & `bfgbidding-0.0.9/bfgbidding/source/acol_responders_rebid.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/bidding.py` & `bfgbidding-0.0.9/bfgbidding/source/bidding.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/blackwood.py` & `bfgbidding-0.0.9/bfgbidding/source/blackwood.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/comments.py` & `bfgbidding-0.0.9/bfgbidding/source/comments.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/hand.py` & `bfgbidding-0.0.9/bfgbidding/source/hand.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/player.py` & `bfgbidding-0.0.9/bfgbidding/source/player.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/source/strategy_xref.py` & `bfgbidding-0.0.9/bfgbidding/source/strategy_xref.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/tests/board_xref.py` & `bfgbidding-0.0.9/bfgbidding/tests/board_xref.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/tests/pbn.py` & `bfgbidding-0.0.9/bfgbidding/tests/pbn.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding/tests/test_bidding.py` & `bfgbidding-0.0.9/bfgbidding/tests/test_bidding.py`

 * *Files identical despite different names*

### Comparing `bfgbidding-0.0.8/bfgbidding.egg-info/PKG-INFO` & `bfgbidding-0.0.9/bfgbidding.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgbidding
-Version: 0.0.8
+Version: 0.0.9
 Summary: """A collection of modules that supports bidding in Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgbidding.git
 Download-URL: https://pypi.org/project/bfgbidding/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, bidding
@@ -20,17 +20,17 @@
 ```bash
 pip install bfgbidding
 ```
 
 
 # Version History
 
-Version 0.0.8 06 Mar 2023
+Version 0.0.9 08 Mar 2023
 
-1. xxx
+1. Add comments, strategies to __init__.py
 
 ------
 
 Version 0.0.7 06 Mar 2023
 
 1. Move comment_data
```

### Comparing `bfgbidding-0.0.8/bfgbidding.egg-info/SOURCES.txt` & `bfgbidding-0.0.9/bfgbidding.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 bfgbidding/__init__.py
 bfgbidding/_version.py
 bfgbidding.egg-info/PKG-INFO
 bfgbidding.egg-info/SOURCES.txt
 bfgbidding.egg-info/dependency_links.txt
 bfgbidding.egg-info/requires.txt
 bfgbidding.egg-info/top_level.txt
+bfgbidding/comment_data/call_board_xref.json
 bfgbidding/comment_data/comment_xref.json
 bfgbidding/comment_data/comments.json
 bfgbidding/comment_data/strategies.json
 bfgbidding/comment_data/strategy_xref.json
 bfgbidding/source/__init__.py
 bfgbidding/source/acol_advancers_bid.py
 bfgbidding/source/acol_advancers_later_bid.py
```

### Comparing `bfgbidding-0.0.8/setup.py` & `bfgbidding-0.0.9/setup.py`

 * *Files identical despite different names*

