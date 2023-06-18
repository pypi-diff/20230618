# Comparing `tmp/osm_easy_api-0.4.2.tar.gz` & `tmp/osm_easy_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-0.4.2.tar", last modified: Sun Jun 11 19:52:09 2023, max compression
+gzip compressed data, was "osm_easy_api-1.0.0.tar", last modified: Sun Jun 18 21:46:37 2023, max compression
```

## Comparing `osm_easy_api-0.4.2.tar` & `osm_easy_api-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.247793 osm_easy_api-0.4.2/
--rw-rw-rw-   0        0        0     3123 2023-06-11 19:50:37.000000 osm_easy_api-0.4.2/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/LICENSE.md
--rw-rw-rw-   0        0        0    44375 2023-06-11 19:52:09.247793 osm_easy_api-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4514 2023-05-03 21:30:36.000000 osm_easy_api-0.4.2/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2023-06-11 19:52:09.250287 osm_easy_api-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.164519 osm_easy_api-0.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.179134 osm_easy_api-0.4.2/src/osm_easy_api/
--rw-rw-rw-   0        0        0      107 2023-06-10 21:50:03.000000 osm_easy_api-0.4.2/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.206474 osm_easy_api-0.4.2/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.224299 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    14405 2023-04-02 18:15:22.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     4369 2023-04-02 18:15:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    17049 2023-06-11 19:37:43.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5540 2023-04-02 18:17:21.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    11406 2023-04-02 18:18:10.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.238508 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     4381 2023-06-11 19:48:45.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-0.4.2/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.242004 osm_easy_api-0.4.2/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-0.4.2/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-0.4.2/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.247793 osm_easy_api-0.4.2/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-0.4.2/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:52:09.200017 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    44375 2023-06-11 19:52:09.000000 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-06-11 19:52:09.000000 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 19:52:09.000000 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-06-11 19:52:09.000000 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-11 19:52:09.000000 osm_easy_api-0.4.2/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.084672 osm_easy_api-1.0.0/
+-rw-rw-rw-   0        0        0     3488 2023-06-18 20:59:09.000000 osm_easy_api-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0    45172 2023-06-18 21:46:37.085674 osm_easy_api-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4946 2023-06-18 21:44:28.000000 osm_easy_api-1.0.0/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1197 2023-06-18 21:46:37.087751 osm_easy_api-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.020171 osm_easy_api-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.031239 osm_easy_api-1.0.0/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      107 2023-06-18 21:01:38.000000 osm_easy_api-1.0.0/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.059458 osm_easy_api-1.0.0/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3033 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     4336 2023-03-08 21:18:46.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.068878 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      520 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    14641 2023-06-18 20:57:38.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     4464 2023-06-18 20:57:49.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    17201 2023-06-18 20:56:56.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     1062 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5559 2023-06-18 20:56:12.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    11501 2023-06-18 20:56:07.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     7047 2023-04-02 18:18:25.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1025 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.078663 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     8062 2023-06-18 17:27:38.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      432 2023-03-22 23:03:24.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2023-03-14 14:11:03.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1144 2023-06-10 21:48:54.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     2635 2023-05-03 15:23:00.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     2786 2023-06-10 21:42:40.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     1725 2023-06-10 21:48:37.000000 osm_easy_api-1.0.0/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.081426 osm_easy_api-1.0.0/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6164 2023-04-01 19:34:36.000000 osm_easy_api-1.0.0/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     9075 2023-03-07 21:24:24.000000 osm_easy_api-1.0.0/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.084672 osm_easy_api-1.0.0/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0       82 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-1.0.0/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2023-06-18 21:46:37.055558 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    45172 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 21:15:07.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-18 21:46:37.000000 osm_easy_api-1.0.0/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-0.4.2/CHANGELOG.md` & `osm_easy_api-1.0.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.0]
+### Added
+- `to_xml()` method in `OsmChange`.
+- `upload()` method in `changeset` `endpoint` has new optional arguments.
+- Test for `to_xml()` method in `OsmChange`.
+- `# pragma: no cover` for unexpected api errors (Those that are not in the specification on the wiki).
+
+### Changed
+- Private `_to_xml()` method in `OsmChange` is now static.
+
 ## [0.4.2]
+
 ### Changed
 - Order of elements in xml generated by `Way._to_xml()`. First tags, then nodes.
 
 ### Fixed
 - `Relation._to_xml()` was returning an xml without osm tags.
 - Deleted disused variable in `Node._to_xml()`.
 - Fixed incorrect relation parsing of data recived by `full` endpoint.
```

### Comparing `osm_easy_api-0.4.2/LICENSE.md` & `osm_easy_api-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/PKG-INFO` & `osm_easy_api-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 206f 736d  : 2.1..Name: osm
 00000020: 5f65 6173 795f 6170 690d 0a56 6572 7369  _easy_api..Versi
-00000030: 6f6e 3a20 302e 342e 320d 0a53 756d 6d61  on: 0.4.2..Summa
+00000030: 6f6e 3a20 312e 302e 300d 0a53 756d 6d61  on: 1.0.0..Summa
 00000040: 7279 3a20 5079 7468 6f6e 2070 6163 6b61  ry: Python packa
 00000050: 6765 2066 6f72 2070 6172 7369 6e67 206f  ge for parsing o
 00000060: 736d 2064 6966 6673 2061 6e64 2063 6f6d  sm diffs and com
 00000070: 6d75 6e69 6361 7469 6e67 2077 6974 6820  municating with 
 00000080: 7468 6520 6f73 6d20 6170 692e 0d0a 486f  the osm api...Ho
 00000090: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 000000a0: 2f67 6974 6875 622e 636f 6d2f 646f 6365  /github.com/doce
@@ -50,2725 +50,2775 @@
 00000310: 3a20 332e 3131 0d0a 5265 7175 6972 6573  : 3.11..Requires
 00000320: 2d50 7974 686f 6e3a 203e 3d33 2e31 300d  -Python: >=3.10.
 00000330: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000340: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000350: 6d61 726b 646f 776e 0d0a 5072 6f76 6964  markdown..Provid
 00000360: 6573 2d45 7874 7261 3a20 7465 7374 696e  es-Extra: testin
 00000370: 670d 0a4c 6963 656e 7365 2d46 696c 653a  g..License-File:
-00000380: 204c 4943 454e 5345 2e6d 640d 0a0d 0a23   LICENSE.md....#
-00000390: 206f 736d 5f65 6173 795f 6170 690d 0a0d   osm_easy_api...
-000003a0: 0a21 5b54 6573 7473 5d28 6874 7470 733a  .![Tests](https:
-000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
-000003c0: 656e 7459 542f 6175 746f 6d61 7465 642d  entYT/automated-
-000003d0: 7079 7468 6f6e 2d74 6573 7473 2d74 6573  python-tests-tes
-000003e0: 7469 6e67 2d72 6570 6f2f 6163 7469 6f6e  ting-repo/action
-000003f0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000400: 732e 7961 6d6c 2f62 6164 6765 2e73 7667  s.yaml/badge.svg
-00000410: 290d 0a21 5b63 6f76 6572 6167 655d 2868  )..![coverage](h
-00000420: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000430: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000440: 2f64 6f63 656e 7459 542f 6f73 6d5f 6561  /docentYT/osm_ea
-00000450: 7379 5f61 7069 2f33 3838 3961 6536 3236  sy_api/3889ae626
-00000460: 6265 3335 3138 3332 3533 3438 3536 3436  be35183253485646
-00000470: 6237 6265 3965 3233 3561 3266 6332 372f  b7be9e235a2fc27/
-00000480: 636f 7665 7261 6765 2d62 6164 6765 2e73  coverage-badge.s
-00000490: 7667 290d 0a5b 215b 5079 5049 2076 6572  vg)..[![PyPI ver
-000004a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
-000004b0: 6467 652e 6675 7279 2e69 6f2f 7079 2f6f  dge.fury.io/py/o
-000004c0: 736d 5f65 6173 795f 6170 692e 7376 6729  sm_easy_api.svg)
-000004d0: 5d28 6874 7470 733a 2f2f 6261 6467 652e  ](https://badge.
-000004e0: 6675 7279 2e69 6f2f 7079 2f6f 736d 5f65  fury.io/py/osm_e
-000004f0: 6173 795f 6170 6929 0d0a 0d0a 5b4d 6520  asy_api)....[Me 
-00000500: 6f6e 206f 7065 6e73 7472 6565 746d 6170  on openstreetmap
-00000510: 5d28 6874 7470 733a 2f2f 7777 772e 6f70  ](https://www.op
-00000520: 656e 7374 7265 6574 6d61 702e 6f72 672f  enstreetmap.org/
-00000530: 7573 6572 2f6b 7769 6174 656b 5f31 3233  user/kwiatek_123
-00000540: 290d 0a0d 0a50 7974 686f 6e20 7061 636b  )....Python pack
-00000550: 6167 6520 666f 7220 7061 7273 696e 6720  age for parsing 
-00000560: 6f73 6d20 6469 6666 7320 616e 6420 636f  osm diffs and co
-00000570: 6d6d 756e 6963 6174 696e 6720 7769 7468  mmunicating with
-00000580: 2074 6865 206f 736d 2061 7069 2e20 5365   the osm api. Se
-00000590: 6520 4150 492e 7478 7420 666f 7220 6c69  e API.txt for li
-000005a0: 7374 206f 6620 7375 7070 6f72 7465 6420  st of supported 
-000005b0: 656e 6470 6f69 6e74 732e 0d0a 0d0a 2323  endpoints.....##
-000005c0: 2057 6861 7427 7320 7468 6520 706f 696e   What's the poin
-000005d0: 7420 6f66 2074 6869 7320 7061 636b 6167  t of this packag
-000005e0: 653f 0d0a 0d0a 5468 6973 2070 6163 6b61  e?....This packa
-000005f0: 6765 2077 6173 2063 7265 6174 6564 2074  ge was created t
-00000600: 6f20 7072 6f76 6964 6520 616e 2065 6173  o provide an eas
-00000610: 7920 7761 7920 746f 2063 7265 6174 6520  y way to create 
-00000620: 6175 746f 6d61 7465 6420 7363 7269 7074  automated script
-00000630: 7320 616e 6420 7072 6f67 7261 6d73 2074  s and programs t
-00000640: 6861 7420 7573 6520 6469 6666 2061 6e64  hat use diff and
-00000650: 2f6f 7220 6f73 6d20 6170 692e 2054 6865  /or osm api. The
-00000660: 206d 6169 6e20 6164 7661 6e74 6167 6520   main advantage 
-00000670: 6973 2074 6865 2063 6c61 7373 6573 2028  is the classes (
-00000680: 6461 7461 5f63 6c61 7373 6573 2920 7468  data_classes) th
-00000690: 6174 2070 726f 7669 6465 2064 6174 6120  at provide data 
-000006a0: 6f66 2065 6c65 6d65 6e74 7320 286e 6f64  of elements (nod
-000006b0: 652c 2077 6179 2c20 7265 6c61 7469 6f6e  e, way, relation
-000006c0: 2c20 4f73 6d43 6861 6e67 652c 2065 7463  , OsmChange, etc
-000006d0: 2e29 2069 6e20 6120 7265 6164 6162 6c65  .) in a readable
-000006e0: 2077 6179 2061 6e64 2074 6865 2070 6f73   way and the pos
-000006f0: 7369 6269 6c69 7479 2074 6f20 7573 6520  sibility to use 
-00000700: 7468 656d 2069 6e20 6469 6666 2061 6e64  them in diff and
-00000710: 2061 7069 2077 6974 686f 7574 2077 6f72   api without wor
-00000720: 7279 696e 6720 6162 6f75 7420 6d69 7373  rying about miss
-00000730: 696e 6720 6461 7461 206f 7220 6469 6374  ing data or dict
-00000740: 696f 6e61 7269 6573 2e20 596f 7520 6361  ionaries. You ca
-00000750: 6e20 6561 7369 6c79 2066 696e 6420 6e6f  n easily find no
-00000760: 6465 7320 696e 2064 6966 662c 2061 6464  des in diff, add
-00000770: 2061 2074 6167 2074 6f20 7468 656d 2061   a tag to them a
-00000780: 6e64 2073 656e 6420 7468 6520 636f 7272  nd send the corr
-00000790: 6563 7465 6420 7665 7273 696f 6e20 746f  ected version to
-000007a0: 206f 736d 2e0d 0a0d 0a23 2320 5768 6174   osm.....## What
-000007b0: 206e 6578 743f 0d0a 5468 6520 706c 616e   next?..The plan
-000007c0: 2069 7320 746f 206f 7074 696d 6973 6520   is to optimise 
-000007d0: 616e 6420 696d 7072 6f76 6520 7468 6520  and improve the 
-000007e0: 636f 6465 2c20 6164 6420 7375 7070 6f72  code, add suppor
-000007f0: 7420 666f 7220 6770 7820 7472 6163 6573  t for gpx traces
-00000800: 2c20 7273 7320 7375 7070 6f72 7420 616e  , rss support an
-00000810: 6420 6f76 6572 7061 7373 2061 7069 2e0d  d overpass api..
-00000820: 0a0d 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
-00000830: 6e0d 0a0d 0a57 6f72 6b73 206f 6e20 7079  n....Works on py
-00000840: 7468 6f6e 203e 3d20 332e 3130 2e20 2844  thon >= 3.10. (D
-00000850: 7565 2074 6f20 6e65 7720 7479 7065 6869  ue to new typehi
-00000860: 6e74 7320 7374 616e 6461 7264 290d 0a0d  nts standard)...
-00000870: 0a49 6e73 7461 6c6c 2060 6f73 6d5f 6561  .Install `osm_ea
-00000880: 7379 5f61 7069 6020 6672 6f6d 205b 5079  sy_api` from [Py
-00000890: 5069 5d28 6874 7470 733a 2f2f 7079 7069  Pi](https://pypi
-000008a0: 2e6f 7267 2f70 726f 6a65 6374 2f6f 736d  .org/project/osm
-000008b0: 2d65 6173 792d 6170 692f 293a 0d0a 6060  -easy-api/):..``
-000008c0: 600d 0a70 6970 2069 6e73 7461 6c6c 206f  `..pip install o
-000008d0: 736d 5f65 6173 795f 6170 690d 0a60 6060  sm_easy_api..```
-000008e0: 200d 0a0d 0a23 2044 6f63 756d 656e 7461   ....# Documenta
-000008f0: 7469 6f6e 0d0a 0d0a 596f 7520 6361 6e20  tion....You can 
-00000900: 7669 6577 2064 6f63 756d 656e 7461 7469  view documentati
-00000910: 6f6e 206f 6e20 5b67 6974 6875 622d 7061  on on [github-pa
-00000920: 6765 735d 2868 7474 7073 3a2f 2f64 6f63  ges](https://doc
-00000930: 656e 7479 742e 6769 7468 7562 2e69 6f2f  entyt.github.io/
-00000940: 6f73 6d5f 6561 7379 5f61 7069 2f6f 736d  osm_easy_api/osm
-00000950: 5f65 6173 795f 6170 692e 6874 6d6c 292e  _easy_api.html).
-00000960: 0d0a 0d0a 446f 6375 6d65 6e74 6174 696f  ....Documentatio
-00000970: 6e20 6973 2062 7569 6c64 2075 7369 6e67  n is build using
-00000980: 205b 7064 6f63 5d28 6874 7470 733a 2f2f   [pdoc](https://
-00000990: 7064 6f63 2e64 6576 292e 0d0a 546f 2072  pdoc.dev)...To r
-000009a0: 756e 2064 6f63 7320 6f6e 2079 6f75 7220  un docs on your 
-000009b0: 6d61 6368 696e 6520 7573 6520 7072 6566  machine use pref
-000009c0: 6572 7265 6420 636f 6d6d 616e 643a 2060  erred command: `
-000009d0: 7064 6f63 202d 2d64 6f63 666f 726d 6174  pdoc --docformat
-000009e0: 2067 6f6f 676c 6520 2d2d 6e6f 2d73 686f   google --no-sho
-000009f0: 772d 736f 7572 6365 206f 736d 5f65 6173  w-source osm_eas
-00000a00: 795f 6170 6920 216f 736d 5f65 6173 795f  y_api !osm_easy_
-00000a10: 6170 692e 7574 696c 7360 2e0d 0a0d 0a23  api.utils`.....#
-00000a20: 2045 7861 6d70 6c65 730d 0a0d 0a23 2320   Examples....## 
-00000a30: 4449 4646 0d0a 0d0a 2323 2320 5072 696e  DIFF....### Prin
-00000a40: 7420 7472 6565 730d 0a0d 0a60 6060 7079  t trees....```py
-00000a50: 0d0a 6672 6f6d 206f 736d 5f65 6173 795f  ..from osm_easy_
-00000a60: 6170 6920 696d 706f 7274 204e 6f64 652c  api import Node,
-00000a70: 2044 6966 662c 2046 7265 7175 656e 6379   Diff, Frequency
-00000a80: 0d0a 0d0a 2320 446f 776e 6c6f 6164 2064  ....# Download d
-00000a90: 6966 6620 6672 6f6d 206c 6173 7420 686f  iff from last ho
-00000aa0: 7572 2e0d 0a64 203d 2044 6966 6628 4672  ur...d = Diff(Fr
-00000ab0: 6571 7565 6e63 792e 484f 5552 290d 0a0d  equency.HOUR)...
-00000ac0: 0a23 2047 6574 204d 6574 6120 6e61 6d65  .# Get Meta name
-00000ad0: 6474 7570 6c65 2066 6f72 2064 6966 6620  dtuple for diff 
-00000ae0: 6d65 7461 6461 7461 2061 6e64 2067 656e  metadata and gen
-00000af0: 6572 6174 6f72 2074 6861 7420 7061 7273  erator that pars
-00000b00: 6520 6469 6666 2066 696c 652e 0d0a 6d65  e diff file...me
-00000b10: 7461 2c20 6765 6e20 3d20 642e 6765 7428  ta, gen = d.get(
-00000b20: 7461 6773 3d22 6e61 7475 7261 6c22 290d  tags="natural").
-00000b30: 0a0d 0a23 2050 7269 6e74 2061 6c6c 2063  ...# Print all c
-00000b40: 7265 6174 6564 2c20 6d6f 6469 6669 6564  reated, modified
-00000b50: 2061 6e64 2064 656c 6574 6564 204e 6f64   and deleted Nod
-00000b60: 6573 2077 6974 6820 6e61 7475 7261 6c3d  es with natural=
-00000b70: 7472 6565 2074 6167 2e0d 0a66 6f72 2061  tree tag...for a
-00000b80: 6374 696f 6e2c 2065 6c65 6d65 6e74 2069  ction, element i
-00000b90: 6e20 6765 6e3a 0d0a 2020 2020 6966 2074  n gen:..    if t
-00000ba0: 7970 6528 656c 656d 656e 7429 203d 3d20  ype(element) == 
-00000bb0: 4e6f 6465 2061 6e64 2065 6c65 6d65 6e74  Node and element
-00000bc0: 2e74 6167 732e 6765 7428 226e 6174 7572  .tags.get("natur
-00000bd0: 616c 2229 203d 3d20 2274 7265 6522 3a0d  al") == "tree":.
-00000be0: 0a20 2020 2020 2020 2070 7269 6e74 2861  .        print(a
-00000bf0: 6374 696f 6e2c 2065 6c65 6d65 6e74 2e69  ction, element.i
-00000c00: 6429 0d0a 6060 600d 0a0d 0a23 2323 2050  d)..```....### P
-00000c10: 7269 6e74 2069 6e63 6f72 7265 6374 6c79  rint incorrectly
-00000c20: 2074 6167 6765 6420 7369 6e67 6c65 2074   tagged single t
-00000c30: 7265 7373 0d0a 0d0a 6060 6070 790d 0a66  ress....```py..f
-00000c40: 726f 6d20 6f73 6d5f 6561 7379 5f61 7069  rom osm_easy_api
-00000c50: 2069 6d70 6f72 7420 4469 6666 2c20 4672   import Diff, Fr
-00000c60: 6571 7565 6e63 792c 2041 6374 696f 6e2c  equency, Action,
-00000c70: 204e 6f64 650d 0a0d 0a64 203d 2044 6966   Node....d = Dif
-00000c80: 6628 4672 6571 7565 6e63 792e 4441 5929  f(Frequency.DAY)
-00000c90: 0d0a 0d0a 6d65 7461 2c20 6765 6e20 3d20  ....meta, gen = 
-00000ca0: 642e 6765 7428 7461 6773 3d22 6e61 7475  d.get(tags="natu
-00000cb0: 7261 6c22 290d 0a0d 0a66 6f72 2061 6374  ral")....for act
-00000cc0: 696f 6e2c 2065 6c65 6d65 6e74 2069 6e20  ion, element in 
-00000cd0: 6765 6e3a 0d0a 2020 2020 6966 2074 7970  gen:..    if typ
-00000ce0: 6528 656c 656d 656e 7429 203d 3d20 4e6f  e(element) == No
-00000cf0: 6465 3a0d 0a20 2020 2020 2020 2069 6620  de:..        if 
-00000d00: 6163 7469 6f6e 203d 3d20 4163 7469 6f6e  action == Action
-00000d10: 2e43 5245 4154 4520 6f72 2061 6374 696f  .CREATE or actio
-00000d20: 6e20 3d3d 2041 6374 696f 6e2e 4d4f 4449  n == Action.MODI
-00000d30: 4659 3a0d 0a20 2020 2020 2020 2020 2020  FY:..           
-00000d40: 2069 6620 656c 656d 656e 742e 7461 6773   if element.tags
-00000d50: 2e67 6574 2822 6e61 7475 7261 6c22 2920  .get("natural") 
-00000d60: 3d3d 2022 776f 6f64 223a 0d0a 2020 2020  == "wood":..    
-00000d70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00000d80: 7428 656c 656d 656e 7429 0d0a 6060 600d  t(element)..```.
-00000d90: 0a45 7861 6d70 6c65 206f 7574 7075 743a  .Example output:
-00000da0: 0d0a 6060 600d 0a4e 6f64 6528 6964 203d  ..```..Node(id =
-00000db0: 2031 3032 3038 3438 3637 3137 2c20 7669   10208486717, vi
-00000dc0: 7369 626c 6520 3d20 4e6f 6e65 2c20 7665  sible = None, ve
-00000dd0: 7273 696f 6e20 3d20 312c 2063 6861 6e67  rsion = 1, chang
-00000de0: 6573 6574 5f69 6420 3d20 3132 3932 3136  eset_id = 129216
-00000df0: 3037 352c 2074 696d 6573 7461 6d70 203d  075, timestamp =
-00000e00: 2032 3032 322d 3131 2d32 3254 3030 3a31   2022-11-22T00:1
-00000e10: 363a 3434 5a2c 2075 7365 725f 6964 203d  6:44Z, user_id =
-00000e20: 2031 3734 3731 3732 312c 2074 6167 7320   17471721, tags 
-00000e30: 3d20 7b27 6c65 6166 5f74 7970 6527 3a20  = {'leaf_type': 
-00000e40: 2762 726f 6164 6c65 6176 6564 272c 2027  'broadleaved', '
-00000e50: 6e61 7475 7261 6c27 3a20 2777 6f6f 6427  natural': 'wood'
-00000e60: 7d2c 206c 6174 6974 7564 6520 3d20 3438  }, latitude = 48
-00000e70: 2e36 3532 3232 3836 2c20 6c6f 6e67 6974  .6522286, longit
-00000e80: 7564 6520 3d20 3132 2e35 3833 3830 392c  ude = 12.583809,
-00000e90: 2029 0d0a 6060 600d 0a0d 0a23 2320 4150   )..```....## AP
-00000ea0: 490d 0a0d 0a23 2323 2041 6464 206d 6973  I....### Add mis
-00000eb0: 7369 6e67 2077 696b 6964 6174 6120 7461  sing wikidata ta
-00000ec0: 670d 0a0d 0a60 6060 7079 0d0a 6672 6f6d  g....```py..from
-00000ed0: 206f 736d 5f65 6173 795f 6170 6920 696d   osm_easy_api im
-00000ee0: 706f 7274 2041 7069 2c20 4e6f 6465 2c20  port Api, Node, 
-00000ef0: 5461 6773 0d0a 0d0a 6170 6920 3d20 4170  Tags....api = Ap
-00000f00: 6928 2268 7474 7073 3a2f 2f6d 6173 7465  i("https://maste
-00000f10: 722e 6170 6973 2e64 6576 2e6f 7065 6e73  r.apis.dev.opens
-00000f20: 7472 6565 746d 6170 2e6f 7267 222c 204c  treetmap.org", L
-00000f30: 4f47 494e 2c20 5041 5353 574f 5244 290d  OGIN, PASSWORD).
-00000f40: 0a0d 0a6e 6f64 6520 3d20 6170 692e 656c  ...node = api.el
-00000f50: 656d 656e 7473 2e67 6574 284e 6f64 652c  ements.get(Node,
-00000f60: 2034 3239 3634 3630 3333 3629 2023 2057   4296460336) # W
-00000f70: 6520 6172 6520 6765 7474 696e 6720 4e6f  e are getting No
-00000f80: 6465 2077 6974 6820 6964 2034 3239 3634  de with id 42964
-00000f90: 3630 3333 3620 7768 6572 6520 7765 2077  60336 where we w
-00000fa0: 616e 7420 746f 2061 6464 2061 206e 6577  ant to add a new
-00000fb0: 2074 6167 2074 6f0d 0a6e 6f64 652e 7461   tag to..node.ta
-00000fc0: 6773 2e61 6464 2822 7769 6b69 6461 7461  gs.add("wikidata
-00000fd0: 222c 2022 5165 7861 6d70 6c65 2229 2023  ", "Qexample") #
-00000fe0: 2041 6464 2061 206e 6577 2074 6167 2074   Add a new tag t
-00000ff0: 6f20 6e6f 6465 2e0d 0a0d 0a6d 795f 6368  o node.....my_ch
-00001000: 616e 6765 7365 7420 3d20 6170 692e 6368  angeset = api.ch
-00001010: 616e 6765 7365 742e 6372 6561 7465 2822  angeset.create("
-00001020: 4164 6420 6d69 7373 696e 6720 7769 6b69  Add missing wiki
-00001030: 6461 7461 2074 6167 222c 2054 6167 7328  data tag", Tags(
-00001040: 7b22 6175 746f 6d61 7469 6322 3a20 2279  {"automatic": "y
-00001050: 6573 227d 2929 2023 2043 7265 6174 6520  es"})) # Create 
-00001060: 6e65 7720 6368 616e 6765 7365 7420 7769  new changeset wi
-00001070: 7468 2064 6573 6372 6970 7469 6f6e 2061  th description a
-00001080: 6e64 2074 6167 0d0a 6170 692e 656c 656d  nd tag..api.elem
-00001090: 656e 7473 2e75 7064 6174 6528 6e6f 6465  ents.update(node
-000010a0: 2c20 6d79 5f63 6861 6e67 6573 6574 2920  , my_changeset) 
-000010b0: 2320 5365 6e64 206e 6577 2076 6572 7369  # Send new versi
-000010c0: 6f6e 206f 6620 6120 6e6f 6465 2074 6f20  on of a node to 
-000010d0: 6f73 6d0d 0a61 7069 2e63 6861 6e67 6573  osm..api.changes
-000010e0: 6574 2e63 6c6f 7365 286d 795f 6368 616e  et.close(my_chan
-000010f0: 6765 7365 7429 2023 2043 6c6f 7365 2063  geset) # Close c
-00001100: 6861 6e67 6573 6574 2e0d 0a60 6060 0d0a  hangeset...```..
-00001110: 0d0a 2320 4e6f 7465 730d 0a0d 0a4e 6f74  ..# Notes....Not
-00001120: 6520 7468 6174 2074 6865 2066 6f6c 6c6f  e that the follo
-00001130: 7769 6e67 2063 6f64 6573 2064 6f20 7468  wing codes do th
-00001140: 6520 7361 6d65 2074 6869 6e67 0d0a 6060  e same thing..``
-00001150: 6070 790d 0a66 726f 6d20 6f73 6d5f 6561  `py..from osm_ea
-00001160: 7379 5f61 7069 2069 6d70 6f72 7420 4469  sy_api import Di
-00001170: 6666 2c20 4672 6571 7565 6e63 790d 0a0d  ff, Frequency...
-00001180: 0a64 203d 2044 6966 6628 4672 6571 7565  .d = Diff(Freque
-00001190: 6e63 792e 4441 5929 0d0a 0d0a 6d65 7461  ncy.DAY)....meta
-000011a0: 2c20 6765 6e20 3d20 642e 6765 7428 290d  , gen = d.get().
-000011b0: 0a0d 0a66 6f72 2061 6374 696f 6e2c 2065  ...for action, e
-000011c0: 6c65 6d65 6e74 2069 6e20 6765 6e3a 0d0a  lement in gen:..
-000011d0: 2020 2020 6966 2065 6c65 6d65 6e74 2e74      if element.t
-000011e0: 6167 732e 6765 7428 2273 686f 7022 2920  ags.get("shop") 
-000011f0: 3d3d 2022 636f 6e76 656e 6965 6e63 6522  == "convenience"
-00001200: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-00001210: 2865 6c65 6d65 6e74 290d 0a60 6060 0d0a  (element)..```..
-00001220: 6060 6070 790d 0a66 726f 6d20 6f73 6d5f  ```py..from osm_
-00001230: 6561 7379 5f61 7069 2069 6d70 6f72 7420  easy_api import 
-00001240: 4469 6666 2c20 4672 6571 7565 6e63 792c  Diff, Frequency,
-00001250: 2054 6167 730d 0a0d 0a64 203d 2044 6966   Tags....d = Dif
-00001260: 6628 4672 6571 7565 6e63 792e 4441 5929  f(Frequency.DAY)
-00001270: 0d0a 0d0a 6d65 7461 2c20 6765 6e20 3d20  ....meta, gen = 
-00001280: 642e 6765 7428 7461 6773 3d54 6167 7328  d.get(tags=Tags(
-00001290: 7b22 7368 6f70 223a 2022 636f 6e76 656e  {"shop": "conven
-000012a0: 6965 6e63 6522 7d29 290d 0a0d 0a66 6f72  ience"}))....for
-000012b0: 2061 6374 696f 6e2c 2065 6c65 6d65 6e74   action, element
-000012c0: 2069 6e20 6765 6e3a 0d0a 2020 2020 2020   in gen:..      
-000012d0: 2020 7072 696e 7428 656c 656d 656e 7429    print(element)
-000012e0: 0d0a 6060 600d 0a62 7574 2074 6865 2073  ..```..but the s
-000012f0: 6563 6f6e 6420 7365 656d 7320 746f 2062  econd seems to b
-00001300: 6520 6661 7374 6572 2e0d 0a0d 0a41 6c73  e faster.....Als
-00001310: 6f20 796f 7520 6361 6e20 7573 6520 4f73  o you can use Os
-00001320: 6d43 6861 6e67 6520 6f62 6a65 6374 2069  mChange object i
-00001330: 6620 796f 7520 646f 6e27 7420 7761 6e74  f you don't want
-00001340: 2074 6f20 7573 6520 6765 6e65 7261 746f   to use generato
-00001350: 720d 0a60 6060 7079 0d0a 6672 6f6d 206f  r..```py..from o
-00001360: 736d 5f65 6173 795f 6170 6920 696d 706f  sm_easy_api impo
-00001370: 7274 2044 6966 662c 2046 7265 7175 656e  rt Diff, Frequen
-00001380: 6379 2c20 4163 7469 6f6e 2c20 4e6f 6465  cy, Action, Node
-00001390: 0d0a 0d0a 6420 3d20 4469 6666 2846 7265  ....d = Diff(Fre
-000013a0: 7175 656e 6379 2e4d 494e 5554 4529 0d0a  quency.MINUTE)..
-000013b0: 0d0a 6f73 6d43 6861 6e67 6520 3d20 642e  ..osmChange = d.
-000013c0: 6765 7428 6765 6e65 7261 746f 723d 4661  get(generator=Fa
-000013d0: 6c73 6529 0d0a 0d0a 6465 6c65 7465 645f  lse)....deleted_
-000013e0: 6e6f 6465 7320 3d20 6f73 6d43 6861 6e67  nodes = osmChang
-000013f0: 652e 6765 7428 4e6f 6465 2c20 4163 7469  e.get(Node, Acti
-00001400: 6f6e 2e44 454c 4554 4529 0d0a 666f 7220  on.DELETE)..for 
-00001410: 6e6f 6465 2069 6e20 6465 6c65 7465 645f  node in deleted_
-00001420: 6e6f 6465 733a 0d0a 2020 2020 7072 696e  nodes:..    prin
-00001430: 7428 6e6f 6465 2e69 6429 0d0a 6060 600d  t(node.id)..```.
-00001440: 0a62 7574 2069 7420 6361 6e20 636f 6e73  .but it can cons
-00001450: 756d 6520 6c61 7267 6520 616d 6f75 6e74  ume large amount
-00001460: 7320 6f66 2072 616d 2061 6e64 2075 7365  s of ram and use
-00001470: 206f 6620 7468 6973 206d 6574 686f 6420   of this method 
-00001480: 6973 206e 6f74 2072 6563 6f6d 6d65 6e64  is not recommend
-00001490: 6564 2066 6f72 206c 6172 6765 2064 6966  ed for large dif
-000014a0: 6627 732e 0d0a 0d0a 2320 5465 7374 730d  f's.....# Tests.
-000014b0: 0a0d 0a59 6f75 2077 696c 6c20 6e65 6564  ...You will need
-000014c0: 2074 6f20 696e 7374 616c 6c20 6074 6573   to install `tes
-000014d0: 742d 7265 7175 6972 656d 656e 7473 2e74  t-requirements.t
-000014e0: 7874 602e 2059 6f75 2063 616e 2075 7365  xt`. You can use
-000014f0: 2074 6f78 2e0d 0a54 6f20 7275 6e20 7465   tox...To run te
-00001500: 7374 7320 6d61 6e75 616c 6c79 2075 7365  sts manually use
-00001510: 2060 7079 7468 6f6e 202d 6d20 756e 6974   `python -m unit
-00001520: 7465 7374 2064 6973 636f 7665 7260 2e0d  test discover`..
-00001530: 0a0d 0a23 2043 6861 6e67 656c 6f67 0d0a  ...# Changelog..
-00001540: 0d0a 416c 6c20 6e6f 7461 626c 6520 6368  ..All notable ch
-00001550: 616e 6765 7320 746f 2074 6869 7320 7072  anges to this pr
-00001560: 6f6a 6563 7420 7769 6c6c 2062 6520 646f  oject will be do
-00001570: 6375 6d65 6e74 6564 2069 6e20 7468 6973  cumented in this
-00001580: 2066 696c 652e 0d0a 0d0a 5468 6520 666f   file.....The fo
-00001590: 726d 6174 2069 7320 6261 7365 6420 6f6e  rmat is based on
-000015a0: 205b 4b65 6570 2061 2043 6861 6e67 656c   [Keep a Changel
-000015b0: 6f67 5d28 6874 7470 733a 2f2f 6b65 6570  og](https://keep
-000015c0: 6163 6861 6e67 656c 6f67 2e63 6f6d 2f65  achangelog.com/e
-000015d0: 6e2f 312e 302e 302f 292c 0d0a 616e 6420  n/1.0.0/),..and 
-000015e0: 7468 6973 2070 726f 6a65 6374 2061 6468  this project adh
-000015f0: 6572 6573 2074 6f20 5b53 656d 616e 7469  eres to [Semanti
-00001600: 6320 5665 7273 696f 6e69 6e67 5d28 6874  c Versioning](ht
-00001610: 7470 733a 2f2f 7365 6d76 6572 2e6f 7267  tps://semver.org
-00001620: 2f73 7065 632f 7632 2e30 2e30 2e68 746d  /spec/v2.0.0.htm
-00001630: 6c29 2e0d 0a0d 0a23 2320 5b30 2e34 2e32  l).....## [0.4.2
-00001640: 5d0d 0a23 2323 2043 6861 6e67 6564 0d0a  ]..### Changed..
-00001650: 2d20 4f72 6465 7220 6f66 2065 6c65 6d65  - Order of eleme
-00001660: 6e74 7320 696e 2078 6d6c 2067 656e 6572  nts in xml gener
-00001670: 6174 6564 2062 7920 6057 6179 2e5f 746f  ated by `Way._to
-00001680: 5f78 6d6c 2829 602e 2046 6972 7374 2074  _xml()`. First t
-00001690: 6167 732c 2074 6865 6e20 6e6f 6465 732e  ags, then nodes.
-000016a0: 0d0a 0d0a 2323 2320 4669 7865 640d 0a2d  ....### Fixed..-
-000016b0: 2060 5265 6c61 7469 6f6e 2e5f 746f 5f78   `Relation._to_x
-000016c0: 6d6c 2829 6020 7761 7320 7265 7475 726e  ml()` was return
-000016d0: 696e 6720 616e 2078 6d6c 2077 6974 686f  ing an xml witho
-000016e0: 7574 206f 736d 2074 6167 732e 0d0a 2d20  ut osm tags...- 
-000016f0: 4465 6c65 7465 6420 6469 7375 7365 6420  Deleted disused 
-00001700: 7661 7269 6162 6c65 2069 6e20 604e 6f64  variable in `Nod
-00001710: 652e 5f74 6f5f 786d 6c28 2960 2e0d 0a2d  e._to_xml()`...-
-00001720: 2046 6978 6564 2069 6e63 6f72 7265 6374   Fixed incorrect
-00001730: 2072 656c 6174 696f 6e20 7061 7273 696e   relation parsin
-00001740: 6720 6f66 2064 6174 6120 7265 6369 7665  g of data recive
-00001750: 6420 6279 2060 6675 6c6c 6020 656e 6470  d by `full` endp
-00001760: 6f69 6e74 2e0d 0a0d 0a23 2320 5b30 2e34  oint.....## [0.4
-00001770: 2e31 5d0d 0a23 2323 2043 6861 6e67 6564  .1]..### Changed
-00001780: 0d0a 2d20 5570 6461 7465 6420 6072 6571  ..- Updated `req
-00001790: 7565 7374 7360 2066 726f 6d20 6032 2e32  uests` from `2.2
-000017a0: 382e 3160 2074 6f20 6032 2e33 312e 3060  8.1` to `2.31.0`
-000017b0: 2e0d 0a0d 0a23 2320 5b30 2e34 2e30 5d0d  .....## [0.4.0].
-000017c0: 0a23 2323 2041 6464 6564 0d0a 2d20 6074  .### Added..- `t
-000017d0: 6f5f 6469 6374 2829 6020 6d65 7468 6f64  o_dict()` method
-000017e0: 2061 6e64 2060 6672 6f6d 5f64 6963 7428   and `from_dict(
-000017f0: 2960 2063 6c61 7373 206d 6574 686f 6420  )` class method 
-00001800: 746f 2060 4e6f 7465 602e 2020 0d0a 2d20  to `Note`.  ..- 
-00001810: 6074 6f5f 6469 6374 2829 6020 6d65 7468  `to_dict()` meth
-00001820: 6f64 2061 6e64 2060 6672 6f6d 5f64 6963  od and `from_dic
-00001830: 7428 2960 2063 6c61 7373 206d 6574 686f  t()` class metho
-00001840: 6420 746f 2060 436f 6d6d 656e 7460 2e0d  d to `Comment`..
-00001850: 0a2d 2060 746f 5f64 6963 7428 2960 206d  .- `to_dict()` m
-00001860: 6574 686f 6420 616e 6420 6066 726f 6d5f  ethod and `from_
-00001870: 6469 6374 2829 6020 636c 6173 7320 6d65  dict()` class me
-00001880: 7468 6f64 2074 6f20 6055 7365 7260 2e0d  thod to `User`..
-00001890: 0a2d 2044 6f63 756d 656e 7461 7469 6f6e  .- Documentation
-000018a0: 2061 626f 7574 2060 4d65 7461 6020 616e   about `Meta` an
-000018b0: 6420 6041 6374 696f 6e60 2063 6c61 7373  d `Action` class
-000018c0: 2e0d 0a2d 2041 7373 6572 7420 6572 726f  ...- Assert erro
-000018d0: 7220 2877 6974 6820 696e 666f 726d 6174  r (with informat
-000018e0: 696f 6e20 746f 2072 6570 6f72 7420 6974  ion to report it
-000018f0: 206f 6e20 6769 7468 7562 2920 7768 656e   on github) when
-00001900: 2061 7069 2072 6574 7572 6e73 2061 6e20   api returns an 
-00001910: 6572 726f 7220 636f 6465 206e 6f74 2064  error code not d
-00001920: 6573 6372 6962 6564 206f 6e20 7468 6520  escribed on the 
-00001930: 7769 6b69 2e0d 0a2d 2060 746f 5f64 6963  wiki...- `to_dic
-00001940: 7428 2960 206d 6574 686f 6420 616e 6420  t()` method and 
-00001950: 6066 726f 6d5f 6469 6374 2829 6020 636c  `from_dict()` cl
-00001960: 6173 7320 6d65 7468 6f64 2074 6f20 6028  ass method to `(
-00001970: 7265 6c61 7469 6f6e 2920 4d65 6d62 6572  relation) Member
-00001980: 602e 0d0a 0d0a 2323 2320 4669 7865 640d  `.....### Fixed.
-00001990: 0a2d 2060 4e6f 7465 6020 6361 6e20 6e6f  .- `Note` can no
-000019a0: 7720 6265 2069 6d70 6f72 7465 6420 6672  w be imported fr
-000019b0: 6f6d 2070 6163 6b61 6765 2e0d 0a2d 2060  om package...- `
-000019c0: 436f 6d6d 656e 7460 2063 616e 206e 6f77  Comment` can now
-000019d0: 2062 6520 696d 706f 7274 6564 2066 726f   be imported fro
-000019e0: 6d20 7061 636b 6167 652e 0d0a 2d20 6055  m package...- `U
-000019f0: 7365 7260 2063 616e 206e 6f77 2062 6520  ser` can now be 
-00001a00: 696d 706f 7274 6564 2066 726f 6d20 7061  imported from pa
-00001a10: 636b 6167 652e 0d0a 2d20 604d 656d 6265  ckage...- `Membe
-00001a20: 7260 2063 616e 206e 6f77 2062 6520 696d  r` can now be im
-00001a30: 706f 7274 6564 2066 726f 6d20 7061 636b  ported from pack
-00001a40: 6167 652e 0d0a 2d20 5064 6f63 2063 6f6d  age...- Pdoc com
-00001a50: 6d61 6e64 2069 6e20 6052 4541 444d 452e  mand in `README.
-00001a60: 6d64 602e 0d0a 2d20 6052 656c 6174 696f  md`...- `Relatio
-00001a70: 6e2e 746f 5f64 6963 7428 2960 206d 6574  n.to_dict()` met
-00001a80: 686f 6420 6e6f 7720 7265 6375 7273 6976  hod now recursiv
-00001a90: 656c 7920 7365 7269 616c 6973 6573 206d  ely serialises m
-00001aa0: 656d 6265 7273 2e0d 0a2d 2060 5761 792e  embers...- `Way.
-00001ab0: 746f 5f64 6963 7428 2960 206d 6574 686f  to_dict()` metho
-00001ac0: 6420 6e6f 7720 7265 6375 7273 6976 656c  d now recursivel
-00001ad0: 7920 7365 7269 616c 6973 6573 206e 6f64  y serialises nod
-00001ae0: 6573 2e0d 0a0d 0a23 2323 2043 6861 6e67  es.....### Chang
-00001af0: 6564 0d0a 2d20 4368 616e 6765 6420 696d  ed..- Changed im
-00001b00: 706f 7274 7320 696e 2060 5265 6c61 7469  ports in `Relati
-00001b10: 6f6e 2e70 7960 2074 6f20 7573 6520 696d  on.py` to use im
-00001b20: 706f 7274 696e 6720 7468 726f 7567 6820  porting through 
-00001b30: 6120 6d6f 6475 6c65 2072 6174 6865 7220  a module rather 
-00001b40: 7468 616e 2064 6972 6563 746c 7920 6672  than directly fr
-00001b50: 6f6d 2061 2066 696c 652e 0d0a 2d20 4164  om a file...- Ad
-00001b60: 6465 6420 6073 616d 706c 655f 6461 7461  ded `sample_data
-00001b70: 636c 6173 7365 732e 7079 6020 6669 6c65  classes.py` file
-00001b80: 2069 6e20 7465 7374 7320 6669 7874 7572   in tests fixtur
-00001b90: 6573 2074 6f20 7265 6475 6365 2063 6f64  es to reduce cod
-00001ba0: 6520 6475 706c 6963 6174 696f 6e2e 0d0a  e duplication...
-00001bb0: 2d20 4368 616e 6765 6420 6675 6e63 7469  - Changed functi
-00001bc0: 6f6e 206e 616d 6520 616e 6420 6465 6c65  on name and dele
-00001bd0: 7465 6420 756e 6e65 6365 7373 6172 7920  ted unnecessary 
-00001be0: 6172 6775 6d65 6e74 2069 6e20 6061 7070  argument in `app
-00001bf0: 656e 645f 656c 656d 656e 7473 5f74 6f5f  end_elements_to_
-00001c00: 6d61 7374 6572 5f65 6c65 6d65 6e74 2829  master_element()
-00001c10: 6020 6e65 7374 6564 2069 6e73 6964 6520  ` nested inside 
-00001c20: 7072 6976 6174 6520 6d65 7468 6f64 2060  private method `
-00001c30: 5f74 6f5f 786d 6c28 2960 2069 6e20 604f  _to_xml()` in `O
-00001c40: 736d 4368 616e 6765 602e 0d0a 0d0a 2323  smChange`.....##
-00001c50: 205b 302e 332e 305d 202d 2032 3032 332d   [0.3.0] - 2023-
-00001c60: 3033 2d31 340d 0a0d 0a23 2323 2041 6464  03-14....### Add
-00001c70: 6564 0d0a 2d20 6074 6f5f 6469 6374 2829  ed..- `to_dict()
-00001c80: 6020 6d65 7468 6f64 2061 6e64 2060 6672  ` method and `fr
-00001c90: 6f6d 5f64 6963 7428 2960 2063 6c61 7373  om_dict()` class
-00001ca0: 206d 6574 686f 6420 746f 2043 6861 6e67   method to Chang
-00001cb0: 6573 6574 2e20 5b23 375d 2868 7474 7073  eset. [#7](https
-00001cc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-00001cd0: 6365 6e74 5954 2f6f 736d 5f65 6173 795f  centYT/osm_easy_
-00001ce0: 6170 692f 6973 7375 6573 2f37 290d 0a2d  api/issues/7)..-
-00001cf0: 2041 6269 6c69 7479 2074 6f20 7365 7420   Ability to set 
-00001d00: 7573 6572 5f61 6765 6e74 2069 6e20 6044  user_agent in `D
-00001d10: 6966 6660 2061 6e64 2060 4170 6960 2063  iff` and `Api` c
-00001d20: 6c61 7373 2e20 5b23 355d 2868 7474 7073  lass. [#5](https
-00001d30: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-00001d40: 6365 6e74 5954 2f6f 736d 5f65 6173 795f  centYT/osm_easy_
-00001d50: 6170 692f 6973 7375 6573 2f35 290d 0a2d  api/issues/5)..-
-00001d60: 2060 6f73 6d5f 6f62 6a65 6374 5f70 7269   `osm_object_pri
-00001d70: 6d69 7469 7665 6020 6066 726f 6d5f 6469  mitive` `from_di
-00001d80: 6374 2829 6020 636c 6173 7320 6d65 7468  ct()` class meth
-00001d90: 6f64 206e 6f77 2072 6169 7365 7320 6056  od now raises `V
-00001da0: 616c 7565 4572 726f 7260 2069 6620 7468  alueError` if th
-00001db0: 6520 6074 7970 6560 206b 6579 2069 7320  e `type` key is 
-00001dc0: 6e6f 7420 666f 756e 642e 0d0a 0d0a 2323  not found.....##
-00001dd0: 2320 4368 616e 6765 640d 0a2d 2060 4368  # Changed..- `Ch
-00001de0: 616e 6765 7365 7460 2069 7320 6e6f 7720  angeset` is now 
-00001df0: 6578 706f 7274 6564 2066 726f 6d20 6461  exported from da
-00001e00: 7461 5f63 6c61 7373 6573 206d 6f64 756c  ta_classes modul
-00001e10: 652e 0d0a 2d20 4d6f 7265 2074 6573 7473  e...- More tests
-00001e20: 2e0d 0a0d 0a23 2320 5b30 2e32 2e30 5d20  .....## [0.2.0] 
-00001e30: 2d20 3230 3233 2d30 332d 3037 0d0a 0d0a  - 2023-03-07....
-00001e40: 2323 2320 4164 6465 640d 0a2d 2060 746f  ### Added..- `to
-00001e50: 5f64 6963 7428 2960 206d 6574 686f 6420  _dict()` method 
-00001e60: 616e 6420 6066 726f 6d5f 6469 6374 2829  and `from_dict()
-00001e70: 6020 636c 6173 7320 6d65 7468 6f64 2074  ` class method t
-00001e80: 6f20 606f 736d 5f6f 626a 6563 745f 7072  o `osm_object_pr
-00001e90: 696d 6974 6976 6560 2e20 2841 6e20 6f62  imitive`. (An ob
-00001ea0: 6a65 6374 2074 6861 7420 6973 2069 6e68  ject that is inh
-00001eb0: 6572 6974 6564 2062 7920 6120 604e 6f64  erited by a `Nod
-00001ec0: 6560 2c20 6057 6179 602c 2060 5265 6c61  e`, `Way`, `Rela
-00001ed0: 7469 6f6e 6029 2e20 5b23 335d 2868 7474  tion`). [#3](htt
-00001ee0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001ef0: 646f 6365 6e74 5954 2f6f 736d 5f65 6173  docentYT/osm_eas
-00001f00: 795f 6170 692f 6973 7375 6573 2f33 290d  y_api/issues/3).
-00001f10: 0a2d 2053 7570 706f 7274 2066 6f72 2068  .- Support for h
-00001f20: 6973 746f 7269 6361 6c20 616e 6f6e 796d  istorical anonym
-00001f30: 6f75 7320 6564 6974 7320 616e 6420 6564  ous edits and ed
-00001f40: 6974 7320 6d61 6465 2062 7920 6465 6c65  its made by dele
-00001f50: 7465 6420 6163 636f 756e 7473 2e20 5b23  ted accounts. [#
-00001f60: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
-00001f70: 622e 636f 6d2f 646f 6365 6e74 5954 2f6f  b.com/docentYT/o
-00001f80: 736d 5f65 6173 795f 6170 692f 6973 7375  sm_easy_api/issu
-00001f90: 6573 2f34 290d 0a0d 0a23 2320 5b30 2e31  es/4)....## [0.1
-00001fa0: 2e34 5d20 2d20 3230 3233 2d30 332d 3035  .4] - 2023-03-05
-00001fb0: 0d0a 0d0a 2323 2320 4669 7865 640d 0a2d  ....### Fixed..-
-00001fc0: 2049 6d70 726f 7665 6d65 6e74 206f 6620   Improvement of 
-00001fd0: 7574 696c 732e 6a6f 696e 5f75 726c 2829  utils.join_url()
-00001fe0: 2066 756e 6374 696f 6e2e 0d0a 2d20 5370   function...- Sp
-00001ff0: 656c 6c69 6e67 2065 7272 6f72 7320 636f  elling errors co
-00002000: 7272 6563 7465 6420 5b40 6d61 746b 6f6e  rrected [@matkon
-00002010: 6965 637a 5d28 6874 7470 733a 2f2f 6769  iecz](https://gi
-00002020: 7468 7562 2e63 6f6d 2f6d 6174 6b6f 6e69  thub.com/matkoni
-00002030: 6563 7a29 0d0a 0d0a 2323 205b 302e 312e  ecz)....## [0.1.
-00002040: 335d 202d 2032 3032 332d 3033 2d30 330d  3] - 2023-03-03.
-00002050: 0a0d 0a23 2323 2046 6978 6564 0d0a 0d0a  ...### Fixed....
-00002060: 2d20 4669 7865 6420 7468 6520 6e6f 6e2d  - Fixed the non-
-00002070: 7365 7474 696e 6720 6f66 2074 6865 2022  setting of the "
-00002080: 7669 7369 626c 6522 2061 7474 7269 6275  visible" attribu
-00002090: 7465 2e0d 0a0d 0a23 2320 5b30 2e31 2e32  te.....## [0.1.2
-000020a0: 5d20 2d20 3230 3233 2d30 332d 3033 0d0a  ] - 2023-03-03..
-000020b0: 0d0a 2323 2320 4669 7865 640d 0a0d 0a2d  ..### Fixed....-
-000020c0: 2046 6978 6564 2072 6574 7572 6e20 7479   Fixed return ty
-000020d0: 7065 206f 6620 6765 6e65 7261 746f 7220  pe of generator 
-000020e0: 696e 2044 6966 662e 6765 7428 2920 6d65  in Diff.get() me
-000020f0: 7468 6f64 2e0d 0a0d 0a23 2320 5b30 2e31  thod.....## [0.1
-00002100: 2e31 5d20 2d20 3230 3233 2d30 332d 3033  .1] - 2023-03-03
-00002110: 0d0a 0d0a 2323 2320 4164 6465 640d 0a0d  ....### Added...
-00002120: 0a2d 204c 6963 656e 7365 0d0a 0d0a 2323  .- License....##
-00002130: 205b 302e 312e 305d 202d 2032 3032 332d   [0.1.0] - 2023-
-00002140: 3033 2d30 330d 0a0d 0a23 2323 2041 6464  03-03....### Add
-00002150: 6564 0d0a 0d0a 2d20 496e 6974 6961 6c20  ed....- Initial 
-00002160: 696d 706f 7274 0d0a 2020 2020 2020 2020  import..        
-00002170: 2020 2020 2020 2020 2020 2020 474e 5520              GNU 
-00002180: 4745 4e45 5241 4c20 5055 424c 4943 204c  GENERAL PUBLIC L
-00002190: 4943 454e 5345 0d0a 2020 2020 2020 2020  ICENSE..        
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2056                 V
-000021b0: 6572 7369 6f6e 2033 2c20 3239 204a 756e  ersion 3, 29 Jun
-000021c0: 6520 3230 3037 0d0a 0d0a 2043 6f70 7972  e 2007.... Copyr
-000021d0: 6967 6874 2028 4329 2032 3030 3720 4672  ight (C) 2007 Fr
-000021e0: 6565 2053 6f66 7477 6172 6520 466f 756e  ee Software Foun
-000021f0: 6461 7469 6f6e 2c20 496e 632e 203c 6874  dation, Inc. <ht
-00002200: 7470 733a 2f2f 6673 662e 6f72 672f 3e0d  tps://fsf.org/>.
-00002210: 0a20 4576 6572 796f 6e65 2069 7320 7065  . Everyone is pe
-00002220: 726d 6974 7465 6420 746f 2063 6f70 7920  rmitted to copy 
-00002230: 616e 6420 6469 7374 7269 6275 7465 2076  and distribute v
-00002240: 6572 6261 7469 6d20 636f 7069 6573 0d0a  erbatim copies..
-00002250: 206f 6620 7468 6973 206c 6963 656e 7365   of this license
-00002260: 2064 6f63 756d 656e 742c 2062 7574 2063   document, but c
-00002270: 6861 6e67 696e 6720 6974 2069 7320 6e6f  hanging it is no
-00002280: 7420 616c 6c6f 7765 642e 0d0a 0d0a 2020  t allowed.....  
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2020 2020 2020 5072 6561 6d62            Preamb
-000022b0: 6c65 0d0a 0d0a 2020 5468 6520 474e 5520  le....  The GNU 
-000022c0: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-000022d0: 6963 656e 7365 2069 7320 6120 6672 6565  icense is a free
-000022e0: 2c20 636f 7079 6c65 6674 206c 6963 656e  , copyleft licen
-000022f0: 7365 2066 6f72 0d0a 736f 6674 7761 7265  se for..software
-00002300: 2061 6e64 206f 7468 6572 206b 696e 6473   and other kinds
-00002310: 206f 6620 776f 726b 732e 0d0a 0d0a 2020   of works.....  
-00002320: 5468 6520 6c69 6365 6e73 6573 2066 6f72  The licenses for
-00002330: 206d 6f73 7420 736f 6674 7761 7265 2061   most software a
-00002340: 6e64 206f 7468 6572 2070 7261 6374 6963  nd other practic
-00002350: 616c 2077 6f72 6b73 2061 7265 2064 6573  al works are des
-00002360: 6967 6e65 640d 0a74 6f20 7461 6b65 2061  igned..to take a
-00002370: 7761 7920 796f 7572 2066 7265 6564 6f6d  way your freedom
-00002380: 2074 6f20 7368 6172 6520 616e 6420 6368   to share and ch
-00002390: 616e 6765 2074 6865 2077 6f72 6b73 2e20  ange the works. 
-000023a0: 2042 7920 636f 6e74 7261 7374 2c0d 0a74   By contrast,..t
-000023b0: 6865 2047 4e55 2047 656e 6572 616c 2050  he GNU General P
-000023c0: 7562 6c69 6320 4c69 6365 6e73 6520 6973  ublic License is
-000023d0: 2069 6e74 656e 6465 6420 746f 2067 7561   intended to gua
-000023e0: 7261 6e74 6565 2079 6f75 7220 6672 6565  rantee your free
-000023f0: 646f 6d20 746f 0d0a 7368 6172 6520 616e  dom to..share an
-00002400: 6420 6368 616e 6765 2061 6c6c 2076 6572  d change all ver
-00002410: 7369 6f6e 7320 6f66 2061 2070 726f 6772  sions of a progr
-00002420: 616d 2d2d 746f 206d 616b 6520 7375 7265  am--to make sure
-00002430: 2069 7420 7265 6d61 696e 7320 6672 6565   it remains free
-00002440: 0d0a 736f 6674 7761 7265 2066 6f72 2061  ..software for a
-00002450: 6c6c 2069 7473 2075 7365 7273 2e20 2057  ll its users.  W
-00002460: 652c 2074 6865 2046 7265 6520 536f 6674  e, the Free Soft
-00002470: 7761 7265 2046 6f75 6e64 6174 696f 6e2c  ware Foundation,
-00002480: 2075 7365 2074 6865 0d0a 474e 5520 4765   use the..GNU Ge
-00002490: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000024a0: 656e 7365 2066 6f72 206d 6f73 7420 6f66  ense for most of
-000024b0: 206f 7572 2073 6f66 7477 6172 653b 2069   our software; i
-000024c0: 7420 6170 706c 6965 7320 616c 736f 2074  t applies also t
-000024d0: 6f0d 0a61 6e79 206f 7468 6572 2077 6f72  o..any other wor
-000024e0: 6b20 7265 6c65 6173 6564 2074 6869 7320  k released this 
-000024f0: 7761 7920 6279 2069 7473 2061 7574 686f  way by its autho
-00002500: 7273 2e20 2059 6f75 2063 616e 2061 7070  rs.  You can app
-00002510: 6c79 2069 7420 746f 0d0a 796f 7572 2070  ly it to..your p
-00002520: 726f 6772 616d 732c 2074 6f6f 2e0d 0a0d  rograms, too....
-00002530: 0a20 2057 6865 6e20 7765 2073 7065 616b  .  When we speak
-00002540: 206f 6620 6672 6565 2073 6f66 7477 6172   of free softwar
-00002550: 652c 2077 6520 6172 6520 7265 6665 7272  e, we are referr
-00002560: 696e 6720 746f 2066 7265 6564 6f6d 2c20  ing to freedom, 
-00002570: 6e6f 740d 0a70 7269 6365 2e20 204f 7572  not..price.  Our
-00002580: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00002590: 4c69 6365 6e73 6573 2061 7265 2064 6573  Licenses are des
-000025a0: 6967 6e65 6420 746f 206d 616b 6520 7375  igned to make su
-000025b0: 7265 2074 6861 7420 796f 750d 0a68 6176  re that you..hav
-000025c0: 6520 7468 6520 6672 6565 646f 6d20 746f  e the freedom to
-000025d0: 2064 6973 7472 6962 7574 6520 636f 7069   distribute copi
-000025e0: 6573 206f 6620 6672 6565 2073 6f66 7477  es of free softw
-000025f0: 6172 6520 2861 6e64 2063 6861 7267 6520  are (and charge 
-00002600: 666f 720d 0a74 6865 6d20 6966 2079 6f75  for..them if you
-00002610: 2077 6973 6829 2c20 7468 6174 2079 6f75   wish), that you
-00002620: 2072 6563 6569 7665 2073 6f75 7263 6520   receive source 
-00002630: 636f 6465 206f 7220 6361 6e20 6765 7420  code or can get 
-00002640: 6974 2069 6620 796f 750d 0a77 616e 7420  it if you..want 
-00002650: 6974 2c20 7468 6174 2079 6f75 2063 616e  it, that you can
-00002660: 2063 6861 6e67 6520 7468 6520 736f 6674   change the soft
-00002670: 7761 7265 206f 7220 7573 6520 7069 6563  ware or use piec
-00002680: 6573 206f 6620 6974 2069 6e20 6e65 770d  es of it in new.
-00002690: 0a66 7265 6520 7072 6f67 7261 6d73 2c20  .free programs, 
-000026a0: 616e 6420 7468 6174 2079 6f75 206b 6e6f  and that you kno
-000026b0: 7720 796f 7520 6361 6e20 646f 2074 6865  w you can do the
-000026c0: 7365 2074 6869 6e67 732e 0d0a 0d0a 2020  se things.....  
-000026d0: 546f 2070 726f 7465 6374 2079 6f75 7220  To protect your 
-000026e0: 7269 6768 7473 2c20 7765 206e 6565 6420  rights, we need 
-000026f0: 746f 2070 7265 7665 6e74 206f 7468 6572  to prevent other
-00002700: 7320 6672 6f6d 2064 656e 7969 6e67 2079  s from denying y
-00002710: 6f75 0d0a 7468 6573 6520 7269 6768 7473  ou..these rights
-00002720: 206f 7220 6173 6b69 6e67 2079 6f75 2074   or asking you t
-00002730: 6f20 7375 7272 656e 6465 7220 7468 6520  o surrender the 
-00002740: 7269 6768 7473 2e20 2054 6865 7265 666f  rights.  Therefo
-00002750: 7265 2c20 796f 7520 6861 7665 0d0a 6365  re, you have..ce
-00002760: 7274 6169 6e20 7265 7370 6f6e 7369 6269  rtain responsibi
-00002770: 6c69 7469 6573 2069 6620 796f 7520 6469  lities if you di
-00002780: 7374 7269 6275 7465 2063 6f70 6965 7320  stribute copies 
-00002790: 6f66 2074 6865 2073 6f66 7477 6172 652c  of the software,
-000027a0: 206f 7220 6966 0d0a 796f 7520 6d6f 6469   or if..you modi
-000027b0: 6679 2069 743a 2072 6573 706f 6e73 6962  fy it: responsib
-000027c0: 696c 6974 6965 7320 746f 2072 6573 7065  ilities to respe
-000027d0: 6374 2074 6865 2066 7265 6564 6f6d 206f  ct the freedom o
-000027e0: 6620 6f74 6865 7273 2e0d 0a0d 0a20 2046  f others.....  F
-000027f0: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-00002800: 6f75 2064 6973 7472 6962 7574 6520 636f  ou distribute co
-00002810: 7069 6573 206f 6620 7375 6368 2061 2070  pies of such a p
-00002820: 726f 6772 616d 2c20 7768 6574 6865 720d  rogram, whether.
-00002830: 0a67 7261 7469 7320 6f72 2066 6f72 2061  .gratis or for a
-00002840: 2066 6565 2c20 796f 7520 6d75 7374 2070   fee, you must p
-00002850: 6173 7320 6f6e 2074 6f20 7468 6520 7265  ass on to the re
-00002860: 6369 7069 656e 7473 2074 6865 2073 616d  cipients the sam
-00002870: 650d 0a66 7265 6564 6f6d 7320 7468 6174  e..freedoms that
-00002880: 2079 6f75 2072 6563 6569 7665 642e 2020   you received.  
-00002890: 596f 7520 6d75 7374 206d 616b 6520 7375  You must make su
-000028a0: 7265 2074 6861 7420 7468 6579 2c20 746f  re that they, to
-000028b0: 6f2c 2072 6563 6569 7665 0d0a 6f72 2063  o, receive..or c
-000028c0: 616e 2067 6574 2074 6865 2073 6f75 7263  an get the sourc
-000028d0: 6520 636f 6465 2e20 2041 6e64 2079 6f75  e code.  And you
-000028e0: 206d 7573 7420 7368 6f77 2074 6865 6d20   must show them 
-000028f0: 7468 6573 6520 7465 726d 7320 736f 2074  these terms so t
-00002900: 6865 790d 0a6b 6e6f 7720 7468 6569 7220  hey..know their 
-00002910: 7269 6768 7473 2e0d 0a0d 0a20 2044 6576  rights.....  Dev
-00002920: 656c 6f70 6572 7320 7468 6174 2075 7365  elopers that use
-00002930: 2074 6865 2047 4e55 2047 504c 2070 726f   the GNU GPL pro
-00002940: 7465 6374 2079 6f75 7220 7269 6768 7473  tect your rights
-00002950: 2077 6974 6820 7477 6f20 7374 6570 733a   with two steps:
-00002960: 0d0a 2831 2920 6173 7365 7274 2063 6f70  ..(1) assert cop
-00002970: 7972 6967 6874 206f 6e20 7468 6520 736f  yright on the so
-00002980: 6674 7761 7265 2c20 616e 6420 2832 2920  ftware, and (2) 
-00002990: 6f66 6665 7220 796f 7520 7468 6973 204c  offer you this L
-000029a0: 6963 656e 7365 0d0a 6769 7669 6e67 2079  icense..giving y
-000029b0: 6f75 206c 6567 616c 2070 6572 6d69 7373  ou legal permiss
-000029c0: 696f 6e20 746f 2063 6f70 792c 2064 6973  ion to copy, dis
-000029d0: 7472 6962 7574 6520 616e 642f 6f72 206d  tribute and/or m
-000029e0: 6f64 6966 7920 6974 2e0d 0a0d 0a20 2046  odify it.....  F
-000029f0: 6f72 2074 6865 2064 6576 656c 6f70 6572  or the developer
-00002a00: 7327 2061 6e64 2061 7574 686f 7273 2720  s' and authors' 
-00002a10: 7072 6f74 6563 7469 6f6e 2c20 7468 6520  protection, the 
-00002a20: 4750 4c20 636c 6561 726c 7920 6578 706c  GPL clearly expl
-00002a30: 6169 6e73 0d0a 7468 6174 2074 6865 7265  ains..that there
-00002a40: 2069 7320 6e6f 2077 6172 7261 6e74 7920   is no warranty 
-00002a50: 666f 7220 7468 6973 2066 7265 6520 736f  for this free so
-00002a60: 6674 7761 7265 2e20 2046 6f72 2062 6f74  ftware.  For bot
-00002a70: 6820 7573 6572 7327 2061 6e64 0d0a 6175  h users' and..au
-00002a80: 7468 6f72 7327 2073 616b 652c 2074 6865  thors' sake, the
-00002a90: 2047 504c 2072 6571 7569 7265 7320 7468   GPL requires th
-00002aa0: 6174 206d 6f64 6966 6965 6420 7665 7273  at modified vers
-00002ab0: 696f 6e73 2062 6520 6d61 726b 6564 2061  ions be marked a
-00002ac0: 730d 0a63 6861 6e67 6564 2c20 736f 2074  s..changed, so t
-00002ad0: 6861 7420 7468 6569 7220 7072 6f62 6c65  hat their proble
-00002ae0: 6d73 2077 696c 6c20 6e6f 7420 6265 2061  ms will not be a
-00002af0: 7474 7269 6275 7465 6420 6572 726f 6e65  ttributed errone
-00002b00: 6f75 736c 7920 746f 0d0a 6175 7468 6f72  ously to..author
-00002b10: 7320 6f66 2070 7265 7669 6f75 7320 7665  s of previous ve
-00002b20: 7273 696f 6e73 2e0d 0a0d 0a20 2053 6f6d  rsions.....  Som
-00002b30: 6520 6465 7669 6365 7320 6172 6520 6465  e devices are de
-00002b40: 7369 676e 6564 2074 6f20 6465 6e79 2075  signed to deny u
-00002b50: 7365 7273 2061 6363 6573 7320 746f 2069  sers access to i
-00002b60: 6e73 7461 6c6c 206f 7220 7275 6e0d 0a6d  nstall or run..m
-00002b70: 6f64 6966 6965 6420 7665 7273 696f 6e73  odified versions
-00002b80: 206f 6620 7468 6520 736f 6674 7761 7265   of the software
-00002b90: 2069 6e73 6964 6520 7468 656d 2c20 616c   inside them, al
-00002ba0: 7468 6f75 6768 2074 6865 206d 616e 7566  though the manuf
-00002bb0: 6163 7475 7265 720d 0a63 616e 2064 6f20  acturer..can do 
-00002bc0: 736f 2e20 2054 6869 7320 6973 2066 756e  so.  This is fun
-00002bd0: 6461 6d65 6e74 616c 6c79 2069 6e63 6f6d  damentally incom
-00002be0: 7061 7469 626c 6520 7769 7468 2074 6865  patible with the
-00002bf0: 2061 696d 206f 660d 0a70 726f 7465 6374   aim of..protect
-00002c00: 696e 6720 7573 6572 7327 2066 7265 6564  ing users' freed
-00002c10: 6f6d 2074 6f20 6368 616e 6765 2074 6865  om to change the
-00002c20: 2073 6f66 7477 6172 652e 2020 5468 6520   software.  The 
-00002c30: 7379 7374 656d 6174 6963 0d0a 7061 7474  systematic..patt
-00002c40: 6572 6e20 6f66 2073 7563 6820 6162 7573  ern of such abus
-00002c50: 6520 6f63 6375 7273 2069 6e20 7468 6520  e occurs in the 
-00002c60: 6172 6561 206f 6620 7072 6f64 7563 7473  area of products
-00002c70: 2066 6f72 2069 6e64 6976 6964 7561 6c73   for individuals
-00002c80: 2074 6f0d 0a75 7365 2c20 7768 6963 6820   to..use, which 
-00002c90: 6973 2070 7265 6369 7365 6c79 2077 6865  is precisely whe
-00002ca0: 7265 2069 7420 6973 206d 6f73 7420 756e  re it is most un
-00002cb0: 6163 6365 7074 6162 6c65 2e20 2054 6865  acceptable.  The
-00002cc0: 7265 666f 7265 2c20 7765 0d0a 6861 7665  refore, we..have
-00002cd0: 2064 6573 6967 6e65 6420 7468 6973 2076   designed this v
-00002ce0: 6572 7369 6f6e 206f 6620 7468 6520 4750  ersion of the GP
-00002cf0: 4c20 746f 2070 726f 6869 6269 7420 7468  L to prohibit th
-00002d00: 6520 7072 6163 7469 6365 2066 6f72 2074  e practice for t
-00002d10: 686f 7365 0d0a 7072 6f64 7563 7473 2e20  hose..products. 
-00002d20: 2049 6620 7375 6368 2070 726f 626c 656d   If such problem
-00002d30: 7320 6172 6973 6520 7375 6273 7461 6e74  s arise substant
-00002d40: 6961 6c6c 7920 696e 206f 7468 6572 2064  ially in other d
-00002d50: 6f6d 6169 6e73 2c20 7765 0d0a 7374 616e  omains, we..stan
-00002d60: 6420 7265 6164 7920 746f 2065 7874 656e  d ready to exten
-00002d70: 6420 7468 6973 2070 726f 7669 7369 6f6e  d this provision
-00002d80: 2074 6f20 7468 6f73 6520 646f 6d61 696e   to those domain
-00002d90: 7320 696e 2066 7574 7572 6520 7665 7273  s in future vers
-00002da0: 696f 6e73 0d0a 6f66 2074 6865 2047 504c  ions..of the GPL
-00002db0: 2c20 6173 206e 6565 6465 6420 746f 2070  , as needed to p
-00002dc0: 726f 7465 6374 2074 6865 2066 7265 6564  rotect the freed
-00002dd0: 6f6d 206f 6620 7573 6572 732e 0d0a 0d0a  om of users.....
-00002de0: 2020 4669 6e61 6c6c 792c 2065 7665 7279    Finally, every
-00002df0: 2070 726f 6772 616d 2069 7320 7468 7265   program is thre
-00002e00: 6174 656e 6564 2063 6f6e 7374 616e 746c  atened constantl
-00002e10: 7920 6279 2073 6f66 7477 6172 6520 7061  y by software pa
-00002e20: 7465 6e74 732e 0d0a 5374 6174 6573 2073  tents...States s
-00002e30: 686f 756c 6420 6e6f 7420 616c 6c6f 7720  hould not allow 
-00002e40: 7061 7465 6e74 7320 746f 2072 6573 7472  patents to restr
-00002e50: 6963 7420 6465 7665 6c6f 706d 656e 7420  ict development 
-00002e60: 616e 6420 7573 6520 6f66 0d0a 736f 6674  and use of..soft
-00002e70: 7761 7265 206f 6e20 6765 6e65 7261 6c2d  ware on general-
-00002e80: 7075 7270 6f73 6520 636f 6d70 7574 6572  purpose computer
-00002e90: 732c 2062 7574 2069 6e20 7468 6f73 6520  s, but in those 
-00002ea0: 7468 6174 2064 6f2c 2077 6520 7769 7368  that do, we wish
-00002eb0: 2074 6f0d 0a61 766f 6964 2074 6865 2073   to..avoid the s
-00002ec0: 7065 6369 616c 2064 616e 6765 7220 7468  pecial danger th
-00002ed0: 6174 2070 6174 656e 7473 2061 7070 6c69  at patents appli
-00002ee0: 6564 2074 6f20 6120 6672 6565 2070 726f  ed to a free pro
-00002ef0: 6772 616d 2063 6f75 6c64 0d0a 6d61 6b65  gram could..make
-00002f00: 2069 7420 6566 6665 6374 6976 656c 7920   it effectively 
-00002f10: 7072 6f70 7269 6574 6172 792e 2020 546f  proprietary.  To
-00002f20: 2070 7265 7665 6e74 2074 6869 732c 2074   prevent this, t
-00002f30: 6865 2047 504c 2061 7373 7572 6573 2074  he GPL assures t
-00002f40: 6861 740d 0a70 6174 656e 7473 2063 616e  hat..patents can
-00002f50: 6e6f 7420 6265 2075 7365 6420 746f 2072  not be used to r
-00002f60: 656e 6465 7220 7468 6520 7072 6f67 7261  ender the progra
-00002f70: 6d20 6e6f 6e2d 6672 6565 2e0d 0a0d 0a20  m non-free..... 
-00002f80: 2054 6865 2070 7265 6369 7365 2074 6572   The precise ter
-00002f90: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
-00002fa0: 7320 666f 7220 636f 7079 696e 672c 2064  s for copying, d
-00002fb0: 6973 7472 6962 7574 696f 6e20 616e 640d  istribution and.
-00002fc0: 0a6d 6f64 6966 6963 6174 696f 6e20 666f  .modification fo
-00002fd0: 6c6c 6f77 2e0d 0a0d 0a20 2020 2020 2020  llow.....       
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 5445 524d 5320 414e 4420 434f 4e44 4954  TERMS AND CONDIT
-00003000: 494f 4e53 0d0a 0d0a 2020 302e 2044 6566  IONS....  0. Def
-00003010: 696e 6974 696f 6e73 2e0d 0a0d 0a20 2022  initions.....  "
-00003020: 5468 6973 204c 6963 656e 7365 2220 7265  This License" re
-00003030: 6665 7273 2074 6f20 7665 7273 696f 6e20  fers to version 
-00003040: 3320 6f66 2074 6865 2047 4e55 2047 656e  3 of the GNU Gen
-00003050: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00003060: 6e73 652e 0d0a 0d0a 2020 2243 6f70 7972  nse.....  "Copyr
-00003070: 6967 6874 2220 616c 736f 206d 6561 6e73  ight" also means
-00003080: 2063 6f70 7972 6967 6874 2d6c 696b 6520   copyright-like 
-00003090: 6c61 7773 2074 6861 7420 6170 706c 7920  laws that apply 
-000030a0: 746f 206f 7468 6572 206b 696e 6473 206f  to other kinds o
-000030b0: 660d 0a77 6f72 6b73 2c20 7375 6368 2061  f..works, such a
-000030c0: 7320 7365 6d69 636f 6e64 7563 746f 7220  s semiconductor 
-000030d0: 6d61 736b 732e 0d0a 0d0a 2020 2254 6865  masks.....  "The
-000030e0: 2050 726f 6772 616d 2220 7265 6665 7273   Program" refers
-000030f0: 2074 6f20 616e 7920 636f 7079 7269 6768   to any copyrigh
-00003100: 7461 626c 6520 776f 726b 206c 6963 656e  table work licen
-00003110: 7365 6420 756e 6465 7220 7468 6973 0d0a  sed under this..
-00003120: 4c69 6365 6e73 652e 2020 4561 6368 206c  License.  Each l
-00003130: 6963 656e 7365 6520 6973 2061 6464 7265  icensee is addre
-00003140: 7373 6564 2061 7320 2279 6f75 222e 2020  ssed as "you".  
-00003150: 224c 6963 656e 7365 6573 2220 616e 640d  "Licensees" and.
-00003160: 0a22 7265 6369 7069 656e 7473 2220 6d61  ."recipients" ma
-00003170: 7920 6265 2069 6e64 6976 6964 7561 6c73  y be individuals
-00003180: 206f 7220 6f72 6761 6e69 7a61 7469 6f6e   or organization
-00003190: 732e 0d0a 0d0a 2020 546f 2022 6d6f 6469  s.....  To "modi
-000031a0: 6679 2220 6120 776f 726b 206d 6561 6e73  fy" a work means
-000031b0: 2074 6f20 636f 7079 2066 726f 6d20 6f72   to copy from or
-000031c0: 2061 6461 7074 2061 6c6c 206f 7220 7061   adapt all or pa
-000031d0: 7274 206f 6620 7468 6520 776f 726b 0d0a  rt of the work..
-000031e0: 696e 2061 2066 6173 6869 6f6e 2072 6571  in a fashion req
-000031f0: 7569 7269 6e67 2063 6f70 7972 6967 6874  uiring copyright
-00003200: 2070 6572 6d69 7373 696f 6e2c 206f 7468   permission, oth
-00003210: 6572 2074 6861 6e20 7468 6520 6d61 6b69  er than the maki
-00003220: 6e67 206f 6620 616e 0d0a 6578 6163 7420  ng of an..exact 
-00003230: 636f 7079 2e20 2054 6865 2072 6573 756c  copy.  The resul
-00003240: 7469 6e67 2077 6f72 6b20 6973 2063 616c  ting work is cal
-00003250: 6c65 6420 6120 226d 6f64 6966 6965 6420  led a "modified 
-00003260: 7665 7273 696f 6e22 206f 6620 7468 650d  version" of the.
-00003270: 0a65 6172 6c69 6572 2077 6f72 6b20 6f72  .earlier work or
-00003280: 2061 2077 6f72 6b20 2262 6173 6564 206f   a work "based o
-00003290: 6e22 2074 6865 2065 6172 6c69 6572 2077  n" the earlier w
-000032a0: 6f72 6b2e 0d0a 0d0a 2020 4120 2263 6f76  ork.....  A "cov
-000032b0: 6572 6564 2077 6f72 6b22 206d 6561 6e73  ered work" means
-000032c0: 2065 6974 6865 7220 7468 6520 756e 6d6f   either the unmo
-000032d0: 6469 6669 6564 2050 726f 6772 616d 206f  dified Program o
-000032e0: 7220 6120 776f 726b 2062 6173 6564 0d0a  r a work based..
-000032f0: 6f6e 2074 6865 2050 726f 6772 616d 2e0d  on the Program..
-00003300: 0a0d 0a20 2054 6f20 2270 726f 7061 6761  ...  To "propaga
-00003310: 7465 2220 6120 776f 726b 206d 6561 6e73  te" a work means
-00003320: 2074 6f20 646f 2061 6e79 7468 696e 6720   to do anything 
-00003330: 7769 7468 2069 7420 7468 6174 2c20 7769  with it that, wi
-00003340: 7468 6f75 740d 0a70 6572 6d69 7373 696f  thout..permissio
-00003350: 6e2c 2077 6f75 6c64 206d 616b 6520 796f  n, would make yo
-00003360: 7520 6469 7265 6374 6c79 206f 7220 7365  u directly or se
-00003370: 636f 6e64 6172 696c 7920 6c69 6162 6c65  condarily liable
-00003380: 2066 6f72 0d0a 696e 6672 696e 6765 6d65   for..infringeme
-00003390: 6e74 2075 6e64 6572 2061 7070 6c69 6361  nt under applica
-000033a0: 626c 6520 636f 7079 7269 6768 7420 6c61  ble copyright la
-000033b0: 772c 2065 7863 6570 7420 6578 6563 7574  w, except execut
-000033c0: 696e 6720 6974 206f 6e20 610d 0a63 6f6d  ing it on a..com
-000033d0: 7075 7465 7220 6f72 206d 6f64 6966 7969  puter or modifyi
-000033e0: 6e67 2061 2070 7269 7661 7465 2063 6f70  ng a private cop
-000033f0: 792e 2020 5072 6f70 6167 6174 696f 6e20  y.  Propagation 
-00003400: 696e 636c 7564 6573 2063 6f70 7969 6e67  includes copying
-00003410: 2c0d 0a64 6973 7472 6962 7574 696f 6e20  ,..distribution 
-00003420: 2877 6974 6820 6f72 2077 6974 686f 7574  (with or without
-00003430: 206d 6f64 6966 6963 6174 696f 6e29 2c20   modification), 
-00003440: 6d61 6b69 6e67 2061 7661 696c 6162 6c65  making available
-00003450: 2074 6f20 7468 650d 0a70 7562 6c69 632c   to the..public,
-00003460: 2061 6e64 2069 6e20 736f 6d65 2063 6f75   and in some cou
-00003470: 6e74 7269 6573 206f 7468 6572 2061 6374  ntries other act
-00003480: 6976 6974 6965 7320 6173 2077 656c 6c2e  ivities as well.
-00003490: 0d0a 0d0a 2020 546f 2022 636f 6e76 6579  ....  To "convey
-000034a0: 2220 6120 776f 726b 206d 6561 6e73 2061  " a work means a
-000034b0: 6e79 206b 696e 6420 6f66 2070 726f 7061  ny kind of propa
-000034c0: 6761 7469 6f6e 2074 6861 7420 656e 6162  gation that enab
-000034d0: 6c65 7320 6f74 6865 720d 0a70 6172 7469  les other..parti
-000034e0: 6573 2074 6f20 6d61 6b65 206f 7220 7265  es to make or re
-000034f0: 6365 6976 6520 636f 7069 6573 2e20 204d  ceive copies.  M
-00003500: 6572 6520 696e 7465 7261 6374 696f 6e20  ere interaction 
-00003510: 7769 7468 2061 2075 7365 7220 7468 726f  with a user thro
-00003520: 7567 680d 0a61 2063 6f6d 7075 7465 7220  ugh..a computer 
-00003530: 6e65 7477 6f72 6b2c 2077 6974 6820 6e6f  network, with no
-00003540: 2074 7261 6e73 6665 7220 6f66 2061 2063   transfer of a c
-00003550: 6f70 792c 2069 7320 6e6f 7420 636f 6e76  opy, is not conv
-00003560: 6579 696e 672e 0d0a 0d0a 2020 416e 2069  eying.....  An i
-00003570: 6e74 6572 6163 7469 7665 2075 7365 7220  nteractive user 
-00003580: 696e 7465 7266 6163 6520 6469 7370 6c61  interface displa
-00003590: 7973 2022 4170 7072 6f70 7269 6174 6520  ys "Appropriate 
-000035a0: 4c65 6761 6c20 4e6f 7469 6365 7322 0d0a  Legal Notices"..
-000035b0: 746f 2074 6865 2065 7874 656e 7420 7468  to the extent th
-000035c0: 6174 2069 7420 696e 636c 7564 6573 2061  at it includes a
-000035d0: 2063 6f6e 7665 6e69 656e 7420 616e 6420   convenient and 
-000035e0: 7072 6f6d 696e 656e 746c 7920 7669 7369  prominently visi
-000035f0: 626c 650d 0a66 6561 7475 7265 2074 6861  ble..feature tha
-00003600: 7420 2831 2920 6469 7370 6c61 7973 2061  t (1) displays a
-00003610: 6e20 6170 7072 6f70 7269 6174 6520 636f  n appropriate co
-00003620: 7079 7269 6768 7420 6e6f 7469 6365 2c20  pyright notice, 
-00003630: 616e 6420 2832 290d 0a74 656c 6c73 2074  and (2)..tells t
-00003640: 6865 2075 7365 7220 7468 6174 2074 6865  he user that the
-00003650: 7265 2069 7320 6e6f 2077 6172 7261 6e74  re is no warrant
-00003660: 7920 666f 7220 7468 6520 776f 726b 2028  y for the work (
-00003670: 6578 6365 7074 2074 6f20 7468 650d 0a65  except to the..e
-00003680: 7874 656e 7420 7468 6174 2077 6172 7261  xtent that warra
-00003690: 6e74 6965 7320 6172 6520 7072 6f76 6964  nties are provid
-000036a0: 6564 292c 2074 6861 7420 6c69 6365 6e73  ed), that licens
-000036b0: 6565 7320 6d61 7920 636f 6e76 6579 2074  ees may convey t
-000036c0: 6865 0d0a 776f 726b 2075 6e64 6572 2074  he..work under t
-000036d0: 6869 7320 4c69 6365 6e73 652c 2061 6e64  his License, and
-000036e0: 2068 6f77 2074 6f20 7669 6577 2061 2063   how to view a c
-000036f0: 6f70 7920 6f66 2074 6869 7320 4c69 6365  opy of this Lice
-00003700: 6e73 652e 2020 4966 0d0a 7468 6520 696e  nse.  If..the in
-00003710: 7465 7266 6163 6520 7072 6573 656e 7473  terface presents
-00003720: 2061 206c 6973 7420 6f66 2075 7365 7220   a list of user 
-00003730: 636f 6d6d 616e 6473 206f 7220 6f70 7469  commands or opti
-00003740: 6f6e 732c 2073 7563 6820 6173 2061 0d0a  ons, such as a..
-00003750: 6d65 6e75 2c20 6120 7072 6f6d 696e 656e  menu, a prominen
-00003760: 7420 6974 656d 2069 6e20 7468 6520 6c69  t item in the li
-00003770: 7374 206d 6565 7473 2074 6869 7320 6372  st meets this cr
-00003780: 6974 6572 696f 6e2e 0d0a 0d0a 2020 312e  iterion.....  1.
-00003790: 2053 6f75 7263 6520 436f 6465 2e0d 0a0d   Source Code....
-000037a0: 0a20 2054 6865 2022 736f 7572 6365 2063  .  The "source c
-000037b0: 6f64 6522 2066 6f72 2061 2077 6f72 6b20  ode" for a work 
-000037c0: 6d65 616e 7320 7468 6520 7072 6566 6572  means the prefer
-000037d0: 7265 6420 666f 726d 206f 6620 7468 6520  red form of the 
-000037e0: 776f 726b 0d0a 666f 7220 6d61 6b69 6e67  work..for making
-000037f0: 206d 6f64 6966 6963 6174 696f 6e73 2074   modifications t
-00003800: 6f20 6974 2e20 2022 4f62 6a65 6374 2063  o it.  "Object c
-00003810: 6f64 6522 206d 6561 6e73 2061 6e79 206e  ode" means any n
-00003820: 6f6e 2d73 6f75 7263 650d 0a66 6f72 6d20  on-source..form 
-00003830: 6f66 2061 2077 6f72 6b2e 0d0a 0d0a 2020  of a work.....  
-00003840: 4120 2253 7461 6e64 6172 6420 496e 7465  A "Standard Inte
-00003850: 7266 6163 6522 206d 6561 6e73 2061 6e20  rface" means an 
-00003860: 696e 7465 7266 6163 6520 7468 6174 2065  interface that e
-00003870: 6974 6865 7220 6973 2061 6e20 6f66 6669  ither is an offi
-00003880: 6369 616c 0d0a 7374 616e 6461 7264 2064  cial..standard d
-00003890: 6566 696e 6564 2062 7920 6120 7265 636f  efined by a reco
-000038a0: 676e 697a 6564 2073 7461 6e64 6172 6473  gnized standards
-000038b0: 2062 6f64 792c 206f 722c 2069 6e20 7468   body, or, in th
-000038c0: 6520 6361 7365 206f 660d 0a69 6e74 6572  e case of..inter
-000038d0: 6661 6365 7320 7370 6563 6966 6965 6420  faces specified 
-000038e0: 666f 7220 6120 7061 7274 6963 756c 6172  for a particular
-000038f0: 2070 726f 6772 616d 6d69 6e67 206c 616e   programming lan
-00003900: 6775 6167 652c 206f 6e65 2074 6861 740d  guage, one that.
-00003910: 0a69 7320 7769 6465 6c79 2075 7365 6420  .is widely used 
-00003920: 616d 6f6e 6720 6465 7665 6c6f 7065 7273  among developers
-00003930: 2077 6f72 6b69 6e67 2069 6e20 7468 6174   working in that
-00003940: 206c 616e 6775 6167 652e 0d0a 0d0a 2020   language.....  
-00003950: 5468 6520 2253 7973 7465 6d20 4c69 6272  The "System Libr
-00003960: 6172 6965 7322 206f 6620 616e 2065 7865  aries" of an exe
-00003970: 6375 7461 626c 6520 776f 726b 2069 6e63  cutable work inc
-00003980: 6c75 6465 2061 6e79 7468 696e 672c 206f  lude anything, o
-00003990: 7468 6572 0d0a 7468 616e 2074 6865 2077  ther..than the w
-000039a0: 6f72 6b20 6173 2061 2077 686f 6c65 2c20  ork as a whole, 
-000039b0: 7468 6174 2028 6129 2069 7320 696e 636c  that (a) is incl
-000039c0: 7564 6564 2069 6e20 7468 6520 6e6f 726d  uded in the norm
-000039d0: 616c 2066 6f72 6d20 6f66 0d0a 7061 636b  al form of..pack
-000039e0: 6167 696e 6720 6120 4d61 6a6f 7220 436f  aging a Major Co
-000039f0: 6d70 6f6e 656e 742c 2062 7574 2077 6869  mponent, but whi
-00003a00: 6368 2069 7320 6e6f 7420 7061 7274 206f  ch is not part o
-00003a10: 6620 7468 6174 204d 616a 6f72 0d0a 436f  f that Major..Co
-00003a20: 6d70 6f6e 656e 742c 2061 6e64 2028 6229  mponent, and (b)
-00003a30: 2073 6572 7665 7320 6f6e 6c79 2074 6f20   serves only to 
-00003a40: 656e 6162 6c65 2075 7365 206f 6620 7468  enable use of th
-00003a50: 6520 776f 726b 2077 6974 6820 7468 6174  e work with that
-00003a60: 0d0a 4d61 6a6f 7220 436f 6d70 6f6e 656e  ..Major Componen
-00003a70: 742c 206f 7220 746f 2069 6d70 6c65 6d65  t, or to impleme
-00003a80: 6e74 2061 2053 7461 6e64 6172 6420 496e  nt a Standard In
-00003a90: 7465 7266 6163 6520 666f 7220 7768 6963  terface for whic
-00003aa0: 6820 616e 0d0a 696d 706c 656d 656e 7461  h an..implementa
-00003ab0: 7469 6f6e 2069 7320 6176 6169 6c61 626c  tion is availabl
-00003ac0: 6520 746f 2074 6865 2070 7562 6c69 6320  e to the public 
-00003ad0: 696e 2073 6f75 7263 6520 636f 6465 2066  in source code f
-00003ae0: 6f72 6d2e 2020 410d 0a22 4d61 6a6f 7220  orm.  A.."Major 
-00003af0: 436f 6d70 6f6e 656e 7422 2c20 696e 2074  Component", in t
-00003b00: 6869 7320 636f 6e74 6578 742c 206d 6561  his context, mea
-00003b10: 6e73 2061 206d 616a 6f72 2065 7373 656e  ns a major essen
-00003b20: 7469 616c 2063 6f6d 706f 6e65 6e74 0d0a  tial component..
-00003b30: 286b 6572 6e65 6c2c 2077 696e 646f 7720  (kernel, window 
-00003b40: 7379 7374 656d 2c20 616e 6420 736f 206f  system, and so o
-00003b50: 6e29 206f 6620 7468 6520 7370 6563 6966  n) of the specif
-00003b60: 6963 206f 7065 7261 7469 6e67 2073 7973  ic operating sys
-00003b70: 7465 6d0d 0a28 6966 2061 6e79 2920 6f6e  tem..(if any) on
-00003b80: 2077 6869 6368 2074 6865 2065 7865 6375   which the execu
-00003b90: 7461 626c 6520 776f 726b 2072 756e 732c  table work runs,
-00003ba0: 206f 7220 6120 636f 6d70 696c 6572 2075   or a compiler u
-00003bb0: 7365 6420 746f 0d0a 7072 6f64 7563 6520  sed to..produce 
-00003bc0: 7468 6520 776f 726b 2c20 6f72 2061 6e20  the work, or an 
-00003bd0: 6f62 6a65 6374 2063 6f64 6520 696e 7465  object code inte
-00003be0: 7270 7265 7465 7220 7573 6564 2074 6f20  rpreter used to 
-00003bf0: 7275 6e20 6974 2e0d 0a0d 0a20 2054 6865  run it.....  The
-00003c00: 2022 436f 7272 6573 706f 6e64 696e 6720   "Corresponding 
-00003c10: 536f 7572 6365 2220 666f 7220 6120 776f  Source" for a wo
-00003c20: 726b 2069 6e20 6f62 6a65 6374 2063 6f64  rk in object cod
-00003c30: 6520 666f 726d 206d 6561 6e73 2061 6c6c  e form means all
-00003c40: 0d0a 7468 6520 736f 7572 6365 2063 6f64  ..the source cod
-00003c50: 6520 6e65 6564 6564 2074 6f20 6765 6e65  e needed to gene
-00003c60: 7261 7465 2c20 696e 7374 616c 6c2c 2061  rate, install, a
-00003c70: 6e64 2028 666f 7220 616e 2065 7865 6375  nd (for an execu
-00003c80: 7461 626c 650d 0a77 6f72 6b29 2072 756e  table..work) run
-00003c90: 2074 6865 206f 626a 6563 7420 636f 6465   the object code
-00003ca0: 2061 6e64 2074 6f20 6d6f 6469 6679 2074   and to modify t
-00003cb0: 6865 2077 6f72 6b2c 2069 6e63 6c75 6469  he work, includi
-00003cc0: 6e67 2073 6372 6970 7473 2074 6f0d 0a63  ng scripts to..c
-00003cd0: 6f6e 7472 6f6c 2074 686f 7365 2061 6374  ontrol those act
-00003ce0: 6976 6974 6965 732e 2020 486f 7765 7665  ivities.  Howeve
-00003cf0: 722c 2069 7420 646f 6573 206e 6f74 2069  r, it does not i
-00003d00: 6e63 6c75 6465 2074 6865 2077 6f72 6b27  nclude the work'
-00003d10: 730d 0a53 7973 7465 6d20 4c69 6272 6172  s..System Librar
-00003d20: 6965 732c 206f 7220 6765 6e65 7261 6c2d  ies, or general-
-00003d30: 7075 7270 6f73 6520 746f 6f6c 7320 6f72  purpose tools or
-00003d40: 2067 656e 6572 616c 6c79 2061 7661 696c   generally avail
-00003d50: 6162 6c65 2066 7265 650d 0a70 726f 6772  able free..progr
-00003d60: 616d 7320 7768 6963 6820 6172 6520 7573  ams which are us
-00003d70: 6564 2075 6e6d 6f64 6966 6965 6420 696e  ed unmodified in
-00003d80: 2070 6572 666f 726d 696e 6720 7468 6f73   performing thos
-00003d90: 6520 6163 7469 7669 7469 6573 2062 7574  e activities but
-00003da0: 0d0a 7768 6963 6820 6172 6520 6e6f 7420  ..which are not 
-00003db0: 7061 7274 206f 6620 7468 6520 776f 726b  part of the work
-00003dc0: 2e20 2046 6f72 2065 7861 6d70 6c65 2c20  .  For example, 
-00003dd0: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
-00003de0: 7572 6365 0d0a 696e 636c 7564 6573 2069  urce..includes i
-00003df0: 6e74 6572 6661 6365 2064 6566 696e 6974  nterface definit
-00003e00: 696f 6e20 6669 6c65 7320 6173 736f 6369  ion files associ
-00003e10: 6174 6564 2077 6974 6820 736f 7572 6365  ated with source
-00003e20: 2066 696c 6573 2066 6f72 0d0a 7468 6520   files for..the 
-00003e30: 776f 726b 2c20 616e 6420 7468 6520 736f  work, and the so
-00003e40: 7572 6365 2063 6f64 6520 666f 7220 7368  urce code for sh
-00003e50: 6172 6564 206c 6962 7261 7269 6573 2061  ared libraries a
-00003e60: 6e64 2064 796e 616d 6963 616c 6c79 0d0a  nd dynamically..
-00003e70: 6c69 6e6b 6564 2073 7562 7072 6f67 7261  linked subprogra
-00003e80: 6d73 2074 6861 7420 7468 6520 776f 726b  ms that the work
-00003e90: 2069 7320 7370 6563 6966 6963 616c 6c79   is specifically
-00003ea0: 2064 6573 6967 6e65 6420 746f 2072 6571   designed to req
-00003eb0: 7569 7265 2c0d 0a73 7563 6820 6173 2062  uire,..such as b
-00003ec0: 7920 696e 7469 6d61 7465 2064 6174 6120  y intimate data 
-00003ed0: 636f 6d6d 756e 6963 6174 696f 6e20 6f72  communication or
-00003ee0: 2063 6f6e 7472 6f6c 2066 6c6f 7720 6265   control flow be
-00003ef0: 7477 6565 6e20 7468 6f73 650d 0a73 7562  tween those..sub
-00003f00: 7072 6f67 7261 6d73 2061 6e64 206f 7468  programs and oth
-00003f10: 6572 2070 6172 7473 206f 6620 7468 6520  er parts of the 
-00003f20: 776f 726b 2e0d 0a0d 0a20 2054 6865 2043  work.....  The C
-00003f30: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
-00003f40: 7263 6520 6e65 6564 206e 6f74 2069 6e63  rce need not inc
-00003f50: 6c75 6465 2061 6e79 7468 696e 6720 7468  lude anything th
-00003f60: 6174 2075 7365 7273 0d0a 6361 6e20 7265  at users..can re
-00003f70: 6765 6e65 7261 7465 2061 7574 6f6d 6174  generate automat
-00003f80: 6963 616c 6c79 2066 726f 6d20 6f74 6865  ically from othe
-00003f90: 7220 7061 7274 7320 6f66 2074 6865 2043  r parts of the C
-00003fa0: 6f72 7265 7370 6f6e 6469 6e67 0d0a 536f  orresponding..So
-00003fb0: 7572 6365 2e0d 0a0d 0a20 2054 6865 2043  urce.....  The C
-00003fc0: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
-00003fd0: 7263 6520 666f 7220 6120 776f 726b 2069  rce for a work i
-00003fe0: 6e20 736f 7572 6365 2063 6f64 6520 666f  n source code fo
-00003ff0: 726d 2069 7320 7468 6174 0d0a 7361 6d65  rm is that..same
-00004000: 2077 6f72 6b2e 0d0a 0d0a 2020 322e 2042   work.....  2. B
-00004010: 6173 6963 2050 6572 6d69 7373 696f 6e73  asic Permissions
-00004020: 2e0d 0a0d 0a20 2041 6c6c 2072 6967 6874  .....  All right
-00004030: 7320 6772 616e 7465 6420 756e 6465 7220  s granted under 
-00004040: 7468 6973 204c 6963 656e 7365 2061 7265  this License are
-00004050: 2067 7261 6e74 6564 2066 6f72 2074 6865   granted for the
-00004060: 2074 6572 6d20 6f66 0d0a 636f 7079 7269   term of..copyri
-00004070: 6768 7420 6f6e 2074 6865 2050 726f 6772  ght on the Progr
-00004080: 616d 2c20 616e 6420 6172 6520 6972 7265  am, and are irre
-00004090: 766f 6361 626c 6520 7072 6f76 6964 6564  vocable provided
-000040a0: 2074 6865 2073 7461 7465 640d 0a63 6f6e   the stated..con
-000040b0: 6469 7469 6f6e 7320 6172 6520 6d65 742e  ditions are met.
-000040c0: 2020 5468 6973 204c 6963 656e 7365 2065    This License e
-000040d0: 7870 6c69 6369 746c 7920 6166 6669 726d  xplicitly affirm
-000040e0: 7320 796f 7572 2075 6e6c 696d 6974 6564  s your unlimited
-000040f0: 0d0a 7065 726d 6973 7369 6f6e 2074 6f20  ..permission to 
-00004100: 7275 6e20 7468 6520 756e 6d6f 6469 6669  run the unmodifi
-00004110: 6564 2050 726f 6772 616d 2e20 2054 6865  ed Program.  The
-00004120: 206f 7574 7075 7420 6672 6f6d 2072 756e   output from run
-00004130: 6e69 6e67 2061 0d0a 636f 7665 7265 6420  ning a..covered 
-00004140: 776f 726b 2069 7320 636f 7665 7265 6420  work is covered 
-00004150: 6279 2074 6869 7320 4c69 6365 6e73 6520  by this License 
-00004160: 6f6e 6c79 2069 6620 7468 6520 6f75 7470  only if the outp
-00004170: 7574 2c20 6769 7665 6e20 6974 730d 0a63  ut, given its..c
-00004180: 6f6e 7465 6e74 2c20 636f 6e73 7469 7475  ontent, constitu
-00004190: 7465 7320 6120 636f 7665 7265 6420 776f  tes a covered wo
-000041a0: 726b 2e20 2054 6869 7320 4c69 6365 6e73  rk.  This Licens
-000041b0: 6520 6163 6b6e 6f77 6c65 6467 6573 2079  e acknowledges y
-000041c0: 6f75 720d 0a72 6967 6874 7320 6f66 2066  our..rights of f
-000041d0: 6169 7220 7573 6520 6f72 206f 7468 6572  air use or other
-000041e0: 2065 7175 6976 616c 656e 742c 2061 7320   equivalent, as 
-000041f0: 7072 6f76 6964 6564 2062 7920 636f 7079  provided by copy
-00004200: 7269 6768 7420 6c61 772e 0d0a 0d0a 2020  right law.....  
-00004210: 596f 7520 6d61 7920 6d61 6b65 2c20 7275  You may make, ru
-00004220: 6e20 616e 6420 7072 6f70 6167 6174 6520  n and propagate 
-00004230: 636f 7665 7265 6420 776f 726b 7320 7468  covered works th
-00004240: 6174 2079 6f75 2064 6f20 6e6f 740d 0a63  at you do not..c
-00004250: 6f6e 7665 792c 2077 6974 686f 7574 2063  onvey, without c
-00004260: 6f6e 6469 7469 6f6e 7320 736f 206c 6f6e  onditions so lon
-00004270: 6720 6173 2079 6f75 7220 6c69 6365 6e73  g as your licens
-00004280: 6520 6f74 6865 7277 6973 6520 7265 6d61  e otherwise rema
-00004290: 696e 730d 0a69 6e20 666f 7263 652e 2020  ins..in force.  
-000042a0: 596f 7520 6d61 7920 636f 6e76 6579 2063  You may convey c
-000042b0: 6f76 6572 6564 2077 6f72 6b73 2074 6f20  overed works to 
-000042c0: 6f74 6865 7273 2066 6f72 2074 6865 2073  others for the s
-000042d0: 6f6c 6520 7075 7270 6f73 650d 0a6f 6620  ole purpose..of 
-000042e0: 6861 7669 6e67 2074 6865 6d20 6d61 6b65  having them make
-000042f0: 206d 6f64 6966 6963 6174 696f 6e73 2065   modifications e
-00004300: 7863 6c75 7369 7665 6c79 2066 6f72 2079  xclusively for y
-00004310: 6f75 2c20 6f72 2070 726f 7669 6465 2079  ou, or provide y
-00004320: 6f75 0d0a 7769 7468 2066 6163 696c 6974  ou..with facilit
-00004330: 6965 7320 666f 7220 7275 6e6e 696e 6720  ies for running 
-00004340: 7468 6f73 6520 776f 726b 732c 2070 726f  those works, pro
-00004350: 7669 6465 6420 7468 6174 2079 6f75 2063  vided that you c
-00004360: 6f6d 706c 7920 7769 7468 0d0a 7468 6520  omply with..the 
-00004370: 7465 726d 7320 6f66 2074 6869 7320 4c69  terms of this Li
-00004380: 6365 6e73 6520 696e 2063 6f6e 7665 7969  cense in conveyi
-00004390: 6e67 2061 6c6c 206d 6174 6572 6961 6c20  ng all material 
-000043a0: 666f 7220 7768 6963 6820 796f 7520 646f  for which you do
-000043b0: 0d0a 6e6f 7420 636f 6e74 726f 6c20 636f  ..not control co
-000043c0: 7079 7269 6768 742e 2020 5468 6f73 6520  pyright.  Those 
-000043d0: 7468 7573 206d 616b 696e 6720 6f72 2072  thus making or r
-000043e0: 756e 6e69 6e67 2074 6865 2063 6f76 6572  unning the cover
-000043f0: 6564 2077 6f72 6b73 0d0a 666f 7220 796f  ed works..for yo
-00004400: 7520 6d75 7374 2064 6f20 736f 2065 7863  u must do so exc
-00004410: 6c75 7369 7665 6c79 206f 6e20 796f 7572  lusively on your
-00004420: 2062 6568 616c 662c 2075 6e64 6572 2079   behalf, under y
-00004430: 6f75 7220 6469 7265 6374 696f 6e0d 0a61  our direction..a
-00004440: 6e64 2063 6f6e 7472 6f6c 2c20 6f6e 2074  nd control, on t
-00004450: 6572 6d73 2074 6861 7420 7072 6f68 6962  erms that prohib
-00004460: 6974 2074 6865 6d20 6672 6f6d 206d 616b  it them from mak
-00004470: 696e 6720 616e 7920 636f 7069 6573 206f  ing any copies o
-00004480: 660d 0a79 6f75 7220 636f 7079 7269 6768  f..your copyrigh
-00004490: 7465 6420 6d61 7465 7269 616c 206f 7574  ted material out
-000044a0: 7369 6465 2074 6865 6972 2072 656c 6174  side their relat
-000044b0: 696f 6e73 6869 7020 7769 7468 2079 6f75  ionship with you
-000044c0: 2e0d 0a0d 0a20 2043 6f6e 7665 7969 6e67  .....  Conveying
-000044d0: 2075 6e64 6572 2061 6e79 206f 7468 6572   under any other
-000044e0: 2063 6972 6375 6d73 7461 6e63 6573 2069   circumstances i
-000044f0: 7320 7065 726d 6974 7465 6420 736f 6c65  s permitted sole
-00004500: 6c79 2075 6e64 6572 0d0a 7468 6520 636f  ly under..the co
-00004510: 6e64 6974 696f 6e73 2073 7461 7465 6420  nditions stated 
-00004520: 6265 6c6f 772e 2020 5375 626c 6963 656e  below.  Sublicen
-00004530: 7369 6e67 2069 7320 6e6f 7420 616c 6c6f  sing is not allo
-00004540: 7765 643b 2073 6563 7469 6f6e 2031 300d  wed; section 10.
-00004550: 0a6d 616b 6573 2069 7420 756e 6e65 6365  .makes it unnece
-00004560: 7373 6172 792e 0d0a 0d0a 2020 332e 2050  ssary.....  3. P
-00004570: 726f 7465 6374 696e 6720 5573 6572 7327  rotecting Users'
-00004580: 204c 6567 616c 2052 6967 6874 7320 4672   Legal Rights Fr
-00004590: 6f6d 2041 6e74 692d 4369 7263 756d 7665  om Anti-Circumve
-000045a0: 6e74 696f 6e20 4c61 772e 0d0a 0d0a 2020  ntion Law.....  
-000045b0: 4e6f 2063 6f76 6572 6564 2077 6f72 6b20  No covered work 
-000045c0: 7368 616c 6c20 6265 2064 6565 6d65 6420  shall be deemed 
-000045d0: 7061 7274 206f 6620 616e 2065 6666 6563  part of an effec
-000045e0: 7469 7665 2074 6563 686e 6f6c 6f67 6963  tive technologic
-000045f0: 616c 0d0a 6d65 6173 7572 6520 756e 6465  al..measure unde
-00004600: 7220 616e 7920 6170 706c 6963 6162 6c65  r any applicable
-00004610: 206c 6177 2066 756c 6669 6c6c 696e 6720   law fulfilling 
-00004620: 6f62 6c69 6761 7469 6f6e 7320 756e 6465  obligations unde
-00004630: 7220 6172 7469 636c 650d 0a31 3120 6f66  r article..11 of
-00004640: 2074 6865 2057 4950 4f20 636f 7079 7269   the WIPO copyri
-00004650: 6768 7420 7472 6561 7479 2061 646f 7074  ght treaty adopt
-00004660: 6564 206f 6e20 3230 2044 6563 656d 6265  ed on 20 Decembe
-00004670: 7220 3139 3936 2c20 6f72 0d0a 7369 6d69  r 1996, or..simi
-00004680: 6c61 7220 6c61 7773 2070 726f 6869 6269  lar laws prohibi
-00004690: 7469 6e67 206f 7220 7265 7374 7269 6374  ting or restrict
-000046a0: 696e 6720 6369 7263 756d 7665 6e74 696f  ing circumventio
-000046b0: 6e20 6f66 2073 7563 680d 0a6d 6561 7375  n of such..measu
-000046c0: 7265 732e 0d0a 0d0a 2020 5768 656e 2079  res.....  When y
-000046d0: 6f75 2063 6f6e 7665 7920 6120 636f 7665  ou convey a cove
-000046e0: 7265 6420 776f 726b 2c20 796f 7520 7761  red work, you wa
-000046f0: 6976 6520 616e 7920 6c65 6761 6c20 706f  ive any legal po
-00004700: 7765 7220 746f 2066 6f72 6269 640d 0a63  wer to forbid..c
-00004710: 6972 6375 6d76 656e 7469 6f6e 206f 6620  ircumvention of 
-00004720: 7465 6368 6e6f 6c6f 6769 6361 6c20 6d65  technological me
-00004730: 6173 7572 6573 2074 6f20 7468 6520 6578  asures to the ex
-00004740: 7465 6e74 2073 7563 6820 6369 7263 756d  tent such circum
-00004750: 7665 6e74 696f 6e0d 0a69 7320 6566 6665  vention..is effe
-00004760: 6374 6564 2062 7920 6578 6572 6369 7369  cted by exercisi
-00004770: 6e67 2072 6967 6874 7320 756e 6465 7220  ng rights under 
-00004780: 7468 6973 204c 6963 656e 7365 2077 6974  this License wit
-00004790: 6820 7265 7370 6563 7420 746f 0d0a 7468  h respect to..th
-000047a0: 6520 636f 7665 7265 6420 776f 726b 2c20  e covered work, 
-000047b0: 616e 6420 796f 7520 6469 7363 6c61 696d  and you disclaim
-000047c0: 2061 6e79 2069 6e74 656e 7469 6f6e 2074   any intention t
-000047d0: 6f20 6c69 6d69 7420 6f70 6572 6174 696f  o limit operatio
-000047e0: 6e20 6f72 0d0a 6d6f 6469 6669 6361 7469  n or..modificati
-000047f0: 6f6e 206f 6620 7468 6520 776f 726b 2061  on of the work a
-00004800: 7320 6120 6d65 616e 7320 6f66 2065 6e66  s a means of enf
-00004810: 6f72 6369 6e67 2c20 6167 6169 6e73 7420  orcing, against 
-00004820: 7468 6520 776f 726b 2773 0d0a 7573 6572  the work's..user
-00004830: 732c 2079 6f75 7220 6f72 2074 6869 7264  s, your or third
-00004840: 2070 6172 7469 6573 2720 6c65 6761 6c20   parties' legal 
-00004850: 7269 6768 7473 2074 6f20 666f 7262 6964  rights to forbid
-00004860: 2063 6972 6375 6d76 656e 7469 6f6e 206f   circumvention o
-00004870: 660d 0a74 6563 686e 6f6c 6f67 6963 616c  f..technological
-00004880: 206d 6561 7375 7265 732e 0d0a 0d0a 2020   measures.....  
-00004890: 342e 2043 6f6e 7665 7969 6e67 2056 6572  4. Conveying Ver
-000048a0: 6261 7469 6d20 436f 7069 6573 2e0d 0a0d  batim Copies....
-000048b0: 0a20 2059 6f75 206d 6179 2063 6f6e 7665  .  You may conve
-000048c0: 7920 7665 7262 6174 696d 2063 6f70 6965  y verbatim copie
-000048d0: 7320 6f66 2074 6865 2050 726f 6772 616d  s of the Program
-000048e0: 2773 2073 6f75 7263 6520 636f 6465 2061  's source code a
-000048f0: 7320 796f 750d 0a72 6563 6569 7665 2069  s you..receive i
-00004900: 742c 2069 6e20 616e 7920 6d65 6469 756d  t, in any medium
-00004910: 2c20 7072 6f76 6964 6564 2074 6861 7420  , provided that 
-00004920: 796f 7520 636f 6e73 7069 6375 6f75 736c  you conspicuousl
-00004930: 7920 616e 640d 0a61 7070 726f 7072 6961  y and..appropria
-00004940: 7465 6c79 2070 7562 6c69 7368 206f 6e20  tely publish on 
-00004950: 6561 6368 2063 6f70 7920 616e 2061 7070  each copy an app
-00004960: 726f 7072 6961 7465 2063 6f70 7972 6967  ropriate copyrig
-00004970: 6874 206e 6f74 6963 653b 0d0a 6b65 6570  ht notice;..keep
-00004980: 2069 6e74 6163 7420 616c 6c20 6e6f 7469   intact all noti
-00004990: 6365 7320 7374 6174 696e 6720 7468 6174  ces stating that
-000049a0: 2074 6869 7320 4c69 6365 6e73 6520 616e   this License an
-000049b0: 6420 616e 790d 0a6e 6f6e 2d70 6572 6d69  d any..non-permi
-000049c0: 7373 6976 6520 7465 726d 7320 6164 6465  ssive terms adde
-000049d0: 6420 696e 2061 6363 6f72 6420 7769 7468  d in accord with
-000049e0: 2073 6563 7469 6f6e 2037 2061 7070 6c79   section 7 apply
-000049f0: 2074 6f20 7468 6520 636f 6465 3b0d 0a6b   to the code;..k
-00004a00: 6565 7020 696e 7461 6374 2061 6c6c 206e  eep intact all n
-00004a10: 6f74 6963 6573 206f 6620 7468 6520 6162  otices of the ab
-00004a20: 7365 6e63 6520 6f66 2061 6e79 2077 6172  sence of any war
-00004a30: 7261 6e74 793b 2061 6e64 2067 6976 6520  ranty; and give 
-00004a40: 616c 6c0d 0a72 6563 6970 6965 6e74 7320  all..recipients 
-00004a50: 6120 636f 7079 206f 6620 7468 6973 204c  a copy of this L
-00004a60: 6963 656e 7365 2061 6c6f 6e67 2077 6974  icense along wit
-00004a70: 6820 7468 6520 5072 6f67 7261 6d2e 0d0a  h the Program...
-00004a80: 0d0a 2020 596f 7520 6d61 7920 6368 6172  ..  You may char
-00004a90: 6765 2061 6e79 2070 7269 6365 206f 7220  ge any price or 
-00004aa0: 6e6f 2070 7269 6365 2066 6f72 2065 6163  no price for eac
-00004ab0: 6820 636f 7079 2074 6861 7420 796f 7520  h copy that you 
-00004ac0: 636f 6e76 6579 2c0d 0a61 6e64 2079 6f75  convey,..and you
-00004ad0: 206d 6179 206f 6666 6572 2073 7570 706f   may offer suppo
-00004ae0: 7274 206f 7220 7761 7272 616e 7479 2070  rt or warranty p
-00004af0: 726f 7465 6374 696f 6e20 666f 7220 6120  rotection for a 
-00004b00: 6665 652e 0d0a 0d0a 2020 352e 2043 6f6e  fee.....  5. Con
-00004b10: 7665 7969 6e67 204d 6f64 6966 6965 6420  veying Modified 
-00004b20: 536f 7572 6365 2056 6572 7369 6f6e 732e  Source Versions.
-00004b30: 0d0a 0d0a 2020 596f 7520 6d61 7920 636f  ....  You may co
-00004b40: 6e76 6579 2061 2077 6f72 6b20 6261 7365  nvey a work base
-00004b50: 6420 6f6e 2074 6865 2050 726f 6772 616d  d on the Program
-00004b60: 2c20 6f72 2074 6865 206d 6f64 6966 6963  , or the modific
-00004b70: 6174 696f 6e73 2074 6f0d 0a70 726f 6475  ations to..produ
-00004b80: 6365 2069 7420 6672 6f6d 2074 6865 2050  ce it from the P
-00004b90: 726f 6772 616d 2c20 696e 2074 6865 2066  rogram, in the f
-00004ba0: 6f72 6d20 6f66 2073 6f75 7263 6520 636f  orm of source co
-00004bb0: 6465 2075 6e64 6572 2074 6865 0d0a 7465  de under the..te
-00004bc0: 726d 7320 6f66 2073 6563 7469 6f6e 2034  rms of section 4
-00004bd0: 2c20 7072 6f76 6964 6564 2074 6861 7420  , provided that 
-00004be0: 796f 7520 616c 736f 206d 6565 7420 616c  you also meet al
-00004bf0: 6c20 6f66 2074 6865 7365 2063 6f6e 6469  l of these condi
-00004c00: 7469 6f6e 733a 0d0a 0d0a 2020 2020 6129  tions:....    a)
-00004c10: 2054 6865 2077 6f72 6b20 6d75 7374 2063   The work must c
-00004c20: 6172 7279 2070 726f 6d69 6e65 6e74 206e  arry prominent n
-00004c30: 6f74 6963 6573 2073 7461 7469 6e67 2074  otices stating t
-00004c40: 6861 7420 796f 7520 6d6f 6469 6669 6564  hat you modified
-00004c50: 0d0a 2020 2020 6974 2c20 616e 6420 6769  ..    it, and gi
-00004c60: 7669 6e67 2061 2072 656c 6576 616e 7420  ving a relevant 
-00004c70: 6461 7465 2e0d 0a0d 0a20 2020 2062 2920  date.....    b) 
-00004c80: 5468 6520 776f 726b 206d 7573 7420 6361  The work must ca
-00004c90: 7272 7920 7072 6f6d 696e 656e 7420 6e6f  rry prominent no
-00004ca0: 7469 6365 7320 7374 6174 696e 6720 7468  tices stating th
-00004cb0: 6174 2069 7420 6973 0d0a 2020 2020 7265  at it is..    re
-00004cc0: 6c65 6173 6564 2075 6e64 6572 2074 6869  leased under thi
-00004cd0: 7320 4c69 6365 6e73 6520 616e 6420 616e  s License and an
-00004ce0: 7920 636f 6e64 6974 696f 6e73 2061 6464  y conditions add
-00004cf0: 6564 2075 6e64 6572 2073 6563 7469 6f6e  ed under section
-00004d00: 0d0a 2020 2020 372e 2020 5468 6973 2072  ..    7.  This r
-00004d10: 6571 7569 7265 6d65 6e74 206d 6f64 6966  equirement modif
-00004d20: 6965 7320 7468 6520 7265 7175 6972 656d  ies the requirem
-00004d30: 656e 7420 696e 2073 6563 7469 6f6e 2034  ent in section 4
-00004d40: 2074 6f0d 0a20 2020 2022 6b65 6570 2069   to..    "keep i
-00004d50: 6e74 6163 7420 616c 6c20 6e6f 7469 6365  ntact all notice
-00004d60: 7322 2e0d 0a0d 0a20 2020 2063 2920 596f  s".....    c) Yo
-00004d70: 7520 6d75 7374 206c 6963 656e 7365 2074  u must license t
-00004d80: 6865 2065 6e74 6972 6520 776f 726b 2c20  he entire work, 
-00004d90: 6173 2061 2077 686f 6c65 2c20 756e 6465  as a whole, unde
-00004da0: 7220 7468 6973 0d0a 2020 2020 4c69 6365  r this..    Lice
-00004db0: 6e73 6520 746f 2061 6e79 6f6e 6520 7768  nse to anyone wh
-00004dc0: 6f20 636f 6d65 7320 696e 746f 2070 6f73  o comes into pos
-00004dd0: 7365 7373 696f 6e20 6f66 2061 2063 6f70  session of a cop
-00004de0: 792e 2020 5468 6973 0d0a 2020 2020 4c69  y.  This..    Li
-00004df0: 6365 6e73 6520 7769 6c6c 2074 6865 7265  cense will there
-00004e00: 666f 7265 2061 7070 6c79 2c20 616c 6f6e  fore apply, alon
-00004e10: 6720 7769 7468 2061 6e79 2061 7070 6c69  g with any appli
-00004e20: 6361 626c 6520 7365 6374 696f 6e20 370d  cable section 7.
-00004e30: 0a20 2020 2061 6464 6974 696f 6e61 6c20  .    additional 
-00004e40: 7465 726d 732c 2074 6f20 7468 6520 7768  terms, to the wh
-00004e50: 6f6c 6520 6f66 2074 6865 2077 6f72 6b2c  ole of the work,
-00004e60: 2061 6e64 2061 6c6c 2069 7473 2070 6172   and all its par
-00004e70: 7473 2c0d 0a20 2020 2072 6567 6172 646c  ts,..    regardl
-00004e80: 6573 7320 6f66 2068 6f77 2074 6865 7920  ess of how they 
-00004e90: 6172 6520 7061 636b 6167 6564 2e20 2054  are packaged.  T
-00004ea0: 6869 7320 4c69 6365 6e73 6520 6769 7665  his License give
-00004eb0: 7320 6e6f 0d0a 2020 2020 7065 726d 6973  s no..    permis
-00004ec0: 7369 6f6e 2074 6f20 6c69 6365 6e73 6520  sion to license 
-00004ed0: 7468 6520 776f 726b 2069 6e20 616e 7920  the work in any 
-00004ee0: 6f74 6865 7220 7761 792c 2062 7574 2069  other way, but i
-00004ef0: 7420 646f 6573 206e 6f74 0d0a 2020 2020  t does not..    
-00004f00: 696e 7661 6c69 6461 7465 2073 7563 6820  invalidate such 
-00004f10: 7065 726d 6973 7369 6f6e 2069 6620 796f  permission if yo
-00004f20: 7520 6861 7665 2073 6570 6172 6174 656c  u have separatel
-00004f30: 7920 7265 6365 6976 6564 2069 742e 0d0a  y received it...
-00004f40: 0d0a 2020 2020 6429 2049 6620 7468 6520  ..    d) If the 
-00004f50: 776f 726b 2068 6173 2069 6e74 6572 6163  work has interac
-00004f60: 7469 7665 2075 7365 7220 696e 7465 7266  tive user interf
-00004f70: 6163 6573 2c20 6561 6368 206d 7573 7420  aces, each must 
-00004f80: 6469 7370 6c61 790d 0a20 2020 2041 7070  display..    App
-00004f90: 726f 7072 6961 7465 204c 6567 616c 204e  ropriate Legal N
-00004fa0: 6f74 6963 6573 3b20 686f 7765 7665 722c  otices; however,
-00004fb0: 2069 6620 7468 6520 5072 6f67 7261 6d20   if the Program 
-00004fc0: 6861 7320 696e 7465 7261 6374 6976 650d  has interactive.
-00004fd0: 0a20 2020 2069 6e74 6572 6661 6365 7320  .    interfaces 
-00004fe0: 7468 6174 2064 6f20 6e6f 7420 6469 7370  that do not disp
-00004ff0: 6c61 7920 4170 7072 6f70 7269 6174 6520  lay Appropriate 
-00005000: 4c65 6761 6c20 4e6f 7469 6365 732c 2079  Legal Notices, y
-00005010: 6f75 720d 0a20 2020 2077 6f72 6b20 6e65  our..    work ne
-00005020: 6564 206e 6f74 206d 616b 6520 7468 656d  ed not make them
-00005030: 2064 6f20 736f 2e0d 0a0d 0a20 2041 2063   do so.....  A c
-00005040: 6f6d 7069 6c61 7469 6f6e 206f 6620 6120  ompilation of a 
-00005050: 636f 7665 7265 6420 776f 726b 2077 6974  covered work wit
-00005060: 6820 6f74 6865 7220 7365 7061 7261 7465  h other separate
-00005070: 2061 6e64 2069 6e64 6570 656e 6465 6e74   and independent
-00005080: 0d0a 776f 726b 732c 2077 6869 6368 2061  ..works, which a
-00005090: 7265 206e 6f74 2062 7920 7468 6569 7220  re not by their 
-000050a0: 6e61 7475 7265 2065 7874 656e 7369 6f6e  nature extension
-000050b0: 7320 6f66 2074 6865 2063 6f76 6572 6564  s of the covered
-000050c0: 2077 6f72 6b2c 0d0a 616e 6420 7768 6963   work,..and whic
-000050d0: 6820 6172 6520 6e6f 7420 636f 6d62 696e  h are not combin
-000050e0: 6564 2077 6974 6820 6974 2073 7563 6820  ed with it such 
-000050f0: 6173 2074 6f20 666f 726d 2061 206c 6172  as to form a lar
-00005100: 6765 7220 7072 6f67 7261 6d2c 0d0a 696e  ger program,..in
-00005110: 206f 7220 6f6e 2061 2076 6f6c 756d 6520   or on a volume 
-00005120: 6f66 2061 2073 746f 7261 6765 206f 7220  of a storage or 
-00005130: 6469 7374 7269 6275 7469 6f6e 206d 6564  distribution med
-00005140: 6975 6d2c 2069 7320 6361 6c6c 6564 2061  ium, is called a
-00005150: 6e0d 0a22 6167 6772 6567 6174 6522 2069  n.."aggregate" i
-00005160: 6620 7468 6520 636f 6d70 696c 6174 696f  f the compilatio
-00005170: 6e20 616e 6420 6974 7320 7265 7375 6c74  n and its result
-00005180: 696e 6720 636f 7079 7269 6768 7420 6172  ing copyright ar
-00005190: 6520 6e6f 740d 0a75 7365 6420 746f 206c  e not..used to l
-000051a0: 696d 6974 2074 6865 2061 6363 6573 7320  imit the access 
-000051b0: 6f72 206c 6567 616c 2072 6967 6874 7320  or legal rights 
-000051c0: 6f66 2074 6865 2063 6f6d 7069 6c61 7469  of the compilati
-000051d0: 6f6e 2773 2075 7365 7273 0d0a 6265 796f  on's users..beyo
-000051e0: 6e64 2077 6861 7420 7468 6520 696e 6469  nd what the indi
-000051f0: 7669 6475 616c 2077 6f72 6b73 2070 6572  vidual works per
-00005200: 6d69 742e 2020 496e 636c 7573 696f 6e20  mit.  Inclusion 
-00005210: 6f66 2061 2063 6f76 6572 6564 2077 6f72  of a covered wor
-00005220: 6b0d 0a69 6e20 616e 2061 6767 7265 6761  k..in an aggrega
-00005230: 7465 2064 6f65 7320 6e6f 7420 6361 7573  te does not caus
-00005240: 6520 7468 6973 204c 6963 656e 7365 2074  e this License t
-00005250: 6f20 6170 706c 7920 746f 2074 6865 206f  o apply to the o
-00005260: 7468 6572 0d0a 7061 7274 7320 6f66 2074  ther..parts of t
-00005270: 6865 2061 6767 7265 6761 7465 2e0d 0a0d  he aggregate....
-00005280: 0a20 2036 2e20 436f 6e76 6579 696e 6720  .  6. Conveying 
-00005290: 4e6f 6e2d 536f 7572 6365 2046 6f72 6d73  Non-Source Forms
-000052a0: 2e0d 0a0d 0a20 2059 6f75 206d 6179 2063  .....  You may c
-000052b0: 6f6e 7665 7920 6120 636f 7665 7265 6420  onvey a covered 
-000052c0: 776f 726b 2069 6e20 6f62 6a65 6374 2063  work in object c
-000052d0: 6f64 6520 666f 726d 2075 6e64 6572 2074  ode form under t
-000052e0: 6865 2074 6572 6d73 0d0a 6f66 2073 6563  he terms..of sec
-000052f0: 7469 6f6e 7320 3420 616e 6420 352c 2070  tions 4 and 5, p
-00005300: 726f 7669 6465 6420 7468 6174 2079 6f75  rovided that you
-00005310: 2061 6c73 6f20 636f 6e76 6579 2074 6865   also convey the
-00005320: 0d0a 6d61 6368 696e 652d 7265 6164 6162  ..machine-readab
-00005330: 6c65 2043 6f72 7265 7370 6f6e 6469 6e67  le Corresponding
-00005340: 2053 6f75 7263 6520 756e 6465 7220 7468   Source under th
-00005350: 6520 7465 726d 7320 6f66 2074 6869 7320  e terms of this 
-00005360: 4c69 6365 6e73 652c 0d0a 696e 206f 6e65  License,..in one
-00005370: 206f 6620 7468 6573 6520 7761 7973 3a0d   of these ways:.
-00005380: 0a0d 0a20 2020 2061 2920 436f 6e76 6579  ...    a) Convey
-00005390: 2074 6865 206f 626a 6563 7420 636f 6465   the object code
-000053a0: 2069 6e2c 206f 7220 656d 626f 6469 6564   in, or embodied
-000053b0: 2069 6e2c 2061 2070 6879 7369 6361 6c20   in, a physical 
-000053c0: 7072 6f64 7563 740d 0a20 2020 2028 696e  product..    (in
-000053d0: 636c 7564 696e 6720 6120 7068 7973 6963  cluding a physic
-000053e0: 616c 2064 6973 7472 6962 7574 696f 6e20  al distribution 
-000053f0: 6d65 6469 756d 292c 2061 6363 6f6d 7061  medium), accompa
-00005400: 6e69 6564 2062 7920 7468 650d 0a20 2020  nied by the..   
-00005410: 2043 6f72 7265 7370 6f6e 6469 6e67 2053   Corresponding S
-00005420: 6f75 7263 6520 6669 7865 6420 6f6e 2061  ource fixed on a
-00005430: 2064 7572 6162 6c65 2070 6879 7369 6361   durable physica
-00005440: 6c20 6d65 6469 756d 0d0a 2020 2020 6375  l medium..    cu
-00005450: 7374 6f6d 6172 696c 7920 7573 6564 2066  stomarily used f
-00005460: 6f72 2073 6f66 7477 6172 6520 696e 7465  or software inte
-00005470: 7263 6861 6e67 652e 0d0a 0d0a 2020 2020  rchange.....    
-00005480: 6229 2043 6f6e 7665 7920 7468 6520 6f62  b) Convey the ob
-00005490: 6a65 6374 2063 6f64 6520 696e 2c20 6f72  ject code in, or
-000054a0: 2065 6d62 6f64 6965 6420 696e 2c20 6120   embodied in, a 
-000054b0: 7068 7973 6963 616c 2070 726f 6475 6374  physical product
-000054c0: 0d0a 2020 2020 2869 6e63 6c75 6469 6e67  ..    (including
-000054d0: 2061 2070 6879 7369 6361 6c20 6469 7374   a physical dist
-000054e0: 7269 6275 7469 6f6e 206d 6564 6975 6d29  ribution medium)
-000054f0: 2c20 6163 636f 6d70 616e 6965 6420 6279  , accompanied by
-00005500: 2061 0d0a 2020 2020 7772 6974 7465 6e20   a..    written 
-00005510: 6f66 6665 722c 2076 616c 6964 2066 6f72  offer, valid for
-00005520: 2061 7420 6c65 6173 7420 7468 7265 6520   at least three 
-00005530: 7965 6172 7320 616e 6420 7661 6c69 6420  years and valid 
-00005540: 666f 7220 6173 0d0a 2020 2020 6c6f 6e67  for as..    long
-00005550: 2061 7320 796f 7520 6f66 6665 7220 7370   as you offer sp
-00005560: 6172 6520 7061 7274 7320 6f72 2063 7573  are parts or cus
-00005570: 746f 6d65 7220 7375 7070 6f72 7420 666f  tomer support fo
-00005580: 7220 7468 6174 2070 726f 6475 6374 0d0a  r that product..
-00005590: 2020 2020 6d6f 6465 6c2c 2074 6f20 6769      model, to gi
-000055a0: 7665 2061 6e79 6f6e 6520 7768 6f20 706f  ve anyone who po
-000055b0: 7373 6573 7365 7320 7468 6520 6f62 6a65  ssesses the obje
-000055c0: 6374 2063 6f64 6520 6569 7468 6572 2028  ct code either (
-000055d0: 3129 2061 0d0a 2020 2020 636f 7079 206f  1) a..    copy o
-000055e0: 6620 7468 6520 436f 7272 6573 706f 6e64  f the Correspond
-000055f0: 696e 6720 536f 7572 6365 2066 6f72 2061  ing Source for a
-00005600: 6c6c 2074 6865 2073 6f66 7477 6172 6520  ll the software 
-00005610: 696e 2074 6865 0d0a 2020 2020 7072 6f64  in the..    prod
-00005620: 7563 7420 7468 6174 2069 7320 636f 7665  uct that is cove
-00005630: 7265 6420 6279 2074 6869 7320 4c69 6365  red by this Lice
-00005640: 6e73 652c 206f 6e20 6120 6475 7261 626c  nse, on a durabl
-00005650: 6520 7068 7973 6963 616c 0d0a 2020 2020  e physical..    
-00005660: 6d65 6469 756d 2063 7573 746f 6d61 7269  medium customari
-00005670: 6c79 2075 7365 6420 666f 7220 736f 6674  ly used for soft
-00005680: 7761 7265 2069 6e74 6572 6368 616e 6765  ware interchange
-00005690: 2c20 666f 7220 6120 7072 6963 6520 6e6f  , for a price no
-000056a0: 0d0a 2020 2020 6d6f 7265 2074 6861 6e20  ..    more than 
-000056b0: 796f 7572 2072 6561 736f 6e61 626c 6520  your reasonable 
-000056c0: 636f 7374 206f 6620 7068 7973 6963 616c  cost of physical
-000056d0: 6c79 2070 6572 666f 726d 696e 6720 7468  ly performing th
-000056e0: 6973 0d0a 2020 2020 636f 6e76 6579 696e  is..    conveyin
-000056f0: 6720 6f66 2073 6f75 7263 652c 206f 7220  g of source, or 
-00005700: 2832 2920 6163 6365 7373 2074 6f20 636f  (2) access to co
-00005710: 7079 2074 6865 0d0a 2020 2020 436f 7272  py the..    Corr
-00005720: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
-00005730: 2066 726f 6d20 6120 6e65 7477 6f72 6b20   from a network 
-00005740: 7365 7276 6572 2061 7420 6e6f 2063 6861  server at no cha
-00005750: 7267 652e 0d0a 0d0a 2020 2020 6329 2043  rge.....    c) C
-00005760: 6f6e 7665 7920 696e 6469 7669 6475 616c  onvey individual
-00005770: 2063 6f70 6965 7320 6f66 2074 6865 206f   copies of the o
-00005780: 626a 6563 7420 636f 6465 2077 6974 6820  bject code with 
-00005790: 6120 636f 7079 206f 6620 7468 650d 0a20  a copy of the.. 
-000057a0: 2020 2077 7269 7474 656e 206f 6666 6572     written offer
-000057b0: 2074 6f20 7072 6f76 6964 6520 7468 6520   to provide the 
-000057c0: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
-000057d0: 7572 6365 2e20 2054 6869 730d 0a20 2020  urce.  This..   
-000057e0: 2061 6c74 6572 6e61 7469 7665 2069 7320   alternative is 
-000057f0: 616c 6c6f 7765 6420 6f6e 6c79 206f 6363  allowed only occ
-00005800: 6173 696f 6e61 6c6c 7920 616e 6420 6e6f  asionally and no
-00005810: 6e63 6f6d 6d65 7263 6961 6c6c 792c 2061  ncommercially, a
-00005820: 6e64 0d0a 2020 2020 6f6e 6c79 2069 6620  nd..    only if 
-00005830: 796f 7520 7265 6365 6976 6564 2074 6865  you received the
-00005840: 206f 626a 6563 7420 636f 6465 2077 6974   object code wit
-00005850: 6820 7375 6368 2061 6e20 6f66 6665 722c  h such an offer,
-00005860: 2069 6e20 6163 636f 7264 0d0a 2020 2020   in accord..    
-00005870: 7769 7468 2073 7562 7365 6374 696f 6e20  with subsection 
-00005880: 3662 2e0d 0a0d 0a20 2020 2064 2920 436f  6b.....    d) Co
-00005890: 6e76 6579 2074 6865 206f 626a 6563 7420  nvey the object 
-000058a0: 636f 6465 2062 7920 6f66 6665 7269 6e67  code by offering
-000058b0: 2061 6363 6573 7320 6672 6f6d 2061 2064   access from a d
-000058c0: 6573 6967 6e61 7465 640d 0a20 2020 2070  esignated..    p
-000058d0: 6c61 6365 2028 6772 6174 6973 206f 7220  lace (gratis or 
-000058e0: 666f 7220 6120 6368 6172 6765 292c 2061  for a charge), a
-000058f0: 6e64 206f 6666 6572 2065 7175 6976 616c  nd offer equival
-00005900: 656e 7420 6163 6365 7373 2074 6f20 7468  ent access to th
-00005910: 650d 0a20 2020 2043 6f72 7265 7370 6f6e  e..    Correspon
-00005920: 6469 6e67 2053 6f75 7263 6520 696e 2074  ding Source in t
-00005930: 6865 2073 616d 6520 7761 7920 7468 726f  he same way thro
-00005940: 7567 6820 7468 6520 7361 6d65 2070 6c61  ugh the same pla
-00005950: 6365 2061 7420 6e6f 0d0a 2020 2020 6675  ce at no..    fu
-00005960: 7274 6865 7220 6368 6172 6765 2e20 2059  rther charge.  Y
-00005970: 6f75 206e 6565 6420 6e6f 7420 7265 7175  ou need not requ
-00005980: 6972 6520 7265 6369 7069 656e 7473 2074  ire recipients t
-00005990: 6f20 636f 7079 2074 6865 0d0a 2020 2020  o copy the..    
-000059a0: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
-000059b0: 7572 6365 2061 6c6f 6e67 2077 6974 6820  urce along with 
-000059c0: 7468 6520 6f62 6a65 6374 2063 6f64 652e  the object code.
-000059d0: 2020 4966 2074 6865 2070 6c61 6365 2074    If the place t
-000059e0: 6f0d 0a20 2020 2063 6f70 7920 7468 6520  o..    copy the 
-000059f0: 6f62 6a65 6374 2063 6f64 6520 6973 2061  object code is a
-00005a00: 206e 6574 776f 726b 2073 6572 7665 722c   network server,
-00005a10: 2074 6865 2043 6f72 7265 7370 6f6e 6469   the Correspondi
-00005a20: 6e67 2053 6f75 7263 650d 0a20 2020 206d  ng Source..    m
-00005a30: 6179 2062 6520 6f6e 2061 2064 6966 6665  ay be on a diffe
-00005a40: 7265 6e74 2073 6572 7665 7220 286f 7065  rent server (ope
-00005a50: 7261 7465 6420 6279 2079 6f75 206f 7220  rated by you or 
-00005a60: 6120 7468 6972 6420 7061 7274 7929 0d0a  a third party)..
-00005a70: 2020 2020 7468 6174 2073 7570 706f 7274      that support
-00005a80: 7320 6571 7569 7661 6c65 6e74 2063 6f70  s equivalent cop
-00005a90: 7969 6e67 2066 6163 696c 6974 6965 732c  ying facilities,
-00005aa0: 2070 726f 7669 6465 6420 796f 7520 6d61   provided you ma
-00005ab0: 696e 7461 696e 0d0a 2020 2020 636c 6561  intain..    clea
-00005ac0: 7220 6469 7265 6374 696f 6e73 206e 6578  r directions nex
-00005ad0: 7420 746f 2074 6865 206f 626a 6563 7420  t to the object 
-00005ae0: 636f 6465 2073 6179 696e 6720 7768 6572  code saying wher
-00005af0: 6520 746f 2066 696e 6420 7468 650d 0a20  e to find the.. 
-00005b00: 2020 2043 6f72 7265 7370 6f6e 6469 6e67     Corresponding
-00005b10: 2053 6f75 7263 652e 2020 5265 6761 7264   Source.  Regard
-00005b20: 6c65 7373 206f 6620 7768 6174 2073 6572  less of what ser
-00005b30: 7665 7220 686f 7374 7320 7468 650d 0a20  ver hosts the.. 
-00005b40: 2020 2043 6f72 7265 7370 6f6e 6469 6e67     Corresponding
-00005b50: 2053 6f75 7263 652c 2079 6f75 2072 656d   Source, you rem
-00005b60: 6169 6e20 6f62 6c69 6761 7465 6420 746f  ain obligated to
-00005b70: 2065 6e73 7572 6520 7468 6174 2069 7420   ensure that it 
-00005b80: 6973 0d0a 2020 2020 6176 6169 6c61 626c  is..    availabl
-00005b90: 6520 666f 7220 6173 206c 6f6e 6720 6173  e for as long as
-00005ba0: 206e 6565 6465 6420 746f 2073 6174 6973   needed to satis
-00005bb0: 6679 2074 6865 7365 2072 6571 7569 7265  fy these require
-00005bc0: 6d65 6e74 732e 0d0a 0d0a 2020 2020 6529  ments.....    e)
-00005bd0: 2043 6f6e 7665 7920 7468 6520 6f62 6a65   Convey the obje
-00005be0: 6374 2063 6f64 6520 7573 696e 6720 7065  ct code using pe
-00005bf0: 6572 2d74 6f2d 7065 6572 2074 7261 6e73  er-to-peer trans
-00005c00: 6d69 7373 696f 6e2c 2070 726f 7669 6465  mission, provide
-00005c10: 640d 0a20 2020 2079 6f75 2069 6e66 6f72  d..    you infor
-00005c20: 6d20 6f74 6865 7220 7065 6572 7320 7768  m other peers wh
-00005c30: 6572 6520 7468 6520 6f62 6a65 6374 2063  ere the object c
-00005c40: 6f64 6520 616e 6420 436f 7272 6573 706f  ode and Correspo
-00005c50: 6e64 696e 670d 0a20 2020 2053 6f75 7263  nding..    Sourc
-00005c60: 6520 6f66 2074 6865 2077 6f72 6b20 6172  e of the work ar
-00005c70: 6520 6265 696e 6720 6f66 6665 7265 6420  e being offered 
-00005c80: 746f 2074 6865 2067 656e 6572 616c 2070  to the general p
-00005c90: 7562 6c69 6320 6174 206e 6f0d 0a20 2020  ublic at no..   
-00005ca0: 2063 6861 7267 6520 756e 6465 7220 7375   charge under su
-00005cb0: 6273 6563 7469 6f6e 2036 642e 0d0a 0d0a  bsection 6d.....
-00005cc0: 2020 4120 7365 7061 7261 626c 6520 706f    A separable po
-00005cd0: 7274 696f 6e20 6f66 2074 6865 206f 626a  rtion of the obj
-00005ce0: 6563 7420 636f 6465 2c20 7768 6f73 6520  ect code, whose 
-00005cf0: 736f 7572 6365 2063 6f64 6520 6973 2065  source code is e
-00005d00: 7863 6c75 6465 640d 0a66 726f 6d20 7468  xcluded..from th
-00005d10: 6520 436f 7272 6573 706f 6e64 696e 6720  e Corresponding 
-00005d20: 536f 7572 6365 2061 7320 6120 5379 7374  Source as a Syst
-00005d30: 656d 204c 6962 7261 7279 2c20 6e65 6564  em Library, need
-00005d40: 206e 6f74 2062 650d 0a69 6e63 6c75 6465   not be..include
-00005d50: 6420 696e 2063 6f6e 7665 7969 6e67 2074  d in conveying t
-00005d60: 6865 206f 626a 6563 7420 636f 6465 2077  he object code w
-00005d70: 6f72 6b2e 0d0a 0d0a 2020 4120 2255 7365  ork.....  A "Use
-00005d80: 7220 5072 6f64 7563 7422 2069 7320 6569  r Product" is ei
-00005d90: 7468 6572 2028 3129 2061 2022 636f 6e73  ther (1) a "cons
-00005da0: 756d 6572 2070 726f 6475 6374 222c 2077  umer product", w
-00005db0: 6869 6368 206d 6561 6e73 2061 6e79 0d0a  hich means any..
-00005dc0: 7461 6e67 6962 6c65 2070 6572 736f 6e61  tangible persona
-00005dd0: 6c20 7072 6f70 6572 7479 2077 6869 6368  l property which
-00005de0: 2069 7320 6e6f 726d 616c 6c79 2075 7365   is normally use
-00005df0: 6420 666f 7220 7065 7273 6f6e 616c 2c20  d for personal, 
-00005e00: 6661 6d69 6c79 2c0d 0a6f 7220 686f 7573  family,..or hous
-00005e10: 6568 6f6c 6420 7075 7270 6f73 6573 2c20  ehold purposes, 
-00005e20: 6f72 2028 3229 2061 6e79 7468 696e 6720  or (2) anything 
-00005e30: 6465 7369 676e 6564 206f 7220 736f 6c64  designed or sold
-00005e40: 2066 6f72 2069 6e63 6f72 706f 7261 7469   for incorporati
-00005e50: 6f6e 0d0a 696e 746f 2061 2064 7765 6c6c  on..into a dwell
-00005e60: 696e 672e 2020 496e 2064 6574 6572 6d69  ing.  In determi
-00005e70: 6e69 6e67 2077 6865 7468 6572 2061 2070  ning whether a p
-00005e80: 726f 6475 6374 2069 7320 6120 636f 6e73  roduct is a cons
-00005e90: 756d 6572 2070 726f 6475 6374 2c0d 0a64  umer product,..d
-00005ea0: 6f75 6274 6675 6c20 6361 7365 7320 7368  oubtful cases sh
-00005eb0: 616c 6c20 6265 2072 6573 6f6c 7665 6420  all be resolved 
-00005ec0: 696e 2066 6176 6f72 206f 6620 636f 7665  in favor of cove
-00005ed0: 7261 6765 2e20 2046 6f72 2061 2070 6172  rage.  For a par
-00005ee0: 7469 6375 6c61 720d 0a70 726f 6475 6374  ticular..product
-00005ef0: 2072 6563 6569 7665 6420 6279 2061 2070   received by a p
-00005f00: 6172 7469 6375 6c61 7220 7573 6572 2c20  articular user, 
-00005f10: 226e 6f72 6d61 6c6c 7920 7573 6564 2220  "normally used" 
-00005f20: 7265 6665 7273 2074 6f20 610d 0a74 7970  refers to a..typ
-00005f30: 6963 616c 206f 7220 636f 6d6d 6f6e 2075  ical or common u
-00005f40: 7365 206f 6620 7468 6174 2063 6c61 7373  se of that class
-00005f50: 206f 6620 7072 6f64 7563 742c 2072 6567   of product, reg
-00005f60: 6172 646c 6573 7320 6f66 2074 6865 2073  ardless of the s
-00005f70: 7461 7475 730d 0a6f 6620 7468 6520 7061  tatus..of the pa
-00005f80: 7274 6963 756c 6172 2075 7365 7220 6f72  rticular user or
-00005f90: 206f 6620 7468 6520 7761 7920 696e 2077   of the way in w
-00005fa0: 6869 6368 2074 6865 2070 6172 7469 6375  hich the particu
-00005fb0: 6c61 7220 7573 6572 0d0a 6163 7475 616c  lar user..actual
-00005fc0: 6c79 2075 7365 732c 206f 7220 6578 7065  ly uses, or expe
-00005fd0: 6374 7320 6f72 2069 7320 6578 7065 6374  cts or is expect
-00005fe0: 6564 2074 6f20 7573 652c 2074 6865 2070  ed to use, the p
-00005ff0: 726f 6475 6374 2e20 2041 2070 726f 6475  roduct.  A produ
-00006000: 6374 0d0a 6973 2061 2063 6f6e 7375 6d65  ct..is a consume
-00006010: 7220 7072 6f64 7563 7420 7265 6761 7264  r product regard
-00006020: 6c65 7373 206f 6620 7768 6574 6865 7220  less of whether 
-00006030: 7468 6520 7072 6f64 7563 7420 6861 7320  the product has 
-00006040: 7375 6273 7461 6e74 6961 6c0d 0a63 6f6d  substantial..com
-00006050: 6d65 7263 6961 6c2c 2069 6e64 7573 7472  mercial, industr
-00006060: 6961 6c20 6f72 206e 6f6e 2d63 6f6e 7375  ial or non-consu
-00006070: 6d65 7220 7573 6573 2c20 756e 6c65 7373  mer uses, unless
-00006080: 2073 7563 6820 7573 6573 2072 6570 7265   such uses repre
-00006090: 7365 6e74 0d0a 7468 6520 6f6e 6c79 2073  sent..the only s
-000060a0: 6967 6e69 6669 6361 6e74 206d 6f64 6520  ignificant mode 
-000060b0: 6f66 2075 7365 206f 6620 7468 6520 7072  of use of the pr
-000060c0: 6f64 7563 742e 0d0a 0d0a 2020 2249 6e73  oduct.....  "Ins
-000060d0: 7461 6c6c 6174 696f 6e20 496e 666f 726d  tallation Inform
-000060e0: 6174 696f 6e22 2066 6f72 2061 2055 7365  ation" for a Use
-000060f0: 7220 5072 6f64 7563 7420 6d65 616e 7320  r Product means 
-00006100: 616e 7920 6d65 7468 6f64 732c 0d0a 7072  any methods,..pr
-00006110: 6f63 6564 7572 6573 2c20 6175 7468 6f72  ocedures, author
-00006120: 697a 6174 696f 6e20 6b65 7973 2c20 6f72  ization keys, or
-00006130: 206f 7468 6572 2069 6e66 6f72 6d61 7469   other informati
-00006140: 6f6e 2072 6571 7569 7265 6420 746f 2069  on required to i
-00006150: 6e73 7461 6c6c 0d0a 616e 6420 6578 6563  nstall..and exec
-00006160: 7574 6520 6d6f 6469 6669 6564 2076 6572  ute modified ver
-00006170: 7369 6f6e 7320 6f66 2061 2063 6f76 6572  sions of a cover
-00006180: 6564 2077 6f72 6b20 696e 2074 6861 7420  ed work in that 
-00006190: 5573 6572 2050 726f 6475 6374 2066 726f  User Product fro
-000061a0: 6d0d 0a61 206d 6f64 6966 6965 6420 7665  m..a modified ve
-000061b0: 7273 696f 6e20 6f66 2069 7473 2043 6f72  rsion of its Cor
-000061c0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
-000061d0: 652e 2020 5468 6520 696e 666f 726d 6174  e.  The informat
-000061e0: 696f 6e20 6d75 7374 0d0a 7375 6666 6963  ion must..suffic
-000061f0: 6520 746f 2065 6e73 7572 6520 7468 6174  e to ensure that
-00006200: 2074 6865 2063 6f6e 7469 6e75 6564 2066   the continued f
-00006210: 756e 6374 696f 6e69 6e67 206f 6620 7468  unctioning of th
-00006220: 6520 6d6f 6469 6669 6564 206f 626a 6563  e modified objec
-00006230: 740d 0a63 6f64 6520 6973 2069 6e20 6e6f  t..code is in no
-00006240: 2063 6173 6520 7072 6576 656e 7465 6420   case prevented 
-00006250: 6f72 2069 6e74 6572 6665 7265 6420 7769  or interfered wi
-00006260: 7468 2073 6f6c 656c 7920 6265 6361 7573  th solely becaus
-00006270: 650d 0a6d 6f64 6966 6963 6174 696f 6e20  e..modification 
-00006280: 6861 7320 6265 656e 206d 6164 652e 0d0a  has been made...
-00006290: 0d0a 2020 4966 2079 6f75 2063 6f6e 7665  ..  If you conve
-000062a0: 7920 616e 206f 626a 6563 7420 636f 6465  y an object code
-000062b0: 2077 6f72 6b20 756e 6465 7220 7468 6973   work under this
-000062c0: 2073 6563 7469 6f6e 2069 6e2c 206f 7220   section in, or 
-000062d0: 7769 7468 2c20 6f72 0d0a 7370 6563 6966  with, or..specif
-000062e0: 6963 616c 6c79 2066 6f72 2075 7365 2069  ically for use i
-000062f0: 6e2c 2061 2055 7365 7220 5072 6f64 7563  n, a User Produc
-00006300: 742c 2061 6e64 2074 6865 2063 6f6e 7665  t, and the conve
-00006310: 7969 6e67 206f 6363 7572 7320 6173 0d0a  ying occurs as..
-00006320: 7061 7274 206f 6620 6120 7472 616e 7361  part of a transa
-00006330: 6374 696f 6e20 696e 2077 6869 6368 2074  ction in which t
-00006340: 6865 2072 6967 6874 206f 6620 706f 7373  he right of poss
-00006350: 6573 7369 6f6e 2061 6e64 2075 7365 206f  ession and use o
-00006360: 6620 7468 650d 0a55 7365 7220 5072 6f64  f the..User Prod
-00006370: 7563 7420 6973 2074 7261 6e73 6665 7272  uct is transferr
-00006380: 6564 2074 6f20 7468 6520 7265 6369 7069  ed to the recipi
-00006390: 656e 7420 696e 2070 6572 7065 7475 6974  ent in perpetuit
-000063a0: 7920 6f72 2066 6f72 2061 0d0a 6669 7865  y or for a..fixe
-000063b0: 6420 7465 726d 2028 7265 6761 7264 6c65  d term (regardle
-000063c0: 7373 206f 6620 686f 7720 7468 6520 7472  ss of how the tr
-000063d0: 616e 7361 6374 696f 6e20 6973 2063 6861  ansaction is cha
-000063e0: 7261 6374 6572 697a 6564 292c 2074 6865  racterized), the
-000063f0: 0d0a 436f 7272 6573 706f 6e64 696e 6720  ..Corresponding 
-00006400: 536f 7572 6365 2063 6f6e 7665 7965 6420  Source conveyed 
-00006410: 756e 6465 7220 7468 6973 2073 6563 7469  under this secti
-00006420: 6f6e 206d 7573 7420 6265 2061 6363 6f6d  on must be accom
-00006430: 7061 6e69 6564 0d0a 6279 2074 6865 2049  panied..by the I
-00006440: 6e73 7461 6c6c 6174 696f 6e20 496e 666f  nstallation Info
-00006450: 726d 6174 696f 6e2e 2020 4275 7420 7468  rmation.  But th
-00006460: 6973 2072 6571 7569 7265 6d65 6e74 2064  is requirement d
-00006470: 6f65 7320 6e6f 7420 6170 706c 790d 0a69  oes not apply..i
-00006480: 6620 6e65 6974 6865 7220 796f 7520 6e6f  f neither you no
-00006490: 7220 616e 7920 7468 6972 6420 7061 7274  r any third part
-000064a0: 7920 7265 7461 696e 7320 7468 6520 6162  y retains the ab
-000064b0: 696c 6974 7920 746f 2069 6e73 7461 6c6c  ility to install
-000064c0: 0d0a 6d6f 6469 6669 6564 206f 626a 6563  ..modified objec
-000064d0: 7420 636f 6465 206f 6e20 7468 6520 5573  t code on the Us
-000064e0: 6572 2050 726f 6475 6374 2028 666f 7220  er Product (for 
-000064f0: 6578 616d 706c 652c 2074 6865 2077 6f72  example, the wor
-00006500: 6b20 6861 730d 0a62 6565 6e20 696e 7374  k has..been inst
-00006510: 616c 6c65 6420 696e 2052 4f4d 292e 0d0a  alled in ROM)...
-00006520: 0d0a 2020 5468 6520 7265 7175 6972 656d  ..  The requirem
-00006530: 656e 7420 746f 2070 726f 7669 6465 2049  ent to provide I
-00006540: 6e73 7461 6c6c 6174 696f 6e20 496e 666f  nstallation Info
-00006550: 726d 6174 696f 6e20 646f 6573 206e 6f74  rmation does not
-00006560: 2069 6e63 6c75 6465 2061 0d0a 7265 7175   include a..requ
-00006570: 6972 656d 656e 7420 746f 2063 6f6e 7469  irement to conti
-00006580: 6e75 6520 746f 2070 726f 7669 6465 2073  nue to provide s
-00006590: 7570 706f 7274 2073 6572 7669 6365 2c20  upport service, 
-000065a0: 7761 7272 616e 7479 2c20 6f72 2075 7064  warranty, or upd
-000065b0: 6174 6573 0d0a 666f 7220 6120 776f 726b  ates..for a work
-000065c0: 2074 6861 7420 6861 7320 6265 656e 206d   that has been m
-000065d0: 6f64 6966 6965 6420 6f72 2069 6e73 7461  odified or insta
-000065e0: 6c6c 6564 2062 7920 7468 6520 7265 6369  lled by the reci
-000065f0: 7069 656e 742c 206f 7220 666f 720d 0a74  pient, or for..t
-00006600: 6865 2055 7365 7220 5072 6f64 7563 7420  he User Product 
-00006610: 696e 2077 6869 6368 2069 7420 6861 7320  in which it has 
-00006620: 6265 656e 206d 6f64 6966 6965 6420 6f72  been modified or
-00006630: 2069 6e73 7461 6c6c 6564 2e20 2041 6363   installed.  Acc
-00006640: 6573 7320 746f 2061 0d0a 6e65 7477 6f72  ess to a..networ
-00006650: 6b20 6d61 7920 6265 2064 656e 6965 6420  k may be denied 
-00006660: 7768 656e 2074 6865 206d 6f64 6966 6963  when the modific
-00006670: 6174 696f 6e20 6974 7365 6c66 206d 6174  ation itself mat
-00006680: 6572 6961 6c6c 7920 616e 640d 0a61 6476  erially and..adv
-00006690: 6572 7365 6c79 2061 6666 6563 7473 2074  ersely affects t
-000066a0: 6865 206f 7065 7261 7469 6f6e 206f 6620  he operation of 
-000066b0: 7468 6520 6e65 7477 6f72 6b20 6f72 2076  the network or v
-000066c0: 696f 6c61 7465 7320 7468 6520 7275 6c65  iolates the rule
-000066d0: 7320 616e 640d 0a70 726f 746f 636f 6c73  s and..protocols
-000066e0: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
-000066f0: 6f6e 2061 6372 6f73 7320 7468 6520 6e65  on across the ne
-00006700: 7477 6f72 6b2e 0d0a 0d0a 2020 436f 7272  twork.....  Corr
-00006710: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
-00006720: 2063 6f6e 7665 7965 642c 2061 6e64 2049   conveyed, and I
-00006730: 6e73 7461 6c6c 6174 696f 6e20 496e 666f  nstallation Info
-00006740: 726d 6174 696f 6e20 7072 6f76 6964 6564  rmation provided
-00006750: 2c0d 0a69 6e20 6163 636f 7264 2077 6974  ,..in accord wit
-00006760: 6820 7468 6973 2073 6563 7469 6f6e 206d  h this section m
-00006770: 7573 7420 6265 2069 6e20 6120 666f 726d  ust be in a form
-00006780: 6174 2074 6861 7420 6973 2070 7562 6c69  at that is publi
-00006790: 636c 790d 0a64 6f63 756d 656e 7465 6420  cly..documented 
-000067a0: 2861 6e64 2077 6974 6820 616e 2069 6d70  (and with an imp
-000067b0: 6c65 6d65 6e74 6174 696f 6e20 6176 6169  lementation avai
-000067c0: 6c61 626c 6520 746f 2074 6865 2070 7562  lable to the pub
-000067d0: 6c69 6320 696e 0d0a 736f 7572 6365 2063  lic in..source c
-000067e0: 6f64 6520 666f 726d 292c 2061 6e64 206d  ode form), and m
-000067f0: 7573 7420 7265 7175 6972 6520 6e6f 2073  ust require no s
-00006800: 7065 6369 616c 2070 6173 7377 6f72 6420  pecial password 
-00006810: 6f72 206b 6579 2066 6f72 0d0a 756e 7061  or key for..unpa
-00006820: 636b 696e 672c 2072 6561 6469 6e67 206f  cking, reading o
-00006830: 7220 636f 7079 696e 672e 0d0a 0d0a 2020  r copying.....  
-00006840: 372e 2041 6464 6974 696f 6e61 6c20 5465  7. Additional Te
-00006850: 726d 732e 0d0a 0d0a 2020 2241 6464 6974  rms.....  "Addit
-00006860: 696f 6e61 6c20 7065 726d 6973 7369 6f6e  ional permission
-00006870: 7322 2061 7265 2074 6572 6d73 2074 6861  s" are terms tha
-00006880: 7420 7375 7070 6c65 6d65 6e74 2074 6865  t supplement the
-00006890: 2074 6572 6d73 206f 6620 7468 6973 0d0a   terms of this..
-000068a0: 4c69 6365 6e73 6520 6279 206d 616b 696e  License by makin
-000068b0: 6720 6578 6365 7074 696f 6e73 2066 726f  g exceptions fro
-000068c0: 6d20 6f6e 6520 6f72 206d 6f72 6520 6f66  m one or more of
-000068d0: 2069 7473 2063 6f6e 6469 7469 6f6e 732e   its conditions.
-000068e0: 0d0a 4164 6469 7469 6f6e 616c 2070 6572  ..Additional per
-000068f0: 6d69 7373 696f 6e73 2074 6861 7420 6172  missions that ar
-00006900: 6520 6170 706c 6963 6162 6c65 2074 6f20  e applicable to 
-00006910: 7468 6520 656e 7469 7265 2050 726f 6772  the entire Progr
-00006920: 616d 2073 6861 6c6c 0d0a 6265 2074 7265  am shall..be tre
-00006930: 6174 6564 2061 7320 7468 6f75 6768 2074  ated as though t
-00006940: 6865 7920 7765 7265 2069 6e63 6c75 6465  hey were include
-00006950: 6420 696e 2074 6869 7320 4c69 6365 6e73  d in this Licens
-00006960: 652c 2074 6f20 7468 6520 6578 7465 6e74  e, to the extent
-00006970: 0d0a 7468 6174 2074 6865 7920 6172 6520  ..that they are 
-00006980: 7661 6c69 6420 756e 6465 7220 6170 706c  valid under appl
-00006990: 6963 6162 6c65 206c 6177 2e20 2049 6620  icable law.  If 
-000069a0: 6164 6469 7469 6f6e 616c 2070 6572 6d69  additional permi
-000069b0: 7373 696f 6e73 0d0a 6170 706c 7920 6f6e  ssions..apply on
-000069c0: 6c79 2074 6f20 7061 7274 206f 6620 7468  ly to part of th
-000069d0: 6520 5072 6f67 7261 6d2c 2074 6861 7420  e Program, that 
-000069e0: 7061 7274 206d 6179 2062 6520 7573 6564  part may be used
-000069f0: 2073 6570 6172 6174 656c 790d 0a75 6e64   separately..und
-00006a00: 6572 2074 686f 7365 2070 6572 6d69 7373  er those permiss
-00006a10: 696f 6e73 2c20 6275 7420 7468 6520 656e  ions, but the en
-00006a20: 7469 7265 2050 726f 6772 616d 2072 656d  tire Program rem
-00006a30: 6169 6e73 2067 6f76 6572 6e65 6420 6279  ains governed by
-00006a40: 0d0a 7468 6973 204c 6963 656e 7365 2077  ..this License w
-00006a50: 6974 686f 7574 2072 6567 6172 6420 746f  ithout regard to
-00006a60: 2074 6865 2061 6464 6974 696f 6e61 6c20   the additional 
-00006a70: 7065 726d 6973 7369 6f6e 732e 0d0a 0d0a  permissions.....
-00006a80: 2020 5768 656e 2079 6f75 2063 6f6e 7665    When you conve
-00006a90: 7920 6120 636f 7079 206f 6620 6120 636f  y a copy of a co
-00006aa0: 7665 7265 6420 776f 726b 2c20 796f 7520  vered work, you 
-00006ab0: 6d61 7920 6174 2079 6f75 7220 6f70 7469  may at your opti
-00006ac0: 6f6e 0d0a 7265 6d6f 7665 2061 6e79 2061  on..remove any a
-00006ad0: 6464 6974 696f 6e61 6c20 7065 726d 6973  dditional permis
-00006ae0: 7369 6f6e 7320 6672 6f6d 2074 6861 7420  sions from that 
-00006af0: 636f 7079 2c20 6f72 2066 726f 6d20 616e  copy, or from an
-00006b00: 7920 7061 7274 206f 660d 0a69 742e 2020  y part of..it.  
-00006b10: 2841 6464 6974 696f 6e61 6c20 7065 726d  (Additional perm
-00006b20: 6973 7369 6f6e 7320 6d61 7920 6265 2077  issions may be w
-00006b30: 7269 7474 656e 2074 6f20 7265 7175 6972  ritten to requir
-00006b40: 6520 7468 6569 7220 6f77 6e0d 0a72 656d  e their own..rem
-00006b50: 6f76 616c 2069 6e20 6365 7274 6169 6e20  oval in certain 
-00006b60: 6361 7365 7320 7768 656e 2079 6f75 206d  cases when you m
-00006b70: 6f64 6966 7920 7468 6520 776f 726b 2e29  odify the work.)
-00006b80: 2020 596f 7520 6d61 7920 706c 6163 650d    You may place.
-00006b90: 0a61 6464 6974 696f 6e61 6c20 7065 726d  .additional perm
-00006ba0: 6973 7369 6f6e 7320 6f6e 206d 6174 6572  issions on mater
-00006bb0: 6961 6c2c 2061 6464 6564 2062 7920 796f  ial, added by yo
-00006bc0: 7520 746f 2061 2063 6f76 6572 6564 2077  u to a covered w
-00006bd0: 6f72 6b2c 0d0a 666f 7220 7768 6963 6820  ork,..for which 
-00006be0: 796f 7520 6861 7665 206f 7220 6361 6e20  you have or can 
-00006bf0: 6769 7665 2061 7070 726f 7072 6961 7465  give appropriate
-00006c00: 2063 6f70 7972 6967 6874 2070 6572 6d69   copyright permi
-00006c10: 7373 696f 6e2e 0d0a 0d0a 2020 4e6f 7477  ssion.....  Notw
-00006c20: 6974 6873 7461 6e64 696e 6720 616e 7920  ithstanding any 
-00006c30: 6f74 6865 7220 7072 6f76 6973 696f 6e20  other provision 
-00006c40: 6f66 2074 6869 7320 4c69 6365 6e73 652c  of this License,
-00006c50: 2066 6f72 206d 6174 6572 6961 6c20 796f   for material yo
-00006c60: 750d 0a61 6464 2074 6f20 6120 636f 7665  u..add to a cove
-00006c70: 7265 6420 776f 726b 2c20 796f 7520 6d61  red work, you ma
-00006c80: 7920 2869 6620 6175 7468 6f72 697a 6564  y (if authorized
-00006c90: 2062 7920 7468 6520 636f 7079 7269 6768   by the copyrigh
-00006ca0: 7420 686f 6c64 6572 7320 6f66 0d0a 7468  t holders of..th
-00006cb0: 6174 206d 6174 6572 6961 6c29 2073 7570  at material) sup
-00006cc0: 706c 656d 656e 7420 7468 6520 7465 726d  plement the term
-00006cd0: 7320 6f66 2074 6869 7320 4c69 6365 6e73  s of this Licens
-00006ce0: 6520 7769 7468 2074 6572 6d73 3a0d 0a0d  e with terms:...
-00006cf0: 0a20 2020 2061 2920 4469 7363 6c61 696d  .    a) Disclaim
-00006d00: 696e 6720 7761 7272 616e 7479 206f 7220  ing warranty or 
-00006d10: 6c69 6d69 7469 6e67 206c 6961 6269 6c69  limiting liabili
-00006d20: 7479 2064 6966 6665 7265 6e74 6c79 2066  ty differently f
-00006d30: 726f 6d20 7468 650d 0a20 2020 2074 6572  rom the..    ter
-00006d40: 6d73 206f 6620 7365 6374 696f 6e73 2031  ms of sections 1
-00006d50: 3520 616e 6420 3136 206f 6620 7468 6973  5 and 16 of this
-00006d60: 204c 6963 656e 7365 3b20 6f72 0d0a 0d0a   License; or....
-00006d70: 2020 2020 6229 2052 6571 7569 7269 6e67      b) Requiring
-00006d80: 2070 7265 7365 7276 6174 696f 6e20 6f66   preservation of
-00006d90: 2073 7065 6369 6669 6564 2072 6561 736f   specified reaso
-00006da0: 6e61 626c 6520 6c65 6761 6c20 6e6f 7469  nable legal noti
-00006db0: 6365 7320 6f72 0d0a 2020 2020 6175 7468  ces or..    auth
-00006dc0: 6f72 2061 7474 7269 6275 7469 6f6e 7320  or attributions 
-00006dd0: 696e 2074 6861 7420 6d61 7465 7269 616c  in that material
-00006de0: 206f 7220 696e 2074 6865 2041 7070 726f   or in the Appro
-00006df0: 7072 6961 7465 204c 6567 616c 0d0a 2020  priate Legal..  
-00006e00: 2020 4e6f 7469 6365 7320 6469 7370 6c61    Notices displa
-00006e10: 7965 6420 6279 2077 6f72 6b73 2063 6f6e  yed by works con
-00006e20: 7461 696e 696e 6720 6974 3b20 6f72 0d0a  taining it; or..
-00006e30: 0d0a 2020 2020 6329 2050 726f 6869 6269  ..    c) Prohibi
-00006e40: 7469 6e67 206d 6973 7265 7072 6573 656e  ting misrepresen
-00006e50: 7461 7469 6f6e 206f 6620 7468 6520 6f72  tation of the or
-00006e60: 6967 696e 206f 6620 7468 6174 206d 6174  igin of that mat
-00006e70: 6572 6961 6c2c 206f 720d 0a20 2020 2072  erial, or..    r
-00006e80: 6571 7569 7269 6e67 2074 6861 7420 6d6f  equiring that mo
-00006e90: 6469 6669 6564 2076 6572 7369 6f6e 7320  dified versions 
-00006ea0: 6f66 2073 7563 6820 6d61 7465 7269 616c  of such material
-00006eb0: 2062 6520 6d61 726b 6564 2069 6e0d 0a20   be marked in.. 
-00006ec0: 2020 2072 6561 736f 6e61 626c 6520 7761     reasonable wa
-00006ed0: 7973 2061 7320 6469 6666 6572 656e 7420  ys as different 
-00006ee0: 6672 6f6d 2074 6865 206f 7269 6769 6e61  from the origina
-00006ef0: 6c20 7665 7273 696f 6e3b 206f 720d 0a0d  l version; or...
-00006f00: 0a20 2020 2064 2920 4c69 6d69 7469 6e67  .    d) Limiting
-00006f10: 2074 6865 2075 7365 2066 6f72 2070 7562   the use for pub
-00006f20: 6c69 6369 7479 2070 7572 706f 7365 7320  licity purposes 
-00006f30: 6f66 206e 616d 6573 206f 6620 6c69 6365  of names of lice
-00006f40: 6e73 6f72 7320 6f72 0d0a 2020 2020 6175  nsors or..    au
-00006f50: 7468 6f72 7320 6f66 2074 6865 206d 6174  thors of the mat
-00006f60: 6572 6961 6c3b 206f 720d 0a0d 0a20 2020  erial; or....   
-00006f70: 2065 2920 4465 636c 696e 696e 6720 746f   e) Declining to
-00006f80: 2067 7261 6e74 2072 6967 6874 7320 756e   grant rights un
-00006f90: 6465 7220 7472 6164 656d 6172 6b20 6c61  der trademark la
-00006fa0: 7720 666f 7220 7573 6520 6f66 2073 6f6d  w for use of som
-00006fb0: 650d 0a20 2020 2074 7261 6465 206e 616d  e..    trade nam
-00006fc0: 6573 2c20 7472 6164 656d 6172 6b73 2c20  es, trademarks, 
-00006fd0: 6f72 2073 6572 7669 6365 206d 6172 6b73  or service marks
-00006fe0: 3b20 6f72 0d0a 0d0a 2020 2020 6629 2052  ; or....    f) R
-00006ff0: 6571 7569 7269 6e67 2069 6e64 656d 6e69  equiring indemni
-00007000: 6669 6361 7469 6f6e 206f 6620 6c69 6365  fication of lice
-00007010: 6e73 6f72 7320 616e 6420 6175 7468 6f72  nsors and author
-00007020: 7320 6f66 2074 6861 740d 0a20 2020 206d  s of that..    m
-00007030: 6174 6572 6961 6c20 6279 2061 6e79 6f6e  aterial by anyon
-00007040: 6520 7768 6f20 636f 6e76 6579 7320 7468  e who conveys th
-00007050: 6520 6d61 7465 7269 616c 2028 6f72 206d  e material (or m
-00007060: 6f64 6966 6965 6420 7665 7273 696f 6e73  odified versions
-00007070: 206f 660d 0a20 2020 2069 7429 2077 6974   of..    it) wit
-00007080: 6820 636f 6e74 7261 6374 7561 6c20 6173  h contractual as
-00007090: 7375 6d70 7469 6f6e 7320 6f66 206c 6961  sumptions of lia
-000070a0: 6269 6c69 7479 2074 6f20 7468 6520 7265  bility to the re
-000070b0: 6369 7069 656e 742c 2066 6f72 0d0a 2020  cipient, for..  
-000070c0: 2020 616e 7920 6c69 6162 696c 6974 7920    any liability 
-000070d0: 7468 6174 2074 6865 7365 2063 6f6e 7472  that these contr
-000070e0: 6163 7475 616c 2061 7373 756d 7074 696f  actual assumptio
-000070f0: 6e73 2064 6972 6563 746c 7920 696d 706f  ns directly impo
-00007100: 7365 206f 6e0d 0a20 2020 2074 686f 7365  se on..    those
-00007110: 206c 6963 656e 736f 7273 2061 6e64 2061   licensors and a
-00007120: 7574 686f 7273 2e0d 0a0d 0a20 2041 6c6c  uthors.....  All
-00007130: 206f 7468 6572 206e 6f6e 2d70 6572 6d69   other non-permi
-00007140: 7373 6976 6520 6164 6469 7469 6f6e 616c  ssive additional
-00007150: 2074 6572 6d73 2061 7265 2063 6f6e 7369   terms are consi
-00007160: 6465 7265 6420 2266 7572 7468 6572 0d0a  dered "further..
-00007170: 7265 7374 7269 6374 696f 6e73 2220 7769  restrictions" wi
-00007180: 7468 696e 2074 6865 206d 6561 6e69 6e67  thin the meaning
-00007190: 206f 6620 7365 6374 696f 6e20 3130 2e20   of section 10. 
-000071a0: 2049 6620 7468 6520 5072 6f67 7261 6d20   If the Program 
-000071b0: 6173 2079 6f75 0d0a 7265 6365 6976 6564  as you..received
-000071c0: 2069 742c 206f 7220 616e 7920 7061 7274   it, or any part
-000071d0: 206f 6620 6974 2c20 636f 6e74 6169 6e73   of it, contains
-000071e0: 2061 206e 6f74 6963 6520 7374 6174 696e   a notice statin
-000071f0: 6720 7468 6174 2069 7420 6973 0d0a 676f  g that it is..go
-00007200: 7665 726e 6564 2062 7920 7468 6973 204c  verned by this L
-00007210: 6963 656e 7365 2061 6c6f 6e67 2077 6974  icense along wit
-00007220: 6820 6120 7465 726d 2074 6861 7420 6973  h a term that is
-00007230: 2061 2066 7572 7468 6572 0d0a 7265 7374   a further..rest
-00007240: 7269 6374 696f 6e2c 2079 6f75 206d 6179  riction, you may
-00007250: 2072 656d 6f76 6520 7468 6174 2074 6572   remove that ter
-00007260: 6d2e 2020 4966 2061 206c 6963 656e 7365  m.  If a license
-00007270: 2064 6f63 756d 656e 7420 636f 6e74 6169   document contai
-00007280: 6e73 0d0a 6120 6675 7274 6865 7220 7265  ns..a further re
-00007290: 7374 7269 6374 696f 6e20 6275 7420 7065  striction but pe
-000072a0: 726d 6974 7320 7265 6c69 6365 6e73 696e  rmits relicensin
-000072b0: 6720 6f72 2063 6f6e 7665 7969 6e67 2075  g or conveying u
-000072c0: 6e64 6572 2074 6869 730d 0a4c 6963 656e  nder this..Licen
-000072d0: 7365 2c20 796f 7520 6d61 7920 6164 6420  se, you may add 
-000072e0: 746f 2061 2063 6f76 6572 6564 2077 6f72  to a covered wor
-000072f0: 6b20 6d61 7465 7269 616c 2067 6f76 6572  k material gover
-00007300: 6e65 6420 6279 2074 6865 2074 6572 6d73  ned by the terms
-00007310: 0d0a 6f66 2074 6861 7420 6c69 6365 6e73  ..of that licens
-00007320: 6520 646f 6375 6d65 6e74 2c20 7072 6f76  e document, prov
-00007330: 6964 6564 2074 6861 7420 7468 6520 6675  ided that the fu
-00007340: 7274 6865 7220 7265 7374 7269 6374 696f  rther restrictio
-00007350: 6e20 646f 6573 0d0a 6e6f 7420 7375 7276  n does..not surv
-00007360: 6976 6520 7375 6368 2072 656c 6963 656e  ive such relicen
-00007370: 7369 6e67 206f 7220 636f 6e76 6579 696e  sing or conveyin
-00007380: 672e 0d0a 0d0a 2020 4966 2079 6f75 2061  g.....  If you a
-00007390: 6464 2074 6572 6d73 2074 6f20 6120 636f  dd terms to a co
-000073a0: 7665 7265 6420 776f 726b 2069 6e20 6163  vered work in ac
-000073b0: 636f 7264 2077 6974 6820 7468 6973 2073  cord with this s
-000073c0: 6563 7469 6f6e 2c20 796f 750d 0a6d 7573  ection, you..mus
-000073d0: 7420 706c 6163 652c 2069 6e20 7468 6520  t place, in the 
-000073e0: 7265 6c65 7661 6e74 2073 6f75 7263 6520  relevant source 
-000073f0: 6669 6c65 732c 2061 2073 7461 7465 6d65  files, a stateme
-00007400: 6e74 206f 6620 7468 650d 0a61 6464 6974  nt of the..addit
-00007410: 696f 6e61 6c20 7465 726d 7320 7468 6174  ional terms that
-00007420: 2061 7070 6c79 2074 6f20 7468 6f73 6520   apply to those 
-00007430: 6669 6c65 732c 206f 7220 6120 6e6f 7469  files, or a noti
-00007440: 6365 2069 6e64 6963 6174 696e 670d 0a77  ce indicating..w
-00007450: 6865 7265 2074 6f20 6669 6e64 2074 6865  here to find the
-00007460: 2061 7070 6c69 6361 626c 6520 7465 726d   applicable term
-00007470: 732e 0d0a 0d0a 2020 4164 6469 7469 6f6e  s.....  Addition
-00007480: 616c 2074 6572 6d73 2c20 7065 726d 6973  al terms, permis
-00007490: 7369 7665 206f 7220 6e6f 6e2d 7065 726d  sive or non-perm
-000074a0: 6973 7369 7665 2c20 6d61 7920 6265 2073  issive, may be s
-000074b0: 7461 7465 6420 696e 2074 6865 0d0a 666f  tated in the..fo
-000074c0: 726d 206f 6620 6120 7365 7061 7261 7465  rm of a separate
-000074d0: 6c79 2077 7269 7474 656e 206c 6963 656e  ly written licen
-000074e0: 7365 2c20 6f72 2073 7461 7465 6420 6173  se, or stated as
-000074f0: 2065 7863 6570 7469 6f6e 733b 0d0a 7468   exceptions;..th
-00007500: 6520 6162 6f76 6520 7265 7175 6972 656d  e above requirem
-00007510: 656e 7473 2061 7070 6c79 2065 6974 6865  ents apply eithe
-00007520: 7220 7761 792e 0d0a 0d0a 2020 382e 2054  r way.....  8. T
-00007530: 6572 6d69 6e61 7469 6f6e 2e0d 0a0d 0a20  ermination..... 
-00007540: 2059 6f75 206d 6179 206e 6f74 2070 726f   You may not pro
-00007550: 7061 6761 7465 206f 7220 6d6f 6469 6679  pagate or modify
-00007560: 2061 2063 6f76 6572 6564 2077 6f72 6b20   a covered work 
-00007570: 6578 6365 7074 2061 7320 6578 7072 6573  except as expres
-00007580: 736c 790d 0a70 726f 7669 6465 6420 756e  sly..provided un
-00007590: 6465 7220 7468 6973 204c 6963 656e 7365  der this License
-000075a0: 2e20 2041 6e79 2061 7474 656d 7074 206f  .  Any attempt o
-000075b0: 7468 6572 7769 7365 2074 6f20 7072 6f70  therwise to prop
-000075c0: 6167 6174 6520 6f72 0d0a 6d6f 6469 6679  agate or..modify
-000075d0: 2069 7420 6973 2076 6f69 642c 2061 6e64   it is void, and
-000075e0: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
-000075f0: 6c6c 7920 7465 726d 696e 6174 6520 796f  lly terminate yo
-00007600: 7572 2072 6967 6874 7320 756e 6465 720d  ur rights under.
-00007610: 0a74 6869 7320 4c69 6365 6e73 6520 2869  .this License (i
-00007620: 6e63 6c75 6469 6e67 2061 6e79 2070 6174  ncluding any pat
-00007630: 656e 7420 6c69 6365 6e73 6573 2067 7261  ent licenses gra
-00007640: 6e74 6564 2075 6e64 6572 2074 6865 2074  nted under the t
-00007650: 6869 7264 0d0a 7061 7261 6772 6170 6820  hird..paragraph 
-00007660: 6f66 2073 6563 7469 6f6e 2031 3129 2e0d  of section 11)..
-00007670: 0a0d 0a20 2048 6f77 6576 6572 2c20 6966  ...  However, if
-00007680: 2079 6f75 2063 6561 7365 2061 6c6c 2076   you cease all v
-00007690: 696f 6c61 7469 6f6e 206f 6620 7468 6973  iolation of this
-000076a0: 204c 6963 656e 7365 2c20 7468 656e 2079   License, then y
-000076b0: 6f75 720d 0a6c 6963 656e 7365 2066 726f  our..license fro
-000076c0: 6d20 6120 7061 7274 6963 756c 6172 2063  m a particular c
-000076d0: 6f70 7972 6967 6874 2068 6f6c 6465 7220  opyright holder 
-000076e0: 6973 2072 6569 6e73 7461 7465 6420 2861  is reinstated (a
-000076f0: 290d 0a70 726f 7669 7369 6f6e 616c 6c79  )..provisionally
-00007700: 2c20 756e 6c65 7373 2061 6e64 2075 6e74  , unless and unt
-00007710: 696c 2074 6865 2063 6f70 7972 6967 6874  il the copyright
-00007720: 2068 6f6c 6465 7220 6578 706c 6963 6974   holder explicit
-00007730: 6c79 2061 6e64 0d0a 6669 6e61 6c6c 7920  ly and..finally 
-00007740: 7465 726d 696e 6174 6573 2079 6f75 7220  terminates your 
-00007750: 6c69 6365 6e73 652c 2061 6e64 2028 6229  license, and (b)
-00007760: 2070 6572 6d61 6e65 6e74 6c79 2c20 6966   permanently, if
-00007770: 2074 6865 2063 6f70 7972 6967 6874 0d0a   the copyright..
-00007780: 686f 6c64 6572 2066 6169 6c73 2074 6f20  holder fails to 
-00007790: 6e6f 7469 6679 2079 6f75 206f 6620 7468  notify you of th
-000077a0: 6520 7669 6f6c 6174 696f 6e20 6279 2073  e violation by s
-000077b0: 6f6d 6520 7265 6173 6f6e 6162 6c65 206d  ome reasonable m
-000077c0: 6561 6e73 0d0a 7072 696f 7220 746f 2036  eans..prior to 6
-000077d0: 3020 6461 7973 2061 6674 6572 2074 6865  0 days after the
-000077e0: 2063 6573 7361 7469 6f6e 2e0d 0a0d 0a20   cessation..... 
-000077f0: 204d 6f72 656f 7665 722c 2079 6f75 7220   Moreover, your 
-00007800: 6c69 6365 6e73 6520 6672 6f6d 2061 2070  license from a p
-00007810: 6172 7469 6375 6c61 7220 636f 7079 7269  articular copyri
-00007820: 6768 7420 686f 6c64 6572 2069 730d 0a72  ght holder is..r
-00007830: 6569 6e73 7461 7465 6420 7065 726d 616e  einstated perman
-00007840: 656e 746c 7920 6966 2074 6865 2063 6f70  ently if the cop
-00007850: 7972 6967 6874 2068 6f6c 6465 7220 6e6f  yright holder no
-00007860: 7469 6669 6573 2079 6f75 206f 6620 7468  tifies you of th
-00007870: 650d 0a76 696f 6c61 7469 6f6e 2062 7920  e..violation by 
-00007880: 736f 6d65 2072 6561 736f 6e61 626c 6520  some reasonable 
-00007890: 6d65 616e 732c 2074 6869 7320 6973 2074  means, this is t
-000078a0: 6865 2066 6972 7374 2074 696d 6520 796f  he first time yo
-000078b0: 7520 6861 7665 0d0a 7265 6365 6976 6564  u have..received
-000078c0: 206e 6f74 6963 6520 6f66 2076 696f 6c61   notice of viola
-000078d0: 7469 6f6e 206f 6620 7468 6973 204c 6963  tion of this Lic
-000078e0: 656e 7365 2028 666f 7220 616e 7920 776f  ense (for any wo
-000078f0: 726b 2920 6672 6f6d 2074 6861 740d 0a63  rk) from that..c
-00007900: 6f70 7972 6967 6874 2068 6f6c 6465 722c  opyright holder,
-00007910: 2061 6e64 2079 6f75 2063 7572 6520 7468   and you cure th
-00007920: 6520 7669 6f6c 6174 696f 6e20 7072 696f  e violation prio
-00007930: 7220 746f 2033 3020 6461 7973 2061 6674  r to 30 days aft
-00007940: 6572 0d0a 796f 7572 2072 6563 6569 7074  er..your receipt
-00007950: 206f 6620 7468 6520 6e6f 7469 6365 2e0d   of the notice..
-00007960: 0a0d 0a20 2054 6572 6d69 6e61 7469 6f6e  ...  Termination
-00007970: 206f 6620 796f 7572 2072 6967 6874 7320   of your rights 
-00007980: 756e 6465 7220 7468 6973 2073 6563 7469  under this secti
-00007990: 6f6e 2064 6f65 7320 6e6f 7420 7465 726d  on does not term
-000079a0: 696e 6174 6520 7468 650d 0a6c 6963 656e  inate the..licen
-000079b0: 7365 7320 6f66 2070 6172 7469 6573 2077  ses of parties w
-000079c0: 686f 2068 6176 6520 7265 6365 6976 6564  ho have received
-000079d0: 2063 6f70 6965 7320 6f72 2072 6967 6874   copies or right
-000079e0: 7320 6672 6f6d 2079 6f75 2075 6e64 6572  s from you under
-000079f0: 0d0a 7468 6973 204c 6963 656e 7365 2e20  ..this License. 
-00007a00: 2049 6620 796f 7572 2072 6967 6874 7320   If your rights 
-00007a10: 6861 7665 2062 6565 6e20 7465 726d 696e  have been termin
-00007a20: 6174 6564 2061 6e64 206e 6f74 2070 6572  ated and not per
-00007a30: 6d61 6e65 6e74 6c79 0d0a 7265 696e 7374  manently..reinst
-00007a40: 6174 6564 2c20 796f 7520 646f 206e 6f74  ated, you do not
-00007a50: 2071 7561 6c69 6679 2074 6f20 7265 6365   qualify to rece
-00007a60: 6976 6520 6e65 7720 6c69 6365 6e73 6573  ive new licenses
-00007a70: 2066 6f72 2074 6865 2073 616d 650d 0a6d   for the same..m
-00007a80: 6174 6572 6961 6c20 756e 6465 7220 7365  aterial under se
-00007a90: 6374 696f 6e20 3130 2e0d 0a0d 0a20 2039  ction 10.....  9
-00007aa0: 2e20 4163 6365 7074 616e 6365 204e 6f74  . Acceptance Not
-00007ab0: 2052 6571 7569 7265 6420 666f 7220 4861   Required for Ha
-00007ac0: 7669 6e67 2043 6f70 6965 732e 0d0a 0d0a  ving Copies.....
-00007ad0: 2020 596f 7520 6172 6520 6e6f 7420 7265    You are not re
-00007ae0: 7175 6972 6564 2074 6f20 6163 6365 7074  quired to accept
-00007af0: 2074 6869 7320 4c69 6365 6e73 6520 696e   this License in
-00007b00: 206f 7264 6572 2074 6f20 7265 6365 6976   order to receiv
-00007b10: 6520 6f72 0d0a 7275 6e20 6120 636f 7079  e or..run a copy
-00007b20: 206f 6620 7468 6520 5072 6f67 7261 6d2e   of the Program.
-00007b30: 2020 416e 6369 6c6c 6172 7920 7072 6f70    Ancillary prop
-00007b40: 6167 6174 696f 6e20 6f66 2061 2063 6f76  agation of a cov
-00007b50: 6572 6564 2077 6f72 6b0d 0a6f 6363 7572  ered work..occur
-00007b60: 7269 6e67 2073 6f6c 656c 7920 6173 2061  ring solely as a
-00007b70: 2063 6f6e 7365 7175 656e 6365 206f 6620   consequence of 
-00007b80: 7573 696e 6720 7065 6572 2d74 6f2d 7065  using peer-to-pe
-00007b90: 6572 2074 7261 6e73 6d69 7373 696f 6e0d  er transmission.
-00007ba0: 0a74 6f20 7265 6365 6976 6520 6120 636f  .to receive a co
-00007bb0: 7079 206c 696b 6577 6973 6520 646f 6573  py likewise does
-00007bc0: 206e 6f74 2072 6571 7569 7265 2061 6363   not require acc
-00007bd0: 6570 7461 6e63 652e 2020 486f 7765 7665  eptance.  Howeve
-00007be0: 722c 0d0a 6e6f 7468 696e 6720 6f74 6865  r,..nothing othe
-00007bf0: 7220 7468 616e 2074 6869 7320 4c69 6365  r than this Lice
-00007c00: 6e73 6520 6772 616e 7473 2079 6f75 2070  nse grants you p
-00007c10: 6572 6d69 7373 696f 6e20 746f 2070 726f  ermission to pro
-00007c20: 7061 6761 7465 206f 720d 0a6d 6f64 6966  pagate or..modif
-00007c30: 7920 616e 7920 636f 7665 7265 6420 776f  y any covered wo
-00007c40: 726b 2e20 2054 6865 7365 2061 6374 696f  rk.  These actio
-00007c50: 6e73 2069 6e66 7269 6e67 6520 636f 7079  ns infringe copy
-00007c60: 7269 6768 7420 6966 2079 6f75 2064 6f0d  right if you do.
-00007c70: 0a6e 6f74 2061 6363 6570 7420 7468 6973  .not accept this
-00007c80: 204c 6963 656e 7365 2e20 2054 6865 7265   License.  There
-00007c90: 666f 7265 2c20 6279 206d 6f64 6966 7969  fore, by modifyi
-00007ca0: 6e67 206f 7220 7072 6f70 6167 6174 696e  ng or propagatin
-00007cb0: 6720 610d 0a63 6f76 6572 6564 2077 6f72  g a..covered wor
-00007cc0: 6b2c 2079 6f75 2069 6e64 6963 6174 6520  k, you indicate 
-00007cd0: 796f 7572 2061 6363 6570 7461 6e63 6520  your acceptance 
-00007ce0: 6f66 2074 6869 7320 4c69 6365 6e73 6520  of this License 
-00007cf0: 746f 2064 6f20 736f 2e0d 0a0d 0a20 2031  to do so.....  1
-00007d00: 302e 2041 7574 6f6d 6174 6963 204c 6963  0. Automatic Lic
-00007d10: 656e 7369 6e67 206f 6620 446f 776e 7374  ensing of Downst
-00007d20: 7265 616d 2052 6563 6970 6965 6e74 732e  ream Recipients.
-00007d30: 0d0a 0d0a 2020 4561 6368 2074 696d 6520  ....  Each time 
-00007d40: 796f 7520 636f 6e76 6579 2061 2063 6f76  you convey a cov
-00007d50: 6572 6564 2077 6f72 6b2c 2074 6865 2072  ered work, the r
-00007d60: 6563 6970 6965 6e74 2061 7574 6f6d 6174  ecipient automat
-00007d70: 6963 616c 6c79 0d0a 7265 6365 6976 6573  ically..receives
-00007d80: 2061 206c 6963 656e 7365 2066 726f 6d20   a license from 
-00007d90: 7468 6520 6f72 6967 696e 616c 206c 6963  the original lic
-00007da0: 656e 736f 7273 2c20 746f 2072 756e 2c20  ensors, to run, 
-00007db0: 6d6f 6469 6679 2061 6e64 0d0a 7072 6f70  modify and..prop
-00007dc0: 6167 6174 6520 7468 6174 2077 6f72 6b2c  agate that work,
-00007dd0: 2073 7562 6a65 6374 2074 6f20 7468 6973   subject to this
-00007de0: 204c 6963 656e 7365 2e20 2059 6f75 2061   License.  You a
-00007df0: 7265 206e 6f74 2072 6573 706f 6e73 6962  re not responsib
-00007e00: 6c65 0d0a 666f 7220 656e 666f 7263 696e  le..for enforcin
-00007e10: 6720 636f 6d70 6c69 616e 6365 2062 7920  g compliance by 
-00007e20: 7468 6972 6420 7061 7274 6965 7320 7769  third parties wi
-00007e30: 7468 2074 6869 7320 4c69 6365 6e73 652e  th this License.
-00007e40: 0d0a 0d0a 2020 416e 2022 656e 7469 7479  ....  An "entity
-00007e50: 2074 7261 6e73 6163 7469 6f6e 2220 6973   transaction" is
-00007e60: 2061 2074 7261 6e73 6163 7469 6f6e 2074   a transaction t
-00007e70: 7261 6e73 6665 7272 696e 6720 636f 6e74  ransferring cont
-00007e80: 726f 6c20 6f66 2061 6e0d 0a6f 7267 616e  rol of an..organ
-00007e90: 697a 6174 696f 6e2c 206f 7220 7375 6273  ization, or subs
-00007ea0: 7461 6e74 6961 6c6c 7920 616c 6c20 6173  tantially all as
-00007eb0: 7365 7473 206f 6620 6f6e 652c 206f 7220  sets of one, or 
-00007ec0: 7375 6264 6976 6964 696e 6720 616e 0d0a  subdividing an..
-00007ed0: 6f72 6761 6e69 7a61 7469 6f6e 2c20 6f72  organization, or
-00007ee0: 206d 6572 6769 6e67 206f 7267 616e 697a   merging organiz
-00007ef0: 6174 696f 6e73 2e20 2049 6620 7072 6f70  ations.  If prop
-00007f00: 6167 6174 696f 6e20 6f66 2061 2063 6f76  agation of a cov
-00007f10: 6572 6564 0d0a 776f 726b 2072 6573 756c  ered..work resul
-00007f20: 7473 2066 726f 6d20 616e 2065 6e74 6974  ts from an entit
-00007f30: 7920 7472 616e 7361 6374 696f 6e2c 2065  y transaction, e
-00007f40: 6163 6820 7061 7274 7920 746f 2074 6861  ach party to tha
-00007f50: 740d 0a74 7261 6e73 6163 7469 6f6e 2077  t..transaction w
-00007f60: 686f 2072 6563 6569 7665 7320 6120 636f  ho receives a co
-00007f70: 7079 206f 6620 7468 6520 776f 726b 2061  py of the work a
-00007f80: 6c73 6f20 7265 6365 6976 6573 2077 6861  lso receives wha
-00007f90: 7465 7665 720d 0a6c 6963 656e 7365 7320  tever..licenses 
-00007fa0: 746f 2074 6865 2077 6f72 6b20 7468 6520  to the work the 
-00007fb0: 7061 7274 7927 7320 7072 6564 6563 6573  party's predeces
-00007fc0: 736f 7220 696e 2069 6e74 6572 6573 7420  sor in interest 
-00007fd0: 6861 6420 6f72 2063 6f75 6c64 0d0a 6769  had or could..gi
-00007fe0: 7665 2075 6e64 6572 2074 6865 2070 7265  ve under the pre
-00007ff0: 7669 6f75 7320 7061 7261 6772 6170 682c  vious paragraph,
-00008000: 2070 6c75 7320 6120 7269 6768 7420 746f   plus a right to
-00008010: 2070 6f73 7365 7373 696f 6e20 6f66 2074   possession of t
-00008020: 6865 0d0a 436f 7272 6573 706f 6e64 696e  he..Correspondin
-00008030: 6720 536f 7572 6365 206f 6620 7468 6520  g Source of the 
-00008040: 776f 726b 2066 726f 6d20 7468 6520 7072  work from the pr
-00008050: 6564 6563 6573 736f 7220 696e 2069 6e74  edecessor in int
-00008060: 6572 6573 742c 2069 660d 0a74 6865 2070  erest, if..the p
-00008070: 7265 6465 6365 7373 6f72 2068 6173 2069  redecessor has i
-00008080: 7420 6f72 2063 616e 2067 6574 2069 7420  t or can get it 
-00008090: 7769 7468 2072 6561 736f 6e61 626c 6520  with reasonable 
-000080a0: 6566 666f 7274 732e 0d0a 0d0a 2020 596f  efforts.....  Yo
-000080b0: 7520 6d61 7920 6e6f 7420 696d 706f 7365  u may not impose
-000080c0: 2061 6e79 2066 7572 7468 6572 2072 6573   any further res
-000080d0: 7472 6963 7469 6f6e 7320 6f6e 2074 6865  trictions on the
-000080e0: 2065 7865 7263 6973 6520 6f66 2074 6865   exercise of the
-000080f0: 0d0a 7269 6768 7473 2067 7261 6e74 6564  ..rights granted
-00008100: 206f 7220 6166 6669 726d 6564 2075 6e64   or affirmed und
-00008110: 6572 2074 6869 7320 4c69 6365 6e73 652e  er this License.
-00008120: 2020 466f 7220 6578 616d 706c 652c 2079    For example, y
-00008130: 6f75 206d 6179 0d0a 6e6f 7420 696d 706f  ou may..not impo
-00008140: 7365 2061 206c 6963 656e 7365 2066 6565  se a license fee
-00008150: 2c20 726f 7961 6c74 792c 206f 7220 6f74  , royalty, or ot
-00008160: 6865 7220 6368 6172 6765 2066 6f72 2065  her charge for e
-00008170: 7865 7263 6973 6520 6f66 0d0a 7269 6768  xercise of..righ
-00008180: 7473 2067 7261 6e74 6564 2075 6e64 6572  ts granted under
-00008190: 2074 6869 7320 4c69 6365 6e73 652c 2061   this License, a
-000081a0: 6e64 2079 6f75 206d 6179 206e 6f74 2069  nd you may not i
-000081b0: 6e69 7469 6174 6520 6c69 7469 6761 7469  nitiate litigati
-000081c0: 6f6e 0d0a 2869 6e63 6c75 6469 6e67 2061  on..(including a
-000081d0: 2063 726f 7373 2d63 6c61 696d 206f 7220   cross-claim or 
-000081e0: 636f 756e 7465 7263 6c61 696d 2069 6e20  counterclaim in 
-000081f0: 6120 6c61 7773 7569 7429 2061 6c6c 6567  a lawsuit) alleg
-00008200: 696e 6720 7468 6174 0d0a 616e 7920 7061  ing that..any pa
-00008210: 7465 6e74 2063 6c61 696d 2069 7320 696e  tent claim is in
-00008220: 6672 696e 6765 6420 6279 206d 616b 696e  fringed by makin
-00008230: 672c 2075 7369 6e67 2c20 7365 6c6c 696e  g, using, sellin
-00008240: 672c 206f 6666 6572 696e 6720 666f 720d  g, offering for.
-00008250: 0a73 616c 652c 206f 7220 696d 706f 7274  .sale, or import
-00008260: 696e 6720 7468 6520 5072 6f67 7261 6d20  ing the Program 
-00008270: 6f72 2061 6e79 2070 6f72 7469 6f6e 206f  or any portion o
-00008280: 6620 6974 2e0d 0a0d 0a20 2031 312e 2050  f it.....  11. P
-00008290: 6174 656e 7473 2e0d 0a0d 0a20 2041 2022  atents.....  A "
-000082a0: 636f 6e74 7269 6275 746f 7222 2069 7320  contributor" is 
-000082b0: 6120 636f 7079 7269 6768 7420 686f 6c64  a copyright hold
-000082c0: 6572 2077 686f 2061 7574 686f 7269 7a65  er who authorize
-000082d0: 7320 7573 6520 756e 6465 7220 7468 6973  s use under this
-000082e0: 0d0a 4c69 6365 6e73 6520 6f66 2074 6865  ..License of the
-000082f0: 2050 726f 6772 616d 206f 7220 6120 776f   Program or a wo
-00008300: 726b 206f 6e20 7768 6963 6820 7468 6520  rk on which the 
-00008310: 5072 6f67 7261 6d20 6973 2062 6173 6564  Program is based
-00008320: 2e20 2054 6865 0d0a 776f 726b 2074 6875  .  The..work thu
-00008330: 7320 6c69 6365 6e73 6564 2069 7320 6361  s licensed is ca
-00008340: 6c6c 6564 2074 6865 2063 6f6e 7472 6962  lled the contrib
-00008350: 7574 6f72 2773 2022 636f 6e74 7269 6275  utor's "contribu
-00008360: 746f 7220 7665 7273 696f 6e22 2e0d 0a0d  tor version"....
-00008370: 0a20 2041 2063 6f6e 7472 6962 7574 6f72  .  A contributor
-00008380: 2773 2022 6573 7365 6e74 6961 6c20 7061  's "essential pa
-00008390: 7465 6e74 2063 6c61 696d 7322 2061 7265  tent claims" are
-000083a0: 2061 6c6c 2070 6174 656e 7420 636c 6169   all patent clai
-000083b0: 6d73 0d0a 6f77 6e65 6420 6f72 2063 6f6e  ms..owned or con
-000083c0: 7472 6f6c 6c65 6420 6279 2074 6865 2063  trolled by the c
-000083d0: 6f6e 7472 6962 7574 6f72 2c20 7768 6574  ontributor, whet
-000083e0: 6865 7220 616c 7265 6164 7920 6163 7175  her already acqu
-000083f0: 6972 6564 206f 720d 0a68 6572 6561 6674  ired or..hereaft
-00008400: 6572 2061 6371 7569 7265 642c 2074 6861  er acquired, tha
-00008410: 7420 776f 756c 6420 6265 2069 6e66 7269  t would be infri
-00008420: 6e67 6564 2062 7920 736f 6d65 206d 616e  nged by some man
-00008430: 6e65 722c 2070 6572 6d69 7474 6564 0d0a  ner, permitted..
-00008440: 6279 2074 6869 7320 4c69 6365 6e73 652c  by this License,
-00008450: 206f 6620 6d61 6b69 6e67 2c20 7573 696e   of making, usin
-00008460: 672c 206f 7220 7365 6c6c 696e 6720 6974  g, or selling it
-00008470: 7320 636f 6e74 7269 6275 746f 7220 7665  s contributor ve
-00008480: 7273 696f 6e2c 0d0a 6275 7420 646f 206e  rsion,..but do n
-00008490: 6f74 2069 6e63 6c75 6465 2063 6c61 696d  ot include claim
-000084a0: 7320 7468 6174 2077 6f75 6c64 2062 6520  s that would be 
-000084b0: 696e 6672 696e 6765 6420 6f6e 6c79 2061  infringed only a
-000084c0: 7320 610d 0a63 6f6e 7365 7175 656e 6365  s a..consequence
-000084d0: 206f 6620 6675 7274 6865 7220 6d6f 6469   of further modi
-000084e0: 6669 6361 7469 6f6e 206f 6620 7468 6520  fication of the 
-000084f0: 636f 6e74 7269 6275 746f 7220 7665 7273  contributor vers
-00008500: 696f 6e2e 2020 466f 720d 0a70 7572 706f  ion.  For..purpo
-00008510: 7365 7320 6f66 2074 6869 7320 6465 6669  ses of this defi
-00008520: 6e69 7469 6f6e 2c20 2263 6f6e 7472 6f6c  nition, "control
-00008530: 2220 696e 636c 7564 6573 2074 6865 2072  " includes the r
-00008540: 6967 6874 2074 6f20 6772 616e 740d 0a70  ight to grant..p
-00008550: 6174 656e 7420 7375 626c 6963 656e 7365  atent sublicense
-00008560: 7320 696e 2061 206d 616e 6e65 7220 636f  s in a manner co
-00008570: 6e73 6973 7465 6e74 2077 6974 6820 7468  nsistent with th
-00008580: 6520 7265 7175 6972 656d 656e 7473 206f  e requirements o
-00008590: 660d 0a74 6869 7320 4c69 6365 6e73 652e  f..this License.
-000085a0: 0d0a 0d0a 2020 4561 6368 2063 6f6e 7472  ....  Each contr
-000085b0: 6962 7574 6f72 2067 7261 6e74 7320 796f  ibutor grants yo
-000085c0: 7520 6120 6e6f 6e2d 6578 636c 7573 6976  u a non-exclusiv
-000085d0: 652c 2077 6f72 6c64 7769 6465 2c20 726f  e, worldwide, ro
-000085e0: 7961 6c74 792d 6672 6565 0d0a 7061 7465  yalty-free..pate
-000085f0: 6e74 206c 6963 656e 7365 2075 6e64 6572  nt license under
-00008600: 2074 6865 2063 6f6e 7472 6962 7574 6f72   the contributor
-00008610: 2773 2065 7373 656e 7469 616c 2070 6174  's essential pat
-00008620: 656e 7420 636c 6169 6d73 2c20 746f 0d0a  ent claims, to..
-00008630: 6d61 6b65 2c20 7573 652c 2073 656c 6c2c  make, use, sell,
-00008640: 206f 6666 6572 2066 6f72 2073 616c 652c   offer for sale,
-00008650: 2069 6d70 6f72 7420 616e 6420 6f74 6865   import and othe
-00008660: 7277 6973 6520 7275 6e2c 206d 6f64 6966  rwise run, modif
-00008670: 7920 616e 640d 0a70 726f 7061 6761 7465  y and..propagate
-00008680: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
-00008690: 2069 7473 2063 6f6e 7472 6962 7574 6f72   its contributor
-000086a0: 2076 6572 7369 6f6e 2e0d 0a0d 0a20 2049   version.....  I
-000086b0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-000086c0: 7468 7265 6520 7061 7261 6772 6170 6873  three paragraphs
-000086d0: 2c20 6120 2270 6174 656e 7420 6c69 6365  , a "patent lice
-000086e0: 6e73 6522 2069 7320 616e 7920 6578 7072  nse" is any expr
-000086f0: 6573 730d 0a61 6772 6565 6d65 6e74 206f  ess..agreement o
-00008700: 7220 636f 6d6d 6974 6d65 6e74 2c20 686f  r commitment, ho
-00008710: 7765 7665 7220 6465 6e6f 6d69 6e61 7465  wever denominate
-00008720: 642c 206e 6f74 2074 6f20 656e 666f 7263  d, not to enforc
-00008730: 6520 6120 7061 7465 6e74 0d0a 2873 7563  e a patent..(suc
-00008740: 6820 6173 2061 6e20 6578 7072 6573 7320  h as an express 
-00008750: 7065 726d 6973 7369 6f6e 2074 6f20 7072  permission to pr
-00008760: 6163 7469 6365 2061 2070 6174 656e 7420  actice a patent 
-00008770: 6f72 2063 6f76 656e 616e 7420 6e6f 7420  or covenant not 
-00008780: 746f 0d0a 7375 6520 666f 7220 7061 7465  to..sue for pate
-00008790: 6e74 2069 6e66 7269 6e67 656d 656e 7429  nt infringement)
-000087a0: 2e20 2054 6f20 2267 7261 6e74 2220 7375  .  To "grant" su
-000087b0: 6368 2061 2070 6174 656e 7420 6c69 6365  ch a patent lice
-000087c0: 6e73 6520 746f 2061 0d0a 7061 7274 7920  nse to a..party 
-000087d0: 6d65 616e 7320 746f 206d 616b 6520 7375  means to make su
-000087e0: 6368 2061 6e20 6167 7265 656d 656e 7420  ch an agreement 
-000087f0: 6f72 2063 6f6d 6d69 746d 656e 7420 6e6f  or commitment no
-00008800: 7420 746f 2065 6e66 6f72 6365 2061 0d0a  t to enforce a..
-00008810: 7061 7465 6e74 2061 6761 696e 7374 2074  patent against t
-00008820: 6865 2070 6172 7479 2e0d 0a0d 0a20 2049  he party.....  I
-00008830: 6620 796f 7520 636f 6e76 6579 2061 2063  f you convey a c
-00008840: 6f76 6572 6564 2077 6f72 6b2c 206b 6e6f  overed work, kno
-00008850: 7769 6e67 6c79 2072 656c 7969 6e67 206f  wingly relying o
-00008860: 6e20 6120 7061 7465 6e74 206c 6963 656e  n a patent licen
-00008870: 7365 2c0d 0a61 6e64 2074 6865 2043 6f72  se,..and the Cor
-00008880: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
-00008890: 6520 6f66 2074 6865 2077 6f72 6b20 6973  e of the work is
-000088a0: 206e 6f74 2061 7661 696c 6162 6c65 2066   not available f
-000088b0: 6f72 2061 6e79 6f6e 650d 0a74 6f20 636f  or anyone..to co
-000088c0: 7079 2c20 6672 6565 206f 6620 6368 6172  py, free of char
-000088d0: 6765 2061 6e64 2075 6e64 6572 2074 6865  ge and under the
-000088e0: 2074 6572 6d73 206f 6620 7468 6973 204c   terms of this L
-000088f0: 6963 656e 7365 2c20 7468 726f 7567 6820  icense, through 
-00008900: 610d 0a70 7562 6c69 636c 7920 6176 6169  a..publicly avai
-00008910: 6c61 626c 6520 6e65 7477 6f72 6b20 7365  lable network se
-00008920: 7276 6572 206f 7220 6f74 6865 7220 7265  rver or other re
-00008930: 6164 696c 7920 6163 6365 7373 6962 6c65  adily accessible
-00008940: 206d 6561 6e73 2c0d 0a74 6865 6e20 796f   means,..then yo
-00008950: 7520 6d75 7374 2065 6974 6865 7220 2831  u must either (1
-00008960: 2920 6361 7573 6520 7468 6520 436f 7272  ) cause the Corr
-00008970: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
-00008980: 2074 6f20 6265 2073 6f0d 0a61 7661 696c   to be so..avail
-00008990: 6162 6c65 2c20 6f72 2028 3229 2061 7272  able, or (2) arr
-000089a0: 616e 6765 2074 6f20 6465 7072 6976 6520  ange to deprive 
-000089b0: 796f 7572 7365 6c66 206f 6620 7468 6520  yourself of the 
-000089c0: 6265 6e65 6669 7420 6f66 2074 6865 0d0a  benefit of the..
-000089d0: 7061 7465 6e74 206c 6963 656e 7365 2066  patent license f
-000089e0: 6f72 2074 6869 7320 7061 7274 6963 756c  or this particul
-000089f0: 6172 2077 6f72 6b2c 206f 7220 2833 2920  ar work, or (3) 
-00008a00: 6172 7261 6e67 652c 2069 6e20 6120 6d61  arrange, in a ma
-00008a10: 6e6e 6572 0d0a 636f 6e73 6973 7465 6e74  nner..consistent
-00008a20: 2077 6974 6820 7468 6520 7265 7175 6972   with the requir
-00008a30: 656d 656e 7473 206f 6620 7468 6973 204c  ements of this L
-00008a40: 6963 656e 7365 2c20 746f 2065 7874 656e  icense, to exten
-00008a50: 6420 7468 6520 7061 7465 6e74 0d0a 6c69  d the patent..li
-00008a60: 6365 6e73 6520 746f 2064 6f77 6e73 7472  cense to downstr
-00008a70: 6561 6d20 7265 6369 7069 656e 7473 2e20  eam recipients. 
-00008a80: 2022 4b6e 6f77 696e 676c 7920 7265 6c79   "Knowingly rely
-00008a90: 696e 6722 206d 6561 6e73 2079 6f75 2068  ing" means you h
-00008aa0: 6176 650d 0a61 6374 7561 6c20 6b6e 6f77  ave..actual know
-00008ab0: 6c65 6467 6520 7468 6174 2c20 6275 7420  ledge that, but 
-00008ac0: 666f 7220 7468 6520 7061 7465 6e74 206c  for the patent l
-00008ad0: 6963 656e 7365 2c20 796f 7572 2063 6f6e  icense, your con
-00008ae0: 7665 7969 6e67 2074 6865 0d0a 636f 7665  veying the..cove
-00008af0: 7265 6420 776f 726b 2069 6e20 6120 636f  red work in a co
-00008b00: 756e 7472 792c 206f 7220 796f 7572 2072  untry, or your r
-00008b10: 6563 6970 6965 6e74 2773 2075 7365 206f  ecipient's use o
-00008b20: 6620 7468 6520 636f 7665 7265 6420 776f  f the covered wo
-00008b30: 726b 0d0a 696e 2061 2063 6f75 6e74 7279  rk..in a country
-00008b40: 2c20 776f 756c 6420 696e 6672 696e 6765  , would infringe
-00008b50: 206f 6e65 206f 7220 6d6f 7265 2069 6465   one or more ide
-00008b60: 6e74 6966 6961 626c 6520 7061 7465 6e74  ntifiable patent
-00008b70: 7320 696e 2074 6861 740d 0a63 6f75 6e74  s in that..count
-00008b80: 7279 2074 6861 7420 796f 7520 6861 7665  ry that you have
-00008b90: 2072 6561 736f 6e20 746f 2062 656c 6965   reason to belie
-00008ba0: 7665 2061 7265 2076 616c 6964 2e0d 0a0d  ve are valid....
-00008bb0: 0a20 2049 662c 2070 7572 7375 616e 7420  .  If, pursuant 
-00008bc0: 746f 206f 7220 696e 2063 6f6e 6e65 6374  to or in connect
-00008bd0: 696f 6e20 7769 7468 2061 2073 696e 676c  ion with a singl
-00008be0: 6520 7472 616e 7361 6374 696f 6e20 6f72  e transaction or
-00008bf0: 0d0a 6172 7261 6e67 656d 656e 742c 2079  ..arrangement, y
-00008c00: 6f75 2063 6f6e 7665 792c 206f 7220 7072  ou convey, or pr
-00008c10: 6f70 6167 6174 6520 6279 2070 726f 6375  opagate by procu
-00008c20: 7269 6e67 2063 6f6e 7665 7961 6e63 6520  ring conveyance 
-00008c30: 6f66 2c20 610d 0a63 6f76 6572 6564 2077  of, a..covered w
-00008c40: 6f72 6b2c 2061 6e64 2067 7261 6e74 2061  ork, and grant a
-00008c50: 2070 6174 656e 7420 6c69 6365 6e73 6520   patent license 
-00008c60: 746f 2073 6f6d 6520 6f66 2074 6865 2070  to some of the p
-00008c70: 6172 7469 6573 0d0a 7265 6365 6976 696e  arties..receivin
-00008c80: 6720 7468 6520 636f 7665 7265 6420 776f  g the covered wo
-00008c90: 726b 2061 7574 686f 7269 7a69 6e67 2074  rk authorizing t
-00008ca0: 6865 6d20 746f 2075 7365 2c20 7072 6f70  hem to use, prop
-00008cb0: 6167 6174 652c 206d 6f64 6966 790d 0a6f  agate, modify..o
-00008cc0: 7220 636f 6e76 6579 2061 2073 7065 6369  r convey a speci
-00008cd0: 6669 6320 636f 7079 206f 6620 7468 6520  fic copy of the 
-00008ce0: 636f 7665 7265 6420 776f 726b 2c20 7468  covered work, th
-00008cf0: 656e 2074 6865 2070 6174 656e 7420 6c69  en the patent li
-00008d00: 6365 6e73 650d 0a79 6f75 2067 7261 6e74  cense..you grant
-00008d10: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
-00008d20: 7920 6578 7465 6e64 6564 2074 6f20 616c  y extended to al
-00008d30: 6c20 7265 6369 7069 656e 7473 206f 6620  l recipients of 
-00008d40: 7468 6520 636f 7665 7265 640d 0a77 6f72  the covered..wor
-00008d50: 6b20 616e 6420 776f 726b 7320 6261 7365  k and works base
-00008d60: 6420 6f6e 2069 742e 0d0a 0d0a 2020 4120  d on it.....  A 
-00008d70: 7061 7465 6e74 206c 6963 656e 7365 2069  patent license i
-00008d80: 7320 2264 6973 6372 696d 696e 6174 6f72  s "discriminator
-00008d90: 7922 2069 6620 6974 2064 6f65 7320 6e6f  y" if it does no
-00008da0: 7420 696e 636c 7564 6520 7769 7468 696e  t include within
-00008db0: 0d0a 7468 6520 7363 6f70 6520 6f66 2069  ..the scope of i
-00008dc0: 7473 2063 6f76 6572 6167 652c 2070 726f  ts coverage, pro
-00008dd0: 6869 6269 7473 2074 6865 2065 7865 7263  hibits the exerc
-00008de0: 6973 6520 6f66 2c20 6f72 2069 730d 0a63  ise of, or is..c
-00008df0: 6f6e 6469 7469 6f6e 6564 206f 6e20 7468  onditioned on th
-00008e00: 6520 6e6f 6e2d 6578 6572 6369 7365 206f  e non-exercise o
-00008e10: 6620 6f6e 6520 6f72 206d 6f72 6520 6f66  f one or more of
-00008e20: 2074 6865 2072 6967 6874 7320 7468 6174   the rights that
-00008e30: 2061 7265 0d0a 7370 6563 6966 6963 616c   are..specifical
-00008e40: 6c79 2067 7261 6e74 6564 2075 6e64 6572  ly granted under
-00008e50: 2074 6869 7320 4c69 6365 6e73 652e 2020   this License.  
-00008e60: 596f 7520 6d61 7920 6e6f 7420 636f 6e76  You may not conv
-00008e70: 6579 2061 2063 6f76 6572 6564 0d0a 776f  ey a covered..wo
-00008e80: 726b 2069 6620 796f 7520 6172 6520 6120  rk if you are a 
-00008e90: 7061 7274 7920 746f 2061 6e20 6172 7261  party to an arra
-00008ea0: 6e67 656d 656e 7420 7769 7468 2061 2074  ngement with a t
-00008eb0: 6869 7264 2070 6172 7479 2074 6861 7420  hird party that 
-00008ec0: 6973 0d0a 696e 2074 6865 2062 7573 696e  is..in the busin
-00008ed0: 6573 7320 6f66 2064 6973 7472 6962 7574  ess of distribut
-00008ee0: 696e 6720 736f 6674 7761 7265 2c20 756e  ing software, un
-00008ef0: 6465 7220 7768 6963 6820 796f 7520 6d61  der which you ma
-00008f00: 6b65 2070 6179 6d65 6e74 0d0a 746f 2074  ke payment..to t
-00008f10: 6865 2074 6869 7264 2070 6172 7479 2062  he third party b
-00008f20: 6173 6564 206f 6e20 7468 6520 6578 7465  ased on the exte
-00008f30: 6e74 206f 6620 796f 7572 2061 6374 6976  nt of your activ
-00008f40: 6974 7920 6f66 2063 6f6e 7665 7969 6e67  ity of conveying
-00008f50: 0d0a 7468 6520 776f 726b 2c20 616e 6420  ..the work, and 
-00008f60: 756e 6465 7220 7768 6963 6820 7468 6520  under which the 
-00008f70: 7468 6972 6420 7061 7274 7920 6772 616e  third party gran
-00008f80: 7473 2c20 746f 2061 6e79 206f 6620 7468  ts, to any of th
-00008f90: 650d 0a70 6172 7469 6573 2077 686f 2077  e..parties who w
-00008fa0: 6f75 6c64 2072 6563 6569 7665 2074 6865  ould receive the
-00008fb0: 2063 6f76 6572 6564 2077 6f72 6b20 6672   covered work fr
-00008fc0: 6f6d 2079 6f75 2c20 6120 6469 7363 7269  om you, a discri
-00008fd0: 6d69 6e61 746f 7279 0d0a 7061 7465 6e74  minatory..patent
-00008fe0: 206c 6963 656e 7365 2028 6129 2069 6e20   license (a) in 
-00008ff0: 636f 6e6e 6563 7469 6f6e 2077 6974 6820  connection with 
-00009000: 636f 7069 6573 206f 6620 7468 6520 636f  copies of the co
-00009010: 7665 7265 6420 776f 726b 0d0a 636f 6e76  vered work..conv
-00009020: 6579 6564 2062 7920 796f 7520 286f 7220  eyed by you (or 
-00009030: 636f 7069 6573 206d 6164 6520 6672 6f6d  copies made from
-00009040: 2074 686f 7365 2063 6f70 6965 7329 2c20   those copies), 
-00009050: 6f72 2028 6229 2070 7269 6d61 7269 6c79  or (b) primarily
-00009060: 0d0a 666f 7220 616e 6420 696e 2063 6f6e  ..for and in con
-00009070: 6e65 6374 696f 6e20 7769 7468 2073 7065  nection with spe
-00009080: 6369 6669 6320 7072 6f64 7563 7473 206f  cific products o
-00009090: 7220 636f 6d70 696c 6174 696f 6e73 2074  r compilations t
-000090a0: 6861 740d 0a63 6f6e 7461 696e 2074 6865  hat..contain the
-000090b0: 2063 6f76 6572 6564 2077 6f72 6b2c 2075   covered work, u
-000090c0: 6e6c 6573 7320 796f 7520 656e 7465 7265  nless you entere
-000090d0: 6420 696e 746f 2074 6861 7420 6172 7261  d into that arra
-000090e0: 6e67 656d 656e 742c 0d0a 6f72 2074 6861  ngement,..or tha
-000090f0: 7420 7061 7465 6e74 206c 6963 656e 7365  t patent license
-00009100: 2077 6173 2067 7261 6e74 6564 2c20 7072   was granted, pr
-00009110: 696f 7220 746f 2032 3820 4d61 7263 6820  ior to 28 March 
-00009120: 3230 3037 2e0d 0a0d 0a20 204e 6f74 6869  2007.....  Nothi
-00009130: 6e67 2069 6e20 7468 6973 204c 6963 656e  ng in this Licen
-00009140: 7365 2073 6861 6c6c 2062 6520 636f 6e73  se shall be cons
-00009150: 7472 7565 6420 6173 2065 7863 6c75 6469  trued as excludi
-00009160: 6e67 206f 7220 6c69 6d69 7469 6e67 0d0a  ng or limiting..
-00009170: 616e 7920 696d 706c 6965 6420 6c69 6365  any implied lice
-00009180: 6e73 6520 6f72 206f 7468 6572 2064 6566  nse or other def
-00009190: 656e 7365 7320 746f 2069 6e66 7269 6e67  enses to infring
-000091a0: 656d 656e 7420 7468 6174 206d 6179 0d0a  ement that may..
-000091b0: 6f74 6865 7277 6973 6520 6265 2061 7661  otherwise be ava
-000091c0: 696c 6162 6c65 2074 6f20 796f 7520 756e  ilable to you un
-000091d0: 6465 7220 6170 706c 6963 6162 6c65 2070  der applicable p
-000091e0: 6174 656e 7420 6c61 772e 0d0a 0d0a 2020  atent law.....  
-000091f0: 3132 2e20 4e6f 2053 7572 7265 6e64 6572  12. No Surrender
-00009200: 206f 6620 4f74 6865 7273 2720 4672 6565   of Others' Free
-00009210: 646f 6d2e 0d0a 0d0a 2020 4966 2063 6f6e  dom.....  If con
-00009220: 6469 7469 6f6e 7320 6172 6520 696d 706f  ditions are impo
-00009230: 7365 6420 6f6e 2079 6f75 2028 7768 6574  sed on you (whet
-00009240: 6865 7220 6279 2063 6f75 7274 206f 7264  her by court ord
-00009250: 6572 2c20 6167 7265 656d 656e 7420 6f72  er, agreement or
-00009260: 0d0a 6f74 6865 7277 6973 6529 2074 6861  ..otherwise) tha
-00009270: 7420 636f 6e74 7261 6469 6374 2074 6865  t contradict the
-00009280: 2063 6f6e 6469 7469 6f6e 7320 6f66 2074   conditions of t
-00009290: 6869 7320 4c69 6365 6e73 652c 2074 6865  his License, the
-000092a0: 7920 646f 206e 6f74 0d0a 6578 6375 7365  y do not..excuse
-000092b0: 2079 6f75 2066 726f 6d20 7468 6520 636f   you from the co
-000092c0: 6e64 6974 696f 6e73 206f 6620 7468 6973  nditions of this
-000092d0: 204c 6963 656e 7365 2e20 2049 6620 796f   License.  If yo
-000092e0: 7520 6361 6e6e 6f74 2063 6f6e 7665 7920  u cannot convey 
-000092f0: 610d 0a63 6f76 6572 6564 2077 6f72 6b20  a..covered work 
-00009300: 736f 2061 7320 746f 2073 6174 6973 6679  so as to satisfy
-00009310: 2073 696d 756c 7461 6e65 6f75 736c 7920   simultaneously 
-00009320: 796f 7572 206f 626c 6967 6174 696f 6e73  your obligations
-00009330: 2075 6e64 6572 2074 6869 730d 0a4c 6963   under this..Lic
-00009340: 656e 7365 2061 6e64 2061 6e79 206f 7468  ense and any oth
-00009350: 6572 2070 6572 7469 6e65 6e74 206f 626c  er pertinent obl
-00009360: 6967 6174 696f 6e73 2c20 7468 656e 2061  igations, then a
-00009370: 7320 6120 636f 6e73 6571 7565 6e63 6520  s a consequence 
-00009380: 796f 7520 6d61 790d 0a6e 6f74 2063 6f6e  you may..not con
-00009390: 7665 7920 6974 2061 7420 616c 6c2e 2020  vey it at all.  
-000093a0: 466f 7220 6578 616d 706c 652c 2069 6620  For example, if 
-000093b0: 796f 7520 6167 7265 6520 746f 2074 6572  you agree to ter
-000093c0: 6d73 2074 6861 7420 6f62 6c69 6761 7465  ms that obligate
-000093d0: 2079 6f75 0d0a 746f 2063 6f6c 6c65 6374   you..to collect
-000093e0: 2061 2072 6f79 616c 7479 2066 6f72 2066   a royalty for f
-000093f0: 7572 7468 6572 2063 6f6e 7665 7969 6e67  urther conveying
-00009400: 2066 726f 6d20 7468 6f73 6520 746f 2077   from those to w
-00009410: 686f 6d20 796f 7520 636f 6e76 6579 0d0a  hom you convey..
-00009420: 7468 6520 5072 6f67 7261 6d2c 2074 6865  the Program, the
-00009430: 206f 6e6c 7920 7761 7920 796f 7520 636f   only way you co
-00009440: 756c 6420 7361 7469 7366 7920 626f 7468  uld satisfy both
-00009450: 2074 686f 7365 2074 6572 6d73 2061 6e64   those terms and
-00009460: 2074 6869 730d 0a4c 6963 656e 7365 2077   this..License w
-00009470: 6f75 6c64 2062 6520 746f 2072 6566 7261  ould be to refra
-00009480: 696e 2065 6e74 6972 656c 7920 6672 6f6d  in entirely from
-00009490: 2063 6f6e 7665 7969 6e67 2074 6865 2050   conveying the P
-000094a0: 726f 6772 616d 2e0d 0a0d 0a20 2031 332e  rogram.....  13.
-000094b0: 2055 7365 2077 6974 6820 7468 6520 474e   Use with the GN
-000094c0: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
-000094d0: 2050 7562 6c69 6320 4c69 6365 6e73 652e   Public License.
-000094e0: 0d0a 0d0a 2020 4e6f 7477 6974 6873 7461  ....  Notwithsta
-000094f0: 6e64 696e 6720 616e 7920 6f74 6865 7220  nding any other 
-00009500: 7072 6f76 6973 696f 6e20 6f66 2074 6869  provision of thi
-00009510: 7320 4c69 6365 6e73 652c 2079 6f75 2068  s License, you h
-00009520: 6176 650d 0a70 6572 6d69 7373 696f 6e20  ave..permission 
-00009530: 746f 206c 696e 6b20 6f72 2063 6f6d 6269  to link or combi
-00009540: 6e65 2061 6e79 2063 6f76 6572 6564 2077  ne any covered w
-00009550: 6f72 6b20 7769 7468 2061 2077 6f72 6b20  ork with a work 
-00009560: 6c69 6365 6e73 6564 0d0a 756e 6465 7220  licensed..under 
-00009570: 7665 7273 696f 6e20 3320 6f66 2074 6865  version 3 of the
-00009580: 2047 4e55 2041 6666 6572 6f20 4765 6e65   GNU Affero Gene
-00009590: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
-000095a0: 7365 2069 6e74 6f20 6120 7369 6e67 6c65  se into a single
-000095b0: 0d0a 636f 6d62 696e 6564 2077 6f72 6b2c  ..combined work,
-000095c0: 2061 6e64 2074 6f20 636f 6e76 6579 2074   and to convey t
-000095d0: 6865 2072 6573 756c 7469 6e67 2077 6f72  he resulting wor
-000095e0: 6b2e 2020 5468 6520 7465 726d 7320 6f66  k.  The terms of
-000095f0: 2074 6869 730d 0a4c 6963 656e 7365 2077   this..License w
-00009600: 696c 6c20 636f 6e74 696e 7565 2074 6f20  ill continue to 
-00009610: 6170 706c 7920 746f 2074 6865 2070 6172  apply to the par
-00009620: 7420 7768 6963 6820 6973 2074 6865 2063  t which is the c
-00009630: 6f76 6572 6564 2077 6f72 6b2c 0d0a 6275  overed work,..bu
-00009640: 7420 7468 6520 7370 6563 6961 6c20 7265  t the special re
-00009650: 7175 6972 656d 656e 7473 206f 6620 7468  quirements of th
-00009660: 6520 474e 5520 4166 6665 726f 2047 656e  e GNU Affero Gen
-00009670: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00009680: 6e73 652c 0d0a 7365 6374 696f 6e20 3133  nse,..section 13
-00009690: 2c20 636f 6e63 6572 6e69 6e67 2069 6e74  , concerning int
-000096a0: 6572 6163 7469 6f6e 2074 6872 6f75 6768  eraction through
-000096b0: 2061 206e 6574 776f 726b 2077 696c 6c20   a network will 
-000096c0: 6170 706c 7920 746f 2074 6865 0d0a 636f  apply to the..co
-000096d0: 6d62 696e 6174 696f 6e20 6173 2073 7563  mbination as suc
-000096e0: 682e 0d0a 0d0a 2020 3134 2e20 5265 7669  h.....  14. Revi
-000096f0: 7365 6420 5665 7273 696f 6e73 206f 6620  sed Versions of 
-00009700: 7468 6973 204c 6963 656e 7365 2e0d 0a0d  this License....
-00009710: 0a20 2054 6865 2046 7265 6520 536f 6674  .  The Free Soft
-00009720: 7761 7265 2046 6f75 6e64 6174 696f 6e20  ware Foundation 
-00009730: 6d61 7920 7075 626c 6973 6820 7265 7669  may publish revi
-00009740: 7365 6420 616e 642f 6f72 206e 6577 2076  sed and/or new v
-00009750: 6572 7369 6f6e 7320 6f66 0d0a 7468 6520  ersions of..the 
-00009760: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-00009770: 6963 204c 6963 656e 7365 2066 726f 6d20  ic License from 
-00009780: 7469 6d65 2074 6f20 7469 6d65 2e20 2053  time to time.  S
-00009790: 7563 6820 6e65 7720 7665 7273 696f 6e73  uch new versions
-000097a0: 2077 696c 6c0d 0a62 6520 7369 6d69 6c61   will..be simila
-000097b0: 7220 696e 2073 7069 7269 7420 746f 2074  r in spirit to t
-000097c0: 6865 2070 7265 7365 6e74 2076 6572 7369  he present versi
-000097d0: 6f6e 2c20 6275 7420 6d61 7920 6469 6666  on, but may diff
-000097e0: 6572 2069 6e20 6465 7461 696c 2074 6f0d  er in detail to.
-000097f0: 0a61 6464 7265 7373 206e 6577 2070 726f  .address new pro
-00009800: 626c 656d 7320 6f72 2063 6f6e 6365 726e  blems or concern
-00009810: 732e 0d0a 0d0a 2020 4561 6368 2076 6572  s.....  Each ver
-00009820: 7369 6f6e 2069 7320 6769 7665 6e20 6120  sion is given a 
-00009830: 6469 7374 696e 6775 6973 6869 6e67 2076  distinguishing v
-00009840: 6572 7369 6f6e 206e 756d 6265 722e 2020  ersion number.  
-00009850: 4966 2074 6865 0d0a 5072 6f67 7261 6d20  If the..Program 
-00009860: 7370 6563 6966 6965 7320 7468 6174 2061  specifies that a
-00009870: 2063 6572 7461 696e 206e 756d 6265 7265   certain numbere
-00009880: 6420 7665 7273 696f 6e20 6f66 2074 6865  d version of the
-00009890: 2047 4e55 2047 656e 6572 616c 0d0a 5075   GNU General..Pu
-000098a0: 626c 6963 204c 6963 656e 7365 2022 6f72  blic License "or
-000098b0: 2061 6e79 206c 6174 6572 2076 6572 7369   any later versi
-000098c0: 6f6e 2220 6170 706c 6965 7320 746f 2069  on" applies to i
-000098d0: 742c 2079 6f75 2068 6176 6520 7468 650d  t, you have the.
-000098e0: 0a6f 7074 696f 6e20 6f66 2066 6f6c 6c6f  .option of follo
-000098f0: 7769 6e67 2074 6865 2074 6572 6d73 2061  wing the terms a
-00009900: 6e64 2063 6f6e 6469 7469 6f6e 7320 6569  nd conditions ei
-00009910: 7468 6572 206f 6620 7468 6174 206e 756d  ther of that num
-00009920: 6265 7265 640d 0a76 6572 7369 6f6e 206f  bered..version o
-00009930: 7220 6f66 2061 6e79 206c 6174 6572 2076  r of any later v
-00009940: 6572 7369 6f6e 2070 7562 6c69 7368 6564  ersion published
-00009950: 2062 7920 7468 6520 4672 6565 2053 6f66   by the Free Sof
-00009960: 7477 6172 650d 0a46 6f75 6e64 6174 696f  tware..Foundatio
-00009970: 6e2e 2020 4966 2074 6865 2050 726f 6772  n.  If the Progr
-00009980: 616d 2064 6f65 7320 6e6f 7420 7370 6563  am does not spec
-00009990: 6966 7920 6120 7665 7273 696f 6e20 6e75  ify a version nu
-000099a0: 6d62 6572 206f 6620 7468 650d 0a47 4e55  mber of the..GNU
-000099b0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-000099c0: 4c69 6365 6e73 652c 2079 6f75 206d 6179  License, you may
-000099d0: 2063 686f 6f73 6520 616e 7920 7665 7273   choose any vers
-000099e0: 696f 6e20 6576 6572 2070 7562 6c69 7368  ion ever publish
-000099f0: 6564 0d0a 6279 2074 6865 2046 7265 6520  ed..by the Free 
-00009a00: 536f 6674 7761 7265 2046 6f75 6e64 6174  Software Foundat
-00009a10: 696f 6e2e 0d0a 0d0a 2020 4966 2074 6865  ion.....  If the
-00009a20: 2050 726f 6772 616d 2073 7065 6369 6669   Program specifi
-00009a30: 6573 2074 6861 7420 6120 7072 6f78 7920  es that a proxy 
-00009a40: 6361 6e20 6465 6369 6465 2077 6869 6368  can decide which
-00009a50: 2066 7574 7572 650d 0a76 6572 7369 6f6e   future..version
-00009a60: 7320 6f66 2074 6865 2047 4e55 2047 656e  s of the GNU Gen
-00009a70: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00009a80: 6e73 6520 6361 6e20 6265 2075 7365 642c  nse can be used,
-00009a90: 2074 6861 7420 7072 6f78 7927 730d 0a70   that proxy's..p
-00009aa0: 7562 6c69 6320 7374 6174 656d 656e 7420  ublic statement 
-00009ab0: 6f66 2061 6363 6570 7461 6e63 6520 6f66  of acceptance of
-00009ac0: 2061 2076 6572 7369 6f6e 2070 6572 6d61   a version perma
-00009ad0: 6e65 6e74 6c79 2061 7574 686f 7269 7a65  nently authorize
-00009ae0: 7320 796f 750d 0a74 6f20 6368 6f6f 7365  s you..to choose
-00009af0: 2074 6861 7420 7665 7273 696f 6e20 666f   that version fo
-00009b00: 7220 7468 6520 5072 6f67 7261 6d2e 0d0a  r the Program...
-00009b10: 0d0a 2020 4c61 7465 7220 6c69 6365 6e73  ..  Later licens
-00009b20: 6520 7665 7273 696f 6e73 206d 6179 2067  e versions may g
-00009b30: 6976 6520 796f 7520 6164 6469 7469 6f6e  ive you addition
-00009b40: 616c 206f 7220 6469 6666 6572 656e 740d  al or different.
-00009b50: 0a70 6572 6d69 7373 696f 6e73 2e20 2048  .permissions.  H
-00009b60: 6f77 6576 6572 2c20 6e6f 2061 6464 6974  owever, no addit
-00009b70: 696f 6e61 6c20 6f62 6c69 6761 7469 6f6e  ional obligation
-00009b80: 7320 6172 6520 696d 706f 7365 6420 6f6e  s are imposed on
-00009b90: 2061 6e79 0d0a 6175 7468 6f72 206f 7220   any..author or 
-00009ba0: 636f 7079 7269 6768 7420 686f 6c64 6572  copyright holder
-00009bb0: 2061 7320 6120 7265 7375 6c74 206f 6620   as a result of 
-00009bc0: 796f 7572 2063 686f 6f73 696e 6720 746f  your choosing to
-00009bd0: 2066 6f6c 6c6f 7720 610d 0a6c 6174 6572   follow a..later
-00009be0: 2076 6572 7369 6f6e 2e0d 0a0d 0a20 2031   version.....  1
-00009bf0: 352e 2044 6973 636c 6169 6d65 7220 6f66  5. Disclaimer of
-00009c00: 2057 6172 7261 6e74 792e 0d0a 0d0a 2020   Warranty.....  
-00009c10: 5448 4552 4520 4953 204e 4f20 5741 5252  THERE IS NO WARR
-00009c20: 414e 5459 2046 4f52 2054 4845 2050 524f  ANTY FOR THE PRO
-00009c30: 4752 414d 2c20 544f 2054 4845 2045 5854  GRAM, TO THE EXT
-00009c40: 454e 5420 5045 524d 4954 5445 4420 4259  ENT PERMITTED BY
-00009c50: 0d0a 4150 504c 4943 4142 4c45 204c 4157  ..APPLICABLE LAW
-00009c60: 2e20 2045 5843 4550 5420 5748 454e 204f  .  EXCEPT WHEN O
-00009c70: 5448 4552 5749 5345 2053 5441 5445 4420  THERWISE STATED 
-00009c80: 494e 2057 5249 5449 4e47 2054 4845 2043  IN WRITING THE C
-00009c90: 4f50 5952 4947 4854 0d0a 484f 4c44 4552  OPYRIGHT..HOLDER
-00009ca0: 5320 414e 442f 4f52 204f 5448 4552 2050  S AND/OR OTHER P
-00009cb0: 4152 5449 4553 2050 524f 5649 4445 2054  ARTIES PROVIDE T
-00009cc0: 4845 2050 524f 4752 414d 2022 4153 2049  HE PROGRAM "AS I
-00009cd0: 5322 2057 4954 484f 5554 2057 4152 5241  S" WITHOUT WARRA
-00009ce0: 4e54 590d 0a4f 4620 414e 5920 4b49 4e44  NTY..OF ANY KIND
-00009cf0: 2c20 4549 5448 4552 2045 5850 5245 5353  , EITHER EXPRESS
-00009d00: 4544 204f 5220 494d 504c 4945 442c 2049  ED OR IMPLIED, I
-00009d10: 4e43 4c55 4449 4e47 2c20 4255 5420 4e4f  NCLUDING, BUT NO
-00009d20: 5420 4c49 4d49 5445 4420 544f 2c0d 0a54  T LIMITED TO,..T
-00009d30: 4845 2049 4d50 4c49 4544 2057 4152 5241  HE IMPLIED WARRA
-00009d40: 4e54 4945 5320 4f46 204d 4552 4348 414e  NTIES OF MERCHAN
-00009d50: 5441 4249 4c49 5459 2041 4e44 2046 4954  TABILITY AND FIT
-00009d60: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-00009d70: 4355 4c41 520d 0a50 5552 504f 5345 2e20  CULAR..PURPOSE. 
-00009d80: 2054 4845 2045 4e54 4952 4520 5249 534b   THE ENTIRE RISK
-00009d90: 2041 5320 544f 2054 4845 2051 5541 4c49   AS TO THE QUALI
-00009da0: 5459 2041 4e44 2050 4552 464f 524d 414e  TY AND PERFORMAN
-00009db0: 4345 204f 4620 5448 4520 5052 4f47 5241  CE OF THE PROGRA
-00009dc0: 4d0d 0a49 5320 5749 5448 2059 4f55 2e20  M..IS WITH YOU. 
-00009dd0: 2053 484f 554c 4420 5448 4520 5052 4f47   SHOULD THE PROG
-00009de0: 5241 4d20 5052 4f56 4520 4445 4645 4354  RAM PROVE DEFECT
-00009df0: 4956 452c 2059 4f55 2041 5353 554d 4520  IVE, YOU ASSUME 
-00009e00: 5448 4520 434f 5354 204f 460d 0a41 4c4c  THE COST OF..ALL
-00009e10: 204e 4543 4553 5341 5259 2053 4552 5649   NECESSARY SERVI
-00009e20: 4349 4e47 2c20 5245 5041 4952 204f 5220  CING, REPAIR OR 
-00009e30: 434f 5252 4543 5449 4f4e 2e0d 0a0d 0a20  CORRECTION..... 
-00009e40: 2031 362e 204c 696d 6974 6174 696f 6e20   16. Limitation 
-00009e50: 6f66 204c 6961 6269 6c69 7479 2e0d 0a0d  of Liability....
-00009e60: 0a20 2049 4e20 4e4f 2045 5645 4e54 2055  .  IN NO EVENT U
-00009e70: 4e4c 4553 5320 5245 5155 4952 4544 2042  NLESS REQUIRED B
-00009e80: 5920 4150 504c 4943 4142 4c45 204c 4157  Y APPLICABLE LAW
-00009e90: 204f 5220 4147 5245 4544 2054 4f20 494e   OR AGREED TO IN
-00009ea0: 2057 5249 5449 4e47 0d0a 5749 4c4c 2041   WRITING..WILL A
-00009eb0: 4e59 2043 4f50 5952 4947 4854 2048 4f4c  NY COPYRIGHT HOL
-00009ec0: 4445 522c 204f 5220 414e 5920 4f54 4845  DER, OR ANY OTHE
-00009ed0: 5220 5041 5254 5920 5748 4f20 4d4f 4449  R PARTY WHO MODI
-00009ee0: 4649 4553 2041 4e44 2f4f 5220 434f 4e56  FIES AND/OR CONV
-00009ef0: 4559 530d 0a54 4845 2050 524f 4752 414d  EYS..THE PROGRAM
-00009f00: 2041 5320 5045 524d 4954 5445 4420 4142   AS PERMITTED AB
-00009f10: 4f56 452c 2042 4520 4c49 4142 4c45 2054  OVE, BE LIABLE T
-00009f20: 4f20 594f 5520 464f 5220 4441 4d41 4745  O YOU FOR DAMAGE
-00009f30: 532c 2049 4e43 4c55 4449 4e47 2041 4e59  S, INCLUDING ANY
-00009f40: 0d0a 4745 4e45 5241 4c2c 2053 5045 4349  ..GENERAL, SPECI
-00009f50: 414c 2c20 494e 4349 4445 4e54 414c 204f  AL, INCIDENTAL O
-00009f60: 5220 434f 4e53 4551 5545 4e54 4941 4c20  R CONSEQUENTIAL 
-00009f70: 4441 4d41 4745 5320 4152 4953 494e 4720  DAMAGES ARISING 
-00009f80: 4f55 5420 4f46 2054 4845 0d0a 5553 4520  OUT OF THE..USE 
-00009f90: 4f52 2049 4e41 4249 4c49 5459 2054 4f20  OR INABILITY TO 
-00009fa0: 5553 4520 5448 4520 5052 4f47 5241 4d20  USE THE PROGRAM 
-00009fb0: 2849 4e43 4c55 4449 4e47 2042 5554 204e  (INCLUDING BUT N
-00009fc0: 4f54 204c 494d 4954 4544 2054 4f20 4c4f  OT LIMITED TO LO
-00009fd0: 5353 204f 460d 0a44 4154 4120 4f52 2044  SS OF..DATA OR D
-00009fe0: 4154 4120 4245 494e 4720 5245 4e44 4552  ATA BEING RENDER
-00009ff0: 4544 2049 4e41 4343 5552 4154 4520 4f52  ED INACCURATE OR
-0000a000: 204c 4f53 5345 5320 5355 5354 4149 4e45   LOSSES SUSTAINE
-0000a010: 4420 4259 2059 4f55 204f 5220 5448 4952  D BY YOU OR THIR
-0000a020: 440d 0a50 4152 5449 4553 204f 5220 4120  D..PARTIES OR A 
-0000a030: 4641 494c 5552 4520 4f46 2054 4845 2050  FAILURE OF THE P
-0000a040: 524f 4752 414d 2054 4f20 4f50 4552 4154  ROGRAM TO OPERAT
-0000a050: 4520 5749 5448 2041 4e59 204f 5448 4552  E WITH ANY OTHER
-0000a060: 2050 524f 4752 414d 5329 2c0d 0a45 5645   PROGRAMS),..EVE
-0000a070: 4e20 4946 2053 5543 4820 484f 4c44 4552  N IF SUCH HOLDER
-0000a080: 204f 5220 4f54 4845 5220 5041 5254 5920   OR OTHER PARTY 
-0000a090: 4841 5320 4245 454e 2041 4456 4953 4544  HAS BEEN ADVISED
-0000a0a0: 204f 4620 5448 4520 504f 5353 4942 494c   OF THE POSSIBIL
-0000a0b0: 4954 5920 4f46 0d0a 5355 4348 2044 414d  ITY OF..SUCH DAM
-0000a0c0: 4147 4553 2e0d 0a0d 0a20 2031 372e 2049  AGES.....  17. I
-0000a0d0: 6e74 6572 7072 6574 6174 696f 6e20 6f66  nterpretation of
-0000a0e0: 2053 6563 7469 6f6e 7320 3135 2061 6e64   Sections 15 and
-0000a0f0: 2031 362e 0d0a 0d0a 2020 4966 2074 6865   16.....  If the
-0000a100: 2064 6973 636c 6169 6d65 7220 6f66 2077   disclaimer of w
-0000a110: 6172 7261 6e74 7920 616e 6420 6c69 6d69  arranty and limi
-0000a120: 7461 7469 6f6e 206f 6620 6c69 6162 696c  tation of liabil
-0000a130: 6974 7920 7072 6f76 6964 6564 0d0a 6162  ity provided..ab
-0000a140: 6f76 6520 6361 6e6e 6f74 2062 6520 6769  ove cannot be gi
-0000a150: 7665 6e20 6c6f 6361 6c20 6c65 6761 6c20  ven local legal 
-0000a160: 6566 6665 6374 2061 6363 6f72 6469 6e67  effect according
-0000a170: 2074 6f20 7468 6569 7220 7465 726d 732c   to their terms,
-0000a180: 0d0a 7265 7669 6577 696e 6720 636f 7572  ..reviewing cour
-0000a190: 7473 2073 6861 6c6c 2061 7070 6c79 206c  ts shall apply l
-0000a1a0: 6f63 616c 206c 6177 2074 6861 7420 6d6f  ocal law that mo
-0000a1b0: 7374 2063 6c6f 7365 6c79 2061 7070 726f  st closely appro
-0000a1c0: 7869 6d61 7465 730d 0a61 6e20 6162 736f  ximates..an abso
-0000a1d0: 6c75 7465 2077 6169 7665 7220 6f66 2061  lute waiver of a
-0000a1e0: 6c6c 2063 6976 696c 206c 6961 6269 6c69  ll civil liabili
-0000a1f0: 7479 2069 6e20 636f 6e6e 6563 7469 6f6e  ty in connection
-0000a200: 2077 6974 6820 7468 650d 0a50 726f 6772   with the..Progr
-0000a210: 616d 2c20 756e 6c65 7373 2061 2077 6172  am, unless a war
-0000a220: 7261 6e74 7920 6f72 2061 7373 756d 7074  ranty or assumpt
-0000a230: 696f 6e20 6f66 206c 6961 6269 6c69 7479  ion of liability
-0000a240: 2061 6363 6f6d 7061 6e69 6573 2061 0d0a   accompanies a..
-0000a250: 636f 7079 206f 6620 7468 6520 5072 6f67  copy of the Prog
-0000a260: 7261 6d20 696e 2072 6574 7572 6e20 666f  ram in return fo
-0000a270: 7220 6120 6665 652e 0d0a 0d0a 2020 2020  r a fee.....    
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2045 4e44 204f 4620 5445 524d 5320 414e   END OF TERMS AN
-0000a2a0: 4420 434f 4e44 4954 494f 4e53 0d0a 0d0a  D CONDITIONS....
-0000a2b0: 2020 2020 2020 2020 2020 2020 486f 7720              How 
-0000a2c0: 746f 2041 7070 6c79 2054 6865 7365 2054  to Apply These T
-0000a2d0: 6572 6d73 2074 6f20 596f 7572 204e 6577  erms to Your New
-0000a2e0: 2050 726f 6772 616d 730d 0a0d 0a20 2049   Programs....  I
-0000a2f0: 6620 796f 7520 6465 7665 6c6f 7020 6120  f you develop a 
-0000a300: 6e65 7720 7072 6f67 7261 6d2c 2061 6e64  new program, and
-0000a310: 2079 6f75 2077 616e 7420 6974 2074 6f20   you want it to 
-0000a320: 6265 206f 6620 7468 6520 6772 6561 7465  be of the greate
-0000a330: 7374 0d0a 706f 7373 6962 6c65 2075 7365  st..possible use
-0000a340: 2074 6f20 7468 6520 7075 626c 6963 2c20   to the public, 
-0000a350: 7468 6520 6265 7374 2077 6179 2074 6f20  the best way to 
-0000a360: 6163 6869 6576 6520 7468 6973 2069 7320  achieve this is 
-0000a370: 746f 206d 616b 6520 6974 0d0a 6672 6565  to make it..free
-0000a380: 2073 6f66 7477 6172 6520 7768 6963 6820   software which 
-0000a390: 6576 6572 796f 6e65 2063 616e 2072 6564  everyone can red
-0000a3a0: 6973 7472 6962 7574 6520 616e 6420 6368  istribute and ch
-0000a3b0: 616e 6765 2075 6e64 6572 2074 6865 7365  ange under these
-0000a3c0: 2074 6572 6d73 2e0d 0a0d 0a20 2054 6f20   terms.....  To 
-0000a3d0: 646f 2073 6f2c 2061 7474 6163 6820 7468  do so, attach th
-0000a3e0: 6520 666f 6c6c 6f77 696e 6720 6e6f 7469  e following noti
-0000a3f0: 6365 7320 746f 2074 6865 2070 726f 6772  ces to the progr
-0000a400: 616d 2e20 2049 7420 6973 2073 6166 6573  am.  It is safes
-0000a410: 740d 0a74 6f20 6174 7461 6368 2074 6865  t..to attach the
-0000a420: 6d20 746f 2074 6865 2073 7461 7274 206f  m to the start o
-0000a430: 6620 6561 6368 2073 6f75 7263 6520 6669  f each source fi
-0000a440: 6c65 2074 6f20 6d6f 7374 2065 6666 6563  le to most effec
-0000a450: 7469 7665 6c79 0d0a 7374 6174 6520 7468  tively..state th
-0000a460: 6520 6578 636c 7573 696f 6e20 6f66 2077  e exclusion of w
-0000a470: 6172 7261 6e74 793b 2061 6e64 2065 6163  arranty; and eac
-0000a480: 6820 6669 6c65 2073 686f 756c 6420 6861  h file should ha
-0000a490: 7665 2061 7420 6c65 6173 740d 0a74 6865  ve at least..the
-0000a4a0: 2022 636f 7079 7269 6768 7422 206c 696e   "copyright" lin
-0000a4b0: 6520 616e 6420 6120 706f 696e 7465 7220  e and a pointer 
-0000a4c0: 746f 2077 6865 7265 2074 6865 2066 756c  to where the ful
-0000a4d0: 6c20 6e6f 7469 6365 2069 7320 666f 756e  l notice is foun
-0000a4e0: 642e 0d0a 0d0a 2020 2020 3c6f 6e65 206c  d.....    <one l
-0000a4f0: 696e 6520 746f 2067 6976 6520 7468 6520  ine to give the 
-0000a500: 7072 6f67 7261 6d27 7320 6e61 6d65 2061  program's name a
-0000a510: 6e64 2061 2062 7269 6566 2069 6465 6120  nd a brief idea 
-0000a520: 6f66 2077 6861 7420 6974 2064 6f65 732e  of what it does.
-0000a530: 3e0d 0a20 2020 2043 6f70 7972 6967 6874  >..    Copyright
-0000a540: 2028 4329 203c 7965 6172 3e20 203c 6e61   (C) <year>  <na
-0000a550: 6d65 206f 6620 6175 7468 6f72 3e0d 0a0d  me of author>...
-0000a560: 0a20 2020 2054 6869 7320 7072 6f67 7261  .    This progra
-0000a570: 6d20 6973 2066 7265 6520 736f 6674 7761  m is free softwa
-0000a580: 7265 3a20 796f 7520 6361 6e20 7265 6469  re: you can redi
-0000a590: 7374 7269 6275 7465 2069 7420 616e 642f  stribute it and/
-0000a5a0: 6f72 206d 6f64 6966 790d 0a20 2020 2069  or modify..    i
-0000a5b0: 7420 756e 6465 7220 7468 6520 7465 726d  t under the term
-0000a5c0: 7320 6f66 2074 6865 2047 4e55 2047 656e  s of the GNU Gen
-0000a5d0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-0000a5e0: 6e73 6520 6173 2070 7562 6c69 7368 6564  nse as published
-0000a5f0: 2062 790d 0a20 2020 2074 6865 2046 7265   by..    the Fre
-0000a600: 6520 536f 6674 7761 7265 2046 6f75 6e64  e Software Found
-0000a610: 6174 696f 6e2c 2065 6974 6865 7220 7665  ation, either ve
-0000a620: 7273 696f 6e20 3320 6f66 2074 6865 204c  rsion 3 of the L
-0000a630: 6963 656e 7365 2c20 6f72 0d0a 2020 2020  icense, or..    
-0000a640: 2861 7420 796f 7572 206f 7074 696f 6e29  (at your option)
-0000a650: 2061 6e79 206c 6174 6572 2076 6572 7369   any later versi
-0000a660: 6f6e 2e0d 0a0d 0a20 2020 2054 6869 7320  on.....    This 
-0000a670: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
-0000a680: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
-0000a690: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
-0000a6a0: 6265 2075 7365 6675 6c2c 0d0a 2020 2020  be useful,..    
-0000a6b0: 6275 7420 5749 5448 4f55 5420 414e 5920  but WITHOUT ANY 
-0000a6c0: 5741 5252 414e 5459 3b20 7769 7468 6f75  WARRANTY; withou
-0000a6d0: 7420 6576 656e 2074 6865 2069 6d70 6c69  t even the impli
-0000a6e0: 6564 2077 6172 7261 6e74 7920 6f66 0d0a  ed warranty of..
-0000a6f0: 2020 2020 4d45 5243 4841 4e54 4142 494c      MERCHANTABIL
-0000a700: 4954 5920 6f72 2046 4954 4e45 5353 2046  ITY or FITNESS F
-0000a710: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
-0000a720: 5055 5250 4f53 452e 2020 5365 6520 7468  PURPOSE.  See th
-0000a730: 650d 0a20 2020 2047 4e55 2047 656e 6572  e..    GNU Gener
-0000a740: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-0000a750: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
-0000a760: 6c73 2e0d 0a0d 0a20 2020 2059 6f75 2073  ls.....    You s
-0000a770: 686f 756c 6420 6861 7665 2072 6563 6569  hould have recei
-0000a780: 7665 6420 6120 636f 7079 206f 6620 7468  ved a copy of th
-0000a790: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
-0000a7a0: 626c 6963 204c 6963 656e 7365 0d0a 2020  blic License..  
-0000a7b0: 2020 616c 6f6e 6720 7769 7468 2074 6869    along with thi
-0000a7c0: 7320 7072 6f67 7261 6d2e 2020 4966 206e  s program.  If n
-0000a7d0: 6f74 2c20 7365 6520 3c68 7474 7073 3a2f  ot, see <https:/
-0000a7e0: 2f77 7777 2e67 6e75 2e6f 7267 2f6c 6963  /www.gnu.org/lic
-0000a7f0: 656e 7365 732f 3e2e 0d0a 0d0a 416c 736f  enses/>.....Also
-0000a800: 2061 6464 2069 6e66 6f72 6d61 7469 6f6e   add information
-0000a810: 206f 6e20 686f 7720 746f 2063 6f6e 7461   on how to conta
-0000a820: 6374 2079 6f75 2062 7920 656c 6563 7472  ct you by electr
-0000a830: 6f6e 6963 2061 6e64 2070 6170 6572 206d  onic and paper m
-0000a840: 6169 6c2e 0d0a 0d0a 2020 4966 2074 6865  ail.....  If the
-0000a850: 2070 726f 6772 616d 2064 6f65 7320 7465   program does te
-0000a860: 726d 696e 616c 2069 6e74 6572 6163 7469  rminal interacti
-0000a870: 6f6e 2c20 6d61 6b65 2069 7420 6f75 7470  on, make it outp
-0000a880: 7574 2061 2073 686f 7274 0d0a 6e6f 7469  ut a short..noti
-0000a890: 6365 206c 696b 6520 7468 6973 2077 6865  ce like this whe
-0000a8a0: 6e20 6974 2073 7461 7274 7320 696e 2061  n it starts in a
-0000a8b0: 6e20 696e 7465 7261 6374 6976 6520 6d6f  n interactive mo
-0000a8c0: 6465 3a0d 0a0d 0a20 2020 203c 7072 6f67  de:....    <prog
-0000a8d0: 7261 6d3e 2020 436f 7079 7269 6768 7420  ram>  Copyright 
-0000a8e0: 2843 2920 3c79 6561 723e 2020 3c6e 616d  (C) <year>  <nam
-0000a8f0: 6520 6f66 2061 7574 686f 723e 0d0a 2020  e of author>..  
-0000a900: 2020 5468 6973 2070 726f 6772 616d 2063    This program c
-0000a910: 6f6d 6573 2077 6974 6820 4142 534f 4c55  omes with ABSOLU
-0000a920: 5445 4c59 204e 4f20 5741 5252 414e 5459  TELY NO WARRANTY
-0000a930: 3b20 666f 7220 6465 7461 696c 7320 7479  ; for details ty
-0000a940: 7065 2060 7368 6f77 2077 272e 0d0a 2020  pe `show w'...  
-0000a950: 2020 5468 6973 2069 7320 6672 6565 2073    This is free s
-0000a960: 6f66 7477 6172 652c 2061 6e64 2079 6f75  oftware, and you
-0000a970: 2061 7265 2077 656c 636f 6d65 2074 6f20   are welcome to 
-0000a980: 7265 6469 7374 7269 6275 7465 2069 740d  redistribute it.
-0000a990: 0a20 2020 2075 6e64 6572 2063 6572 7461  .    under certa
-0000a9a0: 696e 2063 6f6e 6469 7469 6f6e 733b 2074  in conditions; t
-0000a9b0: 7970 6520 6073 686f 7720 6327 2066 6f72  ype `show c' for
-0000a9c0: 2064 6574 6169 6c73 2e0d 0a0d 0a54 6865   details.....The
-0000a9d0: 2068 7970 6f74 6865 7469 6361 6c20 636f   hypothetical co
-0000a9e0: 6d6d 616e 6473 2060 7368 6f77 2077 2720  mmands `show w' 
-0000a9f0: 616e 6420 6073 686f 7720 6327 2073 686f  and `show c' sho
-0000aa00: 756c 6420 7368 6f77 2074 6865 2061 7070  uld show the app
-0000aa10: 726f 7072 6961 7465 0d0a 7061 7274 7320  ropriate..parts 
-0000aa20: 6f66 2074 6865 2047 656e 6572 616c 2050  of the General P
-0000aa30: 7562 6c69 6320 4c69 6365 6e73 652e 2020  ublic License.  
-0000aa40: 4f66 2063 6f75 7273 652c 2079 6f75 7220  Of course, your 
-0000aa50: 7072 6f67 7261 6d27 7320 636f 6d6d 616e  program's comman
-0000aa60: 6473 0d0a 6d69 6768 7420 6265 2064 6966  ds..might be dif
-0000aa70: 6665 7265 6e74 3b20 666f 7220 6120 4755  ferent; for a GU
-0000aa80: 4920 696e 7465 7266 6163 652c 2079 6f75  I interface, you
-0000aa90: 2077 6f75 6c64 2075 7365 2061 6e20 2261   would use an "a
-0000aaa0: 626f 7574 2062 6f78 222e 0d0a 0d0a 2020  bout box".....  
-0000aab0: 596f 7520 7368 6f75 6c64 2061 6c73 6f20  You should also 
-0000aac0: 6765 7420 796f 7572 2065 6d70 6c6f 7965  get your employe
-0000aad0: 7220 2869 6620 796f 7520 776f 726b 2061  r (if you work a
-0000aae0: 7320 6120 7072 6f67 7261 6d6d 6572 2920  s a programmer) 
-0000aaf0: 6f72 2073 6368 6f6f 6c2c 0d0a 6966 2061  or school,..if a
-0000ab00: 6e79 2c20 746f 2073 6967 6e20 6120 2263  ny, to sign a "c
-0000ab10: 6f70 7972 6967 6874 2064 6973 636c 6169  opyright disclai
-0000ab20: 6d65 7222 2066 6f72 2074 6865 2070 726f  mer" for the pro
-0000ab30: 6772 616d 2c20 6966 206e 6563 6573 7361  gram, if necessa
-0000ab40: 7279 2e0d 0a46 6f72 206d 6f72 6520 696e  ry...For more in
-0000ab50: 666f 726d 6174 696f 6e20 6f6e 2074 6869  formation on thi
-0000ab60: 732c 2061 6e64 2068 6f77 2074 6f20 6170  s, and how to ap
-0000ab70: 706c 7920 616e 6420 666f 6c6c 6f77 2074  ply and follow t
-0000ab80: 6865 2047 4e55 2047 504c 2c20 7365 650d  he GNU GPL, see.
-0000ab90: 0a3c 6874 7470 733a 2f2f 7777 772e 676e  .<https://www.gn
-0000aba0: 752e 6f72 672f 6c69 6365 6e73 6573 2f3e  u.org/licenses/>
-0000abb0: 2e0d 0a0d 0a20 2054 6865 2047 4e55 2047  .....  The GNU G
-0000abc0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-0000abd0: 6365 6e73 6520 646f 6573 206e 6f74 2070  cense does not p
-0000abe0: 6572 6d69 7420 696e 636f 7270 6f72 6174  ermit incorporat
-0000abf0: 696e 6720 796f 7572 2070 726f 6772 616d  ing your program
-0000ac00: 0d0a 696e 746f 2070 726f 7072 6965 7461  ..into proprieta
-0000ac10: 7279 2070 726f 6772 616d 732e 2020 4966  ry programs.  If
-0000ac20: 2079 6f75 7220 7072 6f67 7261 6d20 6973   your program is
-0000ac30: 2061 2073 7562 726f 7574 696e 6520 6c69   a subroutine li
-0000ac40: 6272 6172 792c 2079 6f75 0d0a 6d61 7920  brary, you..may 
-0000ac50: 636f 6e73 6964 6572 2069 7420 6d6f 7265  consider it more
-0000ac60: 2075 7365 6675 6c20 746f 2070 6572 6d69   useful to permi
-0000ac70: 7420 6c69 6e6b 696e 6720 7072 6f70 7269  t linking propri
-0000ac80: 6574 6172 7920 6170 706c 6963 6174 696f  etary applicatio
-0000ac90: 6e73 2077 6974 680d 0a74 6865 206c 6962  ns with..the lib
-0000aca0: 7261 7279 2e20 2049 6620 7468 6973 2069  rary.  If this i
-0000acb0: 7320 7768 6174 2079 6f75 2077 616e 7420  s what you want 
-0000acc0: 746f 2064 6f2c 2075 7365 2074 6865 2047  to do, use the G
-0000acd0: 4e55 204c 6573 7365 7220 4765 6e65 7261  NU Lesser Genera
-0000ace0: 6c0d 0a50 7562 6c69 6320 4c69 6365 6e73  l..Public Licens
-0000acf0: 6520 696e 7374 6561 6420 6f66 2074 6869  e instead of thi
-0000ad00: 7320 4c69 6365 6e73 652e 2020 4275 7420  s License.  But 
-0000ad10: 6669 7273 742c 2070 6c65 6173 6520 7265  first, please re
-0000ad20: 6164 0d0a 3c68 7474 7073 3a2f 2f77 7777  ad..<https://www
-0000ad30: 2e67 6e75 2e6f 7267 2f6c 6963 656e 7365  .gnu.org/license
-0000ad40: 732f 7768 792d 6e6f 742d 6c67 706c 2e68  s/why-not-lgpl.h
-0000ad50: 746d 6c3e 2e0d 0a                        tml>...
+00000380: 204c 4943 454e 5345 2e6d 640d 0a0d 0a3c   LICENSE.md....<
+00000390: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
+000003a0: 223e 6f73 6d5f 6561 7379 5f61 7069 3c2f  ">osm_easy_api</
+000003b0: 6831 3e0d 0a3c 7020 616c 6967 6e3d 2263  h1>..<p align="c
+000003c0: 656e 7465 7222 3e0d 0a20 203c 696d 6720  enter">..  <img 
+000003d0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+000003e0: 6875 622e 636f 6d2f 646f 6365 6e74 5954  hub.com/docentYT
+000003f0: 2f61 7574 6f6d 6174 6564 2d70 7974 686f  /automated-pytho
+00000400: 6e2d 7465 7374 732d 7465 7374 696e 672d  n-tests-testing-
+00000410: 7265 706f 2f61 6374 696f 6e73 2f77 6f72  repo/actions/wor
+00000420: 6b66 6c6f 7773 2f74 6573 7473 2e79 616d  kflows/tests.yam
+00000430: 6c2f 6261 6467 652e 7376 6722 202f 3e0d  l/badge.svg" />.
+00000440: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
+00000450: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000460: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00000470: 6f63 656e 7459 542f 6f73 6d5f 6561 7379  ocentYT/osm_easy
+00000480: 5f61 7069 2f33 3838 3961 6536 3236 6265  _api/3889ae626be
+00000490: 3335 3138 3332 3533 3438 3536 3436 6237  35183253485646b7
+000004a0: 6265 3965 3233 3561 3266 6332 372f 636f  be9e235a2fc27/co
+000004b0: 7665 7261 6765 2d62 6164 6765 2e73 7667  verage-badge.svg
+000004c0: 2220 2f3e 0d0a 2020 3c61 2068 7265 663d  " />..  <a href=
+000004d0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+000004e0: 672f 7072 6f6a 6563 742f 6f73 6d2d 6561  g/project/osm-ea
+000004f0: 7379 2d61 7069 2f22 3e0d 0a20 2020 203c  sy-api/">..    <
+00000500: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000510: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000520: 7079 7069 2f76 2f6f 736d 5f65 6173 795f  pypi/v/osm_easy_
+00000530: 6170 6922 202f 3e0d 0a20 203c 2f61 3e0d  api" />..  </a>.
+00000540: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000550: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000560: 6a65 6374 2f6f 736d 2d65 6173 792d 6170  ject/osm-easy-ap
+00000570: 692f 223e 0d0a 2020 2020 3c69 6d67 2073  i/">..    <img s
+00000580: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000590: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000005a0: 646d 2f6f 736d 5f65 6173 795f 6170 6922  dm/osm_easy_api"
+000005b0: 2061 6c74 3d22 7079 7069 2064 6f77 6e6c   alt="pypi downl
+000005c0: 6f61 6473 223e 0d0a 2020 3c2f 613e 0d0a  oads">..  </a>..
+000005d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000005e0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000005f0: 6563 742f 6f73 6d2d 6561 7379 2d61 7069  ect/osm-easy-api
+00000600: 2f22 3e0d 0a20 2020 203c 696d 6720 616c  /">..    <img al
+00000610: 743d 2270 7974 686f 6e20 7665 7273 696f  t="python versio
+00000620: 6e73 2220 7372 633d 2268 7474 7073 3a2f  ns" src="https:/
+00000630: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000640: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000650: 6f73 6d5f 6561 7379 5f61 7069 2220 7461  osm_easy_api" ta
+00000660: 7267 6574 3d22 5f62 6c61 6e6b 2220 2f3e  rget="_blank" />
+00000670: 0d0a 2020 3c2f 613e 0d0a 3c2f 703e 0d0a  ..  </a>..</p>..
+00000680: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000690: 6572 223e 3c61 2068 7265 663d 2268 7474  er"><a href="htt
+000006a0: 7073 3a2f 2f77 7777 2e6f 7065 6e73 7472  ps://www.openstr
+000006b0: 6565 746d 6170 2e6f 7267 2f75 7365 722f  eetmap.org/user/
+000006c0: 6b77 6961 7465 6b5f 3132 3329 223e 4d65  kwiatek_123)">Me
+000006d0: 206f 6e20 4f70 656e 5374 7265 6574 4d61   on OpenStreetMa
+000006e0: 703c 2f61 3e3c 2f70 3e0d 0a0d 0a50 7974  p</a></p>....Pyt
+000006f0: 686f 6e20 7061 636b 6167 6520 666f 7220  hon package for 
+00000700: 7061 7273 696e 6720 6f73 6d20 6469 6666  parsing osm diff
+00000710: 7320 616e 6420 636f 6d6d 756e 6963 6174  s and communicat
+00000720: 696e 6720 7769 7468 2074 6865 204f 7065  ing with the Ope
+00000730: 6e53 7472 6565 744d 6170 2061 7069 2e20  nStreetMap api. 
+00000740: 5365 6520 4150 492e 7478 7420 666f 7220  See API.txt for 
+00000750: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
+00000760: 6420 656e 6470 6f69 6e74 732e 0d0a 0d0a  d endpoints.....
+00000770: 2323 2057 6861 7427 7320 7468 6520 706f  ## What's the po
+00000780: 696e 7420 6f66 2074 6869 7320 7061 636b  int of this pack
+00000790: 6167 653f 0d0a 0d0a 5468 6973 2070 6163  age?....This pac
+000007a0: 6b61 6765 2077 6173 2063 7265 6174 6564  kage was created
+000007b0: 2074 6f20 7072 6f76 6964 6520 616e 2065   to provide an e
+000007c0: 6173 7920 7761 7920 746f 2063 7265 6174  asy way to creat
+000007d0: 6520 6175 746f 6d61 7465 6420 7363 7269  e automated scri
+000007e0: 7074 7320 616e 6420 7072 6f67 7261 6d73  pts and programs
+000007f0: 2074 6861 7420 7573 6520 6469 6666 2061   that use diff a
+00000800: 6e64 2f6f 7220 6f73 6d20 6170 692e 2054  nd/or osm api. T
+00000810: 6865 206d 6169 6e20 6164 7661 6e74 6167  he main advantag
+00000820: 6520 6973 2074 6865 2063 6c61 7373 6573  e is the classes
+00000830: 2028 6461 7461 5f63 6c61 7373 6573 2920   (data_classes) 
+00000840: 7468 6174 2070 726f 7669 6465 2064 6174  that provide dat
+00000850: 6120 6f66 2065 6c65 6d65 6e74 7320 286e  a of elements (n
+00000860: 6f64 652c 2077 6179 2c20 7265 6c61 7469  ode, way, relati
+00000870: 6f6e 2c20 4f73 6d43 6861 6e67 652c 2065  on, OsmChange, e
+00000880: 7463 2e29 2069 6e20 6120 7265 6164 6162  tc.) in a readab
+00000890: 6c65 2077 6179 2061 6e64 2074 6865 2070  le way and the p
+000008a0: 6f73 7369 6269 6c69 7479 2074 6f20 7573  ossibility to us
+000008b0: 6520 7468 656d 2069 6e20 6469 6666 2061  e them in diff a
+000008c0: 6e64 2061 7069 2077 6974 686f 7574 2077  nd api without w
+000008d0: 6f72 7279 696e 6720 6162 6f75 7420 6d69  orrying about mi
+000008e0: 7373 696e 6720 6461 7461 206f 7220 6469  ssing data or di
+000008f0: 6374 696f 6e61 7269 6573 2e20 596f 7520  ctionaries. You 
+00000900: 6361 6e20 6561 7369 6c79 2066 696e 6420  can easily find 
+00000910: 6e6f 6465 7320 696e 2064 6966 662c 2061  nodes in diff, a
+00000920: 6464 2061 2074 6167 2074 6f20 7468 656d  dd a tag to them
+00000930: 2061 6e64 2073 656e 6420 7468 6520 636f   and send the co
+00000940: 7272 6563 7465 6420 7665 7273 696f 6e20  rrected version 
+00000950: 746f 206f 736d 2e0d 0a0d 0a23 2320 5768  to osm.....## Wh
+00000960: 6174 206e 6578 743f 0d0a 5468 6520 706c  at next?..The pl
+00000970: 616e 2069 7320 746f 206f 7074 696d 6973  an is to optimis
+00000980: 6520 616e 6420 696d 7072 6f76 6520 7468  e and improve th
+00000990: 6520 636f 6465 2c20 6164 6420 7375 7070  e code, add supp
+000009a0: 6f72 7420 666f 7220 6770 7820 7472 6163  ort for gpx trac
+000009b0: 6573 2c20 7273 7320 7375 7070 6f72 7420  es, rss support 
+000009c0: 616e 6420 6f76 6572 7061 7373 2061 7069  and overpass api
+000009d0: 2e0d 0a0d 0a23 2049 6e73 7461 6c6c 6174  .....# Installat
+000009e0: 696f 6e0d 0a0d 0a57 6f72 6b73 206f 6e20  ion....Works on 
+000009f0: 7079 7468 6f6e 203e 3d20 332e 3130 2e20  python >= 3.10. 
+00000a00: 2844 7565 2074 6f20 6e65 7720 7479 7065  (Due to new type
+00000a10: 6869 6e74 7320 7374 616e 6461 7264 290d  hints standard).
+00000a20: 0a0d 0a49 6e73 7461 6c6c 2060 6f73 6d5f  ...Install `osm_
+00000a30: 6561 7379 5f61 7069 6020 6672 6f6d 205b  easy_api` from [
+00000a40: 5079 5069 5d28 6874 7470 733a 2f2f 7079  PyPi](https://py
+00000a50: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6f  pi.org/project/o
+00000a60: 736d 2d65 6173 792d 6170 692f 293a 0d0a  sm-easy-api/):..
+00000a70: 6060 600d 0a70 6970 2069 6e73 7461 6c6c  ```..pip install
+00000a80: 206f 736d 5f65 6173 795f 6170 690d 0a60   osm_easy_api..`
+00000a90: 6060 200d 0a0d 0a23 2044 6f63 756d 656e  `` ....# Documen
+00000aa0: 7461 7469 6f6e 0d0a 0d0a 596f 7520 6361  tation....You ca
+00000ab0: 6e20 7669 6577 2064 6f63 756d 656e 7461  n view documenta
+00000ac0: 7469 6f6e 206f 6e20 5b67 6974 6875 622d  tion on [github-
+00000ad0: 7061 6765 735d 2868 7474 7073 3a2f 2f64  pages](https://d
+00000ae0: 6f63 656e 7479 742e 6769 7468 7562 2e69  ocentyt.github.i
+00000af0: 6f2f 6f73 6d5f 6561 7379 5f61 7069 2f6f  o/osm_easy_api/o
+00000b00: 736d 5f65 6173 795f 6170 692e 6874 6d6c  sm_easy_api.html
+00000b10: 292e 0d0a 0d0a 446f 6375 6d65 6e74 6174  ).....Documentat
+00000b20: 696f 6e20 6973 2062 7569 6c64 2075 7369  ion is build usi
+00000b30: 6e67 205b 7064 6f63 5d28 6874 7470 733a  ng [pdoc](https:
+00000b40: 2f2f 7064 6f63 2e64 6576 292e 0d0a 546f  //pdoc.dev)...To
+00000b50: 2072 756e 2064 6f63 7320 6f6e 2079 6f75   run docs on you
+00000b60: 7220 6d61 6368 696e 6520 7573 6520 7072  r machine use pr
+00000b70: 6566 6572 7265 6420 636f 6d6d 616e 643a  eferred command:
+00000b80: 2060 7064 6f63 202d 2d64 6f63 666f 726d   `pdoc --docform
+00000b90: 6174 2067 6f6f 676c 6520 2d2d 6e6f 2d73  at google --no-s
+00000ba0: 686f 772d 736f 7572 6365 206f 736d 5f65  how-source osm_e
+00000bb0: 6173 795f 6170 6920 216f 736d 5f65 6173  asy_api !osm_eas
+00000bc0: 795f 6170 692e 7574 696c 7360 2e0d 0a0d  y_api.utils`....
+00000bd0: 0a23 2045 7861 6d70 6c65 730d 0a0d 0a23  .# Examples....#
+00000be0: 2320 4449 4646 0d0a 0d0a 2323 2320 5072  # DIFF....### Pr
+00000bf0: 696e 7420 7472 6565 730d 0a0d 0a60 6060  int trees....```
+00000c00: 7079 0d0a 6672 6f6d 206f 736d 5f65 6173  py..from osm_eas
+00000c10: 795f 6170 6920 696d 706f 7274 204e 6f64  y_api import Nod
+00000c20: 652c 2044 6966 662c 2046 7265 7175 656e  e, Diff, Frequen
+00000c30: 6379 0d0a 0d0a 2320 446f 776e 6c6f 6164  cy....# Download
+00000c40: 2064 6966 6620 6672 6f6d 206c 6173 7420   diff from last 
+00000c50: 686f 7572 2e0d 0a64 203d 2044 6966 6628  hour...d = Diff(
+00000c60: 4672 6571 7565 6e63 792e 484f 5552 290d  Frequency.HOUR).
+00000c70: 0a0d 0a23 2047 6574 204d 6574 6120 6e61  ...# Get Meta na
+00000c80: 6d65 6474 7570 6c65 2066 6f72 2064 6966  medtuple for dif
+00000c90: 6620 6d65 7461 6461 7461 2061 6e64 2067  f metadata and g
+00000ca0: 656e 6572 6174 6f72 2074 6861 7420 7061  enerator that pa
+00000cb0: 7273 6520 6469 6666 2066 696c 652e 0d0a  rse diff file...
+00000cc0: 6d65 7461 2c20 6765 6e20 3d20 642e 6765  meta, gen = d.ge
+00000cd0: 7428 7461 6773 3d22 6e61 7475 7261 6c22  t(tags="natural"
+00000ce0: 290d 0a0d 0a23 2050 7269 6e74 2061 6c6c  )....# Print all
+00000cf0: 2063 7265 6174 6564 2c20 6d6f 6469 6669   created, modifi
+00000d00: 6564 2061 6e64 2064 656c 6574 6564 204e  ed and deleted N
+00000d10: 6f64 6573 2077 6974 6820 6e61 7475 7261  odes with natura
+00000d20: 6c3d 7472 6565 2074 6167 2e0d 0a66 6f72  l=tree tag...for
+00000d30: 2061 6374 696f 6e2c 2065 6c65 6d65 6e74   action, element
+00000d40: 2069 6e20 6765 6e3a 0d0a 2020 2020 6966   in gen:..    if
+00000d50: 2074 7970 6528 656c 656d 656e 7429 203d   type(element) =
+00000d60: 3d20 4e6f 6465 2061 6e64 2065 6c65 6d65  = Node and eleme
+00000d70: 6e74 2e74 6167 732e 6765 7428 226e 6174  nt.tags.get("nat
+00000d80: 7572 616c 2229 203d 3d20 2274 7265 6522  ural") == "tree"
+00000d90: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00000da0: 2861 6374 696f 6e2c 2065 6c65 6d65 6e74  (action, element
+00000db0: 2e69 6429 0d0a 6060 600d 0a0d 0a23 2323  .id)..```....###
+00000dc0: 2050 7269 6e74 2069 6e63 6f72 7265 6374   Print incorrect
+00000dd0: 6c79 2074 6167 6765 6420 7369 6e67 6c65  ly tagged single
+00000de0: 2074 7265 7373 0d0a 0d0a 6060 6070 790d   tress....```py.
+00000df0: 0a66 726f 6d20 6f73 6d5f 6561 7379 5f61  .from osm_easy_a
+00000e00: 7069 2069 6d70 6f72 7420 4469 6666 2c20  pi import Diff, 
+00000e10: 4672 6571 7565 6e63 792c 2041 6374 696f  Frequency, Actio
+00000e20: 6e2c 204e 6f64 650d 0a0d 0a64 203d 2044  n, Node....d = D
+00000e30: 6966 6628 4672 6571 7565 6e63 792e 4441  iff(Frequency.DA
+00000e40: 5929 0d0a 0d0a 6d65 7461 2c20 6765 6e20  Y)....meta, gen 
+00000e50: 3d20 642e 6765 7428 7461 6773 3d22 6e61  = d.get(tags="na
+00000e60: 7475 7261 6c22 290d 0a0d 0a66 6f72 2061  tural")....for a
+00000e70: 6374 696f 6e2c 2065 6c65 6d65 6e74 2069  ction, element i
+00000e80: 6e20 6765 6e3a 0d0a 2020 2020 6966 2074  n gen:..    if t
+00000e90: 7970 6528 656c 656d 656e 7429 203d 3d20  ype(element) == 
+00000ea0: 4e6f 6465 3a0d 0a20 2020 2020 2020 2069  Node:..        i
+00000eb0: 6620 6163 7469 6f6e 203d 3d20 4163 7469  f action == Acti
+00000ec0: 6f6e 2e43 5245 4154 4520 6f72 2061 6374  on.CREATE or act
+00000ed0: 696f 6e20 3d3d 2041 6374 696f 6e2e 4d4f  ion == Action.MO
+00000ee0: 4449 4659 3a0d 0a20 2020 2020 2020 2020  DIFY:..         
+00000ef0: 2020 2069 6620 656c 656d 656e 742e 7461     if element.ta
+00000f00: 6773 2e67 6574 2822 6e61 7475 7261 6c22  gs.get("natural"
+00000f10: 2920 3d3d 2022 776f 6f64 223a 0d0a 2020  ) == "wood":..  
+00000f20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00000f30: 696e 7428 656c 656d 656e 7429 0d0a 6060  int(element)..``
+00000f40: 600d 0a45 7861 6d70 6c65 206f 7574 7075  `..Example outpu
+00000f50: 743a 0d0a 6060 600d 0a4e 6f64 6528 6964  t:..```..Node(id
+00000f60: 203d 2031 3032 3038 3438 3637 3137 2c20   = 10208486717, 
+00000f70: 7669 7369 626c 6520 3d20 4e6f 6e65 2c20  visible = None, 
+00000f80: 7665 7273 696f 6e20 3d20 312c 2063 6861  version = 1, cha
+00000f90: 6e67 6573 6574 5f69 6420 3d20 3132 3932  ngeset_id = 1292
+00000fa0: 3136 3037 352c 2074 696d 6573 7461 6d70  16075, timestamp
+00000fb0: 203d 2032 3032 322d 3131 2d32 3254 3030   = 2022-11-22T00
+00000fc0: 3a31 363a 3434 5a2c 2075 7365 725f 6964  :16:44Z, user_id
+00000fd0: 203d 2031 3734 3731 3732 312c 2074 6167   = 17471721, tag
+00000fe0: 7320 3d20 7b27 6c65 6166 5f74 7970 6527  s = {'leaf_type'
+00000ff0: 3a20 2762 726f 6164 6c65 6176 6564 272c  : 'broadleaved',
+00001000: 2027 6e61 7475 7261 6c27 3a20 2777 6f6f   'natural': 'woo
+00001010: 6427 7d2c 206c 6174 6974 7564 6520 3d20  d'}, latitude = 
+00001020: 3438 2e36 3532 3232 3836 2c20 6c6f 6e67  48.6522286, long
+00001030: 6974 7564 6520 3d20 3132 2e35 3833 3830  itude = 12.58380
+00001040: 392c 2029 0d0a 6060 600d 0a0d 0a23 2320  9, )..```....## 
+00001050: 4150 490d 0a0d 0a23 2323 2041 6464 206d  API....### Add m
+00001060: 6973 7369 6e67 2077 696b 6964 6174 6120  issing wikidata 
+00001070: 7461 670d 0a0d 0a60 6060 7079 0d0a 6672  tag....```py..fr
+00001080: 6f6d 206f 736d 5f65 6173 795f 6170 6920  om osm_easy_api 
+00001090: 696d 706f 7274 2041 7069 2c20 4e6f 6465  import Api, Node
+000010a0: 2c20 5461 6773 0d0a 0d0a 6170 6920 3d20  , Tags....api = 
+000010b0: 4170 6928 2268 7474 7073 3a2f 2f6d 6173  Api("https://mas
+000010c0: 7465 722e 6170 6973 2e64 6576 2e6f 7065  ter.apis.dev.ope
+000010d0: 6e73 7472 6565 746d 6170 2e6f 7267 222c  nstreetmap.org",
+000010e0: 204c 4f47 494e 2c20 5041 5353 574f 5244   LOGIN, PASSWORD
+000010f0: 290d 0a0d 0a6e 6f64 6520 3d20 6170 692e  )....node = api.
+00001100: 656c 656d 656e 7473 2e67 6574 284e 6f64  elements.get(Nod
+00001110: 652c 2034 3239 3634 3630 3333 3629 2023  e, 4296460336) #
+00001120: 2057 6520 6172 6520 6765 7474 696e 6720   We are getting 
+00001130: 4e6f 6465 2077 6974 6820 6964 2034 3239  Node with id 429
+00001140: 3634 3630 3333 3620 7768 6572 6520 7765  6460336 where we
+00001150: 2077 616e 7420 746f 2061 6464 2061 206e   want to add a n
+00001160: 6577 2074 6167 2074 6f0d 0a6e 6f64 652e  ew tag to..node.
+00001170: 7461 6773 2e61 6464 2822 7769 6b69 6461  tags.add("wikida
+00001180: 7461 222c 2022 5165 7861 6d70 6c65 2229  ta", "Qexample")
+00001190: 2023 2041 6464 2061 206e 6577 2074 6167   # Add a new tag
+000011a0: 2074 6f20 6e6f 6465 2e0d 0a0d 0a6d 795f   to node.....my_
+000011b0: 6368 616e 6765 7365 7420 3d20 6170 692e  changeset = api.
+000011c0: 6368 616e 6765 7365 742e 6372 6561 7465  changeset.create
+000011d0: 2822 4164 6420 6d69 7373 696e 6720 7769  ("Add missing wi
+000011e0: 6b69 6461 7461 2074 6167 222c 2054 6167  kidata tag", Tag
+000011f0: 7328 7b22 6175 746f 6d61 7469 6322 3a20  s({"automatic": 
+00001200: 2279 6573 227d 2929 2023 2043 7265 6174  "yes"})) # Creat
+00001210: 6520 6e65 7720 6368 616e 6765 7365 7420  e new changeset 
+00001220: 7769 7468 2064 6573 6372 6970 7469 6f6e  with description
+00001230: 2061 6e64 2074 6167 0d0a 6170 692e 656c   and tag..api.el
+00001240: 656d 656e 7473 2e75 7064 6174 6528 6e6f  ements.update(no
+00001250: 6465 2c20 6d79 5f63 6861 6e67 6573 6574  de, my_changeset
+00001260: 2920 2320 5365 6e64 206e 6577 2076 6572  ) # Send new ver
+00001270: 7369 6f6e 206f 6620 6120 6e6f 6465 2074  sion of a node t
+00001280: 6f20 6f73 6d0d 0a61 7069 2e63 6861 6e67  o osm..api.chang
+00001290: 6573 6574 2e63 6c6f 7365 286d 795f 6368  eset.close(my_ch
+000012a0: 616e 6765 7365 7429 2023 2043 6c6f 7365  angeset) # Close
+000012b0: 2063 6861 6e67 6573 6574 2e0d 0a60 6060   changeset...```
+000012c0: 0d0a 0d0a 2320 4e6f 7465 730d 0a0d 0a4e  ....# Notes....N
+000012d0: 6f74 6520 7468 6174 2074 6865 2066 6f6c  ote that the fol
+000012e0: 6c6f 7769 6e67 2063 6f64 6573 2064 6f20  lowing codes do 
+000012f0: 7468 6520 7361 6d65 2074 6869 6e67 0d0a  the same thing..
+00001300: 6060 6070 790d 0a66 726f 6d20 6f73 6d5f  ```py..from osm_
+00001310: 6561 7379 5f61 7069 2069 6d70 6f72 7420  easy_api import 
+00001320: 4469 6666 2c20 4672 6571 7565 6e63 790d  Diff, Frequency.
+00001330: 0a0d 0a64 203d 2044 6966 6628 4672 6571  ...d = Diff(Freq
+00001340: 7565 6e63 792e 4441 5929 0d0a 0d0a 6d65  uency.DAY)....me
+00001350: 7461 2c20 6765 6e20 3d20 642e 6765 7428  ta, gen = d.get(
+00001360: 290d 0a0d 0a66 6f72 2061 6374 696f 6e2c  )....for action,
+00001370: 2065 6c65 6d65 6e74 2069 6e20 6765 6e3a   element in gen:
+00001380: 0d0a 2020 2020 6966 2065 6c65 6d65 6e74  ..    if element
+00001390: 2e74 6167 732e 6765 7428 2273 686f 7022  .tags.get("shop"
+000013a0: 2920 3d3d 2022 636f 6e76 656e 6965 6e63  ) == "convenienc
+000013b0: 6522 3a0d 0a20 2020 2020 2020 2070 7269  e":..        pri
+000013c0: 6e74 2865 6c65 6d65 6e74 290d 0a60 6060  nt(element)..```
+000013d0: 0d0a 6060 6070 790d 0a66 726f 6d20 6f73  ..```py..from os
+000013e0: 6d5f 6561 7379 5f61 7069 2069 6d70 6f72  m_easy_api impor
+000013f0: 7420 4469 6666 2c20 4672 6571 7565 6e63  t Diff, Frequenc
+00001400: 792c 2054 6167 730d 0a0d 0a64 203d 2044  y, Tags....d = D
+00001410: 6966 6628 4672 6571 7565 6e63 792e 4441  iff(Frequency.DA
+00001420: 5929 0d0a 0d0a 6d65 7461 2c20 6765 6e20  Y)....meta, gen 
+00001430: 3d20 642e 6765 7428 7461 6773 3d54 6167  = d.get(tags=Tag
+00001440: 7328 7b22 7368 6f70 223a 2022 636f 6e76  s({"shop": "conv
+00001450: 656e 6965 6e63 6522 7d29 290d 0a0d 0a66  enience"}))....f
+00001460: 6f72 2061 6374 696f 6e2c 2065 6c65 6d65  or action, eleme
+00001470: 6e74 2069 6e20 6765 6e3a 0d0a 2020 2020  nt in gen:..    
+00001480: 2020 2020 7072 696e 7428 656c 656d 656e      print(elemen
+00001490: 7429 0d0a 6060 600d 0a62 7574 2074 6865  t)..```..but the
+000014a0: 2073 6563 6f6e 6420 7365 656d 7320 746f   second seems to
+000014b0: 2062 6520 6661 7374 6572 2e0d 0a0d 0a41   be faster.....A
+000014c0: 6c73 6f20 796f 7520 6361 6e20 7573 6520  lso you can use 
+000014d0: 4f73 6d43 6861 6e67 6520 6f62 6a65 6374  OsmChange object
+000014e0: 2069 6620 796f 7520 646f 6e27 7420 7761   if you don't wa
+000014f0: 6e74 2074 6f20 7573 6520 6765 6e65 7261  nt to use genera
+00001500: 746f 720d 0a60 6060 7079 0d0a 6672 6f6d  tor..```py..from
+00001510: 206f 736d 5f65 6173 795f 6170 6920 696d   osm_easy_api im
+00001520: 706f 7274 2044 6966 662c 2046 7265 7175  port Diff, Frequ
+00001530: 656e 6379 2c20 4163 7469 6f6e 2c20 4e6f  ency, Action, No
+00001540: 6465 0d0a 0d0a 6420 3d20 4469 6666 2846  de....d = Diff(F
+00001550: 7265 7175 656e 6379 2e4d 494e 5554 4529  requency.MINUTE)
+00001560: 0d0a 0d0a 6f73 6d43 6861 6e67 6520 3d20  ....osmChange = 
+00001570: 642e 6765 7428 6765 6e65 7261 746f 723d  d.get(generator=
+00001580: 4661 6c73 6529 0d0a 0d0a 6465 6c65 7465  False)....delete
+00001590: 645f 6e6f 6465 7320 3d20 6f73 6d43 6861  d_nodes = osmCha
+000015a0: 6e67 652e 6765 7428 4e6f 6465 2c20 4163  nge.get(Node, Ac
+000015b0: 7469 6f6e 2e44 454c 4554 4529 0d0a 666f  tion.DELETE)..fo
+000015c0: 7220 6e6f 6465 2069 6e20 6465 6c65 7465  r node in delete
+000015d0: 645f 6e6f 6465 733a 0d0a 2020 2020 7072  d_nodes:..    pr
+000015e0: 696e 7428 6e6f 6465 2e69 6429 0d0a 6060  int(node.id)..``
+000015f0: 600d 0a62 7574 2069 7420 6361 6e20 636f  `..but it can co
+00001600: 6e73 756d 6520 6c61 7267 6520 616d 6f75  nsume large amou
+00001610: 6e74 7320 6f66 2072 616d 2061 6e64 2075  nts of ram and u
+00001620: 7365 206f 6620 7468 6973 206d 6574 686f  se of this metho
+00001630: 6420 6973 206e 6f74 2072 6563 6f6d 6d65  d is not recomme
+00001640: 6e64 6564 2066 6f72 206c 6172 6765 2064  nded for large d
+00001650: 6966 6627 732e 0d0a 0d0a 2320 5465 7374  iff's.....# Test
+00001660: 730d 0a0d 0a59 6f75 2077 696c 6c20 6e65  s....You will ne
+00001670: 6564 2074 6f20 696e 7374 616c 6c20 6074  ed to install `t
+00001680: 6573 742d 7265 7175 6972 656d 656e 7473  est-requirements
+00001690: 2e74 7874 602e 2059 6f75 2063 616e 2075  .txt`. You can u
+000016a0: 7365 2074 6f78 2e0d 0a54 6f20 7275 6e20  se tox...To run 
+000016b0: 7465 7374 7320 6d61 6e75 616c 6c79 2075  tests manually u
+000016c0: 7365 2060 7079 7468 6f6e 202d 6d20 756e  se `python -m un
+000016d0: 6974 7465 7374 2064 6973 636f 7665 7260  ittest discover`
+000016e0: 2e0d 0a23 2043 6861 6e67 656c 6f67 0d0a  ...# Changelog..
+000016f0: 0d0a 416c 6c20 6e6f 7461 626c 6520 6368  ..All notable ch
+00001700: 616e 6765 7320 746f 2074 6869 7320 7072  anges to this pr
+00001710: 6f6a 6563 7420 7769 6c6c 2062 6520 646f  oject will be do
+00001720: 6375 6d65 6e74 6564 2069 6e20 7468 6973  cumented in this
+00001730: 2066 696c 652e 0d0a 0d0a 5468 6520 666f   file.....The fo
+00001740: 726d 6174 2069 7320 6261 7365 6420 6f6e  rmat is based on
+00001750: 205b 4b65 6570 2061 2043 6861 6e67 656c   [Keep a Changel
+00001760: 6f67 5d28 6874 7470 733a 2f2f 6b65 6570  og](https://keep
+00001770: 6163 6861 6e67 656c 6f67 2e63 6f6d 2f65  achangelog.com/e
+00001780: 6e2f 312e 302e 302f 292c 0d0a 616e 6420  n/1.0.0/),..and 
+00001790: 7468 6973 2070 726f 6a65 6374 2061 6468  this project adh
+000017a0: 6572 6573 2074 6f20 5b53 656d 616e 7469  eres to [Semanti
+000017b0: 6320 5665 7273 696f 6e69 6e67 5d28 6874  c Versioning](ht
+000017c0: 7470 733a 2f2f 7365 6d76 6572 2e6f 7267  tps://semver.org
+000017d0: 2f73 7065 632f 7632 2e30 2e30 2e68 746d  /spec/v2.0.0.htm
+000017e0: 6c29 2e0d 0a0d 0a23 2320 5b31 2e30 2e30  l).....## [1.0.0
+000017f0: 5d0d 0a23 2323 2041 6464 6564 0d0a 2d20  ]..### Added..- 
+00001800: 6074 6f5f 786d 6c28 2960 206d 6574 686f  `to_xml()` metho
+00001810: 6420 696e 2060 4f73 6d43 6861 6e67 6560  d in `OsmChange`
+00001820: 2e0d 0a2d 2060 7570 6c6f 6164 2829 6020  ...- `upload()` 
+00001830: 6d65 7468 6f64 2069 6e20 6063 6861 6e67  method in `chang
+00001840: 6573 6574 6020 6065 6e64 706f 696e 7460  eset` `endpoint`
+00001850: 2068 6173 206e 6577 206f 7074 696f 6e61   has new optiona
+00001860: 6c20 6172 6775 6d65 6e74 732e 0d0a 2d20  l arguments...- 
+00001870: 5465 7374 2066 6f72 2060 746f 5f78 6d6c  Test for `to_xml
+00001880: 2829 6020 6d65 7468 6f64 2069 6e20 604f  ()` method in `O
+00001890: 736d 4368 616e 6765 602e 0d0a 2d20 6023  smChange`...- `#
+000018a0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+000018b0: 7260 2066 6f72 2075 6e65 7870 6563 7465  r` for unexpecte
+000018c0: 6420 6170 6920 6572 726f 7273 2028 5468  d api errors (Th
+000018d0: 6f73 6520 7468 6174 2061 7265 206e 6f74  ose that are not
+000018e0: 2069 6e20 7468 6520 7370 6563 6966 6963   in the specific
+000018f0: 6174 696f 6e20 6f6e 2074 6865 2077 696b  ation on the wik
+00001900: 6929 2e0d 0a0d 0a23 2323 2043 6861 6e67  i).....### Chang
+00001910: 6564 0d0a 2d20 5072 6976 6174 6520 605f  ed..- Private `_
+00001920: 746f 5f78 6d6c 2829 6020 6d65 7468 6f64  to_xml()` method
+00001930: 2069 6e20 604f 736d 4368 616e 6765 6020   in `OsmChange` 
+00001940: 6973 206e 6f77 2073 7461 7469 632e 0d0a  is now static...
+00001950: 0d0a 2323 205b 302e 342e 325d 0d0a 0d0a  ..## [0.4.2]....
+00001960: 2323 2320 4368 616e 6765 640d 0a2d 204f  ### Changed..- O
+00001970: 7264 6572 206f 6620 656c 656d 656e 7473  rder of elements
+00001980: 2069 6e20 786d 6c20 6765 6e65 7261 7465   in xml generate
+00001990: 6420 6279 2060 5761 792e 5f74 6f5f 786d  d by `Way._to_xm
+000019a0: 6c28 2960 2e20 4669 7273 7420 7461 6773  l()`. First tags
+000019b0: 2c20 7468 656e 206e 6f64 6573 2e0d 0a0d  , then nodes....
+000019c0: 0a23 2323 2046 6978 6564 0d0a 2d20 6052  .### Fixed..- `R
+000019d0: 656c 6174 696f 6e2e 5f74 6f5f 786d 6c28  elation._to_xml(
+000019e0: 2960 2077 6173 2072 6574 7572 6e69 6e67  )` was returning
+000019f0: 2061 6e20 786d 6c20 7769 7468 6f75 7420   an xml without 
+00001a00: 6f73 6d20 7461 6773 2e0d 0a2d 2044 656c  osm tags...- Del
+00001a10: 6574 6564 2064 6973 7573 6564 2076 6172  eted disused var
+00001a20: 6961 626c 6520 696e 2060 4e6f 6465 2e5f  iable in `Node._
+00001a30: 746f 5f78 6d6c 2829 602e 0d0a 2d20 4669  to_xml()`...- Fi
+00001a40: 7865 6420 696e 636f 7272 6563 7420 7265  xed incorrect re
+00001a50: 6c61 7469 6f6e 2070 6172 7369 6e67 206f  lation parsing o
+00001a60: 6620 6461 7461 2072 6563 6976 6564 2062  f data recived b
+00001a70: 7920 6066 756c 6c60 2065 6e64 706f 696e  y `full` endpoin
+00001a80: 742e 0d0a 0d0a 2323 205b 302e 342e 315d  t.....## [0.4.1]
+00001a90: 0d0a 2323 2320 4368 616e 6765 640d 0a2d  ..### Changed..-
+00001aa0: 2055 7064 6174 6564 2060 7265 7175 6573   Updated `reques
+00001ab0: 7473 6020 6672 6f6d 2060 322e 3238 2e31  ts` from `2.28.1
+00001ac0: 6020 746f 2060 322e 3331 2e30 602e 0d0a  ` to `2.31.0`...
+00001ad0: 0d0a 2323 205b 302e 342e 305d 0d0a 2323  ..## [0.4.0]..##
+00001ae0: 2320 4164 6465 640d 0a2d 2060 746f 5f64  # Added..- `to_d
+00001af0: 6963 7428 2960 206d 6574 686f 6420 616e  ict()` method an
+00001b00: 6420 6066 726f 6d5f 6469 6374 2829 6020  d `from_dict()` 
+00001b10: 636c 6173 7320 6d65 7468 6f64 2074 6f20  class method to 
+00001b20: 604e 6f74 6560 2e20 200d 0a2d 2060 746f  `Note`.  ..- `to
+00001b30: 5f64 6963 7428 2960 206d 6574 686f 6420  _dict()` method 
+00001b40: 616e 6420 6066 726f 6d5f 6469 6374 2829  and `from_dict()
+00001b50: 6020 636c 6173 7320 6d65 7468 6f64 2074  ` class method t
+00001b60: 6f20 6043 6f6d 6d65 6e74 602e 0d0a 2d20  o `Comment`...- 
+00001b70: 6074 6f5f 6469 6374 2829 6020 6d65 7468  `to_dict()` meth
+00001b80: 6f64 2061 6e64 2060 6672 6f6d 5f64 6963  od and `from_dic
+00001b90: 7428 2960 2063 6c61 7373 206d 6574 686f  t()` class metho
+00001ba0: 6420 746f 2060 5573 6572 602e 0d0a 2d20  d to `User`...- 
+00001bb0: 446f 6375 6d65 6e74 6174 696f 6e20 6162  Documentation ab
+00001bc0: 6f75 7420 604d 6574 6160 2061 6e64 2060  out `Meta` and `
+00001bd0: 4163 7469 6f6e 6020 636c 6173 732e 0d0a  Action` class...
+00001be0: 2d20 4173 7365 7274 2065 7272 6f72 2028  - Assert error (
+00001bf0: 7769 7468 2069 6e66 6f72 6d61 7469 6f6e  with information
+00001c00: 2074 6f20 7265 706f 7274 2069 7420 6f6e   to report it on
+00001c10: 2067 6974 6875 6229 2077 6865 6e20 6170   github) when ap
+00001c20: 6920 7265 7475 726e 7320 616e 2065 7272  i returns an err
+00001c30: 6f72 2063 6f64 6520 6e6f 7420 6465 7363  or code not desc
+00001c40: 7269 6265 6420 6f6e 2074 6865 2077 696b  ribed on the wik
+00001c50: 692e 0d0a 2d20 6074 6f5f 6469 6374 2829  i...- `to_dict()
+00001c60: 6020 6d65 7468 6f64 2061 6e64 2060 6672  ` method and `fr
+00001c70: 6f6d 5f64 6963 7428 2960 2063 6c61 7373  om_dict()` class
+00001c80: 206d 6574 686f 6420 746f 2060 2872 656c   method to `(rel
+00001c90: 6174 696f 6e29 204d 656d 6265 7260 2e0d  ation) Member`..
+00001ca0: 0a0d 0a23 2323 2046 6978 6564 0d0a 2d20  ...### Fixed..- 
+00001cb0: 604e 6f74 6560 2063 616e 206e 6f77 2062  `Note` can now b
+00001cc0: 6520 696d 706f 7274 6564 2066 726f 6d20  e imported from 
+00001cd0: 7061 636b 6167 652e 0d0a 2d20 6043 6f6d  package...- `Com
+00001ce0: 6d65 6e74 6020 6361 6e20 6e6f 7720 6265  ment` can now be
+00001cf0: 2069 6d70 6f72 7465 6420 6672 6f6d 2070   imported from p
+00001d00: 6163 6b61 6765 2e0d 0a2d 2060 5573 6572  ackage...- `User
+00001d10: 6020 6361 6e20 6e6f 7720 6265 2069 6d70  ` can now be imp
+00001d20: 6f72 7465 6420 6672 6f6d 2070 6163 6b61  orted from packa
+00001d30: 6765 2e0d 0a2d 2060 4d65 6d62 6572 6020  ge...- `Member` 
+00001d40: 6361 6e20 6e6f 7720 6265 2069 6d70 6f72  can now be impor
+00001d50: 7465 6420 6672 6f6d 2070 6163 6b61 6765  ted from package
+00001d60: 2e0d 0a2d 2050 646f 6320 636f 6d6d 616e  ...- Pdoc comman
+00001d70: 6420 696e 2060 5245 4144 4d45 2e6d 6460  d in `README.md`
+00001d80: 2e0d 0a2d 2060 5265 6c61 7469 6f6e 2e74  ...- `Relation.t
+00001d90: 6f5f 6469 6374 2829 6020 6d65 7468 6f64  o_dict()` method
+00001da0: 206e 6f77 2072 6563 7572 7369 7665 6c79   now recursively
+00001db0: 2073 6572 6961 6c69 7365 7320 6d65 6d62   serialises memb
+00001dc0: 6572 732e 0d0a 2d20 6057 6179 2e74 6f5f  ers...- `Way.to_
+00001dd0: 6469 6374 2829 6020 6d65 7468 6f64 206e  dict()` method n
+00001de0: 6f77 2072 6563 7572 7369 7665 6c79 2073  ow recursively s
+00001df0: 6572 6961 6c69 7365 7320 6e6f 6465 732e  erialises nodes.
+00001e00: 0d0a 0d0a 2323 2320 4368 616e 6765 640d  ....### Changed.
+00001e10: 0a2d 2043 6861 6e67 6564 2069 6d70 6f72  .- Changed impor
+00001e20: 7473 2069 6e20 6052 656c 6174 696f 6e2e  ts in `Relation.
+00001e30: 7079 6020 746f 2075 7365 2069 6d70 6f72  py` to use impor
+00001e40: 7469 6e67 2074 6872 6f75 6768 2061 206d  ting through a m
+00001e50: 6f64 756c 6520 7261 7468 6572 2074 6861  odule rather tha
+00001e60: 6e20 6469 7265 6374 6c79 2066 726f 6d20  n directly from 
+00001e70: 6120 6669 6c65 2e0d 0a2d 2041 6464 6564  a file...- Added
+00001e80: 2060 7361 6d70 6c65 5f64 6174 6163 6c61   `sample_datacla
+00001e90: 7373 6573 2e70 7960 2066 696c 6520 696e  sses.py` file in
+00001ea0: 2074 6573 7473 2066 6978 7475 7265 7320   tests fixtures 
+00001eb0: 746f 2072 6564 7563 6520 636f 6465 2064  to reduce code d
+00001ec0: 7570 6c69 6361 7469 6f6e 2e0d 0a2d 2043  uplication...- C
+00001ed0: 6861 6e67 6564 2066 756e 6374 696f 6e20  hanged function 
+00001ee0: 6e61 6d65 2061 6e64 2064 656c 6574 6564  name and deleted
+00001ef0: 2075 6e6e 6563 6573 7361 7279 2061 7267   unnecessary arg
+00001f00: 756d 656e 7420 696e 2060 6170 7065 6e64  ument in `append
+00001f10: 5f65 6c65 6d65 6e74 735f 746f 5f6d 6173  _elements_to_mas
+00001f20: 7465 725f 656c 656d 656e 7428 2960 206e  ter_element()` n
+00001f30: 6573 7465 6420 696e 7369 6465 2070 7269  ested inside pri
+00001f40: 7661 7465 206d 6574 686f 6420 605f 746f  vate method `_to
+00001f50: 5f78 6d6c 2829 6020 696e 2060 4f73 6d43  _xml()` in `OsmC
+00001f60: 6861 6e67 6560 2e0d 0a0d 0a23 2320 5b30  hange`.....## [0
+00001f70: 2e33 2e30 5d20 2d20 3230 3233 2d30 332d  .3.0] - 2023-03-
+00001f80: 3134 0d0a 0d0a 2323 2320 4164 6465 640d  14....### Added.
+00001f90: 0a2d 2060 746f 5f64 6963 7428 2960 206d  .- `to_dict()` m
+00001fa0: 6574 686f 6420 616e 6420 6066 726f 6d5f  ethod and `from_
+00001fb0: 6469 6374 2829 6020 636c 6173 7320 6d65  dict()` class me
+00001fc0: 7468 6f64 2074 6f20 4368 616e 6765 7365  thod to Changese
+00001fd0: 742e 205b 2337 5d28 6874 7470 733a 2f2f  t. [#7](https://
+00001fe0: 6769 7468 7562 2e63 6f6d 2f64 6f63 656e  github.com/docen
+00001ff0: 7459 542f 6f73 6d5f 6561 7379 5f61 7069  tYT/osm_easy_api
+00002000: 2f69 7373 7565 732f 3729 0d0a 2d20 4162  /issues/7)..- Ab
+00002010: 696c 6974 7920 746f 2073 6574 2075 7365  ility to set use
+00002020: 725f 6167 656e 7420 696e 2060 4469 6666  r_agent in `Diff
+00002030: 6020 616e 6420 6041 7069 6020 636c 6173  ` and `Api` clas
+00002040: 732e 205b 2335 5d28 6874 7470 733a 2f2f  s. [#5](https://
+00002050: 6769 7468 7562 2e63 6f6d 2f64 6f63 656e  github.com/docen
+00002060: 7459 542f 6f73 6d5f 6561 7379 5f61 7069  tYT/osm_easy_api
+00002070: 2f69 7373 7565 732f 3529 0d0a 2d20 606f  /issues/5)..- `o
+00002080: 736d 5f6f 626a 6563 745f 7072 696d 6974  sm_object_primit
+00002090: 6976 6560 2060 6672 6f6d 5f64 6963 7428  ive` `from_dict(
+000020a0: 2960 2063 6c61 7373 206d 6574 686f 6420  )` class method 
+000020b0: 6e6f 7720 7261 6973 6573 2060 5661 6c75  now raises `Valu
+000020c0: 6545 7272 6f72 6020 6966 2074 6865 2060  eError` if the `
+000020d0: 7479 7065 6020 6b65 7920 6973 206e 6f74  type` key is not
+000020e0: 2066 6f75 6e64 2e0d 0a0d 0a23 2323 2043   found.....### C
+000020f0: 6861 6e67 6564 0d0a 2d20 6043 6861 6e67  hanged..- `Chang
+00002100: 6573 6574 6020 6973 206e 6f77 2065 7870  eset` is now exp
+00002110: 6f72 7465 6420 6672 6f6d 2064 6174 615f  orted from data_
+00002120: 636c 6173 7365 7320 6d6f 6475 6c65 2e0d  classes module..
+00002130: 0a2d 204d 6f72 6520 7465 7374 732e 0d0a  .- More tests...
+00002140: 0d0a 2323 205b 302e 322e 305d 202d 2032  ..## [0.2.0] - 2
+00002150: 3032 332d 3033 2d30 370d 0a0d 0a23 2323  023-03-07....###
+00002160: 2041 6464 6564 0d0a 2d20 6074 6f5f 6469   Added..- `to_di
+00002170: 6374 2829 6020 6d65 7468 6f64 2061 6e64  ct()` method and
+00002180: 2060 6672 6f6d 5f64 6963 7428 2960 2063   `from_dict()` c
+00002190: 6c61 7373 206d 6574 686f 6420 746f 2060  lass method to `
+000021a0: 6f73 6d5f 6f62 6a65 6374 5f70 7269 6d69  osm_object_primi
+000021b0: 7469 7665 602e 2028 416e 206f 626a 6563  tive`. (An objec
+000021c0: 7420 7468 6174 2069 7320 696e 6865 7269  t that is inheri
+000021d0: 7465 6420 6279 2061 2060 4e6f 6465 602c  ted by a `Node`,
+000021e0: 2060 5761 7960 2c20 6052 656c 6174 696f   `Way`, `Relatio
+000021f0: 6e60 292e 205b 2333 5d28 6874 7470 733a  n`). [#3](https:
+00002200: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+00002210: 656e 7459 542f 6f73 6d5f 6561 7379 5f61  entYT/osm_easy_a
+00002220: 7069 2f69 7373 7565 732f 3329 0d0a 2d20  pi/issues/3)..- 
+00002230: 5375 7070 6f72 7420 666f 7220 6869 7374  Support for hist
+00002240: 6f72 6963 616c 2061 6e6f 6e79 6d6f 7573  orical anonymous
+00002250: 2065 6469 7473 2061 6e64 2065 6469 7473   edits and edits
+00002260: 206d 6164 6520 6279 2064 656c 6574 6564   made by deleted
+00002270: 2061 6363 6f75 6e74 732e 205b 2334 5d28   accounts. [#4](
+00002280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002290: 6f6d 2f64 6f63 656e 7459 542f 6f73 6d5f  om/docentYT/osm_
+000022a0: 6561 7379 5f61 7069 2f69 7373 7565 732f  easy_api/issues/
+000022b0: 3429 0d0a 0d0a 2323 205b 302e 312e 345d  4)....## [0.1.4]
+000022c0: 202d 2032 3032 332d 3033 2d30 350d 0a0d   - 2023-03-05...
+000022d0: 0a23 2323 2046 6978 6564 0d0a 2d20 496d  .### Fixed..- Im
+000022e0: 7072 6f76 656d 656e 7420 6f66 2075 7469  provement of uti
+000022f0: 6c73 2e6a 6f69 6e5f 7572 6c28 2920 6675  ls.join_url() fu
+00002300: 6e63 7469 6f6e 2e0d 0a2d 2053 7065 6c6c  nction...- Spell
+00002310: 696e 6720 6572 726f 7273 2063 6f72 7265  ing errors corre
+00002320: 6374 6564 205b 406d 6174 6b6f 6e69 6563  cted [@matkoniec
+00002330: 7a5d 2868 7474 7073 3a2f 2f67 6974 6875  z](https://githu
+00002340: 622e 636f 6d2f 6d61 746b 6f6e 6965 637a  b.com/matkoniecz
+00002350: 290d 0a0d 0a23 2320 5b30 2e31 2e33 5d20  )....## [0.1.3] 
+00002360: 2d20 3230 3233 2d30 332d 3033 0d0a 0d0a  - 2023-03-03....
+00002370: 2323 2320 4669 7865 640d 0a0d 0a2d 2046  ### Fixed....- F
+00002380: 6978 6564 2074 6865 206e 6f6e 2d73 6574  ixed the non-set
+00002390: 7469 6e67 206f 6620 7468 6520 2276 6973  ting of the "vis
+000023a0: 6962 6c65 2220 6174 7472 6962 7574 652e  ible" attribute.
+000023b0: 0d0a 0d0a 2323 205b 302e 312e 325d 202d  ....## [0.1.2] -
+000023c0: 2032 3032 332d 3033 2d30 330d 0a0d 0a23   2023-03-03....#
+000023d0: 2323 2046 6978 6564 0d0a 0d0a 2d20 4669  ## Fixed....- Fi
+000023e0: 7865 6420 7265 7475 726e 2074 7970 6520  xed return type 
+000023f0: 6f66 2067 656e 6572 6174 6f72 2069 6e20  of generator in 
+00002400: 4469 6666 2e67 6574 2829 206d 6574 686f  Diff.get() metho
+00002410: 642e 0d0a 0d0a 2323 205b 302e 312e 315d  d.....## [0.1.1]
+00002420: 202d 2032 3032 332d 3033 2d30 330d 0a0d   - 2023-03-03...
+00002430: 0a23 2323 2041 6464 6564 0d0a 0d0a 2d20  .### Added....- 
+00002440: 4c69 6365 6e73 650d 0a0d 0a23 2320 5b30  License....## [0
+00002450: 2e31 2e30 5d20 2d20 3230 3233 2d30 332d  .1.0] - 2023-03-
+00002460: 3033 0d0a 0d0a 2323 2320 4164 6465 640d  03....### Added.
+00002470: 0a0d 0a2d 2049 6e69 7469 616c 2069 6d70  ...- Initial imp
+00002480: 6f72 740d 0a20 2020 2020 2020 2020 2020  ort..           
+00002490: 2020 2020 2020 2020 2047 4e55 2047 454e           GNU GEN
+000024a0: 4552 414c 2050 5542 4c49 4320 4c49 4345  ERAL PUBLIC LICE
+000024b0: 4e53 450d 0a20 2020 2020 2020 2020 2020  NSE..           
+000024c0: 2020 2020 2020 2020 2020 2020 5665 7273              Vers
+000024d0: 696f 6e20 332c 2032 3920 4a75 6e65 2032  ion 3, 29 June 2
+000024e0: 3030 370d 0a0d 0a20 436f 7079 7269 6768  007.... Copyrigh
+000024f0: 7420 2843 2920 3230 3037 2046 7265 6520  t (C) 2007 Free 
+00002500: 536f 6674 7761 7265 2046 6f75 6e64 6174  Software Foundat
+00002510: 696f 6e2c 2049 6e63 2e20 3c68 7474 7073  ion, Inc. <https
+00002520: 3a2f 2f66 7366 2e6f 7267 2f3e 0d0a 2045  ://fsf.org/>.. E
+00002530: 7665 7279 6f6e 6520 6973 2070 6572 6d69  veryone is permi
+00002540: 7474 6564 2074 6f20 636f 7079 2061 6e64  tted to copy and
+00002550: 2064 6973 7472 6962 7574 6520 7665 7262   distribute verb
+00002560: 6174 696d 2063 6f70 6965 730d 0a20 6f66  atim copies.. of
+00002570: 2074 6869 7320 6c69 6365 6e73 6520 646f   this license do
+00002580: 6375 6d65 6e74 2c20 6275 7420 6368 616e  cument, but chan
+00002590: 6769 6e67 2069 7420 6973 206e 6f74 2061  ging it is not a
+000025a0: 6c6c 6f77 6564 2e0d 0a0d 0a20 2020 2020  llowed.....     
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 2020 2020 2020 2050 7265 616d 626c 650d         Preamble.
+000025d0: 0a0d 0a20 2054 6865 2047 4e55 2047 656e  ...  The GNU Gen
+000025e0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+000025f0: 6e73 6520 6973 2061 2066 7265 652c 2063  nse is a free, c
+00002600: 6f70 796c 6566 7420 6c69 6365 6e73 6520  opyleft license 
+00002610: 666f 720d 0a73 6f66 7477 6172 6520 616e  for..software an
+00002620: 6420 6f74 6865 7220 6b69 6e64 7320 6f66  d other kinds of
+00002630: 2077 6f72 6b73 2e0d 0a0d 0a20 2054 6865   works.....  The
+00002640: 206c 6963 656e 7365 7320 666f 7220 6d6f   licenses for mo
+00002650: 7374 2073 6f66 7477 6172 6520 616e 6420  st software and 
+00002660: 6f74 6865 7220 7072 6163 7469 6361 6c20  other practical 
+00002670: 776f 726b 7320 6172 6520 6465 7369 676e  works are design
+00002680: 6564 0d0a 746f 2074 616b 6520 6177 6179  ed..to take away
+00002690: 2079 6f75 7220 6672 6565 646f 6d20 746f   your freedom to
+000026a0: 2073 6861 7265 2061 6e64 2063 6861 6e67   share and chang
+000026b0: 6520 7468 6520 776f 726b 732e 2020 4279  e the works.  By
+000026c0: 2063 6f6e 7472 6173 742c 0d0a 7468 6520   contrast,..the 
+000026d0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
+000026e0: 6963 204c 6963 656e 7365 2069 7320 696e  ic License is in
+000026f0: 7465 6e64 6564 2074 6f20 6775 6172 616e  tended to guaran
+00002700: 7465 6520 796f 7572 2066 7265 6564 6f6d  tee your freedom
+00002710: 2074 6f0d 0a73 6861 7265 2061 6e64 2063   to..share and c
+00002720: 6861 6e67 6520 616c 6c20 7665 7273 696f  hange all versio
+00002730: 6e73 206f 6620 6120 7072 6f67 7261 6d2d  ns of a program-
+00002740: 2d74 6f20 6d61 6b65 2073 7572 6520 6974  -to make sure it
+00002750: 2072 656d 6169 6e73 2066 7265 650d 0a73   remains free..s
+00002760: 6f66 7477 6172 6520 666f 7220 616c 6c20  oftware for all 
+00002770: 6974 7320 7573 6572 732e 2020 5765 2c20  its users.  We, 
+00002780: 7468 6520 4672 6565 2053 6f66 7477 6172  the Free Softwar
+00002790: 6520 466f 756e 6461 7469 6f6e 2c20 7573  e Foundation, us
+000027a0: 6520 7468 650d 0a47 4e55 2047 656e 6572  e the..GNU Gener
+000027b0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+000027c0: 6520 666f 7220 6d6f 7374 206f 6620 6f75  e for most of ou
+000027d0: 7220 736f 6674 7761 7265 3b20 6974 2061  r software; it a
+000027e0: 7070 6c69 6573 2061 6c73 6f20 746f 0d0a  pplies also to..
+000027f0: 616e 7920 6f74 6865 7220 776f 726b 2072  any other work r
+00002800: 656c 6561 7365 6420 7468 6973 2077 6179  eleased this way
+00002810: 2062 7920 6974 7320 6175 7468 6f72 732e   by its authors.
+00002820: 2020 596f 7520 6361 6e20 6170 706c 7920    You can apply 
+00002830: 6974 2074 6f0d 0a79 6f75 7220 7072 6f67  it to..your prog
+00002840: 7261 6d73 2c20 746f 6f2e 0d0a 0d0a 2020  rams, too.....  
+00002850: 5768 656e 2077 6520 7370 6561 6b20 6f66  When we speak of
+00002860: 2066 7265 6520 736f 6674 7761 7265 2c20   free software, 
+00002870: 7765 2061 7265 2072 6566 6572 7269 6e67  we are referring
+00002880: 2074 6f20 6672 6565 646f 6d2c 206e 6f74   to freedom, not
+00002890: 0d0a 7072 6963 652e 2020 4f75 7220 4765  ..price.  Our Ge
+000028a0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+000028b0: 656e 7365 7320 6172 6520 6465 7369 676e  enses are design
+000028c0: 6564 2074 6f20 6d61 6b65 2073 7572 6520  ed to make sure 
+000028d0: 7468 6174 2079 6f75 0d0a 6861 7665 2074  that you..have t
+000028e0: 6865 2066 7265 6564 6f6d 2074 6f20 6469  he freedom to di
+000028f0: 7374 7269 6275 7465 2063 6f70 6965 7320  stribute copies 
+00002900: 6f66 2066 7265 6520 736f 6674 7761 7265  of free software
+00002910: 2028 616e 6420 6368 6172 6765 2066 6f72   (and charge for
+00002920: 0d0a 7468 656d 2069 6620 796f 7520 7769  ..them if you wi
+00002930: 7368 292c 2074 6861 7420 796f 7520 7265  sh), that you re
+00002940: 6365 6976 6520 736f 7572 6365 2063 6f64  ceive source cod
+00002950: 6520 6f72 2063 616e 2067 6574 2069 7420  e or can get it 
+00002960: 6966 2079 6f75 0d0a 7761 6e74 2069 742c  if you..want it,
+00002970: 2074 6861 7420 796f 7520 6361 6e20 6368   that you can ch
+00002980: 616e 6765 2074 6865 2073 6f66 7477 6172  ange the softwar
+00002990: 6520 6f72 2075 7365 2070 6965 6365 7320  e or use pieces 
+000029a0: 6f66 2069 7420 696e 206e 6577 0d0a 6672  of it in new..fr
+000029b0: 6565 2070 726f 6772 616d 732c 2061 6e64  ee programs, and
+000029c0: 2074 6861 7420 796f 7520 6b6e 6f77 2079   that you know y
+000029d0: 6f75 2063 616e 2064 6f20 7468 6573 6520  ou can do these 
+000029e0: 7468 696e 6773 2e0d 0a0d 0a20 2054 6f20  things.....  To 
+000029f0: 7072 6f74 6563 7420 796f 7572 2072 6967  protect your rig
+00002a00: 6874 732c 2077 6520 6e65 6564 2074 6f20  hts, we need to 
+00002a10: 7072 6576 656e 7420 6f74 6865 7273 2066  prevent others f
+00002a20: 726f 6d20 6465 6e79 696e 6720 796f 750d  rom denying you.
+00002a30: 0a74 6865 7365 2072 6967 6874 7320 6f72  .these rights or
+00002a40: 2061 736b 696e 6720 796f 7520 746f 2073   asking you to s
+00002a50: 7572 7265 6e64 6572 2074 6865 2072 6967  urrender the rig
+00002a60: 6874 732e 2020 5468 6572 6566 6f72 652c  hts.  Therefore,
+00002a70: 2079 6f75 2068 6176 650d 0a63 6572 7461   you have..certa
+00002a80: 696e 2072 6573 706f 6e73 6962 696c 6974  in responsibilit
+00002a90: 6965 7320 6966 2079 6f75 2064 6973 7472  ies if you distr
+00002aa0: 6962 7574 6520 636f 7069 6573 206f 6620  ibute copies of 
+00002ab0: 7468 6520 736f 6674 7761 7265 2c20 6f72  the software, or
+00002ac0: 2069 660d 0a79 6f75 206d 6f64 6966 7920   if..you modify 
+00002ad0: 6974 3a20 7265 7370 6f6e 7369 6269 6c69  it: responsibili
+00002ae0: 7469 6573 2074 6f20 7265 7370 6563 7420  ties to respect 
+00002af0: 7468 6520 6672 6565 646f 6d20 6f66 206f  the freedom of o
+00002b00: 7468 6572 732e 0d0a 0d0a 2020 466f 7220  thers.....  For 
+00002b10: 6578 616d 706c 652c 2069 6620 796f 7520  example, if you 
+00002b20: 6469 7374 7269 6275 7465 2063 6f70 6965  distribute copie
+00002b30: 7320 6f66 2073 7563 6820 6120 7072 6f67  s of such a prog
+00002b40: 7261 6d2c 2077 6865 7468 6572 0d0a 6772  ram, whether..gr
+00002b50: 6174 6973 206f 7220 666f 7220 6120 6665  atis or for a fe
+00002b60: 652c 2079 6f75 206d 7573 7420 7061 7373  e, you must pass
+00002b70: 206f 6e20 746f 2074 6865 2072 6563 6970   on to the recip
+00002b80: 6965 6e74 7320 7468 6520 7361 6d65 0d0a  ients the same..
+00002b90: 6672 6565 646f 6d73 2074 6861 7420 796f  freedoms that yo
+00002ba0: 7520 7265 6365 6976 6564 2e20 2059 6f75  u received.  You
+00002bb0: 206d 7573 7420 6d61 6b65 2073 7572 6520   must make sure 
+00002bc0: 7468 6174 2074 6865 792c 2074 6f6f 2c20  that they, too, 
+00002bd0: 7265 6365 6976 650d 0a6f 7220 6361 6e20  receive..or can 
+00002be0: 6765 7420 7468 6520 736f 7572 6365 2063  get the source c
+00002bf0: 6f64 652e 2020 416e 6420 796f 7520 6d75  ode.  And you mu
+00002c00: 7374 2073 686f 7720 7468 656d 2074 6865  st show them the
+00002c10: 7365 2074 6572 6d73 2073 6f20 7468 6579  se terms so they
+00002c20: 0d0a 6b6e 6f77 2074 6865 6972 2072 6967  ..know their rig
+00002c30: 6874 732e 0d0a 0d0a 2020 4465 7665 6c6f  hts.....  Develo
+00002c40: 7065 7273 2074 6861 7420 7573 6520 7468  pers that use th
+00002c50: 6520 474e 5520 4750 4c20 7072 6f74 6563  e GNU GPL protec
+00002c60: 7420 796f 7572 2072 6967 6874 7320 7769  t your rights wi
+00002c70: 7468 2074 776f 2073 7465 7073 3a0d 0a28  th two steps:..(
+00002c80: 3129 2061 7373 6572 7420 636f 7079 7269  1) assert copyri
+00002c90: 6768 7420 6f6e 2074 6865 2073 6f66 7477  ght on the softw
+00002ca0: 6172 652c 2061 6e64 2028 3229 206f 6666  are, and (2) off
+00002cb0: 6572 2079 6f75 2074 6869 7320 4c69 6365  er you this Lice
+00002cc0: 6e73 650d 0a67 6976 696e 6720 796f 7520  nse..giving you 
+00002cd0: 6c65 6761 6c20 7065 726d 6973 7369 6f6e  legal permission
+00002ce0: 2074 6f20 636f 7079 2c20 6469 7374 7269   to copy, distri
+00002cf0: 6275 7465 2061 6e64 2f6f 7220 6d6f 6469  bute and/or modi
+00002d00: 6679 2069 742e 0d0a 0d0a 2020 466f 7220  fy it.....  For 
+00002d10: 7468 6520 6465 7665 6c6f 7065 7273 2720  the developers' 
+00002d20: 616e 6420 6175 7468 6f72 7327 2070 726f  and authors' pro
+00002d30: 7465 6374 696f 6e2c 2074 6865 2047 504c  tection, the GPL
+00002d40: 2063 6c65 6172 6c79 2065 7870 6c61 696e   clearly explain
+00002d50: 730d 0a74 6861 7420 7468 6572 6520 6973  s..that there is
+00002d60: 206e 6f20 7761 7272 616e 7479 2066 6f72   no warranty for
+00002d70: 2074 6869 7320 6672 6565 2073 6f66 7477   this free softw
+00002d80: 6172 652e 2020 466f 7220 626f 7468 2075  are.  For both u
+00002d90: 7365 7273 2720 616e 640d 0a61 7574 686f  sers' and..autho
+00002da0: 7273 2720 7361 6b65 2c20 7468 6520 4750  rs' sake, the GP
+00002db0: 4c20 7265 7175 6972 6573 2074 6861 7420  L requires that 
+00002dc0: 6d6f 6469 6669 6564 2076 6572 7369 6f6e  modified version
+00002dd0: 7320 6265 206d 6172 6b65 6420 6173 0d0a  s be marked as..
+00002de0: 6368 616e 6765 642c 2073 6f20 7468 6174  changed, so that
+00002df0: 2074 6865 6972 2070 726f 626c 656d 7320   their problems 
+00002e00: 7769 6c6c 206e 6f74 2062 6520 6174 7472  will not be attr
+00002e10: 6962 7574 6564 2065 7272 6f6e 656f 7573  ibuted erroneous
+00002e20: 6c79 2074 6f0d 0a61 7574 686f 7273 206f  ly to..authors o
+00002e30: 6620 7072 6576 696f 7573 2076 6572 7369  f previous versi
+00002e40: 6f6e 732e 0d0a 0d0a 2020 536f 6d65 2064  ons.....  Some d
+00002e50: 6576 6963 6573 2061 7265 2064 6573 6967  evices are desig
+00002e60: 6e65 6420 746f 2064 656e 7920 7573 6572  ned to deny user
+00002e70: 7320 6163 6365 7373 2074 6f20 696e 7374  s access to inst
+00002e80: 616c 6c20 6f72 2072 756e 0d0a 6d6f 6469  all or run..modi
+00002e90: 6669 6564 2076 6572 7369 6f6e 7320 6f66  fied versions of
+00002ea0: 2074 6865 2073 6f66 7477 6172 6520 696e   the software in
+00002eb0: 7369 6465 2074 6865 6d2c 2061 6c74 686f  side them, altho
+00002ec0: 7567 6820 7468 6520 6d61 6e75 6661 6374  ugh the manufact
+00002ed0: 7572 6572 0d0a 6361 6e20 646f 2073 6f2e  urer..can do so.
+00002ee0: 2020 5468 6973 2069 7320 6675 6e64 616d    This is fundam
+00002ef0: 656e 7461 6c6c 7920 696e 636f 6d70 6174  entally incompat
+00002f00: 6962 6c65 2077 6974 6820 7468 6520 6169  ible with the ai
+00002f10: 6d20 6f66 0d0a 7072 6f74 6563 7469 6e67  m of..protecting
+00002f20: 2075 7365 7273 2720 6672 6565 646f 6d20   users' freedom 
+00002f30: 746f 2063 6861 6e67 6520 7468 6520 736f  to change the so
+00002f40: 6674 7761 7265 2e20 2054 6865 2073 7973  ftware.  The sys
+00002f50: 7465 6d61 7469 630d 0a70 6174 7465 726e  tematic..pattern
+00002f60: 206f 6620 7375 6368 2061 6275 7365 206f   of such abuse o
+00002f70: 6363 7572 7320 696e 2074 6865 2061 7265  ccurs in the are
+00002f80: 6120 6f66 2070 726f 6475 6374 7320 666f  a of products fo
+00002f90: 7220 696e 6469 7669 6475 616c 7320 746f  r individuals to
+00002fa0: 0d0a 7573 652c 2077 6869 6368 2069 7320  ..use, which is 
+00002fb0: 7072 6563 6973 656c 7920 7768 6572 6520  precisely where 
+00002fc0: 6974 2069 7320 6d6f 7374 2075 6e61 6363  it is most unacc
+00002fd0: 6570 7461 626c 652e 2020 5468 6572 6566  eptable.  Theref
+00002fe0: 6f72 652c 2077 650d 0a68 6176 6520 6465  ore, we..have de
+00002ff0: 7369 676e 6564 2074 6869 7320 7665 7273  signed this vers
+00003000: 696f 6e20 6f66 2074 6865 2047 504c 2074  ion of the GPL t
+00003010: 6f20 7072 6f68 6962 6974 2074 6865 2070  o prohibit the p
+00003020: 7261 6374 6963 6520 666f 7220 7468 6f73  ractice for thos
+00003030: 650d 0a70 726f 6475 6374 732e 2020 4966  e..products.  If
+00003040: 2073 7563 6820 7072 6f62 6c65 6d73 2061   such problems a
+00003050: 7269 7365 2073 7562 7374 616e 7469 616c  rise substantial
+00003060: 6c79 2069 6e20 6f74 6865 7220 646f 6d61  ly in other doma
+00003070: 696e 732c 2077 650d 0a73 7461 6e64 2072  ins, we..stand r
+00003080: 6561 6479 2074 6f20 6578 7465 6e64 2074  eady to extend t
+00003090: 6869 7320 7072 6f76 6973 696f 6e20 746f  his provision to
+000030a0: 2074 686f 7365 2064 6f6d 6169 6e73 2069   those domains i
+000030b0: 6e20 6675 7475 7265 2076 6572 7369 6f6e  n future version
+000030c0: 730d 0a6f 6620 7468 6520 4750 4c2c 2061  s..of the GPL, a
+000030d0: 7320 6e65 6564 6564 2074 6f20 7072 6f74  s needed to prot
+000030e0: 6563 7420 7468 6520 6672 6565 646f 6d20  ect the freedom 
+000030f0: 6f66 2075 7365 7273 2e0d 0a0d 0a20 2046  of users.....  F
+00003100: 696e 616c 6c79 2c20 6576 6572 7920 7072  inally, every pr
+00003110: 6f67 7261 6d20 6973 2074 6872 6561 7465  ogram is threate
+00003120: 6e65 6420 636f 6e73 7461 6e74 6c79 2062  ned constantly b
+00003130: 7920 736f 6674 7761 7265 2070 6174 656e  y software paten
+00003140: 7473 2e0d 0a53 7461 7465 7320 7368 6f75  ts...States shou
+00003150: 6c64 206e 6f74 2061 6c6c 6f77 2070 6174  ld not allow pat
+00003160: 656e 7473 2074 6f20 7265 7374 7269 6374  ents to restrict
+00003170: 2064 6576 656c 6f70 6d65 6e74 2061 6e64   development and
+00003180: 2075 7365 206f 660d 0a73 6f66 7477 6172   use of..softwar
+00003190: 6520 6f6e 2067 656e 6572 616c 2d70 7572  e on general-pur
+000031a0: 706f 7365 2063 6f6d 7075 7465 7273 2c20  pose computers, 
+000031b0: 6275 7420 696e 2074 686f 7365 2074 6861  but in those tha
+000031c0: 7420 646f 2c20 7765 2077 6973 6820 746f  t do, we wish to
+000031d0: 0d0a 6176 6f69 6420 7468 6520 7370 6563  ..avoid the spec
+000031e0: 6961 6c20 6461 6e67 6572 2074 6861 7420  ial danger that 
+000031f0: 7061 7465 6e74 7320 6170 706c 6965 6420  patents applied 
+00003200: 746f 2061 2066 7265 6520 7072 6f67 7261  to a free progra
+00003210: 6d20 636f 756c 640d 0a6d 616b 6520 6974  m could..make it
+00003220: 2065 6666 6563 7469 7665 6c79 2070 726f   effectively pro
+00003230: 7072 6965 7461 7279 2e20 2054 6f20 7072  prietary.  To pr
+00003240: 6576 656e 7420 7468 6973 2c20 7468 6520  event this, the 
+00003250: 4750 4c20 6173 7375 7265 7320 7468 6174  GPL assures that
+00003260: 0d0a 7061 7465 6e74 7320 6361 6e6e 6f74  ..patents cannot
+00003270: 2062 6520 7573 6564 2074 6f20 7265 6e64   be used to rend
+00003280: 6572 2074 6865 2070 726f 6772 616d 206e  er the program n
+00003290: 6f6e 2d66 7265 652e 0d0a 0d0a 2020 5468  on-free.....  Th
+000032a0: 6520 7072 6563 6973 6520 7465 726d 7320  e precise terms 
+000032b0: 616e 6420 636f 6e64 6974 696f 6e73 2066  and conditions f
+000032c0: 6f72 2063 6f70 7969 6e67 2c20 6469 7374  or copying, dist
+000032d0: 7269 6275 7469 6f6e 2061 6e64 0d0a 6d6f  ribution and..mo
+000032e0: 6469 6669 6361 7469 6f6e 2066 6f6c 6c6f  dification follo
+000032f0: 772e 0d0a 0d0a 2020 2020 2020 2020 2020  w.....          
+00003300: 2020 2020 2020 2020 2020 2020 2054 4552               TER
+00003310: 4d53 2041 4e44 2043 4f4e 4449 5449 4f4e  MS AND CONDITION
+00003320: 530d 0a0d 0a20 2030 2e20 4465 6669 6e69  S....  0. Defini
+00003330: 7469 6f6e 732e 0d0a 0d0a 2020 2254 6869  tions.....  "Thi
+00003340: 7320 4c69 6365 6e73 6522 2072 6566 6572  s License" refer
+00003350: 7320 746f 2076 6572 7369 6f6e 2033 206f  s to version 3 o
+00003360: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00003370: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00003380: 2e0d 0a0d 0a20 2022 436f 7079 7269 6768  .....  "Copyrigh
+00003390: 7422 2061 6c73 6f20 6d65 616e 7320 636f  t" also means co
+000033a0: 7079 7269 6768 742d 6c69 6b65 206c 6177  pyright-like law
+000033b0: 7320 7468 6174 2061 7070 6c79 2074 6f20  s that apply to 
+000033c0: 6f74 6865 7220 6b69 6e64 7320 6f66 0d0a  other kinds of..
+000033d0: 776f 726b 732c 2073 7563 6820 6173 2073  works, such as s
+000033e0: 656d 6963 6f6e 6475 6374 6f72 206d 6173  emiconductor mas
+000033f0: 6b73 2e0d 0a0d 0a20 2022 5468 6520 5072  ks.....  "The Pr
+00003400: 6f67 7261 6d22 2072 6566 6572 7320 746f  ogram" refers to
+00003410: 2061 6e79 2063 6f70 7972 6967 6874 6162   any copyrightab
+00003420: 6c65 2077 6f72 6b20 6c69 6365 6e73 6564  le work licensed
+00003430: 2075 6e64 6572 2074 6869 730d 0a4c 6963   under this..Lic
+00003440: 656e 7365 2e20 2045 6163 6820 6c69 6365  ense.  Each lice
+00003450: 6e73 6565 2069 7320 6164 6472 6573 7365  nsee is addresse
+00003460: 6420 6173 2022 796f 7522 2e20 2022 4c69  d as "you".  "Li
+00003470: 6365 6e73 6565 7322 2061 6e64 0d0a 2272  censees" and.."r
+00003480: 6563 6970 6965 6e74 7322 206d 6179 2062  ecipients" may b
+00003490: 6520 696e 6469 7669 6475 616c 7320 6f72  e individuals or
+000034a0: 206f 7267 616e 697a 6174 696f 6e73 2e0d   organizations..
+000034b0: 0a0d 0a20 2054 6f20 226d 6f64 6966 7922  ...  To "modify"
+000034c0: 2061 2077 6f72 6b20 6d65 616e 7320 746f   a work means to
+000034d0: 2063 6f70 7920 6672 6f6d 206f 7220 6164   copy from or ad
+000034e0: 6170 7420 616c 6c20 6f72 2070 6172 7420  apt all or part 
+000034f0: 6f66 2074 6865 2077 6f72 6b0d 0a69 6e20  of the work..in 
+00003500: 6120 6661 7368 696f 6e20 7265 7175 6972  a fashion requir
+00003510: 696e 6720 636f 7079 7269 6768 7420 7065  ing copyright pe
+00003520: 726d 6973 7369 6f6e 2c20 6f74 6865 7220  rmission, other 
+00003530: 7468 616e 2074 6865 206d 616b 696e 6720  than the making 
+00003540: 6f66 2061 6e0d 0a65 7861 6374 2063 6f70  of an..exact cop
+00003550: 792e 2020 5468 6520 7265 7375 6c74 696e  y.  The resultin
+00003560: 6720 776f 726b 2069 7320 6361 6c6c 6564  g work is called
+00003570: 2061 2022 6d6f 6469 6669 6564 2076 6572   a "modified ver
+00003580: 7369 6f6e 2220 6f66 2074 6865 0d0a 6561  sion" of the..ea
+00003590: 726c 6965 7220 776f 726b 206f 7220 6120  rlier work or a 
+000035a0: 776f 726b 2022 6261 7365 6420 6f6e 2220  work "based on" 
+000035b0: 7468 6520 6561 726c 6965 7220 776f 726b  the earlier work
+000035c0: 2e0d 0a0d 0a20 2041 2022 636f 7665 7265  .....  A "covere
+000035d0: 6420 776f 726b 2220 6d65 616e 7320 6569  d work" means ei
+000035e0: 7468 6572 2074 6865 2075 6e6d 6f64 6966  ther the unmodif
+000035f0: 6965 6420 5072 6f67 7261 6d20 6f72 2061  ied Program or a
+00003600: 2077 6f72 6b20 6261 7365 640d 0a6f 6e20   work based..on 
+00003610: 7468 6520 5072 6f67 7261 6d2e 0d0a 0d0a  the Program.....
+00003620: 2020 546f 2022 7072 6f70 6167 6174 6522    To "propagate"
+00003630: 2061 2077 6f72 6b20 6d65 616e 7320 746f   a work means to
+00003640: 2064 6f20 616e 7974 6869 6e67 2077 6974   do anything wit
+00003650: 6820 6974 2074 6861 742c 2077 6974 686f  h it that, witho
+00003660: 7574 0d0a 7065 726d 6973 7369 6f6e 2c20  ut..permission, 
+00003670: 776f 756c 6420 6d61 6b65 2079 6f75 2064  would make you d
+00003680: 6972 6563 746c 7920 6f72 2073 6563 6f6e  irectly or secon
+00003690: 6461 7269 6c79 206c 6961 626c 6520 666f  darily liable fo
+000036a0: 720d 0a69 6e66 7269 6e67 656d 656e 7420  r..infringement 
+000036b0: 756e 6465 7220 6170 706c 6963 6162 6c65  under applicable
+000036c0: 2063 6f70 7972 6967 6874 206c 6177 2c20   copyright law, 
+000036d0: 6578 6365 7074 2065 7865 6375 7469 6e67  except executing
+000036e0: 2069 7420 6f6e 2061 0d0a 636f 6d70 7574   it on a..comput
+000036f0: 6572 206f 7220 6d6f 6469 6679 696e 6720  er or modifying 
+00003700: 6120 7072 6976 6174 6520 636f 7079 2e20  a private copy. 
+00003710: 2050 726f 7061 6761 7469 6f6e 2069 6e63   Propagation inc
+00003720: 6c75 6465 7320 636f 7079 696e 672c 0d0a  ludes copying,..
+00003730: 6469 7374 7269 6275 7469 6f6e 2028 7769  distribution (wi
+00003740: 7468 206f 7220 7769 7468 6f75 7420 6d6f  th or without mo
+00003750: 6469 6669 6361 7469 6f6e 292c 206d 616b  dification), mak
+00003760: 696e 6720 6176 6169 6c61 626c 6520 746f  ing available to
+00003770: 2074 6865 0d0a 7075 626c 6963 2c20 616e   the..public, an
+00003780: 6420 696e 2073 6f6d 6520 636f 756e 7472  d in some countr
+00003790: 6965 7320 6f74 6865 7220 6163 7469 7669  ies other activi
+000037a0: 7469 6573 2061 7320 7765 6c6c 2e0d 0a0d  ties as well....
+000037b0: 0a20 2054 6f20 2263 6f6e 7665 7922 2061  .  To "convey" a
+000037c0: 2077 6f72 6b20 6d65 616e 7320 616e 7920   work means any 
+000037d0: 6b69 6e64 206f 6620 7072 6f70 6167 6174  kind of propagat
+000037e0: 696f 6e20 7468 6174 2065 6e61 626c 6573  ion that enables
+000037f0: 206f 7468 6572 0d0a 7061 7274 6965 7320   other..parties 
+00003800: 746f 206d 616b 6520 6f72 2072 6563 6569  to make or recei
+00003810: 7665 2063 6f70 6965 732e 2020 4d65 7265  ve copies.  Mere
+00003820: 2069 6e74 6572 6163 7469 6f6e 2077 6974   interaction wit
+00003830: 6820 6120 7573 6572 2074 6872 6f75 6768  h a user through
+00003840: 0d0a 6120 636f 6d70 7574 6572 206e 6574  ..a computer net
+00003850: 776f 726b 2c20 7769 7468 206e 6f20 7472  work, with no tr
+00003860: 616e 7366 6572 206f 6620 6120 636f 7079  ansfer of a copy
+00003870: 2c20 6973 206e 6f74 2063 6f6e 7665 7969  , is not conveyi
+00003880: 6e67 2e0d 0a0d 0a20 2041 6e20 696e 7465  ng.....  An inte
+00003890: 7261 6374 6976 6520 7573 6572 2069 6e74  ractive user int
+000038a0: 6572 6661 6365 2064 6973 706c 6179 7320  erface displays 
+000038b0: 2241 7070 726f 7072 6961 7465 204c 6567  "Appropriate Leg
+000038c0: 616c 204e 6f74 6963 6573 220d 0a74 6f20  al Notices"..to 
+000038d0: 7468 6520 6578 7465 6e74 2074 6861 7420  the extent that 
+000038e0: 6974 2069 6e63 6c75 6465 7320 6120 636f  it includes a co
+000038f0: 6e76 656e 6965 6e74 2061 6e64 2070 726f  nvenient and pro
+00003900: 6d69 6e65 6e74 6c79 2076 6973 6962 6c65  minently visible
+00003910: 0d0a 6665 6174 7572 6520 7468 6174 2028  ..feature that (
+00003920: 3129 2064 6973 706c 6179 7320 616e 2061  1) displays an a
+00003930: 7070 726f 7072 6961 7465 2063 6f70 7972  ppropriate copyr
+00003940: 6967 6874 206e 6f74 6963 652c 2061 6e64  ight notice, and
+00003950: 2028 3229 0d0a 7465 6c6c 7320 7468 6520   (2)..tells the 
+00003960: 7573 6572 2074 6861 7420 7468 6572 6520  user that there 
+00003970: 6973 206e 6f20 7761 7272 616e 7479 2066  is no warranty f
+00003980: 6f72 2074 6865 2077 6f72 6b20 2865 7863  or the work (exc
+00003990: 6570 7420 746f 2074 6865 0d0a 6578 7465  ept to the..exte
+000039a0: 6e74 2074 6861 7420 7761 7272 616e 7469  nt that warranti
+000039b0: 6573 2061 7265 2070 726f 7669 6465 6429  es are provided)
+000039c0: 2c20 7468 6174 206c 6963 656e 7365 6573  , that licensees
+000039d0: 206d 6179 2063 6f6e 7665 7920 7468 650d   may convey the.
+000039e0: 0a77 6f72 6b20 756e 6465 7220 7468 6973  .work under this
+000039f0: 204c 6963 656e 7365 2c20 616e 6420 686f   License, and ho
+00003a00: 7720 746f 2076 6965 7720 6120 636f 7079  w to view a copy
+00003a10: 206f 6620 7468 6973 204c 6963 656e 7365   of this License
+00003a20: 2e20 2049 660d 0a74 6865 2069 6e74 6572  .  If..the inter
+00003a30: 6661 6365 2070 7265 7365 6e74 7320 6120  face presents a 
+00003a40: 6c69 7374 206f 6620 7573 6572 2063 6f6d  list of user com
+00003a50: 6d61 6e64 7320 6f72 206f 7074 696f 6e73  mands or options
+00003a60: 2c20 7375 6368 2061 7320 610d 0a6d 656e  , such as a..men
+00003a70: 752c 2061 2070 726f 6d69 6e65 6e74 2069  u, a prominent i
+00003a80: 7465 6d20 696e 2074 6865 206c 6973 7420  tem in the list 
+00003a90: 6d65 6574 7320 7468 6973 2063 7269 7465  meets this crite
+00003aa0: 7269 6f6e 2e0d 0a0d 0a20 2031 2e20 536f  rion.....  1. So
+00003ab0: 7572 6365 2043 6f64 652e 0d0a 0d0a 2020  urce Code.....  
+00003ac0: 5468 6520 2273 6f75 7263 6520 636f 6465  The "source code
+00003ad0: 2220 666f 7220 6120 776f 726b 206d 6561  " for a work mea
+00003ae0: 6e73 2074 6865 2070 7265 6665 7272 6564  ns the preferred
+00003af0: 2066 6f72 6d20 6f66 2074 6865 2077 6f72   form of the wor
+00003b00: 6b0d 0a66 6f72 206d 616b 696e 6720 6d6f  k..for making mo
+00003b10: 6469 6669 6361 7469 6f6e 7320 746f 2069  difications to i
+00003b20: 742e 2020 224f 626a 6563 7420 636f 6465  t.  "Object code
+00003b30: 2220 6d65 616e 7320 616e 7920 6e6f 6e2d  " means any non-
+00003b40: 736f 7572 6365 0d0a 666f 726d 206f 6620  source..form of 
+00003b50: 6120 776f 726b 2e0d 0a0d 0a20 2041 2022  a work.....  A "
+00003b60: 5374 616e 6461 7264 2049 6e74 6572 6661  Standard Interfa
+00003b70: 6365 2220 6d65 616e 7320 616e 2069 6e74  ce" means an int
+00003b80: 6572 6661 6365 2074 6861 7420 6569 7468  erface that eith
+00003b90: 6572 2069 7320 616e 206f 6666 6963 6961  er is an officia
+00003ba0: 6c0d 0a73 7461 6e64 6172 6420 6465 6669  l..standard defi
+00003bb0: 6e65 6420 6279 2061 2072 6563 6f67 6e69  ned by a recogni
+00003bc0: 7a65 6420 7374 616e 6461 7264 7320 626f  zed standards bo
+00003bd0: 6479 2c20 6f72 2c20 696e 2074 6865 2063  dy, or, in the c
+00003be0: 6173 6520 6f66 0d0a 696e 7465 7266 6163  ase of..interfac
+00003bf0: 6573 2073 7065 6369 6669 6564 2066 6f72  es specified for
+00003c00: 2061 2070 6172 7469 6375 6c61 7220 7072   a particular pr
+00003c10: 6f67 7261 6d6d 696e 6720 6c61 6e67 7561  ogramming langua
+00003c20: 6765 2c20 6f6e 6520 7468 6174 0d0a 6973  ge, one that..is
+00003c30: 2077 6964 656c 7920 7573 6564 2061 6d6f   widely used amo
+00003c40: 6e67 2064 6576 656c 6f70 6572 7320 776f  ng developers wo
+00003c50: 726b 696e 6720 696e 2074 6861 7420 6c61  rking in that la
+00003c60: 6e67 7561 6765 2e0d 0a0d 0a20 2054 6865  nguage.....  The
+00003c70: 2022 5379 7374 656d 204c 6962 7261 7269   "System Librari
+00003c80: 6573 2220 6f66 2061 6e20 6578 6563 7574  es" of an execut
+00003c90: 6162 6c65 2077 6f72 6b20 696e 636c 7564  able work includ
+00003ca0: 6520 616e 7974 6869 6e67 2c20 6f74 6865  e anything, othe
+00003cb0: 720d 0a74 6861 6e20 7468 6520 776f 726b  r..than the work
+00003cc0: 2061 7320 6120 7768 6f6c 652c 2074 6861   as a whole, tha
+00003cd0: 7420 2861 2920 6973 2069 6e63 6c75 6465  t (a) is include
+00003ce0: 6420 696e 2074 6865 206e 6f72 6d61 6c20  d in the normal 
+00003cf0: 666f 726d 206f 660d 0a70 6163 6b61 6769  form of..packagi
+00003d00: 6e67 2061 204d 616a 6f72 2043 6f6d 706f  ng a Major Compo
+00003d10: 6e65 6e74 2c20 6275 7420 7768 6963 6820  nent, but which 
+00003d20: 6973 206e 6f74 2070 6172 7420 6f66 2074  is not part of t
+00003d30: 6861 7420 4d61 6a6f 720d 0a43 6f6d 706f  hat Major..Compo
+00003d40: 6e65 6e74 2c20 616e 6420 2862 2920 7365  nent, and (b) se
+00003d50: 7276 6573 206f 6e6c 7920 746f 2065 6e61  rves only to ena
+00003d60: 626c 6520 7573 6520 6f66 2074 6865 2077  ble use of the w
+00003d70: 6f72 6b20 7769 7468 2074 6861 740d 0a4d  ork with that..M
+00003d80: 616a 6f72 2043 6f6d 706f 6e65 6e74 2c20  ajor Component, 
+00003d90: 6f72 2074 6f20 696d 706c 656d 656e 7420  or to implement 
+00003da0: 6120 5374 616e 6461 7264 2049 6e74 6572  a Standard Inter
+00003db0: 6661 6365 2066 6f72 2077 6869 6368 2061  face for which a
+00003dc0: 6e0d 0a69 6d70 6c65 6d65 6e74 6174 696f  n..implementatio
+00003dd0: 6e20 6973 2061 7661 696c 6162 6c65 2074  n is available t
+00003de0: 6f20 7468 6520 7075 626c 6963 2069 6e20  o the public in 
+00003df0: 736f 7572 6365 2063 6f64 6520 666f 726d  source code form
+00003e00: 2e20 2041 0d0a 224d 616a 6f72 2043 6f6d  .  A.."Major Com
+00003e10: 706f 6e65 6e74 222c 2069 6e20 7468 6973  ponent", in this
+00003e20: 2063 6f6e 7465 7874 2c20 6d65 616e 7320   context, means 
+00003e30: 6120 6d61 6a6f 7220 6573 7365 6e74 6961  a major essentia
+00003e40: 6c20 636f 6d70 6f6e 656e 740d 0a28 6b65  l component..(ke
+00003e50: 726e 656c 2c20 7769 6e64 6f77 2073 7973  rnel, window sys
+00003e60: 7465 6d2c 2061 6e64 2073 6f20 6f6e 2920  tem, and so on) 
+00003e70: 6f66 2074 6865 2073 7065 6369 6669 6320  of the specific 
+00003e80: 6f70 6572 6174 696e 6720 7379 7374 656d  operating system
+00003e90: 0d0a 2869 6620 616e 7929 206f 6e20 7768  ..(if any) on wh
+00003ea0: 6963 6820 7468 6520 6578 6563 7574 6162  ich the executab
+00003eb0: 6c65 2077 6f72 6b20 7275 6e73 2c20 6f72  le work runs, or
+00003ec0: 2061 2063 6f6d 7069 6c65 7220 7573 6564   a compiler used
+00003ed0: 2074 6f0d 0a70 726f 6475 6365 2074 6865   to..produce the
+00003ee0: 2077 6f72 6b2c 206f 7220 616e 206f 626a   work, or an obj
+00003ef0: 6563 7420 636f 6465 2069 6e74 6572 7072  ect code interpr
+00003f00: 6574 6572 2075 7365 6420 746f 2072 756e  eter used to run
+00003f10: 2069 742e 0d0a 0d0a 2020 5468 6520 2243   it.....  The "C
+00003f20: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
+00003f30: 7263 6522 2066 6f72 2061 2077 6f72 6b20  rce" for a work 
+00003f40: 696e 206f 626a 6563 7420 636f 6465 2066  in object code f
+00003f50: 6f72 6d20 6d65 616e 7320 616c 6c0d 0a74  orm means all..t
+00003f60: 6865 2073 6f75 7263 6520 636f 6465 206e  he source code n
+00003f70: 6565 6465 6420 746f 2067 656e 6572 6174  eeded to generat
+00003f80: 652c 2069 6e73 7461 6c6c 2c20 616e 6420  e, install, and 
+00003f90: 2866 6f72 2061 6e20 6578 6563 7574 6162  (for an executab
+00003fa0: 6c65 0d0a 776f 726b 2920 7275 6e20 7468  le..work) run th
+00003fb0: 6520 6f62 6a65 6374 2063 6f64 6520 616e  e object code an
+00003fc0: 6420 746f 206d 6f64 6966 7920 7468 6520  d to modify the 
+00003fd0: 776f 726b 2c20 696e 636c 7564 696e 6720  work, including 
+00003fe0: 7363 7269 7074 7320 746f 0d0a 636f 6e74  scripts to..cont
+00003ff0: 726f 6c20 7468 6f73 6520 6163 7469 7669  rol those activi
+00004000: 7469 6573 2e20 2048 6f77 6576 6572 2c20  ties.  However, 
+00004010: 6974 2064 6f65 7320 6e6f 7420 696e 636c  it does not incl
+00004020: 7564 6520 7468 6520 776f 726b 2773 0d0a  ude the work's..
+00004030: 5379 7374 656d 204c 6962 7261 7269 6573  System Libraries
+00004040: 2c20 6f72 2067 656e 6572 616c 2d70 7572  , or general-pur
+00004050: 706f 7365 2074 6f6f 6c73 206f 7220 6765  pose tools or ge
+00004060: 6e65 7261 6c6c 7920 6176 6169 6c61 626c  nerally availabl
+00004070: 6520 6672 6565 0d0a 7072 6f67 7261 6d73  e free..programs
+00004080: 2077 6869 6368 2061 7265 2075 7365 6420   which are used 
+00004090: 756e 6d6f 6469 6669 6564 2069 6e20 7065  unmodified in pe
+000040a0: 7266 6f72 6d69 6e67 2074 686f 7365 2061  rforming those a
+000040b0: 6374 6976 6974 6965 7320 6275 740d 0a77  ctivities but..w
+000040c0: 6869 6368 2061 7265 206e 6f74 2070 6172  hich are not par
+000040d0: 7420 6f66 2074 6865 2077 6f72 6b2e 2020  t of the work.  
+000040e0: 466f 7220 6578 616d 706c 652c 2043 6f72  For example, Cor
+000040f0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
+00004100: 650d 0a69 6e63 6c75 6465 7320 696e 7465  e..includes inte
+00004110: 7266 6163 6520 6465 6669 6e69 7469 6f6e  rface definition
+00004120: 2066 696c 6573 2061 7373 6f63 6961 7465   files associate
+00004130: 6420 7769 7468 2073 6f75 7263 6520 6669  d with source fi
+00004140: 6c65 7320 666f 720d 0a74 6865 2077 6f72  les for..the wor
+00004150: 6b2c 2061 6e64 2074 6865 2073 6f75 7263  k, and the sourc
+00004160: 6520 636f 6465 2066 6f72 2073 6861 7265  e code for share
+00004170: 6420 6c69 6272 6172 6965 7320 616e 6420  d libraries and 
+00004180: 6479 6e61 6d69 6361 6c6c 790d 0a6c 696e  dynamically..lin
+00004190: 6b65 6420 7375 6270 726f 6772 616d 7320  ked subprograms 
+000041a0: 7468 6174 2074 6865 2077 6f72 6b20 6973  that the work is
+000041b0: 2073 7065 6369 6669 6361 6c6c 7920 6465   specifically de
+000041c0: 7369 676e 6564 2074 6f20 7265 7175 6972  signed to requir
+000041d0: 652c 0d0a 7375 6368 2061 7320 6279 2069  e,..such as by i
+000041e0: 6e74 696d 6174 6520 6461 7461 2063 6f6d  ntimate data com
+000041f0: 6d75 6e69 6361 7469 6f6e 206f 7220 636f  munication or co
+00004200: 6e74 726f 6c20 666c 6f77 2062 6574 7765  ntrol flow betwe
+00004210: 656e 2074 686f 7365 0d0a 7375 6270 726f  en those..subpro
+00004220: 6772 616d 7320 616e 6420 6f74 6865 7220  grams and other 
+00004230: 7061 7274 7320 6f66 2074 6865 2077 6f72  parts of the wor
+00004240: 6b2e 0d0a 0d0a 2020 5468 6520 436f 7272  k.....  The Corr
+00004250: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
+00004260: 206e 6565 6420 6e6f 7420 696e 636c 7564   need not includ
+00004270: 6520 616e 7974 6869 6e67 2074 6861 7420  e anything that 
+00004280: 7573 6572 730d 0a63 616e 2072 6567 656e  users..can regen
+00004290: 6572 6174 6520 6175 746f 6d61 7469 6361  erate automatica
+000042a0: 6c6c 7920 6672 6f6d 206f 7468 6572 2070  lly from other p
+000042b0: 6172 7473 206f 6620 7468 6520 436f 7272  arts of the Corr
+000042c0: 6573 706f 6e64 696e 670d 0a53 6f75 7263  esponding..Sourc
+000042d0: 652e 0d0a 0d0a 2020 5468 6520 436f 7272  e.....  The Corr
+000042e0: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
+000042f0: 2066 6f72 2061 2077 6f72 6b20 696e 2073   for a work in s
+00004300: 6f75 7263 6520 636f 6465 2066 6f72 6d20  ource code form 
+00004310: 6973 2074 6861 740d 0a73 616d 6520 776f  is that..same wo
+00004320: 726b 2e0d 0a0d 0a20 2032 2e20 4261 7369  rk.....  2. Basi
+00004330: 6320 5065 726d 6973 7369 6f6e 732e 0d0a  c Permissions...
+00004340: 0d0a 2020 416c 6c20 7269 6768 7473 2067  ..  All rights g
+00004350: 7261 6e74 6564 2075 6e64 6572 2074 6869  ranted under thi
+00004360: 7320 4c69 6365 6e73 6520 6172 6520 6772  s License are gr
+00004370: 616e 7465 6420 666f 7220 7468 6520 7465  anted for the te
+00004380: 726d 206f 660d 0a63 6f70 7972 6967 6874  rm of..copyright
+00004390: 206f 6e20 7468 6520 5072 6f67 7261 6d2c   on the Program,
+000043a0: 2061 6e64 2061 7265 2069 7272 6576 6f63   and are irrevoc
+000043b0: 6162 6c65 2070 726f 7669 6465 6420 7468  able provided th
+000043c0: 6520 7374 6174 6564 0d0a 636f 6e64 6974  e stated..condit
+000043d0: 696f 6e73 2061 7265 206d 6574 2e20 2054  ions are met.  T
+000043e0: 6869 7320 4c69 6365 6e73 6520 6578 706c  his License expl
+000043f0: 6963 6974 6c79 2061 6666 6972 6d73 2079  icitly affirms y
+00004400: 6f75 7220 756e 6c69 6d69 7465 640d 0a70  our unlimited..p
+00004410: 6572 6d69 7373 696f 6e20 746f 2072 756e  ermission to run
+00004420: 2074 6865 2075 6e6d 6f64 6966 6965 6420   the unmodified 
+00004430: 5072 6f67 7261 6d2e 2020 5468 6520 6f75  Program.  The ou
+00004440: 7470 7574 2066 726f 6d20 7275 6e6e 696e  tput from runnin
+00004450: 6720 610d 0a63 6f76 6572 6564 2077 6f72  g a..covered wor
+00004460: 6b20 6973 2063 6f76 6572 6564 2062 7920  k is covered by 
+00004470: 7468 6973 204c 6963 656e 7365 206f 6e6c  this License onl
+00004480: 7920 6966 2074 6865 206f 7574 7075 742c  y if the output,
+00004490: 2067 6976 656e 2069 7473 0d0a 636f 6e74   given its..cont
+000044a0: 656e 742c 2063 6f6e 7374 6974 7574 6573  ent, constitutes
+000044b0: 2061 2063 6f76 6572 6564 2077 6f72 6b2e   a covered work.
+000044c0: 2020 5468 6973 204c 6963 656e 7365 2061    This License a
+000044d0: 636b 6e6f 776c 6564 6765 7320 796f 7572  cknowledges your
+000044e0: 0d0a 7269 6768 7473 206f 6620 6661 6972  ..rights of fair
+000044f0: 2075 7365 206f 7220 6f74 6865 7220 6571   use or other eq
+00004500: 7569 7661 6c65 6e74 2c20 6173 2070 726f  uivalent, as pro
+00004510: 7669 6465 6420 6279 2063 6f70 7972 6967  vided by copyrig
+00004520: 6874 206c 6177 2e0d 0a0d 0a20 2059 6f75  ht law.....  You
+00004530: 206d 6179 206d 616b 652c 2072 756e 2061   may make, run a
+00004540: 6e64 2070 726f 7061 6761 7465 2063 6f76  nd propagate cov
+00004550: 6572 6564 2077 6f72 6b73 2074 6861 7420  ered works that 
+00004560: 796f 7520 646f 206e 6f74 0d0a 636f 6e76  you do not..conv
+00004570: 6579 2c20 7769 7468 6f75 7420 636f 6e64  ey, without cond
+00004580: 6974 696f 6e73 2073 6f20 6c6f 6e67 2061  itions so long a
+00004590: 7320 796f 7572 206c 6963 656e 7365 206f  s your license o
+000045a0: 7468 6572 7769 7365 2072 656d 6169 6e73  therwise remains
+000045b0: 0d0a 696e 2066 6f72 6365 2e20 2059 6f75  ..in force.  You
+000045c0: 206d 6179 2063 6f6e 7665 7920 636f 7665   may convey cove
+000045d0: 7265 6420 776f 726b 7320 746f 206f 7468  red works to oth
+000045e0: 6572 7320 666f 7220 7468 6520 736f 6c65  ers for the sole
+000045f0: 2070 7572 706f 7365 0d0a 6f66 2068 6176   purpose..of hav
+00004600: 696e 6720 7468 656d 206d 616b 6520 6d6f  ing them make mo
+00004610: 6469 6669 6361 7469 6f6e 7320 6578 636c  difications excl
+00004620: 7573 6976 656c 7920 666f 7220 796f 752c  usively for you,
+00004630: 206f 7220 7072 6f76 6964 6520 796f 750d   or provide you.
+00004640: 0a77 6974 6820 6661 6369 6c69 7469 6573  .with facilities
+00004650: 2066 6f72 2072 756e 6e69 6e67 2074 686f   for running tho
+00004660: 7365 2077 6f72 6b73 2c20 7072 6f76 6964  se works, provid
+00004670: 6564 2074 6861 7420 796f 7520 636f 6d70  ed that you comp
+00004680: 6c79 2077 6974 680d 0a74 6865 2074 6572  ly with..the ter
+00004690: 6d73 206f 6620 7468 6973 204c 6963 656e  ms of this Licen
+000046a0: 7365 2069 6e20 636f 6e76 6579 696e 6720  se in conveying 
+000046b0: 616c 6c20 6d61 7465 7269 616c 2066 6f72  all material for
+000046c0: 2077 6869 6368 2079 6f75 2064 6f0d 0a6e   which you do..n
+000046d0: 6f74 2063 6f6e 7472 6f6c 2063 6f70 7972  ot control copyr
+000046e0: 6967 6874 2e20 2054 686f 7365 2074 6875  ight.  Those thu
+000046f0: 7320 6d61 6b69 6e67 206f 7220 7275 6e6e  s making or runn
+00004700: 696e 6720 7468 6520 636f 7665 7265 6420  ing the covered 
+00004710: 776f 726b 730d 0a66 6f72 2079 6f75 206d  works..for you m
+00004720: 7573 7420 646f 2073 6f20 6578 636c 7573  ust do so exclus
+00004730: 6976 656c 7920 6f6e 2079 6f75 7220 6265  ively on your be
+00004740: 6861 6c66 2c20 756e 6465 7220 796f 7572  half, under your
+00004750: 2064 6972 6563 7469 6f6e 0d0a 616e 6420   direction..and 
+00004760: 636f 6e74 726f 6c2c 206f 6e20 7465 726d  control, on term
+00004770: 7320 7468 6174 2070 726f 6869 6269 7420  s that prohibit 
+00004780: 7468 656d 2066 726f 6d20 6d61 6b69 6e67  them from making
+00004790: 2061 6e79 2063 6f70 6965 7320 6f66 0d0a   any copies of..
+000047a0: 796f 7572 2063 6f70 7972 6967 6874 6564  your copyrighted
+000047b0: 206d 6174 6572 6961 6c20 6f75 7473 6964   material outsid
+000047c0: 6520 7468 6569 7220 7265 6c61 7469 6f6e  e their relation
+000047d0: 7368 6970 2077 6974 6820 796f 752e 0d0a  ship with you...
+000047e0: 0d0a 2020 436f 6e76 6579 696e 6720 756e  ..  Conveying un
+000047f0: 6465 7220 616e 7920 6f74 6865 7220 6369  der any other ci
+00004800: 7263 756d 7374 616e 6365 7320 6973 2070  rcumstances is p
+00004810: 6572 6d69 7474 6564 2073 6f6c 656c 7920  ermitted solely 
+00004820: 756e 6465 720d 0a74 6865 2063 6f6e 6469  under..the condi
+00004830: 7469 6f6e 7320 7374 6174 6564 2062 656c  tions stated bel
+00004840: 6f77 2e20 2053 7562 6c69 6365 6e73 696e  ow.  Sublicensin
+00004850: 6720 6973 206e 6f74 2061 6c6c 6f77 6564  g is not allowed
+00004860: 3b20 7365 6374 696f 6e20 3130 0d0a 6d61  ; section 10..ma
+00004870: 6b65 7320 6974 2075 6e6e 6563 6573 7361  kes it unnecessa
+00004880: 7279 2e0d 0a0d 0a20 2033 2e20 5072 6f74  ry.....  3. Prot
+00004890: 6563 7469 6e67 2055 7365 7273 2720 4c65  ecting Users' Le
+000048a0: 6761 6c20 5269 6768 7473 2046 726f 6d20  gal Rights From 
+000048b0: 416e 7469 2d43 6972 6375 6d76 656e 7469  Anti-Circumventi
+000048c0: 6f6e 204c 6177 2e0d 0a0d 0a20 204e 6f20  on Law.....  No 
+000048d0: 636f 7665 7265 6420 776f 726b 2073 6861  covered work sha
+000048e0: 6c6c 2062 6520 6465 656d 6564 2070 6172  ll be deemed par
+000048f0: 7420 6f66 2061 6e20 6566 6665 6374 6976  t of an effectiv
+00004900: 6520 7465 6368 6e6f 6c6f 6769 6361 6c0d  e technological.
+00004910: 0a6d 6561 7375 7265 2075 6e64 6572 2061  .measure under a
+00004920: 6e79 2061 7070 6c69 6361 626c 6520 6c61  ny applicable la
+00004930: 7720 6675 6c66 696c 6c69 6e67 206f 626c  w fulfilling obl
+00004940: 6967 6174 696f 6e73 2075 6e64 6572 2061  igations under a
+00004950: 7274 6963 6c65 0d0a 3131 206f 6620 7468  rticle..11 of th
+00004960: 6520 5749 504f 2063 6f70 7972 6967 6874  e WIPO copyright
+00004970: 2074 7265 6174 7920 6164 6f70 7465 6420   treaty adopted 
+00004980: 6f6e 2032 3020 4465 6365 6d62 6572 2031  on 20 December 1
+00004990: 3939 362c 206f 720d 0a73 696d 696c 6172  996, or..similar
+000049a0: 206c 6177 7320 7072 6f68 6962 6974 696e   laws prohibitin
+000049b0: 6720 6f72 2072 6573 7472 6963 7469 6e67  g or restricting
+000049c0: 2063 6972 6375 6d76 656e 7469 6f6e 206f   circumvention o
+000049d0: 6620 7375 6368 0d0a 6d65 6173 7572 6573  f such..measures
+000049e0: 2e0d 0a0d 0a20 2057 6865 6e20 796f 7520  .....  When you 
+000049f0: 636f 6e76 6579 2061 2063 6f76 6572 6564  convey a covered
+00004a00: 2077 6f72 6b2c 2079 6f75 2077 6169 7665   work, you waive
+00004a10: 2061 6e79 206c 6567 616c 2070 6f77 6572   any legal power
+00004a20: 2074 6f20 666f 7262 6964 0d0a 6369 7263   to forbid..circ
+00004a30: 756d 7665 6e74 696f 6e20 6f66 2074 6563  umvention of tec
+00004a40: 686e 6f6c 6f67 6963 616c 206d 6561 7375  hnological measu
+00004a50: 7265 7320 746f 2074 6865 2065 7874 656e  res to the exten
+00004a60: 7420 7375 6368 2063 6972 6375 6d76 656e  t such circumven
+00004a70: 7469 6f6e 0d0a 6973 2065 6666 6563 7465  tion..is effecte
+00004a80: 6420 6279 2065 7865 7263 6973 696e 6720  d by exercising 
+00004a90: 7269 6768 7473 2075 6e64 6572 2074 6869  rights under thi
+00004aa0: 7320 4c69 6365 6e73 6520 7769 7468 2072  s License with r
+00004ab0: 6573 7065 6374 2074 6f0d 0a74 6865 2063  espect to..the c
+00004ac0: 6f76 6572 6564 2077 6f72 6b2c 2061 6e64  overed work, and
+00004ad0: 2079 6f75 2064 6973 636c 6169 6d20 616e   you disclaim an
+00004ae0: 7920 696e 7465 6e74 696f 6e20 746f 206c  y intention to l
+00004af0: 696d 6974 206f 7065 7261 7469 6f6e 206f  imit operation o
+00004b00: 720d 0a6d 6f64 6966 6963 6174 696f 6e20  r..modification 
+00004b10: 6f66 2074 6865 2077 6f72 6b20 6173 2061  of the work as a
+00004b20: 206d 6561 6e73 206f 6620 656e 666f 7263   means of enforc
+00004b30: 696e 672c 2061 6761 696e 7374 2074 6865  ing, against the
+00004b40: 2077 6f72 6b27 730d 0a75 7365 7273 2c20   work's..users, 
+00004b50: 796f 7572 206f 7220 7468 6972 6420 7061  your or third pa
+00004b60: 7274 6965 7327 206c 6567 616c 2072 6967  rties' legal rig
+00004b70: 6874 7320 746f 2066 6f72 6269 6420 6369  hts to forbid ci
+00004b80: 7263 756d 7665 6e74 696f 6e20 6f66 0d0a  rcumvention of..
+00004b90: 7465 6368 6e6f 6c6f 6769 6361 6c20 6d65  technological me
+00004ba0: 6173 7572 6573 2e0d 0a0d 0a20 2034 2e20  asures.....  4. 
+00004bb0: 436f 6e76 6579 696e 6720 5665 7262 6174  Conveying Verbat
+00004bc0: 696d 2043 6f70 6965 732e 0d0a 0d0a 2020  im Copies.....  
+00004bd0: 596f 7520 6d61 7920 636f 6e76 6579 2076  You may convey v
+00004be0: 6572 6261 7469 6d20 636f 7069 6573 206f  erbatim copies o
+00004bf0: 6620 7468 6520 5072 6f67 7261 6d27 7320  f the Program's 
+00004c00: 736f 7572 6365 2063 6f64 6520 6173 2079  source code as y
+00004c10: 6f75 0d0a 7265 6365 6976 6520 6974 2c20  ou..receive it, 
+00004c20: 696e 2061 6e79 206d 6564 6975 6d2c 2070  in any medium, p
+00004c30: 726f 7669 6465 6420 7468 6174 2079 6f75  rovided that you
+00004c40: 2063 6f6e 7370 6963 756f 7573 6c79 2061   conspicuously a
+00004c50: 6e64 0d0a 6170 7072 6f70 7269 6174 656c  nd..appropriatel
+00004c60: 7920 7075 626c 6973 6820 6f6e 2065 6163  y publish on eac
+00004c70: 6820 636f 7079 2061 6e20 6170 7072 6f70  h copy an approp
+00004c80: 7269 6174 6520 636f 7079 7269 6768 7420  riate copyright 
+00004c90: 6e6f 7469 6365 3b0d 0a6b 6565 7020 696e  notice;..keep in
+00004ca0: 7461 6374 2061 6c6c 206e 6f74 6963 6573  tact all notices
+00004cb0: 2073 7461 7469 6e67 2074 6861 7420 7468   stating that th
+00004cc0: 6973 204c 6963 656e 7365 2061 6e64 2061  is License and a
+00004cd0: 6e79 0d0a 6e6f 6e2d 7065 726d 6973 7369  ny..non-permissi
+00004ce0: 7665 2074 6572 6d73 2061 6464 6564 2069  ve terms added i
+00004cf0: 6e20 6163 636f 7264 2077 6974 6820 7365  n accord with se
+00004d00: 6374 696f 6e20 3720 6170 706c 7920 746f  ction 7 apply to
+00004d10: 2074 6865 2063 6f64 653b 0d0a 6b65 6570   the code;..keep
+00004d20: 2069 6e74 6163 7420 616c 6c20 6e6f 7469   intact all noti
+00004d30: 6365 7320 6f66 2074 6865 2061 6273 656e  ces of the absen
+00004d40: 6365 206f 6620 616e 7920 7761 7272 616e  ce of any warran
+00004d50: 7479 3b20 616e 6420 6769 7665 2061 6c6c  ty; and give all
+00004d60: 0d0a 7265 6369 7069 656e 7473 2061 2063  ..recipients a c
+00004d70: 6f70 7920 6f66 2074 6869 7320 4c69 6365  opy of this Lice
+00004d80: 6e73 6520 616c 6f6e 6720 7769 7468 2074  nse along with t
+00004d90: 6865 2050 726f 6772 616d 2e0d 0a0d 0a20  he Program..... 
+00004da0: 2059 6f75 206d 6179 2063 6861 7267 6520   You may charge 
+00004db0: 616e 7920 7072 6963 6520 6f72 206e 6f20  any price or no 
+00004dc0: 7072 6963 6520 666f 7220 6561 6368 2063  price for each c
+00004dd0: 6f70 7920 7468 6174 2079 6f75 2063 6f6e  opy that you con
+00004de0: 7665 792c 0d0a 616e 6420 796f 7520 6d61  vey,..and you ma
+00004df0: 7920 6f66 6665 7220 7375 7070 6f72 7420  y offer support 
+00004e00: 6f72 2077 6172 7261 6e74 7920 7072 6f74  or warranty prot
+00004e10: 6563 7469 6f6e 2066 6f72 2061 2066 6565  ection for a fee
+00004e20: 2e0d 0a0d 0a20 2035 2e20 436f 6e76 6579  .....  5. Convey
+00004e30: 696e 6720 4d6f 6469 6669 6564 2053 6f75  ing Modified Sou
+00004e40: 7263 6520 5665 7273 696f 6e73 2e0d 0a0d  rce Versions....
+00004e50: 0a20 2059 6f75 206d 6179 2063 6f6e 7665  .  You may conve
+00004e60: 7920 6120 776f 726b 2062 6173 6564 206f  y a work based o
+00004e70: 6e20 7468 6520 5072 6f67 7261 6d2c 206f  n the Program, o
+00004e80: 7220 7468 6520 6d6f 6469 6669 6361 7469  r the modificati
+00004e90: 6f6e 7320 746f 0d0a 7072 6f64 7563 6520  ons to..produce 
+00004ea0: 6974 2066 726f 6d20 7468 6520 5072 6f67  it from the Prog
+00004eb0: 7261 6d2c 2069 6e20 7468 6520 666f 726d  ram, in the form
+00004ec0: 206f 6620 736f 7572 6365 2063 6f64 6520   of source code 
+00004ed0: 756e 6465 7220 7468 650d 0a74 6572 6d73  under the..terms
+00004ee0: 206f 6620 7365 6374 696f 6e20 342c 2070   of section 4, p
+00004ef0: 726f 7669 6465 6420 7468 6174 2079 6f75  rovided that you
+00004f00: 2061 6c73 6f20 6d65 6574 2061 6c6c 206f   also meet all o
+00004f10: 6620 7468 6573 6520 636f 6e64 6974 696f  f these conditio
+00004f20: 6e73 3a0d 0a0d 0a20 2020 2061 2920 5468  ns:....    a) Th
+00004f30: 6520 776f 726b 206d 7573 7420 6361 7272  e work must carr
+00004f40: 7920 7072 6f6d 696e 656e 7420 6e6f 7469  y prominent noti
+00004f50: 6365 7320 7374 6174 696e 6720 7468 6174  ces stating that
+00004f60: 2079 6f75 206d 6f64 6966 6965 640d 0a20   you modified.. 
+00004f70: 2020 2069 742c 2061 6e64 2067 6976 696e     it, and givin
+00004f80: 6720 6120 7265 6c65 7661 6e74 2064 6174  g a relevant dat
+00004f90: 652e 0d0a 0d0a 2020 2020 6229 2054 6865  e.....    b) The
+00004fa0: 2077 6f72 6b20 6d75 7374 2063 6172 7279   work must carry
+00004fb0: 2070 726f 6d69 6e65 6e74 206e 6f74 6963   prominent notic
+00004fc0: 6573 2073 7461 7469 6e67 2074 6861 7420  es stating that 
+00004fd0: 6974 2069 730d 0a20 2020 2072 656c 6561  it is..    relea
+00004fe0: 7365 6420 756e 6465 7220 7468 6973 204c  sed under this L
+00004ff0: 6963 656e 7365 2061 6e64 2061 6e79 2063  icense and any c
+00005000: 6f6e 6469 7469 6f6e 7320 6164 6465 6420  onditions added 
+00005010: 756e 6465 7220 7365 6374 696f 6e0d 0a20  under section.. 
+00005020: 2020 2037 2e20 2054 6869 7320 7265 7175     7.  This requ
+00005030: 6972 656d 656e 7420 6d6f 6469 6669 6573  irement modifies
+00005040: 2074 6865 2072 6571 7569 7265 6d65 6e74   the requirement
+00005050: 2069 6e20 7365 6374 696f 6e20 3420 746f   in section 4 to
+00005060: 0d0a 2020 2020 226b 6565 7020 696e 7461  ..    "keep inta
+00005070: 6374 2061 6c6c 206e 6f74 6963 6573 222e  ct all notices".
+00005080: 0d0a 0d0a 2020 2020 6329 2059 6f75 206d  ....    c) You m
+00005090: 7573 7420 6c69 6365 6e73 6520 7468 6520  ust license the 
+000050a0: 656e 7469 7265 2077 6f72 6b2c 2061 7320  entire work, as 
+000050b0: 6120 7768 6f6c 652c 2075 6e64 6572 2074  a whole, under t
+000050c0: 6869 730d 0a20 2020 204c 6963 656e 7365  his..    License
+000050d0: 2074 6f20 616e 796f 6e65 2077 686f 2063   to anyone who c
+000050e0: 6f6d 6573 2069 6e74 6f20 706f 7373 6573  omes into posses
+000050f0: 7369 6f6e 206f 6620 6120 636f 7079 2e20  sion of a copy. 
+00005100: 2054 6869 730d 0a20 2020 204c 6963 656e   This..    Licen
+00005110: 7365 2077 696c 6c20 7468 6572 6566 6f72  se will therefor
+00005120: 6520 6170 706c 792c 2061 6c6f 6e67 2077  e apply, along w
+00005130: 6974 6820 616e 7920 6170 706c 6963 6162  ith any applicab
+00005140: 6c65 2073 6563 7469 6f6e 2037 0d0a 2020  le section 7..  
+00005150: 2020 6164 6469 7469 6f6e 616c 2074 6572    additional ter
+00005160: 6d73 2c20 746f 2074 6865 2077 686f 6c65  ms, to the whole
+00005170: 206f 6620 7468 6520 776f 726b 2c20 616e   of the work, an
+00005180: 6420 616c 6c20 6974 7320 7061 7274 732c  d all its parts,
+00005190: 0d0a 2020 2020 7265 6761 7264 6c65 7373  ..    regardless
+000051a0: 206f 6620 686f 7720 7468 6579 2061 7265   of how they are
+000051b0: 2070 6163 6b61 6765 642e 2020 5468 6973   packaged.  This
+000051c0: 204c 6963 656e 7365 2067 6976 6573 206e   License gives n
+000051d0: 6f0d 0a20 2020 2070 6572 6d69 7373 696f  o..    permissio
+000051e0: 6e20 746f 206c 6963 656e 7365 2074 6865  n to license the
+000051f0: 2077 6f72 6b20 696e 2061 6e79 206f 7468   work in any oth
+00005200: 6572 2077 6179 2c20 6275 7420 6974 2064  er way, but it d
+00005210: 6f65 7320 6e6f 740d 0a20 2020 2069 6e76  oes not..    inv
+00005220: 616c 6964 6174 6520 7375 6368 2070 6572  alidate such per
+00005230: 6d69 7373 696f 6e20 6966 2079 6f75 2068  mission if you h
+00005240: 6176 6520 7365 7061 7261 7465 6c79 2072  ave separately r
+00005250: 6563 6569 7665 6420 6974 2e0d 0a0d 0a20  eceived it..... 
+00005260: 2020 2064 2920 4966 2074 6865 2077 6f72     d) If the wor
+00005270: 6b20 6861 7320 696e 7465 7261 6374 6976  k has interactiv
+00005280: 6520 7573 6572 2069 6e74 6572 6661 6365  e user interface
+00005290: 732c 2065 6163 6820 6d75 7374 2064 6973  s, each must dis
+000052a0: 706c 6179 0d0a 2020 2020 4170 7072 6f70  play..    Approp
+000052b0: 7269 6174 6520 4c65 6761 6c20 4e6f 7469  riate Legal Noti
+000052c0: 6365 733b 2068 6f77 6576 6572 2c20 6966  ces; however, if
+000052d0: 2074 6865 2050 726f 6772 616d 2068 6173   the Program has
+000052e0: 2069 6e74 6572 6163 7469 7665 0d0a 2020   interactive..  
+000052f0: 2020 696e 7465 7266 6163 6573 2074 6861    interfaces tha
+00005300: 7420 646f 206e 6f74 2064 6973 706c 6179  t do not display
+00005310: 2041 7070 726f 7072 6961 7465 204c 6567   Appropriate Leg
+00005320: 616c 204e 6f74 6963 6573 2c20 796f 7572  al Notices, your
+00005330: 0d0a 2020 2020 776f 726b 206e 6565 6420  ..    work need 
+00005340: 6e6f 7420 6d61 6b65 2074 6865 6d20 646f  not make them do
+00005350: 2073 6f2e 0d0a 0d0a 2020 4120 636f 6d70   so.....  A comp
+00005360: 696c 6174 696f 6e20 6f66 2061 2063 6f76  ilation of a cov
+00005370: 6572 6564 2077 6f72 6b20 7769 7468 206f  ered work with o
+00005380: 7468 6572 2073 6570 6172 6174 6520 616e  ther separate an
+00005390: 6420 696e 6465 7065 6e64 656e 740d 0a77  d independent..w
+000053a0: 6f72 6b73 2c20 7768 6963 6820 6172 6520  orks, which are 
+000053b0: 6e6f 7420 6279 2074 6865 6972 206e 6174  not by their nat
+000053c0: 7572 6520 6578 7465 6e73 696f 6e73 206f  ure extensions o
+000053d0: 6620 7468 6520 636f 7665 7265 6420 776f  f the covered wo
+000053e0: 726b 2c0d 0a61 6e64 2077 6869 6368 2061  rk,..and which a
+000053f0: 7265 206e 6f74 2063 6f6d 6269 6e65 6420  re not combined 
+00005400: 7769 7468 2069 7420 7375 6368 2061 7320  with it such as 
+00005410: 746f 2066 6f72 6d20 6120 6c61 7267 6572  to form a larger
+00005420: 2070 726f 6772 616d 2c0d 0a69 6e20 6f72   program,..in or
+00005430: 206f 6e20 6120 766f 6c75 6d65 206f 6620   on a volume of 
+00005440: 6120 7374 6f72 6167 6520 6f72 2064 6973  a storage or dis
+00005450: 7472 6962 7574 696f 6e20 6d65 6469 756d  tribution medium
+00005460: 2c20 6973 2063 616c 6c65 6420 616e 0d0a  , is called an..
+00005470: 2261 6767 7265 6761 7465 2220 6966 2074  "aggregate" if t
+00005480: 6865 2063 6f6d 7069 6c61 7469 6f6e 2061  he compilation a
+00005490: 6e64 2069 7473 2072 6573 756c 7469 6e67  nd its resulting
+000054a0: 2063 6f70 7972 6967 6874 2061 7265 206e   copyright are n
+000054b0: 6f74 0d0a 7573 6564 2074 6f20 6c69 6d69  ot..used to limi
+000054c0: 7420 7468 6520 6163 6365 7373 206f 7220  t the access or 
+000054d0: 6c65 6761 6c20 7269 6768 7473 206f 6620  legal rights of 
+000054e0: 7468 6520 636f 6d70 696c 6174 696f 6e27  the compilation'
+000054f0: 7320 7573 6572 730d 0a62 6579 6f6e 6420  s users..beyond 
+00005500: 7768 6174 2074 6865 2069 6e64 6976 6964  what the individ
+00005510: 7561 6c20 776f 726b 7320 7065 726d 6974  ual works permit
+00005520: 2e20 2049 6e63 6c75 7369 6f6e 206f 6620  .  Inclusion of 
+00005530: 6120 636f 7665 7265 6420 776f 726b 0d0a  a covered work..
+00005540: 696e 2061 6e20 6167 6772 6567 6174 6520  in an aggregate 
+00005550: 646f 6573 206e 6f74 2063 6175 7365 2074  does not cause t
+00005560: 6869 7320 4c69 6365 6e73 6520 746f 2061  his License to a
+00005570: 7070 6c79 2074 6f20 7468 6520 6f74 6865  pply to the othe
+00005580: 720d 0a70 6172 7473 206f 6620 7468 6520  r..parts of the 
+00005590: 6167 6772 6567 6174 652e 0d0a 0d0a 2020  aggregate.....  
+000055a0: 362e 2043 6f6e 7665 7969 6e67 204e 6f6e  6. Conveying Non
+000055b0: 2d53 6f75 7263 6520 466f 726d 732e 0d0a  -Source Forms...
+000055c0: 0d0a 2020 596f 7520 6d61 7920 636f 6e76  ..  You may conv
+000055d0: 6579 2061 2063 6f76 6572 6564 2077 6f72  ey a covered wor
+000055e0: 6b20 696e 206f 626a 6563 7420 636f 6465  k in object code
+000055f0: 2066 6f72 6d20 756e 6465 7220 7468 6520   form under the 
+00005600: 7465 726d 730d 0a6f 6620 7365 6374 696f  terms..of sectio
+00005610: 6e73 2034 2061 6e64 2035 2c20 7072 6f76  ns 4 and 5, prov
+00005620: 6964 6564 2074 6861 7420 796f 7520 616c  ided that you al
+00005630: 736f 2063 6f6e 7665 7920 7468 650d 0a6d  so convey the..m
+00005640: 6163 6869 6e65 2d72 6561 6461 626c 6520  achine-readable 
+00005650: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
+00005660: 7572 6365 2075 6e64 6572 2074 6865 2074  urce under the t
+00005670: 6572 6d73 206f 6620 7468 6973 204c 6963  erms of this Lic
+00005680: 656e 7365 2c0d 0a69 6e20 6f6e 6520 6f66  ense,..in one of
+00005690: 2074 6865 7365 2077 6179 733a 0d0a 0d0a   these ways:....
+000056a0: 2020 2020 6129 2043 6f6e 7665 7920 7468      a) Convey th
+000056b0: 6520 6f62 6a65 6374 2063 6f64 6520 696e  e object code in
+000056c0: 2c20 6f72 2065 6d62 6f64 6965 6420 696e  , or embodied in
+000056d0: 2c20 6120 7068 7973 6963 616c 2070 726f  , a physical pro
+000056e0: 6475 6374 0d0a 2020 2020 2869 6e63 6c75  duct..    (inclu
+000056f0: 6469 6e67 2061 2070 6879 7369 6361 6c20  ding a physical 
+00005700: 6469 7374 7269 6275 7469 6f6e 206d 6564  distribution med
+00005710: 6975 6d29 2c20 6163 636f 6d70 616e 6965  ium), accompanie
+00005720: 6420 6279 2074 6865 0d0a 2020 2020 436f  d by the..    Co
+00005730: 7272 6573 706f 6e64 696e 6720 536f 7572  rresponding Sour
+00005740: 6365 2066 6978 6564 206f 6e20 6120 6475  ce fixed on a du
+00005750: 7261 626c 6520 7068 7973 6963 616c 206d  rable physical m
+00005760: 6564 6975 6d0d 0a20 2020 2063 7573 746f  edium..    custo
+00005770: 6d61 7269 6c79 2075 7365 6420 666f 7220  marily used for 
+00005780: 736f 6674 7761 7265 2069 6e74 6572 6368  software interch
+00005790: 616e 6765 2e0d 0a0d 0a20 2020 2062 2920  ange.....    b) 
+000057a0: 436f 6e76 6579 2074 6865 206f 626a 6563  Convey the objec
+000057b0: 7420 636f 6465 2069 6e2c 206f 7220 656d  t code in, or em
+000057c0: 626f 6469 6564 2069 6e2c 2061 2070 6879  bodied in, a phy
+000057d0: 7369 6361 6c20 7072 6f64 7563 740d 0a20  sical product.. 
+000057e0: 2020 2028 696e 636c 7564 696e 6720 6120     (including a 
+000057f0: 7068 7973 6963 616c 2064 6973 7472 6962  physical distrib
+00005800: 7574 696f 6e20 6d65 6469 756d 292c 2061  ution medium), a
+00005810: 6363 6f6d 7061 6e69 6564 2062 7920 610d  ccompanied by a.
+00005820: 0a20 2020 2077 7269 7474 656e 206f 6666  .    written off
+00005830: 6572 2c20 7661 6c69 6420 666f 7220 6174  er, valid for at
+00005840: 206c 6561 7374 2074 6872 6565 2079 6561   least three yea
+00005850: 7273 2061 6e64 2076 616c 6964 2066 6f72  rs and valid for
+00005860: 2061 730d 0a20 2020 206c 6f6e 6720 6173   as..    long as
+00005870: 2079 6f75 206f 6666 6572 2073 7061 7265   you offer spare
+00005880: 2070 6172 7473 206f 7220 6375 7374 6f6d   parts or custom
+00005890: 6572 2073 7570 706f 7274 2066 6f72 2074  er support for t
+000058a0: 6861 7420 7072 6f64 7563 740d 0a20 2020  hat product..   
+000058b0: 206d 6f64 656c 2c20 746f 2067 6976 6520   model, to give 
+000058c0: 616e 796f 6e65 2077 686f 2070 6f73 7365  anyone who posse
+000058d0: 7373 6573 2074 6865 206f 626a 6563 7420  sses the object 
+000058e0: 636f 6465 2065 6974 6865 7220 2831 2920  code either (1) 
+000058f0: 610d 0a20 2020 2063 6f70 7920 6f66 2074  a..    copy of t
+00005900: 6865 2043 6f72 7265 7370 6f6e 6469 6e67  he Corresponding
+00005910: 2053 6f75 7263 6520 666f 7220 616c 6c20   Source for all 
+00005920: 7468 6520 736f 6674 7761 7265 2069 6e20  the software in 
+00005930: 7468 650d 0a20 2020 2070 726f 6475 6374  the..    product
+00005940: 2074 6861 7420 6973 2063 6f76 6572 6564   that is covered
+00005950: 2062 7920 7468 6973 204c 6963 656e 7365   by this License
+00005960: 2c20 6f6e 2061 2064 7572 6162 6c65 2070  , on a durable p
+00005970: 6879 7369 6361 6c0d 0a20 2020 206d 6564  hysical..    med
+00005980: 6975 6d20 6375 7374 6f6d 6172 696c 7920  ium customarily 
+00005990: 7573 6564 2066 6f72 2073 6f66 7477 6172  used for softwar
+000059a0: 6520 696e 7465 7263 6861 6e67 652c 2066  e interchange, f
+000059b0: 6f72 2061 2070 7269 6365 206e 6f0d 0a20  or a price no.. 
+000059c0: 2020 206d 6f72 6520 7468 616e 2079 6f75     more than you
+000059d0: 7220 7265 6173 6f6e 6162 6c65 2063 6f73  r reasonable cos
+000059e0: 7420 6f66 2070 6879 7369 6361 6c6c 7920  t of physically 
+000059f0: 7065 7266 6f72 6d69 6e67 2074 6869 730d  performing this.
+00005a00: 0a20 2020 2063 6f6e 7665 7969 6e67 206f  .    conveying o
+00005a10: 6620 736f 7572 6365 2c20 6f72 2028 3229  f source, or (2)
+00005a20: 2061 6363 6573 7320 746f 2063 6f70 7920   access to copy 
+00005a30: 7468 650d 0a20 2020 2043 6f72 7265 7370  the..    Corresp
+00005a40: 6f6e 6469 6e67 2053 6f75 7263 6520 6672  onding Source fr
+00005a50: 6f6d 2061 206e 6574 776f 726b 2073 6572  om a network ser
+00005a60: 7665 7220 6174 206e 6f20 6368 6172 6765  ver at no charge
+00005a70: 2e0d 0a0d 0a20 2020 2063 2920 436f 6e76  .....    c) Conv
+00005a80: 6579 2069 6e64 6976 6964 7561 6c20 636f  ey individual co
+00005a90: 7069 6573 206f 6620 7468 6520 6f62 6a65  pies of the obje
+00005aa0: 6374 2063 6f64 6520 7769 7468 2061 2063  ct code with a c
+00005ab0: 6f70 7920 6f66 2074 6865 0d0a 2020 2020  opy of the..    
+00005ac0: 7772 6974 7465 6e20 6f66 6665 7220 746f  written offer to
+00005ad0: 2070 726f 7669 6465 2074 6865 2043 6f72   provide the Cor
+00005ae0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
+00005af0: 652e 2020 5468 6973 0d0a 2020 2020 616c  e.  This..    al
+00005b00: 7465 726e 6174 6976 6520 6973 2061 6c6c  ternative is all
+00005b10: 6f77 6564 206f 6e6c 7920 6f63 6361 7369  owed only occasi
+00005b20: 6f6e 616c 6c79 2061 6e64 206e 6f6e 636f  onally and nonco
+00005b30: 6d6d 6572 6369 616c 6c79 2c20 616e 640d  mmercially, and.
+00005b40: 0a20 2020 206f 6e6c 7920 6966 2079 6f75  .    only if you
+00005b50: 2072 6563 6569 7665 6420 7468 6520 6f62   received the ob
+00005b60: 6a65 6374 2063 6f64 6520 7769 7468 2073  ject code with s
+00005b70: 7563 6820 616e 206f 6666 6572 2c20 696e  uch an offer, in
+00005b80: 2061 6363 6f72 640d 0a20 2020 2077 6974   accord..    wit
+00005b90: 6820 7375 6273 6563 7469 6f6e 2036 622e  h subsection 6b.
+00005ba0: 0d0a 0d0a 2020 2020 6429 2043 6f6e 7665  ....    d) Conve
+00005bb0: 7920 7468 6520 6f62 6a65 6374 2063 6f64  y the object cod
+00005bc0: 6520 6279 206f 6666 6572 696e 6720 6163  e by offering ac
+00005bd0: 6365 7373 2066 726f 6d20 6120 6465 7369  cess from a desi
+00005be0: 676e 6174 6564 0d0a 2020 2020 706c 6163  gnated..    plac
+00005bf0: 6520 2867 7261 7469 7320 6f72 2066 6f72  e (gratis or for
+00005c00: 2061 2063 6861 7267 6529 2c20 616e 6420   a charge), and 
+00005c10: 6f66 6665 7220 6571 7569 7661 6c65 6e74  offer equivalent
+00005c20: 2061 6363 6573 7320 746f 2074 6865 0d0a   access to the..
+00005c30: 2020 2020 436f 7272 6573 706f 6e64 696e      Correspondin
+00005c40: 6720 536f 7572 6365 2069 6e20 7468 6520  g Source in the 
+00005c50: 7361 6d65 2077 6179 2074 6872 6f75 6768  same way through
+00005c60: 2074 6865 2073 616d 6520 706c 6163 6520   the same place 
+00005c70: 6174 206e 6f0d 0a20 2020 2066 7572 7468  at no..    furth
+00005c80: 6572 2063 6861 7267 652e 2020 596f 7520  er charge.  You 
+00005c90: 6e65 6564 206e 6f74 2072 6571 7569 7265  need not require
+00005ca0: 2072 6563 6970 6965 6e74 7320 746f 2063   recipients to c
+00005cb0: 6f70 7920 7468 650d 0a20 2020 2043 6f72  opy the..    Cor
+00005cc0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
+00005cd0: 6520 616c 6f6e 6720 7769 7468 2074 6865  e along with the
+00005ce0: 206f 626a 6563 7420 636f 6465 2e20 2049   object code.  I
+00005cf0: 6620 7468 6520 706c 6163 6520 746f 0d0a  f the place to..
+00005d00: 2020 2020 636f 7079 2074 6865 206f 626a      copy the obj
+00005d10: 6563 7420 636f 6465 2069 7320 6120 6e65  ect code is a ne
+00005d20: 7477 6f72 6b20 7365 7276 6572 2c20 7468  twork server, th
+00005d30: 6520 436f 7272 6573 706f 6e64 696e 6720  e Corresponding 
+00005d40: 536f 7572 6365 0d0a 2020 2020 6d61 7920  Source..    may 
+00005d50: 6265 206f 6e20 6120 6469 6666 6572 656e  be on a differen
+00005d60: 7420 7365 7276 6572 2028 6f70 6572 6174  t server (operat
+00005d70: 6564 2062 7920 796f 7520 6f72 2061 2074  ed by you or a t
+00005d80: 6869 7264 2070 6172 7479 290d 0a20 2020  hird party)..   
+00005d90: 2074 6861 7420 7375 7070 6f72 7473 2065   that supports e
+00005da0: 7175 6976 616c 656e 7420 636f 7079 696e  quivalent copyin
+00005db0: 6720 6661 6369 6c69 7469 6573 2c20 7072  g facilities, pr
+00005dc0: 6f76 6964 6564 2079 6f75 206d 6169 6e74  ovided you maint
+00005dd0: 6169 6e0d 0a20 2020 2063 6c65 6172 2064  ain..    clear d
+00005de0: 6972 6563 7469 6f6e 7320 6e65 7874 2074  irections next t
+00005df0: 6f20 7468 6520 6f62 6a65 6374 2063 6f64  o the object cod
+00005e00: 6520 7361 7969 6e67 2077 6865 7265 2074  e saying where t
+00005e10: 6f20 6669 6e64 2074 6865 0d0a 2020 2020  o find the..    
+00005e20: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
+00005e30: 7572 6365 2e20 2052 6567 6172 646c 6573  urce.  Regardles
+00005e40: 7320 6f66 2077 6861 7420 7365 7276 6572  s of what server
+00005e50: 2068 6f73 7473 2074 6865 0d0a 2020 2020   hosts the..    
+00005e60: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
+00005e70: 7572 6365 2c20 796f 7520 7265 6d61 696e  urce, you remain
+00005e80: 206f 626c 6967 6174 6564 2074 6f20 656e   obligated to en
+00005e90: 7375 7265 2074 6861 7420 6974 2069 730d  sure that it is.
+00005ea0: 0a20 2020 2061 7661 696c 6162 6c65 2066  .    available f
+00005eb0: 6f72 2061 7320 6c6f 6e67 2061 7320 6e65  or as long as ne
+00005ec0: 6564 6564 2074 6f20 7361 7469 7366 7920  eded to satisfy 
+00005ed0: 7468 6573 6520 7265 7175 6972 656d 656e  these requiremen
+00005ee0: 7473 2e0d 0a0d 0a20 2020 2065 2920 436f  ts.....    e) Co
+00005ef0: 6e76 6579 2074 6865 206f 626a 6563 7420  nvey the object 
+00005f00: 636f 6465 2075 7369 6e67 2070 6565 722d  code using peer-
+00005f10: 746f 2d70 6565 7220 7472 616e 736d 6973  to-peer transmis
+00005f20: 7369 6f6e 2c20 7072 6f76 6964 6564 0d0a  sion, provided..
+00005f30: 2020 2020 796f 7520 696e 666f 726d 206f      you inform o
+00005f40: 7468 6572 2070 6565 7273 2077 6865 7265  ther peers where
+00005f50: 2074 6865 206f 626a 6563 7420 636f 6465   the object code
+00005f60: 2061 6e64 2043 6f72 7265 7370 6f6e 6469   and Correspondi
+00005f70: 6e67 0d0a 2020 2020 536f 7572 6365 206f  ng..    Source o
+00005f80: 6620 7468 6520 776f 726b 2061 7265 2062  f the work are b
+00005f90: 6569 6e67 206f 6666 6572 6564 2074 6f20  eing offered to 
+00005fa0: 7468 6520 6765 6e65 7261 6c20 7075 626c  the general publ
+00005fb0: 6963 2061 7420 6e6f 0d0a 2020 2020 6368  ic at no..    ch
+00005fc0: 6172 6765 2075 6e64 6572 2073 7562 7365  arge under subse
+00005fd0: 6374 696f 6e20 3664 2e0d 0a0d 0a20 2041  ction 6d.....  A
+00005fe0: 2073 6570 6172 6162 6c65 2070 6f72 7469   separable porti
+00005ff0: 6f6e 206f 6620 7468 6520 6f62 6a65 6374  on of the object
+00006000: 2063 6f64 652c 2077 686f 7365 2073 6f75   code, whose sou
+00006010: 7263 6520 636f 6465 2069 7320 6578 636c  rce code is excl
+00006020: 7564 6564 0d0a 6672 6f6d 2074 6865 2043  uded..from the C
+00006030: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
+00006040: 7263 6520 6173 2061 2053 7973 7465 6d20  rce as a System 
+00006050: 4c69 6272 6172 792c 206e 6565 6420 6e6f  Library, need no
+00006060: 7420 6265 0d0a 696e 636c 7564 6564 2069  t be..included i
+00006070: 6e20 636f 6e76 6579 696e 6720 7468 6520  n conveying the 
+00006080: 6f62 6a65 6374 2063 6f64 6520 776f 726b  object code work
+00006090: 2e0d 0a0d 0a20 2041 2022 5573 6572 2050  .....  A "User P
+000060a0: 726f 6475 6374 2220 6973 2065 6974 6865  roduct" is eithe
+000060b0: 7220 2831 2920 6120 2263 6f6e 7375 6d65  r (1) a "consume
+000060c0: 7220 7072 6f64 7563 7422 2c20 7768 6963  r product", whic
+000060d0: 6820 6d65 616e 7320 616e 790d 0a74 616e  h means any..tan
+000060e0: 6769 626c 6520 7065 7273 6f6e 616c 2070  gible personal p
+000060f0: 726f 7065 7274 7920 7768 6963 6820 6973  roperty which is
+00006100: 206e 6f72 6d61 6c6c 7920 7573 6564 2066   normally used f
+00006110: 6f72 2070 6572 736f 6e61 6c2c 2066 616d  or personal, fam
+00006120: 696c 792c 0d0a 6f72 2068 6f75 7365 686f  ily,..or househo
+00006130: 6c64 2070 7572 706f 7365 732c 206f 7220  ld purposes, or 
+00006140: 2832 2920 616e 7974 6869 6e67 2064 6573  (2) anything des
+00006150: 6967 6e65 6420 6f72 2073 6f6c 6420 666f  igned or sold fo
+00006160: 7220 696e 636f 7270 6f72 6174 696f 6e0d  r incorporation.
+00006170: 0a69 6e74 6f20 6120 6477 656c 6c69 6e67  .into a dwelling
+00006180: 2e20 2049 6e20 6465 7465 726d 696e 696e  .  In determinin
+00006190: 6720 7768 6574 6865 7220 6120 7072 6f64  g whether a prod
+000061a0: 7563 7420 6973 2061 2063 6f6e 7375 6d65  uct is a consume
+000061b0: 7220 7072 6f64 7563 742c 0d0a 646f 7562  r product,..doub
+000061c0: 7466 756c 2063 6173 6573 2073 6861 6c6c  tful cases shall
+000061d0: 2062 6520 7265 736f 6c76 6564 2069 6e20   be resolved in 
+000061e0: 6661 766f 7220 6f66 2063 6f76 6572 6167  favor of coverag
+000061f0: 652e 2020 466f 7220 6120 7061 7274 6963  e.  For a partic
+00006200: 756c 6172 0d0a 7072 6f64 7563 7420 7265  ular..product re
+00006210: 6365 6976 6564 2062 7920 6120 7061 7274  ceived by a part
+00006220: 6963 756c 6172 2075 7365 722c 2022 6e6f  icular user, "no
+00006230: 726d 616c 6c79 2075 7365 6422 2072 6566  rmally used" ref
+00006240: 6572 7320 746f 2061 0d0a 7479 7069 6361  ers to a..typica
+00006250: 6c20 6f72 2063 6f6d 6d6f 6e20 7573 6520  l or common use 
+00006260: 6f66 2074 6861 7420 636c 6173 7320 6f66  of that class of
+00006270: 2070 726f 6475 6374 2c20 7265 6761 7264   product, regard
+00006280: 6c65 7373 206f 6620 7468 6520 7374 6174  less of the stat
+00006290: 7573 0d0a 6f66 2074 6865 2070 6172 7469  us..of the parti
+000062a0: 6375 6c61 7220 7573 6572 206f 7220 6f66  cular user or of
+000062b0: 2074 6865 2077 6179 2069 6e20 7768 6963   the way in whic
+000062c0: 6820 7468 6520 7061 7274 6963 756c 6172  h the particular
+000062d0: 2075 7365 720d 0a61 6374 7561 6c6c 7920   user..actually 
+000062e0: 7573 6573 2c20 6f72 2065 7870 6563 7473  uses, or expects
+000062f0: 206f 7220 6973 2065 7870 6563 7465 6420   or is expected 
+00006300: 746f 2075 7365 2c20 7468 6520 7072 6f64  to use, the prod
+00006310: 7563 742e 2020 4120 7072 6f64 7563 740d  uct.  A product.
+00006320: 0a69 7320 6120 636f 6e73 756d 6572 2070  .is a consumer p
+00006330: 726f 6475 6374 2072 6567 6172 646c 6573  roduct regardles
+00006340: 7320 6f66 2077 6865 7468 6572 2074 6865  s of whether the
+00006350: 2070 726f 6475 6374 2068 6173 2073 7562   product has sub
+00006360: 7374 616e 7469 616c 0d0a 636f 6d6d 6572  stantial..commer
+00006370: 6369 616c 2c20 696e 6475 7374 7269 616c  cial, industrial
+00006380: 206f 7220 6e6f 6e2d 636f 6e73 756d 6572   or non-consumer
+00006390: 2075 7365 732c 2075 6e6c 6573 7320 7375   uses, unless su
+000063a0: 6368 2075 7365 7320 7265 7072 6573 656e  ch uses represen
+000063b0: 740d 0a74 6865 206f 6e6c 7920 7369 676e  t..the only sign
+000063c0: 6966 6963 616e 7420 6d6f 6465 206f 6620  ificant mode of 
+000063d0: 7573 6520 6f66 2074 6865 2070 726f 6475  use of the produ
+000063e0: 6374 2e0d 0a0d 0a20 2022 496e 7374 616c  ct.....  "Instal
+000063f0: 6c61 7469 6f6e 2049 6e66 6f72 6d61 7469  lation Informati
+00006400: 6f6e 2220 666f 7220 6120 5573 6572 2050  on" for a User P
+00006410: 726f 6475 6374 206d 6561 6e73 2061 6e79  roduct means any
+00006420: 206d 6574 686f 6473 2c0d 0a70 726f 6365   methods,..proce
+00006430: 6475 7265 732c 2061 7574 686f 7269 7a61  dures, authoriza
+00006440: 7469 6f6e 206b 6579 732c 206f 7220 6f74  tion keys, or ot
+00006450: 6865 7220 696e 666f 726d 6174 696f 6e20  her information 
+00006460: 7265 7175 6972 6564 2074 6f20 696e 7374  required to inst
+00006470: 616c 6c0d 0a61 6e64 2065 7865 6375 7465  all..and execute
+00006480: 206d 6f64 6966 6965 6420 7665 7273 696f   modified versio
+00006490: 6e73 206f 6620 6120 636f 7665 7265 6420  ns of a covered 
+000064a0: 776f 726b 2069 6e20 7468 6174 2055 7365  work in that Use
+000064b0: 7220 5072 6f64 7563 7420 6672 6f6d 0d0a  r Product from..
+000064c0: 6120 6d6f 6469 6669 6564 2076 6572 7369  a modified versi
+000064d0: 6f6e 206f 6620 6974 7320 436f 7272 6573  on of its Corres
+000064e0: 706f 6e64 696e 6720 536f 7572 6365 2e20  ponding Source. 
+000064f0: 2054 6865 2069 6e66 6f72 6d61 7469 6f6e   The information
+00006500: 206d 7573 740d 0a73 7566 6669 6365 2074   must..suffice t
+00006510: 6f20 656e 7375 7265 2074 6861 7420 7468  o ensure that th
+00006520: 6520 636f 6e74 696e 7565 6420 6675 6e63  e continued func
+00006530: 7469 6f6e 696e 6720 6f66 2074 6865 206d  tioning of the m
+00006540: 6f64 6966 6965 6420 6f62 6a65 6374 0d0a  odified object..
+00006550: 636f 6465 2069 7320 696e 206e 6f20 6361  code is in no ca
+00006560: 7365 2070 7265 7665 6e74 6564 206f 7220  se prevented or 
+00006570: 696e 7465 7266 6572 6564 2077 6974 6820  interfered with 
+00006580: 736f 6c65 6c79 2062 6563 6175 7365 0d0a  solely because..
+00006590: 6d6f 6469 6669 6361 7469 6f6e 2068 6173  modification has
+000065a0: 2062 6565 6e20 6d61 6465 2e0d 0a0d 0a20   been made..... 
+000065b0: 2049 6620 796f 7520 636f 6e76 6579 2061   If you convey a
+000065c0: 6e20 6f62 6a65 6374 2063 6f64 6520 776f  n object code wo
+000065d0: 726b 2075 6e64 6572 2074 6869 7320 7365  rk under this se
+000065e0: 6374 696f 6e20 696e 2c20 6f72 2077 6974  ction in, or wit
+000065f0: 682c 206f 720d 0a73 7065 6369 6669 6361  h, or..specifica
+00006600: 6c6c 7920 666f 7220 7573 6520 696e 2c20  lly for use in, 
+00006610: 6120 5573 6572 2050 726f 6475 6374 2c20  a User Product, 
+00006620: 616e 6420 7468 6520 636f 6e76 6579 696e  and the conveyin
+00006630: 6720 6f63 6375 7273 2061 730d 0a70 6172  g occurs as..par
+00006640: 7420 6f66 2061 2074 7261 6e73 6163 7469  t of a transacti
+00006650: 6f6e 2069 6e20 7768 6963 6820 7468 6520  on in which the 
+00006660: 7269 6768 7420 6f66 2070 6f73 7365 7373  right of possess
+00006670: 696f 6e20 616e 6420 7573 6520 6f66 2074  ion and use of t
+00006680: 6865 0d0a 5573 6572 2050 726f 6475 6374  he..User Product
+00006690: 2069 7320 7472 616e 7366 6572 7265 6420   is transferred 
+000066a0: 746f 2074 6865 2072 6563 6970 6965 6e74  to the recipient
+000066b0: 2069 6e20 7065 7270 6574 7569 7479 206f   in perpetuity o
+000066c0: 7220 666f 7220 610d 0a66 6978 6564 2074  r for a..fixed t
+000066d0: 6572 6d20 2872 6567 6172 646c 6573 7320  erm (regardless 
+000066e0: 6f66 2068 6f77 2074 6865 2074 7261 6e73  of how the trans
+000066f0: 6163 7469 6f6e 2069 7320 6368 6172 6163  action is charac
+00006700: 7465 7269 7a65 6429 2c20 7468 650d 0a43  terized), the..C
+00006710: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
+00006720: 7263 6520 636f 6e76 6579 6564 2075 6e64  rce conveyed und
+00006730: 6572 2074 6869 7320 7365 6374 696f 6e20  er this section 
+00006740: 6d75 7374 2062 6520 6163 636f 6d70 616e  must be accompan
+00006750: 6965 640d 0a62 7920 7468 6520 496e 7374  ied..by the Inst
+00006760: 616c 6c61 7469 6f6e 2049 6e66 6f72 6d61  allation Informa
+00006770: 7469 6f6e 2e20 2042 7574 2074 6869 7320  tion.  But this 
+00006780: 7265 7175 6972 656d 656e 7420 646f 6573  requirement does
+00006790: 206e 6f74 2061 7070 6c79 0d0a 6966 206e   not apply..if n
+000067a0: 6569 7468 6572 2079 6f75 206e 6f72 2061  either you nor a
+000067b0: 6e79 2074 6869 7264 2070 6172 7479 2072  ny third party r
+000067c0: 6574 6169 6e73 2074 6865 2061 6269 6c69  etains the abili
+000067d0: 7479 2074 6f20 696e 7374 616c 6c0d 0a6d  ty to install..m
+000067e0: 6f64 6966 6965 6420 6f62 6a65 6374 2063  odified object c
+000067f0: 6f64 6520 6f6e 2074 6865 2055 7365 7220  ode on the User 
+00006800: 5072 6f64 7563 7420 2866 6f72 2065 7861  Product (for exa
+00006810: 6d70 6c65 2c20 7468 6520 776f 726b 2068  mple, the work h
+00006820: 6173 0d0a 6265 656e 2069 6e73 7461 6c6c  as..been install
+00006830: 6564 2069 6e20 524f 4d29 2e0d 0a0d 0a20  ed in ROM)..... 
+00006840: 2054 6865 2072 6571 7569 7265 6d65 6e74   The requirement
+00006850: 2074 6f20 7072 6f76 6964 6520 496e 7374   to provide Inst
+00006860: 616c 6c61 7469 6f6e 2049 6e66 6f72 6d61  allation Informa
+00006870: 7469 6f6e 2064 6f65 7320 6e6f 7420 696e  tion does not in
+00006880: 636c 7564 6520 610d 0a72 6571 7569 7265  clude a..require
+00006890: 6d65 6e74 2074 6f20 636f 6e74 696e 7565  ment to continue
+000068a0: 2074 6f20 7072 6f76 6964 6520 7375 7070   to provide supp
+000068b0: 6f72 7420 7365 7276 6963 652c 2077 6172  ort service, war
+000068c0: 7261 6e74 792c 206f 7220 7570 6461 7465  ranty, or update
+000068d0: 730d 0a66 6f72 2061 2077 6f72 6b20 7468  s..for a work th
+000068e0: 6174 2068 6173 2062 6565 6e20 6d6f 6469  at has been modi
+000068f0: 6669 6564 206f 7220 696e 7374 616c 6c65  fied or installe
+00006900: 6420 6279 2074 6865 2072 6563 6970 6965  d by the recipie
+00006910: 6e74 2c20 6f72 2066 6f72 0d0a 7468 6520  nt, or for..the 
+00006920: 5573 6572 2050 726f 6475 6374 2069 6e20  User Product in 
+00006930: 7768 6963 6820 6974 2068 6173 2062 6565  which it has bee
+00006940: 6e20 6d6f 6469 6669 6564 206f 7220 696e  n modified or in
+00006950: 7374 616c 6c65 642e 2020 4163 6365 7373  stalled.  Access
+00006960: 2074 6f20 610d 0a6e 6574 776f 726b 206d   to a..network m
+00006970: 6179 2062 6520 6465 6e69 6564 2077 6865  ay be denied whe
+00006980: 6e20 7468 6520 6d6f 6469 6669 6361 7469  n the modificati
+00006990: 6f6e 2069 7473 656c 6620 6d61 7465 7269  on itself materi
+000069a0: 616c 6c79 2061 6e64 0d0a 6164 7665 7273  ally and..advers
+000069b0: 656c 7920 6166 6665 6374 7320 7468 6520  ely affects the 
+000069c0: 6f70 6572 6174 696f 6e20 6f66 2074 6865  operation of the
+000069d0: 206e 6574 776f 726b 206f 7220 7669 6f6c   network or viol
+000069e0: 6174 6573 2074 6865 2072 756c 6573 2061  ates the rules a
+000069f0: 6e64 0d0a 7072 6f74 6f63 6f6c 7320 666f  nd..protocols fo
+00006a00: 7220 636f 6d6d 756e 6963 6174 696f 6e20  r communication 
+00006a10: 6163 726f 7373 2074 6865 206e 6574 776f  across the netwo
+00006a20: 726b 2e0d 0a0d 0a20 2043 6f72 7265 7370  rk.....  Corresp
+00006a30: 6f6e 6469 6e67 2053 6f75 7263 6520 636f  onding Source co
+00006a40: 6e76 6579 6564 2c20 616e 6420 496e 7374  nveyed, and Inst
+00006a50: 616c 6c61 7469 6f6e 2049 6e66 6f72 6d61  allation Informa
+00006a60: 7469 6f6e 2070 726f 7669 6465 642c 0d0a  tion provided,..
+00006a70: 696e 2061 6363 6f72 6420 7769 7468 2074  in accord with t
+00006a80: 6869 7320 7365 6374 696f 6e20 6d75 7374  his section must
+00006a90: 2062 6520 696e 2061 2066 6f72 6d61 7420   be in a format 
+00006aa0: 7468 6174 2069 7320 7075 626c 6963 6c79  that is publicly
+00006ab0: 0d0a 646f 6375 6d65 6e74 6564 2028 616e  ..documented (an
+00006ac0: 6420 7769 7468 2061 6e20 696d 706c 656d  d with an implem
+00006ad0: 656e 7461 7469 6f6e 2061 7661 696c 6162  entation availab
+00006ae0: 6c65 2074 6f20 7468 6520 7075 626c 6963  le to the public
+00006af0: 2069 6e0d 0a73 6f75 7263 6520 636f 6465   in..source code
+00006b00: 2066 6f72 6d29 2c20 616e 6420 6d75 7374   form), and must
+00006b10: 2072 6571 7569 7265 206e 6f20 7370 6563   require no spec
+00006b20: 6961 6c20 7061 7373 776f 7264 206f 7220  ial password or 
+00006b30: 6b65 7920 666f 720d 0a75 6e70 6163 6b69  key for..unpacki
+00006b40: 6e67 2c20 7265 6164 696e 6720 6f72 2063  ng, reading or c
+00006b50: 6f70 7969 6e67 2e0d 0a0d 0a20 2037 2e20  opying.....  7. 
+00006b60: 4164 6469 7469 6f6e 616c 2054 6572 6d73  Additional Terms
+00006b70: 2e0d 0a0d 0a20 2022 4164 6469 7469 6f6e  .....  "Addition
+00006b80: 616c 2070 6572 6d69 7373 696f 6e73 2220  al permissions" 
+00006b90: 6172 6520 7465 726d 7320 7468 6174 2073  are terms that s
+00006ba0: 7570 706c 656d 656e 7420 7468 6520 7465  upplement the te
+00006bb0: 726d 7320 6f66 2074 6869 730d 0a4c 6963  rms of this..Lic
+00006bc0: 656e 7365 2062 7920 6d61 6b69 6e67 2065  ense by making e
+00006bd0: 7863 6570 7469 6f6e 7320 6672 6f6d 206f  xceptions from o
+00006be0: 6e65 206f 7220 6d6f 7265 206f 6620 6974  ne or more of it
+00006bf0: 7320 636f 6e64 6974 696f 6e73 2e0d 0a41  s conditions...A
+00006c00: 6464 6974 696f 6e61 6c20 7065 726d 6973  dditional permis
+00006c10: 7369 6f6e 7320 7468 6174 2061 7265 2061  sions that are a
+00006c20: 7070 6c69 6361 626c 6520 746f 2074 6865  pplicable to the
+00006c30: 2065 6e74 6972 6520 5072 6f67 7261 6d20   entire Program 
+00006c40: 7368 616c 6c0d 0a62 6520 7472 6561 7465  shall..be treate
+00006c50: 6420 6173 2074 686f 7567 6820 7468 6579  d as though they
+00006c60: 2077 6572 6520 696e 636c 7564 6564 2069   were included i
+00006c70: 6e20 7468 6973 204c 6963 656e 7365 2c20  n this License, 
+00006c80: 746f 2074 6865 2065 7874 656e 740d 0a74  to the extent..t
+00006c90: 6861 7420 7468 6579 2061 7265 2076 616c  hat they are val
+00006ca0: 6964 2075 6e64 6572 2061 7070 6c69 6361  id under applica
+00006cb0: 626c 6520 6c61 772e 2020 4966 2061 6464  ble law.  If add
+00006cc0: 6974 696f 6e61 6c20 7065 726d 6973 7369  itional permissi
+00006cd0: 6f6e 730d 0a61 7070 6c79 206f 6e6c 7920  ons..apply only 
+00006ce0: 746f 2070 6172 7420 6f66 2074 6865 2050  to part of the P
+00006cf0: 726f 6772 616d 2c20 7468 6174 2070 6172  rogram, that par
+00006d00: 7420 6d61 7920 6265 2075 7365 6420 7365  t may be used se
+00006d10: 7061 7261 7465 6c79 0d0a 756e 6465 7220  parately..under 
+00006d20: 7468 6f73 6520 7065 726d 6973 7369 6f6e  those permission
+00006d30: 732c 2062 7574 2074 6865 2065 6e74 6972  s, but the entir
+00006d40: 6520 5072 6f67 7261 6d20 7265 6d61 696e  e Program remain
+00006d50: 7320 676f 7665 726e 6564 2062 790d 0a74  s governed by..t
+00006d60: 6869 7320 4c69 6365 6e73 6520 7769 7468  his License with
+00006d70: 6f75 7420 7265 6761 7264 2074 6f20 7468  out regard to th
+00006d80: 6520 6164 6469 7469 6f6e 616c 2070 6572  e additional per
+00006d90: 6d69 7373 696f 6e73 2e0d 0a0d 0a20 2057  missions.....  W
+00006da0: 6865 6e20 796f 7520 636f 6e76 6579 2061  hen you convey a
+00006db0: 2063 6f70 7920 6f66 2061 2063 6f76 6572   copy of a cover
+00006dc0: 6564 2077 6f72 6b2c 2079 6f75 206d 6179  ed work, you may
+00006dd0: 2061 7420 796f 7572 206f 7074 696f 6e0d   at your option.
+00006de0: 0a72 656d 6f76 6520 616e 7920 6164 6469  .remove any addi
+00006df0: 7469 6f6e 616c 2070 6572 6d69 7373 696f  tional permissio
+00006e00: 6e73 2066 726f 6d20 7468 6174 2063 6f70  ns from that cop
+00006e10: 792c 206f 7220 6672 6f6d 2061 6e79 2070  y, or from any p
+00006e20: 6172 7420 6f66 0d0a 6974 2e20 2028 4164  art of..it.  (Ad
+00006e30: 6469 7469 6f6e 616c 2070 6572 6d69 7373  ditional permiss
+00006e40: 696f 6e73 206d 6179 2062 6520 7772 6974  ions may be writ
+00006e50: 7465 6e20 746f 2072 6571 7569 7265 2074  ten to require t
+00006e60: 6865 6972 206f 776e 0d0a 7265 6d6f 7661  heir own..remova
+00006e70: 6c20 696e 2063 6572 7461 696e 2063 6173  l in certain cas
+00006e80: 6573 2077 6865 6e20 796f 7520 6d6f 6469  es when you modi
+00006e90: 6679 2074 6865 2077 6f72 6b2e 2920 2059  fy the work.)  Y
+00006ea0: 6f75 206d 6179 2070 6c61 6365 0d0a 6164  ou may place..ad
+00006eb0: 6469 7469 6f6e 616c 2070 6572 6d69 7373  ditional permiss
+00006ec0: 696f 6e73 206f 6e20 6d61 7465 7269 616c  ions on material
+00006ed0: 2c20 6164 6465 6420 6279 2079 6f75 2074  , added by you t
+00006ee0: 6f20 6120 636f 7665 7265 6420 776f 726b  o a covered work
+00006ef0: 2c0d 0a66 6f72 2077 6869 6368 2079 6f75  ,..for which you
+00006f00: 2068 6176 6520 6f72 2063 616e 2067 6976   have or can giv
+00006f10: 6520 6170 7072 6f70 7269 6174 6520 636f  e appropriate co
+00006f20: 7079 7269 6768 7420 7065 726d 6973 7369  pyright permissi
+00006f30: 6f6e 2e0d 0a0d 0a20 204e 6f74 7769 7468  on.....  Notwith
+00006f40: 7374 616e 6469 6e67 2061 6e79 206f 7468  standing any oth
+00006f50: 6572 2070 726f 7669 7369 6f6e 206f 6620  er provision of 
+00006f60: 7468 6973 204c 6963 656e 7365 2c20 666f  this License, fo
+00006f70: 7220 6d61 7465 7269 616c 2079 6f75 0d0a  r material you..
+00006f80: 6164 6420 746f 2061 2063 6f76 6572 6564  add to a covered
+00006f90: 2077 6f72 6b2c 2079 6f75 206d 6179 2028   work, you may (
+00006fa0: 6966 2061 7574 686f 7269 7a65 6420 6279  if authorized by
+00006fb0: 2074 6865 2063 6f70 7972 6967 6874 2068   the copyright h
+00006fc0: 6f6c 6465 7273 206f 660d 0a74 6861 7420  olders of..that 
+00006fd0: 6d61 7465 7269 616c 2920 7375 7070 6c65  material) supple
+00006fe0: 6d65 6e74 2074 6865 2074 6572 6d73 206f  ment the terms o
+00006ff0: 6620 7468 6973 204c 6963 656e 7365 2077  f this License w
+00007000: 6974 6820 7465 726d 733a 0d0a 0d0a 2020  ith terms:....  
+00007010: 2020 6129 2044 6973 636c 6169 6d69 6e67    a) Disclaiming
+00007020: 2077 6172 7261 6e74 7920 6f72 206c 696d   warranty or lim
+00007030: 6974 696e 6720 6c69 6162 696c 6974 7920  iting liability 
+00007040: 6469 6666 6572 656e 746c 7920 6672 6f6d  differently from
+00007050: 2074 6865 0d0a 2020 2020 7465 726d 7320   the..    terms 
+00007060: 6f66 2073 6563 7469 6f6e 7320 3135 2061  of sections 15 a
+00007070: 6e64 2031 3620 6f66 2074 6869 7320 4c69  nd 16 of this Li
+00007080: 6365 6e73 653b 206f 720d 0a0d 0a20 2020  cense; or....   
+00007090: 2062 2920 5265 7175 6972 696e 6720 7072   b) Requiring pr
+000070a0: 6573 6572 7661 7469 6f6e 206f 6620 7370  eservation of sp
+000070b0: 6563 6966 6965 6420 7265 6173 6f6e 6162  ecified reasonab
+000070c0: 6c65 206c 6567 616c 206e 6f74 6963 6573  le legal notices
+000070d0: 206f 720d 0a20 2020 2061 7574 686f 7220   or..    author 
+000070e0: 6174 7472 6962 7574 696f 6e73 2069 6e20  attributions in 
+000070f0: 7468 6174 206d 6174 6572 6961 6c20 6f72  that material or
+00007100: 2069 6e20 7468 6520 4170 7072 6f70 7269   in the Appropri
+00007110: 6174 6520 4c65 6761 6c0d 0a20 2020 204e  ate Legal..    N
+00007120: 6f74 6963 6573 2064 6973 706c 6179 6564  otices displayed
+00007130: 2062 7920 776f 726b 7320 636f 6e74 6169   by works contai
+00007140: 6e69 6e67 2069 743b 206f 720d 0a0d 0a20  ning it; or.... 
+00007150: 2020 2063 2920 5072 6f68 6962 6974 696e     c) Prohibitin
+00007160: 6720 6d69 7372 6570 7265 7365 6e74 6174  g misrepresentat
+00007170: 696f 6e20 6f66 2074 6865 206f 7269 6769  ion of the origi
+00007180: 6e20 6f66 2074 6861 7420 6d61 7465 7269  n of that materi
+00007190: 616c 2c20 6f72 0d0a 2020 2020 7265 7175  al, or..    requ
+000071a0: 6972 696e 6720 7468 6174 206d 6f64 6966  iring that modif
+000071b0: 6965 6420 7665 7273 696f 6e73 206f 6620  ied versions of 
+000071c0: 7375 6368 206d 6174 6572 6961 6c20 6265  such material be
+000071d0: 206d 6172 6b65 6420 696e 0d0a 2020 2020   marked in..    
+000071e0: 7265 6173 6f6e 6162 6c65 2077 6179 7320  reasonable ways 
+000071f0: 6173 2064 6966 6665 7265 6e74 2066 726f  as different fro
+00007200: 6d20 7468 6520 6f72 6967 696e 616c 2076  m the original v
+00007210: 6572 7369 6f6e 3b20 6f72 0d0a 0d0a 2020  ersion; or....  
+00007220: 2020 6429 204c 696d 6974 696e 6720 7468    d) Limiting th
+00007230: 6520 7573 6520 666f 7220 7075 626c 6963  e use for public
+00007240: 6974 7920 7075 7270 6f73 6573 206f 6620  ity purposes of 
+00007250: 6e61 6d65 7320 6f66 206c 6963 656e 736f  names of licenso
+00007260: 7273 206f 720d 0a20 2020 2061 7574 686f  rs or..    autho
+00007270: 7273 206f 6620 7468 6520 6d61 7465 7269  rs of the materi
+00007280: 616c 3b20 6f72 0d0a 0d0a 2020 2020 6529  al; or....    e)
+00007290: 2044 6563 6c69 6e69 6e67 2074 6f20 6772   Declining to gr
+000072a0: 616e 7420 7269 6768 7473 2075 6e64 6572  ant rights under
+000072b0: 2074 7261 6465 6d61 726b 206c 6177 2066   trademark law f
+000072c0: 6f72 2075 7365 206f 6620 736f 6d65 0d0a  or use of some..
+000072d0: 2020 2020 7472 6164 6520 6e61 6d65 732c      trade names,
+000072e0: 2074 7261 6465 6d61 726b 732c 206f 7220   trademarks, or 
+000072f0: 7365 7276 6963 6520 6d61 726b 733b 206f  service marks; o
+00007300: 720d 0a0d 0a20 2020 2066 2920 5265 7175  r....    f) Requ
+00007310: 6972 696e 6720 696e 6465 6d6e 6966 6963  iring indemnific
+00007320: 6174 696f 6e20 6f66 206c 6963 656e 736f  ation of licenso
+00007330: 7273 2061 6e64 2061 7574 686f 7273 206f  rs and authors o
+00007340: 6620 7468 6174 0d0a 2020 2020 6d61 7465  f that..    mate
+00007350: 7269 616c 2062 7920 616e 796f 6e65 2077  rial by anyone w
+00007360: 686f 2063 6f6e 7665 7973 2074 6865 206d  ho conveys the m
+00007370: 6174 6572 6961 6c20 286f 7220 6d6f 6469  aterial (or modi
+00007380: 6669 6564 2076 6572 7369 6f6e 7320 6f66  fied versions of
+00007390: 0d0a 2020 2020 6974 2920 7769 7468 2063  ..    it) with c
+000073a0: 6f6e 7472 6163 7475 616c 2061 7373 756d  ontractual assum
+000073b0: 7074 696f 6e73 206f 6620 6c69 6162 696c  ptions of liabil
+000073c0: 6974 7920 746f 2074 6865 2072 6563 6970  ity to the recip
+000073d0: 6965 6e74 2c20 666f 720d 0a20 2020 2061  ient, for..    a
+000073e0: 6e79 206c 6961 6269 6c69 7479 2074 6861  ny liability tha
+000073f0: 7420 7468 6573 6520 636f 6e74 7261 6374  t these contract
+00007400: 7561 6c20 6173 7375 6d70 7469 6f6e 7320  ual assumptions 
+00007410: 6469 7265 6374 6c79 2069 6d70 6f73 6520  directly impose 
+00007420: 6f6e 0d0a 2020 2020 7468 6f73 6520 6c69  on..    those li
+00007430: 6365 6e73 6f72 7320 616e 6420 6175 7468  censors and auth
+00007440: 6f72 732e 0d0a 0d0a 2020 416c 6c20 6f74  ors.....  All ot
+00007450: 6865 7220 6e6f 6e2d 7065 726d 6973 7369  her non-permissi
+00007460: 7665 2061 6464 6974 696f 6e61 6c20 7465  ve additional te
+00007470: 726d 7320 6172 6520 636f 6e73 6964 6572  rms are consider
+00007480: 6564 2022 6675 7274 6865 720d 0a72 6573  ed "further..res
+00007490: 7472 6963 7469 6f6e 7322 2077 6974 6869  trictions" withi
+000074a0: 6e20 7468 6520 6d65 616e 696e 6720 6f66  n the meaning of
+000074b0: 2073 6563 7469 6f6e 2031 302e 2020 4966   section 10.  If
+000074c0: 2074 6865 2050 726f 6772 616d 2061 7320   the Program as 
+000074d0: 796f 750d 0a72 6563 6569 7665 6420 6974  you..received it
+000074e0: 2c20 6f72 2061 6e79 2070 6172 7420 6f66  , or any part of
+000074f0: 2069 742c 2063 6f6e 7461 696e 7320 6120   it, contains a 
+00007500: 6e6f 7469 6365 2073 7461 7469 6e67 2074  notice stating t
+00007510: 6861 7420 6974 2069 730d 0a67 6f76 6572  hat it is..gover
+00007520: 6e65 6420 6279 2074 6869 7320 4c69 6365  ned by this Lice
+00007530: 6e73 6520 616c 6f6e 6720 7769 7468 2061  nse along with a
+00007540: 2074 6572 6d20 7468 6174 2069 7320 6120   term that is a 
+00007550: 6675 7274 6865 720d 0a72 6573 7472 6963  further..restric
+00007560: 7469 6f6e 2c20 796f 7520 6d61 7920 7265  tion, you may re
+00007570: 6d6f 7665 2074 6861 7420 7465 726d 2e20  move that term. 
+00007580: 2049 6620 6120 6c69 6365 6e73 6520 646f   If a license do
+00007590: 6375 6d65 6e74 2063 6f6e 7461 696e 730d  cument contains.
+000075a0: 0a61 2066 7572 7468 6572 2072 6573 7472  .a further restr
+000075b0: 6963 7469 6f6e 2062 7574 2070 6572 6d69  iction but permi
+000075c0: 7473 2072 656c 6963 656e 7369 6e67 206f  ts relicensing o
+000075d0: 7220 636f 6e76 6579 696e 6720 756e 6465  r conveying unde
+000075e0: 7220 7468 6973 0d0a 4c69 6365 6e73 652c  r this..License,
+000075f0: 2079 6f75 206d 6179 2061 6464 2074 6f20   you may add to 
+00007600: 6120 636f 7665 7265 6420 776f 726b 206d  a covered work m
+00007610: 6174 6572 6961 6c20 676f 7665 726e 6564  aterial governed
+00007620: 2062 7920 7468 6520 7465 726d 730d 0a6f   by the terms..o
+00007630: 6620 7468 6174 206c 6963 656e 7365 2064  f that license d
+00007640: 6f63 756d 656e 742c 2070 726f 7669 6465  ocument, provide
+00007650: 6420 7468 6174 2074 6865 2066 7572 7468  d that the furth
+00007660: 6572 2072 6573 7472 6963 7469 6f6e 2064  er restriction d
+00007670: 6f65 730d 0a6e 6f74 2073 7572 7669 7665  oes..not survive
+00007680: 2073 7563 6820 7265 6c69 6365 6e73 696e   such relicensin
+00007690: 6720 6f72 2063 6f6e 7665 7969 6e67 2e0d  g or conveying..
+000076a0: 0a0d 0a20 2049 6620 796f 7520 6164 6420  ...  If you add 
+000076b0: 7465 726d 7320 746f 2061 2063 6f76 6572  terms to a cover
+000076c0: 6564 2077 6f72 6b20 696e 2061 6363 6f72  ed work in accor
+000076d0: 6420 7769 7468 2074 6869 7320 7365 6374  d with this sect
+000076e0: 696f 6e2c 2079 6f75 0d0a 6d75 7374 2070  ion, you..must p
+000076f0: 6c61 6365 2c20 696e 2074 6865 2072 656c  lace, in the rel
+00007700: 6576 616e 7420 736f 7572 6365 2066 696c  evant source fil
+00007710: 6573 2c20 6120 7374 6174 656d 656e 7420  es, a statement 
+00007720: 6f66 2074 6865 0d0a 6164 6469 7469 6f6e  of the..addition
+00007730: 616c 2074 6572 6d73 2074 6861 7420 6170  al terms that ap
+00007740: 706c 7920 746f 2074 686f 7365 2066 696c  ply to those fil
+00007750: 6573 2c20 6f72 2061 206e 6f74 6963 6520  es, or a notice 
+00007760: 696e 6469 6361 7469 6e67 0d0a 7768 6572  indicating..wher
+00007770: 6520 746f 2066 696e 6420 7468 6520 6170  e to find the ap
+00007780: 706c 6963 6162 6c65 2074 6572 6d73 2e0d  plicable terms..
+00007790: 0a0d 0a20 2041 6464 6974 696f 6e61 6c20  ...  Additional 
+000077a0: 7465 726d 732c 2070 6572 6d69 7373 6976  terms, permissiv
+000077b0: 6520 6f72 206e 6f6e 2d70 6572 6d69 7373  e or non-permiss
+000077c0: 6976 652c 206d 6179 2062 6520 7374 6174  ive, may be stat
+000077d0: 6564 2069 6e20 7468 650d 0a66 6f72 6d20  ed in the..form 
+000077e0: 6f66 2061 2073 6570 6172 6174 656c 7920  of a separately 
+000077f0: 7772 6974 7465 6e20 6c69 6365 6e73 652c  written license,
+00007800: 206f 7220 7374 6174 6564 2061 7320 6578   or stated as ex
+00007810: 6365 7074 696f 6e73 3b0d 0a74 6865 2061  ceptions;..the a
+00007820: 626f 7665 2072 6571 7569 7265 6d65 6e74  bove requirement
+00007830: 7320 6170 706c 7920 6569 7468 6572 2077  s apply either w
+00007840: 6179 2e0d 0a0d 0a20 2038 2e20 5465 726d  ay.....  8. Term
+00007850: 696e 6174 696f 6e2e 0d0a 0d0a 2020 596f  ination.....  Yo
+00007860: 7520 6d61 7920 6e6f 7420 7072 6f70 6167  u may not propag
+00007870: 6174 6520 6f72 206d 6f64 6966 7920 6120  ate or modify a 
+00007880: 636f 7665 7265 6420 776f 726b 2065 7863  covered work exc
+00007890: 6570 7420 6173 2065 7870 7265 7373 6c79  ept as expressly
+000078a0: 0d0a 7072 6f76 6964 6564 2075 6e64 6572  ..provided under
+000078b0: 2074 6869 7320 4c69 6365 6e73 652e 2020   this License.  
+000078c0: 416e 7920 6174 7465 6d70 7420 6f74 6865  Any attempt othe
+000078d0: 7277 6973 6520 746f 2070 726f 7061 6761  rwise to propaga
+000078e0: 7465 206f 720d 0a6d 6f64 6966 7920 6974  te or..modify it
+000078f0: 2069 7320 766f 6964 2c20 616e 6420 7769   is void, and wi
+00007900: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00007910: 2074 6572 6d69 6e61 7465 2079 6f75 7220   terminate your 
+00007920: 7269 6768 7473 2075 6e64 6572 0d0a 7468  rights under..th
+00007930: 6973 204c 6963 656e 7365 2028 696e 636c  is License (incl
+00007940: 7564 696e 6720 616e 7920 7061 7465 6e74  uding any patent
+00007950: 206c 6963 656e 7365 7320 6772 616e 7465   licenses grante
+00007960: 6420 756e 6465 7220 7468 6520 7468 6972  d under the thir
+00007970: 640d 0a70 6172 6167 7261 7068 206f 6620  d..paragraph of 
+00007980: 7365 6374 696f 6e20 3131 292e 0d0a 0d0a  section 11).....
+00007990: 2020 486f 7765 7665 722c 2069 6620 796f    However, if yo
+000079a0: 7520 6365 6173 6520 616c 6c20 7669 6f6c  u cease all viol
+000079b0: 6174 696f 6e20 6f66 2074 6869 7320 4c69  ation of this Li
+000079c0: 6365 6e73 652c 2074 6865 6e20 796f 7572  cense, then your
+000079d0: 0d0a 6c69 6365 6e73 6520 6672 6f6d 2061  ..license from a
+000079e0: 2070 6172 7469 6375 6c61 7220 636f 7079   particular copy
+000079f0: 7269 6768 7420 686f 6c64 6572 2069 7320  right holder is 
+00007a00: 7265 696e 7374 6174 6564 2028 6129 0d0a  reinstated (a)..
+00007a10: 7072 6f76 6973 696f 6e61 6c6c 792c 2075  provisionally, u
+00007a20: 6e6c 6573 7320 616e 6420 756e 7469 6c20  nless and until 
+00007a30: 7468 6520 636f 7079 7269 6768 7420 686f  the copyright ho
+00007a40: 6c64 6572 2065 7870 6c69 6369 746c 7920  lder explicitly 
+00007a50: 616e 640d 0a66 696e 616c 6c79 2074 6572  and..finally ter
+00007a60: 6d69 6e61 7465 7320 796f 7572 206c 6963  minates your lic
+00007a70: 656e 7365 2c20 616e 6420 2862 2920 7065  ense, and (b) pe
+00007a80: 726d 616e 656e 746c 792c 2069 6620 7468  rmanently, if th
+00007a90: 6520 636f 7079 7269 6768 740d 0a68 6f6c  e copyright..hol
+00007aa0: 6465 7220 6661 696c 7320 746f 206e 6f74  der fails to not
+00007ab0: 6966 7920 796f 7520 6f66 2074 6865 2076  ify you of the v
+00007ac0: 696f 6c61 7469 6f6e 2062 7920 736f 6d65  iolation by some
+00007ad0: 2072 6561 736f 6e61 626c 6520 6d65 616e   reasonable mean
+00007ae0: 730d 0a70 7269 6f72 2074 6f20 3630 2064  s..prior to 60 d
+00007af0: 6179 7320 6166 7465 7220 7468 6520 6365  ays after the ce
+00007b00: 7373 6174 696f 6e2e 0d0a 0d0a 2020 4d6f  ssation.....  Mo
+00007b10: 7265 6f76 6572 2c20 796f 7572 206c 6963  reover, your lic
+00007b20: 656e 7365 2066 726f 6d20 6120 7061 7274  ense from a part
+00007b30: 6963 756c 6172 2063 6f70 7972 6967 6874  icular copyright
+00007b40: 2068 6f6c 6465 7220 6973 0d0a 7265 696e   holder is..rein
+00007b50: 7374 6174 6564 2070 6572 6d61 6e65 6e74  stated permanent
+00007b60: 6c79 2069 6620 7468 6520 636f 7079 7269  ly if the copyri
+00007b70: 6768 7420 686f 6c64 6572 206e 6f74 6966  ght holder notif
+00007b80: 6965 7320 796f 7520 6f66 2074 6865 0d0a  ies you of the..
+00007b90: 7669 6f6c 6174 696f 6e20 6279 2073 6f6d  violation by som
+00007ba0: 6520 7265 6173 6f6e 6162 6c65 206d 6561  e reasonable mea
+00007bb0: 6e73 2c20 7468 6973 2069 7320 7468 6520  ns, this is the 
+00007bc0: 6669 7273 7420 7469 6d65 2079 6f75 2068  first time you h
+00007bd0: 6176 650d 0a72 6563 6569 7665 6420 6e6f  ave..received no
+00007be0: 7469 6365 206f 6620 7669 6f6c 6174 696f  tice of violatio
+00007bf0: 6e20 6f66 2074 6869 7320 4c69 6365 6e73  n of this Licens
+00007c00: 6520 2866 6f72 2061 6e79 2077 6f72 6b29  e (for any work)
+00007c10: 2066 726f 6d20 7468 6174 0d0a 636f 7079   from that..copy
+00007c20: 7269 6768 7420 686f 6c64 6572 2c20 616e  right holder, an
+00007c30: 6420 796f 7520 6375 7265 2074 6865 2076  d you cure the v
+00007c40: 696f 6c61 7469 6f6e 2070 7269 6f72 2074  iolation prior t
+00007c50: 6f20 3330 2064 6179 7320 6166 7465 720d  o 30 days after.
+00007c60: 0a79 6f75 7220 7265 6365 6970 7420 6f66  .your receipt of
+00007c70: 2074 6865 206e 6f74 6963 652e 0d0a 0d0a   the notice.....
+00007c80: 2020 5465 726d 696e 6174 696f 6e20 6f66    Termination of
+00007c90: 2079 6f75 7220 7269 6768 7473 2075 6e64   your rights und
+00007ca0: 6572 2074 6869 7320 7365 6374 696f 6e20  er this section 
+00007cb0: 646f 6573 206e 6f74 2074 6572 6d69 6e61  does not termina
+00007cc0: 7465 2074 6865 0d0a 6c69 6365 6e73 6573  te the..licenses
+00007cd0: 206f 6620 7061 7274 6965 7320 7768 6f20   of parties who 
+00007ce0: 6861 7665 2072 6563 6569 7665 6420 636f  have received co
+00007cf0: 7069 6573 206f 7220 7269 6768 7473 2066  pies or rights f
+00007d00: 726f 6d20 796f 7520 756e 6465 720d 0a74  rom you under..t
+00007d10: 6869 7320 4c69 6365 6e73 652e 2020 4966  his License.  If
+00007d20: 2079 6f75 7220 7269 6768 7473 2068 6176   your rights hav
+00007d30: 6520 6265 656e 2074 6572 6d69 6e61 7465  e been terminate
+00007d40: 6420 616e 6420 6e6f 7420 7065 726d 616e  d and not perman
+00007d50: 656e 746c 790d 0a72 6569 6e73 7461 7465  ently..reinstate
+00007d60: 642c 2079 6f75 2064 6f20 6e6f 7420 7175  d, you do not qu
+00007d70: 616c 6966 7920 746f 2072 6563 6569 7665  alify to receive
+00007d80: 206e 6577 206c 6963 656e 7365 7320 666f   new licenses fo
+00007d90: 7220 7468 6520 7361 6d65 0d0a 6d61 7465  r the same..mate
+00007da0: 7269 616c 2075 6e64 6572 2073 6563 7469  rial under secti
+00007db0: 6f6e 2031 302e 0d0a 0d0a 2020 392e 2041  on 10.....  9. A
+00007dc0: 6363 6570 7461 6e63 6520 4e6f 7420 5265  cceptance Not Re
+00007dd0: 7175 6972 6564 2066 6f72 2048 6176 696e  quired for Havin
+00007de0: 6720 436f 7069 6573 2e0d 0a0d 0a20 2059  g Copies.....  Y
+00007df0: 6f75 2061 7265 206e 6f74 2072 6571 7569  ou are not requi
+00007e00: 7265 6420 746f 2061 6363 6570 7420 7468  red to accept th
+00007e10: 6973 204c 6963 656e 7365 2069 6e20 6f72  is License in or
+00007e20: 6465 7220 746f 2072 6563 6569 7665 206f  der to receive o
+00007e30: 720d 0a72 756e 2061 2063 6f70 7920 6f66  r..run a copy of
+00007e40: 2074 6865 2050 726f 6772 616d 2e20 2041   the Program.  A
+00007e50: 6e63 696c 6c61 7279 2070 726f 7061 6761  ncillary propaga
+00007e60: 7469 6f6e 206f 6620 6120 636f 7665 7265  tion of a covere
+00007e70: 6420 776f 726b 0d0a 6f63 6375 7272 696e  d work..occurrin
+00007e80: 6720 736f 6c65 6c79 2061 7320 6120 636f  g solely as a co
+00007e90: 6e73 6571 7565 6e63 6520 6f66 2075 7369  nsequence of usi
+00007ea0: 6e67 2070 6565 722d 746f 2d70 6565 7220  ng peer-to-peer 
+00007eb0: 7472 616e 736d 6973 7369 6f6e 0d0a 746f  transmission..to
+00007ec0: 2072 6563 6569 7665 2061 2063 6f70 7920   receive a copy 
+00007ed0: 6c69 6b65 7769 7365 2064 6f65 7320 6e6f  likewise does no
+00007ee0: 7420 7265 7175 6972 6520 6163 6365 7074  t require accept
+00007ef0: 616e 6365 2e20 2048 6f77 6576 6572 2c0d  ance.  However,.
+00007f00: 0a6e 6f74 6869 6e67 206f 7468 6572 2074  .nothing other t
+00007f10: 6861 6e20 7468 6973 204c 6963 656e 7365  han this License
+00007f20: 2067 7261 6e74 7320 796f 7520 7065 726d   grants you perm
+00007f30: 6973 7369 6f6e 2074 6f20 7072 6f70 6167  ission to propag
+00007f40: 6174 6520 6f72 0d0a 6d6f 6469 6679 2061  ate or..modify a
+00007f50: 6e79 2063 6f76 6572 6564 2077 6f72 6b2e  ny covered work.
+00007f60: 2020 5468 6573 6520 6163 7469 6f6e 7320    These actions 
+00007f70: 696e 6672 696e 6765 2063 6f70 7972 6967  infringe copyrig
+00007f80: 6874 2069 6620 796f 7520 646f 0d0a 6e6f  ht if you do..no
+00007f90: 7420 6163 6365 7074 2074 6869 7320 4c69  t accept this Li
+00007fa0: 6365 6e73 652e 2020 5468 6572 6566 6f72  cense.  Therefor
+00007fb0: 652c 2062 7920 6d6f 6469 6679 696e 6720  e, by modifying 
+00007fc0: 6f72 2070 726f 7061 6761 7469 6e67 2061  or propagating a
+00007fd0: 0d0a 636f 7665 7265 6420 776f 726b 2c20  ..covered work, 
+00007fe0: 796f 7520 696e 6469 6361 7465 2079 6f75  you indicate you
+00007ff0: 7220 6163 6365 7074 616e 6365 206f 6620  r acceptance of 
+00008000: 7468 6973 204c 6963 656e 7365 2074 6f20  this License to 
+00008010: 646f 2073 6f2e 0d0a 0d0a 2020 3130 2e20  do so.....  10. 
+00008020: 4175 746f 6d61 7469 6320 4c69 6365 6e73  Automatic Licens
+00008030: 696e 6720 6f66 2044 6f77 6e73 7472 6561  ing of Downstrea
+00008040: 6d20 5265 6369 7069 656e 7473 2e0d 0a0d  m Recipients....
+00008050: 0a20 2045 6163 6820 7469 6d65 2079 6f75  .  Each time you
+00008060: 2063 6f6e 7665 7920 6120 636f 7665 7265   convey a covere
+00008070: 6420 776f 726b 2c20 7468 6520 7265 6369  d work, the reci
+00008080: 7069 656e 7420 6175 746f 6d61 7469 6361  pient automatica
+00008090: 6c6c 790d 0a72 6563 6569 7665 7320 6120  lly..receives a 
+000080a0: 6c69 6365 6e73 6520 6672 6f6d 2074 6865  license from the
+000080b0: 206f 7269 6769 6e61 6c20 6c69 6365 6e73   original licens
+000080c0: 6f72 732c 2074 6f20 7275 6e2c 206d 6f64  ors, to run, mod
+000080d0: 6966 7920 616e 640d 0a70 726f 7061 6761  ify and..propaga
+000080e0: 7465 2074 6861 7420 776f 726b 2c20 7375  te that work, su
+000080f0: 626a 6563 7420 746f 2074 6869 7320 4c69  bject to this Li
+00008100: 6365 6e73 652e 2020 596f 7520 6172 6520  cense.  You are 
+00008110: 6e6f 7420 7265 7370 6f6e 7369 626c 650d  not responsible.
+00008120: 0a66 6f72 2065 6e66 6f72 6369 6e67 2063  .for enforcing c
+00008130: 6f6d 706c 6961 6e63 6520 6279 2074 6869  ompliance by thi
+00008140: 7264 2070 6172 7469 6573 2077 6974 6820  rd parties with 
+00008150: 7468 6973 204c 6963 656e 7365 2e0d 0a0d  this License....
+00008160: 0a20 2041 6e20 2265 6e74 6974 7920 7472  .  An "entity tr
+00008170: 616e 7361 6374 696f 6e22 2069 7320 6120  ansaction" is a 
+00008180: 7472 616e 7361 6374 696f 6e20 7472 616e  transaction tran
+00008190: 7366 6572 7269 6e67 2063 6f6e 7472 6f6c  sferring control
+000081a0: 206f 6620 616e 0d0a 6f72 6761 6e69 7a61   of an..organiza
+000081b0: 7469 6f6e 2c20 6f72 2073 7562 7374 616e  tion, or substan
+000081c0: 7469 616c 6c79 2061 6c6c 2061 7373 6574  tially all asset
+000081d0: 7320 6f66 206f 6e65 2c20 6f72 2073 7562  s of one, or sub
+000081e0: 6469 7669 6469 6e67 2061 6e0d 0a6f 7267  dividing an..org
+000081f0: 616e 697a 6174 696f 6e2c 206f 7220 6d65  anization, or me
+00008200: 7267 696e 6720 6f72 6761 6e69 7a61 7469  rging organizati
+00008210: 6f6e 732e 2020 4966 2070 726f 7061 6761  ons.  If propaga
+00008220: 7469 6f6e 206f 6620 6120 636f 7665 7265  tion of a covere
+00008230: 640d 0a77 6f72 6b20 7265 7375 6c74 7320  d..work results 
+00008240: 6672 6f6d 2061 6e20 656e 7469 7479 2074  from an entity t
+00008250: 7261 6e73 6163 7469 6f6e 2c20 6561 6368  ransaction, each
+00008260: 2070 6172 7479 2074 6f20 7468 6174 0d0a   party to that..
+00008270: 7472 616e 7361 6374 696f 6e20 7768 6f20  transaction who 
+00008280: 7265 6365 6976 6573 2061 2063 6f70 7920  receives a copy 
+00008290: 6f66 2074 6865 2077 6f72 6b20 616c 736f  of the work also
+000082a0: 2072 6563 6569 7665 7320 7768 6174 6576   receives whatev
+000082b0: 6572 0d0a 6c69 6365 6e73 6573 2074 6f20  er..licenses to 
+000082c0: 7468 6520 776f 726b 2074 6865 2070 6172  the work the par
+000082d0: 7479 2773 2070 7265 6465 6365 7373 6f72  ty's predecessor
+000082e0: 2069 6e20 696e 7465 7265 7374 2068 6164   in interest had
+000082f0: 206f 7220 636f 756c 640d 0a67 6976 6520   or could..give 
+00008300: 756e 6465 7220 7468 6520 7072 6576 696f  under the previo
+00008310: 7573 2070 6172 6167 7261 7068 2c20 706c  us paragraph, pl
+00008320: 7573 2061 2072 6967 6874 2074 6f20 706f  us a right to po
+00008330: 7373 6573 7369 6f6e 206f 6620 7468 650d  ssession of the.
+00008340: 0a43 6f72 7265 7370 6f6e 6469 6e67 2053  .Corresponding S
+00008350: 6f75 7263 6520 6f66 2074 6865 2077 6f72  ource of the wor
+00008360: 6b20 6672 6f6d 2074 6865 2070 7265 6465  k from the prede
+00008370: 6365 7373 6f72 2069 6e20 696e 7465 7265  cessor in intere
+00008380: 7374 2c20 6966 0d0a 7468 6520 7072 6564  st, if..the pred
+00008390: 6563 6573 736f 7220 6861 7320 6974 206f  ecessor has it o
+000083a0: 7220 6361 6e20 6765 7420 6974 2077 6974  r can get it wit
+000083b0: 6820 7265 6173 6f6e 6162 6c65 2065 6666  h reasonable eff
+000083c0: 6f72 7473 2e0d 0a0d 0a20 2059 6f75 206d  orts.....  You m
+000083d0: 6179 206e 6f74 2069 6d70 6f73 6520 616e  ay not impose an
+000083e0: 7920 6675 7274 6865 7220 7265 7374 7269  y further restri
+000083f0: 6374 696f 6e73 206f 6e20 7468 6520 6578  ctions on the ex
+00008400: 6572 6369 7365 206f 6620 7468 650d 0a72  ercise of the..r
+00008410: 6967 6874 7320 6772 616e 7465 6420 6f72  ights granted or
+00008420: 2061 6666 6972 6d65 6420 756e 6465 7220   affirmed under 
+00008430: 7468 6973 204c 6963 656e 7365 2e20 2046  this License.  F
+00008440: 6f72 2065 7861 6d70 6c65 2c20 796f 7520  or example, you 
+00008450: 6d61 790d 0a6e 6f74 2069 6d70 6f73 6520  may..not impose 
+00008460: 6120 6c69 6365 6e73 6520 6665 652c 2072  a license fee, r
+00008470: 6f79 616c 7479 2c20 6f72 206f 7468 6572  oyalty, or other
+00008480: 2063 6861 7267 6520 666f 7220 6578 6572   charge for exer
+00008490: 6369 7365 206f 660d 0a72 6967 6874 7320  cise of..rights 
+000084a0: 6772 616e 7465 6420 756e 6465 7220 7468  granted under th
+000084b0: 6973 204c 6963 656e 7365 2c20 616e 6420  is License, and 
+000084c0: 796f 7520 6d61 7920 6e6f 7420 696e 6974  you may not init
+000084d0: 6961 7465 206c 6974 6967 6174 696f 6e0d  iate litigation.
+000084e0: 0a28 696e 636c 7564 696e 6720 6120 6372  .(including a cr
+000084f0: 6f73 732d 636c 6169 6d20 6f72 2063 6f75  oss-claim or cou
+00008500: 6e74 6572 636c 6169 6d20 696e 2061 206c  nterclaim in a l
+00008510: 6177 7375 6974 2920 616c 6c65 6769 6e67  awsuit) alleging
+00008520: 2074 6861 740d 0a61 6e79 2070 6174 656e   that..any paten
+00008530: 7420 636c 6169 6d20 6973 2069 6e66 7269  t claim is infri
+00008540: 6e67 6564 2062 7920 6d61 6b69 6e67 2c20  nged by making, 
+00008550: 7573 696e 672c 2073 656c 6c69 6e67 2c20  using, selling, 
+00008560: 6f66 6665 7269 6e67 2066 6f72 0d0a 7361  offering for..sa
+00008570: 6c65 2c20 6f72 2069 6d70 6f72 7469 6e67  le, or importing
+00008580: 2074 6865 2050 726f 6772 616d 206f 7220   the Program or 
+00008590: 616e 7920 706f 7274 696f 6e20 6f66 2069  any portion of i
+000085a0: 742e 0d0a 0d0a 2020 3131 2e20 5061 7465  t.....  11. Pate
+000085b0: 6e74 732e 0d0a 0d0a 2020 4120 2263 6f6e  nts.....  A "con
+000085c0: 7472 6962 7574 6f72 2220 6973 2061 2063  tributor" is a c
+000085d0: 6f70 7972 6967 6874 2068 6f6c 6465 7220  opyright holder 
+000085e0: 7768 6f20 6175 7468 6f72 697a 6573 2075  who authorizes u
+000085f0: 7365 2075 6e64 6572 2074 6869 730d 0a4c  se under this..L
+00008600: 6963 656e 7365 206f 6620 7468 6520 5072  icense of the Pr
+00008610: 6f67 7261 6d20 6f72 2061 2077 6f72 6b20  ogram or a work 
+00008620: 6f6e 2077 6869 6368 2074 6865 2050 726f  on which the Pro
+00008630: 6772 616d 2069 7320 6261 7365 642e 2020  gram is based.  
+00008640: 5468 650d 0a77 6f72 6b20 7468 7573 206c  The..work thus l
+00008650: 6963 656e 7365 6420 6973 2063 616c 6c65  icensed is calle
+00008660: 6420 7468 6520 636f 6e74 7269 6275 746f  d the contributo
+00008670: 7227 7320 2263 6f6e 7472 6962 7574 6f72  r's "contributor
+00008680: 2076 6572 7369 6f6e 222e 0d0a 0d0a 2020   version".....  
+00008690: 4120 636f 6e74 7269 6275 746f 7227 7320  A contributor's 
+000086a0: 2265 7373 656e 7469 616c 2070 6174 656e  "essential paten
+000086b0: 7420 636c 6169 6d73 2220 6172 6520 616c  t claims" are al
+000086c0: 6c20 7061 7465 6e74 2063 6c61 696d 730d  l patent claims.
+000086d0: 0a6f 776e 6564 206f 7220 636f 6e74 726f  .owned or contro
+000086e0: 6c6c 6564 2062 7920 7468 6520 636f 6e74  lled by the cont
+000086f0: 7269 6275 746f 722c 2077 6865 7468 6572  ributor, whether
+00008700: 2061 6c72 6561 6479 2061 6371 7569 7265   already acquire
+00008710: 6420 6f72 0d0a 6865 7265 6166 7465 7220  d or..hereafter 
+00008720: 6163 7175 6972 6564 2c20 7468 6174 2077  acquired, that w
+00008730: 6f75 6c64 2062 6520 696e 6672 696e 6765  ould be infringe
+00008740: 6420 6279 2073 6f6d 6520 6d61 6e6e 6572  d by some manner
+00008750: 2c20 7065 726d 6974 7465 640d 0a62 7920  , permitted..by 
+00008760: 7468 6973 204c 6963 656e 7365 2c20 6f66  this License, of
+00008770: 206d 616b 696e 672c 2075 7369 6e67 2c20   making, using, 
+00008780: 6f72 2073 656c 6c69 6e67 2069 7473 2063  or selling its c
+00008790: 6f6e 7472 6962 7574 6f72 2076 6572 7369  ontributor versi
+000087a0: 6f6e 2c0d 0a62 7574 2064 6f20 6e6f 7420  on,..but do not 
+000087b0: 696e 636c 7564 6520 636c 6169 6d73 2074  include claims t
+000087c0: 6861 7420 776f 756c 6420 6265 2069 6e66  hat would be inf
+000087d0: 7269 6e67 6564 206f 6e6c 7920 6173 2061  ringed only as a
+000087e0: 0d0a 636f 6e73 6571 7565 6e63 6520 6f66  ..consequence of
+000087f0: 2066 7572 7468 6572 206d 6f64 6966 6963   further modific
+00008800: 6174 696f 6e20 6f66 2074 6865 2063 6f6e  ation of the con
+00008810: 7472 6962 7574 6f72 2076 6572 7369 6f6e  tributor version
+00008820: 2e20 2046 6f72 0d0a 7075 7270 6f73 6573  .  For..purposes
+00008830: 206f 6620 7468 6973 2064 6566 696e 6974   of this definit
+00008840: 696f 6e2c 2022 636f 6e74 726f 6c22 2069  ion, "control" i
+00008850: 6e63 6c75 6465 7320 7468 6520 7269 6768  ncludes the righ
+00008860: 7420 746f 2067 7261 6e74 0d0a 7061 7465  t to grant..pate
+00008870: 6e74 2073 7562 6c69 6365 6e73 6573 2069  nt sublicenses i
+00008880: 6e20 6120 6d61 6e6e 6572 2063 6f6e 7369  n a manner consi
+00008890: 7374 656e 7420 7769 7468 2074 6865 2072  stent with the r
+000088a0: 6571 7569 7265 6d65 6e74 7320 6f66 0d0a  equirements of..
+000088b0: 7468 6973 204c 6963 656e 7365 2e0d 0a0d  this License....
+000088c0: 0a20 2045 6163 6820 636f 6e74 7269 6275  .  Each contribu
+000088d0: 746f 7220 6772 616e 7473 2079 6f75 2061  tor grants you a
+000088e0: 206e 6f6e 2d65 7863 6c75 7369 7665 2c20   non-exclusive, 
+000088f0: 776f 726c 6477 6964 652c 2072 6f79 616c  worldwide, royal
+00008900: 7479 2d66 7265 650d 0a70 6174 656e 7420  ty-free..patent 
+00008910: 6c69 6365 6e73 6520 756e 6465 7220 7468  license under th
+00008920: 6520 636f 6e74 7269 6275 746f 7227 7320  e contributor's 
+00008930: 6573 7365 6e74 6961 6c20 7061 7465 6e74  essential patent
+00008940: 2063 6c61 696d 732c 2074 6f0d 0a6d 616b   claims, to..mak
+00008950: 652c 2075 7365 2c20 7365 6c6c 2c20 6f66  e, use, sell, of
+00008960: 6665 7220 666f 7220 7361 6c65 2c20 696d  fer for sale, im
+00008970: 706f 7274 2061 6e64 206f 7468 6572 7769  port and otherwi
+00008980: 7365 2072 756e 2c20 6d6f 6469 6679 2061  se run, modify a
+00008990: 6e64 0d0a 7072 6f70 6167 6174 6520 7468  nd..propagate th
+000089a0: 6520 636f 6e74 656e 7473 206f 6620 6974  e contents of it
+000089b0: 7320 636f 6e74 7269 6275 746f 7220 7665  s contributor ve
+000089c0: 7273 696f 6e2e 0d0a 0d0a 2020 496e 2074  rsion.....  In t
+000089d0: 6865 2066 6f6c 6c6f 7769 6e67 2074 6872  he following thr
+000089e0: 6565 2070 6172 6167 7261 7068 732c 2061  ee paragraphs, a
+000089f0: 2022 7061 7465 6e74 206c 6963 656e 7365   "patent license
+00008a00: 2220 6973 2061 6e79 2065 7870 7265 7373  " is any express
+00008a10: 0d0a 6167 7265 656d 656e 7420 6f72 2063  ..agreement or c
+00008a20: 6f6d 6d69 746d 656e 742c 2068 6f77 6576  ommitment, howev
+00008a30: 6572 2064 656e 6f6d 696e 6174 6564 2c20  er denominated, 
+00008a40: 6e6f 7420 746f 2065 6e66 6f72 6365 2061  not to enforce a
+00008a50: 2070 6174 656e 740d 0a28 7375 6368 2061   patent..(such a
+00008a60: 7320 616e 2065 7870 7265 7373 2070 6572  s an express per
+00008a70: 6d69 7373 696f 6e20 746f 2070 7261 6374  mission to pract
+00008a80: 6963 6520 6120 7061 7465 6e74 206f 7220  ice a patent or 
+00008a90: 636f 7665 6e61 6e74 206e 6f74 2074 6f0d  covenant not to.
+00008aa0: 0a73 7565 2066 6f72 2070 6174 656e 7420  .sue for patent 
+00008ab0: 696e 6672 696e 6765 6d65 6e74 292e 2020  infringement).  
+00008ac0: 546f 2022 6772 616e 7422 2073 7563 6820  To "grant" such 
+00008ad0: 6120 7061 7465 6e74 206c 6963 656e 7365  a patent license
+00008ae0: 2074 6f20 610d 0a70 6172 7479 206d 6561   to a..party mea
+00008af0: 6e73 2074 6f20 6d61 6b65 2073 7563 6820  ns to make such 
+00008b00: 616e 2061 6772 6565 6d65 6e74 206f 7220  an agreement or 
+00008b10: 636f 6d6d 6974 6d65 6e74 206e 6f74 2074  commitment not t
+00008b20: 6f20 656e 666f 7263 6520 610d 0a70 6174  o enforce a..pat
+00008b30: 656e 7420 6167 6169 6e73 7420 7468 6520  ent against the 
+00008b40: 7061 7274 792e 0d0a 0d0a 2020 4966 2079  party.....  If y
+00008b50: 6f75 2063 6f6e 7665 7920 6120 636f 7665  ou convey a cove
+00008b60: 7265 6420 776f 726b 2c20 6b6e 6f77 696e  red work, knowin
+00008b70: 676c 7920 7265 6c79 696e 6720 6f6e 2061  gly relying on a
+00008b80: 2070 6174 656e 7420 6c69 6365 6e73 652c   patent license,
+00008b90: 0d0a 616e 6420 7468 6520 436f 7272 6573  ..and the Corres
+00008ba0: 706f 6e64 696e 6720 536f 7572 6365 206f  ponding Source o
+00008bb0: 6620 7468 6520 776f 726b 2069 7320 6e6f  f the work is no
+00008bc0: 7420 6176 6169 6c61 626c 6520 666f 7220  t available for 
+00008bd0: 616e 796f 6e65 0d0a 746f 2063 6f70 792c  anyone..to copy,
+00008be0: 2066 7265 6520 6f66 2063 6861 7267 6520   free of charge 
+00008bf0: 616e 6420 756e 6465 7220 7468 6520 7465  and under the te
+00008c00: 726d 7320 6f66 2074 6869 7320 4c69 6365  rms of this Lice
+00008c10: 6e73 652c 2074 6872 6f75 6768 2061 0d0a  nse, through a..
+00008c20: 7075 626c 6963 6c79 2061 7661 696c 6162  publicly availab
+00008c30: 6c65 206e 6574 776f 726b 2073 6572 7665  le network serve
+00008c40: 7220 6f72 206f 7468 6572 2072 6561 6469  r or other readi
+00008c50: 6c79 2061 6363 6573 7369 626c 6520 6d65  ly accessible me
+00008c60: 616e 732c 0d0a 7468 656e 2079 6f75 206d  ans,..then you m
+00008c70: 7573 7420 6569 7468 6572 2028 3129 2063  ust either (1) c
+00008c80: 6175 7365 2074 6865 2043 6f72 7265 7370  ause the Corresp
+00008c90: 6f6e 6469 6e67 2053 6f75 7263 6520 746f  onding Source to
+00008ca0: 2062 6520 736f 0d0a 6176 6169 6c61 626c   be so..availabl
+00008cb0: 652c 206f 7220 2832 2920 6172 7261 6e67  e, or (2) arrang
+00008cc0: 6520 746f 2064 6570 7269 7665 2079 6f75  e to deprive you
+00008cd0: 7273 656c 6620 6f66 2074 6865 2062 656e  rself of the ben
+00008ce0: 6566 6974 206f 6620 7468 650d 0a70 6174  efit of the..pat
+00008cf0: 656e 7420 6c69 6365 6e73 6520 666f 7220  ent license for 
+00008d00: 7468 6973 2070 6172 7469 6375 6c61 7220  this particular 
+00008d10: 776f 726b 2c20 6f72 2028 3329 2061 7272  work, or (3) arr
+00008d20: 616e 6765 2c20 696e 2061 206d 616e 6e65  ange, in a manne
+00008d30: 720d 0a63 6f6e 7369 7374 656e 7420 7769  r..consistent wi
+00008d40: 7468 2074 6865 2072 6571 7569 7265 6d65  th the requireme
+00008d50: 6e74 7320 6f66 2074 6869 7320 4c69 6365  nts of this Lice
+00008d60: 6e73 652c 2074 6f20 6578 7465 6e64 2074  nse, to extend t
+00008d70: 6865 2070 6174 656e 740d 0a6c 6963 656e  he patent..licen
+00008d80: 7365 2074 6f20 646f 776e 7374 7265 616d  se to downstream
+00008d90: 2072 6563 6970 6965 6e74 732e 2020 224b   recipients.  "K
+00008da0: 6e6f 7769 6e67 6c79 2072 656c 7969 6e67  nowingly relying
+00008db0: 2220 6d65 616e 7320 796f 7520 6861 7665  " means you have
+00008dc0: 0d0a 6163 7475 616c 206b 6e6f 776c 6564  ..actual knowled
+00008dd0: 6765 2074 6861 742c 2062 7574 2066 6f72  ge that, but for
+00008de0: 2074 6865 2070 6174 656e 7420 6c69 6365   the patent lice
+00008df0: 6e73 652c 2079 6f75 7220 636f 6e76 6579  nse, your convey
+00008e00: 696e 6720 7468 650d 0a63 6f76 6572 6564  ing the..covered
+00008e10: 2077 6f72 6b20 696e 2061 2063 6f75 6e74   work in a count
+00008e20: 7279 2c20 6f72 2079 6f75 7220 7265 6369  ry, or your reci
+00008e30: 7069 656e 7427 7320 7573 6520 6f66 2074  pient's use of t
+00008e40: 6865 2063 6f76 6572 6564 2077 6f72 6b0d  he covered work.
+00008e50: 0a69 6e20 6120 636f 756e 7472 792c 2077  .in a country, w
+00008e60: 6f75 6c64 2069 6e66 7269 6e67 6520 6f6e  ould infringe on
+00008e70: 6520 6f72 206d 6f72 6520 6964 656e 7469  e or more identi
+00008e80: 6669 6162 6c65 2070 6174 656e 7473 2069  fiable patents i
+00008e90: 6e20 7468 6174 0d0a 636f 756e 7472 7920  n that..country 
+00008ea0: 7468 6174 2079 6f75 2068 6176 6520 7265  that you have re
+00008eb0: 6173 6f6e 2074 6f20 6265 6c69 6576 6520  ason to believe 
+00008ec0: 6172 6520 7661 6c69 642e 0d0a 0d0a 2020  are valid.....  
+00008ed0: 4966 2c20 7075 7273 7561 6e74 2074 6f20  If, pursuant to 
+00008ee0: 6f72 2069 6e20 636f 6e6e 6563 7469 6f6e  or in connection
+00008ef0: 2077 6974 6820 6120 7369 6e67 6c65 2074   with a single t
+00008f00: 7261 6e73 6163 7469 6f6e 206f 720d 0a61  ransaction or..a
+00008f10: 7272 616e 6765 6d65 6e74 2c20 796f 7520  rrangement, you 
+00008f20: 636f 6e76 6579 2c20 6f72 2070 726f 7061  convey, or propa
+00008f30: 6761 7465 2062 7920 7072 6f63 7572 696e  gate by procurin
+00008f40: 6720 636f 6e76 6579 616e 6365 206f 662c  g conveyance of,
+00008f50: 2061 0d0a 636f 7665 7265 6420 776f 726b   a..covered work
+00008f60: 2c20 616e 6420 6772 616e 7420 6120 7061  , and grant a pa
+00008f70: 7465 6e74 206c 6963 656e 7365 2074 6f20  tent license to 
+00008f80: 736f 6d65 206f 6620 7468 6520 7061 7274  some of the part
+00008f90: 6965 730d 0a72 6563 6569 7669 6e67 2074  ies..receiving t
+00008fa0: 6865 2063 6f76 6572 6564 2077 6f72 6b20  he covered work 
+00008fb0: 6175 7468 6f72 697a 696e 6720 7468 656d  authorizing them
+00008fc0: 2074 6f20 7573 652c 2070 726f 7061 6761   to use, propaga
+00008fd0: 7465 2c20 6d6f 6469 6679 0d0a 6f72 2063  te, modify..or c
+00008fe0: 6f6e 7665 7920 6120 7370 6563 6966 6963  onvey a specific
+00008ff0: 2063 6f70 7920 6f66 2074 6865 2063 6f76   copy of the cov
+00009000: 6572 6564 2077 6f72 6b2c 2074 6865 6e20  ered work, then 
+00009010: 7468 6520 7061 7465 6e74 206c 6963 656e  the patent licen
+00009020: 7365 0d0a 796f 7520 6772 616e 7420 6973  se..you grant is
+00009030: 2061 7574 6f6d 6174 6963 616c 6c79 2065   automatically e
+00009040: 7874 656e 6465 6420 746f 2061 6c6c 2072  xtended to all r
+00009050: 6563 6970 6965 6e74 7320 6f66 2074 6865  ecipients of the
+00009060: 2063 6f76 6572 6564 0d0a 776f 726b 2061   covered..work a
+00009070: 6e64 2077 6f72 6b73 2062 6173 6564 206f  nd works based o
+00009080: 6e20 6974 2e0d 0a0d 0a20 2041 2070 6174  n it.....  A pat
+00009090: 656e 7420 6c69 6365 6e73 6520 6973 2022  ent license is "
+000090a0: 6469 7363 7269 6d69 6e61 746f 7279 2220  discriminatory" 
+000090b0: 6966 2069 7420 646f 6573 206e 6f74 2069  if it does not i
+000090c0: 6e63 6c75 6465 2077 6974 6869 6e0d 0a74  nclude within..t
+000090d0: 6865 2073 636f 7065 206f 6620 6974 7320  he scope of its 
+000090e0: 636f 7665 7261 6765 2c20 7072 6f68 6962  coverage, prohib
+000090f0: 6974 7320 7468 6520 6578 6572 6369 7365  its the exercise
+00009100: 206f 662c 206f 7220 6973 0d0a 636f 6e64   of, or is..cond
+00009110: 6974 696f 6e65 6420 6f6e 2074 6865 206e  itioned on the n
+00009120: 6f6e 2d65 7865 7263 6973 6520 6f66 206f  on-exercise of o
+00009130: 6e65 206f 7220 6d6f 7265 206f 6620 7468  ne or more of th
+00009140: 6520 7269 6768 7473 2074 6861 7420 6172  e rights that ar
+00009150: 650d 0a73 7065 6369 6669 6361 6c6c 7920  e..specifically 
+00009160: 6772 616e 7465 6420 756e 6465 7220 7468  granted under th
+00009170: 6973 204c 6963 656e 7365 2e20 2059 6f75  is License.  You
+00009180: 206d 6179 206e 6f74 2063 6f6e 7665 7920   may not convey 
+00009190: 6120 636f 7665 7265 640d 0a77 6f72 6b20  a covered..work 
+000091a0: 6966 2079 6f75 2061 7265 2061 2070 6172  if you are a par
+000091b0: 7479 2074 6f20 616e 2061 7272 616e 6765  ty to an arrange
+000091c0: 6d65 6e74 2077 6974 6820 6120 7468 6972  ment with a thir
+000091d0: 6420 7061 7274 7920 7468 6174 2069 730d  d party that is.
+000091e0: 0a69 6e20 7468 6520 6275 7369 6e65 7373  .in the business
+000091f0: 206f 6620 6469 7374 7269 6275 7469 6e67   of distributing
+00009200: 2073 6f66 7477 6172 652c 2075 6e64 6572   software, under
+00009210: 2077 6869 6368 2079 6f75 206d 616b 6520   which you make 
+00009220: 7061 796d 656e 740d 0a74 6f20 7468 6520  payment..to the 
+00009230: 7468 6972 6420 7061 7274 7920 6261 7365  third party base
+00009240: 6420 6f6e 2074 6865 2065 7874 656e 7420  d on the extent 
+00009250: 6f66 2079 6f75 7220 6163 7469 7669 7479  of your activity
+00009260: 206f 6620 636f 6e76 6579 696e 670d 0a74   of conveying..t
+00009270: 6865 2077 6f72 6b2c 2061 6e64 2075 6e64  he work, and und
+00009280: 6572 2077 6869 6368 2074 6865 2074 6869  er which the thi
+00009290: 7264 2070 6172 7479 2067 7261 6e74 732c  rd party grants,
+000092a0: 2074 6f20 616e 7920 6f66 2074 6865 0d0a   to any of the..
+000092b0: 7061 7274 6965 7320 7768 6f20 776f 756c  parties who woul
+000092c0: 6420 7265 6365 6976 6520 7468 6520 636f  d receive the co
+000092d0: 7665 7265 6420 776f 726b 2066 726f 6d20  vered work from 
+000092e0: 796f 752c 2061 2064 6973 6372 696d 696e  you, a discrimin
+000092f0: 6174 6f72 790d 0a70 6174 656e 7420 6c69  atory..patent li
+00009300: 6365 6e73 6520 2861 2920 696e 2063 6f6e  cense (a) in con
+00009310: 6e65 6374 696f 6e20 7769 7468 2063 6f70  nection with cop
+00009320: 6965 7320 6f66 2074 6865 2063 6f76 6572  ies of the cover
+00009330: 6564 2077 6f72 6b0d 0a63 6f6e 7665 7965  ed work..conveye
+00009340: 6420 6279 2079 6f75 2028 6f72 2063 6f70  d by you (or cop
+00009350: 6965 7320 6d61 6465 2066 726f 6d20 7468  ies made from th
+00009360: 6f73 6520 636f 7069 6573 292c 206f 7220  ose copies), or 
+00009370: 2862 2920 7072 696d 6172 696c 790d 0a66  (b) primarily..f
+00009380: 6f72 2061 6e64 2069 6e20 636f 6e6e 6563  or and in connec
+00009390: 7469 6f6e 2077 6974 6820 7370 6563 6966  tion with specif
+000093a0: 6963 2070 726f 6475 6374 7320 6f72 2063  ic products or c
+000093b0: 6f6d 7069 6c61 7469 6f6e 7320 7468 6174  ompilations that
+000093c0: 0d0a 636f 6e74 6169 6e20 7468 6520 636f  ..contain the co
+000093d0: 7665 7265 6420 776f 726b 2c20 756e 6c65  vered work, unle
+000093e0: 7373 2079 6f75 2065 6e74 6572 6564 2069  ss you entered i
+000093f0: 6e74 6f20 7468 6174 2061 7272 616e 6765  nto that arrange
+00009400: 6d65 6e74 2c0d 0a6f 7220 7468 6174 2070  ment,..or that p
+00009410: 6174 656e 7420 6c69 6365 6e73 6520 7761  atent license wa
+00009420: 7320 6772 616e 7465 642c 2070 7269 6f72  s granted, prior
+00009430: 2074 6f20 3238 204d 6172 6368 2032 3030   to 28 March 200
+00009440: 372e 0d0a 0d0a 2020 4e6f 7468 696e 6720  7.....  Nothing 
+00009450: 696e 2074 6869 7320 4c69 6365 6e73 6520  in this License 
+00009460: 7368 616c 6c20 6265 2063 6f6e 7374 7275  shall be constru
+00009470: 6564 2061 7320 6578 636c 7564 696e 6720  ed as excluding 
+00009480: 6f72 206c 696d 6974 696e 670d 0a61 6e79  or limiting..any
+00009490: 2069 6d70 6c69 6564 206c 6963 656e 7365   implied license
+000094a0: 206f 7220 6f74 6865 7220 6465 6665 6e73   or other defens
+000094b0: 6573 2074 6f20 696e 6672 696e 6765 6d65  es to infringeme
+000094c0: 6e74 2074 6861 7420 6d61 790d 0a6f 7468  nt that may..oth
+000094d0: 6572 7769 7365 2062 6520 6176 6169 6c61  erwise be availa
+000094e0: 626c 6520 746f 2079 6f75 2075 6e64 6572  ble to you under
+000094f0: 2061 7070 6c69 6361 626c 6520 7061 7465   applicable pate
+00009500: 6e74 206c 6177 2e0d 0a0d 0a20 2031 322e  nt law.....  12.
+00009510: 204e 6f20 5375 7272 656e 6465 7220 6f66   No Surrender of
+00009520: 204f 7468 6572 7327 2046 7265 6564 6f6d   Others' Freedom
+00009530: 2e0d 0a0d 0a20 2049 6620 636f 6e64 6974  .....  If condit
+00009540: 696f 6e73 2061 7265 2069 6d70 6f73 6564  ions are imposed
+00009550: 206f 6e20 796f 7520 2877 6865 7468 6572   on you (whether
+00009560: 2062 7920 636f 7572 7420 6f72 6465 722c   by court order,
+00009570: 2061 6772 6565 6d65 6e74 206f 720d 0a6f   agreement or..o
+00009580: 7468 6572 7769 7365 2920 7468 6174 2063  therwise) that c
+00009590: 6f6e 7472 6164 6963 7420 7468 6520 636f  ontradict the co
+000095a0: 6e64 6974 696f 6e73 206f 6620 7468 6973  nditions of this
+000095b0: 204c 6963 656e 7365 2c20 7468 6579 2064   License, they d
+000095c0: 6f20 6e6f 740d 0a65 7863 7573 6520 796f  o not..excuse yo
+000095d0: 7520 6672 6f6d 2074 6865 2063 6f6e 6469  u from the condi
+000095e0: 7469 6f6e 7320 6f66 2074 6869 7320 4c69  tions of this Li
+000095f0: 6365 6e73 652e 2020 4966 2079 6f75 2063  cense.  If you c
+00009600: 616e 6e6f 7420 636f 6e76 6579 2061 0d0a  annot convey a..
+00009610: 636f 7665 7265 6420 776f 726b 2073 6f20  covered work so 
+00009620: 6173 2074 6f20 7361 7469 7366 7920 7369  as to satisfy si
+00009630: 6d75 6c74 616e 656f 7573 6c79 2079 6f75  multaneously you
+00009640: 7220 6f62 6c69 6761 7469 6f6e 7320 756e  r obligations un
+00009650: 6465 7220 7468 6973 0d0a 4c69 6365 6e73  der this..Licens
+00009660: 6520 616e 6420 616e 7920 6f74 6865 7220  e and any other 
+00009670: 7065 7274 696e 656e 7420 6f62 6c69 6761  pertinent obliga
+00009680: 7469 6f6e 732c 2074 6865 6e20 6173 2061  tions, then as a
+00009690: 2063 6f6e 7365 7175 656e 6365 2079 6f75   consequence you
+000096a0: 206d 6179 0d0a 6e6f 7420 636f 6e76 6579   may..not convey
+000096b0: 2069 7420 6174 2061 6c6c 2e20 2046 6f72   it at all.  For
+000096c0: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
+000096d0: 2061 6772 6565 2074 6f20 7465 726d 7320   agree to terms 
+000096e0: 7468 6174 206f 626c 6967 6174 6520 796f  that obligate yo
+000096f0: 750d 0a74 6f20 636f 6c6c 6563 7420 6120  u..to collect a 
+00009700: 726f 7961 6c74 7920 666f 7220 6675 7274  royalty for furt
+00009710: 6865 7220 636f 6e76 6579 696e 6720 6672  her conveying fr
+00009720: 6f6d 2074 686f 7365 2074 6f20 7768 6f6d  om those to whom
+00009730: 2079 6f75 2063 6f6e 7665 790d 0a74 6865   you convey..the
+00009740: 2050 726f 6772 616d 2c20 7468 6520 6f6e   Program, the on
+00009750: 6c79 2077 6179 2079 6f75 2063 6f75 6c64  ly way you could
+00009760: 2073 6174 6973 6679 2062 6f74 6820 7468   satisfy both th
+00009770: 6f73 6520 7465 726d 7320 616e 6420 7468  ose terms and th
+00009780: 6973 0d0a 4c69 6365 6e73 6520 776f 756c  is..License woul
+00009790: 6420 6265 2074 6f20 7265 6672 6169 6e20  d be to refrain 
+000097a0: 656e 7469 7265 6c79 2066 726f 6d20 636f  entirely from co
+000097b0: 6e76 6579 696e 6720 7468 6520 5072 6f67  nveying the Prog
+000097c0: 7261 6d2e 0d0a 0d0a 2020 3133 2e20 5573  ram.....  13. Us
+000097d0: 6520 7769 7468 2074 6865 2047 4e55 2041  e with the GNU A
+000097e0: 6666 6572 6f20 4765 6e65 7261 6c20 5075  ffero General Pu
+000097f0: 626c 6963 204c 6963 656e 7365 2e0d 0a0d  blic License....
+00009800: 0a20 204e 6f74 7769 7468 7374 616e 6469  .  Notwithstandi
+00009810: 6e67 2061 6e79 206f 7468 6572 2070 726f  ng any other pro
+00009820: 7669 7369 6f6e 206f 6620 7468 6973 204c  vision of this L
+00009830: 6963 656e 7365 2c20 796f 7520 6861 7665  icense, you have
+00009840: 0d0a 7065 726d 6973 7369 6f6e 2074 6f20  ..permission to 
+00009850: 6c69 6e6b 206f 7220 636f 6d62 696e 6520  link or combine 
+00009860: 616e 7920 636f 7665 7265 6420 776f 726b  any covered work
+00009870: 2077 6974 6820 6120 776f 726b 206c 6963   with a work lic
+00009880: 656e 7365 640d 0a75 6e64 6572 2076 6572  ensed..under ver
+00009890: 7369 6f6e 2033 206f 6620 7468 6520 474e  sion 3 of the GN
+000098a0: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
+000098b0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000098c0: 696e 746f 2061 2073 696e 676c 650d 0a63  into a single..c
+000098d0: 6f6d 6269 6e65 6420 776f 726b 2c20 616e  ombined work, an
+000098e0: 6420 746f 2063 6f6e 7665 7920 7468 6520  d to convey the 
+000098f0: 7265 7375 6c74 696e 6720 776f 726b 2e20  resulting work. 
+00009900: 2054 6865 2074 6572 6d73 206f 6620 7468   The terms of th
+00009910: 6973 0d0a 4c69 6365 6e73 6520 7769 6c6c  is..License will
+00009920: 2063 6f6e 7469 6e75 6520 746f 2061 7070   continue to app
+00009930: 6c79 2074 6f20 7468 6520 7061 7274 2077  ly to the part w
+00009940: 6869 6368 2069 7320 7468 6520 636f 7665  hich is the cove
+00009950: 7265 6420 776f 726b 2c0d 0a62 7574 2074  red work,..but t
+00009960: 6865 2073 7065 6369 616c 2072 6571 7569  he special requi
+00009970: 7265 6d65 6e74 7320 6f66 2074 6865 2047  rements of the G
+00009980: 4e55 2041 6666 6572 6f20 4765 6e65 7261  NU Affero Genera
+00009990: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000099a0: 2c0d 0a73 6563 7469 6f6e 2031 332c 2063  ,..section 13, c
+000099b0: 6f6e 6365 726e 696e 6720 696e 7465 7261  oncerning intera
+000099c0: 6374 696f 6e20 7468 726f 7567 6820 6120  ction through a 
+000099d0: 6e65 7477 6f72 6b20 7769 6c6c 2061 7070  network will app
+000099e0: 6c79 2074 6f20 7468 650d 0a63 6f6d 6269  ly to the..combi
+000099f0: 6e61 7469 6f6e 2061 7320 7375 6368 2e0d  nation as such..
+00009a00: 0a0d 0a20 2031 342e 2052 6576 6973 6564  ...  14. Revised
+00009a10: 2056 6572 7369 6f6e 7320 6f66 2074 6869   Versions of thi
+00009a20: 7320 4c69 6365 6e73 652e 0d0a 0d0a 2020  s License.....  
+00009a30: 5468 6520 4672 6565 2053 6f66 7477 6172  The Free Softwar
+00009a40: 6520 466f 756e 6461 7469 6f6e 206d 6179  e Foundation may
+00009a50: 2070 7562 6c69 7368 2072 6576 6973 6564   publish revised
+00009a60: 2061 6e64 2f6f 7220 6e65 7720 7665 7273   and/or new vers
+00009a70: 696f 6e73 206f 660d 0a74 6865 2047 4e55  ions of..the GNU
+00009a80: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+00009a90: 4c69 6365 6e73 6520 6672 6f6d 2074 696d  License from tim
+00009aa0: 6520 746f 2074 696d 652e 2020 5375 6368  e to time.  Such
+00009ab0: 206e 6577 2076 6572 7369 6f6e 7320 7769   new versions wi
+00009ac0: 6c6c 0d0a 6265 2073 696d 696c 6172 2069  ll..be similar i
+00009ad0: 6e20 7370 6972 6974 2074 6f20 7468 6520  n spirit to the 
+00009ae0: 7072 6573 656e 7420 7665 7273 696f 6e2c  present version,
+00009af0: 2062 7574 206d 6179 2064 6966 6665 7220   but may differ 
+00009b00: 696e 2064 6574 6169 6c20 746f 0d0a 6164  in detail to..ad
+00009b10: 6472 6573 7320 6e65 7720 7072 6f62 6c65  dress new proble
+00009b20: 6d73 206f 7220 636f 6e63 6572 6e73 2e0d  ms or concerns..
+00009b30: 0a0d 0a20 2045 6163 6820 7665 7273 696f  ...  Each versio
+00009b40: 6e20 6973 2067 6976 656e 2061 2064 6973  n is given a dis
+00009b50: 7469 6e67 7569 7368 696e 6720 7665 7273  tinguishing vers
+00009b60: 696f 6e20 6e75 6d62 6572 2e20 2049 6620  ion number.  If 
+00009b70: 7468 650d 0a50 726f 6772 616d 2073 7065  the..Program spe
+00009b80: 6369 6669 6573 2074 6861 7420 6120 6365  cifies that a ce
+00009b90: 7274 6169 6e20 6e75 6d62 6572 6564 2076  rtain numbered v
+00009ba0: 6572 7369 6f6e 206f 6620 7468 6520 474e  ersion of the GN
+00009bb0: 5520 4765 6e65 7261 6c0d 0a50 7562 6c69  U General..Publi
+00009bc0: 6320 4c69 6365 6e73 6520 226f 7220 616e  c License "or an
+00009bd0: 7920 6c61 7465 7220 7665 7273 696f 6e22  y later version"
+00009be0: 2061 7070 6c69 6573 2074 6f20 6974 2c20   applies to it, 
+00009bf0: 796f 7520 6861 7665 2074 6865 0d0a 6f70  you have the..op
+00009c00: 7469 6f6e 206f 6620 666f 6c6c 6f77 696e  tion of followin
+00009c10: 6720 7468 6520 7465 726d 7320 616e 6420  g the terms and 
+00009c20: 636f 6e64 6974 696f 6e73 2065 6974 6865  conditions eithe
+00009c30: 7220 6f66 2074 6861 7420 6e75 6d62 6572  r of that number
+00009c40: 6564 0d0a 7665 7273 696f 6e20 6f72 206f  ed..version or o
+00009c50: 6620 616e 7920 6c61 7465 7220 7665 7273  f any later vers
+00009c60: 696f 6e20 7075 626c 6973 6865 6420 6279  ion published by
+00009c70: 2074 6865 2046 7265 6520 536f 6674 7761   the Free Softwa
+00009c80: 7265 0d0a 466f 756e 6461 7469 6f6e 2e20  re..Foundation. 
+00009c90: 2049 6620 7468 6520 5072 6f67 7261 6d20   If the Program 
+00009ca0: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
+00009cb0: 2061 2076 6572 7369 6f6e 206e 756d 6265   a version numbe
+00009cc0: 7220 6f66 2074 6865 0d0a 474e 5520 4765  r of the..GNU Ge
+00009cd0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+00009ce0: 656e 7365 2c20 796f 7520 6d61 7920 6368  ense, you may ch
+00009cf0: 6f6f 7365 2061 6e79 2076 6572 7369 6f6e  oose any version
+00009d00: 2065 7665 7220 7075 626c 6973 6865 640d   ever published.
+00009d10: 0a62 7920 7468 6520 4672 6565 2053 6f66  .by the Free Sof
+00009d20: 7477 6172 6520 466f 756e 6461 7469 6f6e  tware Foundation
+00009d30: 2e0d 0a0d 0a20 2049 6620 7468 6520 5072  .....  If the Pr
+00009d40: 6f67 7261 6d20 7370 6563 6966 6965 7320  ogram specifies 
+00009d50: 7468 6174 2061 2070 726f 7879 2063 616e  that a proxy can
+00009d60: 2064 6563 6964 6520 7768 6963 6820 6675   decide which fu
+00009d70: 7475 7265 0d0a 7665 7273 696f 6e73 206f  ture..versions o
+00009d80: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00009d90: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00009da0: 2063 616e 2062 6520 7573 6564 2c20 7468   can be used, th
+00009db0: 6174 2070 726f 7879 2773 0d0a 7075 626c  at proxy's..publ
+00009dc0: 6963 2073 7461 7465 6d65 6e74 206f 6620  ic statement of 
+00009dd0: 6163 6365 7074 616e 6365 206f 6620 6120  acceptance of a 
+00009de0: 7665 7273 696f 6e20 7065 726d 616e 656e  version permanen
+00009df0: 746c 7920 6175 7468 6f72 697a 6573 2079  tly authorizes y
+00009e00: 6f75 0d0a 746f 2063 686f 6f73 6520 7468  ou..to choose th
+00009e10: 6174 2076 6572 7369 6f6e 2066 6f72 2074  at version for t
+00009e20: 6865 2050 726f 6772 616d 2e0d 0a0d 0a20  he Program..... 
+00009e30: 204c 6174 6572 206c 6963 656e 7365 2076   Later license v
+00009e40: 6572 7369 6f6e 7320 6d61 7920 6769 7665  ersions may give
+00009e50: 2079 6f75 2061 6464 6974 696f 6e61 6c20   you additional 
+00009e60: 6f72 2064 6966 6665 7265 6e74 0d0a 7065  or different..pe
+00009e70: 726d 6973 7369 6f6e 732e 2020 486f 7765  rmissions.  Howe
+00009e80: 7665 722c 206e 6f20 6164 6469 7469 6f6e  ver, no addition
+00009e90: 616c 206f 626c 6967 6174 696f 6e73 2061  al obligations a
+00009ea0: 7265 2069 6d70 6f73 6564 206f 6e20 616e  re imposed on an
+00009eb0: 790d 0a61 7574 686f 7220 6f72 2063 6f70  y..author or cop
+00009ec0: 7972 6967 6874 2068 6f6c 6465 7220 6173  yright holder as
+00009ed0: 2061 2072 6573 756c 7420 6f66 2079 6f75   a result of you
+00009ee0: 7220 6368 6f6f 7369 6e67 2074 6f20 666f  r choosing to fo
+00009ef0: 6c6c 6f77 2061 0d0a 6c61 7465 7220 7665  llow a..later ve
+00009f00: 7273 696f 6e2e 0d0a 0d0a 2020 3135 2e20  rsion.....  15. 
+00009f10: 4469 7363 6c61 696d 6572 206f 6620 5761  Disclaimer of Wa
+00009f20: 7272 616e 7479 2e0d 0a0d 0a20 2054 4845  rranty.....  THE
+00009f30: 5245 2049 5320 4e4f 2057 4152 5241 4e54  RE IS NO WARRANT
+00009f40: 5920 464f 5220 5448 4520 5052 4f47 5241  Y FOR THE PROGRA
+00009f50: 4d2c 2054 4f20 5448 4520 4558 5445 4e54  M, TO THE EXTENT
+00009f60: 2050 4552 4d49 5454 4544 2042 590d 0a41   PERMITTED BY..A
+00009f70: 5050 4c49 4341 424c 4520 4c41 572e 2020  PPLICABLE LAW.  
+00009f80: 4558 4345 5054 2057 4845 4e20 4f54 4845  EXCEPT WHEN OTHE
+00009f90: 5257 4953 4520 5354 4154 4544 2049 4e20  RWISE STATED IN 
+00009fa0: 5752 4954 494e 4720 5448 4520 434f 5059  WRITING THE COPY
+00009fb0: 5249 4748 540d 0a48 4f4c 4445 5253 2041  RIGHT..HOLDERS A
+00009fc0: 4e44 2f4f 5220 4f54 4845 5220 5041 5254  ND/OR OTHER PART
+00009fd0: 4945 5320 5052 4f56 4944 4520 5448 4520  IES PROVIDE THE 
+00009fe0: 5052 4f47 5241 4d20 2241 5320 4953 2220  PROGRAM "AS IS" 
+00009ff0: 5749 5448 4f55 5420 5741 5252 414e 5459  WITHOUT WARRANTY
+0000a000: 0d0a 4f46 2041 4e59 204b 494e 442c 2045  ..OF ANY KIND, E
+0000a010: 4954 4845 5220 4558 5052 4553 5345 4420  ITHER EXPRESSED 
+0000a020: 4f52 2049 4d50 4c49 4544 2c20 494e 434c  OR IMPLIED, INCL
+0000a030: 5544 494e 472c 2042 5554 204e 4f54 204c  UDING, BUT NOT L
+0000a040: 494d 4954 4544 2054 4f2c 0d0a 5448 4520  IMITED TO,..THE 
+0000a050: 494d 504c 4945 4420 5741 5252 414e 5449  IMPLIED WARRANTI
+0000a060: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
+0000a070: 494c 4954 5920 414e 4420 4649 544e 4553  ILITY AND FITNES
+0000a080: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
+0000a090: 4152 0d0a 5055 5250 4f53 452e 2020 5448  AR..PURPOSE.  TH
+0000a0a0: 4520 454e 5449 5245 2052 4953 4b20 4153  E ENTIRE RISK AS
+0000a0b0: 2054 4f20 5448 4520 5155 414c 4954 5920   TO THE QUALITY 
+0000a0c0: 414e 4420 5045 5246 4f52 4d41 4e43 4520  AND PERFORMANCE 
+0000a0d0: 4f46 2054 4845 2050 524f 4752 414d 0d0a  OF THE PROGRAM..
+0000a0e0: 4953 2057 4954 4820 594f 552e 2020 5348  IS WITH YOU.  SH
+0000a0f0: 4f55 4c44 2054 4845 2050 524f 4752 414d  OULD THE PROGRAM
+0000a100: 2050 524f 5645 2044 4546 4543 5449 5645   PROVE DEFECTIVE
+0000a110: 2c20 594f 5520 4153 5355 4d45 2054 4845  , YOU ASSUME THE
+0000a120: 2043 4f53 5420 4f46 0d0a 414c 4c20 4e45   COST OF..ALL NE
+0000a130: 4345 5353 4152 5920 5345 5256 4943 494e  CESSARY SERVICIN
+0000a140: 472c 2052 4550 4149 5220 4f52 2043 4f52  G, REPAIR OR COR
+0000a150: 5245 4354 494f 4e2e 0d0a 0d0a 2020 3136  RECTION.....  16
+0000a160: 2e20 4c69 6d69 7461 7469 6f6e 206f 6620  . Limitation of 
+0000a170: 4c69 6162 696c 6974 792e 0d0a 0d0a 2020  Liability.....  
+0000a180: 494e 204e 4f20 4556 454e 5420 554e 4c45  IN NO EVENT UNLE
+0000a190: 5353 2052 4551 5549 5245 4420 4259 2041  SS REQUIRED BY A
+0000a1a0: 5050 4c49 4341 424c 4520 4c41 5720 4f52  PPLICABLE LAW OR
+0000a1b0: 2041 4752 4545 4420 544f 2049 4e20 5752   AGREED TO IN WR
+0000a1c0: 4954 494e 470d 0a57 494c 4c20 414e 5920  ITING..WILL ANY 
+0000a1d0: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
+0000a1e0: 2c20 4f52 2041 4e59 204f 5448 4552 2050  , OR ANY OTHER P
+0000a1f0: 4152 5459 2057 484f 204d 4f44 4946 4945  ARTY WHO MODIFIE
+0000a200: 5320 414e 442f 4f52 2043 4f4e 5645 5953  S AND/OR CONVEYS
+0000a210: 0d0a 5448 4520 5052 4f47 5241 4d20 4153  ..THE PROGRAM AS
+0000a220: 2050 4552 4d49 5454 4544 2041 424f 5645   PERMITTED ABOVE
+0000a230: 2c20 4245 204c 4941 424c 4520 544f 2059  , BE LIABLE TO Y
+0000a240: 4f55 2046 4f52 2044 414d 4147 4553 2c20  OU FOR DAMAGES, 
+0000a250: 494e 434c 5544 494e 4720 414e 590d 0a47  INCLUDING ANY..G
+0000a260: 454e 4552 414c 2c20 5350 4543 4941 4c2c  ENERAL, SPECIAL,
+0000a270: 2049 4e43 4944 454e 5441 4c20 4f52 2043   INCIDENTAL OR C
+0000a280: 4f4e 5345 5155 454e 5449 414c 2044 414d  ONSEQUENTIAL DAM
+0000a290: 4147 4553 2041 5249 5349 4e47 204f 5554  AGES ARISING OUT
+0000a2a0: 204f 4620 5448 450d 0a55 5345 204f 5220   OF THE..USE OR 
+0000a2b0: 494e 4142 494c 4954 5920 544f 2055 5345  INABILITY TO USE
+0000a2c0: 2054 4845 2050 524f 4752 414d 2028 494e   THE PROGRAM (IN
+0000a2d0: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
+0000a2e0: 4c49 4d49 5445 4420 544f 204c 4f53 5320  LIMITED TO LOSS 
+0000a2f0: 4f46 0d0a 4441 5441 204f 5220 4441 5441  OF..DATA OR DATA
+0000a300: 2042 4549 4e47 2052 454e 4445 5245 4420   BEING RENDERED 
+0000a310: 494e 4143 4355 5241 5445 204f 5220 4c4f  INACCURATE OR LO
+0000a320: 5353 4553 2053 5553 5441 494e 4544 2042  SSES SUSTAINED B
+0000a330: 5920 594f 5520 4f52 2054 4849 5244 0d0a  Y YOU OR THIRD..
+0000a340: 5041 5254 4945 5320 4f52 2041 2046 4149  PARTIES OR A FAI
+0000a350: 4c55 5245 204f 4620 5448 4520 5052 4f47  LURE OF THE PROG
+0000a360: 5241 4d20 544f 204f 5045 5241 5445 2057  RAM TO OPERATE W
+0000a370: 4954 4820 414e 5920 4f54 4845 5220 5052  ITH ANY OTHER PR
+0000a380: 4f47 5241 4d53 292c 0d0a 4556 454e 2049  OGRAMS),..EVEN I
+0000a390: 4620 5355 4348 2048 4f4c 4445 5220 4f52  F SUCH HOLDER OR
+0000a3a0: 204f 5448 4552 2050 4152 5459 2048 4153   OTHER PARTY HAS
+0000a3b0: 2042 4545 4e20 4144 5649 5345 4420 4f46   BEEN ADVISED OF
+0000a3c0: 2054 4845 2050 4f53 5349 4249 4c49 5459   THE POSSIBILITY
+0000a3d0: 204f 460d 0a53 5543 4820 4441 4d41 4745   OF..SUCH DAMAGE
+0000a3e0: 532e 0d0a 0d0a 2020 3137 2e20 496e 7465  S.....  17. Inte
+0000a3f0: 7270 7265 7461 7469 6f6e 206f 6620 5365  rpretation of Se
+0000a400: 6374 696f 6e73 2031 3520 616e 6420 3136  ctions 15 and 16
+0000a410: 2e0d 0a0d 0a20 2049 6620 7468 6520 6469  .....  If the di
+0000a420: 7363 6c61 696d 6572 206f 6620 7761 7272  sclaimer of warr
+0000a430: 616e 7479 2061 6e64 206c 696d 6974 6174  anty and limitat
+0000a440: 696f 6e20 6f66 206c 6961 6269 6c69 7479  ion of liability
+0000a450: 2070 726f 7669 6465 640d 0a61 626f 7665   provided..above
+0000a460: 2063 616e 6e6f 7420 6265 2067 6976 656e   cannot be given
+0000a470: 206c 6f63 616c 206c 6567 616c 2065 6666   local legal eff
+0000a480: 6563 7420 6163 636f 7264 696e 6720 746f  ect according to
+0000a490: 2074 6865 6972 2074 6572 6d73 2c0d 0a72   their terms,..r
+0000a4a0: 6576 6965 7769 6e67 2063 6f75 7274 7320  eviewing courts 
+0000a4b0: 7368 616c 6c20 6170 706c 7920 6c6f 6361  shall apply loca
+0000a4c0: 6c20 6c61 7720 7468 6174 206d 6f73 7420  l law that most 
+0000a4d0: 636c 6f73 656c 7920 6170 7072 6f78 696d  closely approxim
+0000a4e0: 6174 6573 0d0a 616e 2061 6273 6f6c 7574  ates..an absolut
+0000a4f0: 6520 7761 6976 6572 206f 6620 616c 6c20  e waiver of all 
+0000a500: 6369 7669 6c20 6c69 6162 696c 6974 7920  civil liability 
+0000a510: 696e 2063 6f6e 6e65 6374 696f 6e20 7769  in connection wi
+0000a520: 7468 2074 6865 0d0a 5072 6f67 7261 6d2c  th the..Program,
+0000a530: 2075 6e6c 6573 7320 6120 7761 7272 616e   unless a warran
+0000a540: 7479 206f 7220 6173 7375 6d70 7469 6f6e  ty or assumption
+0000a550: 206f 6620 6c69 6162 696c 6974 7920 6163   of liability ac
+0000a560: 636f 6d70 616e 6965 7320 610d 0a63 6f70  companies a..cop
+0000a570: 7920 6f66 2074 6865 2050 726f 6772 616d  y of the Program
+0000a580: 2069 6e20 7265 7475 726e 2066 6f72 2061   in return for a
+0000a590: 2066 6565 2e0d 0a0d 0a20 2020 2020 2020   fee.....       
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 454e                EN
+0000a5b0: 4420 4f46 2054 4552 4d53 2041 4e44 2043  D OF TERMS AND C
+0000a5c0: 4f4e 4449 5449 4f4e 530d 0a0d 0a20 2020  ONDITIONS....   
+0000a5d0: 2020 2020 2020 2020 2048 6f77 2074 6f20           How to 
+0000a5e0: 4170 706c 7920 5468 6573 6520 5465 726d  Apply These Term
+0000a5f0: 7320 746f 2059 6f75 7220 4e65 7720 5072  s to Your New Pr
+0000a600: 6f67 7261 6d73 0d0a 0d0a 2020 4966 2079  ograms....  If y
+0000a610: 6f75 2064 6576 656c 6f70 2061 206e 6577  ou develop a new
+0000a620: 2070 726f 6772 616d 2c20 616e 6420 796f   program, and yo
+0000a630: 7520 7761 6e74 2069 7420 746f 2062 6520  u want it to be 
+0000a640: 6f66 2074 6865 2067 7265 6174 6573 740d  of the greatest.
+0000a650: 0a70 6f73 7369 626c 6520 7573 6520 746f  .possible use to
+0000a660: 2074 6865 2070 7562 6c69 632c 2074 6865   the public, the
+0000a670: 2062 6573 7420 7761 7920 746f 2061 6368   best way to ach
+0000a680: 6965 7665 2074 6869 7320 6973 2074 6f20  ieve this is to 
+0000a690: 6d61 6b65 2069 740d 0a66 7265 6520 736f  make it..free so
+0000a6a0: 6674 7761 7265 2077 6869 6368 2065 7665  ftware which eve
+0000a6b0: 7279 6f6e 6520 6361 6e20 7265 6469 7374  ryone can redist
+0000a6c0: 7269 6275 7465 2061 6e64 2063 6861 6e67  ribute and chang
+0000a6d0: 6520 756e 6465 7220 7468 6573 6520 7465  e under these te
+0000a6e0: 726d 732e 0d0a 0d0a 2020 546f 2064 6f20  rms.....  To do 
+0000a6f0: 736f 2c20 6174 7461 6368 2074 6865 2066  so, attach the f
+0000a700: 6f6c 6c6f 7769 6e67 206e 6f74 6963 6573  ollowing notices
+0000a710: 2074 6f20 7468 6520 7072 6f67 7261 6d2e   to the program.
+0000a720: 2020 4974 2069 7320 7361 6665 7374 0d0a    It is safest..
+0000a730: 746f 2061 7474 6163 6820 7468 656d 2074  to attach them t
+0000a740: 6f20 7468 6520 7374 6172 7420 6f66 2065  o the start of e
+0000a750: 6163 6820 736f 7572 6365 2066 696c 6520  ach source file 
+0000a760: 746f 206d 6f73 7420 6566 6665 6374 6976  to most effectiv
+0000a770: 656c 790d 0a73 7461 7465 2074 6865 2065  ely..state the e
+0000a780: 7863 6c75 7369 6f6e 206f 6620 7761 7272  xclusion of warr
+0000a790: 616e 7479 3b20 616e 6420 6561 6368 2066  anty; and each f
+0000a7a0: 696c 6520 7368 6f75 6c64 2068 6176 6520  ile should have 
+0000a7b0: 6174 206c 6561 7374 0d0a 7468 6520 2263  at least..the "c
+0000a7c0: 6f70 7972 6967 6874 2220 6c69 6e65 2061  opyright" line a
+0000a7d0: 6e64 2061 2070 6f69 6e74 6572 2074 6f20  nd a pointer to 
+0000a7e0: 7768 6572 6520 7468 6520 6675 6c6c 206e  where the full n
+0000a7f0: 6f74 6963 6520 6973 2066 6f75 6e64 2e0d  otice is found..
+0000a800: 0a0d 0a20 2020 203c 6f6e 6520 6c69 6e65  ...    <one line
+0000a810: 2074 6f20 6769 7665 2074 6865 2070 726f   to give the pro
+0000a820: 6772 616d 2773 206e 616d 6520 616e 6420  gram's name and 
+0000a830: 6120 6272 6965 6620 6964 6561 206f 6620  a brief idea of 
+0000a840: 7768 6174 2069 7420 646f 6573 2e3e 0d0a  what it does.>..
+0000a850: 2020 2020 436f 7079 7269 6768 7420 2843      Copyright (C
+0000a860: 2920 3c79 6561 723e 2020 3c6e 616d 6520  ) <year>  <name 
+0000a870: 6f66 2061 7574 686f 723e 0d0a 0d0a 2020  of author>....  
+0000a880: 2020 5468 6973 2070 726f 6772 616d 2069    This program i
+0000a890: 7320 6672 6565 2073 6f66 7477 6172 653a  s free software:
+0000a8a0: 2079 6f75 2063 616e 2072 6564 6973 7472   you can redistr
+0000a8b0: 6962 7574 6520 6974 2061 6e64 2f6f 7220  ibute it and/or 
+0000a8c0: 6d6f 6469 6679 0d0a 2020 2020 6974 2075  modify..    it u
+0000a8d0: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
+0000a8e0: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+0000a8f0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+0000a900: 2061 7320 7075 626c 6973 6865 6420 6279   as published by
+0000a910: 0d0a 2020 2020 7468 6520 4672 6565 2053  ..    the Free S
+0000a920: 6f66 7477 6172 6520 466f 756e 6461 7469  oftware Foundati
+0000a930: 6f6e 2c20 6569 7468 6572 2076 6572 7369  on, either versi
+0000a940: 6f6e 2033 206f 6620 7468 6520 4c69 6365  on 3 of the Lice
+0000a950: 6e73 652c 206f 720d 0a20 2020 2028 6174  nse, or..    (at
+0000a960: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
+0000a970: 7920 6c61 7465 7220 7665 7273 696f 6e2e  y later version.
+0000a980: 0d0a 0d0a 2020 2020 5468 6973 2070 726f  ....    This pro
+0000a990: 6772 616d 2069 7320 6469 7374 7269 6275  gram is distribu
+0000a9a0: 7465 6420 696e 2074 6865 2068 6f70 6520  ted in the hope 
+0000a9b0: 7468 6174 2069 7420 7769 6c6c 2062 6520  that it will be 
+0000a9c0: 7573 6566 756c 2c0d 0a20 2020 2062 7574  useful,..    but
+0000a9d0: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+0000a9e0: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+0000a9f0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+0000aa00: 7761 7272 616e 7479 206f 660d 0a20 2020  warranty of..   
+0000aa10: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
+0000aa20: 206f 7220 4649 544e 4553 5320 464f 5220   or FITNESS FOR 
+0000aa30: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
+0000aa40: 504f 5345 2e20 2053 6565 2074 6865 0d0a  POSE.  See the..
+0000aa50: 2020 2020 474e 5520 4765 6e65 7261 6c20      GNU General 
+0000aa60: 5075 626c 6963 204c 6963 656e 7365 2066  Public License f
+0000aa70: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
+0000aa80: 0d0a 0d0a 2020 2020 596f 7520 7368 6f75  ....    You shou
+0000aa90: 6c64 2068 6176 6520 7265 6365 6976 6564  ld have received
+0000aaa0: 2061 2063 6f70 7920 6f66 2074 6865 2047   a copy of the G
+0000aab0: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
+0000aac0: 6320 4c69 6365 6e73 650d 0a20 2020 2061  c License..    a
+0000aad0: 6c6f 6e67 2077 6974 6820 7468 6973 2070  long with this p
+0000aae0: 726f 6772 616d 2e20 2049 6620 6e6f 742c  rogram.  If not,
+0000aaf0: 2073 6565 203c 6874 7470 733a 2f2f 7777   see <https://ww
+0000ab00: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+0000ab10: 6573 2f3e 2e0d 0a0d 0a41 6c73 6f20 6164  es/>.....Also ad
+0000ab20: 6420 696e 666f 726d 6174 696f 6e20 6f6e  d information on
+0000ab30: 2068 6f77 2074 6f20 636f 6e74 6163 7420   how to contact 
+0000ab40: 796f 7520 6279 2065 6c65 6374 726f 6e69  you by electroni
+0000ab50: 6320 616e 6420 7061 7065 7220 6d61 696c  c and paper mail
+0000ab60: 2e0d 0a0d 0a20 2049 6620 7468 6520 7072  .....  If the pr
+0000ab70: 6f67 7261 6d20 646f 6573 2074 6572 6d69  ogram does termi
+0000ab80: 6e61 6c20 696e 7465 7261 6374 696f 6e2c  nal interaction,
+0000ab90: 206d 616b 6520 6974 206f 7574 7075 7420   make it output 
+0000aba0: 6120 7368 6f72 740d 0a6e 6f74 6963 6520  a short..notice 
+0000abb0: 6c69 6b65 2074 6869 7320 7768 656e 2069  like this when i
+0000abc0: 7420 7374 6172 7473 2069 6e20 616e 2069  t starts in an i
+0000abd0: 6e74 6572 6163 7469 7665 206d 6f64 653a  nteractive mode:
+0000abe0: 0d0a 0d0a 2020 2020 3c70 726f 6772 616d  ....    <program
+0000abf0: 3e20 2043 6f70 7972 6967 6874 2028 4329  >  Copyright (C)
+0000ac00: 203c 7965 6172 3e20 203c 6e61 6d65 206f   <year>  <name o
+0000ac10: 6620 6175 7468 6f72 3e0d 0a20 2020 2054  f author>..    T
+0000ac20: 6869 7320 7072 6f67 7261 6d20 636f 6d65  his program come
+0000ac30: 7320 7769 7468 2041 4253 4f4c 5554 454c  s with ABSOLUTEL
+0000ac40: 5920 4e4f 2057 4152 5241 4e54 593b 2066  Y NO WARRANTY; f
+0000ac50: 6f72 2064 6574 6169 6c73 2074 7970 6520  or details type 
+0000ac60: 6073 686f 7720 7727 2e0d 0a20 2020 2054  `show w'...    T
+0000ac70: 6869 7320 6973 2066 7265 6520 736f 6674  his is free soft
+0000ac80: 7761 7265 2c20 616e 6420 796f 7520 6172  ware, and you ar
+0000ac90: 6520 7765 6c63 6f6d 6520 746f 2072 6564  e welcome to red
+0000aca0: 6973 7472 6962 7574 6520 6974 0d0a 2020  istribute it..  
+0000acb0: 2020 756e 6465 7220 6365 7274 6169 6e20    under certain 
+0000acc0: 636f 6e64 6974 696f 6e73 3b20 7479 7065  conditions; type
+0000acd0: 2060 7368 6f77 2063 2720 666f 7220 6465   `show c' for de
+0000ace0: 7461 696c 732e 0d0a 0d0a 5468 6520 6879  tails.....The hy
+0000acf0: 706f 7468 6574 6963 616c 2063 6f6d 6d61  pothetical comma
+0000ad00: 6e64 7320 6073 686f 7720 7727 2061 6e64  nds `show w' and
+0000ad10: 2060 7368 6f77 2063 2720 7368 6f75 6c64   `show c' should
+0000ad20: 2073 686f 7720 7468 6520 6170 7072 6f70   show the approp
+0000ad30: 7269 6174 650d 0a70 6172 7473 206f 6620  riate..parts of 
+0000ad40: 7468 6520 4765 6e65 7261 6c20 5075 626c  the General Publ
+0000ad50: 6963 204c 6963 656e 7365 2e20 204f 6620  ic License.  Of 
+0000ad60: 636f 7572 7365 2c20 796f 7572 2070 726f  course, your pro
+0000ad70: 6772 616d 2773 2063 6f6d 6d61 6e64 730d  gram's commands.
+0000ad80: 0a6d 6967 6874 2062 6520 6469 6666 6572  .might be differ
+0000ad90: 656e 743b 2066 6f72 2061 2047 5549 2069  ent; for a GUI i
+0000ada0: 6e74 6572 6661 6365 2c20 796f 7520 776f  nterface, you wo
+0000adb0: 756c 6420 7573 6520 616e 2022 6162 6f75  uld use an "abou
+0000adc0: 7420 626f 7822 2e0d 0a0d 0a20 2059 6f75  t box".....  You
+0000add0: 2073 686f 756c 6420 616c 736f 2067 6574   should also get
+0000ade0: 2079 6f75 7220 656d 706c 6f79 6572 2028   your employer (
+0000adf0: 6966 2079 6f75 2077 6f72 6b20 6173 2061  if you work as a
+0000ae00: 2070 726f 6772 616d 6d65 7229 206f 7220   programmer) or 
+0000ae10: 7363 686f 6f6c 2c0d 0a69 6620 616e 792c  school,..if any,
+0000ae20: 2074 6f20 7369 676e 2061 2022 636f 7079   to sign a "copy
+0000ae30: 7269 6768 7420 6469 7363 6c61 696d 6572  right disclaimer
+0000ae40: 2220 666f 7220 7468 6520 7072 6f67 7261  " for the progra
+0000ae50: 6d2c 2069 6620 6e65 6365 7373 6172 792e  m, if necessary.
+0000ae60: 0d0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
+0000ae70: 6d61 7469 6f6e 206f 6e20 7468 6973 2c20  mation on this, 
+0000ae80: 616e 6420 686f 7720 746f 2061 7070 6c79  and how to apply
+0000ae90: 2061 6e64 2066 6f6c 6c6f 7720 7468 6520   and follow the 
+0000aea0: 474e 5520 4750 4c2c 2073 6565 0d0a 3c68  GNU GPL, see..<h
+0000aeb0: 7474 7073 3a2f 2f77 7777 2e67 6e75 2e6f  ttps://www.gnu.o
+0000aec0: 7267 2f6c 6963 656e 7365 732f 3e2e 0d0a  rg/licenses/>...
+0000aed0: 0d0a 2020 5468 6520 474e 5520 4765 6e65  ..  The GNU Gene
+0000aee0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+0000aef0: 7365 2064 6f65 7320 6e6f 7420 7065 726d  se does not perm
+0000af00: 6974 2069 6e63 6f72 706f 7261 7469 6e67  it incorporating
+0000af10: 2079 6f75 7220 7072 6f67 7261 6d0d 0a69   your program..i
+0000af20: 6e74 6f20 7072 6f70 7269 6574 6172 7920  nto proprietary 
+0000af30: 7072 6f67 7261 6d73 2e20 2049 6620 796f  programs.  If yo
+0000af40: 7572 2070 726f 6772 616d 2069 7320 6120  ur program is a 
+0000af50: 7375 6272 6f75 7469 6e65 206c 6962 7261  subroutine libra
+0000af60: 7279 2c20 796f 750d 0a6d 6179 2063 6f6e  ry, you..may con
+0000af70: 7369 6465 7220 6974 206d 6f72 6520 7573  sider it more us
+0000af80: 6566 756c 2074 6f20 7065 726d 6974 206c  eful to permit l
+0000af90: 696e 6b69 6e67 2070 726f 7072 6965 7461  inking proprieta
+0000afa0: 7279 2061 7070 6c69 6361 7469 6f6e 7320  ry applications 
+0000afb0: 7769 7468 0d0a 7468 6520 6c69 6272 6172  with..the librar
+0000afc0: 792e 2020 4966 2074 6869 7320 6973 2077  y.  If this is w
+0000afd0: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
+0000afe0: 646f 2c20 7573 6520 7468 6520 474e 5520  do, use the GNU 
+0000aff0: 4c65 7373 6572 2047 656e 6572 616c 0d0a  Lesser General..
+0000b000: 5075 626c 6963 204c 6963 656e 7365 2069  Public License i
+0000b010: 6e73 7465 6164 206f 6620 7468 6973 204c  nstead of this L
+0000b020: 6963 656e 7365 2e20 2042 7574 2066 6972  icense.  But fir
+0000b030: 7374 2c20 706c 6561 7365 2072 6561 640d  st, please read.
+0000b040: 0a3c 6874 7470 733a 2f2f 7777 772e 676e  .<https://www.gn
+0000b050: 752e 6f72 672f 6c69 6365 6e73 6573 2f77  u.org/licenses/w
+0000b060: 6879 2d6e 6f74 2d6c 6770 6c2e 6874 6d6c  hy-not-lgpl.html
+0000b070: 3e2e 0d0a                                >...
```

### Comparing `osm_easy_api-0.4.2/README.md` & `osm_easy_api-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,283 +1,310 @@
-00000000: 2320 6f73 6d5f 6561 7379 5f61 7069 0d0a  # osm_easy_api..
-00000010: 0d0a 215b 5465 7374 735d 2868 7474 7073  ..![Tests](https
-00000020: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-00000030: 6365 6e74 5954 2f61 7574 6f6d 6174 6564  centYT/automated
-00000040: 2d70 7974 686f 6e2d 7465 7374 732d 7465  -python-tests-te
-00000050: 7374 696e 672d 7265 706f 2f61 6374 696f  sting-repo/actio
-00000060: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
-00000070: 7473 2e79 616d 6c2f 6261 6467 652e 7376  ts.yaml/badge.sv
-00000080: 6729 0d0a 215b 636f 7665 7261 6765 5d28  g)..![coverage](
-00000090: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
-000000a0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000000b0: 6d2f 646f 6365 6e74 5954 2f6f 736d 5f65  m/docentYT/osm_e
-000000c0: 6173 795f 6170 692f 3338 3839 6165 3632  asy_api/3889ae62
-000000d0: 3662 6533 3531 3833 3235 3334 3835 3634  6be3518325348564
-000000e0: 3662 3762 6539 6532 3335 6132 6663 3237  6b7be9e235a2fc27
-000000f0: 2f63 6f76 6572 6167 652d 6261 6467 652e  /coverage-badge.
-00000100: 7376 6729 0d0a 5b21 5b50 7950 4920 7665  svg)..[![PyPI ve
-00000110: 7273 696f 6e5d 2868 7474 7073 3a2f 2f62  rsion](https://b
-00000120: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
-00000130: 6f73 6d5f 6561 7379 5f61 7069 2e73 7667  osm_easy_api.svg
-00000140: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
-00000150: 2e66 7572 792e 696f 2f70 792f 6f73 6d5f  .fury.io/py/osm_
-00000160: 6561 7379 5f61 7069 290d 0a0d 0a5b 4d65  easy_api)....[Me
-00000170: 206f 6e20 6f70 656e 7374 7265 6574 6d61   on openstreetma
-00000180: 705d 2868 7474 7073 3a2f 2f77 7777 2e6f  p](https://www.o
-00000190: 7065 6e73 7472 6565 746d 6170 2e6f 7267  penstreetmap.org
-000001a0: 2f75 7365 722f 6b77 6961 7465 6b5f 3132  /user/kwiatek_12
-000001b0: 3329 0d0a 0d0a 5079 7468 6f6e 2070 6163  3)....Python pac
-000001c0: 6b61 6765 2066 6f72 2070 6172 7369 6e67  kage for parsing
-000001d0: 206f 736d 2064 6966 6673 2061 6e64 2063   osm diffs and c
-000001e0: 6f6d 6d75 6e69 6361 7469 6e67 2077 6974  ommunicating wit
-000001f0: 6820 7468 6520 6f73 6d20 6170 692e 2053  h the osm api. S
-00000200: 6565 2041 5049 2e74 7874 2066 6f72 206c  ee API.txt for l
-00000210: 6973 7420 6f66 2073 7570 706f 7274 6564  ist of supported
-00000220: 2065 6e64 706f 696e 7473 2e0d 0a0d 0a23   endpoints.....#
-00000230: 2320 5768 6174 2773 2074 6865 2070 6f69  # What's the poi
-00000240: 6e74 206f 6620 7468 6973 2070 6163 6b61  nt of this packa
-00000250: 6765 3f0d 0a0d 0a54 6869 7320 7061 636b  ge?....This pack
-00000260: 6167 6520 7761 7320 6372 6561 7465 6420  age was created 
-00000270: 746f 2070 726f 7669 6465 2061 6e20 6561  to provide an ea
-00000280: 7379 2077 6179 2074 6f20 6372 6561 7465  sy way to create
-00000290: 2061 7574 6f6d 6174 6564 2073 6372 6970   automated scrip
-000002a0: 7473 2061 6e64 2070 726f 6772 616d 7320  ts and programs 
-000002b0: 7468 6174 2075 7365 2064 6966 6620 616e  that use diff an
-000002c0: 642f 6f72 206f 736d 2061 7069 2e20 5468  d/or osm api. Th
-000002d0: 6520 6d61 696e 2061 6476 616e 7461 6765  e main advantage
-000002e0: 2069 7320 7468 6520 636c 6173 7365 7320   is the classes 
-000002f0: 2864 6174 615f 636c 6173 7365 7329 2074  (data_classes) t
-00000300: 6861 7420 7072 6f76 6964 6520 6461 7461  hat provide data
-00000310: 206f 6620 656c 656d 656e 7473 2028 6e6f   of elements (no
-00000320: 6465 2c20 7761 792c 2072 656c 6174 696f  de, way, relatio
-00000330: 6e2c 204f 736d 4368 616e 6765 2c20 6574  n, OsmChange, et
-00000340: 632e 2920 696e 2061 2072 6561 6461 626c  c.) in a readabl
-00000350: 6520 7761 7920 616e 6420 7468 6520 706f  e way and the po
-00000360: 7373 6962 696c 6974 7920 746f 2075 7365  ssibility to use
-00000370: 2074 6865 6d20 696e 2064 6966 6620 616e   them in diff an
-00000380: 6420 6170 6920 7769 7468 6f75 7420 776f  d api without wo
-00000390: 7272 7969 6e67 2061 626f 7574 206d 6973  rrying about mis
-000003a0: 7369 6e67 2064 6174 6120 6f72 2064 6963  sing data or dic
-000003b0: 7469 6f6e 6172 6965 732e 2059 6f75 2063  tionaries. You c
-000003c0: 616e 2065 6173 696c 7920 6669 6e64 206e  an easily find n
-000003d0: 6f64 6573 2069 6e20 6469 6666 2c20 6164  odes in diff, ad
-000003e0: 6420 6120 7461 6720 746f 2074 6865 6d20  d a tag to them 
-000003f0: 616e 6420 7365 6e64 2074 6865 2063 6f72  and send the cor
-00000400: 7265 6374 6564 2076 6572 7369 6f6e 2074  rected version t
-00000410: 6f20 6f73 6d2e 0d0a 0d0a 2323 2057 6861  o osm.....## Wha
-00000420: 7420 6e65 7874 3f0d 0a54 6865 2070 6c61  t next?..The pla
-00000430: 6e20 6973 2074 6f20 6f70 7469 6d69 7365  n is to optimise
-00000440: 2061 6e64 2069 6d70 726f 7665 2074 6865   and improve the
-00000450: 2063 6f64 652c 2061 6464 2073 7570 706f   code, add suppo
-00000460: 7274 2066 6f72 2067 7078 2074 7261 6365  rt for gpx trace
-00000470: 732c 2072 7373 2073 7570 706f 7274 2061  s, rss support a
-00000480: 6e64 206f 7665 7270 6173 7320 6170 692e  nd overpass api.
-00000490: 0d0a 0d0a 2320 496e 7374 616c 6c61 7469  ....# Installati
-000004a0: 6f6e 0d0a 0d0a 576f 726b 7320 6f6e 2070  on....Works on p
-000004b0: 7974 686f 6e20 3e3d 2033 2e31 302e 2028  ython >= 3.10. (
-000004c0: 4475 6520 746f 206e 6577 2074 7970 6568  Due to new typeh
-000004d0: 696e 7473 2073 7461 6e64 6172 6429 0d0a  ints standard)..
-000004e0: 0d0a 496e 7374 616c 6c20 606f 736d 5f65  ..Install `osm_e
-000004f0: 6173 795f 6170 6960 2066 726f 6d20 5b50  asy_api` from [P
-00000500: 7950 695d 2868 7474 7073 3a2f 2f70 7970  yPi](https://pyp
-00000510: 692e 6f72 672f 7072 6f6a 6563 742f 6f73  i.org/project/os
-00000520: 6d2d 6561 7379 2d61 7069 2f29 3a0d 0a60  m-easy-api/):..`
-00000530: 6060 0d0a 7069 7020 696e 7374 616c 6c20  ``..pip install 
-00000540: 6f73 6d5f 6561 7379 5f61 7069 0d0a 6060  osm_easy_api..``
-00000550: 6020 0d0a 0d0a 2320 446f 6375 6d65 6e74  ` ....# Document
-00000560: 6174 696f 6e0d 0a0d 0a59 6f75 2063 616e  ation....You can
-00000570: 2076 6965 7720 646f 6375 6d65 6e74 6174   view documentat
-00000580: 696f 6e20 6f6e 205b 6769 7468 7562 2d70  ion on [github-p
-00000590: 6167 6573 5d28 6874 7470 733a 2f2f 646f  ages](https://do
-000005a0: 6365 6e74 7974 2e67 6974 6875 622e 696f  centyt.github.io
-000005b0: 2f6f 736d 5f65 6173 795f 6170 692f 6f73  /osm_easy_api/os
-000005c0: 6d5f 6561 7379 5f61 7069 2e68 746d 6c29  m_easy_api.html)
-000005d0: 2e0d 0a0d 0a44 6f63 756d 656e 7461 7469  .....Documentati
-000005e0: 6f6e 2069 7320 6275 696c 6420 7573 696e  on is build usin
-000005f0: 6720 5b70 646f 635d 2868 7474 7073 3a2f  g [pdoc](https:/
-00000600: 2f70 646f 632e 6465 7629 2e0d 0a54 6f20  /pdoc.dev)...To 
-00000610: 7275 6e20 646f 6373 206f 6e20 796f 7572  run docs on your
-00000620: 206d 6163 6869 6e65 2075 7365 2070 7265   machine use pre
-00000630: 6665 7272 6564 2063 6f6d 6d61 6e64 3a20  ferred command: 
-00000640: 6070 646f 6320 2d2d 646f 6366 6f72 6d61  `pdoc --docforma
-00000650: 7420 676f 6f67 6c65 202d 2d6e 6f2d 7368  t google --no-sh
-00000660: 6f77 2d73 6f75 7263 6520 6f73 6d5f 6561  ow-source osm_ea
-00000670: 7379 5f61 7069 2021 6f73 6d5f 6561 7379  sy_api !osm_easy
-00000680: 5f61 7069 2e75 7469 6c73 602e 0d0a 0d0a  _api.utils`.....
-00000690: 2320 4578 616d 706c 6573 0d0a 0d0a 2323  # Examples....##
-000006a0: 2044 4946 460d 0a0d 0a23 2323 2050 7269   DIFF....### Pri
-000006b0: 6e74 2074 7265 6573 0d0a 0d0a 6060 6070  nt trees....```p
-000006c0: 790d 0a66 726f 6d20 6f73 6d5f 6561 7379  y..from osm_easy
-000006d0: 5f61 7069 2069 6d70 6f72 7420 4e6f 6465  _api import Node
-000006e0: 2c20 4469 6666 2c20 4672 6571 7565 6e63  , Diff, Frequenc
-000006f0: 790d 0a0d 0a23 2044 6f77 6e6c 6f61 6420  y....# Download 
-00000700: 6469 6666 2066 726f 6d20 6c61 7374 2068  diff from last h
-00000710: 6f75 722e 0d0a 6420 3d20 4469 6666 2846  our...d = Diff(F
-00000720: 7265 7175 656e 6379 2e48 4f55 5229 0d0a  requency.HOUR)..
-00000730: 0d0a 2320 4765 7420 4d65 7461 206e 616d  ..# Get Meta nam
-00000740: 6564 7475 706c 6520 666f 7220 6469 6666  edtuple for diff
-00000750: 206d 6574 6164 6174 6120 616e 6420 6765   metadata and ge
-00000760: 6e65 7261 746f 7220 7468 6174 2070 6172  nerator that par
-00000770: 7365 2064 6966 6620 6669 6c65 2e0d 0a6d  se diff file...m
-00000780: 6574 612c 2067 656e 203d 2064 2e67 6574  eta, gen = d.get
-00000790: 2874 6167 733d 226e 6174 7572 616c 2229  (tags="natural")
-000007a0: 0d0a 0d0a 2320 5072 696e 7420 616c 6c20  ....# Print all 
-000007b0: 6372 6561 7465 642c 206d 6f64 6966 6965  created, modifie
-000007c0: 6420 616e 6420 6465 6c65 7465 6420 4e6f  d and deleted No
-000007d0: 6465 7320 7769 7468 206e 6174 7572 616c  des with natural
-000007e0: 3d74 7265 6520 7461 672e 0d0a 666f 7220  =tree tag...for 
-000007f0: 6163 7469 6f6e 2c20 656c 656d 656e 7420  action, element 
-00000800: 696e 2067 656e 3a0d 0a20 2020 2069 6620  in gen:..    if 
-00000810: 7479 7065 2865 6c65 6d65 6e74 2920 3d3d  type(element) ==
-00000820: 204e 6f64 6520 616e 6420 656c 656d 656e   Node and elemen
-00000830: 742e 7461 6773 2e67 6574 2822 6e61 7475  t.tags.get("natu
-00000840: 7261 6c22 2920 3d3d 2022 7472 6565 223a  ral") == "tree":
-00000850: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00000860: 6163 7469 6f6e 2c20 656c 656d 656e 742e  action, element.
-00000870: 6964 290d 0a60 6060 0d0a 0d0a 2323 2320  id)..```....### 
-00000880: 5072 696e 7420 696e 636f 7272 6563 746c  Print incorrectl
-00000890: 7920 7461 6767 6564 2073 696e 676c 6520  y tagged single 
-000008a0: 7472 6573 730d 0a0d 0a60 6060 7079 0d0a  tress....```py..
-000008b0: 6672 6f6d 206f 736d 5f65 6173 795f 6170  from osm_easy_ap
-000008c0: 6920 696d 706f 7274 2044 6966 662c 2046  i import Diff, F
-000008d0: 7265 7175 656e 6379 2c20 4163 7469 6f6e  requency, Action
-000008e0: 2c20 4e6f 6465 0d0a 0d0a 6420 3d20 4469  , Node....d = Di
-000008f0: 6666 2846 7265 7175 656e 6379 2e44 4159  ff(Frequency.DAY
-00000900: 290d 0a0d 0a6d 6574 612c 2067 656e 203d  )....meta, gen =
-00000910: 2064 2e67 6574 2874 6167 733d 226e 6174   d.get(tags="nat
-00000920: 7572 616c 2229 0d0a 0d0a 666f 7220 6163  ural")....for ac
-00000930: 7469 6f6e 2c20 656c 656d 656e 7420 696e  tion, element in
-00000940: 2067 656e 3a0d 0a20 2020 2069 6620 7479   gen:..    if ty
-00000950: 7065 2865 6c65 6d65 6e74 2920 3d3d 204e  pe(element) == N
-00000960: 6f64 653a 0d0a 2020 2020 2020 2020 6966  ode:..        if
-00000970: 2061 6374 696f 6e20 3d3d 2041 6374 696f   action == Actio
-00000980: 6e2e 4352 4541 5445 206f 7220 6163 7469  n.CREATE or acti
-00000990: 6f6e 203d 3d20 4163 7469 6f6e 2e4d 4f44  on == Action.MOD
-000009a0: 4946 593a 0d0a 2020 2020 2020 2020 2020  IFY:..          
-000009b0: 2020 6966 2065 6c65 6d65 6e74 2e74 6167    if element.tag
-000009c0: 732e 6765 7428 226e 6174 7572 616c 2229  s.get("natural")
-000009d0: 203d 3d20 2277 6f6f 6422 3a0d 0a20 2020   == "wood":..   
-000009e0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000009f0: 6e74 2865 6c65 6d65 6e74 290d 0a60 6060  nt(element)..```
-00000a00: 0d0a 4578 616d 706c 6520 6f75 7470 7574  ..Example output
-00000a10: 3a0d 0a60 6060 0d0a 4e6f 6465 2869 6420  :..```..Node(id 
-00000a20: 3d20 3130 3230 3834 3836 3731 372c 2076  = 10208486717, v
-00000a30: 6973 6962 6c65 203d 204e 6f6e 652c 2076  isible = None, v
-00000a40: 6572 7369 6f6e 203d 2031 2c20 6368 616e  ersion = 1, chan
-00000a50: 6765 7365 745f 6964 203d 2031 3239 3231  geset_id = 12921
-00000a60: 3630 3735 2c20 7469 6d65 7374 616d 7020  6075, timestamp 
-00000a70: 3d20 3230 3232 2d31 312d 3232 5430 303a  = 2022-11-22T00:
-00000a80: 3136 3a34 345a 2c20 7573 6572 5f69 6420  16:44Z, user_id 
-00000a90: 3d20 3137 3437 3137 3231 2c20 7461 6773  = 17471721, tags
-00000aa0: 203d 207b 276c 6561 665f 7479 7065 273a   = {'leaf_type':
-00000ab0: 2027 6272 6f61 646c 6561 7665 6427 2c20   'broadleaved', 
-00000ac0: 276e 6174 7572 616c 273a 2027 776f 6f64  'natural': 'wood
-00000ad0: 277d 2c20 6c61 7469 7475 6465 203d 2034  '}, latitude = 4
-00000ae0: 382e 3635 3232 3238 362c 206c 6f6e 6769  8.6522286, longi
-00000af0: 7475 6465 203d 2031 322e 3538 3338 3039  tude = 12.583809
-00000b00: 2c20 290d 0a60 6060 0d0a 0d0a 2323 2041  , )..```....## A
-00000b10: 5049 0d0a 0d0a 2323 2320 4164 6420 6d69  PI....### Add mi
-00000b20: 7373 696e 6720 7769 6b69 6461 7461 2074  ssing wikidata t
-00000b30: 6167 0d0a 0d0a 6060 6070 790d 0a66 726f  ag....```py..fro
-00000b40: 6d20 6f73 6d5f 6561 7379 5f61 7069 2069  m osm_easy_api i
-00000b50: 6d70 6f72 7420 4170 692c 204e 6f64 652c  mport Api, Node,
-00000b60: 2054 6167 730d 0a0d 0a61 7069 203d 2041   Tags....api = A
-00000b70: 7069 2822 6874 7470 733a 2f2f 6d61 7374  pi("https://mast
-00000b80: 6572 2e61 7069 732e 6465 762e 6f70 656e  er.apis.dev.open
-00000b90: 7374 7265 6574 6d61 702e 6f72 6722 2c20  streetmap.org", 
-00000ba0: 4c4f 4749 4e2c 2050 4153 5357 4f52 4429  LOGIN, PASSWORD)
-00000bb0: 0d0a 0d0a 6e6f 6465 203d 2061 7069 2e65  ....node = api.e
-00000bc0: 6c65 6d65 6e74 732e 6765 7428 4e6f 6465  lements.get(Node
-00000bd0: 2c20 3432 3936 3436 3033 3336 2920 2320  , 4296460336) # 
-00000be0: 5765 2061 7265 2067 6574 7469 6e67 204e  We are getting N
-00000bf0: 6f64 6520 7769 7468 2069 6420 3432 3936  ode with id 4296
-00000c00: 3436 3033 3336 2077 6865 7265 2077 6520  460336 where we 
-00000c10: 7761 6e74 2074 6f20 6164 6420 6120 6e65  want to add a ne
-00000c20: 7720 7461 6720 746f 0d0a 6e6f 6465 2e74  w tag to..node.t
-00000c30: 6167 732e 6164 6428 2277 696b 6964 6174  ags.add("wikidat
-00000c40: 6122 2c20 2251 6578 616d 706c 6522 2920  a", "Qexample") 
-00000c50: 2320 4164 6420 6120 6e65 7720 7461 6720  # Add a new tag 
-00000c60: 746f 206e 6f64 652e 0d0a 0d0a 6d79 5f63  to node.....my_c
-00000c70: 6861 6e67 6573 6574 203d 2061 7069 2e63  hangeset = api.c
-00000c80: 6861 6e67 6573 6574 2e63 7265 6174 6528  hangeset.create(
-00000c90: 2241 6464 206d 6973 7369 6e67 2077 696b  "Add missing wik
-00000ca0: 6964 6174 6120 7461 6722 2c20 5461 6773  idata tag", Tags
-00000cb0: 287b 2261 7574 6f6d 6174 6963 223a 2022  ({"automatic": "
-00000cc0: 7965 7322 7d29 2920 2320 4372 6561 7465  yes"})) # Create
-00000cd0: 206e 6577 2063 6861 6e67 6573 6574 2077   new changeset w
-00000ce0: 6974 6820 6465 7363 7269 7074 696f 6e20  ith description 
-00000cf0: 616e 6420 7461 670d 0a61 7069 2e65 6c65  and tag..api.ele
-00000d00: 6d65 6e74 732e 7570 6461 7465 286e 6f64  ments.update(nod
-00000d10: 652c 206d 795f 6368 616e 6765 7365 7429  e, my_changeset)
-00000d20: 2023 2053 656e 6420 6e65 7720 7665 7273   # Send new vers
-00000d30: 696f 6e20 6f66 2061 206e 6f64 6520 746f  ion of a node to
-00000d40: 206f 736d 0d0a 6170 692e 6368 616e 6765   osm..api.change
-00000d50: 7365 742e 636c 6f73 6528 6d79 5f63 6861  set.close(my_cha
-00000d60: 6e67 6573 6574 2920 2320 436c 6f73 6520  ngeset) # Close 
-00000d70: 6368 616e 6765 7365 742e 0d0a 6060 600d  changeset...```.
-00000d80: 0a0d 0a23 204e 6f74 6573 0d0a 0d0a 4e6f  ...# Notes....No
-00000d90: 7465 2074 6861 7420 7468 6520 666f 6c6c  te that the foll
-00000da0: 6f77 696e 6720 636f 6465 7320 646f 2074  owing codes do t
-00000db0: 6865 2073 616d 6520 7468 696e 670d 0a60  he same thing..`
-00000dc0: 6060 7079 0d0a 6672 6f6d 206f 736d 5f65  ``py..from osm_e
-00000dd0: 6173 795f 6170 6920 696d 706f 7274 2044  asy_api import D
-00000de0: 6966 662c 2046 7265 7175 656e 6379 0d0a  iff, Frequency..
-00000df0: 0d0a 6420 3d20 4469 6666 2846 7265 7175  ..d = Diff(Frequ
-00000e00: 656e 6379 2e44 4159 290d 0a0d 0a6d 6574  ency.DAY)....met
-00000e10: 612c 2067 656e 203d 2064 2e67 6574 2829  a, gen = d.get()
-00000e20: 0d0a 0d0a 666f 7220 6163 7469 6f6e 2c20  ....for action, 
-00000e30: 656c 656d 656e 7420 696e 2067 656e 3a0d  element in gen:.
-00000e40: 0a20 2020 2069 6620 656c 656d 656e 742e  .    if element.
-00000e50: 7461 6773 2e67 6574 2822 7368 6f70 2229  tags.get("shop")
-00000e60: 203d 3d20 2263 6f6e 7665 6e69 656e 6365   == "convenience
-00000e70: 223a 0d0a 2020 2020 2020 2020 7072 696e  ":..        prin
-00000e80: 7428 656c 656d 656e 7429 0d0a 6060 600d  t(element)..```.
-00000e90: 0a60 6060 7079 0d0a 6672 6f6d 206f 736d  .```py..from osm
-00000ea0: 5f65 6173 795f 6170 6920 696d 706f 7274  _easy_api import
-00000eb0: 2044 6966 662c 2046 7265 7175 656e 6379   Diff, Frequency
-00000ec0: 2c20 5461 6773 0d0a 0d0a 6420 3d20 4469  , Tags....d = Di
-00000ed0: 6666 2846 7265 7175 656e 6379 2e44 4159  ff(Frequency.DAY
-00000ee0: 290d 0a0d 0a6d 6574 612c 2067 656e 203d  )....meta, gen =
-00000ef0: 2064 2e67 6574 2874 6167 733d 5461 6773   d.get(tags=Tags
-00000f00: 287b 2273 686f 7022 3a20 2263 6f6e 7665  ({"shop": "conve
-00000f10: 6e69 656e 6365 227d 2929 0d0a 0d0a 666f  nience"}))....fo
-00000f20: 7220 6163 7469 6f6e 2c20 656c 656d 656e  r action, elemen
-00000f30: 7420 696e 2067 656e 3a0d 0a20 2020 2020  t in gen:..     
-00000f40: 2020 2070 7269 6e74 2865 6c65 6d65 6e74     print(element
-00000f50: 290d 0a60 6060 0d0a 6275 7420 7468 6520  )..```..but the 
-00000f60: 7365 636f 6e64 2073 6565 6d73 2074 6f20  second seems to 
-00000f70: 6265 2066 6173 7465 722e 0d0a 0d0a 416c  be faster.....Al
-00000f80: 736f 2079 6f75 2063 616e 2075 7365 204f  so you can use O
-00000f90: 736d 4368 616e 6765 206f 626a 6563 7420  smChange object 
-00000fa0: 6966 2079 6f75 2064 6f6e 2774 2077 616e  if you don't wan
-00000fb0: 7420 746f 2075 7365 2067 656e 6572 6174  t to use generat
-00000fc0: 6f72 0d0a 6060 6070 790d 0a66 726f 6d20  or..```py..from 
-00000fd0: 6f73 6d5f 6561 7379 5f61 7069 2069 6d70  osm_easy_api imp
-00000fe0: 6f72 7420 4469 6666 2c20 4672 6571 7565  ort Diff, Freque
-00000ff0: 6e63 792c 2041 6374 696f 6e2c 204e 6f64  ncy, Action, Nod
-00001000: 650d 0a0d 0a64 203d 2044 6966 6628 4672  e....d = Diff(Fr
-00001010: 6571 7565 6e63 792e 4d49 4e55 5445 290d  equency.MINUTE).
-00001020: 0a0d 0a6f 736d 4368 616e 6765 203d 2064  ...osmChange = d
-00001030: 2e67 6574 2867 656e 6572 6174 6f72 3d46  .get(generator=F
-00001040: 616c 7365 290d 0a0d 0a64 656c 6574 6564  alse)....deleted
-00001050: 5f6e 6f64 6573 203d 206f 736d 4368 616e  _nodes = osmChan
-00001060: 6765 2e67 6574 284e 6f64 652c 2041 6374  ge.get(Node, Act
-00001070: 696f 6e2e 4445 4c45 5445 290d 0a66 6f72  ion.DELETE)..for
-00001080: 206e 6f64 6520 696e 2064 656c 6574 6564   node in deleted
-00001090: 5f6e 6f64 6573 3a0d 0a20 2020 2070 7269  _nodes:..    pri
-000010a0: 6e74 286e 6f64 652e 6964 290d 0a60 6060  nt(node.id)..```
-000010b0: 0d0a 6275 7420 6974 2063 616e 2063 6f6e  ..but it can con
-000010c0: 7375 6d65 206c 6172 6765 2061 6d6f 756e  sume large amoun
-000010d0: 7473 206f 6620 7261 6d20 616e 6420 7573  ts of ram and us
-000010e0: 6520 6f66 2074 6869 7320 6d65 7468 6f64  e of this method
-000010f0: 2069 7320 6e6f 7420 7265 636f 6d6d 656e   is not recommen
-00001100: 6465 6420 666f 7220 6c61 7267 6520 6469  ded for large di
-00001110: 6666 2773 2e0d 0a0d 0a23 2054 6573 7473  ff's.....# Tests
-00001120: 0d0a 0d0a 596f 7520 7769 6c6c 206e 6565  ....You will nee
-00001130: 6420 746f 2069 6e73 7461 6c6c 2060 7465  d to install `te
-00001140: 7374 2d72 6571 7569 7265 6d65 6e74 732e  st-requirements.
-00001150: 7478 7460 2e20 596f 7520 6361 6e20 7573  txt`. You can us
-00001160: 6520 746f 782e 0d0a 546f 2072 756e 2074  e tox...To run t
-00001170: 6573 7473 206d 616e 7561 6c6c 7920 7573  ests manually us
-00001180: 6520 6070 7974 686f 6e20 2d6d 2075 6e69  e `python -m uni
-00001190: 7474 6573 7420 6469 7363 6f76 6572 602e  ttest discover`.
-000011a0: 0d0a                                     ..
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e6f 736d 5f65 6173 795f 6170 693c  r">osm_easy_api<
+00000020: 2f68 313e 0d0a 3c70 2061 6c69 676e 3d22  /h1>..<p align="
+00000030: 6365 6e74 6572 223e 0d0a 2020 3c69 6d67  center">..  <img
+00000040: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000050: 7468 7562 2e63 6f6d 2f64 6f63 656e 7459  thub.com/docentY
+00000060: 542f 6175 746f 6d61 7465 642d 7079 7468  T/automated-pyth
+00000070: 6f6e 2d74 6573 7473 2d74 6573 7469 6e67  on-tests-testing
+00000080: 2d72 6570 6f2f 6163 7469 6f6e 732f 776f  -repo/actions/wo
+00000090: 726b 666c 6f77 732f 7465 7374 732e 7961  rkflows/tests.ya
+000000a0: 6d6c 2f62 6164 6765 2e73 7667 2220 2f3e  ml/badge.svg" />
+000000b0: 0d0a 2020 3c69 6d67 2073 7263 3d22 6874  ..  <img src="ht
+000000c0: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
+000000d0: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
+000000e0: 646f 6365 6e74 5954 2f6f 736d 5f65 6173  docentYT/osm_eas
+000000f0: 795f 6170 692f 3338 3839 6165 3632 3662  y_api/3889ae626b
+00000100: 6533 3531 3833 3235 3334 3835 3634 3662  e35183253485646b
+00000110: 3762 6539 6532 3335 6132 6663 3237 2f63  7be9e235a2fc27/c
+00000120: 6f76 6572 6167 652d 6261 6467 652e 7376  overage-badge.sv
+00000130: 6722 202f 3e0d 0a20 203c 6120 6872 6566  g" />..  <a href
+00000140: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000150: 7267 2f70 726f 6a65 6374 2f6f 736d 2d65  rg/project/osm-e
+00000160: 6173 792d 6170 692f 223e 0d0a 2020 2020  asy-api/">..    
+00000170: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000180: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000190: 2f70 7970 692f 762f 6f73 6d5f 6561 7379  /pypi/v/osm_easy
+000001a0: 5f61 7069 2220 2f3e 0d0a 2020 3c2f 613e  _api" />..  </a>
+000001b0: 0d0a 2020 3c61 2068 7265 663d 2268 7474  ..  <a href="htt
+000001c0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000001d0: 6f6a 6563 742f 6f73 6d2d 6561 7379 2d61  oject/osm-easy-a
+000001e0: 7069 2f22 3e0d 0a20 2020 203c 696d 6720  pi/">..    <img 
+000001f0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000200: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000210: 2f64 6d2f 6f73 6d5f 6561 7379 5f61 7069  /dm/osm_easy_api
+00000220: 2220 616c 743d 2270 7970 6920 646f 776e  " alt="pypi down
+00000230: 6c6f 6164 7322 3e0d 0a20 203c 2f61 3e0d  loads">..  </a>.
+00000240: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000250: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000260: 6a65 6374 2f6f 736d 2d65 6173 792d 6170  ject/osm-easy-ap
+00000270: 692f 223e 0d0a 2020 2020 3c69 6d67 2061  i/">..    <img a
+00000280: 6c74 3d22 7079 7468 6f6e 2076 6572 7369  lt="python versi
+00000290: 6f6e 7322 2073 7263 3d22 6874 7470 733a  ons" src="https:
+000002a0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000002b0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000002c0: 2f6f 736d 5f65 6173 795f 6170 6922 2074  /osm_easy_api" t
+000002d0: 6172 6765 743d 225f 626c 616e 6b22 202f  arget="_blank" /
+000002e0: 3e0d 0a20 203c 2f61 3e0d 0a3c 2f70 3e0d  >..  </a>..</p>.
+000002f0: 0a0d 0a3c 7020 616c 6967 6e3d 2263 656e  ...<p align="cen
+00000300: 7465 7222 3e3c 6120 6872 6566 3d22 6874  ter"><a href="ht
+00000310: 7470 733a 2f2f 7777 772e 6f70 656e 7374  tps://www.openst
+00000320: 7265 6574 6d61 702e 6f72 672f 7573 6572  reetmap.org/user
+00000330: 2f6b 7769 6174 656b 5f31 3233 2922 3e4d  /kwiatek_123)">M
+00000340: 6520 6f6e 204f 7065 6e53 7472 6565 744d  e on OpenStreetM
+00000350: 6170 3c2f 613e 3c2f 703e 0d0a 0d0a 5079  ap</a></p>....Py
+00000360: 7468 6f6e 2070 6163 6b61 6765 2066 6f72  thon package for
+00000370: 2070 6172 7369 6e67 206f 736d 2064 6966   parsing osm dif
+00000380: 6673 2061 6e64 2063 6f6d 6d75 6e69 6361  fs and communica
+00000390: 7469 6e67 2077 6974 6820 7468 6520 4f70  ting with the Op
+000003a0: 656e 5374 7265 6574 4d61 7020 6170 692e  enStreetMap api.
+000003b0: 2053 6565 2041 5049 2e74 7874 2066 6f72   See API.txt for
+000003c0: 206c 6973 7420 6f66 2073 7570 706f 7274   list of support
+000003d0: 6564 2065 6e64 706f 696e 7473 2e0d 0a0d  ed endpoints....
+000003e0: 0a23 2320 5768 6174 2773 2074 6865 2070  .## What's the p
+000003f0: 6f69 6e74 206f 6620 7468 6973 2070 6163  oint of this pac
+00000400: 6b61 6765 3f0d 0a0d 0a54 6869 7320 7061  kage?....This pa
+00000410: 636b 6167 6520 7761 7320 6372 6561 7465  ckage was create
+00000420: 6420 746f 2070 726f 7669 6465 2061 6e20  d to provide an 
+00000430: 6561 7379 2077 6179 2074 6f20 6372 6561  easy way to crea
+00000440: 7465 2061 7574 6f6d 6174 6564 2073 6372  te automated scr
+00000450: 6970 7473 2061 6e64 2070 726f 6772 616d  ipts and program
+00000460: 7320 7468 6174 2075 7365 2064 6966 6620  s that use diff 
+00000470: 616e 642f 6f72 206f 736d 2061 7069 2e20  and/or osm api. 
+00000480: 5468 6520 6d61 696e 2061 6476 616e 7461  The main advanta
+00000490: 6765 2069 7320 7468 6520 636c 6173 7365  ge is the classe
+000004a0: 7320 2864 6174 615f 636c 6173 7365 7329  s (data_classes)
+000004b0: 2074 6861 7420 7072 6f76 6964 6520 6461   that provide da
+000004c0: 7461 206f 6620 656c 656d 656e 7473 2028  ta of elements (
+000004d0: 6e6f 6465 2c20 7761 792c 2072 656c 6174  node, way, relat
+000004e0: 696f 6e2c 204f 736d 4368 616e 6765 2c20  ion, OsmChange, 
+000004f0: 6574 632e 2920 696e 2061 2072 6561 6461  etc.) in a reada
+00000500: 626c 6520 7761 7920 616e 6420 7468 6520  ble way and the 
+00000510: 706f 7373 6962 696c 6974 7920 746f 2075  possibility to u
+00000520: 7365 2074 6865 6d20 696e 2064 6966 6620  se them in diff 
+00000530: 616e 6420 6170 6920 7769 7468 6f75 7420  and api without 
+00000540: 776f 7272 7969 6e67 2061 626f 7574 206d  worrying about m
+00000550: 6973 7369 6e67 2064 6174 6120 6f72 2064  issing data or d
+00000560: 6963 7469 6f6e 6172 6965 732e 2059 6f75  ictionaries. You
+00000570: 2063 616e 2065 6173 696c 7920 6669 6e64   can easily find
+00000580: 206e 6f64 6573 2069 6e20 6469 6666 2c20   nodes in diff, 
+00000590: 6164 6420 6120 7461 6720 746f 2074 6865  add a tag to the
+000005a0: 6d20 616e 6420 7365 6e64 2074 6865 2063  m and send the c
+000005b0: 6f72 7265 6374 6564 2076 6572 7369 6f6e  orrected version
+000005c0: 2074 6f20 6f73 6d2e 0d0a 0d0a 2323 2057   to osm.....## W
+000005d0: 6861 7420 6e65 7874 3f0d 0a54 6865 2070  hat next?..The p
+000005e0: 6c61 6e20 6973 2074 6f20 6f70 7469 6d69  lan is to optimi
+000005f0: 7365 2061 6e64 2069 6d70 726f 7665 2074  se and improve t
+00000600: 6865 2063 6f64 652c 2061 6464 2073 7570  he code, add sup
+00000610: 706f 7274 2066 6f72 2067 7078 2074 7261  port for gpx tra
+00000620: 6365 732c 2072 7373 2073 7570 706f 7274  ces, rss support
+00000630: 2061 6e64 206f 7665 7270 6173 7320 6170   and overpass ap
+00000640: 692e 0d0a 0d0a 2320 496e 7374 616c 6c61  i.....# Installa
+00000650: 7469 6f6e 0d0a 0d0a 576f 726b 7320 6f6e  tion....Works on
+00000660: 2070 7974 686f 6e20 3e3d 2033 2e31 302e   python >= 3.10.
+00000670: 2028 4475 6520 746f 206e 6577 2074 7970   (Due to new typ
+00000680: 6568 696e 7473 2073 7461 6e64 6172 6429  ehints standard)
+00000690: 0d0a 0d0a 496e 7374 616c 6c20 606f 736d  ....Install `osm
+000006a0: 5f65 6173 795f 6170 6960 2066 726f 6d20  _easy_api` from 
+000006b0: 5b50 7950 695d 2868 7474 7073 3a2f 2f70  [PyPi](https://p
+000006c0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000006d0: 6f73 6d2d 6561 7379 2d61 7069 2f29 3a0d  osm-easy-api/):.
+000006e0: 0a60 6060 0d0a 7069 7020 696e 7374 616c  .```..pip instal
+000006f0: 6c20 6f73 6d5f 6561 7379 5f61 7069 0d0a  l osm_easy_api..
+00000700: 6060 6020 0d0a 0d0a 2320 446f 6375 6d65  ``` ....# Docume
+00000710: 6e74 6174 696f 6e0d 0a0d 0a59 6f75 2063  ntation....You c
+00000720: 616e 2076 6965 7720 646f 6375 6d65 6e74  an view document
+00000730: 6174 696f 6e20 6f6e 205b 6769 7468 7562  ation on [github
+00000740: 2d70 6167 6573 5d28 6874 7470 733a 2f2f  -pages](https://
+00000750: 646f 6365 6e74 7974 2e67 6974 6875 622e  docentyt.github.
+00000760: 696f 2f6f 736d 5f65 6173 795f 6170 692f  io/osm_easy_api/
+00000770: 6f73 6d5f 6561 7379 5f61 7069 2e68 746d  osm_easy_api.htm
+00000780: 6c29 2e0d 0a0d 0a44 6f63 756d 656e 7461  l).....Documenta
+00000790: 7469 6f6e 2069 7320 6275 696c 6420 7573  tion is build us
+000007a0: 696e 6720 5b70 646f 635d 2868 7474 7073  ing [pdoc](https
+000007b0: 3a2f 2f70 646f 632e 6465 7629 2e0d 0a54  ://pdoc.dev)...T
+000007c0: 6f20 7275 6e20 646f 6373 206f 6e20 796f  o run docs on yo
+000007d0: 7572 206d 6163 6869 6e65 2075 7365 2070  ur machine use p
+000007e0: 7265 6665 7272 6564 2063 6f6d 6d61 6e64  referred command
+000007f0: 3a20 6070 646f 6320 2d2d 646f 6366 6f72  : `pdoc --docfor
+00000800: 6d61 7420 676f 6f67 6c65 202d 2d6e 6f2d  mat google --no-
+00000810: 7368 6f77 2d73 6f75 7263 6520 6f73 6d5f  show-source osm_
+00000820: 6561 7379 5f61 7069 2021 6f73 6d5f 6561  easy_api !osm_ea
+00000830: 7379 5f61 7069 2e75 7469 6c73 602e 0d0a  sy_api.utils`...
+00000840: 0d0a 2320 4578 616d 706c 6573 0d0a 0d0a  ..# Examples....
+00000850: 2323 2044 4946 460d 0a0d 0a23 2323 2050  ## DIFF....### P
+00000860: 7269 6e74 2074 7265 6573 0d0a 0d0a 6060  rint trees....``
+00000870: 6070 790d 0a66 726f 6d20 6f73 6d5f 6561  `py..from osm_ea
+00000880: 7379 5f61 7069 2069 6d70 6f72 7420 4e6f  sy_api import No
+00000890: 6465 2c20 4469 6666 2c20 4672 6571 7565  de, Diff, Freque
+000008a0: 6e63 790d 0a0d 0a23 2044 6f77 6e6c 6f61  ncy....# Downloa
+000008b0: 6420 6469 6666 2066 726f 6d20 6c61 7374  d diff from last
+000008c0: 2068 6f75 722e 0d0a 6420 3d20 4469 6666   hour...d = Diff
+000008d0: 2846 7265 7175 656e 6379 2e48 4f55 5229  (Frequency.HOUR)
+000008e0: 0d0a 0d0a 2320 4765 7420 4d65 7461 206e  ....# Get Meta n
+000008f0: 616d 6564 7475 706c 6520 666f 7220 6469  amedtuple for di
+00000900: 6666 206d 6574 6164 6174 6120 616e 6420  ff metadata and 
+00000910: 6765 6e65 7261 746f 7220 7468 6174 2070  generator that p
+00000920: 6172 7365 2064 6966 6620 6669 6c65 2e0d  arse diff file..
+00000930: 0a6d 6574 612c 2067 656e 203d 2064 2e67  .meta, gen = d.g
+00000940: 6574 2874 6167 733d 226e 6174 7572 616c  et(tags="natural
+00000950: 2229 0d0a 0d0a 2320 5072 696e 7420 616c  ")....# Print al
+00000960: 6c20 6372 6561 7465 642c 206d 6f64 6966  l created, modif
+00000970: 6965 6420 616e 6420 6465 6c65 7465 6420  ied and deleted 
+00000980: 4e6f 6465 7320 7769 7468 206e 6174 7572  Nodes with natur
+00000990: 616c 3d74 7265 6520 7461 672e 0d0a 666f  al=tree tag...fo
+000009a0: 7220 6163 7469 6f6e 2c20 656c 656d 656e  r action, elemen
+000009b0: 7420 696e 2067 656e 3a0d 0a20 2020 2069  t in gen:..    i
+000009c0: 6620 7479 7065 2865 6c65 6d65 6e74 2920  f type(element) 
+000009d0: 3d3d 204e 6f64 6520 616e 6420 656c 656d  == Node and elem
+000009e0: 656e 742e 7461 6773 2e67 6574 2822 6e61  ent.tags.get("na
+000009f0: 7475 7261 6c22 2920 3d3d 2022 7472 6565  tural") == "tree
+00000a00: 223a 0d0a 2020 2020 2020 2020 7072 696e  ":..        prin
+00000a10: 7428 6163 7469 6f6e 2c20 656c 656d 656e  t(action, elemen
+00000a20: 742e 6964 290d 0a60 6060 0d0a 0d0a 2323  t.id)..```....##
+00000a30: 2320 5072 696e 7420 696e 636f 7272 6563  # Print incorrec
+00000a40: 746c 7920 7461 6767 6564 2073 696e 676c  tly tagged singl
+00000a50: 6520 7472 6573 730d 0a0d 0a60 6060 7079  e tress....```py
+00000a60: 0d0a 6672 6f6d 206f 736d 5f65 6173 795f  ..from osm_easy_
+00000a70: 6170 6920 696d 706f 7274 2044 6966 662c  api import Diff,
+00000a80: 2046 7265 7175 656e 6379 2c20 4163 7469   Frequency, Acti
+00000a90: 6f6e 2c20 4e6f 6465 0d0a 0d0a 6420 3d20  on, Node....d = 
+00000aa0: 4469 6666 2846 7265 7175 656e 6379 2e44  Diff(Frequency.D
+00000ab0: 4159 290d 0a0d 0a6d 6574 612c 2067 656e  AY)....meta, gen
+00000ac0: 203d 2064 2e67 6574 2874 6167 733d 226e   = d.get(tags="n
+00000ad0: 6174 7572 616c 2229 0d0a 0d0a 666f 7220  atural")....for 
+00000ae0: 6163 7469 6f6e 2c20 656c 656d 656e 7420  action, element 
+00000af0: 696e 2067 656e 3a0d 0a20 2020 2069 6620  in gen:..    if 
+00000b00: 7479 7065 2865 6c65 6d65 6e74 2920 3d3d  type(element) ==
+00000b10: 204e 6f64 653a 0d0a 2020 2020 2020 2020   Node:..        
+00000b20: 6966 2061 6374 696f 6e20 3d3d 2041 6374  if action == Act
+00000b30: 696f 6e2e 4352 4541 5445 206f 7220 6163  ion.CREATE or ac
+00000b40: 7469 6f6e 203d 3d20 4163 7469 6f6e 2e4d  tion == Action.M
+00000b50: 4f44 4946 593a 0d0a 2020 2020 2020 2020  ODIFY:..        
+00000b60: 2020 2020 6966 2065 6c65 6d65 6e74 2e74      if element.t
+00000b70: 6167 732e 6765 7428 226e 6174 7572 616c  ags.get("natural
+00000b80: 2229 203d 3d20 2277 6f6f 6422 3a0d 0a20  ") == "wood":.. 
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00000ba0: 7269 6e74 2865 6c65 6d65 6e74 290d 0a60  rint(element)..`
+00000bb0: 6060 0d0a 4578 616d 706c 6520 6f75 7470  ``..Example outp
+00000bc0: 7574 3a0d 0a60 6060 0d0a 4e6f 6465 2869  ut:..```..Node(i
+00000bd0: 6420 3d20 3130 3230 3834 3836 3731 372c  d = 10208486717,
+00000be0: 2076 6973 6962 6c65 203d 204e 6f6e 652c   visible = None,
+00000bf0: 2076 6572 7369 6f6e 203d 2031 2c20 6368   version = 1, ch
+00000c00: 616e 6765 7365 745f 6964 203d 2031 3239  angeset_id = 129
+00000c10: 3231 3630 3735 2c20 7469 6d65 7374 616d  216075, timestam
+00000c20: 7020 3d20 3230 3232 2d31 312d 3232 5430  p = 2022-11-22T0
+00000c30: 303a 3136 3a34 345a 2c20 7573 6572 5f69  0:16:44Z, user_i
+00000c40: 6420 3d20 3137 3437 3137 3231 2c20 7461  d = 17471721, ta
+00000c50: 6773 203d 207b 276c 6561 665f 7479 7065  gs = {'leaf_type
+00000c60: 273a 2027 6272 6f61 646c 6561 7665 6427  ': 'broadleaved'
+00000c70: 2c20 276e 6174 7572 616c 273a 2027 776f  , 'natural': 'wo
+00000c80: 6f64 277d 2c20 6c61 7469 7475 6465 203d  od'}, latitude =
+00000c90: 2034 382e 3635 3232 3238 362c 206c 6f6e   48.6522286, lon
+00000ca0: 6769 7475 6465 203d 2031 322e 3538 3338  gitude = 12.5838
+00000cb0: 3039 2c20 290d 0a60 6060 0d0a 0d0a 2323  09, )..```....##
+00000cc0: 2041 5049 0d0a 0d0a 2323 2320 4164 6420   API....### Add 
+00000cd0: 6d69 7373 696e 6720 7769 6b69 6461 7461  missing wikidata
+00000ce0: 2074 6167 0d0a 0d0a 6060 6070 790d 0a66   tag....```py..f
+00000cf0: 726f 6d20 6f73 6d5f 6561 7379 5f61 7069  rom osm_easy_api
+00000d00: 2069 6d70 6f72 7420 4170 692c 204e 6f64   import Api, Nod
+00000d10: 652c 2054 6167 730d 0a0d 0a61 7069 203d  e, Tags....api =
+00000d20: 2041 7069 2822 6874 7470 733a 2f2f 6d61   Api("https://ma
+00000d30: 7374 6572 2e61 7069 732e 6465 762e 6f70  ster.apis.dev.op
+00000d40: 656e 7374 7265 6574 6d61 702e 6f72 6722  enstreetmap.org"
+00000d50: 2c20 4c4f 4749 4e2c 2050 4153 5357 4f52  , LOGIN, PASSWOR
+00000d60: 4429 0d0a 0d0a 6e6f 6465 203d 2061 7069  D)....node = api
+00000d70: 2e65 6c65 6d65 6e74 732e 6765 7428 4e6f  .elements.get(No
+00000d80: 6465 2c20 3432 3936 3436 3033 3336 2920  de, 4296460336) 
+00000d90: 2320 5765 2061 7265 2067 6574 7469 6e67  # We are getting
+00000da0: 204e 6f64 6520 7769 7468 2069 6420 3432   Node with id 42
+00000db0: 3936 3436 3033 3336 2077 6865 7265 2077  96460336 where w
+00000dc0: 6520 7761 6e74 2074 6f20 6164 6420 6120  e want to add a 
+00000dd0: 6e65 7720 7461 6720 746f 0d0a 6e6f 6465  new tag to..node
+00000de0: 2e74 6167 732e 6164 6428 2277 696b 6964  .tags.add("wikid
+00000df0: 6174 6122 2c20 2251 6578 616d 706c 6522  ata", "Qexample"
+00000e00: 2920 2320 4164 6420 6120 6e65 7720 7461  ) # Add a new ta
+00000e10: 6720 746f 206e 6f64 652e 0d0a 0d0a 6d79  g to node.....my
+00000e20: 5f63 6861 6e67 6573 6574 203d 2061 7069  _changeset = api
+00000e30: 2e63 6861 6e67 6573 6574 2e63 7265 6174  .changeset.creat
+00000e40: 6528 2241 6464 206d 6973 7369 6e67 2077  e("Add missing w
+00000e50: 696b 6964 6174 6120 7461 6722 2c20 5461  ikidata tag", Ta
+00000e60: 6773 287b 2261 7574 6f6d 6174 6963 223a  gs({"automatic":
+00000e70: 2022 7965 7322 7d29 2920 2320 4372 6561   "yes"})) # Crea
+00000e80: 7465 206e 6577 2063 6861 6e67 6573 6574  te new changeset
+00000e90: 2077 6974 6820 6465 7363 7269 7074 696f   with descriptio
+00000ea0: 6e20 616e 6420 7461 670d 0a61 7069 2e65  n and tag..api.e
+00000eb0: 6c65 6d65 6e74 732e 7570 6461 7465 286e  lements.update(n
+00000ec0: 6f64 652c 206d 795f 6368 616e 6765 7365  ode, my_changese
+00000ed0: 7429 2023 2053 656e 6420 6e65 7720 7665  t) # Send new ve
+00000ee0: 7273 696f 6e20 6f66 2061 206e 6f64 6520  rsion of a node 
+00000ef0: 746f 206f 736d 0d0a 6170 692e 6368 616e  to osm..api.chan
+00000f00: 6765 7365 742e 636c 6f73 6528 6d79 5f63  geset.close(my_c
+00000f10: 6861 6e67 6573 6574 2920 2320 436c 6f73  hangeset) # Clos
+00000f20: 6520 6368 616e 6765 7365 742e 0d0a 6060  e changeset...``
+00000f30: 600d 0a0d 0a23 204e 6f74 6573 0d0a 0d0a  `....# Notes....
+00000f40: 4e6f 7465 2074 6861 7420 7468 6520 666f  Note that the fo
+00000f50: 6c6c 6f77 696e 6720 636f 6465 7320 646f  llowing codes do
+00000f60: 2074 6865 2073 616d 6520 7468 696e 670d   the same thing.
+00000f70: 0a60 6060 7079 0d0a 6672 6f6d 206f 736d  .```py..from osm
+00000f80: 5f65 6173 795f 6170 6920 696d 706f 7274  _easy_api import
+00000f90: 2044 6966 662c 2046 7265 7175 656e 6379   Diff, Frequency
+00000fa0: 0d0a 0d0a 6420 3d20 4469 6666 2846 7265  ....d = Diff(Fre
+00000fb0: 7175 656e 6379 2e44 4159 290d 0a0d 0a6d  quency.DAY)....m
+00000fc0: 6574 612c 2067 656e 203d 2064 2e67 6574  eta, gen = d.get
+00000fd0: 2829 0d0a 0d0a 666f 7220 6163 7469 6f6e  ()....for action
+00000fe0: 2c20 656c 656d 656e 7420 696e 2067 656e  , element in gen
+00000ff0: 3a0d 0a20 2020 2069 6620 656c 656d 656e  :..    if elemen
+00001000: 742e 7461 6773 2e67 6574 2822 7368 6f70  t.tags.get("shop
+00001010: 2229 203d 3d20 2263 6f6e 7665 6e69 656e  ") == "convenien
+00001020: 6365 223a 0d0a 2020 2020 2020 2020 7072  ce":..        pr
+00001030: 696e 7428 656c 656d 656e 7429 0d0a 6060  int(element)..``
+00001040: 600d 0a60 6060 7079 0d0a 6672 6f6d 206f  `..```py..from o
+00001050: 736d 5f65 6173 795f 6170 6920 696d 706f  sm_easy_api impo
+00001060: 7274 2044 6966 662c 2046 7265 7175 656e  rt Diff, Frequen
+00001070: 6379 2c20 5461 6773 0d0a 0d0a 6420 3d20  cy, Tags....d = 
+00001080: 4469 6666 2846 7265 7175 656e 6379 2e44  Diff(Frequency.D
+00001090: 4159 290d 0a0d 0a6d 6574 612c 2067 656e  AY)....meta, gen
+000010a0: 203d 2064 2e67 6574 2874 6167 733d 5461   = d.get(tags=Ta
+000010b0: 6773 287b 2273 686f 7022 3a20 2263 6f6e  gs({"shop": "con
+000010c0: 7665 6e69 656e 6365 227d 2929 0d0a 0d0a  venience"}))....
+000010d0: 666f 7220 6163 7469 6f6e 2c20 656c 656d  for action, elem
+000010e0: 656e 7420 696e 2067 656e 3a0d 0a20 2020  ent in gen:..   
+000010f0: 2020 2020 2070 7269 6e74 2865 6c65 6d65       print(eleme
+00001100: 6e74 290d 0a60 6060 0d0a 6275 7420 7468  nt)..```..but th
+00001110: 6520 7365 636f 6e64 2073 6565 6d73 2074  e second seems t
+00001120: 6f20 6265 2066 6173 7465 722e 0d0a 0d0a  o be faster.....
+00001130: 416c 736f 2079 6f75 2063 616e 2075 7365  Also you can use
+00001140: 204f 736d 4368 616e 6765 206f 626a 6563   OsmChange objec
+00001150: 7420 6966 2079 6f75 2064 6f6e 2774 2077  t if you don't w
+00001160: 616e 7420 746f 2075 7365 2067 656e 6572  ant to use gener
+00001170: 6174 6f72 0d0a 6060 6070 790d 0a66 726f  ator..```py..fro
+00001180: 6d20 6f73 6d5f 6561 7379 5f61 7069 2069  m osm_easy_api i
+00001190: 6d70 6f72 7420 4469 6666 2c20 4672 6571  mport Diff, Freq
+000011a0: 7565 6e63 792c 2041 6374 696f 6e2c 204e  uency, Action, N
+000011b0: 6f64 650d 0a0d 0a64 203d 2044 6966 6628  ode....d = Diff(
+000011c0: 4672 6571 7565 6e63 792e 4d49 4e55 5445  Frequency.MINUTE
+000011d0: 290d 0a0d 0a6f 736d 4368 616e 6765 203d  )....osmChange =
+000011e0: 2064 2e67 6574 2867 656e 6572 6174 6f72   d.get(generator
+000011f0: 3d46 616c 7365 290d 0a0d 0a64 656c 6574  =False)....delet
+00001200: 6564 5f6e 6f64 6573 203d 206f 736d 4368  ed_nodes = osmCh
+00001210: 616e 6765 2e67 6574 284e 6f64 652c 2041  ange.get(Node, A
+00001220: 6374 696f 6e2e 4445 4c45 5445 290d 0a66  ction.DELETE)..f
+00001230: 6f72 206e 6f64 6520 696e 2064 656c 6574  or node in delet
+00001240: 6564 5f6e 6f64 6573 3a0d 0a20 2020 2070  ed_nodes:..    p
+00001250: 7269 6e74 286e 6f64 652e 6964 290d 0a60  rint(node.id)..`
+00001260: 6060 0d0a 6275 7420 6974 2063 616e 2063  ``..but it can c
+00001270: 6f6e 7375 6d65 206c 6172 6765 2061 6d6f  onsume large amo
+00001280: 756e 7473 206f 6620 7261 6d20 616e 6420  unts of ram and 
+00001290: 7573 6520 6f66 2074 6869 7320 6d65 7468  use of this meth
+000012a0: 6f64 2069 7320 6e6f 7420 7265 636f 6d6d  od is not recomm
+000012b0: 656e 6465 6420 666f 7220 6c61 7267 6520  ended for large 
+000012c0: 6469 6666 2773 2e0d 0a0d 0a23 2054 6573  diff's.....# Tes
+000012d0: 7473 0d0a 0d0a 596f 7520 7769 6c6c 206e  ts....You will n
+000012e0: 6565 6420 746f 2069 6e73 7461 6c6c 2060  eed to install `
+000012f0: 7465 7374 2d72 6571 7569 7265 6d65 6e74  test-requirement
+00001300: 732e 7478 7460 2e20 596f 7520 6361 6e20  s.txt`. You can 
+00001310: 7573 6520 746f 782e 0d0a 546f 2072 756e  use tox...To run
+00001320: 2074 6573 7473 206d 616e 7561 6c6c 7920   tests manually 
+00001330: 7573 6520 6070 7974 686f 6e20 2d6d 2075  use `python -m u
+00001340: 6e69 7474 6573 7420 6469 7363 6f76 6572  nittest discover
+00001350: 602e                                     `.
```

### Comparing `osm_easy_api-0.4.2/setup.cfg` & `osm_easy_api-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/_URLs.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/api.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             url=join_url(self.outer._url.changeset["get"], param),
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
 
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         return self._xml_to_changeset(generator, include_discussion)[0] # type: ignore
 
     def get_query(self, left: float | None = None, bottom: float | None = None, right: float | None = None, top: float | None = None,
     user_id: str | None = None, display_name: str | None = None,
     time_one: str | None = None, time_two: str | None = None,
     open: bool = False, closed: bool = False,
@@ -165,15 +165,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
 
         match status_code:
             case 200: pass
             case 400: raise ValueError("Invalid arguments. See https://wiki.openstreetmap.org/wiki/API_v0.6#Query:_GET_/api/0.6/changesets for more info.")
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         return self._xml_to_changeset(generator) # type: ignore
     
     def update(self, id: int, comment: str | None = None, tags: Tags | None = None) -> Changeset:
         """Updates the changeset with new comment or tags or both.
 
         Args:
@@ -213,15 +213,15 @@
         response = self.outer._request(self.outer._RequestMethods.PUT,
             self.outer._url.changeset["update"].format(id=id), self.outer._Requirement.YES, body=xml_str, stream=True, auto_status_code_handling = False)
 
         match response.status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.text)
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
         response.raw.decode_content = True
         return self._xml_to_changeset(self.outer._raw_stream_parser(response.raw), True)[0]
 
     def close(self, id: int) -> None:
         """Close changeset by ID.
 
@@ -233,15 +233,15 @@
             exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor: The changeset was already closer or you are not the author.
         """
         response = self.outer._request(self.outer._RequestMethods.PUT, self.outer._url.changeset["close"].format(id = id), self.outer._Requirement.YES, auto_status_code_handling = False)
         match response.status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.text)
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
     def download(self, id: int) -> Generator[Tuple['Action', 'Node | Way | Relation'], None, None]:
         """Download changes made in changeset. Like in 'diff' module.
 
         Args:
             id (int): Changeset ID.
 
@@ -252,44 +252,45 @@
             Generator: Diff generator like in 'diff' module.
         """
         stream = self.outer._request(self.outer._RequestMethods.GET, self.outer._url.changeset["download"].format(id=id), self.outer._Requirement.NO, stream=True, auto_status_code_handling = False)
 
         match stream.status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {stream.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {stream.status_code}. Please report it on github." # pragma: no cover
         
         stream.raw.decode_content = True
         def generator() -> Generator[tuple['Action', 'Node | Way | Relation'], None, None]:   
             gen = OsmChange_parser_generator(stream.raw, None)
             next(gen) # for meta data
             for action, element in gen: # type: ignore
                 assert isinstance(action, Action), "ERROR::API::ENDPOINTS::CHANGESET::download action TYPE IS NOT EQUAL TO ACTION"
                 yield (action, element) # type: ignore (We checked if it is Action)
         return generator()
 
-    def upload(self, changeset_id: int, osmChange: OsmChange):
+    def upload(self, changeset_id: int, osmChange: OsmChange, make_osmChange_valid: bool = True, work_on_copy: bool = False):
         # TODO: Parse returned xml
         """Upload OsmChange to OSM. You must provide changeset ID for open changeset.
 
         Args:
             changeset_id (int): Open changeset ID.
             osmChange (OsmChange): OsmChange instance with changes you want to upload. Action cannot be empty!
+            make_osmChange_valid (bool): 
 
         Raises:
             exceptions.ErrorWhenParsingXML: Incorrect OsmChange object. Maybe missing elements attributes.
             exceptions.IdNotFoundError: No changeset with provided ID or can't find element with ID in OsmChange.
             exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor: Changeset already closed or you are not an author.
             ValueError: Unexpected but correct error.
         """
         response = self.outer._request(
             method=self.outer._RequestMethods.POST,
             url=self.outer._url.changeset["upload"].format(id=changeset_id),
             auth_requirement=self.outer._Requirement.YES,
-            body = osmChange._to_xml(changeset_id),
+            body = osmChange.to_xml(changeset_id, make_osmChange_valid, work_on_copy),
             auto_status_code_handling=False
         )
         match response.status_code:
             case 200: pass
             case 400: raise exceptions.ErrorWhenParsingXML(response.text)
             case 404: raise exceptions.IdNotFoundError(response.text)
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor()
```

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             exceptions.ChangesetNotClosed: Changeset must be closed to add comment.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["comment"].format(id=changeset_id, text=text), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 409: raise exceptions.ChangesetNotClosed()
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
     def subscribe(self, changeset_id: int) -> None:
         """Subscribe to the discussion to receive notifications for new comments.
 
         Args:
             changeset_id (int): Changeset id.
 
@@ -35,15 +35,15 @@
             exceptions.AlreadySubscribed: You are already subscribed to this changeset.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["subscribe"].format(id=changeset_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 409: raise exceptions.AlreadySubscribed()
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
     def unsubscribe(self, changeset_id: int) -> None:
         """Unsubscribe from discussion to stop receiving notifications.
 
         Args:
             changeset_id (int): Changeset id.
 
@@ -51,15 +51,15 @@
             exceptions.NotSubscribed: You are not subscribed to this changeset.
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["unsubscribe"].format(id=changeset_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 404: raise exceptions.NotSubscribed()
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
     def hide(self, comment_id: int) -> None:
         """Set visible flag on changeset comment to false. MODERATOR ONLY!
 
         Args:
             comment_id (int): Comment id.
 
@@ -69,15 +69,15 @@
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["hide"].format(comment_id=comment_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 403: raise exceptions.NotAModerator()
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
     def unhide(self, comment_id: int) -> None:
         """Set visible flag on changeset comment to true. MODERATOR ONLY!
 
         Args:
             comment_id (int): Comment id.
 
@@ -87,8 +87,8 @@
         """
         response = self.outer._request(self.outer._RequestMethods.POST, self.outer._url.changeset_discussion["unhide"].format(comment_id=comment_id), self.outer._Requirement.YES, auto_status_code_handling=False)
         
         match response.status_code:
             case 200: pass
             case 403: raise exceptions.NotAModerator()
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
```

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         response = self.outer._request(self.outer._RequestMethods.PUT, self.outer._url.elements["create"].format(element_type=element_name), self.outer._Requirement.YES, body=body, auto_status_code_handling=False)
 
         match response.status_code:
             case 200: pass
             case 400: raise ValueError(response.content)
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.content)
             case 412: raise ValueError(response.content)
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
         
         return int(response.text)
 
     def get(self, element: type[Node_Way_Relation], id: int) -> Node_Way_Relation :
         """""Get element by id
 
         Args:
@@ -66,15 +66,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 410: raise exceptions.ElementDeleted()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
         
         for event, elem in generator:
             if elem.tag in ("node", "way", "relation") and event == "start":
                 object = _element_to_osm_object(elem)
                 return object
             
         return object
@@ -102,15 +102,15 @@
 
         match response.status_code:
             case 200: pass
             case 400: raise ValueError(response.content)
             case 409: raise ValueError(response.content)
             case 404: raise exceptions.IdNotFoundError()
             case 412: raise exceptions.IdNotFoundError(response.content)
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
         return int(response.content)
     
     def delete(self, element: Node | Way | Relation, changeset_id: int) -> int:
         """Deletes element. 
 
         Args:
             element (Node | Way | Relation): Element object which you want to delete. Id is not sufficient.
@@ -134,15 +134,15 @@
         match response.status_code:
             case 200: pass
             case 400: raise ValueError(response.content)
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.ChangesetAlreadyClosedOrUserIsNotAnAuthor(response.content)
             case 410: raise exceptions.ElementDeleted()
             case 412: raise ValueError(response.content)
-            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
         return int(response.content)
     
     def history(self, element: type[Node_Way_Relation], id: int) -> list[Node_Way_Relation]:
         """Returns all old versions of element.
 
         Args:
             element (type[Node_Way_Relation]): Element type to search for.
@@ -160,15 +160,15 @@
             url=url,
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
         
         objects_list = []
         for event, elem in generator:
             if elem.tag == element_name and event == "start":
                 objects_list.append(_element_to_osm_object(elem))
             
         return objects_list
@@ -195,15 +195,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 403: raise exceptions.IdNotFoundError("This version of the element is not available (due to redaction)")
             case 404: raise exceptions.IdNotFoundError()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
         
         for event, elem in generator:
             if elem.tag in ("node", "way", "relation"):
                 object = _element_to_osm_object(elem)
                 return object
         assert False, "[ERROR::API::ENDPOINTS::ELEMENTS::version] Cannot create an element."
     
@@ -233,15 +233,15 @@
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 400: raise ValueError()
             case 404: raise exceptions.IdNotFoundError()
             case 414: raise ValueError("URL too long (too many ids)")
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
         
         objects_list = []
         for event, elem in generator:
             if elem.tag == element.__name__.lower() and event == "start":
                 objects_list.append(_element_to_osm_object(elem))
             
         return objects_list
@@ -313,15 +313,15 @@
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 410: raise exceptions.ElementDeleted()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
         
         nodes_dict: dict[int, Node] = {}
         ways_dict:  dict[int, Way]  = {}
         relations_dict: dict[int, Relation] = {}
         for event, elem in generator:
             if event == "start":
                 if elem.tag == "node":
```

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 auto_status_code_handling=False
             )
 
             match response.status_code:
                 case 200: pass
                 case 400: raise exceptions.LimitsExceeded("You are trying to download too much data.")
                 case 509: raise exceptions.LimitsExceeded("You have downloaded too much data. Please try again later. See https://wiki.openstreetmap.org/wiki/Developer_FAQ#I've_been_blocked_from_the_API_for_downloading_too_much._Now_what?")
-                case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github."
+                case _: assert False, f"Unexpected response status code {response.status_code}. Please report it on github." # pragma: no cover
 
             response.raw.decode_content = True
             def generator():
                 gen = OsmChange_parser_generator(response.raw, None)
                 next(gen) # for meta data
                 for action, element in gen: # type: ignore
                     yield element           # type: ignore
```

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             url=url,
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 400: raise ValueError("Limits exceeded")
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         return self._xml_to_note(generator)
     
     def create(self, latitude: str, longitude: str, text: str) -> Note:
         """Creates new note.
 
         Args:
@@ -151,15 +151,15 @@
             auth_requirement=self.outer._Requirement.YES,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.NoteAlreadyClosed()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         return self._xml_to_note(generator)[0]
     
     def close(self, id: int, text: str | None = None) -> Note:
         """Close a note as fixed.
 
         Args:
@@ -181,15 +181,15 @@
             auth_requirement=self.outer._Requirement.YES,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.NoteAlreadyClosed()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         return self._xml_to_note(generator)[0]
     
     def reopen(self, id: int, text: str | None = None) -> Note:
         """Close a note as fixed.
 
         Args:
@@ -212,15 +212,15 @@
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 404: raise exceptions.IdNotFoundError()
             case 409: raise exceptions.NoteAlreadyOpen()
             case 410: raise exceptions.ElementDeleted()
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         return self._xml_to_note(generator)[0]
     
     def search(self, text: str, limit: int = 100, closed_days: int = 7, user_id: int | None = None, from_date: str | None = None, to_date: str | None = None, sort: str = "updated_at", order: str = "newest") -> list[Note]:
         """Search for notes with initial text and comments.
 
         Args:
@@ -251,13 +251,13 @@
             url=url,
             auth_requirement=self.outer._Requirement.NO,
             auto_status_code_handling=False)
         
         match status_code:
             case 200: pass
             case 400: raise ValueError("Limits exceeded")
-            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github."
+            case _: assert False, f"Unexpected response status code {status_code}. Please report it on github." # pragma: no cover
 
         try:
             return self._xml_to_note(generator)
         except:
             return []
```

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-1.0.0/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/note.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/note.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/relation.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/relation.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/user.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/data_classes/way.py` & `osm_easy_api-1.0.0/src/osm_easy_api/data_classes/way.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/diff/diff.py` & `osm_easy_api-1.0.0/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-1.0.0/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-1.0.0/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 206f 736d  : 2.1..Name: osm
 00000020: 2d65 6173 792d 6170 690d 0a56 6572 7369  -easy-api..Versi
-00000030: 6f6e 3a20 302e 342e 320d 0a53 756d 6d61  on: 0.4.2..Summa
+00000030: 6f6e 3a20 312e 302e 300d 0a53 756d 6d61  on: 1.0.0..Summa
 00000040: 7279 3a20 5079 7468 6f6e 2070 6163 6b61  ry: Python packa
 00000050: 6765 2066 6f72 2070 6172 7369 6e67 206f  ge for parsing o
 00000060: 736d 2064 6966 6673 2061 6e64 2063 6f6d  sm diffs and com
 00000070: 6d75 6e69 6361 7469 6e67 2077 6974 6820  municating with 
 00000080: 7468 6520 6f73 6d20 6170 692e 0d0a 486f  the osm api...Ho
 00000090: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 000000a0: 2f67 6974 6875 622e 636f 6d2f 646f 6365  /github.com/doce
@@ -50,2725 +50,2775 @@
 00000310: 3a20 332e 3131 0d0a 5265 7175 6972 6573  : 3.11..Requires
 00000320: 2d50 7974 686f 6e3a 203e 3d33 2e31 300d  -Python: >=3.10.
 00000330: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
 00000340: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
 00000350: 6d61 726b 646f 776e 0d0a 5072 6f76 6964  markdown..Provid
 00000360: 6573 2d45 7874 7261 3a20 7465 7374 696e  es-Extra: testin
 00000370: 670d 0a4c 6963 656e 7365 2d46 696c 653a  g..License-File:
-00000380: 204c 4943 454e 5345 2e6d 640d 0a0d 0a23   LICENSE.md....#
-00000390: 206f 736d 5f65 6173 795f 6170 690d 0a0d   osm_easy_api...
-000003a0: 0a21 5b54 6573 7473 5d28 6874 7470 733a  .![Tests](https:
-000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
-000003c0: 656e 7459 542f 6175 746f 6d61 7465 642d  entYT/automated-
-000003d0: 7079 7468 6f6e 2d74 6573 7473 2d74 6573  python-tests-tes
-000003e0: 7469 6e67 2d72 6570 6f2f 6163 7469 6f6e  ting-repo/action
-000003f0: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000400: 732e 7961 6d6c 2f62 6164 6765 2e73 7667  s.yaml/badge.svg
-00000410: 290d 0a21 5b63 6f76 6572 6167 655d 2868  )..![coverage](h
-00000420: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00000430: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00000440: 2f64 6f63 656e 7459 542f 6f73 6d5f 6561  /docentYT/osm_ea
-00000450: 7379 5f61 7069 2f33 3838 3961 6536 3236  sy_api/3889ae626
-00000460: 6265 3335 3138 3332 3533 3438 3536 3436  be35183253485646
-00000470: 6237 6265 3965 3233 3561 3266 6332 372f  b7be9e235a2fc27/
-00000480: 636f 7665 7261 6765 2d62 6164 6765 2e73  coverage-badge.s
-00000490: 7667 290d 0a5b 215b 5079 5049 2076 6572  vg)..[![PyPI ver
-000004a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
-000004b0: 6467 652e 6675 7279 2e69 6f2f 7079 2f6f  dge.fury.io/py/o
-000004c0: 736d 5f65 6173 795f 6170 692e 7376 6729  sm_easy_api.svg)
-000004d0: 5d28 6874 7470 733a 2f2f 6261 6467 652e  ](https://badge.
-000004e0: 6675 7279 2e69 6f2f 7079 2f6f 736d 5f65  fury.io/py/osm_e
-000004f0: 6173 795f 6170 6929 0d0a 0d0a 5b4d 6520  asy_api)....[Me 
-00000500: 6f6e 206f 7065 6e73 7472 6565 746d 6170  on openstreetmap
-00000510: 5d28 6874 7470 733a 2f2f 7777 772e 6f70  ](https://www.op
-00000520: 656e 7374 7265 6574 6d61 702e 6f72 672f  enstreetmap.org/
-00000530: 7573 6572 2f6b 7769 6174 656b 5f31 3233  user/kwiatek_123
-00000540: 290d 0a0d 0a50 7974 686f 6e20 7061 636b  )....Python pack
-00000550: 6167 6520 666f 7220 7061 7273 696e 6720  age for parsing 
-00000560: 6f73 6d20 6469 6666 7320 616e 6420 636f  osm diffs and co
-00000570: 6d6d 756e 6963 6174 696e 6720 7769 7468  mmunicating with
-00000580: 2074 6865 206f 736d 2061 7069 2e20 5365   the osm api. Se
-00000590: 6520 4150 492e 7478 7420 666f 7220 6c69  e API.txt for li
-000005a0: 7374 206f 6620 7375 7070 6f72 7465 6420  st of supported 
-000005b0: 656e 6470 6f69 6e74 732e 0d0a 0d0a 2323  endpoints.....##
-000005c0: 2057 6861 7427 7320 7468 6520 706f 696e   What's the poin
-000005d0: 7420 6f66 2074 6869 7320 7061 636b 6167  t of this packag
-000005e0: 653f 0d0a 0d0a 5468 6973 2070 6163 6b61  e?....This packa
-000005f0: 6765 2077 6173 2063 7265 6174 6564 2074  ge was created t
-00000600: 6f20 7072 6f76 6964 6520 616e 2065 6173  o provide an eas
-00000610: 7920 7761 7920 746f 2063 7265 6174 6520  y way to create 
-00000620: 6175 746f 6d61 7465 6420 7363 7269 7074  automated script
-00000630: 7320 616e 6420 7072 6f67 7261 6d73 2074  s and programs t
-00000640: 6861 7420 7573 6520 6469 6666 2061 6e64  hat use diff and
-00000650: 2f6f 7220 6f73 6d20 6170 692e 2054 6865  /or osm api. The
-00000660: 206d 6169 6e20 6164 7661 6e74 6167 6520   main advantage 
-00000670: 6973 2074 6865 2063 6c61 7373 6573 2028  is the classes (
-00000680: 6461 7461 5f63 6c61 7373 6573 2920 7468  data_classes) th
-00000690: 6174 2070 726f 7669 6465 2064 6174 6120  at provide data 
-000006a0: 6f66 2065 6c65 6d65 6e74 7320 286e 6f64  of elements (nod
-000006b0: 652c 2077 6179 2c20 7265 6c61 7469 6f6e  e, way, relation
-000006c0: 2c20 4f73 6d43 6861 6e67 652c 2065 7463  , OsmChange, etc
-000006d0: 2e29 2069 6e20 6120 7265 6164 6162 6c65  .) in a readable
-000006e0: 2077 6179 2061 6e64 2074 6865 2070 6f73   way and the pos
-000006f0: 7369 6269 6c69 7479 2074 6f20 7573 6520  sibility to use 
-00000700: 7468 656d 2069 6e20 6469 6666 2061 6e64  them in diff and
-00000710: 2061 7069 2077 6974 686f 7574 2077 6f72   api without wor
-00000720: 7279 696e 6720 6162 6f75 7420 6d69 7373  rying about miss
-00000730: 696e 6720 6461 7461 206f 7220 6469 6374  ing data or dict
-00000740: 696f 6e61 7269 6573 2e20 596f 7520 6361  ionaries. You ca
-00000750: 6e20 6561 7369 6c79 2066 696e 6420 6e6f  n easily find no
-00000760: 6465 7320 696e 2064 6966 662c 2061 6464  des in diff, add
-00000770: 2061 2074 6167 2074 6f20 7468 656d 2061   a tag to them a
-00000780: 6e64 2073 656e 6420 7468 6520 636f 7272  nd send the corr
-00000790: 6563 7465 6420 7665 7273 696f 6e20 746f  ected version to
-000007a0: 206f 736d 2e0d 0a0d 0a23 2320 5768 6174   osm.....## What
-000007b0: 206e 6578 743f 0d0a 5468 6520 706c 616e   next?..The plan
-000007c0: 2069 7320 746f 206f 7074 696d 6973 6520   is to optimise 
-000007d0: 616e 6420 696d 7072 6f76 6520 7468 6520  and improve the 
-000007e0: 636f 6465 2c20 6164 6420 7375 7070 6f72  code, add suppor
-000007f0: 7420 666f 7220 6770 7820 7472 6163 6573  t for gpx traces
-00000800: 2c20 7273 7320 7375 7070 6f72 7420 616e  , rss support an
-00000810: 6420 6f76 6572 7061 7373 2061 7069 2e0d  d overpass api..
-00000820: 0a0d 0a23 2049 6e73 7461 6c6c 6174 696f  ...# Installatio
-00000830: 6e0d 0a0d 0a57 6f72 6b73 206f 6e20 7079  n....Works on py
-00000840: 7468 6f6e 203e 3d20 332e 3130 2e20 2844  thon >= 3.10. (D
-00000850: 7565 2074 6f20 6e65 7720 7479 7065 6869  ue to new typehi
-00000860: 6e74 7320 7374 616e 6461 7264 290d 0a0d  nts standard)...
-00000870: 0a49 6e73 7461 6c6c 2060 6f73 6d5f 6561  .Install `osm_ea
-00000880: 7379 5f61 7069 6020 6672 6f6d 205b 5079  sy_api` from [Py
-00000890: 5069 5d28 6874 7470 733a 2f2f 7079 7069  Pi](https://pypi
-000008a0: 2e6f 7267 2f70 726f 6a65 6374 2f6f 736d  .org/project/osm
-000008b0: 2d65 6173 792d 6170 692f 293a 0d0a 6060  -easy-api/):..``
-000008c0: 600d 0a70 6970 2069 6e73 7461 6c6c 206f  `..pip install o
-000008d0: 736d 5f65 6173 795f 6170 690d 0a60 6060  sm_easy_api..```
-000008e0: 200d 0a0d 0a23 2044 6f63 756d 656e 7461   ....# Documenta
-000008f0: 7469 6f6e 0d0a 0d0a 596f 7520 6361 6e20  tion....You can 
-00000900: 7669 6577 2064 6f63 756d 656e 7461 7469  view documentati
-00000910: 6f6e 206f 6e20 5b67 6974 6875 622d 7061  on on [github-pa
-00000920: 6765 735d 2868 7474 7073 3a2f 2f64 6f63  ges](https://doc
-00000930: 656e 7479 742e 6769 7468 7562 2e69 6f2f  entyt.github.io/
-00000940: 6f73 6d5f 6561 7379 5f61 7069 2f6f 736d  osm_easy_api/osm
-00000950: 5f65 6173 795f 6170 692e 6874 6d6c 292e  _easy_api.html).
-00000960: 0d0a 0d0a 446f 6375 6d65 6e74 6174 696f  ....Documentatio
-00000970: 6e20 6973 2062 7569 6c64 2075 7369 6e67  n is build using
-00000980: 205b 7064 6f63 5d28 6874 7470 733a 2f2f   [pdoc](https://
-00000990: 7064 6f63 2e64 6576 292e 0d0a 546f 2072  pdoc.dev)...To r
-000009a0: 756e 2064 6f63 7320 6f6e 2079 6f75 7220  un docs on your 
-000009b0: 6d61 6368 696e 6520 7573 6520 7072 6566  machine use pref
-000009c0: 6572 7265 6420 636f 6d6d 616e 643a 2060  erred command: `
-000009d0: 7064 6f63 202d 2d64 6f63 666f 726d 6174  pdoc --docformat
-000009e0: 2067 6f6f 676c 6520 2d2d 6e6f 2d73 686f   google --no-sho
-000009f0: 772d 736f 7572 6365 206f 736d 5f65 6173  w-source osm_eas
-00000a00: 795f 6170 6920 216f 736d 5f65 6173 795f  y_api !osm_easy_
-00000a10: 6170 692e 7574 696c 7360 2e0d 0a0d 0a23  api.utils`.....#
-00000a20: 2045 7861 6d70 6c65 730d 0a0d 0a23 2320   Examples....## 
-00000a30: 4449 4646 0d0a 0d0a 2323 2320 5072 696e  DIFF....### Prin
-00000a40: 7420 7472 6565 730d 0a0d 0a60 6060 7079  t trees....```py
-00000a50: 0d0a 6672 6f6d 206f 736d 5f65 6173 795f  ..from osm_easy_
-00000a60: 6170 6920 696d 706f 7274 204e 6f64 652c  api import Node,
-00000a70: 2044 6966 662c 2046 7265 7175 656e 6379   Diff, Frequency
-00000a80: 0d0a 0d0a 2320 446f 776e 6c6f 6164 2064  ....# Download d
-00000a90: 6966 6620 6672 6f6d 206c 6173 7420 686f  iff from last ho
-00000aa0: 7572 2e0d 0a64 203d 2044 6966 6628 4672  ur...d = Diff(Fr
-00000ab0: 6571 7565 6e63 792e 484f 5552 290d 0a0d  equency.HOUR)...
-00000ac0: 0a23 2047 6574 204d 6574 6120 6e61 6d65  .# Get Meta name
-00000ad0: 6474 7570 6c65 2066 6f72 2064 6966 6620  dtuple for diff 
-00000ae0: 6d65 7461 6461 7461 2061 6e64 2067 656e  metadata and gen
-00000af0: 6572 6174 6f72 2074 6861 7420 7061 7273  erator that pars
-00000b00: 6520 6469 6666 2066 696c 652e 0d0a 6d65  e diff file...me
-00000b10: 7461 2c20 6765 6e20 3d20 642e 6765 7428  ta, gen = d.get(
-00000b20: 7461 6773 3d22 6e61 7475 7261 6c22 290d  tags="natural").
-00000b30: 0a0d 0a23 2050 7269 6e74 2061 6c6c 2063  ...# Print all c
-00000b40: 7265 6174 6564 2c20 6d6f 6469 6669 6564  reated, modified
-00000b50: 2061 6e64 2064 656c 6574 6564 204e 6f64   and deleted Nod
-00000b60: 6573 2077 6974 6820 6e61 7475 7261 6c3d  es with natural=
-00000b70: 7472 6565 2074 6167 2e0d 0a66 6f72 2061  tree tag...for a
-00000b80: 6374 696f 6e2c 2065 6c65 6d65 6e74 2069  ction, element i
-00000b90: 6e20 6765 6e3a 0d0a 2020 2020 6966 2074  n gen:..    if t
-00000ba0: 7970 6528 656c 656d 656e 7429 203d 3d20  ype(element) == 
-00000bb0: 4e6f 6465 2061 6e64 2065 6c65 6d65 6e74  Node and element
-00000bc0: 2e74 6167 732e 6765 7428 226e 6174 7572  .tags.get("natur
-00000bd0: 616c 2229 203d 3d20 2274 7265 6522 3a0d  al") == "tree":.
-00000be0: 0a20 2020 2020 2020 2070 7269 6e74 2861  .        print(a
-00000bf0: 6374 696f 6e2c 2065 6c65 6d65 6e74 2e69  ction, element.i
-00000c00: 6429 0d0a 6060 600d 0a0d 0a23 2323 2050  d)..```....### P
-00000c10: 7269 6e74 2069 6e63 6f72 7265 6374 6c79  rint incorrectly
-00000c20: 2074 6167 6765 6420 7369 6e67 6c65 2074   tagged single t
-00000c30: 7265 7373 0d0a 0d0a 6060 6070 790d 0a66  ress....```py..f
-00000c40: 726f 6d20 6f73 6d5f 6561 7379 5f61 7069  rom osm_easy_api
-00000c50: 2069 6d70 6f72 7420 4469 6666 2c20 4672   import Diff, Fr
-00000c60: 6571 7565 6e63 792c 2041 6374 696f 6e2c  equency, Action,
-00000c70: 204e 6f64 650d 0a0d 0a64 203d 2044 6966   Node....d = Dif
-00000c80: 6628 4672 6571 7565 6e63 792e 4441 5929  f(Frequency.DAY)
-00000c90: 0d0a 0d0a 6d65 7461 2c20 6765 6e20 3d20  ....meta, gen = 
-00000ca0: 642e 6765 7428 7461 6773 3d22 6e61 7475  d.get(tags="natu
-00000cb0: 7261 6c22 290d 0a0d 0a66 6f72 2061 6374  ral")....for act
-00000cc0: 696f 6e2c 2065 6c65 6d65 6e74 2069 6e20  ion, element in 
-00000cd0: 6765 6e3a 0d0a 2020 2020 6966 2074 7970  gen:..    if typ
-00000ce0: 6528 656c 656d 656e 7429 203d 3d20 4e6f  e(element) == No
-00000cf0: 6465 3a0d 0a20 2020 2020 2020 2069 6620  de:..        if 
-00000d00: 6163 7469 6f6e 203d 3d20 4163 7469 6f6e  action == Action
-00000d10: 2e43 5245 4154 4520 6f72 2061 6374 696f  .CREATE or actio
-00000d20: 6e20 3d3d 2041 6374 696f 6e2e 4d4f 4449  n == Action.MODI
-00000d30: 4659 3a0d 0a20 2020 2020 2020 2020 2020  FY:..           
-00000d40: 2069 6620 656c 656d 656e 742e 7461 6773   if element.tags
-00000d50: 2e67 6574 2822 6e61 7475 7261 6c22 2920  .get("natural") 
-00000d60: 3d3d 2022 776f 6f64 223a 0d0a 2020 2020  == "wood":..    
-00000d70: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00000d80: 7428 656c 656d 656e 7429 0d0a 6060 600d  t(element)..```.
-00000d90: 0a45 7861 6d70 6c65 206f 7574 7075 743a  .Example output:
-00000da0: 0d0a 6060 600d 0a4e 6f64 6528 6964 203d  ..```..Node(id =
-00000db0: 2031 3032 3038 3438 3637 3137 2c20 7669   10208486717, vi
-00000dc0: 7369 626c 6520 3d20 4e6f 6e65 2c20 7665  sible = None, ve
-00000dd0: 7273 696f 6e20 3d20 312c 2063 6861 6e67  rsion = 1, chang
-00000de0: 6573 6574 5f69 6420 3d20 3132 3932 3136  eset_id = 129216
-00000df0: 3037 352c 2074 696d 6573 7461 6d70 203d  075, timestamp =
-00000e00: 2032 3032 322d 3131 2d32 3254 3030 3a31   2022-11-22T00:1
-00000e10: 363a 3434 5a2c 2075 7365 725f 6964 203d  6:44Z, user_id =
-00000e20: 2031 3734 3731 3732 312c 2074 6167 7320   17471721, tags 
-00000e30: 3d20 7b27 6c65 6166 5f74 7970 6527 3a20  = {'leaf_type': 
-00000e40: 2762 726f 6164 6c65 6176 6564 272c 2027  'broadleaved', '
-00000e50: 6e61 7475 7261 6c27 3a20 2777 6f6f 6427  natural': 'wood'
-00000e60: 7d2c 206c 6174 6974 7564 6520 3d20 3438  }, latitude = 48
-00000e70: 2e36 3532 3232 3836 2c20 6c6f 6e67 6974  .6522286, longit
-00000e80: 7564 6520 3d20 3132 2e35 3833 3830 392c  ude = 12.583809,
-00000e90: 2029 0d0a 6060 600d 0a0d 0a23 2320 4150   )..```....## AP
-00000ea0: 490d 0a0d 0a23 2323 2041 6464 206d 6973  I....### Add mis
-00000eb0: 7369 6e67 2077 696b 6964 6174 6120 7461  sing wikidata ta
-00000ec0: 670d 0a0d 0a60 6060 7079 0d0a 6672 6f6d  g....```py..from
-00000ed0: 206f 736d 5f65 6173 795f 6170 6920 696d   osm_easy_api im
-00000ee0: 706f 7274 2041 7069 2c20 4e6f 6465 2c20  port Api, Node, 
-00000ef0: 5461 6773 0d0a 0d0a 6170 6920 3d20 4170  Tags....api = Ap
-00000f00: 6928 2268 7474 7073 3a2f 2f6d 6173 7465  i("https://maste
-00000f10: 722e 6170 6973 2e64 6576 2e6f 7065 6e73  r.apis.dev.opens
-00000f20: 7472 6565 746d 6170 2e6f 7267 222c 204c  treetmap.org", L
-00000f30: 4f47 494e 2c20 5041 5353 574f 5244 290d  OGIN, PASSWORD).
-00000f40: 0a0d 0a6e 6f64 6520 3d20 6170 692e 656c  ...node = api.el
-00000f50: 656d 656e 7473 2e67 6574 284e 6f64 652c  ements.get(Node,
-00000f60: 2034 3239 3634 3630 3333 3629 2023 2057   4296460336) # W
-00000f70: 6520 6172 6520 6765 7474 696e 6720 4e6f  e are getting No
-00000f80: 6465 2077 6974 6820 6964 2034 3239 3634  de with id 42964
-00000f90: 3630 3333 3620 7768 6572 6520 7765 2077  60336 where we w
-00000fa0: 616e 7420 746f 2061 6464 2061 206e 6577  ant to add a new
-00000fb0: 2074 6167 2074 6f0d 0a6e 6f64 652e 7461   tag to..node.ta
-00000fc0: 6773 2e61 6464 2822 7769 6b69 6461 7461  gs.add("wikidata
-00000fd0: 222c 2022 5165 7861 6d70 6c65 2229 2023  ", "Qexample") #
-00000fe0: 2041 6464 2061 206e 6577 2074 6167 2074   Add a new tag t
-00000ff0: 6f20 6e6f 6465 2e0d 0a0d 0a6d 795f 6368  o node.....my_ch
-00001000: 616e 6765 7365 7420 3d20 6170 692e 6368  angeset = api.ch
-00001010: 616e 6765 7365 742e 6372 6561 7465 2822  angeset.create("
-00001020: 4164 6420 6d69 7373 696e 6720 7769 6b69  Add missing wiki
-00001030: 6461 7461 2074 6167 222c 2054 6167 7328  data tag", Tags(
-00001040: 7b22 6175 746f 6d61 7469 6322 3a20 2279  {"automatic": "y
-00001050: 6573 227d 2929 2023 2043 7265 6174 6520  es"})) # Create 
-00001060: 6e65 7720 6368 616e 6765 7365 7420 7769  new changeset wi
-00001070: 7468 2064 6573 6372 6970 7469 6f6e 2061  th description a
-00001080: 6e64 2074 6167 0d0a 6170 692e 656c 656d  nd tag..api.elem
-00001090: 656e 7473 2e75 7064 6174 6528 6e6f 6465  ents.update(node
-000010a0: 2c20 6d79 5f63 6861 6e67 6573 6574 2920  , my_changeset) 
-000010b0: 2320 5365 6e64 206e 6577 2076 6572 7369  # Send new versi
-000010c0: 6f6e 206f 6620 6120 6e6f 6465 2074 6f20  on of a node to 
-000010d0: 6f73 6d0d 0a61 7069 2e63 6861 6e67 6573  osm..api.changes
-000010e0: 6574 2e63 6c6f 7365 286d 795f 6368 616e  et.close(my_chan
-000010f0: 6765 7365 7429 2023 2043 6c6f 7365 2063  geset) # Close c
-00001100: 6861 6e67 6573 6574 2e0d 0a60 6060 0d0a  hangeset...```..
-00001110: 0d0a 2320 4e6f 7465 730d 0a0d 0a4e 6f74  ..# Notes....Not
-00001120: 6520 7468 6174 2074 6865 2066 6f6c 6c6f  e that the follo
-00001130: 7769 6e67 2063 6f64 6573 2064 6f20 7468  wing codes do th
-00001140: 6520 7361 6d65 2074 6869 6e67 0d0a 6060  e same thing..``
-00001150: 6070 790d 0a66 726f 6d20 6f73 6d5f 6561  `py..from osm_ea
-00001160: 7379 5f61 7069 2069 6d70 6f72 7420 4469  sy_api import Di
-00001170: 6666 2c20 4672 6571 7565 6e63 790d 0a0d  ff, Frequency...
-00001180: 0a64 203d 2044 6966 6628 4672 6571 7565  .d = Diff(Freque
-00001190: 6e63 792e 4441 5929 0d0a 0d0a 6d65 7461  ncy.DAY)....meta
-000011a0: 2c20 6765 6e20 3d20 642e 6765 7428 290d  , gen = d.get().
-000011b0: 0a0d 0a66 6f72 2061 6374 696f 6e2c 2065  ...for action, e
-000011c0: 6c65 6d65 6e74 2069 6e20 6765 6e3a 0d0a  lement in gen:..
-000011d0: 2020 2020 6966 2065 6c65 6d65 6e74 2e74      if element.t
-000011e0: 6167 732e 6765 7428 2273 686f 7022 2920  ags.get("shop") 
-000011f0: 3d3d 2022 636f 6e76 656e 6965 6e63 6522  == "convenience"
-00001200: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
-00001210: 2865 6c65 6d65 6e74 290d 0a60 6060 0d0a  (element)..```..
-00001220: 6060 6070 790d 0a66 726f 6d20 6f73 6d5f  ```py..from osm_
-00001230: 6561 7379 5f61 7069 2069 6d70 6f72 7420  easy_api import 
-00001240: 4469 6666 2c20 4672 6571 7565 6e63 792c  Diff, Frequency,
-00001250: 2054 6167 730d 0a0d 0a64 203d 2044 6966   Tags....d = Dif
-00001260: 6628 4672 6571 7565 6e63 792e 4441 5929  f(Frequency.DAY)
-00001270: 0d0a 0d0a 6d65 7461 2c20 6765 6e20 3d20  ....meta, gen = 
-00001280: 642e 6765 7428 7461 6773 3d54 6167 7328  d.get(tags=Tags(
-00001290: 7b22 7368 6f70 223a 2022 636f 6e76 656e  {"shop": "conven
-000012a0: 6965 6e63 6522 7d29 290d 0a0d 0a66 6f72  ience"}))....for
-000012b0: 2061 6374 696f 6e2c 2065 6c65 6d65 6e74   action, element
-000012c0: 2069 6e20 6765 6e3a 0d0a 2020 2020 2020   in gen:..      
-000012d0: 2020 7072 696e 7428 656c 656d 656e 7429    print(element)
-000012e0: 0d0a 6060 600d 0a62 7574 2074 6865 2073  ..```..but the s
-000012f0: 6563 6f6e 6420 7365 656d 7320 746f 2062  econd seems to b
-00001300: 6520 6661 7374 6572 2e0d 0a0d 0a41 6c73  e faster.....Als
-00001310: 6f20 796f 7520 6361 6e20 7573 6520 4f73  o you can use Os
-00001320: 6d43 6861 6e67 6520 6f62 6a65 6374 2069  mChange object i
-00001330: 6620 796f 7520 646f 6e27 7420 7761 6e74  f you don't want
-00001340: 2074 6f20 7573 6520 6765 6e65 7261 746f   to use generato
-00001350: 720d 0a60 6060 7079 0d0a 6672 6f6d 206f  r..```py..from o
-00001360: 736d 5f65 6173 795f 6170 6920 696d 706f  sm_easy_api impo
-00001370: 7274 2044 6966 662c 2046 7265 7175 656e  rt Diff, Frequen
-00001380: 6379 2c20 4163 7469 6f6e 2c20 4e6f 6465  cy, Action, Node
-00001390: 0d0a 0d0a 6420 3d20 4469 6666 2846 7265  ....d = Diff(Fre
-000013a0: 7175 656e 6379 2e4d 494e 5554 4529 0d0a  quency.MINUTE)..
-000013b0: 0d0a 6f73 6d43 6861 6e67 6520 3d20 642e  ..osmChange = d.
-000013c0: 6765 7428 6765 6e65 7261 746f 723d 4661  get(generator=Fa
-000013d0: 6c73 6529 0d0a 0d0a 6465 6c65 7465 645f  lse)....deleted_
-000013e0: 6e6f 6465 7320 3d20 6f73 6d43 6861 6e67  nodes = osmChang
-000013f0: 652e 6765 7428 4e6f 6465 2c20 4163 7469  e.get(Node, Acti
-00001400: 6f6e 2e44 454c 4554 4529 0d0a 666f 7220  on.DELETE)..for 
-00001410: 6e6f 6465 2069 6e20 6465 6c65 7465 645f  node in deleted_
-00001420: 6e6f 6465 733a 0d0a 2020 2020 7072 696e  nodes:..    prin
-00001430: 7428 6e6f 6465 2e69 6429 0d0a 6060 600d  t(node.id)..```.
-00001440: 0a62 7574 2069 7420 6361 6e20 636f 6e73  .but it can cons
-00001450: 756d 6520 6c61 7267 6520 616d 6f75 6e74  ume large amount
-00001460: 7320 6f66 2072 616d 2061 6e64 2075 7365  s of ram and use
-00001470: 206f 6620 7468 6973 206d 6574 686f 6420   of this method 
-00001480: 6973 206e 6f74 2072 6563 6f6d 6d65 6e64  is not recommend
-00001490: 6564 2066 6f72 206c 6172 6765 2064 6966  ed for large dif
-000014a0: 6627 732e 0d0a 0d0a 2320 5465 7374 730d  f's.....# Tests.
-000014b0: 0a0d 0a59 6f75 2077 696c 6c20 6e65 6564  ...You will need
-000014c0: 2074 6f20 696e 7374 616c 6c20 6074 6573   to install `tes
-000014d0: 742d 7265 7175 6972 656d 656e 7473 2e74  t-requirements.t
-000014e0: 7874 602e 2059 6f75 2063 616e 2075 7365  xt`. You can use
-000014f0: 2074 6f78 2e0d 0a54 6f20 7275 6e20 7465   tox...To run te
-00001500: 7374 7320 6d61 6e75 616c 6c79 2075 7365  sts manually use
-00001510: 2060 7079 7468 6f6e 202d 6d20 756e 6974   `python -m unit
-00001520: 7465 7374 2064 6973 636f 7665 7260 2e0d  test discover`..
-00001530: 0a0d 0a23 2043 6861 6e67 656c 6f67 0d0a  ...# Changelog..
-00001540: 0d0a 416c 6c20 6e6f 7461 626c 6520 6368  ..All notable ch
-00001550: 616e 6765 7320 746f 2074 6869 7320 7072  anges to this pr
-00001560: 6f6a 6563 7420 7769 6c6c 2062 6520 646f  oject will be do
-00001570: 6375 6d65 6e74 6564 2069 6e20 7468 6973  cumented in this
-00001580: 2066 696c 652e 0d0a 0d0a 5468 6520 666f   file.....The fo
-00001590: 726d 6174 2069 7320 6261 7365 6420 6f6e  rmat is based on
-000015a0: 205b 4b65 6570 2061 2043 6861 6e67 656c   [Keep a Changel
-000015b0: 6f67 5d28 6874 7470 733a 2f2f 6b65 6570  og](https://keep
-000015c0: 6163 6861 6e67 656c 6f67 2e63 6f6d 2f65  achangelog.com/e
-000015d0: 6e2f 312e 302e 302f 292c 0d0a 616e 6420  n/1.0.0/),..and 
-000015e0: 7468 6973 2070 726f 6a65 6374 2061 6468  this project adh
-000015f0: 6572 6573 2074 6f20 5b53 656d 616e 7469  eres to [Semanti
-00001600: 6320 5665 7273 696f 6e69 6e67 5d28 6874  c Versioning](ht
-00001610: 7470 733a 2f2f 7365 6d76 6572 2e6f 7267  tps://semver.org
-00001620: 2f73 7065 632f 7632 2e30 2e30 2e68 746d  /spec/v2.0.0.htm
-00001630: 6c29 2e0d 0a0d 0a23 2320 5b30 2e34 2e32  l).....## [0.4.2
-00001640: 5d0d 0a23 2323 2043 6861 6e67 6564 0d0a  ]..### Changed..
-00001650: 2d20 4f72 6465 7220 6f66 2065 6c65 6d65  - Order of eleme
-00001660: 6e74 7320 696e 2078 6d6c 2067 656e 6572  nts in xml gener
-00001670: 6174 6564 2062 7920 6057 6179 2e5f 746f  ated by `Way._to
-00001680: 5f78 6d6c 2829 602e 2046 6972 7374 2074  _xml()`. First t
-00001690: 6167 732c 2074 6865 6e20 6e6f 6465 732e  ags, then nodes.
-000016a0: 0d0a 0d0a 2323 2320 4669 7865 640d 0a2d  ....### Fixed..-
-000016b0: 2060 5265 6c61 7469 6f6e 2e5f 746f 5f78   `Relation._to_x
-000016c0: 6d6c 2829 6020 7761 7320 7265 7475 726e  ml()` was return
-000016d0: 696e 6720 616e 2078 6d6c 2077 6974 686f  ing an xml witho
-000016e0: 7574 206f 736d 2074 6167 732e 0d0a 2d20  ut osm tags...- 
-000016f0: 4465 6c65 7465 6420 6469 7375 7365 6420  Deleted disused 
-00001700: 7661 7269 6162 6c65 2069 6e20 604e 6f64  variable in `Nod
-00001710: 652e 5f74 6f5f 786d 6c28 2960 2e0d 0a2d  e._to_xml()`...-
-00001720: 2046 6978 6564 2069 6e63 6f72 7265 6374   Fixed incorrect
-00001730: 2072 656c 6174 696f 6e20 7061 7273 696e   relation parsin
-00001740: 6720 6f66 2064 6174 6120 7265 6369 7665  g of data recive
-00001750: 6420 6279 2060 6675 6c6c 6020 656e 6470  d by `full` endp
-00001760: 6f69 6e74 2e0d 0a0d 0a23 2320 5b30 2e34  oint.....## [0.4
-00001770: 2e31 5d0d 0a23 2323 2043 6861 6e67 6564  .1]..### Changed
-00001780: 0d0a 2d20 5570 6461 7465 6420 6072 6571  ..- Updated `req
-00001790: 7565 7374 7360 2066 726f 6d20 6032 2e32  uests` from `2.2
-000017a0: 382e 3160 2074 6f20 6032 2e33 312e 3060  8.1` to `2.31.0`
-000017b0: 2e0d 0a0d 0a23 2320 5b30 2e34 2e30 5d0d  .....## [0.4.0].
-000017c0: 0a23 2323 2041 6464 6564 0d0a 2d20 6074  .### Added..- `t
-000017d0: 6f5f 6469 6374 2829 6020 6d65 7468 6f64  o_dict()` method
-000017e0: 2061 6e64 2060 6672 6f6d 5f64 6963 7428   and `from_dict(
-000017f0: 2960 2063 6c61 7373 206d 6574 686f 6420  )` class method 
-00001800: 746f 2060 4e6f 7465 602e 2020 0d0a 2d20  to `Note`.  ..- 
-00001810: 6074 6f5f 6469 6374 2829 6020 6d65 7468  `to_dict()` meth
-00001820: 6f64 2061 6e64 2060 6672 6f6d 5f64 6963  od and `from_dic
-00001830: 7428 2960 2063 6c61 7373 206d 6574 686f  t()` class metho
-00001840: 6420 746f 2060 436f 6d6d 656e 7460 2e0d  d to `Comment`..
-00001850: 0a2d 2060 746f 5f64 6963 7428 2960 206d  .- `to_dict()` m
-00001860: 6574 686f 6420 616e 6420 6066 726f 6d5f  ethod and `from_
-00001870: 6469 6374 2829 6020 636c 6173 7320 6d65  dict()` class me
-00001880: 7468 6f64 2074 6f20 6055 7365 7260 2e0d  thod to `User`..
-00001890: 0a2d 2044 6f63 756d 656e 7461 7469 6f6e  .- Documentation
-000018a0: 2061 626f 7574 2060 4d65 7461 6020 616e   about `Meta` an
-000018b0: 6420 6041 6374 696f 6e60 2063 6c61 7373  d `Action` class
-000018c0: 2e0d 0a2d 2041 7373 6572 7420 6572 726f  ...- Assert erro
-000018d0: 7220 2877 6974 6820 696e 666f 726d 6174  r (with informat
-000018e0: 696f 6e20 746f 2072 6570 6f72 7420 6974  ion to report it
-000018f0: 206f 6e20 6769 7468 7562 2920 7768 656e   on github) when
-00001900: 2061 7069 2072 6574 7572 6e73 2061 6e20   api returns an 
-00001910: 6572 726f 7220 636f 6465 206e 6f74 2064  error code not d
-00001920: 6573 6372 6962 6564 206f 6e20 7468 6520  escribed on the 
-00001930: 7769 6b69 2e0d 0a2d 2060 746f 5f64 6963  wiki...- `to_dic
-00001940: 7428 2960 206d 6574 686f 6420 616e 6420  t()` method and 
-00001950: 6066 726f 6d5f 6469 6374 2829 6020 636c  `from_dict()` cl
-00001960: 6173 7320 6d65 7468 6f64 2074 6f20 6028  ass method to `(
-00001970: 7265 6c61 7469 6f6e 2920 4d65 6d62 6572  relation) Member
-00001980: 602e 0d0a 0d0a 2323 2320 4669 7865 640d  `.....### Fixed.
-00001990: 0a2d 2060 4e6f 7465 6020 6361 6e20 6e6f  .- `Note` can no
-000019a0: 7720 6265 2069 6d70 6f72 7465 6420 6672  w be imported fr
-000019b0: 6f6d 2070 6163 6b61 6765 2e0d 0a2d 2060  om package...- `
-000019c0: 436f 6d6d 656e 7460 2063 616e 206e 6f77  Comment` can now
-000019d0: 2062 6520 696d 706f 7274 6564 2066 726f   be imported fro
-000019e0: 6d20 7061 636b 6167 652e 0d0a 2d20 6055  m package...- `U
-000019f0: 7365 7260 2063 616e 206e 6f77 2062 6520  ser` can now be 
-00001a00: 696d 706f 7274 6564 2066 726f 6d20 7061  imported from pa
-00001a10: 636b 6167 652e 0d0a 2d20 604d 656d 6265  ckage...- `Membe
-00001a20: 7260 2063 616e 206e 6f77 2062 6520 696d  r` can now be im
-00001a30: 706f 7274 6564 2066 726f 6d20 7061 636b  ported from pack
-00001a40: 6167 652e 0d0a 2d20 5064 6f63 2063 6f6d  age...- Pdoc com
-00001a50: 6d61 6e64 2069 6e20 6052 4541 444d 452e  mand in `README.
-00001a60: 6d64 602e 0d0a 2d20 6052 656c 6174 696f  md`...- `Relatio
-00001a70: 6e2e 746f 5f64 6963 7428 2960 206d 6574  n.to_dict()` met
-00001a80: 686f 6420 6e6f 7720 7265 6375 7273 6976  hod now recursiv
-00001a90: 656c 7920 7365 7269 616c 6973 6573 206d  ely serialises m
-00001aa0: 656d 6265 7273 2e0d 0a2d 2060 5761 792e  embers...- `Way.
-00001ab0: 746f 5f64 6963 7428 2960 206d 6574 686f  to_dict()` metho
-00001ac0: 6420 6e6f 7720 7265 6375 7273 6976 656c  d now recursivel
-00001ad0: 7920 7365 7269 616c 6973 6573 206e 6f64  y serialises nod
-00001ae0: 6573 2e0d 0a0d 0a23 2323 2043 6861 6e67  es.....### Chang
-00001af0: 6564 0d0a 2d20 4368 616e 6765 6420 696d  ed..- Changed im
-00001b00: 706f 7274 7320 696e 2060 5265 6c61 7469  ports in `Relati
-00001b10: 6f6e 2e70 7960 2074 6f20 7573 6520 696d  on.py` to use im
-00001b20: 706f 7274 696e 6720 7468 726f 7567 6820  porting through 
-00001b30: 6120 6d6f 6475 6c65 2072 6174 6865 7220  a module rather 
-00001b40: 7468 616e 2064 6972 6563 746c 7920 6672  than directly fr
-00001b50: 6f6d 2061 2066 696c 652e 0d0a 2d20 4164  om a file...- Ad
-00001b60: 6465 6420 6073 616d 706c 655f 6461 7461  ded `sample_data
-00001b70: 636c 6173 7365 732e 7079 6020 6669 6c65  classes.py` file
-00001b80: 2069 6e20 7465 7374 7320 6669 7874 7572   in tests fixtur
-00001b90: 6573 2074 6f20 7265 6475 6365 2063 6f64  es to reduce cod
-00001ba0: 6520 6475 706c 6963 6174 696f 6e2e 0d0a  e duplication...
-00001bb0: 2d20 4368 616e 6765 6420 6675 6e63 7469  - Changed functi
-00001bc0: 6f6e 206e 616d 6520 616e 6420 6465 6c65  on name and dele
-00001bd0: 7465 6420 756e 6e65 6365 7373 6172 7920  ted unnecessary 
-00001be0: 6172 6775 6d65 6e74 2069 6e20 6061 7070  argument in `app
-00001bf0: 656e 645f 656c 656d 656e 7473 5f74 6f5f  end_elements_to_
-00001c00: 6d61 7374 6572 5f65 6c65 6d65 6e74 2829  master_element()
-00001c10: 6020 6e65 7374 6564 2069 6e73 6964 6520  ` nested inside 
-00001c20: 7072 6976 6174 6520 6d65 7468 6f64 2060  private method `
-00001c30: 5f74 6f5f 786d 6c28 2960 2069 6e20 604f  _to_xml()` in `O
-00001c40: 736d 4368 616e 6765 602e 0d0a 0d0a 2323  smChange`.....##
-00001c50: 205b 302e 332e 305d 202d 2032 3032 332d   [0.3.0] - 2023-
-00001c60: 3033 2d31 340d 0a0d 0a23 2323 2041 6464  03-14....### Add
-00001c70: 6564 0d0a 2d20 6074 6f5f 6469 6374 2829  ed..- `to_dict()
-00001c80: 6020 6d65 7468 6f64 2061 6e64 2060 6672  ` method and `fr
-00001c90: 6f6d 5f64 6963 7428 2960 2063 6c61 7373  om_dict()` class
-00001ca0: 206d 6574 686f 6420 746f 2043 6861 6e67   method to Chang
-00001cb0: 6573 6574 2e20 5b23 375d 2868 7474 7073  eset. [#7](https
-00001cc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-00001cd0: 6365 6e74 5954 2f6f 736d 5f65 6173 795f  centYT/osm_easy_
-00001ce0: 6170 692f 6973 7375 6573 2f37 290d 0a2d  api/issues/7)..-
-00001cf0: 2041 6269 6c69 7479 2074 6f20 7365 7420   Ability to set 
-00001d00: 7573 6572 5f61 6765 6e74 2069 6e20 6044  user_agent in `D
-00001d10: 6966 6660 2061 6e64 2060 4170 6960 2063  iff` and `Api` c
-00001d20: 6c61 7373 2e20 5b23 355d 2868 7474 7073  lass. [#5](https
-00001d30: 3a2f 2f67 6974 6875 622e 636f 6d2f 646f  ://github.com/do
-00001d40: 6365 6e74 5954 2f6f 736d 5f65 6173 795f  centYT/osm_easy_
-00001d50: 6170 692f 6973 7375 6573 2f35 290d 0a2d  api/issues/5)..-
-00001d60: 2060 6f73 6d5f 6f62 6a65 6374 5f70 7269   `osm_object_pri
-00001d70: 6d69 7469 7665 6020 6066 726f 6d5f 6469  mitive` `from_di
-00001d80: 6374 2829 6020 636c 6173 7320 6d65 7468  ct()` class meth
-00001d90: 6f64 206e 6f77 2072 6169 7365 7320 6056  od now raises `V
-00001da0: 616c 7565 4572 726f 7260 2069 6620 7468  alueError` if th
-00001db0: 6520 6074 7970 6560 206b 6579 2069 7320  e `type` key is 
-00001dc0: 6e6f 7420 666f 756e 642e 0d0a 0d0a 2323  not found.....##
-00001dd0: 2320 4368 616e 6765 640d 0a2d 2060 4368  # Changed..- `Ch
-00001de0: 616e 6765 7365 7460 2069 7320 6e6f 7720  angeset` is now 
-00001df0: 6578 706f 7274 6564 2066 726f 6d20 6461  exported from da
-00001e00: 7461 5f63 6c61 7373 6573 206d 6f64 756c  ta_classes modul
-00001e10: 652e 0d0a 2d20 4d6f 7265 2074 6573 7473  e...- More tests
-00001e20: 2e0d 0a0d 0a23 2320 5b30 2e32 2e30 5d20  .....## [0.2.0] 
-00001e30: 2d20 3230 3233 2d30 332d 3037 0d0a 0d0a  - 2023-03-07....
-00001e40: 2323 2320 4164 6465 640d 0a2d 2060 746f  ### Added..- `to
-00001e50: 5f64 6963 7428 2960 206d 6574 686f 6420  _dict()` method 
-00001e60: 616e 6420 6066 726f 6d5f 6469 6374 2829  and `from_dict()
-00001e70: 6020 636c 6173 7320 6d65 7468 6f64 2074  ` class method t
-00001e80: 6f20 606f 736d 5f6f 626a 6563 745f 7072  o `osm_object_pr
-00001e90: 696d 6974 6976 6560 2e20 2841 6e20 6f62  imitive`. (An ob
-00001ea0: 6a65 6374 2074 6861 7420 6973 2069 6e68  ject that is inh
-00001eb0: 6572 6974 6564 2062 7920 6120 604e 6f64  erited by a `Nod
-00001ec0: 6560 2c20 6057 6179 602c 2060 5265 6c61  e`, `Way`, `Rela
-00001ed0: 7469 6f6e 6029 2e20 5b23 335d 2868 7474  tion`). [#3](htt
-00001ee0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001ef0: 646f 6365 6e74 5954 2f6f 736d 5f65 6173  docentYT/osm_eas
-00001f00: 795f 6170 692f 6973 7375 6573 2f33 290d  y_api/issues/3).
-00001f10: 0a2d 2053 7570 706f 7274 2066 6f72 2068  .- Support for h
-00001f20: 6973 746f 7269 6361 6c20 616e 6f6e 796d  istorical anonym
-00001f30: 6f75 7320 6564 6974 7320 616e 6420 6564  ous edits and ed
-00001f40: 6974 7320 6d61 6465 2062 7920 6465 6c65  its made by dele
-00001f50: 7465 6420 6163 636f 756e 7473 2e20 5b23  ted accounts. [#
-00001f60: 345d 2868 7474 7073 3a2f 2f67 6974 6875  4](https://githu
-00001f70: 622e 636f 6d2f 646f 6365 6e74 5954 2f6f  b.com/docentYT/o
-00001f80: 736d 5f65 6173 795f 6170 692f 6973 7375  sm_easy_api/issu
-00001f90: 6573 2f34 290d 0a0d 0a23 2320 5b30 2e31  es/4)....## [0.1
-00001fa0: 2e34 5d20 2d20 3230 3233 2d30 332d 3035  .4] - 2023-03-05
-00001fb0: 0d0a 0d0a 2323 2320 4669 7865 640d 0a2d  ....### Fixed..-
-00001fc0: 2049 6d70 726f 7665 6d65 6e74 206f 6620   Improvement of 
-00001fd0: 7574 696c 732e 6a6f 696e 5f75 726c 2829  utils.join_url()
-00001fe0: 2066 756e 6374 696f 6e2e 0d0a 2d20 5370   function...- Sp
-00001ff0: 656c 6c69 6e67 2065 7272 6f72 7320 636f  elling errors co
-00002000: 7272 6563 7465 6420 5b40 6d61 746b 6f6e  rrected [@matkon
-00002010: 6965 637a 5d28 6874 7470 733a 2f2f 6769  iecz](https://gi
-00002020: 7468 7562 2e63 6f6d 2f6d 6174 6b6f 6e69  thub.com/matkoni
-00002030: 6563 7a29 0d0a 0d0a 2323 205b 302e 312e  ecz)....## [0.1.
-00002040: 335d 202d 2032 3032 332d 3033 2d30 330d  3] - 2023-03-03.
-00002050: 0a0d 0a23 2323 2046 6978 6564 0d0a 0d0a  ...### Fixed....
-00002060: 2d20 4669 7865 6420 7468 6520 6e6f 6e2d  - Fixed the non-
-00002070: 7365 7474 696e 6720 6f66 2074 6865 2022  setting of the "
-00002080: 7669 7369 626c 6522 2061 7474 7269 6275  visible" attribu
-00002090: 7465 2e0d 0a0d 0a23 2320 5b30 2e31 2e32  te.....## [0.1.2
-000020a0: 5d20 2d20 3230 3233 2d30 332d 3033 0d0a  ] - 2023-03-03..
-000020b0: 0d0a 2323 2320 4669 7865 640d 0a0d 0a2d  ..### Fixed....-
-000020c0: 2046 6978 6564 2072 6574 7572 6e20 7479   Fixed return ty
-000020d0: 7065 206f 6620 6765 6e65 7261 746f 7220  pe of generator 
-000020e0: 696e 2044 6966 662e 6765 7428 2920 6d65  in Diff.get() me
-000020f0: 7468 6f64 2e0d 0a0d 0a23 2320 5b30 2e31  thod.....## [0.1
-00002100: 2e31 5d20 2d20 3230 3233 2d30 332d 3033  .1] - 2023-03-03
-00002110: 0d0a 0d0a 2323 2320 4164 6465 640d 0a0d  ....### Added...
-00002120: 0a2d 204c 6963 656e 7365 0d0a 0d0a 2323  .- License....##
-00002130: 205b 302e 312e 305d 202d 2032 3032 332d   [0.1.0] - 2023-
-00002140: 3033 2d30 330d 0a0d 0a23 2323 2041 6464  03-03....### Add
-00002150: 6564 0d0a 0d0a 2d20 496e 6974 6961 6c20  ed....- Initial 
-00002160: 696d 706f 7274 0d0a 2020 2020 2020 2020  import..        
-00002170: 2020 2020 2020 2020 2020 2020 474e 5520              GNU 
-00002180: 4745 4e45 5241 4c20 5055 424c 4943 204c  GENERAL PUBLIC L
-00002190: 4943 454e 5345 0d0a 2020 2020 2020 2020  ICENSE..        
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2056                 V
-000021b0: 6572 7369 6f6e 2033 2c20 3239 204a 756e  ersion 3, 29 Jun
-000021c0: 6520 3230 3037 0d0a 0d0a 2043 6f70 7972  e 2007.... Copyr
-000021d0: 6967 6874 2028 4329 2032 3030 3720 4672  ight (C) 2007 Fr
-000021e0: 6565 2053 6f66 7477 6172 6520 466f 756e  ee Software Foun
-000021f0: 6461 7469 6f6e 2c20 496e 632e 203c 6874  dation, Inc. <ht
-00002200: 7470 733a 2f2f 6673 662e 6f72 672f 3e0d  tps://fsf.org/>.
-00002210: 0a20 4576 6572 796f 6e65 2069 7320 7065  . Everyone is pe
-00002220: 726d 6974 7465 6420 746f 2063 6f70 7920  rmitted to copy 
-00002230: 616e 6420 6469 7374 7269 6275 7465 2076  and distribute v
-00002240: 6572 6261 7469 6d20 636f 7069 6573 0d0a  erbatim copies..
-00002250: 206f 6620 7468 6973 206c 6963 656e 7365   of this license
-00002260: 2064 6f63 756d 656e 742c 2062 7574 2063   document, but c
-00002270: 6861 6e67 696e 6720 6974 2069 7320 6e6f  hanging it is no
-00002280: 7420 616c 6c6f 7765 642e 0d0a 0d0a 2020  t allowed.....  
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2020 2020 2020 5072 6561 6d62            Preamb
-000022b0: 6c65 0d0a 0d0a 2020 5468 6520 474e 5520  le....  The GNU 
-000022c0: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-000022d0: 6963 656e 7365 2069 7320 6120 6672 6565  icense is a free
-000022e0: 2c20 636f 7079 6c65 6674 206c 6963 656e  , copyleft licen
-000022f0: 7365 2066 6f72 0d0a 736f 6674 7761 7265  se for..software
-00002300: 2061 6e64 206f 7468 6572 206b 696e 6473   and other kinds
-00002310: 206f 6620 776f 726b 732e 0d0a 0d0a 2020   of works.....  
-00002320: 5468 6520 6c69 6365 6e73 6573 2066 6f72  The licenses for
-00002330: 206d 6f73 7420 736f 6674 7761 7265 2061   most software a
-00002340: 6e64 206f 7468 6572 2070 7261 6374 6963  nd other practic
-00002350: 616c 2077 6f72 6b73 2061 7265 2064 6573  al works are des
-00002360: 6967 6e65 640d 0a74 6f20 7461 6b65 2061  igned..to take a
-00002370: 7761 7920 796f 7572 2066 7265 6564 6f6d  way your freedom
-00002380: 2074 6f20 7368 6172 6520 616e 6420 6368   to share and ch
-00002390: 616e 6765 2074 6865 2077 6f72 6b73 2e20  ange the works. 
-000023a0: 2042 7920 636f 6e74 7261 7374 2c0d 0a74   By contrast,..t
-000023b0: 6865 2047 4e55 2047 656e 6572 616c 2050  he GNU General P
-000023c0: 7562 6c69 6320 4c69 6365 6e73 6520 6973  ublic License is
-000023d0: 2069 6e74 656e 6465 6420 746f 2067 7561   intended to gua
-000023e0: 7261 6e74 6565 2079 6f75 7220 6672 6565  rantee your free
-000023f0: 646f 6d20 746f 0d0a 7368 6172 6520 616e  dom to..share an
-00002400: 6420 6368 616e 6765 2061 6c6c 2076 6572  d change all ver
-00002410: 7369 6f6e 7320 6f66 2061 2070 726f 6772  sions of a progr
-00002420: 616d 2d2d 746f 206d 616b 6520 7375 7265  am--to make sure
-00002430: 2069 7420 7265 6d61 696e 7320 6672 6565   it remains free
-00002440: 0d0a 736f 6674 7761 7265 2066 6f72 2061  ..software for a
-00002450: 6c6c 2069 7473 2075 7365 7273 2e20 2057  ll its users.  W
-00002460: 652c 2074 6865 2046 7265 6520 536f 6674  e, the Free Soft
-00002470: 7761 7265 2046 6f75 6e64 6174 696f 6e2c  ware Foundation,
-00002480: 2075 7365 2074 6865 0d0a 474e 5520 4765   use the..GNU Ge
-00002490: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000024a0: 656e 7365 2066 6f72 206d 6f73 7420 6f66  ense for most of
-000024b0: 206f 7572 2073 6f66 7477 6172 653b 2069   our software; i
-000024c0: 7420 6170 706c 6965 7320 616c 736f 2074  t applies also t
-000024d0: 6f0d 0a61 6e79 206f 7468 6572 2077 6f72  o..any other wor
-000024e0: 6b20 7265 6c65 6173 6564 2074 6869 7320  k released this 
-000024f0: 7761 7920 6279 2069 7473 2061 7574 686f  way by its autho
-00002500: 7273 2e20 2059 6f75 2063 616e 2061 7070  rs.  You can app
-00002510: 6c79 2069 7420 746f 0d0a 796f 7572 2070  ly it to..your p
-00002520: 726f 6772 616d 732c 2074 6f6f 2e0d 0a0d  rograms, too....
-00002530: 0a20 2057 6865 6e20 7765 2073 7065 616b  .  When we speak
-00002540: 206f 6620 6672 6565 2073 6f66 7477 6172   of free softwar
-00002550: 652c 2077 6520 6172 6520 7265 6665 7272  e, we are referr
-00002560: 696e 6720 746f 2066 7265 6564 6f6d 2c20  ing to freedom, 
-00002570: 6e6f 740d 0a70 7269 6365 2e20 204f 7572  not..price.  Our
-00002580: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-00002590: 4c69 6365 6e73 6573 2061 7265 2064 6573  Licenses are des
-000025a0: 6967 6e65 6420 746f 206d 616b 6520 7375  igned to make su
-000025b0: 7265 2074 6861 7420 796f 750d 0a68 6176  re that you..hav
-000025c0: 6520 7468 6520 6672 6565 646f 6d20 746f  e the freedom to
-000025d0: 2064 6973 7472 6962 7574 6520 636f 7069   distribute copi
-000025e0: 6573 206f 6620 6672 6565 2073 6f66 7477  es of free softw
-000025f0: 6172 6520 2861 6e64 2063 6861 7267 6520  are (and charge 
-00002600: 666f 720d 0a74 6865 6d20 6966 2079 6f75  for..them if you
-00002610: 2077 6973 6829 2c20 7468 6174 2079 6f75   wish), that you
-00002620: 2072 6563 6569 7665 2073 6f75 7263 6520   receive source 
-00002630: 636f 6465 206f 7220 6361 6e20 6765 7420  code or can get 
-00002640: 6974 2069 6620 796f 750d 0a77 616e 7420  it if you..want 
-00002650: 6974 2c20 7468 6174 2079 6f75 2063 616e  it, that you can
-00002660: 2063 6861 6e67 6520 7468 6520 736f 6674   change the soft
-00002670: 7761 7265 206f 7220 7573 6520 7069 6563  ware or use piec
-00002680: 6573 206f 6620 6974 2069 6e20 6e65 770d  es of it in new.
-00002690: 0a66 7265 6520 7072 6f67 7261 6d73 2c20  .free programs, 
-000026a0: 616e 6420 7468 6174 2079 6f75 206b 6e6f  and that you kno
-000026b0: 7720 796f 7520 6361 6e20 646f 2074 6865  w you can do the
-000026c0: 7365 2074 6869 6e67 732e 0d0a 0d0a 2020  se things.....  
-000026d0: 546f 2070 726f 7465 6374 2079 6f75 7220  To protect your 
-000026e0: 7269 6768 7473 2c20 7765 206e 6565 6420  rights, we need 
-000026f0: 746f 2070 7265 7665 6e74 206f 7468 6572  to prevent other
-00002700: 7320 6672 6f6d 2064 656e 7969 6e67 2079  s from denying y
-00002710: 6f75 0d0a 7468 6573 6520 7269 6768 7473  ou..these rights
-00002720: 206f 7220 6173 6b69 6e67 2079 6f75 2074   or asking you t
-00002730: 6f20 7375 7272 656e 6465 7220 7468 6520  o surrender the 
-00002740: 7269 6768 7473 2e20 2054 6865 7265 666f  rights.  Therefo
-00002750: 7265 2c20 796f 7520 6861 7665 0d0a 6365  re, you have..ce
-00002760: 7274 6169 6e20 7265 7370 6f6e 7369 6269  rtain responsibi
-00002770: 6c69 7469 6573 2069 6620 796f 7520 6469  lities if you di
-00002780: 7374 7269 6275 7465 2063 6f70 6965 7320  stribute copies 
-00002790: 6f66 2074 6865 2073 6f66 7477 6172 652c  of the software,
-000027a0: 206f 7220 6966 0d0a 796f 7520 6d6f 6469   or if..you modi
-000027b0: 6679 2069 743a 2072 6573 706f 6e73 6962  fy it: responsib
-000027c0: 696c 6974 6965 7320 746f 2072 6573 7065  ilities to respe
-000027d0: 6374 2074 6865 2066 7265 6564 6f6d 206f  ct the freedom o
-000027e0: 6620 6f74 6865 7273 2e0d 0a0d 0a20 2046  f others.....  F
-000027f0: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
-00002800: 6f75 2064 6973 7472 6962 7574 6520 636f  ou distribute co
-00002810: 7069 6573 206f 6620 7375 6368 2061 2070  pies of such a p
-00002820: 726f 6772 616d 2c20 7768 6574 6865 720d  rogram, whether.
-00002830: 0a67 7261 7469 7320 6f72 2066 6f72 2061  .gratis or for a
-00002840: 2066 6565 2c20 796f 7520 6d75 7374 2070   fee, you must p
-00002850: 6173 7320 6f6e 2074 6f20 7468 6520 7265  ass on to the re
-00002860: 6369 7069 656e 7473 2074 6865 2073 616d  cipients the sam
-00002870: 650d 0a66 7265 6564 6f6d 7320 7468 6174  e..freedoms that
-00002880: 2079 6f75 2072 6563 6569 7665 642e 2020   you received.  
-00002890: 596f 7520 6d75 7374 206d 616b 6520 7375  You must make su
-000028a0: 7265 2074 6861 7420 7468 6579 2c20 746f  re that they, to
-000028b0: 6f2c 2072 6563 6569 7665 0d0a 6f72 2063  o, receive..or c
-000028c0: 616e 2067 6574 2074 6865 2073 6f75 7263  an get the sourc
-000028d0: 6520 636f 6465 2e20 2041 6e64 2079 6f75  e code.  And you
-000028e0: 206d 7573 7420 7368 6f77 2074 6865 6d20   must show them 
-000028f0: 7468 6573 6520 7465 726d 7320 736f 2074  these terms so t
-00002900: 6865 790d 0a6b 6e6f 7720 7468 6569 7220  hey..know their 
-00002910: 7269 6768 7473 2e0d 0a0d 0a20 2044 6576  rights.....  Dev
-00002920: 656c 6f70 6572 7320 7468 6174 2075 7365  elopers that use
-00002930: 2074 6865 2047 4e55 2047 504c 2070 726f   the GNU GPL pro
-00002940: 7465 6374 2079 6f75 7220 7269 6768 7473  tect your rights
-00002950: 2077 6974 6820 7477 6f20 7374 6570 733a   with two steps:
-00002960: 0d0a 2831 2920 6173 7365 7274 2063 6f70  ..(1) assert cop
-00002970: 7972 6967 6874 206f 6e20 7468 6520 736f  yright on the so
-00002980: 6674 7761 7265 2c20 616e 6420 2832 2920  ftware, and (2) 
-00002990: 6f66 6665 7220 796f 7520 7468 6973 204c  offer you this L
-000029a0: 6963 656e 7365 0d0a 6769 7669 6e67 2079  icense..giving y
-000029b0: 6f75 206c 6567 616c 2070 6572 6d69 7373  ou legal permiss
-000029c0: 696f 6e20 746f 2063 6f70 792c 2064 6973  ion to copy, dis
-000029d0: 7472 6962 7574 6520 616e 642f 6f72 206d  tribute and/or m
-000029e0: 6f64 6966 7920 6974 2e0d 0a0d 0a20 2046  odify it.....  F
-000029f0: 6f72 2074 6865 2064 6576 656c 6f70 6572  or the developer
-00002a00: 7327 2061 6e64 2061 7574 686f 7273 2720  s' and authors' 
-00002a10: 7072 6f74 6563 7469 6f6e 2c20 7468 6520  protection, the 
-00002a20: 4750 4c20 636c 6561 726c 7920 6578 706c  GPL clearly expl
-00002a30: 6169 6e73 0d0a 7468 6174 2074 6865 7265  ains..that there
-00002a40: 2069 7320 6e6f 2077 6172 7261 6e74 7920   is no warranty 
-00002a50: 666f 7220 7468 6973 2066 7265 6520 736f  for this free so
-00002a60: 6674 7761 7265 2e20 2046 6f72 2062 6f74  ftware.  For bot
-00002a70: 6820 7573 6572 7327 2061 6e64 0d0a 6175  h users' and..au
-00002a80: 7468 6f72 7327 2073 616b 652c 2074 6865  thors' sake, the
-00002a90: 2047 504c 2072 6571 7569 7265 7320 7468   GPL requires th
-00002aa0: 6174 206d 6f64 6966 6965 6420 7665 7273  at modified vers
-00002ab0: 696f 6e73 2062 6520 6d61 726b 6564 2061  ions be marked a
-00002ac0: 730d 0a63 6861 6e67 6564 2c20 736f 2074  s..changed, so t
-00002ad0: 6861 7420 7468 6569 7220 7072 6f62 6c65  hat their proble
-00002ae0: 6d73 2077 696c 6c20 6e6f 7420 6265 2061  ms will not be a
-00002af0: 7474 7269 6275 7465 6420 6572 726f 6e65  ttributed errone
-00002b00: 6f75 736c 7920 746f 0d0a 6175 7468 6f72  ously to..author
-00002b10: 7320 6f66 2070 7265 7669 6f75 7320 7665  s of previous ve
-00002b20: 7273 696f 6e73 2e0d 0a0d 0a20 2053 6f6d  rsions.....  Som
-00002b30: 6520 6465 7669 6365 7320 6172 6520 6465  e devices are de
-00002b40: 7369 676e 6564 2074 6f20 6465 6e79 2075  signed to deny u
-00002b50: 7365 7273 2061 6363 6573 7320 746f 2069  sers access to i
-00002b60: 6e73 7461 6c6c 206f 7220 7275 6e0d 0a6d  nstall or run..m
-00002b70: 6f64 6966 6965 6420 7665 7273 696f 6e73  odified versions
-00002b80: 206f 6620 7468 6520 736f 6674 7761 7265   of the software
-00002b90: 2069 6e73 6964 6520 7468 656d 2c20 616c   inside them, al
-00002ba0: 7468 6f75 6768 2074 6865 206d 616e 7566  though the manuf
-00002bb0: 6163 7475 7265 720d 0a63 616e 2064 6f20  acturer..can do 
-00002bc0: 736f 2e20 2054 6869 7320 6973 2066 756e  so.  This is fun
-00002bd0: 6461 6d65 6e74 616c 6c79 2069 6e63 6f6d  damentally incom
-00002be0: 7061 7469 626c 6520 7769 7468 2074 6865  patible with the
-00002bf0: 2061 696d 206f 660d 0a70 726f 7465 6374   aim of..protect
-00002c00: 696e 6720 7573 6572 7327 2066 7265 6564  ing users' freed
-00002c10: 6f6d 2074 6f20 6368 616e 6765 2074 6865  om to change the
-00002c20: 2073 6f66 7477 6172 652e 2020 5468 6520   software.  The 
-00002c30: 7379 7374 656d 6174 6963 0d0a 7061 7474  systematic..patt
-00002c40: 6572 6e20 6f66 2073 7563 6820 6162 7573  ern of such abus
-00002c50: 6520 6f63 6375 7273 2069 6e20 7468 6520  e occurs in the 
-00002c60: 6172 6561 206f 6620 7072 6f64 7563 7473  area of products
-00002c70: 2066 6f72 2069 6e64 6976 6964 7561 6c73   for individuals
-00002c80: 2074 6f0d 0a75 7365 2c20 7768 6963 6820   to..use, which 
-00002c90: 6973 2070 7265 6369 7365 6c79 2077 6865  is precisely whe
-00002ca0: 7265 2069 7420 6973 206d 6f73 7420 756e  re it is most un
-00002cb0: 6163 6365 7074 6162 6c65 2e20 2054 6865  acceptable.  The
-00002cc0: 7265 666f 7265 2c20 7765 0d0a 6861 7665  refore, we..have
-00002cd0: 2064 6573 6967 6e65 6420 7468 6973 2076   designed this v
-00002ce0: 6572 7369 6f6e 206f 6620 7468 6520 4750  ersion of the GP
-00002cf0: 4c20 746f 2070 726f 6869 6269 7420 7468  L to prohibit th
-00002d00: 6520 7072 6163 7469 6365 2066 6f72 2074  e practice for t
-00002d10: 686f 7365 0d0a 7072 6f64 7563 7473 2e20  hose..products. 
-00002d20: 2049 6620 7375 6368 2070 726f 626c 656d   If such problem
-00002d30: 7320 6172 6973 6520 7375 6273 7461 6e74  s arise substant
-00002d40: 6961 6c6c 7920 696e 206f 7468 6572 2064  ially in other d
-00002d50: 6f6d 6169 6e73 2c20 7765 0d0a 7374 616e  omains, we..stan
-00002d60: 6420 7265 6164 7920 746f 2065 7874 656e  d ready to exten
-00002d70: 6420 7468 6973 2070 726f 7669 7369 6f6e  d this provision
-00002d80: 2074 6f20 7468 6f73 6520 646f 6d61 696e   to those domain
-00002d90: 7320 696e 2066 7574 7572 6520 7665 7273  s in future vers
-00002da0: 696f 6e73 0d0a 6f66 2074 6865 2047 504c  ions..of the GPL
-00002db0: 2c20 6173 206e 6565 6465 6420 746f 2070  , as needed to p
-00002dc0: 726f 7465 6374 2074 6865 2066 7265 6564  rotect the freed
-00002dd0: 6f6d 206f 6620 7573 6572 732e 0d0a 0d0a  om of users.....
-00002de0: 2020 4669 6e61 6c6c 792c 2065 7665 7279    Finally, every
-00002df0: 2070 726f 6772 616d 2069 7320 7468 7265   program is thre
-00002e00: 6174 656e 6564 2063 6f6e 7374 616e 746c  atened constantl
-00002e10: 7920 6279 2073 6f66 7477 6172 6520 7061  y by software pa
-00002e20: 7465 6e74 732e 0d0a 5374 6174 6573 2073  tents...States s
-00002e30: 686f 756c 6420 6e6f 7420 616c 6c6f 7720  hould not allow 
-00002e40: 7061 7465 6e74 7320 746f 2072 6573 7472  patents to restr
-00002e50: 6963 7420 6465 7665 6c6f 706d 656e 7420  ict development 
-00002e60: 616e 6420 7573 6520 6f66 0d0a 736f 6674  and use of..soft
-00002e70: 7761 7265 206f 6e20 6765 6e65 7261 6c2d  ware on general-
-00002e80: 7075 7270 6f73 6520 636f 6d70 7574 6572  purpose computer
-00002e90: 732c 2062 7574 2069 6e20 7468 6f73 6520  s, but in those 
-00002ea0: 7468 6174 2064 6f2c 2077 6520 7769 7368  that do, we wish
-00002eb0: 2074 6f0d 0a61 766f 6964 2074 6865 2073   to..avoid the s
-00002ec0: 7065 6369 616c 2064 616e 6765 7220 7468  pecial danger th
-00002ed0: 6174 2070 6174 656e 7473 2061 7070 6c69  at patents appli
-00002ee0: 6564 2074 6f20 6120 6672 6565 2070 726f  ed to a free pro
-00002ef0: 6772 616d 2063 6f75 6c64 0d0a 6d61 6b65  gram could..make
-00002f00: 2069 7420 6566 6665 6374 6976 656c 7920   it effectively 
-00002f10: 7072 6f70 7269 6574 6172 792e 2020 546f  proprietary.  To
-00002f20: 2070 7265 7665 6e74 2074 6869 732c 2074   prevent this, t
-00002f30: 6865 2047 504c 2061 7373 7572 6573 2074  he GPL assures t
-00002f40: 6861 740d 0a70 6174 656e 7473 2063 616e  hat..patents can
-00002f50: 6e6f 7420 6265 2075 7365 6420 746f 2072  not be used to r
-00002f60: 656e 6465 7220 7468 6520 7072 6f67 7261  ender the progra
-00002f70: 6d20 6e6f 6e2d 6672 6565 2e0d 0a0d 0a20  m non-free..... 
-00002f80: 2054 6865 2070 7265 6369 7365 2074 6572   The precise ter
-00002f90: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
-00002fa0: 7320 666f 7220 636f 7079 696e 672c 2064  s for copying, d
-00002fb0: 6973 7472 6962 7574 696f 6e20 616e 640d  istribution and.
-00002fc0: 0a6d 6f64 6966 6963 6174 696f 6e20 666f  .modification fo
-00002fd0: 6c6c 6f77 2e0d 0a0d 0a20 2020 2020 2020  llow.....       
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 5445 524d 5320 414e 4420 434f 4e44 4954  TERMS AND CONDIT
-00003000: 494f 4e53 0d0a 0d0a 2020 302e 2044 6566  IONS....  0. Def
-00003010: 696e 6974 696f 6e73 2e0d 0a0d 0a20 2022  initions.....  "
-00003020: 5468 6973 204c 6963 656e 7365 2220 7265  This License" re
-00003030: 6665 7273 2074 6f20 7665 7273 696f 6e20  fers to version 
-00003040: 3320 6f66 2074 6865 2047 4e55 2047 656e  3 of the GNU Gen
-00003050: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00003060: 6e73 652e 0d0a 0d0a 2020 2243 6f70 7972  nse.....  "Copyr
-00003070: 6967 6874 2220 616c 736f 206d 6561 6e73  ight" also means
-00003080: 2063 6f70 7972 6967 6874 2d6c 696b 6520   copyright-like 
-00003090: 6c61 7773 2074 6861 7420 6170 706c 7920  laws that apply 
-000030a0: 746f 206f 7468 6572 206b 696e 6473 206f  to other kinds o
-000030b0: 660d 0a77 6f72 6b73 2c20 7375 6368 2061  f..works, such a
-000030c0: 7320 7365 6d69 636f 6e64 7563 746f 7220  s semiconductor 
-000030d0: 6d61 736b 732e 0d0a 0d0a 2020 2254 6865  masks.....  "The
-000030e0: 2050 726f 6772 616d 2220 7265 6665 7273   Program" refers
-000030f0: 2074 6f20 616e 7920 636f 7079 7269 6768   to any copyrigh
-00003100: 7461 626c 6520 776f 726b 206c 6963 656e  table work licen
-00003110: 7365 6420 756e 6465 7220 7468 6973 0d0a  sed under this..
-00003120: 4c69 6365 6e73 652e 2020 4561 6368 206c  License.  Each l
-00003130: 6963 656e 7365 6520 6973 2061 6464 7265  icensee is addre
-00003140: 7373 6564 2061 7320 2279 6f75 222e 2020  ssed as "you".  
-00003150: 224c 6963 656e 7365 6573 2220 616e 640d  "Licensees" and.
-00003160: 0a22 7265 6369 7069 656e 7473 2220 6d61  ."recipients" ma
-00003170: 7920 6265 2069 6e64 6976 6964 7561 6c73  y be individuals
-00003180: 206f 7220 6f72 6761 6e69 7a61 7469 6f6e   or organization
-00003190: 732e 0d0a 0d0a 2020 546f 2022 6d6f 6469  s.....  To "modi
-000031a0: 6679 2220 6120 776f 726b 206d 6561 6e73  fy" a work means
-000031b0: 2074 6f20 636f 7079 2066 726f 6d20 6f72   to copy from or
-000031c0: 2061 6461 7074 2061 6c6c 206f 7220 7061   adapt all or pa
-000031d0: 7274 206f 6620 7468 6520 776f 726b 0d0a  rt of the work..
-000031e0: 696e 2061 2066 6173 6869 6f6e 2072 6571  in a fashion req
-000031f0: 7569 7269 6e67 2063 6f70 7972 6967 6874  uiring copyright
-00003200: 2070 6572 6d69 7373 696f 6e2c 206f 7468   permission, oth
-00003210: 6572 2074 6861 6e20 7468 6520 6d61 6b69  er than the maki
-00003220: 6e67 206f 6620 616e 0d0a 6578 6163 7420  ng of an..exact 
-00003230: 636f 7079 2e20 2054 6865 2072 6573 756c  copy.  The resul
-00003240: 7469 6e67 2077 6f72 6b20 6973 2063 616c  ting work is cal
-00003250: 6c65 6420 6120 226d 6f64 6966 6965 6420  led a "modified 
-00003260: 7665 7273 696f 6e22 206f 6620 7468 650d  version" of the.
-00003270: 0a65 6172 6c69 6572 2077 6f72 6b20 6f72  .earlier work or
-00003280: 2061 2077 6f72 6b20 2262 6173 6564 206f   a work "based o
-00003290: 6e22 2074 6865 2065 6172 6c69 6572 2077  n" the earlier w
-000032a0: 6f72 6b2e 0d0a 0d0a 2020 4120 2263 6f76  ork.....  A "cov
-000032b0: 6572 6564 2077 6f72 6b22 206d 6561 6e73  ered work" means
-000032c0: 2065 6974 6865 7220 7468 6520 756e 6d6f   either the unmo
-000032d0: 6469 6669 6564 2050 726f 6772 616d 206f  dified Program o
-000032e0: 7220 6120 776f 726b 2062 6173 6564 0d0a  r a work based..
-000032f0: 6f6e 2074 6865 2050 726f 6772 616d 2e0d  on the Program..
-00003300: 0a0d 0a20 2054 6f20 2270 726f 7061 6761  ...  To "propaga
-00003310: 7465 2220 6120 776f 726b 206d 6561 6e73  te" a work means
-00003320: 2074 6f20 646f 2061 6e79 7468 696e 6720   to do anything 
-00003330: 7769 7468 2069 7420 7468 6174 2c20 7769  with it that, wi
-00003340: 7468 6f75 740d 0a70 6572 6d69 7373 696f  thout..permissio
-00003350: 6e2c 2077 6f75 6c64 206d 616b 6520 796f  n, would make yo
-00003360: 7520 6469 7265 6374 6c79 206f 7220 7365  u directly or se
-00003370: 636f 6e64 6172 696c 7920 6c69 6162 6c65  condarily liable
-00003380: 2066 6f72 0d0a 696e 6672 696e 6765 6d65   for..infringeme
-00003390: 6e74 2075 6e64 6572 2061 7070 6c69 6361  nt under applica
-000033a0: 626c 6520 636f 7079 7269 6768 7420 6c61  ble copyright la
-000033b0: 772c 2065 7863 6570 7420 6578 6563 7574  w, except execut
-000033c0: 696e 6720 6974 206f 6e20 610d 0a63 6f6d  ing it on a..com
-000033d0: 7075 7465 7220 6f72 206d 6f64 6966 7969  puter or modifyi
-000033e0: 6e67 2061 2070 7269 7661 7465 2063 6f70  ng a private cop
-000033f0: 792e 2020 5072 6f70 6167 6174 696f 6e20  y.  Propagation 
-00003400: 696e 636c 7564 6573 2063 6f70 7969 6e67  includes copying
-00003410: 2c0d 0a64 6973 7472 6962 7574 696f 6e20  ,..distribution 
-00003420: 2877 6974 6820 6f72 2077 6974 686f 7574  (with or without
-00003430: 206d 6f64 6966 6963 6174 696f 6e29 2c20   modification), 
-00003440: 6d61 6b69 6e67 2061 7661 696c 6162 6c65  making available
-00003450: 2074 6f20 7468 650d 0a70 7562 6c69 632c   to the..public,
-00003460: 2061 6e64 2069 6e20 736f 6d65 2063 6f75   and in some cou
-00003470: 6e74 7269 6573 206f 7468 6572 2061 6374  ntries other act
-00003480: 6976 6974 6965 7320 6173 2077 656c 6c2e  ivities as well.
-00003490: 0d0a 0d0a 2020 546f 2022 636f 6e76 6579  ....  To "convey
-000034a0: 2220 6120 776f 726b 206d 6561 6e73 2061  " a work means a
-000034b0: 6e79 206b 696e 6420 6f66 2070 726f 7061  ny kind of propa
-000034c0: 6761 7469 6f6e 2074 6861 7420 656e 6162  gation that enab
-000034d0: 6c65 7320 6f74 6865 720d 0a70 6172 7469  les other..parti
-000034e0: 6573 2074 6f20 6d61 6b65 206f 7220 7265  es to make or re
-000034f0: 6365 6976 6520 636f 7069 6573 2e20 204d  ceive copies.  M
-00003500: 6572 6520 696e 7465 7261 6374 696f 6e20  ere interaction 
-00003510: 7769 7468 2061 2075 7365 7220 7468 726f  with a user thro
-00003520: 7567 680d 0a61 2063 6f6d 7075 7465 7220  ugh..a computer 
-00003530: 6e65 7477 6f72 6b2c 2077 6974 6820 6e6f  network, with no
-00003540: 2074 7261 6e73 6665 7220 6f66 2061 2063   transfer of a c
-00003550: 6f70 792c 2069 7320 6e6f 7420 636f 6e76  opy, is not conv
-00003560: 6579 696e 672e 0d0a 0d0a 2020 416e 2069  eying.....  An i
-00003570: 6e74 6572 6163 7469 7665 2075 7365 7220  nteractive user 
-00003580: 696e 7465 7266 6163 6520 6469 7370 6c61  interface displa
-00003590: 7973 2022 4170 7072 6f70 7269 6174 6520  ys "Appropriate 
-000035a0: 4c65 6761 6c20 4e6f 7469 6365 7322 0d0a  Legal Notices"..
-000035b0: 746f 2074 6865 2065 7874 656e 7420 7468  to the extent th
-000035c0: 6174 2069 7420 696e 636c 7564 6573 2061  at it includes a
-000035d0: 2063 6f6e 7665 6e69 656e 7420 616e 6420   convenient and 
-000035e0: 7072 6f6d 696e 656e 746c 7920 7669 7369  prominently visi
-000035f0: 626c 650d 0a66 6561 7475 7265 2074 6861  ble..feature tha
-00003600: 7420 2831 2920 6469 7370 6c61 7973 2061  t (1) displays a
-00003610: 6e20 6170 7072 6f70 7269 6174 6520 636f  n appropriate co
-00003620: 7079 7269 6768 7420 6e6f 7469 6365 2c20  pyright notice, 
-00003630: 616e 6420 2832 290d 0a74 656c 6c73 2074  and (2)..tells t
-00003640: 6865 2075 7365 7220 7468 6174 2074 6865  he user that the
-00003650: 7265 2069 7320 6e6f 2077 6172 7261 6e74  re is no warrant
-00003660: 7920 666f 7220 7468 6520 776f 726b 2028  y for the work (
-00003670: 6578 6365 7074 2074 6f20 7468 650d 0a65  except to the..e
-00003680: 7874 656e 7420 7468 6174 2077 6172 7261  xtent that warra
-00003690: 6e74 6965 7320 6172 6520 7072 6f76 6964  nties are provid
-000036a0: 6564 292c 2074 6861 7420 6c69 6365 6e73  ed), that licens
-000036b0: 6565 7320 6d61 7920 636f 6e76 6579 2074  ees may convey t
-000036c0: 6865 0d0a 776f 726b 2075 6e64 6572 2074  he..work under t
-000036d0: 6869 7320 4c69 6365 6e73 652c 2061 6e64  his License, and
-000036e0: 2068 6f77 2074 6f20 7669 6577 2061 2063   how to view a c
-000036f0: 6f70 7920 6f66 2074 6869 7320 4c69 6365  opy of this Lice
-00003700: 6e73 652e 2020 4966 0d0a 7468 6520 696e  nse.  If..the in
-00003710: 7465 7266 6163 6520 7072 6573 656e 7473  terface presents
-00003720: 2061 206c 6973 7420 6f66 2075 7365 7220   a list of user 
-00003730: 636f 6d6d 616e 6473 206f 7220 6f70 7469  commands or opti
-00003740: 6f6e 732c 2073 7563 6820 6173 2061 0d0a  ons, such as a..
-00003750: 6d65 6e75 2c20 6120 7072 6f6d 696e 656e  menu, a prominen
-00003760: 7420 6974 656d 2069 6e20 7468 6520 6c69  t item in the li
-00003770: 7374 206d 6565 7473 2074 6869 7320 6372  st meets this cr
-00003780: 6974 6572 696f 6e2e 0d0a 0d0a 2020 312e  iterion.....  1.
-00003790: 2053 6f75 7263 6520 436f 6465 2e0d 0a0d   Source Code....
-000037a0: 0a20 2054 6865 2022 736f 7572 6365 2063  .  The "source c
-000037b0: 6f64 6522 2066 6f72 2061 2077 6f72 6b20  ode" for a work 
-000037c0: 6d65 616e 7320 7468 6520 7072 6566 6572  means the prefer
-000037d0: 7265 6420 666f 726d 206f 6620 7468 6520  red form of the 
-000037e0: 776f 726b 0d0a 666f 7220 6d61 6b69 6e67  work..for making
-000037f0: 206d 6f64 6966 6963 6174 696f 6e73 2074   modifications t
-00003800: 6f20 6974 2e20 2022 4f62 6a65 6374 2063  o it.  "Object c
-00003810: 6f64 6522 206d 6561 6e73 2061 6e79 206e  ode" means any n
-00003820: 6f6e 2d73 6f75 7263 650d 0a66 6f72 6d20  on-source..form 
-00003830: 6f66 2061 2077 6f72 6b2e 0d0a 0d0a 2020  of a work.....  
-00003840: 4120 2253 7461 6e64 6172 6420 496e 7465  A "Standard Inte
-00003850: 7266 6163 6522 206d 6561 6e73 2061 6e20  rface" means an 
-00003860: 696e 7465 7266 6163 6520 7468 6174 2065  interface that e
-00003870: 6974 6865 7220 6973 2061 6e20 6f66 6669  ither is an offi
-00003880: 6369 616c 0d0a 7374 616e 6461 7264 2064  cial..standard d
-00003890: 6566 696e 6564 2062 7920 6120 7265 636f  efined by a reco
-000038a0: 676e 697a 6564 2073 7461 6e64 6172 6473  gnized standards
-000038b0: 2062 6f64 792c 206f 722c 2069 6e20 7468   body, or, in th
-000038c0: 6520 6361 7365 206f 660d 0a69 6e74 6572  e case of..inter
-000038d0: 6661 6365 7320 7370 6563 6966 6965 6420  faces specified 
-000038e0: 666f 7220 6120 7061 7274 6963 756c 6172  for a particular
-000038f0: 2070 726f 6772 616d 6d69 6e67 206c 616e   programming lan
-00003900: 6775 6167 652c 206f 6e65 2074 6861 740d  guage, one that.
-00003910: 0a69 7320 7769 6465 6c79 2075 7365 6420  .is widely used 
-00003920: 616d 6f6e 6720 6465 7665 6c6f 7065 7273  among developers
-00003930: 2077 6f72 6b69 6e67 2069 6e20 7468 6174   working in that
-00003940: 206c 616e 6775 6167 652e 0d0a 0d0a 2020   language.....  
-00003950: 5468 6520 2253 7973 7465 6d20 4c69 6272  The "System Libr
-00003960: 6172 6965 7322 206f 6620 616e 2065 7865  aries" of an exe
-00003970: 6375 7461 626c 6520 776f 726b 2069 6e63  cutable work inc
-00003980: 6c75 6465 2061 6e79 7468 696e 672c 206f  lude anything, o
-00003990: 7468 6572 0d0a 7468 616e 2074 6865 2077  ther..than the w
-000039a0: 6f72 6b20 6173 2061 2077 686f 6c65 2c20  ork as a whole, 
-000039b0: 7468 6174 2028 6129 2069 7320 696e 636c  that (a) is incl
-000039c0: 7564 6564 2069 6e20 7468 6520 6e6f 726d  uded in the norm
-000039d0: 616c 2066 6f72 6d20 6f66 0d0a 7061 636b  al form of..pack
-000039e0: 6167 696e 6720 6120 4d61 6a6f 7220 436f  aging a Major Co
-000039f0: 6d70 6f6e 656e 742c 2062 7574 2077 6869  mponent, but whi
-00003a00: 6368 2069 7320 6e6f 7420 7061 7274 206f  ch is not part o
-00003a10: 6620 7468 6174 204d 616a 6f72 0d0a 436f  f that Major..Co
-00003a20: 6d70 6f6e 656e 742c 2061 6e64 2028 6229  mponent, and (b)
-00003a30: 2073 6572 7665 7320 6f6e 6c79 2074 6f20   serves only to 
-00003a40: 656e 6162 6c65 2075 7365 206f 6620 7468  enable use of th
-00003a50: 6520 776f 726b 2077 6974 6820 7468 6174  e work with that
-00003a60: 0d0a 4d61 6a6f 7220 436f 6d70 6f6e 656e  ..Major Componen
-00003a70: 742c 206f 7220 746f 2069 6d70 6c65 6d65  t, or to impleme
-00003a80: 6e74 2061 2053 7461 6e64 6172 6420 496e  nt a Standard In
-00003a90: 7465 7266 6163 6520 666f 7220 7768 6963  terface for whic
-00003aa0: 6820 616e 0d0a 696d 706c 656d 656e 7461  h an..implementa
-00003ab0: 7469 6f6e 2069 7320 6176 6169 6c61 626c  tion is availabl
-00003ac0: 6520 746f 2074 6865 2070 7562 6c69 6320  e to the public 
-00003ad0: 696e 2073 6f75 7263 6520 636f 6465 2066  in source code f
-00003ae0: 6f72 6d2e 2020 410d 0a22 4d61 6a6f 7220  orm.  A.."Major 
-00003af0: 436f 6d70 6f6e 656e 7422 2c20 696e 2074  Component", in t
-00003b00: 6869 7320 636f 6e74 6578 742c 206d 6561  his context, mea
-00003b10: 6e73 2061 206d 616a 6f72 2065 7373 656e  ns a major essen
-00003b20: 7469 616c 2063 6f6d 706f 6e65 6e74 0d0a  tial component..
-00003b30: 286b 6572 6e65 6c2c 2077 696e 646f 7720  (kernel, window 
-00003b40: 7379 7374 656d 2c20 616e 6420 736f 206f  system, and so o
-00003b50: 6e29 206f 6620 7468 6520 7370 6563 6966  n) of the specif
-00003b60: 6963 206f 7065 7261 7469 6e67 2073 7973  ic operating sys
-00003b70: 7465 6d0d 0a28 6966 2061 6e79 2920 6f6e  tem..(if any) on
-00003b80: 2077 6869 6368 2074 6865 2065 7865 6375   which the execu
-00003b90: 7461 626c 6520 776f 726b 2072 756e 732c  table work runs,
-00003ba0: 206f 7220 6120 636f 6d70 696c 6572 2075   or a compiler u
-00003bb0: 7365 6420 746f 0d0a 7072 6f64 7563 6520  sed to..produce 
-00003bc0: 7468 6520 776f 726b 2c20 6f72 2061 6e20  the work, or an 
-00003bd0: 6f62 6a65 6374 2063 6f64 6520 696e 7465  object code inte
-00003be0: 7270 7265 7465 7220 7573 6564 2074 6f20  rpreter used to 
-00003bf0: 7275 6e20 6974 2e0d 0a0d 0a20 2054 6865  run it.....  The
-00003c00: 2022 436f 7272 6573 706f 6e64 696e 6720   "Corresponding 
-00003c10: 536f 7572 6365 2220 666f 7220 6120 776f  Source" for a wo
-00003c20: 726b 2069 6e20 6f62 6a65 6374 2063 6f64  rk in object cod
-00003c30: 6520 666f 726d 206d 6561 6e73 2061 6c6c  e form means all
-00003c40: 0d0a 7468 6520 736f 7572 6365 2063 6f64  ..the source cod
-00003c50: 6520 6e65 6564 6564 2074 6f20 6765 6e65  e needed to gene
-00003c60: 7261 7465 2c20 696e 7374 616c 6c2c 2061  rate, install, a
-00003c70: 6e64 2028 666f 7220 616e 2065 7865 6375  nd (for an execu
-00003c80: 7461 626c 650d 0a77 6f72 6b29 2072 756e  table..work) run
-00003c90: 2074 6865 206f 626a 6563 7420 636f 6465   the object code
-00003ca0: 2061 6e64 2074 6f20 6d6f 6469 6679 2074   and to modify t
-00003cb0: 6865 2077 6f72 6b2c 2069 6e63 6c75 6469  he work, includi
-00003cc0: 6e67 2073 6372 6970 7473 2074 6f0d 0a63  ng scripts to..c
-00003cd0: 6f6e 7472 6f6c 2074 686f 7365 2061 6374  ontrol those act
-00003ce0: 6976 6974 6965 732e 2020 486f 7765 7665  ivities.  Howeve
-00003cf0: 722c 2069 7420 646f 6573 206e 6f74 2069  r, it does not i
-00003d00: 6e63 6c75 6465 2074 6865 2077 6f72 6b27  nclude the work'
-00003d10: 730d 0a53 7973 7465 6d20 4c69 6272 6172  s..System Librar
-00003d20: 6965 732c 206f 7220 6765 6e65 7261 6c2d  ies, or general-
-00003d30: 7075 7270 6f73 6520 746f 6f6c 7320 6f72  purpose tools or
-00003d40: 2067 656e 6572 616c 6c79 2061 7661 696c   generally avail
-00003d50: 6162 6c65 2066 7265 650d 0a70 726f 6772  able free..progr
-00003d60: 616d 7320 7768 6963 6820 6172 6520 7573  ams which are us
-00003d70: 6564 2075 6e6d 6f64 6966 6965 6420 696e  ed unmodified in
-00003d80: 2070 6572 666f 726d 696e 6720 7468 6f73   performing thos
-00003d90: 6520 6163 7469 7669 7469 6573 2062 7574  e activities but
-00003da0: 0d0a 7768 6963 6820 6172 6520 6e6f 7420  ..which are not 
-00003db0: 7061 7274 206f 6620 7468 6520 776f 726b  part of the work
-00003dc0: 2e20 2046 6f72 2065 7861 6d70 6c65 2c20  .  For example, 
-00003dd0: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
-00003de0: 7572 6365 0d0a 696e 636c 7564 6573 2069  urce..includes i
-00003df0: 6e74 6572 6661 6365 2064 6566 696e 6974  nterface definit
-00003e00: 696f 6e20 6669 6c65 7320 6173 736f 6369  ion files associ
-00003e10: 6174 6564 2077 6974 6820 736f 7572 6365  ated with source
-00003e20: 2066 696c 6573 2066 6f72 0d0a 7468 6520   files for..the 
-00003e30: 776f 726b 2c20 616e 6420 7468 6520 736f  work, and the so
-00003e40: 7572 6365 2063 6f64 6520 666f 7220 7368  urce code for sh
-00003e50: 6172 6564 206c 6962 7261 7269 6573 2061  ared libraries a
-00003e60: 6e64 2064 796e 616d 6963 616c 6c79 0d0a  nd dynamically..
-00003e70: 6c69 6e6b 6564 2073 7562 7072 6f67 7261  linked subprogra
-00003e80: 6d73 2074 6861 7420 7468 6520 776f 726b  ms that the work
-00003e90: 2069 7320 7370 6563 6966 6963 616c 6c79   is specifically
-00003ea0: 2064 6573 6967 6e65 6420 746f 2072 6571   designed to req
-00003eb0: 7569 7265 2c0d 0a73 7563 6820 6173 2062  uire,..such as b
-00003ec0: 7920 696e 7469 6d61 7465 2064 6174 6120  y intimate data 
-00003ed0: 636f 6d6d 756e 6963 6174 696f 6e20 6f72  communication or
-00003ee0: 2063 6f6e 7472 6f6c 2066 6c6f 7720 6265   control flow be
-00003ef0: 7477 6565 6e20 7468 6f73 650d 0a73 7562  tween those..sub
-00003f00: 7072 6f67 7261 6d73 2061 6e64 206f 7468  programs and oth
-00003f10: 6572 2070 6172 7473 206f 6620 7468 6520  er parts of the 
-00003f20: 776f 726b 2e0d 0a0d 0a20 2054 6865 2043  work.....  The C
-00003f30: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
-00003f40: 7263 6520 6e65 6564 206e 6f74 2069 6e63  rce need not inc
-00003f50: 6c75 6465 2061 6e79 7468 696e 6720 7468  lude anything th
-00003f60: 6174 2075 7365 7273 0d0a 6361 6e20 7265  at users..can re
-00003f70: 6765 6e65 7261 7465 2061 7574 6f6d 6174  generate automat
-00003f80: 6963 616c 6c79 2066 726f 6d20 6f74 6865  ically from othe
-00003f90: 7220 7061 7274 7320 6f66 2074 6865 2043  r parts of the C
-00003fa0: 6f72 7265 7370 6f6e 6469 6e67 0d0a 536f  orresponding..So
-00003fb0: 7572 6365 2e0d 0a0d 0a20 2054 6865 2043  urce.....  The C
-00003fc0: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
-00003fd0: 7263 6520 666f 7220 6120 776f 726b 2069  rce for a work i
-00003fe0: 6e20 736f 7572 6365 2063 6f64 6520 666f  n source code fo
-00003ff0: 726d 2069 7320 7468 6174 0d0a 7361 6d65  rm is that..same
-00004000: 2077 6f72 6b2e 0d0a 0d0a 2020 322e 2042   work.....  2. B
-00004010: 6173 6963 2050 6572 6d69 7373 696f 6e73  asic Permissions
-00004020: 2e0d 0a0d 0a20 2041 6c6c 2072 6967 6874  .....  All right
-00004030: 7320 6772 616e 7465 6420 756e 6465 7220  s granted under 
-00004040: 7468 6973 204c 6963 656e 7365 2061 7265  this License are
-00004050: 2067 7261 6e74 6564 2066 6f72 2074 6865   granted for the
-00004060: 2074 6572 6d20 6f66 0d0a 636f 7079 7269   term of..copyri
-00004070: 6768 7420 6f6e 2074 6865 2050 726f 6772  ght on the Progr
-00004080: 616d 2c20 616e 6420 6172 6520 6972 7265  am, and are irre
-00004090: 766f 6361 626c 6520 7072 6f76 6964 6564  vocable provided
-000040a0: 2074 6865 2073 7461 7465 640d 0a63 6f6e   the stated..con
-000040b0: 6469 7469 6f6e 7320 6172 6520 6d65 742e  ditions are met.
-000040c0: 2020 5468 6973 204c 6963 656e 7365 2065    This License e
-000040d0: 7870 6c69 6369 746c 7920 6166 6669 726d  xplicitly affirm
-000040e0: 7320 796f 7572 2075 6e6c 696d 6974 6564  s your unlimited
-000040f0: 0d0a 7065 726d 6973 7369 6f6e 2074 6f20  ..permission to 
-00004100: 7275 6e20 7468 6520 756e 6d6f 6469 6669  run the unmodifi
-00004110: 6564 2050 726f 6772 616d 2e20 2054 6865  ed Program.  The
-00004120: 206f 7574 7075 7420 6672 6f6d 2072 756e   output from run
-00004130: 6e69 6e67 2061 0d0a 636f 7665 7265 6420  ning a..covered 
-00004140: 776f 726b 2069 7320 636f 7665 7265 6420  work is covered 
-00004150: 6279 2074 6869 7320 4c69 6365 6e73 6520  by this License 
-00004160: 6f6e 6c79 2069 6620 7468 6520 6f75 7470  only if the outp
-00004170: 7574 2c20 6769 7665 6e20 6974 730d 0a63  ut, given its..c
-00004180: 6f6e 7465 6e74 2c20 636f 6e73 7469 7475  ontent, constitu
-00004190: 7465 7320 6120 636f 7665 7265 6420 776f  tes a covered wo
-000041a0: 726b 2e20 2054 6869 7320 4c69 6365 6e73  rk.  This Licens
-000041b0: 6520 6163 6b6e 6f77 6c65 6467 6573 2079  e acknowledges y
-000041c0: 6f75 720d 0a72 6967 6874 7320 6f66 2066  our..rights of f
-000041d0: 6169 7220 7573 6520 6f72 206f 7468 6572  air use or other
-000041e0: 2065 7175 6976 616c 656e 742c 2061 7320   equivalent, as 
-000041f0: 7072 6f76 6964 6564 2062 7920 636f 7079  provided by copy
-00004200: 7269 6768 7420 6c61 772e 0d0a 0d0a 2020  right law.....  
-00004210: 596f 7520 6d61 7920 6d61 6b65 2c20 7275  You may make, ru
-00004220: 6e20 616e 6420 7072 6f70 6167 6174 6520  n and propagate 
-00004230: 636f 7665 7265 6420 776f 726b 7320 7468  covered works th
-00004240: 6174 2079 6f75 2064 6f20 6e6f 740d 0a63  at you do not..c
-00004250: 6f6e 7665 792c 2077 6974 686f 7574 2063  onvey, without c
-00004260: 6f6e 6469 7469 6f6e 7320 736f 206c 6f6e  onditions so lon
-00004270: 6720 6173 2079 6f75 7220 6c69 6365 6e73  g as your licens
-00004280: 6520 6f74 6865 7277 6973 6520 7265 6d61  e otherwise rema
-00004290: 696e 730d 0a69 6e20 666f 7263 652e 2020  ins..in force.  
-000042a0: 596f 7520 6d61 7920 636f 6e76 6579 2063  You may convey c
-000042b0: 6f76 6572 6564 2077 6f72 6b73 2074 6f20  overed works to 
-000042c0: 6f74 6865 7273 2066 6f72 2074 6865 2073  others for the s
-000042d0: 6f6c 6520 7075 7270 6f73 650d 0a6f 6620  ole purpose..of 
-000042e0: 6861 7669 6e67 2074 6865 6d20 6d61 6b65  having them make
-000042f0: 206d 6f64 6966 6963 6174 696f 6e73 2065   modifications e
-00004300: 7863 6c75 7369 7665 6c79 2066 6f72 2079  xclusively for y
-00004310: 6f75 2c20 6f72 2070 726f 7669 6465 2079  ou, or provide y
-00004320: 6f75 0d0a 7769 7468 2066 6163 696c 6974  ou..with facilit
-00004330: 6965 7320 666f 7220 7275 6e6e 696e 6720  ies for running 
-00004340: 7468 6f73 6520 776f 726b 732c 2070 726f  those works, pro
-00004350: 7669 6465 6420 7468 6174 2079 6f75 2063  vided that you c
-00004360: 6f6d 706c 7920 7769 7468 0d0a 7468 6520  omply with..the 
-00004370: 7465 726d 7320 6f66 2074 6869 7320 4c69  terms of this Li
-00004380: 6365 6e73 6520 696e 2063 6f6e 7665 7969  cense in conveyi
-00004390: 6e67 2061 6c6c 206d 6174 6572 6961 6c20  ng all material 
-000043a0: 666f 7220 7768 6963 6820 796f 7520 646f  for which you do
-000043b0: 0d0a 6e6f 7420 636f 6e74 726f 6c20 636f  ..not control co
-000043c0: 7079 7269 6768 742e 2020 5468 6f73 6520  pyright.  Those 
-000043d0: 7468 7573 206d 616b 696e 6720 6f72 2072  thus making or r
-000043e0: 756e 6e69 6e67 2074 6865 2063 6f76 6572  unning the cover
-000043f0: 6564 2077 6f72 6b73 0d0a 666f 7220 796f  ed works..for yo
-00004400: 7520 6d75 7374 2064 6f20 736f 2065 7863  u must do so exc
-00004410: 6c75 7369 7665 6c79 206f 6e20 796f 7572  lusively on your
-00004420: 2062 6568 616c 662c 2075 6e64 6572 2079   behalf, under y
-00004430: 6f75 7220 6469 7265 6374 696f 6e0d 0a61  our direction..a
-00004440: 6e64 2063 6f6e 7472 6f6c 2c20 6f6e 2074  nd control, on t
-00004450: 6572 6d73 2074 6861 7420 7072 6f68 6962  erms that prohib
-00004460: 6974 2074 6865 6d20 6672 6f6d 206d 616b  it them from mak
-00004470: 696e 6720 616e 7920 636f 7069 6573 206f  ing any copies o
-00004480: 660d 0a79 6f75 7220 636f 7079 7269 6768  f..your copyrigh
-00004490: 7465 6420 6d61 7465 7269 616c 206f 7574  ted material out
-000044a0: 7369 6465 2074 6865 6972 2072 656c 6174  side their relat
-000044b0: 696f 6e73 6869 7020 7769 7468 2079 6f75  ionship with you
-000044c0: 2e0d 0a0d 0a20 2043 6f6e 7665 7969 6e67  .....  Conveying
-000044d0: 2075 6e64 6572 2061 6e79 206f 7468 6572   under any other
-000044e0: 2063 6972 6375 6d73 7461 6e63 6573 2069   circumstances i
-000044f0: 7320 7065 726d 6974 7465 6420 736f 6c65  s permitted sole
-00004500: 6c79 2075 6e64 6572 0d0a 7468 6520 636f  ly under..the co
-00004510: 6e64 6974 696f 6e73 2073 7461 7465 6420  nditions stated 
-00004520: 6265 6c6f 772e 2020 5375 626c 6963 656e  below.  Sublicen
-00004530: 7369 6e67 2069 7320 6e6f 7420 616c 6c6f  sing is not allo
-00004540: 7765 643b 2073 6563 7469 6f6e 2031 300d  wed; section 10.
-00004550: 0a6d 616b 6573 2069 7420 756e 6e65 6365  .makes it unnece
-00004560: 7373 6172 792e 0d0a 0d0a 2020 332e 2050  ssary.....  3. P
-00004570: 726f 7465 6374 696e 6720 5573 6572 7327  rotecting Users'
-00004580: 204c 6567 616c 2052 6967 6874 7320 4672   Legal Rights Fr
-00004590: 6f6d 2041 6e74 692d 4369 7263 756d 7665  om Anti-Circumve
-000045a0: 6e74 696f 6e20 4c61 772e 0d0a 0d0a 2020  ntion Law.....  
-000045b0: 4e6f 2063 6f76 6572 6564 2077 6f72 6b20  No covered work 
-000045c0: 7368 616c 6c20 6265 2064 6565 6d65 6420  shall be deemed 
-000045d0: 7061 7274 206f 6620 616e 2065 6666 6563  part of an effec
-000045e0: 7469 7665 2074 6563 686e 6f6c 6f67 6963  tive technologic
-000045f0: 616c 0d0a 6d65 6173 7572 6520 756e 6465  al..measure unde
-00004600: 7220 616e 7920 6170 706c 6963 6162 6c65  r any applicable
-00004610: 206c 6177 2066 756c 6669 6c6c 696e 6720   law fulfilling 
-00004620: 6f62 6c69 6761 7469 6f6e 7320 756e 6465  obligations unde
-00004630: 7220 6172 7469 636c 650d 0a31 3120 6f66  r article..11 of
-00004640: 2074 6865 2057 4950 4f20 636f 7079 7269   the WIPO copyri
-00004650: 6768 7420 7472 6561 7479 2061 646f 7074  ght treaty adopt
-00004660: 6564 206f 6e20 3230 2044 6563 656d 6265  ed on 20 Decembe
-00004670: 7220 3139 3936 2c20 6f72 0d0a 7369 6d69  r 1996, or..simi
-00004680: 6c61 7220 6c61 7773 2070 726f 6869 6269  lar laws prohibi
-00004690: 7469 6e67 206f 7220 7265 7374 7269 6374  ting or restrict
-000046a0: 696e 6720 6369 7263 756d 7665 6e74 696f  ing circumventio
-000046b0: 6e20 6f66 2073 7563 680d 0a6d 6561 7375  n of such..measu
-000046c0: 7265 732e 0d0a 0d0a 2020 5768 656e 2079  res.....  When y
-000046d0: 6f75 2063 6f6e 7665 7920 6120 636f 7665  ou convey a cove
-000046e0: 7265 6420 776f 726b 2c20 796f 7520 7761  red work, you wa
-000046f0: 6976 6520 616e 7920 6c65 6761 6c20 706f  ive any legal po
-00004700: 7765 7220 746f 2066 6f72 6269 640d 0a63  wer to forbid..c
-00004710: 6972 6375 6d76 656e 7469 6f6e 206f 6620  ircumvention of 
-00004720: 7465 6368 6e6f 6c6f 6769 6361 6c20 6d65  technological me
-00004730: 6173 7572 6573 2074 6f20 7468 6520 6578  asures to the ex
-00004740: 7465 6e74 2073 7563 6820 6369 7263 756d  tent such circum
-00004750: 7665 6e74 696f 6e0d 0a69 7320 6566 6665  vention..is effe
-00004760: 6374 6564 2062 7920 6578 6572 6369 7369  cted by exercisi
-00004770: 6e67 2072 6967 6874 7320 756e 6465 7220  ng rights under 
-00004780: 7468 6973 204c 6963 656e 7365 2077 6974  this License wit
-00004790: 6820 7265 7370 6563 7420 746f 0d0a 7468  h respect to..th
-000047a0: 6520 636f 7665 7265 6420 776f 726b 2c20  e covered work, 
-000047b0: 616e 6420 796f 7520 6469 7363 6c61 696d  and you disclaim
-000047c0: 2061 6e79 2069 6e74 656e 7469 6f6e 2074   any intention t
-000047d0: 6f20 6c69 6d69 7420 6f70 6572 6174 696f  o limit operatio
-000047e0: 6e20 6f72 0d0a 6d6f 6469 6669 6361 7469  n or..modificati
-000047f0: 6f6e 206f 6620 7468 6520 776f 726b 2061  on of the work a
-00004800: 7320 6120 6d65 616e 7320 6f66 2065 6e66  s a means of enf
-00004810: 6f72 6369 6e67 2c20 6167 6169 6e73 7420  orcing, against 
-00004820: 7468 6520 776f 726b 2773 0d0a 7573 6572  the work's..user
-00004830: 732c 2079 6f75 7220 6f72 2074 6869 7264  s, your or third
-00004840: 2070 6172 7469 6573 2720 6c65 6761 6c20   parties' legal 
-00004850: 7269 6768 7473 2074 6f20 666f 7262 6964  rights to forbid
-00004860: 2063 6972 6375 6d76 656e 7469 6f6e 206f   circumvention o
-00004870: 660d 0a74 6563 686e 6f6c 6f67 6963 616c  f..technological
-00004880: 206d 6561 7375 7265 732e 0d0a 0d0a 2020   measures.....  
-00004890: 342e 2043 6f6e 7665 7969 6e67 2056 6572  4. Conveying Ver
-000048a0: 6261 7469 6d20 436f 7069 6573 2e0d 0a0d  batim Copies....
-000048b0: 0a20 2059 6f75 206d 6179 2063 6f6e 7665  .  You may conve
-000048c0: 7920 7665 7262 6174 696d 2063 6f70 6965  y verbatim copie
-000048d0: 7320 6f66 2074 6865 2050 726f 6772 616d  s of the Program
-000048e0: 2773 2073 6f75 7263 6520 636f 6465 2061  's source code a
-000048f0: 7320 796f 750d 0a72 6563 6569 7665 2069  s you..receive i
-00004900: 742c 2069 6e20 616e 7920 6d65 6469 756d  t, in any medium
-00004910: 2c20 7072 6f76 6964 6564 2074 6861 7420  , provided that 
-00004920: 796f 7520 636f 6e73 7069 6375 6f75 736c  you conspicuousl
-00004930: 7920 616e 640d 0a61 7070 726f 7072 6961  y and..appropria
-00004940: 7465 6c79 2070 7562 6c69 7368 206f 6e20  tely publish on 
-00004950: 6561 6368 2063 6f70 7920 616e 2061 7070  each copy an app
-00004960: 726f 7072 6961 7465 2063 6f70 7972 6967  ropriate copyrig
-00004970: 6874 206e 6f74 6963 653b 0d0a 6b65 6570  ht notice;..keep
-00004980: 2069 6e74 6163 7420 616c 6c20 6e6f 7469   intact all noti
-00004990: 6365 7320 7374 6174 696e 6720 7468 6174  ces stating that
-000049a0: 2074 6869 7320 4c69 6365 6e73 6520 616e   this License an
-000049b0: 6420 616e 790d 0a6e 6f6e 2d70 6572 6d69  d any..non-permi
-000049c0: 7373 6976 6520 7465 726d 7320 6164 6465  ssive terms adde
-000049d0: 6420 696e 2061 6363 6f72 6420 7769 7468  d in accord with
-000049e0: 2073 6563 7469 6f6e 2037 2061 7070 6c79   section 7 apply
-000049f0: 2074 6f20 7468 6520 636f 6465 3b0d 0a6b   to the code;..k
-00004a00: 6565 7020 696e 7461 6374 2061 6c6c 206e  eep intact all n
-00004a10: 6f74 6963 6573 206f 6620 7468 6520 6162  otices of the ab
-00004a20: 7365 6e63 6520 6f66 2061 6e79 2077 6172  sence of any war
-00004a30: 7261 6e74 793b 2061 6e64 2067 6976 6520  ranty; and give 
-00004a40: 616c 6c0d 0a72 6563 6970 6965 6e74 7320  all..recipients 
-00004a50: 6120 636f 7079 206f 6620 7468 6973 204c  a copy of this L
-00004a60: 6963 656e 7365 2061 6c6f 6e67 2077 6974  icense along wit
-00004a70: 6820 7468 6520 5072 6f67 7261 6d2e 0d0a  h the Program...
-00004a80: 0d0a 2020 596f 7520 6d61 7920 6368 6172  ..  You may char
-00004a90: 6765 2061 6e79 2070 7269 6365 206f 7220  ge any price or 
-00004aa0: 6e6f 2070 7269 6365 2066 6f72 2065 6163  no price for eac
-00004ab0: 6820 636f 7079 2074 6861 7420 796f 7520  h copy that you 
-00004ac0: 636f 6e76 6579 2c0d 0a61 6e64 2079 6f75  convey,..and you
-00004ad0: 206d 6179 206f 6666 6572 2073 7570 706f   may offer suppo
-00004ae0: 7274 206f 7220 7761 7272 616e 7479 2070  rt or warranty p
-00004af0: 726f 7465 6374 696f 6e20 666f 7220 6120  rotection for a 
-00004b00: 6665 652e 0d0a 0d0a 2020 352e 2043 6f6e  fee.....  5. Con
-00004b10: 7665 7969 6e67 204d 6f64 6966 6965 6420  veying Modified 
-00004b20: 536f 7572 6365 2056 6572 7369 6f6e 732e  Source Versions.
-00004b30: 0d0a 0d0a 2020 596f 7520 6d61 7920 636f  ....  You may co
-00004b40: 6e76 6579 2061 2077 6f72 6b20 6261 7365  nvey a work base
-00004b50: 6420 6f6e 2074 6865 2050 726f 6772 616d  d on the Program
-00004b60: 2c20 6f72 2074 6865 206d 6f64 6966 6963  , or the modific
-00004b70: 6174 696f 6e73 2074 6f0d 0a70 726f 6475  ations to..produ
-00004b80: 6365 2069 7420 6672 6f6d 2074 6865 2050  ce it from the P
-00004b90: 726f 6772 616d 2c20 696e 2074 6865 2066  rogram, in the f
-00004ba0: 6f72 6d20 6f66 2073 6f75 7263 6520 636f  orm of source co
-00004bb0: 6465 2075 6e64 6572 2074 6865 0d0a 7465  de under the..te
-00004bc0: 726d 7320 6f66 2073 6563 7469 6f6e 2034  rms of section 4
-00004bd0: 2c20 7072 6f76 6964 6564 2074 6861 7420  , provided that 
-00004be0: 796f 7520 616c 736f 206d 6565 7420 616c  you also meet al
-00004bf0: 6c20 6f66 2074 6865 7365 2063 6f6e 6469  l of these condi
-00004c00: 7469 6f6e 733a 0d0a 0d0a 2020 2020 6129  tions:....    a)
-00004c10: 2054 6865 2077 6f72 6b20 6d75 7374 2063   The work must c
-00004c20: 6172 7279 2070 726f 6d69 6e65 6e74 206e  arry prominent n
-00004c30: 6f74 6963 6573 2073 7461 7469 6e67 2074  otices stating t
-00004c40: 6861 7420 796f 7520 6d6f 6469 6669 6564  hat you modified
-00004c50: 0d0a 2020 2020 6974 2c20 616e 6420 6769  ..    it, and gi
-00004c60: 7669 6e67 2061 2072 656c 6576 616e 7420  ving a relevant 
-00004c70: 6461 7465 2e0d 0a0d 0a20 2020 2062 2920  date.....    b) 
-00004c80: 5468 6520 776f 726b 206d 7573 7420 6361  The work must ca
-00004c90: 7272 7920 7072 6f6d 696e 656e 7420 6e6f  rry prominent no
-00004ca0: 7469 6365 7320 7374 6174 696e 6720 7468  tices stating th
-00004cb0: 6174 2069 7420 6973 0d0a 2020 2020 7265  at it is..    re
-00004cc0: 6c65 6173 6564 2075 6e64 6572 2074 6869  leased under thi
-00004cd0: 7320 4c69 6365 6e73 6520 616e 6420 616e  s License and an
-00004ce0: 7920 636f 6e64 6974 696f 6e73 2061 6464  y conditions add
-00004cf0: 6564 2075 6e64 6572 2073 6563 7469 6f6e  ed under section
-00004d00: 0d0a 2020 2020 372e 2020 5468 6973 2072  ..    7.  This r
-00004d10: 6571 7569 7265 6d65 6e74 206d 6f64 6966  equirement modif
-00004d20: 6965 7320 7468 6520 7265 7175 6972 656d  ies the requirem
-00004d30: 656e 7420 696e 2073 6563 7469 6f6e 2034  ent in section 4
-00004d40: 2074 6f0d 0a20 2020 2022 6b65 6570 2069   to..    "keep i
-00004d50: 6e74 6163 7420 616c 6c20 6e6f 7469 6365  ntact all notice
-00004d60: 7322 2e0d 0a0d 0a20 2020 2063 2920 596f  s".....    c) Yo
-00004d70: 7520 6d75 7374 206c 6963 656e 7365 2074  u must license t
-00004d80: 6865 2065 6e74 6972 6520 776f 726b 2c20  he entire work, 
-00004d90: 6173 2061 2077 686f 6c65 2c20 756e 6465  as a whole, unde
-00004da0: 7220 7468 6973 0d0a 2020 2020 4c69 6365  r this..    Lice
-00004db0: 6e73 6520 746f 2061 6e79 6f6e 6520 7768  nse to anyone wh
-00004dc0: 6f20 636f 6d65 7320 696e 746f 2070 6f73  o comes into pos
-00004dd0: 7365 7373 696f 6e20 6f66 2061 2063 6f70  session of a cop
-00004de0: 792e 2020 5468 6973 0d0a 2020 2020 4c69  y.  This..    Li
-00004df0: 6365 6e73 6520 7769 6c6c 2074 6865 7265  cense will there
-00004e00: 666f 7265 2061 7070 6c79 2c20 616c 6f6e  fore apply, alon
-00004e10: 6720 7769 7468 2061 6e79 2061 7070 6c69  g with any appli
-00004e20: 6361 626c 6520 7365 6374 696f 6e20 370d  cable section 7.
-00004e30: 0a20 2020 2061 6464 6974 696f 6e61 6c20  .    additional 
-00004e40: 7465 726d 732c 2074 6f20 7468 6520 7768  terms, to the wh
-00004e50: 6f6c 6520 6f66 2074 6865 2077 6f72 6b2c  ole of the work,
-00004e60: 2061 6e64 2061 6c6c 2069 7473 2070 6172   and all its par
-00004e70: 7473 2c0d 0a20 2020 2072 6567 6172 646c  ts,..    regardl
-00004e80: 6573 7320 6f66 2068 6f77 2074 6865 7920  ess of how they 
-00004e90: 6172 6520 7061 636b 6167 6564 2e20 2054  are packaged.  T
-00004ea0: 6869 7320 4c69 6365 6e73 6520 6769 7665  his License give
-00004eb0: 7320 6e6f 0d0a 2020 2020 7065 726d 6973  s no..    permis
-00004ec0: 7369 6f6e 2074 6f20 6c69 6365 6e73 6520  sion to license 
-00004ed0: 7468 6520 776f 726b 2069 6e20 616e 7920  the work in any 
-00004ee0: 6f74 6865 7220 7761 792c 2062 7574 2069  other way, but i
-00004ef0: 7420 646f 6573 206e 6f74 0d0a 2020 2020  t does not..    
-00004f00: 696e 7661 6c69 6461 7465 2073 7563 6820  invalidate such 
-00004f10: 7065 726d 6973 7369 6f6e 2069 6620 796f  permission if yo
-00004f20: 7520 6861 7665 2073 6570 6172 6174 656c  u have separatel
-00004f30: 7920 7265 6365 6976 6564 2069 742e 0d0a  y received it...
-00004f40: 0d0a 2020 2020 6429 2049 6620 7468 6520  ..    d) If the 
-00004f50: 776f 726b 2068 6173 2069 6e74 6572 6163  work has interac
-00004f60: 7469 7665 2075 7365 7220 696e 7465 7266  tive user interf
-00004f70: 6163 6573 2c20 6561 6368 206d 7573 7420  aces, each must 
-00004f80: 6469 7370 6c61 790d 0a20 2020 2041 7070  display..    App
-00004f90: 726f 7072 6961 7465 204c 6567 616c 204e  ropriate Legal N
-00004fa0: 6f74 6963 6573 3b20 686f 7765 7665 722c  otices; however,
-00004fb0: 2069 6620 7468 6520 5072 6f67 7261 6d20   if the Program 
-00004fc0: 6861 7320 696e 7465 7261 6374 6976 650d  has interactive.
-00004fd0: 0a20 2020 2069 6e74 6572 6661 6365 7320  .    interfaces 
-00004fe0: 7468 6174 2064 6f20 6e6f 7420 6469 7370  that do not disp
-00004ff0: 6c61 7920 4170 7072 6f70 7269 6174 6520  lay Appropriate 
-00005000: 4c65 6761 6c20 4e6f 7469 6365 732c 2079  Legal Notices, y
-00005010: 6f75 720d 0a20 2020 2077 6f72 6b20 6e65  our..    work ne
-00005020: 6564 206e 6f74 206d 616b 6520 7468 656d  ed not make them
-00005030: 2064 6f20 736f 2e0d 0a0d 0a20 2041 2063   do so.....  A c
-00005040: 6f6d 7069 6c61 7469 6f6e 206f 6620 6120  ompilation of a 
-00005050: 636f 7665 7265 6420 776f 726b 2077 6974  covered work wit
-00005060: 6820 6f74 6865 7220 7365 7061 7261 7465  h other separate
-00005070: 2061 6e64 2069 6e64 6570 656e 6465 6e74   and independent
-00005080: 0d0a 776f 726b 732c 2077 6869 6368 2061  ..works, which a
-00005090: 7265 206e 6f74 2062 7920 7468 6569 7220  re not by their 
-000050a0: 6e61 7475 7265 2065 7874 656e 7369 6f6e  nature extension
-000050b0: 7320 6f66 2074 6865 2063 6f76 6572 6564  s of the covered
-000050c0: 2077 6f72 6b2c 0d0a 616e 6420 7768 6963   work,..and whic
-000050d0: 6820 6172 6520 6e6f 7420 636f 6d62 696e  h are not combin
-000050e0: 6564 2077 6974 6820 6974 2073 7563 6820  ed with it such 
-000050f0: 6173 2074 6f20 666f 726d 2061 206c 6172  as to form a lar
-00005100: 6765 7220 7072 6f67 7261 6d2c 0d0a 696e  ger program,..in
-00005110: 206f 7220 6f6e 2061 2076 6f6c 756d 6520   or on a volume 
-00005120: 6f66 2061 2073 746f 7261 6765 206f 7220  of a storage or 
-00005130: 6469 7374 7269 6275 7469 6f6e 206d 6564  distribution med
-00005140: 6975 6d2c 2069 7320 6361 6c6c 6564 2061  ium, is called a
-00005150: 6e0d 0a22 6167 6772 6567 6174 6522 2069  n.."aggregate" i
-00005160: 6620 7468 6520 636f 6d70 696c 6174 696f  f the compilatio
-00005170: 6e20 616e 6420 6974 7320 7265 7375 6c74  n and its result
-00005180: 696e 6720 636f 7079 7269 6768 7420 6172  ing copyright ar
-00005190: 6520 6e6f 740d 0a75 7365 6420 746f 206c  e not..used to l
-000051a0: 696d 6974 2074 6865 2061 6363 6573 7320  imit the access 
-000051b0: 6f72 206c 6567 616c 2072 6967 6874 7320  or legal rights 
-000051c0: 6f66 2074 6865 2063 6f6d 7069 6c61 7469  of the compilati
-000051d0: 6f6e 2773 2075 7365 7273 0d0a 6265 796f  on's users..beyo
-000051e0: 6e64 2077 6861 7420 7468 6520 696e 6469  nd what the indi
-000051f0: 7669 6475 616c 2077 6f72 6b73 2070 6572  vidual works per
-00005200: 6d69 742e 2020 496e 636c 7573 696f 6e20  mit.  Inclusion 
-00005210: 6f66 2061 2063 6f76 6572 6564 2077 6f72  of a covered wor
-00005220: 6b0d 0a69 6e20 616e 2061 6767 7265 6761  k..in an aggrega
-00005230: 7465 2064 6f65 7320 6e6f 7420 6361 7573  te does not caus
-00005240: 6520 7468 6973 204c 6963 656e 7365 2074  e this License t
-00005250: 6f20 6170 706c 7920 746f 2074 6865 206f  o apply to the o
-00005260: 7468 6572 0d0a 7061 7274 7320 6f66 2074  ther..parts of t
-00005270: 6865 2061 6767 7265 6761 7465 2e0d 0a0d  he aggregate....
-00005280: 0a20 2036 2e20 436f 6e76 6579 696e 6720  .  6. Conveying 
-00005290: 4e6f 6e2d 536f 7572 6365 2046 6f72 6d73  Non-Source Forms
-000052a0: 2e0d 0a0d 0a20 2059 6f75 206d 6179 2063  .....  You may c
-000052b0: 6f6e 7665 7920 6120 636f 7665 7265 6420  onvey a covered 
-000052c0: 776f 726b 2069 6e20 6f62 6a65 6374 2063  work in object c
-000052d0: 6f64 6520 666f 726d 2075 6e64 6572 2074  ode form under t
-000052e0: 6865 2074 6572 6d73 0d0a 6f66 2073 6563  he terms..of sec
-000052f0: 7469 6f6e 7320 3420 616e 6420 352c 2070  tions 4 and 5, p
-00005300: 726f 7669 6465 6420 7468 6174 2079 6f75  rovided that you
-00005310: 2061 6c73 6f20 636f 6e76 6579 2074 6865   also convey the
-00005320: 0d0a 6d61 6368 696e 652d 7265 6164 6162  ..machine-readab
-00005330: 6c65 2043 6f72 7265 7370 6f6e 6469 6e67  le Corresponding
-00005340: 2053 6f75 7263 6520 756e 6465 7220 7468   Source under th
-00005350: 6520 7465 726d 7320 6f66 2074 6869 7320  e terms of this 
-00005360: 4c69 6365 6e73 652c 0d0a 696e 206f 6e65  License,..in one
-00005370: 206f 6620 7468 6573 6520 7761 7973 3a0d   of these ways:.
-00005380: 0a0d 0a20 2020 2061 2920 436f 6e76 6579  ...    a) Convey
-00005390: 2074 6865 206f 626a 6563 7420 636f 6465   the object code
-000053a0: 2069 6e2c 206f 7220 656d 626f 6469 6564   in, or embodied
-000053b0: 2069 6e2c 2061 2070 6879 7369 6361 6c20   in, a physical 
-000053c0: 7072 6f64 7563 740d 0a20 2020 2028 696e  product..    (in
-000053d0: 636c 7564 696e 6720 6120 7068 7973 6963  cluding a physic
-000053e0: 616c 2064 6973 7472 6962 7574 696f 6e20  al distribution 
-000053f0: 6d65 6469 756d 292c 2061 6363 6f6d 7061  medium), accompa
-00005400: 6e69 6564 2062 7920 7468 650d 0a20 2020  nied by the..   
-00005410: 2043 6f72 7265 7370 6f6e 6469 6e67 2053   Corresponding S
-00005420: 6f75 7263 6520 6669 7865 6420 6f6e 2061  ource fixed on a
-00005430: 2064 7572 6162 6c65 2070 6879 7369 6361   durable physica
-00005440: 6c20 6d65 6469 756d 0d0a 2020 2020 6375  l medium..    cu
-00005450: 7374 6f6d 6172 696c 7920 7573 6564 2066  stomarily used f
-00005460: 6f72 2073 6f66 7477 6172 6520 696e 7465  or software inte
-00005470: 7263 6861 6e67 652e 0d0a 0d0a 2020 2020  rchange.....    
-00005480: 6229 2043 6f6e 7665 7920 7468 6520 6f62  b) Convey the ob
-00005490: 6a65 6374 2063 6f64 6520 696e 2c20 6f72  ject code in, or
-000054a0: 2065 6d62 6f64 6965 6420 696e 2c20 6120   embodied in, a 
-000054b0: 7068 7973 6963 616c 2070 726f 6475 6374  physical product
-000054c0: 0d0a 2020 2020 2869 6e63 6c75 6469 6e67  ..    (including
-000054d0: 2061 2070 6879 7369 6361 6c20 6469 7374   a physical dist
-000054e0: 7269 6275 7469 6f6e 206d 6564 6975 6d29  ribution medium)
-000054f0: 2c20 6163 636f 6d70 616e 6965 6420 6279  , accompanied by
-00005500: 2061 0d0a 2020 2020 7772 6974 7465 6e20   a..    written 
-00005510: 6f66 6665 722c 2076 616c 6964 2066 6f72  offer, valid for
-00005520: 2061 7420 6c65 6173 7420 7468 7265 6520   at least three 
-00005530: 7965 6172 7320 616e 6420 7661 6c69 6420  years and valid 
-00005540: 666f 7220 6173 0d0a 2020 2020 6c6f 6e67  for as..    long
-00005550: 2061 7320 796f 7520 6f66 6665 7220 7370   as you offer sp
-00005560: 6172 6520 7061 7274 7320 6f72 2063 7573  are parts or cus
-00005570: 746f 6d65 7220 7375 7070 6f72 7420 666f  tomer support fo
-00005580: 7220 7468 6174 2070 726f 6475 6374 0d0a  r that product..
-00005590: 2020 2020 6d6f 6465 6c2c 2074 6f20 6769      model, to gi
-000055a0: 7665 2061 6e79 6f6e 6520 7768 6f20 706f  ve anyone who po
-000055b0: 7373 6573 7365 7320 7468 6520 6f62 6a65  ssesses the obje
-000055c0: 6374 2063 6f64 6520 6569 7468 6572 2028  ct code either (
-000055d0: 3129 2061 0d0a 2020 2020 636f 7079 206f  1) a..    copy o
-000055e0: 6620 7468 6520 436f 7272 6573 706f 6e64  f the Correspond
-000055f0: 696e 6720 536f 7572 6365 2066 6f72 2061  ing Source for a
-00005600: 6c6c 2074 6865 2073 6f66 7477 6172 6520  ll the software 
-00005610: 696e 2074 6865 0d0a 2020 2020 7072 6f64  in the..    prod
-00005620: 7563 7420 7468 6174 2069 7320 636f 7665  uct that is cove
-00005630: 7265 6420 6279 2074 6869 7320 4c69 6365  red by this Lice
-00005640: 6e73 652c 206f 6e20 6120 6475 7261 626c  nse, on a durabl
-00005650: 6520 7068 7973 6963 616c 0d0a 2020 2020  e physical..    
-00005660: 6d65 6469 756d 2063 7573 746f 6d61 7269  medium customari
-00005670: 6c79 2075 7365 6420 666f 7220 736f 6674  ly used for soft
-00005680: 7761 7265 2069 6e74 6572 6368 616e 6765  ware interchange
-00005690: 2c20 666f 7220 6120 7072 6963 6520 6e6f  , for a price no
-000056a0: 0d0a 2020 2020 6d6f 7265 2074 6861 6e20  ..    more than 
-000056b0: 796f 7572 2072 6561 736f 6e61 626c 6520  your reasonable 
-000056c0: 636f 7374 206f 6620 7068 7973 6963 616c  cost of physical
-000056d0: 6c79 2070 6572 666f 726d 696e 6720 7468  ly performing th
-000056e0: 6973 0d0a 2020 2020 636f 6e76 6579 696e  is..    conveyin
-000056f0: 6720 6f66 2073 6f75 7263 652c 206f 7220  g of source, or 
-00005700: 2832 2920 6163 6365 7373 2074 6f20 636f  (2) access to co
-00005710: 7079 2074 6865 0d0a 2020 2020 436f 7272  py the..    Corr
-00005720: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
-00005730: 2066 726f 6d20 6120 6e65 7477 6f72 6b20   from a network 
-00005740: 7365 7276 6572 2061 7420 6e6f 2063 6861  server at no cha
-00005750: 7267 652e 0d0a 0d0a 2020 2020 6329 2043  rge.....    c) C
-00005760: 6f6e 7665 7920 696e 6469 7669 6475 616c  onvey individual
-00005770: 2063 6f70 6965 7320 6f66 2074 6865 206f   copies of the o
-00005780: 626a 6563 7420 636f 6465 2077 6974 6820  bject code with 
-00005790: 6120 636f 7079 206f 6620 7468 650d 0a20  a copy of the.. 
-000057a0: 2020 2077 7269 7474 656e 206f 6666 6572     written offer
-000057b0: 2074 6f20 7072 6f76 6964 6520 7468 6520   to provide the 
-000057c0: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
-000057d0: 7572 6365 2e20 2054 6869 730d 0a20 2020  urce.  This..   
-000057e0: 2061 6c74 6572 6e61 7469 7665 2069 7320   alternative is 
-000057f0: 616c 6c6f 7765 6420 6f6e 6c79 206f 6363  allowed only occ
-00005800: 6173 696f 6e61 6c6c 7920 616e 6420 6e6f  asionally and no
-00005810: 6e63 6f6d 6d65 7263 6961 6c6c 792c 2061  ncommercially, a
-00005820: 6e64 0d0a 2020 2020 6f6e 6c79 2069 6620  nd..    only if 
-00005830: 796f 7520 7265 6365 6976 6564 2074 6865  you received the
-00005840: 206f 626a 6563 7420 636f 6465 2077 6974   object code wit
-00005850: 6820 7375 6368 2061 6e20 6f66 6665 722c  h such an offer,
-00005860: 2069 6e20 6163 636f 7264 0d0a 2020 2020   in accord..    
-00005870: 7769 7468 2073 7562 7365 6374 696f 6e20  with subsection 
-00005880: 3662 2e0d 0a0d 0a20 2020 2064 2920 436f  6b.....    d) Co
-00005890: 6e76 6579 2074 6865 206f 626a 6563 7420  nvey the object 
-000058a0: 636f 6465 2062 7920 6f66 6665 7269 6e67  code by offering
-000058b0: 2061 6363 6573 7320 6672 6f6d 2061 2064   access from a d
-000058c0: 6573 6967 6e61 7465 640d 0a20 2020 2070  esignated..    p
-000058d0: 6c61 6365 2028 6772 6174 6973 206f 7220  lace (gratis or 
-000058e0: 666f 7220 6120 6368 6172 6765 292c 2061  for a charge), a
-000058f0: 6e64 206f 6666 6572 2065 7175 6976 616c  nd offer equival
-00005900: 656e 7420 6163 6365 7373 2074 6f20 7468  ent access to th
-00005910: 650d 0a20 2020 2043 6f72 7265 7370 6f6e  e..    Correspon
-00005920: 6469 6e67 2053 6f75 7263 6520 696e 2074  ding Source in t
-00005930: 6865 2073 616d 6520 7761 7920 7468 726f  he same way thro
-00005940: 7567 6820 7468 6520 7361 6d65 2070 6c61  ugh the same pla
-00005950: 6365 2061 7420 6e6f 0d0a 2020 2020 6675  ce at no..    fu
-00005960: 7274 6865 7220 6368 6172 6765 2e20 2059  rther charge.  Y
-00005970: 6f75 206e 6565 6420 6e6f 7420 7265 7175  ou need not requ
-00005980: 6972 6520 7265 6369 7069 656e 7473 2074  ire recipients t
-00005990: 6f20 636f 7079 2074 6865 0d0a 2020 2020  o copy the..    
-000059a0: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
-000059b0: 7572 6365 2061 6c6f 6e67 2077 6974 6820  urce along with 
-000059c0: 7468 6520 6f62 6a65 6374 2063 6f64 652e  the object code.
-000059d0: 2020 4966 2074 6865 2070 6c61 6365 2074    If the place t
-000059e0: 6f0d 0a20 2020 2063 6f70 7920 7468 6520  o..    copy the 
-000059f0: 6f62 6a65 6374 2063 6f64 6520 6973 2061  object code is a
-00005a00: 206e 6574 776f 726b 2073 6572 7665 722c   network server,
-00005a10: 2074 6865 2043 6f72 7265 7370 6f6e 6469   the Correspondi
-00005a20: 6e67 2053 6f75 7263 650d 0a20 2020 206d  ng Source..    m
-00005a30: 6179 2062 6520 6f6e 2061 2064 6966 6665  ay be on a diffe
-00005a40: 7265 6e74 2073 6572 7665 7220 286f 7065  rent server (ope
-00005a50: 7261 7465 6420 6279 2079 6f75 206f 7220  rated by you or 
-00005a60: 6120 7468 6972 6420 7061 7274 7929 0d0a  a third party)..
-00005a70: 2020 2020 7468 6174 2073 7570 706f 7274      that support
-00005a80: 7320 6571 7569 7661 6c65 6e74 2063 6f70  s equivalent cop
-00005a90: 7969 6e67 2066 6163 696c 6974 6965 732c  ying facilities,
-00005aa0: 2070 726f 7669 6465 6420 796f 7520 6d61   provided you ma
-00005ab0: 696e 7461 696e 0d0a 2020 2020 636c 6561  intain..    clea
-00005ac0: 7220 6469 7265 6374 696f 6e73 206e 6578  r directions nex
-00005ad0: 7420 746f 2074 6865 206f 626a 6563 7420  t to the object 
-00005ae0: 636f 6465 2073 6179 696e 6720 7768 6572  code saying wher
-00005af0: 6520 746f 2066 696e 6420 7468 650d 0a20  e to find the.. 
-00005b00: 2020 2043 6f72 7265 7370 6f6e 6469 6e67     Corresponding
-00005b10: 2053 6f75 7263 652e 2020 5265 6761 7264   Source.  Regard
-00005b20: 6c65 7373 206f 6620 7768 6174 2073 6572  less of what ser
-00005b30: 7665 7220 686f 7374 7320 7468 650d 0a20  ver hosts the.. 
-00005b40: 2020 2043 6f72 7265 7370 6f6e 6469 6e67     Corresponding
-00005b50: 2053 6f75 7263 652c 2079 6f75 2072 656d   Source, you rem
-00005b60: 6169 6e20 6f62 6c69 6761 7465 6420 746f  ain obligated to
-00005b70: 2065 6e73 7572 6520 7468 6174 2069 7420   ensure that it 
-00005b80: 6973 0d0a 2020 2020 6176 6169 6c61 626c  is..    availabl
-00005b90: 6520 666f 7220 6173 206c 6f6e 6720 6173  e for as long as
-00005ba0: 206e 6565 6465 6420 746f 2073 6174 6973   needed to satis
-00005bb0: 6679 2074 6865 7365 2072 6571 7569 7265  fy these require
-00005bc0: 6d65 6e74 732e 0d0a 0d0a 2020 2020 6529  ments.....    e)
-00005bd0: 2043 6f6e 7665 7920 7468 6520 6f62 6a65   Convey the obje
-00005be0: 6374 2063 6f64 6520 7573 696e 6720 7065  ct code using pe
-00005bf0: 6572 2d74 6f2d 7065 6572 2074 7261 6e73  er-to-peer trans
-00005c00: 6d69 7373 696f 6e2c 2070 726f 7669 6465  mission, provide
-00005c10: 640d 0a20 2020 2079 6f75 2069 6e66 6f72  d..    you infor
-00005c20: 6d20 6f74 6865 7220 7065 6572 7320 7768  m other peers wh
-00005c30: 6572 6520 7468 6520 6f62 6a65 6374 2063  ere the object c
-00005c40: 6f64 6520 616e 6420 436f 7272 6573 706f  ode and Correspo
-00005c50: 6e64 696e 670d 0a20 2020 2053 6f75 7263  nding..    Sourc
-00005c60: 6520 6f66 2074 6865 2077 6f72 6b20 6172  e of the work ar
-00005c70: 6520 6265 696e 6720 6f66 6665 7265 6420  e being offered 
-00005c80: 746f 2074 6865 2067 656e 6572 616c 2070  to the general p
-00005c90: 7562 6c69 6320 6174 206e 6f0d 0a20 2020  ublic at no..   
-00005ca0: 2063 6861 7267 6520 756e 6465 7220 7375   charge under su
-00005cb0: 6273 6563 7469 6f6e 2036 642e 0d0a 0d0a  bsection 6d.....
-00005cc0: 2020 4120 7365 7061 7261 626c 6520 706f    A separable po
-00005cd0: 7274 696f 6e20 6f66 2074 6865 206f 626a  rtion of the obj
-00005ce0: 6563 7420 636f 6465 2c20 7768 6f73 6520  ect code, whose 
-00005cf0: 736f 7572 6365 2063 6f64 6520 6973 2065  source code is e
-00005d00: 7863 6c75 6465 640d 0a66 726f 6d20 7468  xcluded..from th
-00005d10: 6520 436f 7272 6573 706f 6e64 696e 6720  e Corresponding 
-00005d20: 536f 7572 6365 2061 7320 6120 5379 7374  Source as a Syst
-00005d30: 656d 204c 6962 7261 7279 2c20 6e65 6564  em Library, need
-00005d40: 206e 6f74 2062 650d 0a69 6e63 6c75 6465   not be..include
-00005d50: 6420 696e 2063 6f6e 7665 7969 6e67 2074  d in conveying t
-00005d60: 6865 206f 626a 6563 7420 636f 6465 2077  he object code w
-00005d70: 6f72 6b2e 0d0a 0d0a 2020 4120 2255 7365  ork.....  A "Use
-00005d80: 7220 5072 6f64 7563 7422 2069 7320 6569  r Product" is ei
-00005d90: 7468 6572 2028 3129 2061 2022 636f 6e73  ther (1) a "cons
-00005da0: 756d 6572 2070 726f 6475 6374 222c 2077  umer product", w
-00005db0: 6869 6368 206d 6561 6e73 2061 6e79 0d0a  hich means any..
-00005dc0: 7461 6e67 6962 6c65 2070 6572 736f 6e61  tangible persona
-00005dd0: 6c20 7072 6f70 6572 7479 2077 6869 6368  l property which
-00005de0: 2069 7320 6e6f 726d 616c 6c79 2075 7365   is normally use
-00005df0: 6420 666f 7220 7065 7273 6f6e 616c 2c20  d for personal, 
-00005e00: 6661 6d69 6c79 2c0d 0a6f 7220 686f 7573  family,..or hous
-00005e10: 6568 6f6c 6420 7075 7270 6f73 6573 2c20  ehold purposes, 
-00005e20: 6f72 2028 3229 2061 6e79 7468 696e 6720  or (2) anything 
-00005e30: 6465 7369 676e 6564 206f 7220 736f 6c64  designed or sold
-00005e40: 2066 6f72 2069 6e63 6f72 706f 7261 7469   for incorporati
-00005e50: 6f6e 0d0a 696e 746f 2061 2064 7765 6c6c  on..into a dwell
-00005e60: 696e 672e 2020 496e 2064 6574 6572 6d69  ing.  In determi
-00005e70: 6e69 6e67 2077 6865 7468 6572 2061 2070  ning whether a p
-00005e80: 726f 6475 6374 2069 7320 6120 636f 6e73  roduct is a cons
-00005e90: 756d 6572 2070 726f 6475 6374 2c0d 0a64  umer product,..d
-00005ea0: 6f75 6274 6675 6c20 6361 7365 7320 7368  oubtful cases sh
-00005eb0: 616c 6c20 6265 2072 6573 6f6c 7665 6420  all be resolved 
-00005ec0: 696e 2066 6176 6f72 206f 6620 636f 7665  in favor of cove
-00005ed0: 7261 6765 2e20 2046 6f72 2061 2070 6172  rage.  For a par
-00005ee0: 7469 6375 6c61 720d 0a70 726f 6475 6374  ticular..product
-00005ef0: 2072 6563 6569 7665 6420 6279 2061 2070   received by a p
-00005f00: 6172 7469 6375 6c61 7220 7573 6572 2c20  articular user, 
-00005f10: 226e 6f72 6d61 6c6c 7920 7573 6564 2220  "normally used" 
-00005f20: 7265 6665 7273 2074 6f20 610d 0a74 7970  refers to a..typ
-00005f30: 6963 616c 206f 7220 636f 6d6d 6f6e 2075  ical or common u
-00005f40: 7365 206f 6620 7468 6174 2063 6c61 7373  se of that class
-00005f50: 206f 6620 7072 6f64 7563 742c 2072 6567   of product, reg
-00005f60: 6172 646c 6573 7320 6f66 2074 6865 2073  ardless of the s
-00005f70: 7461 7475 730d 0a6f 6620 7468 6520 7061  tatus..of the pa
-00005f80: 7274 6963 756c 6172 2075 7365 7220 6f72  rticular user or
-00005f90: 206f 6620 7468 6520 7761 7920 696e 2077   of the way in w
-00005fa0: 6869 6368 2074 6865 2070 6172 7469 6375  hich the particu
-00005fb0: 6c61 7220 7573 6572 0d0a 6163 7475 616c  lar user..actual
-00005fc0: 6c79 2075 7365 732c 206f 7220 6578 7065  ly uses, or expe
-00005fd0: 6374 7320 6f72 2069 7320 6578 7065 6374  cts or is expect
-00005fe0: 6564 2074 6f20 7573 652c 2074 6865 2070  ed to use, the p
-00005ff0: 726f 6475 6374 2e20 2041 2070 726f 6475  roduct.  A produ
-00006000: 6374 0d0a 6973 2061 2063 6f6e 7375 6d65  ct..is a consume
-00006010: 7220 7072 6f64 7563 7420 7265 6761 7264  r product regard
-00006020: 6c65 7373 206f 6620 7768 6574 6865 7220  less of whether 
-00006030: 7468 6520 7072 6f64 7563 7420 6861 7320  the product has 
-00006040: 7375 6273 7461 6e74 6961 6c0d 0a63 6f6d  substantial..com
-00006050: 6d65 7263 6961 6c2c 2069 6e64 7573 7472  mercial, industr
-00006060: 6961 6c20 6f72 206e 6f6e 2d63 6f6e 7375  ial or non-consu
-00006070: 6d65 7220 7573 6573 2c20 756e 6c65 7373  mer uses, unless
-00006080: 2073 7563 6820 7573 6573 2072 6570 7265   such uses repre
-00006090: 7365 6e74 0d0a 7468 6520 6f6e 6c79 2073  sent..the only s
-000060a0: 6967 6e69 6669 6361 6e74 206d 6f64 6520  ignificant mode 
-000060b0: 6f66 2075 7365 206f 6620 7468 6520 7072  of use of the pr
-000060c0: 6f64 7563 742e 0d0a 0d0a 2020 2249 6e73  oduct.....  "Ins
-000060d0: 7461 6c6c 6174 696f 6e20 496e 666f 726d  tallation Inform
-000060e0: 6174 696f 6e22 2066 6f72 2061 2055 7365  ation" for a Use
-000060f0: 7220 5072 6f64 7563 7420 6d65 616e 7320  r Product means 
-00006100: 616e 7920 6d65 7468 6f64 732c 0d0a 7072  any methods,..pr
-00006110: 6f63 6564 7572 6573 2c20 6175 7468 6f72  ocedures, author
-00006120: 697a 6174 696f 6e20 6b65 7973 2c20 6f72  ization keys, or
-00006130: 206f 7468 6572 2069 6e66 6f72 6d61 7469   other informati
-00006140: 6f6e 2072 6571 7569 7265 6420 746f 2069  on required to i
-00006150: 6e73 7461 6c6c 0d0a 616e 6420 6578 6563  nstall..and exec
-00006160: 7574 6520 6d6f 6469 6669 6564 2076 6572  ute modified ver
-00006170: 7369 6f6e 7320 6f66 2061 2063 6f76 6572  sions of a cover
-00006180: 6564 2077 6f72 6b20 696e 2074 6861 7420  ed work in that 
-00006190: 5573 6572 2050 726f 6475 6374 2066 726f  User Product fro
-000061a0: 6d0d 0a61 206d 6f64 6966 6965 6420 7665  m..a modified ve
-000061b0: 7273 696f 6e20 6f66 2069 7473 2043 6f72  rsion of its Cor
-000061c0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
-000061d0: 652e 2020 5468 6520 696e 666f 726d 6174  e.  The informat
-000061e0: 696f 6e20 6d75 7374 0d0a 7375 6666 6963  ion must..suffic
-000061f0: 6520 746f 2065 6e73 7572 6520 7468 6174  e to ensure that
-00006200: 2074 6865 2063 6f6e 7469 6e75 6564 2066   the continued f
-00006210: 756e 6374 696f 6e69 6e67 206f 6620 7468  unctioning of th
-00006220: 6520 6d6f 6469 6669 6564 206f 626a 6563  e modified objec
-00006230: 740d 0a63 6f64 6520 6973 2069 6e20 6e6f  t..code is in no
-00006240: 2063 6173 6520 7072 6576 656e 7465 6420   case prevented 
-00006250: 6f72 2069 6e74 6572 6665 7265 6420 7769  or interfered wi
-00006260: 7468 2073 6f6c 656c 7920 6265 6361 7573  th solely becaus
-00006270: 650d 0a6d 6f64 6966 6963 6174 696f 6e20  e..modification 
-00006280: 6861 7320 6265 656e 206d 6164 652e 0d0a  has been made...
-00006290: 0d0a 2020 4966 2079 6f75 2063 6f6e 7665  ..  If you conve
-000062a0: 7920 616e 206f 626a 6563 7420 636f 6465  y an object code
-000062b0: 2077 6f72 6b20 756e 6465 7220 7468 6973   work under this
-000062c0: 2073 6563 7469 6f6e 2069 6e2c 206f 7220   section in, or 
-000062d0: 7769 7468 2c20 6f72 0d0a 7370 6563 6966  with, or..specif
-000062e0: 6963 616c 6c79 2066 6f72 2075 7365 2069  ically for use i
-000062f0: 6e2c 2061 2055 7365 7220 5072 6f64 7563  n, a User Produc
-00006300: 742c 2061 6e64 2074 6865 2063 6f6e 7665  t, and the conve
-00006310: 7969 6e67 206f 6363 7572 7320 6173 0d0a  ying occurs as..
-00006320: 7061 7274 206f 6620 6120 7472 616e 7361  part of a transa
-00006330: 6374 696f 6e20 696e 2077 6869 6368 2074  ction in which t
-00006340: 6865 2072 6967 6874 206f 6620 706f 7373  he right of poss
-00006350: 6573 7369 6f6e 2061 6e64 2075 7365 206f  ession and use o
-00006360: 6620 7468 650d 0a55 7365 7220 5072 6f64  f the..User Prod
-00006370: 7563 7420 6973 2074 7261 6e73 6665 7272  uct is transferr
-00006380: 6564 2074 6f20 7468 6520 7265 6369 7069  ed to the recipi
-00006390: 656e 7420 696e 2070 6572 7065 7475 6974  ent in perpetuit
-000063a0: 7920 6f72 2066 6f72 2061 0d0a 6669 7865  y or for a..fixe
-000063b0: 6420 7465 726d 2028 7265 6761 7264 6c65  d term (regardle
-000063c0: 7373 206f 6620 686f 7720 7468 6520 7472  ss of how the tr
-000063d0: 616e 7361 6374 696f 6e20 6973 2063 6861  ansaction is cha
-000063e0: 7261 6374 6572 697a 6564 292c 2074 6865  racterized), the
-000063f0: 0d0a 436f 7272 6573 706f 6e64 696e 6720  ..Corresponding 
-00006400: 536f 7572 6365 2063 6f6e 7665 7965 6420  Source conveyed 
-00006410: 756e 6465 7220 7468 6973 2073 6563 7469  under this secti
-00006420: 6f6e 206d 7573 7420 6265 2061 6363 6f6d  on must be accom
-00006430: 7061 6e69 6564 0d0a 6279 2074 6865 2049  panied..by the I
-00006440: 6e73 7461 6c6c 6174 696f 6e20 496e 666f  nstallation Info
-00006450: 726d 6174 696f 6e2e 2020 4275 7420 7468  rmation.  But th
-00006460: 6973 2072 6571 7569 7265 6d65 6e74 2064  is requirement d
-00006470: 6f65 7320 6e6f 7420 6170 706c 790d 0a69  oes not apply..i
-00006480: 6620 6e65 6974 6865 7220 796f 7520 6e6f  f neither you no
-00006490: 7220 616e 7920 7468 6972 6420 7061 7274  r any third part
-000064a0: 7920 7265 7461 696e 7320 7468 6520 6162  y retains the ab
-000064b0: 696c 6974 7920 746f 2069 6e73 7461 6c6c  ility to install
-000064c0: 0d0a 6d6f 6469 6669 6564 206f 626a 6563  ..modified objec
-000064d0: 7420 636f 6465 206f 6e20 7468 6520 5573  t code on the Us
-000064e0: 6572 2050 726f 6475 6374 2028 666f 7220  er Product (for 
-000064f0: 6578 616d 706c 652c 2074 6865 2077 6f72  example, the wor
-00006500: 6b20 6861 730d 0a62 6565 6e20 696e 7374  k has..been inst
-00006510: 616c 6c65 6420 696e 2052 4f4d 292e 0d0a  alled in ROM)...
-00006520: 0d0a 2020 5468 6520 7265 7175 6972 656d  ..  The requirem
-00006530: 656e 7420 746f 2070 726f 7669 6465 2049  ent to provide I
-00006540: 6e73 7461 6c6c 6174 696f 6e20 496e 666f  nstallation Info
-00006550: 726d 6174 696f 6e20 646f 6573 206e 6f74  rmation does not
-00006560: 2069 6e63 6c75 6465 2061 0d0a 7265 7175   include a..requ
-00006570: 6972 656d 656e 7420 746f 2063 6f6e 7469  irement to conti
-00006580: 6e75 6520 746f 2070 726f 7669 6465 2073  nue to provide s
-00006590: 7570 706f 7274 2073 6572 7669 6365 2c20  upport service, 
-000065a0: 7761 7272 616e 7479 2c20 6f72 2075 7064  warranty, or upd
-000065b0: 6174 6573 0d0a 666f 7220 6120 776f 726b  ates..for a work
-000065c0: 2074 6861 7420 6861 7320 6265 656e 206d   that has been m
-000065d0: 6f64 6966 6965 6420 6f72 2069 6e73 7461  odified or insta
-000065e0: 6c6c 6564 2062 7920 7468 6520 7265 6369  lled by the reci
-000065f0: 7069 656e 742c 206f 7220 666f 720d 0a74  pient, or for..t
-00006600: 6865 2055 7365 7220 5072 6f64 7563 7420  he User Product 
-00006610: 696e 2077 6869 6368 2069 7420 6861 7320  in which it has 
-00006620: 6265 656e 206d 6f64 6966 6965 6420 6f72  been modified or
-00006630: 2069 6e73 7461 6c6c 6564 2e20 2041 6363   installed.  Acc
-00006640: 6573 7320 746f 2061 0d0a 6e65 7477 6f72  ess to a..networ
-00006650: 6b20 6d61 7920 6265 2064 656e 6965 6420  k may be denied 
-00006660: 7768 656e 2074 6865 206d 6f64 6966 6963  when the modific
-00006670: 6174 696f 6e20 6974 7365 6c66 206d 6174  ation itself mat
-00006680: 6572 6961 6c6c 7920 616e 640d 0a61 6476  erially and..adv
-00006690: 6572 7365 6c79 2061 6666 6563 7473 2074  ersely affects t
-000066a0: 6865 206f 7065 7261 7469 6f6e 206f 6620  he operation of 
-000066b0: 7468 6520 6e65 7477 6f72 6b20 6f72 2076  the network or v
-000066c0: 696f 6c61 7465 7320 7468 6520 7275 6c65  iolates the rule
-000066d0: 7320 616e 640d 0a70 726f 746f 636f 6c73  s and..protocols
-000066e0: 2066 6f72 2063 6f6d 6d75 6e69 6361 7469   for communicati
-000066f0: 6f6e 2061 6372 6f73 7320 7468 6520 6e65  on across the ne
-00006700: 7477 6f72 6b2e 0d0a 0d0a 2020 436f 7272  twork.....  Corr
-00006710: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
-00006720: 2063 6f6e 7665 7965 642c 2061 6e64 2049   conveyed, and I
-00006730: 6e73 7461 6c6c 6174 696f 6e20 496e 666f  nstallation Info
-00006740: 726d 6174 696f 6e20 7072 6f76 6964 6564  rmation provided
-00006750: 2c0d 0a69 6e20 6163 636f 7264 2077 6974  ,..in accord wit
-00006760: 6820 7468 6973 2073 6563 7469 6f6e 206d  h this section m
-00006770: 7573 7420 6265 2069 6e20 6120 666f 726d  ust be in a form
-00006780: 6174 2074 6861 7420 6973 2070 7562 6c69  at that is publi
-00006790: 636c 790d 0a64 6f63 756d 656e 7465 6420  cly..documented 
-000067a0: 2861 6e64 2077 6974 6820 616e 2069 6d70  (and with an imp
-000067b0: 6c65 6d65 6e74 6174 696f 6e20 6176 6169  lementation avai
-000067c0: 6c61 626c 6520 746f 2074 6865 2070 7562  lable to the pub
-000067d0: 6c69 6320 696e 0d0a 736f 7572 6365 2063  lic in..source c
-000067e0: 6f64 6520 666f 726d 292c 2061 6e64 206d  ode form), and m
-000067f0: 7573 7420 7265 7175 6972 6520 6e6f 2073  ust require no s
-00006800: 7065 6369 616c 2070 6173 7377 6f72 6420  pecial password 
-00006810: 6f72 206b 6579 2066 6f72 0d0a 756e 7061  or key for..unpa
-00006820: 636b 696e 672c 2072 6561 6469 6e67 206f  cking, reading o
-00006830: 7220 636f 7079 696e 672e 0d0a 0d0a 2020  r copying.....  
-00006840: 372e 2041 6464 6974 696f 6e61 6c20 5465  7. Additional Te
-00006850: 726d 732e 0d0a 0d0a 2020 2241 6464 6974  rms.....  "Addit
-00006860: 696f 6e61 6c20 7065 726d 6973 7369 6f6e  ional permission
-00006870: 7322 2061 7265 2074 6572 6d73 2074 6861  s" are terms tha
-00006880: 7420 7375 7070 6c65 6d65 6e74 2074 6865  t supplement the
-00006890: 2074 6572 6d73 206f 6620 7468 6973 0d0a   terms of this..
-000068a0: 4c69 6365 6e73 6520 6279 206d 616b 696e  License by makin
-000068b0: 6720 6578 6365 7074 696f 6e73 2066 726f  g exceptions fro
-000068c0: 6d20 6f6e 6520 6f72 206d 6f72 6520 6f66  m one or more of
-000068d0: 2069 7473 2063 6f6e 6469 7469 6f6e 732e   its conditions.
-000068e0: 0d0a 4164 6469 7469 6f6e 616c 2070 6572  ..Additional per
-000068f0: 6d69 7373 696f 6e73 2074 6861 7420 6172  missions that ar
-00006900: 6520 6170 706c 6963 6162 6c65 2074 6f20  e applicable to 
-00006910: 7468 6520 656e 7469 7265 2050 726f 6772  the entire Progr
-00006920: 616d 2073 6861 6c6c 0d0a 6265 2074 7265  am shall..be tre
-00006930: 6174 6564 2061 7320 7468 6f75 6768 2074  ated as though t
-00006940: 6865 7920 7765 7265 2069 6e63 6c75 6465  hey were include
-00006950: 6420 696e 2074 6869 7320 4c69 6365 6e73  d in this Licens
-00006960: 652c 2074 6f20 7468 6520 6578 7465 6e74  e, to the extent
-00006970: 0d0a 7468 6174 2074 6865 7920 6172 6520  ..that they are 
-00006980: 7661 6c69 6420 756e 6465 7220 6170 706c  valid under appl
-00006990: 6963 6162 6c65 206c 6177 2e20 2049 6620  icable law.  If 
-000069a0: 6164 6469 7469 6f6e 616c 2070 6572 6d69  additional permi
-000069b0: 7373 696f 6e73 0d0a 6170 706c 7920 6f6e  ssions..apply on
-000069c0: 6c79 2074 6f20 7061 7274 206f 6620 7468  ly to part of th
-000069d0: 6520 5072 6f67 7261 6d2c 2074 6861 7420  e Program, that 
-000069e0: 7061 7274 206d 6179 2062 6520 7573 6564  part may be used
-000069f0: 2073 6570 6172 6174 656c 790d 0a75 6e64   separately..und
-00006a00: 6572 2074 686f 7365 2070 6572 6d69 7373  er those permiss
-00006a10: 696f 6e73 2c20 6275 7420 7468 6520 656e  ions, but the en
-00006a20: 7469 7265 2050 726f 6772 616d 2072 656d  tire Program rem
-00006a30: 6169 6e73 2067 6f76 6572 6e65 6420 6279  ains governed by
-00006a40: 0d0a 7468 6973 204c 6963 656e 7365 2077  ..this License w
-00006a50: 6974 686f 7574 2072 6567 6172 6420 746f  ithout regard to
-00006a60: 2074 6865 2061 6464 6974 696f 6e61 6c20   the additional 
-00006a70: 7065 726d 6973 7369 6f6e 732e 0d0a 0d0a  permissions.....
-00006a80: 2020 5768 656e 2079 6f75 2063 6f6e 7665    When you conve
-00006a90: 7920 6120 636f 7079 206f 6620 6120 636f  y a copy of a co
-00006aa0: 7665 7265 6420 776f 726b 2c20 796f 7520  vered work, you 
-00006ab0: 6d61 7920 6174 2079 6f75 7220 6f70 7469  may at your opti
-00006ac0: 6f6e 0d0a 7265 6d6f 7665 2061 6e79 2061  on..remove any a
-00006ad0: 6464 6974 696f 6e61 6c20 7065 726d 6973  dditional permis
-00006ae0: 7369 6f6e 7320 6672 6f6d 2074 6861 7420  sions from that 
-00006af0: 636f 7079 2c20 6f72 2066 726f 6d20 616e  copy, or from an
-00006b00: 7920 7061 7274 206f 660d 0a69 742e 2020  y part of..it.  
-00006b10: 2841 6464 6974 696f 6e61 6c20 7065 726d  (Additional perm
-00006b20: 6973 7369 6f6e 7320 6d61 7920 6265 2077  issions may be w
-00006b30: 7269 7474 656e 2074 6f20 7265 7175 6972  ritten to requir
-00006b40: 6520 7468 6569 7220 6f77 6e0d 0a72 656d  e their own..rem
-00006b50: 6f76 616c 2069 6e20 6365 7274 6169 6e20  oval in certain 
-00006b60: 6361 7365 7320 7768 656e 2079 6f75 206d  cases when you m
-00006b70: 6f64 6966 7920 7468 6520 776f 726b 2e29  odify the work.)
-00006b80: 2020 596f 7520 6d61 7920 706c 6163 650d    You may place.
-00006b90: 0a61 6464 6974 696f 6e61 6c20 7065 726d  .additional perm
-00006ba0: 6973 7369 6f6e 7320 6f6e 206d 6174 6572  issions on mater
-00006bb0: 6961 6c2c 2061 6464 6564 2062 7920 796f  ial, added by yo
-00006bc0: 7520 746f 2061 2063 6f76 6572 6564 2077  u to a covered w
-00006bd0: 6f72 6b2c 0d0a 666f 7220 7768 6963 6820  ork,..for which 
-00006be0: 796f 7520 6861 7665 206f 7220 6361 6e20  you have or can 
-00006bf0: 6769 7665 2061 7070 726f 7072 6961 7465  give appropriate
-00006c00: 2063 6f70 7972 6967 6874 2070 6572 6d69   copyright permi
-00006c10: 7373 696f 6e2e 0d0a 0d0a 2020 4e6f 7477  ssion.....  Notw
-00006c20: 6974 6873 7461 6e64 696e 6720 616e 7920  ithstanding any 
-00006c30: 6f74 6865 7220 7072 6f76 6973 696f 6e20  other provision 
-00006c40: 6f66 2074 6869 7320 4c69 6365 6e73 652c  of this License,
-00006c50: 2066 6f72 206d 6174 6572 6961 6c20 796f   for material yo
-00006c60: 750d 0a61 6464 2074 6f20 6120 636f 7665  u..add to a cove
-00006c70: 7265 6420 776f 726b 2c20 796f 7520 6d61  red work, you ma
-00006c80: 7920 2869 6620 6175 7468 6f72 697a 6564  y (if authorized
-00006c90: 2062 7920 7468 6520 636f 7079 7269 6768   by the copyrigh
-00006ca0: 7420 686f 6c64 6572 7320 6f66 0d0a 7468  t holders of..th
-00006cb0: 6174 206d 6174 6572 6961 6c29 2073 7570  at material) sup
-00006cc0: 706c 656d 656e 7420 7468 6520 7465 726d  plement the term
-00006cd0: 7320 6f66 2074 6869 7320 4c69 6365 6e73  s of this Licens
-00006ce0: 6520 7769 7468 2074 6572 6d73 3a0d 0a0d  e with terms:...
-00006cf0: 0a20 2020 2061 2920 4469 7363 6c61 696d  .    a) Disclaim
-00006d00: 696e 6720 7761 7272 616e 7479 206f 7220  ing warranty or 
-00006d10: 6c69 6d69 7469 6e67 206c 6961 6269 6c69  limiting liabili
-00006d20: 7479 2064 6966 6665 7265 6e74 6c79 2066  ty differently f
-00006d30: 726f 6d20 7468 650d 0a20 2020 2074 6572  rom the..    ter
-00006d40: 6d73 206f 6620 7365 6374 696f 6e73 2031  ms of sections 1
-00006d50: 3520 616e 6420 3136 206f 6620 7468 6973  5 and 16 of this
-00006d60: 204c 6963 656e 7365 3b20 6f72 0d0a 0d0a   License; or....
-00006d70: 2020 2020 6229 2052 6571 7569 7269 6e67      b) Requiring
-00006d80: 2070 7265 7365 7276 6174 696f 6e20 6f66   preservation of
-00006d90: 2073 7065 6369 6669 6564 2072 6561 736f   specified reaso
-00006da0: 6e61 626c 6520 6c65 6761 6c20 6e6f 7469  nable legal noti
-00006db0: 6365 7320 6f72 0d0a 2020 2020 6175 7468  ces or..    auth
-00006dc0: 6f72 2061 7474 7269 6275 7469 6f6e 7320  or attributions 
-00006dd0: 696e 2074 6861 7420 6d61 7465 7269 616c  in that material
-00006de0: 206f 7220 696e 2074 6865 2041 7070 726f   or in the Appro
-00006df0: 7072 6961 7465 204c 6567 616c 0d0a 2020  priate Legal..  
-00006e00: 2020 4e6f 7469 6365 7320 6469 7370 6c61    Notices displa
-00006e10: 7965 6420 6279 2077 6f72 6b73 2063 6f6e  yed by works con
-00006e20: 7461 696e 696e 6720 6974 3b20 6f72 0d0a  taining it; or..
-00006e30: 0d0a 2020 2020 6329 2050 726f 6869 6269  ..    c) Prohibi
-00006e40: 7469 6e67 206d 6973 7265 7072 6573 656e  ting misrepresen
-00006e50: 7461 7469 6f6e 206f 6620 7468 6520 6f72  tation of the or
-00006e60: 6967 696e 206f 6620 7468 6174 206d 6174  igin of that mat
-00006e70: 6572 6961 6c2c 206f 720d 0a20 2020 2072  erial, or..    r
-00006e80: 6571 7569 7269 6e67 2074 6861 7420 6d6f  equiring that mo
-00006e90: 6469 6669 6564 2076 6572 7369 6f6e 7320  dified versions 
-00006ea0: 6f66 2073 7563 6820 6d61 7465 7269 616c  of such material
-00006eb0: 2062 6520 6d61 726b 6564 2069 6e0d 0a20   be marked in.. 
-00006ec0: 2020 2072 6561 736f 6e61 626c 6520 7761     reasonable wa
-00006ed0: 7973 2061 7320 6469 6666 6572 656e 7420  ys as different 
-00006ee0: 6672 6f6d 2074 6865 206f 7269 6769 6e61  from the origina
-00006ef0: 6c20 7665 7273 696f 6e3b 206f 720d 0a0d  l version; or...
-00006f00: 0a20 2020 2064 2920 4c69 6d69 7469 6e67  .    d) Limiting
-00006f10: 2074 6865 2075 7365 2066 6f72 2070 7562   the use for pub
-00006f20: 6c69 6369 7479 2070 7572 706f 7365 7320  licity purposes 
-00006f30: 6f66 206e 616d 6573 206f 6620 6c69 6365  of names of lice
-00006f40: 6e73 6f72 7320 6f72 0d0a 2020 2020 6175  nsors or..    au
-00006f50: 7468 6f72 7320 6f66 2074 6865 206d 6174  thors of the mat
-00006f60: 6572 6961 6c3b 206f 720d 0a0d 0a20 2020  erial; or....   
-00006f70: 2065 2920 4465 636c 696e 696e 6720 746f   e) Declining to
-00006f80: 2067 7261 6e74 2072 6967 6874 7320 756e   grant rights un
-00006f90: 6465 7220 7472 6164 656d 6172 6b20 6c61  der trademark la
-00006fa0: 7720 666f 7220 7573 6520 6f66 2073 6f6d  w for use of som
-00006fb0: 650d 0a20 2020 2074 7261 6465 206e 616d  e..    trade nam
-00006fc0: 6573 2c20 7472 6164 656d 6172 6b73 2c20  es, trademarks, 
-00006fd0: 6f72 2073 6572 7669 6365 206d 6172 6b73  or service marks
-00006fe0: 3b20 6f72 0d0a 0d0a 2020 2020 6629 2052  ; or....    f) R
-00006ff0: 6571 7569 7269 6e67 2069 6e64 656d 6e69  equiring indemni
-00007000: 6669 6361 7469 6f6e 206f 6620 6c69 6365  fication of lice
-00007010: 6e73 6f72 7320 616e 6420 6175 7468 6f72  nsors and author
-00007020: 7320 6f66 2074 6861 740d 0a20 2020 206d  s of that..    m
-00007030: 6174 6572 6961 6c20 6279 2061 6e79 6f6e  aterial by anyon
-00007040: 6520 7768 6f20 636f 6e76 6579 7320 7468  e who conveys th
-00007050: 6520 6d61 7465 7269 616c 2028 6f72 206d  e material (or m
-00007060: 6f64 6966 6965 6420 7665 7273 696f 6e73  odified versions
-00007070: 206f 660d 0a20 2020 2069 7429 2077 6974   of..    it) wit
-00007080: 6820 636f 6e74 7261 6374 7561 6c20 6173  h contractual as
-00007090: 7375 6d70 7469 6f6e 7320 6f66 206c 6961  sumptions of lia
-000070a0: 6269 6c69 7479 2074 6f20 7468 6520 7265  bility to the re
-000070b0: 6369 7069 656e 742c 2066 6f72 0d0a 2020  cipient, for..  
-000070c0: 2020 616e 7920 6c69 6162 696c 6974 7920    any liability 
-000070d0: 7468 6174 2074 6865 7365 2063 6f6e 7472  that these contr
-000070e0: 6163 7475 616c 2061 7373 756d 7074 696f  actual assumptio
-000070f0: 6e73 2064 6972 6563 746c 7920 696d 706f  ns directly impo
-00007100: 7365 206f 6e0d 0a20 2020 2074 686f 7365  se on..    those
-00007110: 206c 6963 656e 736f 7273 2061 6e64 2061   licensors and a
-00007120: 7574 686f 7273 2e0d 0a0d 0a20 2041 6c6c  uthors.....  All
-00007130: 206f 7468 6572 206e 6f6e 2d70 6572 6d69   other non-permi
-00007140: 7373 6976 6520 6164 6469 7469 6f6e 616c  ssive additional
-00007150: 2074 6572 6d73 2061 7265 2063 6f6e 7369   terms are consi
-00007160: 6465 7265 6420 2266 7572 7468 6572 0d0a  dered "further..
-00007170: 7265 7374 7269 6374 696f 6e73 2220 7769  restrictions" wi
-00007180: 7468 696e 2074 6865 206d 6561 6e69 6e67  thin the meaning
-00007190: 206f 6620 7365 6374 696f 6e20 3130 2e20   of section 10. 
-000071a0: 2049 6620 7468 6520 5072 6f67 7261 6d20   If the Program 
-000071b0: 6173 2079 6f75 0d0a 7265 6365 6976 6564  as you..received
-000071c0: 2069 742c 206f 7220 616e 7920 7061 7274   it, or any part
-000071d0: 206f 6620 6974 2c20 636f 6e74 6169 6e73   of it, contains
-000071e0: 2061 206e 6f74 6963 6520 7374 6174 696e   a notice statin
-000071f0: 6720 7468 6174 2069 7420 6973 0d0a 676f  g that it is..go
-00007200: 7665 726e 6564 2062 7920 7468 6973 204c  verned by this L
-00007210: 6963 656e 7365 2061 6c6f 6e67 2077 6974  icense along wit
-00007220: 6820 6120 7465 726d 2074 6861 7420 6973  h a term that is
-00007230: 2061 2066 7572 7468 6572 0d0a 7265 7374   a further..rest
-00007240: 7269 6374 696f 6e2c 2079 6f75 206d 6179  riction, you may
-00007250: 2072 656d 6f76 6520 7468 6174 2074 6572   remove that ter
-00007260: 6d2e 2020 4966 2061 206c 6963 656e 7365  m.  If a license
-00007270: 2064 6f63 756d 656e 7420 636f 6e74 6169   document contai
-00007280: 6e73 0d0a 6120 6675 7274 6865 7220 7265  ns..a further re
-00007290: 7374 7269 6374 696f 6e20 6275 7420 7065  striction but pe
-000072a0: 726d 6974 7320 7265 6c69 6365 6e73 696e  rmits relicensin
-000072b0: 6720 6f72 2063 6f6e 7665 7969 6e67 2075  g or conveying u
-000072c0: 6e64 6572 2074 6869 730d 0a4c 6963 656e  nder this..Licen
-000072d0: 7365 2c20 796f 7520 6d61 7920 6164 6420  se, you may add 
-000072e0: 746f 2061 2063 6f76 6572 6564 2077 6f72  to a covered wor
-000072f0: 6b20 6d61 7465 7269 616c 2067 6f76 6572  k material gover
-00007300: 6e65 6420 6279 2074 6865 2074 6572 6d73  ned by the terms
-00007310: 0d0a 6f66 2074 6861 7420 6c69 6365 6e73  ..of that licens
-00007320: 6520 646f 6375 6d65 6e74 2c20 7072 6f76  e document, prov
-00007330: 6964 6564 2074 6861 7420 7468 6520 6675  ided that the fu
-00007340: 7274 6865 7220 7265 7374 7269 6374 696f  rther restrictio
-00007350: 6e20 646f 6573 0d0a 6e6f 7420 7375 7276  n does..not surv
-00007360: 6976 6520 7375 6368 2072 656c 6963 656e  ive such relicen
-00007370: 7369 6e67 206f 7220 636f 6e76 6579 696e  sing or conveyin
-00007380: 672e 0d0a 0d0a 2020 4966 2079 6f75 2061  g.....  If you a
-00007390: 6464 2074 6572 6d73 2074 6f20 6120 636f  dd terms to a co
-000073a0: 7665 7265 6420 776f 726b 2069 6e20 6163  vered work in ac
-000073b0: 636f 7264 2077 6974 6820 7468 6973 2073  cord with this s
-000073c0: 6563 7469 6f6e 2c20 796f 750d 0a6d 7573  ection, you..mus
-000073d0: 7420 706c 6163 652c 2069 6e20 7468 6520  t place, in the 
-000073e0: 7265 6c65 7661 6e74 2073 6f75 7263 6520  relevant source 
-000073f0: 6669 6c65 732c 2061 2073 7461 7465 6d65  files, a stateme
-00007400: 6e74 206f 6620 7468 650d 0a61 6464 6974  nt of the..addit
-00007410: 696f 6e61 6c20 7465 726d 7320 7468 6174  ional terms that
-00007420: 2061 7070 6c79 2074 6f20 7468 6f73 6520   apply to those 
-00007430: 6669 6c65 732c 206f 7220 6120 6e6f 7469  files, or a noti
-00007440: 6365 2069 6e64 6963 6174 696e 670d 0a77  ce indicating..w
-00007450: 6865 7265 2074 6f20 6669 6e64 2074 6865  here to find the
-00007460: 2061 7070 6c69 6361 626c 6520 7465 726d   applicable term
-00007470: 732e 0d0a 0d0a 2020 4164 6469 7469 6f6e  s.....  Addition
-00007480: 616c 2074 6572 6d73 2c20 7065 726d 6973  al terms, permis
-00007490: 7369 7665 206f 7220 6e6f 6e2d 7065 726d  sive or non-perm
-000074a0: 6973 7369 7665 2c20 6d61 7920 6265 2073  issive, may be s
-000074b0: 7461 7465 6420 696e 2074 6865 0d0a 666f  tated in the..fo
-000074c0: 726d 206f 6620 6120 7365 7061 7261 7465  rm of a separate
-000074d0: 6c79 2077 7269 7474 656e 206c 6963 656e  ly written licen
-000074e0: 7365 2c20 6f72 2073 7461 7465 6420 6173  se, or stated as
-000074f0: 2065 7863 6570 7469 6f6e 733b 0d0a 7468   exceptions;..th
-00007500: 6520 6162 6f76 6520 7265 7175 6972 656d  e above requirem
-00007510: 656e 7473 2061 7070 6c79 2065 6974 6865  ents apply eithe
-00007520: 7220 7761 792e 0d0a 0d0a 2020 382e 2054  r way.....  8. T
-00007530: 6572 6d69 6e61 7469 6f6e 2e0d 0a0d 0a20  ermination..... 
-00007540: 2059 6f75 206d 6179 206e 6f74 2070 726f   You may not pro
-00007550: 7061 6761 7465 206f 7220 6d6f 6469 6679  pagate or modify
-00007560: 2061 2063 6f76 6572 6564 2077 6f72 6b20   a covered work 
-00007570: 6578 6365 7074 2061 7320 6578 7072 6573  except as expres
-00007580: 736c 790d 0a70 726f 7669 6465 6420 756e  sly..provided un
-00007590: 6465 7220 7468 6973 204c 6963 656e 7365  der this License
-000075a0: 2e20 2041 6e79 2061 7474 656d 7074 206f  .  Any attempt o
-000075b0: 7468 6572 7769 7365 2074 6f20 7072 6f70  therwise to prop
-000075c0: 6167 6174 6520 6f72 0d0a 6d6f 6469 6679  agate or..modify
-000075d0: 2069 7420 6973 2076 6f69 642c 2061 6e64   it is void, and
-000075e0: 2077 696c 6c20 6175 746f 6d61 7469 6361   will automatica
-000075f0: 6c6c 7920 7465 726d 696e 6174 6520 796f  lly terminate yo
-00007600: 7572 2072 6967 6874 7320 756e 6465 720d  ur rights under.
-00007610: 0a74 6869 7320 4c69 6365 6e73 6520 2869  .this License (i
-00007620: 6e63 6c75 6469 6e67 2061 6e79 2070 6174  ncluding any pat
-00007630: 656e 7420 6c69 6365 6e73 6573 2067 7261  ent licenses gra
-00007640: 6e74 6564 2075 6e64 6572 2074 6865 2074  nted under the t
-00007650: 6869 7264 0d0a 7061 7261 6772 6170 6820  hird..paragraph 
-00007660: 6f66 2073 6563 7469 6f6e 2031 3129 2e0d  of section 11)..
-00007670: 0a0d 0a20 2048 6f77 6576 6572 2c20 6966  ...  However, if
-00007680: 2079 6f75 2063 6561 7365 2061 6c6c 2076   you cease all v
-00007690: 696f 6c61 7469 6f6e 206f 6620 7468 6973  iolation of this
-000076a0: 204c 6963 656e 7365 2c20 7468 656e 2079   License, then y
-000076b0: 6f75 720d 0a6c 6963 656e 7365 2066 726f  our..license fro
-000076c0: 6d20 6120 7061 7274 6963 756c 6172 2063  m a particular c
-000076d0: 6f70 7972 6967 6874 2068 6f6c 6465 7220  opyright holder 
-000076e0: 6973 2072 6569 6e73 7461 7465 6420 2861  is reinstated (a
-000076f0: 290d 0a70 726f 7669 7369 6f6e 616c 6c79  )..provisionally
-00007700: 2c20 756e 6c65 7373 2061 6e64 2075 6e74  , unless and unt
-00007710: 696c 2074 6865 2063 6f70 7972 6967 6874  il the copyright
-00007720: 2068 6f6c 6465 7220 6578 706c 6963 6974   holder explicit
-00007730: 6c79 2061 6e64 0d0a 6669 6e61 6c6c 7920  ly and..finally 
-00007740: 7465 726d 696e 6174 6573 2079 6f75 7220  terminates your 
-00007750: 6c69 6365 6e73 652c 2061 6e64 2028 6229  license, and (b)
-00007760: 2070 6572 6d61 6e65 6e74 6c79 2c20 6966   permanently, if
-00007770: 2074 6865 2063 6f70 7972 6967 6874 0d0a   the copyright..
-00007780: 686f 6c64 6572 2066 6169 6c73 2074 6f20  holder fails to 
-00007790: 6e6f 7469 6679 2079 6f75 206f 6620 7468  notify you of th
-000077a0: 6520 7669 6f6c 6174 696f 6e20 6279 2073  e violation by s
-000077b0: 6f6d 6520 7265 6173 6f6e 6162 6c65 206d  ome reasonable m
-000077c0: 6561 6e73 0d0a 7072 696f 7220 746f 2036  eans..prior to 6
-000077d0: 3020 6461 7973 2061 6674 6572 2074 6865  0 days after the
-000077e0: 2063 6573 7361 7469 6f6e 2e0d 0a0d 0a20   cessation..... 
-000077f0: 204d 6f72 656f 7665 722c 2079 6f75 7220   Moreover, your 
-00007800: 6c69 6365 6e73 6520 6672 6f6d 2061 2070  license from a p
-00007810: 6172 7469 6375 6c61 7220 636f 7079 7269  articular copyri
-00007820: 6768 7420 686f 6c64 6572 2069 730d 0a72  ght holder is..r
-00007830: 6569 6e73 7461 7465 6420 7065 726d 616e  einstated perman
-00007840: 656e 746c 7920 6966 2074 6865 2063 6f70  ently if the cop
-00007850: 7972 6967 6874 2068 6f6c 6465 7220 6e6f  yright holder no
-00007860: 7469 6669 6573 2079 6f75 206f 6620 7468  tifies you of th
-00007870: 650d 0a76 696f 6c61 7469 6f6e 2062 7920  e..violation by 
-00007880: 736f 6d65 2072 6561 736f 6e61 626c 6520  some reasonable 
-00007890: 6d65 616e 732c 2074 6869 7320 6973 2074  means, this is t
-000078a0: 6865 2066 6972 7374 2074 696d 6520 796f  he first time yo
-000078b0: 7520 6861 7665 0d0a 7265 6365 6976 6564  u have..received
-000078c0: 206e 6f74 6963 6520 6f66 2076 696f 6c61   notice of viola
-000078d0: 7469 6f6e 206f 6620 7468 6973 204c 6963  tion of this Lic
-000078e0: 656e 7365 2028 666f 7220 616e 7920 776f  ense (for any wo
-000078f0: 726b 2920 6672 6f6d 2074 6861 740d 0a63  rk) from that..c
-00007900: 6f70 7972 6967 6874 2068 6f6c 6465 722c  opyright holder,
-00007910: 2061 6e64 2079 6f75 2063 7572 6520 7468   and you cure th
-00007920: 6520 7669 6f6c 6174 696f 6e20 7072 696f  e violation prio
-00007930: 7220 746f 2033 3020 6461 7973 2061 6674  r to 30 days aft
-00007940: 6572 0d0a 796f 7572 2072 6563 6569 7074  er..your receipt
-00007950: 206f 6620 7468 6520 6e6f 7469 6365 2e0d   of the notice..
-00007960: 0a0d 0a20 2054 6572 6d69 6e61 7469 6f6e  ...  Termination
-00007970: 206f 6620 796f 7572 2072 6967 6874 7320   of your rights 
-00007980: 756e 6465 7220 7468 6973 2073 6563 7469  under this secti
-00007990: 6f6e 2064 6f65 7320 6e6f 7420 7465 726d  on does not term
-000079a0: 696e 6174 6520 7468 650d 0a6c 6963 656e  inate the..licen
-000079b0: 7365 7320 6f66 2070 6172 7469 6573 2077  ses of parties w
-000079c0: 686f 2068 6176 6520 7265 6365 6976 6564  ho have received
-000079d0: 2063 6f70 6965 7320 6f72 2072 6967 6874   copies or right
-000079e0: 7320 6672 6f6d 2079 6f75 2075 6e64 6572  s from you under
-000079f0: 0d0a 7468 6973 204c 6963 656e 7365 2e20  ..this License. 
-00007a00: 2049 6620 796f 7572 2072 6967 6874 7320   If your rights 
-00007a10: 6861 7665 2062 6565 6e20 7465 726d 696e  have been termin
-00007a20: 6174 6564 2061 6e64 206e 6f74 2070 6572  ated and not per
-00007a30: 6d61 6e65 6e74 6c79 0d0a 7265 696e 7374  manently..reinst
-00007a40: 6174 6564 2c20 796f 7520 646f 206e 6f74  ated, you do not
-00007a50: 2071 7561 6c69 6679 2074 6f20 7265 6365   qualify to rece
-00007a60: 6976 6520 6e65 7720 6c69 6365 6e73 6573  ive new licenses
-00007a70: 2066 6f72 2074 6865 2073 616d 650d 0a6d   for the same..m
-00007a80: 6174 6572 6961 6c20 756e 6465 7220 7365  aterial under se
-00007a90: 6374 696f 6e20 3130 2e0d 0a0d 0a20 2039  ction 10.....  9
-00007aa0: 2e20 4163 6365 7074 616e 6365 204e 6f74  . Acceptance Not
-00007ab0: 2052 6571 7569 7265 6420 666f 7220 4861   Required for Ha
-00007ac0: 7669 6e67 2043 6f70 6965 732e 0d0a 0d0a  ving Copies.....
-00007ad0: 2020 596f 7520 6172 6520 6e6f 7420 7265    You are not re
-00007ae0: 7175 6972 6564 2074 6f20 6163 6365 7074  quired to accept
-00007af0: 2074 6869 7320 4c69 6365 6e73 6520 696e   this License in
-00007b00: 206f 7264 6572 2074 6f20 7265 6365 6976   order to receiv
-00007b10: 6520 6f72 0d0a 7275 6e20 6120 636f 7079  e or..run a copy
-00007b20: 206f 6620 7468 6520 5072 6f67 7261 6d2e   of the Program.
-00007b30: 2020 416e 6369 6c6c 6172 7920 7072 6f70    Ancillary prop
-00007b40: 6167 6174 696f 6e20 6f66 2061 2063 6f76  agation of a cov
-00007b50: 6572 6564 2077 6f72 6b0d 0a6f 6363 7572  ered work..occur
-00007b60: 7269 6e67 2073 6f6c 656c 7920 6173 2061  ring solely as a
-00007b70: 2063 6f6e 7365 7175 656e 6365 206f 6620   consequence of 
-00007b80: 7573 696e 6720 7065 6572 2d74 6f2d 7065  using peer-to-pe
-00007b90: 6572 2074 7261 6e73 6d69 7373 696f 6e0d  er transmission.
-00007ba0: 0a74 6f20 7265 6365 6976 6520 6120 636f  .to receive a co
-00007bb0: 7079 206c 696b 6577 6973 6520 646f 6573  py likewise does
-00007bc0: 206e 6f74 2072 6571 7569 7265 2061 6363   not require acc
-00007bd0: 6570 7461 6e63 652e 2020 486f 7765 7665  eptance.  Howeve
-00007be0: 722c 0d0a 6e6f 7468 696e 6720 6f74 6865  r,..nothing othe
-00007bf0: 7220 7468 616e 2074 6869 7320 4c69 6365  r than this Lice
-00007c00: 6e73 6520 6772 616e 7473 2079 6f75 2070  nse grants you p
-00007c10: 6572 6d69 7373 696f 6e20 746f 2070 726f  ermission to pro
-00007c20: 7061 6761 7465 206f 720d 0a6d 6f64 6966  pagate or..modif
-00007c30: 7920 616e 7920 636f 7665 7265 6420 776f  y any covered wo
-00007c40: 726b 2e20 2054 6865 7365 2061 6374 696f  rk.  These actio
-00007c50: 6e73 2069 6e66 7269 6e67 6520 636f 7079  ns infringe copy
-00007c60: 7269 6768 7420 6966 2079 6f75 2064 6f0d  right if you do.
-00007c70: 0a6e 6f74 2061 6363 6570 7420 7468 6973  .not accept this
-00007c80: 204c 6963 656e 7365 2e20 2054 6865 7265   License.  There
-00007c90: 666f 7265 2c20 6279 206d 6f64 6966 7969  fore, by modifyi
-00007ca0: 6e67 206f 7220 7072 6f70 6167 6174 696e  ng or propagatin
-00007cb0: 6720 610d 0a63 6f76 6572 6564 2077 6f72  g a..covered wor
-00007cc0: 6b2c 2079 6f75 2069 6e64 6963 6174 6520  k, you indicate 
-00007cd0: 796f 7572 2061 6363 6570 7461 6e63 6520  your acceptance 
-00007ce0: 6f66 2074 6869 7320 4c69 6365 6e73 6520  of this License 
-00007cf0: 746f 2064 6f20 736f 2e0d 0a0d 0a20 2031  to do so.....  1
-00007d00: 302e 2041 7574 6f6d 6174 6963 204c 6963  0. Automatic Lic
-00007d10: 656e 7369 6e67 206f 6620 446f 776e 7374  ensing of Downst
-00007d20: 7265 616d 2052 6563 6970 6965 6e74 732e  ream Recipients.
-00007d30: 0d0a 0d0a 2020 4561 6368 2074 696d 6520  ....  Each time 
-00007d40: 796f 7520 636f 6e76 6579 2061 2063 6f76  you convey a cov
-00007d50: 6572 6564 2077 6f72 6b2c 2074 6865 2072  ered work, the r
-00007d60: 6563 6970 6965 6e74 2061 7574 6f6d 6174  ecipient automat
-00007d70: 6963 616c 6c79 0d0a 7265 6365 6976 6573  ically..receives
-00007d80: 2061 206c 6963 656e 7365 2066 726f 6d20   a license from 
-00007d90: 7468 6520 6f72 6967 696e 616c 206c 6963  the original lic
-00007da0: 656e 736f 7273 2c20 746f 2072 756e 2c20  ensors, to run, 
-00007db0: 6d6f 6469 6679 2061 6e64 0d0a 7072 6f70  modify and..prop
-00007dc0: 6167 6174 6520 7468 6174 2077 6f72 6b2c  agate that work,
-00007dd0: 2073 7562 6a65 6374 2074 6f20 7468 6973   subject to this
-00007de0: 204c 6963 656e 7365 2e20 2059 6f75 2061   License.  You a
-00007df0: 7265 206e 6f74 2072 6573 706f 6e73 6962  re not responsib
-00007e00: 6c65 0d0a 666f 7220 656e 666f 7263 696e  le..for enforcin
-00007e10: 6720 636f 6d70 6c69 616e 6365 2062 7920  g compliance by 
-00007e20: 7468 6972 6420 7061 7274 6965 7320 7769  third parties wi
-00007e30: 7468 2074 6869 7320 4c69 6365 6e73 652e  th this License.
-00007e40: 0d0a 0d0a 2020 416e 2022 656e 7469 7479  ....  An "entity
-00007e50: 2074 7261 6e73 6163 7469 6f6e 2220 6973   transaction" is
-00007e60: 2061 2074 7261 6e73 6163 7469 6f6e 2074   a transaction t
-00007e70: 7261 6e73 6665 7272 696e 6720 636f 6e74  ransferring cont
-00007e80: 726f 6c20 6f66 2061 6e0d 0a6f 7267 616e  rol of an..organ
-00007e90: 697a 6174 696f 6e2c 206f 7220 7375 6273  ization, or subs
-00007ea0: 7461 6e74 6961 6c6c 7920 616c 6c20 6173  tantially all as
-00007eb0: 7365 7473 206f 6620 6f6e 652c 206f 7220  sets of one, or 
-00007ec0: 7375 6264 6976 6964 696e 6720 616e 0d0a  subdividing an..
-00007ed0: 6f72 6761 6e69 7a61 7469 6f6e 2c20 6f72  organization, or
-00007ee0: 206d 6572 6769 6e67 206f 7267 616e 697a   merging organiz
-00007ef0: 6174 696f 6e73 2e20 2049 6620 7072 6f70  ations.  If prop
-00007f00: 6167 6174 696f 6e20 6f66 2061 2063 6f76  agation of a cov
-00007f10: 6572 6564 0d0a 776f 726b 2072 6573 756c  ered..work resul
-00007f20: 7473 2066 726f 6d20 616e 2065 6e74 6974  ts from an entit
-00007f30: 7920 7472 616e 7361 6374 696f 6e2c 2065  y transaction, e
-00007f40: 6163 6820 7061 7274 7920 746f 2074 6861  ach party to tha
-00007f50: 740d 0a74 7261 6e73 6163 7469 6f6e 2077  t..transaction w
-00007f60: 686f 2072 6563 6569 7665 7320 6120 636f  ho receives a co
-00007f70: 7079 206f 6620 7468 6520 776f 726b 2061  py of the work a
-00007f80: 6c73 6f20 7265 6365 6976 6573 2077 6861  lso receives wha
-00007f90: 7465 7665 720d 0a6c 6963 656e 7365 7320  tever..licenses 
-00007fa0: 746f 2074 6865 2077 6f72 6b20 7468 6520  to the work the 
-00007fb0: 7061 7274 7927 7320 7072 6564 6563 6573  party's predeces
-00007fc0: 736f 7220 696e 2069 6e74 6572 6573 7420  sor in interest 
-00007fd0: 6861 6420 6f72 2063 6f75 6c64 0d0a 6769  had or could..gi
-00007fe0: 7665 2075 6e64 6572 2074 6865 2070 7265  ve under the pre
-00007ff0: 7669 6f75 7320 7061 7261 6772 6170 682c  vious paragraph,
-00008000: 2070 6c75 7320 6120 7269 6768 7420 746f   plus a right to
-00008010: 2070 6f73 7365 7373 696f 6e20 6f66 2074   possession of t
-00008020: 6865 0d0a 436f 7272 6573 706f 6e64 696e  he..Correspondin
-00008030: 6720 536f 7572 6365 206f 6620 7468 6520  g Source of the 
-00008040: 776f 726b 2066 726f 6d20 7468 6520 7072  work from the pr
-00008050: 6564 6563 6573 736f 7220 696e 2069 6e74  edecessor in int
-00008060: 6572 6573 742c 2069 660d 0a74 6865 2070  erest, if..the p
-00008070: 7265 6465 6365 7373 6f72 2068 6173 2069  redecessor has i
-00008080: 7420 6f72 2063 616e 2067 6574 2069 7420  t or can get it 
-00008090: 7769 7468 2072 6561 736f 6e61 626c 6520  with reasonable 
-000080a0: 6566 666f 7274 732e 0d0a 0d0a 2020 596f  efforts.....  Yo
-000080b0: 7520 6d61 7920 6e6f 7420 696d 706f 7365  u may not impose
-000080c0: 2061 6e79 2066 7572 7468 6572 2072 6573   any further res
-000080d0: 7472 6963 7469 6f6e 7320 6f6e 2074 6865  trictions on the
-000080e0: 2065 7865 7263 6973 6520 6f66 2074 6865   exercise of the
-000080f0: 0d0a 7269 6768 7473 2067 7261 6e74 6564  ..rights granted
-00008100: 206f 7220 6166 6669 726d 6564 2075 6e64   or affirmed und
-00008110: 6572 2074 6869 7320 4c69 6365 6e73 652e  er this License.
-00008120: 2020 466f 7220 6578 616d 706c 652c 2079    For example, y
-00008130: 6f75 206d 6179 0d0a 6e6f 7420 696d 706f  ou may..not impo
-00008140: 7365 2061 206c 6963 656e 7365 2066 6565  se a license fee
-00008150: 2c20 726f 7961 6c74 792c 206f 7220 6f74  , royalty, or ot
-00008160: 6865 7220 6368 6172 6765 2066 6f72 2065  her charge for e
-00008170: 7865 7263 6973 6520 6f66 0d0a 7269 6768  xercise of..righ
-00008180: 7473 2067 7261 6e74 6564 2075 6e64 6572  ts granted under
-00008190: 2074 6869 7320 4c69 6365 6e73 652c 2061   this License, a
-000081a0: 6e64 2079 6f75 206d 6179 206e 6f74 2069  nd you may not i
-000081b0: 6e69 7469 6174 6520 6c69 7469 6761 7469  nitiate litigati
-000081c0: 6f6e 0d0a 2869 6e63 6c75 6469 6e67 2061  on..(including a
-000081d0: 2063 726f 7373 2d63 6c61 696d 206f 7220   cross-claim or 
-000081e0: 636f 756e 7465 7263 6c61 696d 2069 6e20  counterclaim in 
-000081f0: 6120 6c61 7773 7569 7429 2061 6c6c 6567  a lawsuit) alleg
-00008200: 696e 6720 7468 6174 0d0a 616e 7920 7061  ing that..any pa
-00008210: 7465 6e74 2063 6c61 696d 2069 7320 696e  tent claim is in
-00008220: 6672 696e 6765 6420 6279 206d 616b 696e  fringed by makin
-00008230: 672c 2075 7369 6e67 2c20 7365 6c6c 696e  g, using, sellin
-00008240: 672c 206f 6666 6572 696e 6720 666f 720d  g, offering for.
-00008250: 0a73 616c 652c 206f 7220 696d 706f 7274  .sale, or import
-00008260: 696e 6720 7468 6520 5072 6f67 7261 6d20  ing the Program 
-00008270: 6f72 2061 6e79 2070 6f72 7469 6f6e 206f  or any portion o
-00008280: 6620 6974 2e0d 0a0d 0a20 2031 312e 2050  f it.....  11. P
-00008290: 6174 656e 7473 2e0d 0a0d 0a20 2041 2022  atents.....  A "
-000082a0: 636f 6e74 7269 6275 746f 7222 2069 7320  contributor" is 
-000082b0: 6120 636f 7079 7269 6768 7420 686f 6c64  a copyright hold
-000082c0: 6572 2077 686f 2061 7574 686f 7269 7a65  er who authorize
-000082d0: 7320 7573 6520 756e 6465 7220 7468 6973  s use under this
-000082e0: 0d0a 4c69 6365 6e73 6520 6f66 2074 6865  ..License of the
-000082f0: 2050 726f 6772 616d 206f 7220 6120 776f   Program or a wo
-00008300: 726b 206f 6e20 7768 6963 6820 7468 6520  rk on which the 
-00008310: 5072 6f67 7261 6d20 6973 2062 6173 6564  Program is based
-00008320: 2e20 2054 6865 0d0a 776f 726b 2074 6875  .  The..work thu
-00008330: 7320 6c69 6365 6e73 6564 2069 7320 6361  s licensed is ca
-00008340: 6c6c 6564 2074 6865 2063 6f6e 7472 6962  lled the contrib
-00008350: 7574 6f72 2773 2022 636f 6e74 7269 6275  utor's "contribu
-00008360: 746f 7220 7665 7273 696f 6e22 2e0d 0a0d  tor version"....
-00008370: 0a20 2041 2063 6f6e 7472 6962 7574 6f72  .  A contributor
-00008380: 2773 2022 6573 7365 6e74 6961 6c20 7061  's "essential pa
-00008390: 7465 6e74 2063 6c61 696d 7322 2061 7265  tent claims" are
-000083a0: 2061 6c6c 2070 6174 656e 7420 636c 6169   all patent clai
-000083b0: 6d73 0d0a 6f77 6e65 6420 6f72 2063 6f6e  ms..owned or con
-000083c0: 7472 6f6c 6c65 6420 6279 2074 6865 2063  trolled by the c
-000083d0: 6f6e 7472 6962 7574 6f72 2c20 7768 6574  ontributor, whet
-000083e0: 6865 7220 616c 7265 6164 7920 6163 7175  her already acqu
-000083f0: 6972 6564 206f 720d 0a68 6572 6561 6674  ired or..hereaft
-00008400: 6572 2061 6371 7569 7265 642c 2074 6861  er acquired, tha
-00008410: 7420 776f 756c 6420 6265 2069 6e66 7269  t would be infri
-00008420: 6e67 6564 2062 7920 736f 6d65 206d 616e  nged by some man
-00008430: 6e65 722c 2070 6572 6d69 7474 6564 0d0a  ner, permitted..
-00008440: 6279 2074 6869 7320 4c69 6365 6e73 652c  by this License,
-00008450: 206f 6620 6d61 6b69 6e67 2c20 7573 696e   of making, usin
-00008460: 672c 206f 7220 7365 6c6c 696e 6720 6974  g, or selling it
-00008470: 7320 636f 6e74 7269 6275 746f 7220 7665  s contributor ve
-00008480: 7273 696f 6e2c 0d0a 6275 7420 646f 206e  rsion,..but do n
-00008490: 6f74 2069 6e63 6c75 6465 2063 6c61 696d  ot include claim
-000084a0: 7320 7468 6174 2077 6f75 6c64 2062 6520  s that would be 
-000084b0: 696e 6672 696e 6765 6420 6f6e 6c79 2061  infringed only a
-000084c0: 7320 610d 0a63 6f6e 7365 7175 656e 6365  s a..consequence
-000084d0: 206f 6620 6675 7274 6865 7220 6d6f 6469   of further modi
-000084e0: 6669 6361 7469 6f6e 206f 6620 7468 6520  fication of the 
-000084f0: 636f 6e74 7269 6275 746f 7220 7665 7273  contributor vers
-00008500: 696f 6e2e 2020 466f 720d 0a70 7572 706f  ion.  For..purpo
-00008510: 7365 7320 6f66 2074 6869 7320 6465 6669  ses of this defi
-00008520: 6e69 7469 6f6e 2c20 2263 6f6e 7472 6f6c  nition, "control
-00008530: 2220 696e 636c 7564 6573 2074 6865 2072  " includes the r
-00008540: 6967 6874 2074 6f20 6772 616e 740d 0a70  ight to grant..p
-00008550: 6174 656e 7420 7375 626c 6963 656e 7365  atent sublicense
-00008560: 7320 696e 2061 206d 616e 6e65 7220 636f  s in a manner co
-00008570: 6e73 6973 7465 6e74 2077 6974 6820 7468  nsistent with th
-00008580: 6520 7265 7175 6972 656d 656e 7473 206f  e requirements o
-00008590: 660d 0a74 6869 7320 4c69 6365 6e73 652e  f..this License.
-000085a0: 0d0a 0d0a 2020 4561 6368 2063 6f6e 7472  ....  Each contr
-000085b0: 6962 7574 6f72 2067 7261 6e74 7320 796f  ibutor grants yo
-000085c0: 7520 6120 6e6f 6e2d 6578 636c 7573 6976  u a non-exclusiv
-000085d0: 652c 2077 6f72 6c64 7769 6465 2c20 726f  e, worldwide, ro
-000085e0: 7961 6c74 792d 6672 6565 0d0a 7061 7465  yalty-free..pate
-000085f0: 6e74 206c 6963 656e 7365 2075 6e64 6572  nt license under
-00008600: 2074 6865 2063 6f6e 7472 6962 7574 6f72   the contributor
-00008610: 2773 2065 7373 656e 7469 616c 2070 6174  's essential pat
-00008620: 656e 7420 636c 6169 6d73 2c20 746f 0d0a  ent claims, to..
-00008630: 6d61 6b65 2c20 7573 652c 2073 656c 6c2c  make, use, sell,
-00008640: 206f 6666 6572 2066 6f72 2073 616c 652c   offer for sale,
-00008650: 2069 6d70 6f72 7420 616e 6420 6f74 6865   import and othe
-00008660: 7277 6973 6520 7275 6e2c 206d 6f64 6966  rwise run, modif
-00008670: 7920 616e 640d 0a70 726f 7061 6761 7465  y and..propagate
-00008680: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
-00008690: 2069 7473 2063 6f6e 7472 6962 7574 6f72   its contributor
-000086a0: 2076 6572 7369 6f6e 2e0d 0a0d 0a20 2049   version.....  I
-000086b0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-000086c0: 7468 7265 6520 7061 7261 6772 6170 6873  three paragraphs
-000086d0: 2c20 6120 2270 6174 656e 7420 6c69 6365  , a "patent lice
-000086e0: 6e73 6522 2069 7320 616e 7920 6578 7072  nse" is any expr
-000086f0: 6573 730d 0a61 6772 6565 6d65 6e74 206f  ess..agreement o
-00008700: 7220 636f 6d6d 6974 6d65 6e74 2c20 686f  r commitment, ho
-00008710: 7765 7665 7220 6465 6e6f 6d69 6e61 7465  wever denominate
-00008720: 642c 206e 6f74 2074 6f20 656e 666f 7263  d, not to enforc
-00008730: 6520 6120 7061 7465 6e74 0d0a 2873 7563  e a patent..(suc
-00008740: 6820 6173 2061 6e20 6578 7072 6573 7320  h as an express 
-00008750: 7065 726d 6973 7369 6f6e 2074 6f20 7072  permission to pr
-00008760: 6163 7469 6365 2061 2070 6174 656e 7420  actice a patent 
-00008770: 6f72 2063 6f76 656e 616e 7420 6e6f 7420  or covenant not 
-00008780: 746f 0d0a 7375 6520 666f 7220 7061 7465  to..sue for pate
-00008790: 6e74 2069 6e66 7269 6e67 656d 656e 7429  nt infringement)
-000087a0: 2e20 2054 6f20 2267 7261 6e74 2220 7375  .  To "grant" su
-000087b0: 6368 2061 2070 6174 656e 7420 6c69 6365  ch a patent lice
-000087c0: 6e73 6520 746f 2061 0d0a 7061 7274 7920  nse to a..party 
-000087d0: 6d65 616e 7320 746f 206d 616b 6520 7375  means to make su
-000087e0: 6368 2061 6e20 6167 7265 656d 656e 7420  ch an agreement 
-000087f0: 6f72 2063 6f6d 6d69 746d 656e 7420 6e6f  or commitment no
-00008800: 7420 746f 2065 6e66 6f72 6365 2061 0d0a  t to enforce a..
-00008810: 7061 7465 6e74 2061 6761 696e 7374 2074  patent against t
-00008820: 6865 2070 6172 7479 2e0d 0a0d 0a20 2049  he party.....  I
-00008830: 6620 796f 7520 636f 6e76 6579 2061 2063  f you convey a c
-00008840: 6f76 6572 6564 2077 6f72 6b2c 206b 6e6f  overed work, kno
-00008850: 7769 6e67 6c79 2072 656c 7969 6e67 206f  wingly relying o
-00008860: 6e20 6120 7061 7465 6e74 206c 6963 656e  n a patent licen
-00008870: 7365 2c0d 0a61 6e64 2074 6865 2043 6f72  se,..and the Cor
-00008880: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
-00008890: 6520 6f66 2074 6865 2077 6f72 6b20 6973  e of the work is
-000088a0: 206e 6f74 2061 7661 696c 6162 6c65 2066   not available f
-000088b0: 6f72 2061 6e79 6f6e 650d 0a74 6f20 636f  or anyone..to co
-000088c0: 7079 2c20 6672 6565 206f 6620 6368 6172  py, free of char
-000088d0: 6765 2061 6e64 2075 6e64 6572 2074 6865  ge and under the
-000088e0: 2074 6572 6d73 206f 6620 7468 6973 204c   terms of this L
-000088f0: 6963 656e 7365 2c20 7468 726f 7567 6820  icense, through 
-00008900: 610d 0a70 7562 6c69 636c 7920 6176 6169  a..publicly avai
-00008910: 6c61 626c 6520 6e65 7477 6f72 6b20 7365  lable network se
-00008920: 7276 6572 206f 7220 6f74 6865 7220 7265  rver or other re
-00008930: 6164 696c 7920 6163 6365 7373 6962 6c65  adily accessible
-00008940: 206d 6561 6e73 2c0d 0a74 6865 6e20 796f   means,..then yo
-00008950: 7520 6d75 7374 2065 6974 6865 7220 2831  u must either (1
-00008960: 2920 6361 7573 6520 7468 6520 436f 7272  ) cause the Corr
-00008970: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
-00008980: 2074 6f20 6265 2073 6f0d 0a61 7661 696c   to be so..avail
-00008990: 6162 6c65 2c20 6f72 2028 3229 2061 7272  able, or (2) arr
-000089a0: 616e 6765 2074 6f20 6465 7072 6976 6520  ange to deprive 
-000089b0: 796f 7572 7365 6c66 206f 6620 7468 6520  yourself of the 
-000089c0: 6265 6e65 6669 7420 6f66 2074 6865 0d0a  benefit of the..
-000089d0: 7061 7465 6e74 206c 6963 656e 7365 2066  patent license f
-000089e0: 6f72 2074 6869 7320 7061 7274 6963 756c  or this particul
-000089f0: 6172 2077 6f72 6b2c 206f 7220 2833 2920  ar work, or (3) 
-00008a00: 6172 7261 6e67 652c 2069 6e20 6120 6d61  arrange, in a ma
-00008a10: 6e6e 6572 0d0a 636f 6e73 6973 7465 6e74  nner..consistent
-00008a20: 2077 6974 6820 7468 6520 7265 7175 6972   with the requir
-00008a30: 656d 656e 7473 206f 6620 7468 6973 204c  ements of this L
-00008a40: 6963 656e 7365 2c20 746f 2065 7874 656e  icense, to exten
-00008a50: 6420 7468 6520 7061 7465 6e74 0d0a 6c69  d the patent..li
-00008a60: 6365 6e73 6520 746f 2064 6f77 6e73 7472  cense to downstr
-00008a70: 6561 6d20 7265 6369 7069 656e 7473 2e20  eam recipients. 
-00008a80: 2022 4b6e 6f77 696e 676c 7920 7265 6c79   "Knowingly rely
-00008a90: 696e 6722 206d 6561 6e73 2079 6f75 2068  ing" means you h
-00008aa0: 6176 650d 0a61 6374 7561 6c20 6b6e 6f77  ave..actual know
-00008ab0: 6c65 6467 6520 7468 6174 2c20 6275 7420  ledge that, but 
-00008ac0: 666f 7220 7468 6520 7061 7465 6e74 206c  for the patent l
-00008ad0: 6963 656e 7365 2c20 796f 7572 2063 6f6e  icense, your con
-00008ae0: 7665 7969 6e67 2074 6865 0d0a 636f 7665  veying the..cove
-00008af0: 7265 6420 776f 726b 2069 6e20 6120 636f  red work in a co
-00008b00: 756e 7472 792c 206f 7220 796f 7572 2072  untry, or your r
-00008b10: 6563 6970 6965 6e74 2773 2075 7365 206f  ecipient's use o
-00008b20: 6620 7468 6520 636f 7665 7265 6420 776f  f the covered wo
-00008b30: 726b 0d0a 696e 2061 2063 6f75 6e74 7279  rk..in a country
-00008b40: 2c20 776f 756c 6420 696e 6672 696e 6765  , would infringe
-00008b50: 206f 6e65 206f 7220 6d6f 7265 2069 6465   one or more ide
-00008b60: 6e74 6966 6961 626c 6520 7061 7465 6e74  ntifiable patent
-00008b70: 7320 696e 2074 6861 740d 0a63 6f75 6e74  s in that..count
-00008b80: 7279 2074 6861 7420 796f 7520 6861 7665  ry that you have
-00008b90: 2072 6561 736f 6e20 746f 2062 656c 6965   reason to belie
-00008ba0: 7665 2061 7265 2076 616c 6964 2e0d 0a0d  ve are valid....
-00008bb0: 0a20 2049 662c 2070 7572 7375 616e 7420  .  If, pursuant 
-00008bc0: 746f 206f 7220 696e 2063 6f6e 6e65 6374  to or in connect
-00008bd0: 696f 6e20 7769 7468 2061 2073 696e 676c  ion with a singl
-00008be0: 6520 7472 616e 7361 6374 696f 6e20 6f72  e transaction or
-00008bf0: 0d0a 6172 7261 6e67 656d 656e 742c 2079  ..arrangement, y
-00008c00: 6f75 2063 6f6e 7665 792c 206f 7220 7072  ou convey, or pr
-00008c10: 6f70 6167 6174 6520 6279 2070 726f 6375  opagate by procu
-00008c20: 7269 6e67 2063 6f6e 7665 7961 6e63 6520  ring conveyance 
-00008c30: 6f66 2c20 610d 0a63 6f76 6572 6564 2077  of, a..covered w
-00008c40: 6f72 6b2c 2061 6e64 2067 7261 6e74 2061  ork, and grant a
-00008c50: 2070 6174 656e 7420 6c69 6365 6e73 6520   patent license 
-00008c60: 746f 2073 6f6d 6520 6f66 2074 6865 2070  to some of the p
-00008c70: 6172 7469 6573 0d0a 7265 6365 6976 696e  arties..receivin
-00008c80: 6720 7468 6520 636f 7665 7265 6420 776f  g the covered wo
-00008c90: 726b 2061 7574 686f 7269 7a69 6e67 2074  rk authorizing t
-00008ca0: 6865 6d20 746f 2075 7365 2c20 7072 6f70  hem to use, prop
-00008cb0: 6167 6174 652c 206d 6f64 6966 790d 0a6f  agate, modify..o
-00008cc0: 7220 636f 6e76 6579 2061 2073 7065 6369  r convey a speci
-00008cd0: 6669 6320 636f 7079 206f 6620 7468 6520  fic copy of the 
-00008ce0: 636f 7665 7265 6420 776f 726b 2c20 7468  covered work, th
-00008cf0: 656e 2074 6865 2070 6174 656e 7420 6c69  en the patent li
-00008d00: 6365 6e73 650d 0a79 6f75 2067 7261 6e74  cense..you grant
-00008d10: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
-00008d20: 7920 6578 7465 6e64 6564 2074 6f20 616c  y extended to al
-00008d30: 6c20 7265 6369 7069 656e 7473 206f 6620  l recipients of 
-00008d40: 7468 6520 636f 7665 7265 640d 0a77 6f72  the covered..wor
-00008d50: 6b20 616e 6420 776f 726b 7320 6261 7365  k and works base
-00008d60: 6420 6f6e 2069 742e 0d0a 0d0a 2020 4120  d on it.....  A 
-00008d70: 7061 7465 6e74 206c 6963 656e 7365 2069  patent license i
-00008d80: 7320 2264 6973 6372 696d 696e 6174 6f72  s "discriminator
-00008d90: 7922 2069 6620 6974 2064 6f65 7320 6e6f  y" if it does no
-00008da0: 7420 696e 636c 7564 6520 7769 7468 696e  t include within
-00008db0: 0d0a 7468 6520 7363 6f70 6520 6f66 2069  ..the scope of i
-00008dc0: 7473 2063 6f76 6572 6167 652c 2070 726f  ts coverage, pro
-00008dd0: 6869 6269 7473 2074 6865 2065 7865 7263  hibits the exerc
-00008de0: 6973 6520 6f66 2c20 6f72 2069 730d 0a63  ise of, or is..c
-00008df0: 6f6e 6469 7469 6f6e 6564 206f 6e20 7468  onditioned on th
-00008e00: 6520 6e6f 6e2d 6578 6572 6369 7365 206f  e non-exercise o
-00008e10: 6620 6f6e 6520 6f72 206d 6f72 6520 6f66  f one or more of
-00008e20: 2074 6865 2072 6967 6874 7320 7468 6174   the rights that
-00008e30: 2061 7265 0d0a 7370 6563 6966 6963 616c   are..specifical
-00008e40: 6c79 2067 7261 6e74 6564 2075 6e64 6572  ly granted under
-00008e50: 2074 6869 7320 4c69 6365 6e73 652e 2020   this License.  
-00008e60: 596f 7520 6d61 7920 6e6f 7420 636f 6e76  You may not conv
-00008e70: 6579 2061 2063 6f76 6572 6564 0d0a 776f  ey a covered..wo
-00008e80: 726b 2069 6620 796f 7520 6172 6520 6120  rk if you are a 
-00008e90: 7061 7274 7920 746f 2061 6e20 6172 7261  party to an arra
-00008ea0: 6e67 656d 656e 7420 7769 7468 2061 2074  ngement with a t
-00008eb0: 6869 7264 2070 6172 7479 2074 6861 7420  hird party that 
-00008ec0: 6973 0d0a 696e 2074 6865 2062 7573 696e  is..in the busin
-00008ed0: 6573 7320 6f66 2064 6973 7472 6962 7574  ess of distribut
-00008ee0: 696e 6720 736f 6674 7761 7265 2c20 756e  ing software, un
-00008ef0: 6465 7220 7768 6963 6820 796f 7520 6d61  der which you ma
-00008f00: 6b65 2070 6179 6d65 6e74 0d0a 746f 2074  ke payment..to t
-00008f10: 6865 2074 6869 7264 2070 6172 7479 2062  he third party b
-00008f20: 6173 6564 206f 6e20 7468 6520 6578 7465  ased on the exte
-00008f30: 6e74 206f 6620 796f 7572 2061 6374 6976  nt of your activ
-00008f40: 6974 7920 6f66 2063 6f6e 7665 7969 6e67  ity of conveying
-00008f50: 0d0a 7468 6520 776f 726b 2c20 616e 6420  ..the work, and 
-00008f60: 756e 6465 7220 7768 6963 6820 7468 6520  under which the 
-00008f70: 7468 6972 6420 7061 7274 7920 6772 616e  third party gran
-00008f80: 7473 2c20 746f 2061 6e79 206f 6620 7468  ts, to any of th
-00008f90: 650d 0a70 6172 7469 6573 2077 686f 2077  e..parties who w
-00008fa0: 6f75 6c64 2072 6563 6569 7665 2074 6865  ould receive the
-00008fb0: 2063 6f76 6572 6564 2077 6f72 6b20 6672   covered work fr
-00008fc0: 6f6d 2079 6f75 2c20 6120 6469 7363 7269  om you, a discri
-00008fd0: 6d69 6e61 746f 7279 0d0a 7061 7465 6e74  minatory..patent
-00008fe0: 206c 6963 656e 7365 2028 6129 2069 6e20   license (a) in 
-00008ff0: 636f 6e6e 6563 7469 6f6e 2077 6974 6820  connection with 
-00009000: 636f 7069 6573 206f 6620 7468 6520 636f  copies of the co
-00009010: 7665 7265 6420 776f 726b 0d0a 636f 6e76  vered work..conv
-00009020: 6579 6564 2062 7920 796f 7520 286f 7220  eyed by you (or 
-00009030: 636f 7069 6573 206d 6164 6520 6672 6f6d  copies made from
-00009040: 2074 686f 7365 2063 6f70 6965 7329 2c20   those copies), 
-00009050: 6f72 2028 6229 2070 7269 6d61 7269 6c79  or (b) primarily
-00009060: 0d0a 666f 7220 616e 6420 696e 2063 6f6e  ..for and in con
-00009070: 6e65 6374 696f 6e20 7769 7468 2073 7065  nection with spe
-00009080: 6369 6669 6320 7072 6f64 7563 7473 206f  cific products o
-00009090: 7220 636f 6d70 696c 6174 696f 6e73 2074  r compilations t
-000090a0: 6861 740d 0a63 6f6e 7461 696e 2074 6865  hat..contain the
-000090b0: 2063 6f76 6572 6564 2077 6f72 6b2c 2075   covered work, u
-000090c0: 6e6c 6573 7320 796f 7520 656e 7465 7265  nless you entere
-000090d0: 6420 696e 746f 2074 6861 7420 6172 7261  d into that arra
-000090e0: 6e67 656d 656e 742c 0d0a 6f72 2074 6861  ngement,..or tha
-000090f0: 7420 7061 7465 6e74 206c 6963 656e 7365  t patent license
-00009100: 2077 6173 2067 7261 6e74 6564 2c20 7072   was granted, pr
-00009110: 696f 7220 746f 2032 3820 4d61 7263 6820  ior to 28 March 
-00009120: 3230 3037 2e0d 0a0d 0a20 204e 6f74 6869  2007.....  Nothi
-00009130: 6e67 2069 6e20 7468 6973 204c 6963 656e  ng in this Licen
-00009140: 7365 2073 6861 6c6c 2062 6520 636f 6e73  se shall be cons
-00009150: 7472 7565 6420 6173 2065 7863 6c75 6469  trued as excludi
-00009160: 6e67 206f 7220 6c69 6d69 7469 6e67 0d0a  ng or limiting..
-00009170: 616e 7920 696d 706c 6965 6420 6c69 6365  any implied lice
-00009180: 6e73 6520 6f72 206f 7468 6572 2064 6566  nse or other def
-00009190: 656e 7365 7320 746f 2069 6e66 7269 6e67  enses to infring
-000091a0: 656d 656e 7420 7468 6174 206d 6179 0d0a  ement that may..
-000091b0: 6f74 6865 7277 6973 6520 6265 2061 7661  otherwise be ava
-000091c0: 696c 6162 6c65 2074 6f20 796f 7520 756e  ilable to you un
-000091d0: 6465 7220 6170 706c 6963 6162 6c65 2070  der applicable p
-000091e0: 6174 656e 7420 6c61 772e 0d0a 0d0a 2020  atent law.....  
-000091f0: 3132 2e20 4e6f 2053 7572 7265 6e64 6572  12. No Surrender
-00009200: 206f 6620 4f74 6865 7273 2720 4672 6565   of Others' Free
-00009210: 646f 6d2e 0d0a 0d0a 2020 4966 2063 6f6e  dom.....  If con
-00009220: 6469 7469 6f6e 7320 6172 6520 696d 706f  ditions are impo
-00009230: 7365 6420 6f6e 2079 6f75 2028 7768 6574  sed on you (whet
-00009240: 6865 7220 6279 2063 6f75 7274 206f 7264  her by court ord
-00009250: 6572 2c20 6167 7265 656d 656e 7420 6f72  er, agreement or
-00009260: 0d0a 6f74 6865 7277 6973 6529 2074 6861  ..otherwise) tha
-00009270: 7420 636f 6e74 7261 6469 6374 2074 6865  t contradict the
-00009280: 2063 6f6e 6469 7469 6f6e 7320 6f66 2074   conditions of t
-00009290: 6869 7320 4c69 6365 6e73 652c 2074 6865  his License, the
-000092a0: 7920 646f 206e 6f74 0d0a 6578 6375 7365  y do not..excuse
-000092b0: 2079 6f75 2066 726f 6d20 7468 6520 636f   you from the co
-000092c0: 6e64 6974 696f 6e73 206f 6620 7468 6973  nditions of this
-000092d0: 204c 6963 656e 7365 2e20 2049 6620 796f   License.  If yo
-000092e0: 7520 6361 6e6e 6f74 2063 6f6e 7665 7920  u cannot convey 
-000092f0: 610d 0a63 6f76 6572 6564 2077 6f72 6b20  a..covered work 
-00009300: 736f 2061 7320 746f 2073 6174 6973 6679  so as to satisfy
-00009310: 2073 696d 756c 7461 6e65 6f75 736c 7920   simultaneously 
-00009320: 796f 7572 206f 626c 6967 6174 696f 6e73  your obligations
-00009330: 2075 6e64 6572 2074 6869 730d 0a4c 6963   under this..Lic
-00009340: 656e 7365 2061 6e64 2061 6e79 206f 7468  ense and any oth
-00009350: 6572 2070 6572 7469 6e65 6e74 206f 626c  er pertinent obl
-00009360: 6967 6174 696f 6e73 2c20 7468 656e 2061  igations, then a
-00009370: 7320 6120 636f 6e73 6571 7565 6e63 6520  s a consequence 
-00009380: 796f 7520 6d61 790d 0a6e 6f74 2063 6f6e  you may..not con
-00009390: 7665 7920 6974 2061 7420 616c 6c2e 2020  vey it at all.  
-000093a0: 466f 7220 6578 616d 706c 652c 2069 6620  For example, if 
-000093b0: 796f 7520 6167 7265 6520 746f 2074 6572  you agree to ter
-000093c0: 6d73 2074 6861 7420 6f62 6c69 6761 7465  ms that obligate
-000093d0: 2079 6f75 0d0a 746f 2063 6f6c 6c65 6374   you..to collect
-000093e0: 2061 2072 6f79 616c 7479 2066 6f72 2066   a royalty for f
-000093f0: 7572 7468 6572 2063 6f6e 7665 7969 6e67  urther conveying
-00009400: 2066 726f 6d20 7468 6f73 6520 746f 2077   from those to w
-00009410: 686f 6d20 796f 7520 636f 6e76 6579 0d0a  hom you convey..
-00009420: 7468 6520 5072 6f67 7261 6d2c 2074 6865  the Program, the
-00009430: 206f 6e6c 7920 7761 7920 796f 7520 636f   only way you co
-00009440: 756c 6420 7361 7469 7366 7920 626f 7468  uld satisfy both
-00009450: 2074 686f 7365 2074 6572 6d73 2061 6e64   those terms and
-00009460: 2074 6869 730d 0a4c 6963 656e 7365 2077   this..License w
-00009470: 6f75 6c64 2062 6520 746f 2072 6566 7261  ould be to refra
-00009480: 696e 2065 6e74 6972 656c 7920 6672 6f6d  in entirely from
-00009490: 2063 6f6e 7665 7969 6e67 2074 6865 2050   conveying the P
-000094a0: 726f 6772 616d 2e0d 0a0d 0a20 2031 332e  rogram.....  13.
-000094b0: 2055 7365 2077 6974 6820 7468 6520 474e   Use with the GN
-000094c0: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
-000094d0: 2050 7562 6c69 6320 4c69 6365 6e73 652e   Public License.
-000094e0: 0d0a 0d0a 2020 4e6f 7477 6974 6873 7461  ....  Notwithsta
-000094f0: 6e64 696e 6720 616e 7920 6f74 6865 7220  nding any other 
-00009500: 7072 6f76 6973 696f 6e20 6f66 2074 6869  provision of thi
-00009510: 7320 4c69 6365 6e73 652c 2079 6f75 2068  s License, you h
-00009520: 6176 650d 0a70 6572 6d69 7373 696f 6e20  ave..permission 
-00009530: 746f 206c 696e 6b20 6f72 2063 6f6d 6269  to link or combi
-00009540: 6e65 2061 6e79 2063 6f76 6572 6564 2077  ne any covered w
-00009550: 6f72 6b20 7769 7468 2061 2077 6f72 6b20  ork with a work 
-00009560: 6c69 6365 6e73 6564 0d0a 756e 6465 7220  licensed..under 
-00009570: 7665 7273 696f 6e20 3320 6f66 2074 6865  version 3 of the
-00009580: 2047 4e55 2041 6666 6572 6f20 4765 6e65   GNU Affero Gene
-00009590: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
-000095a0: 7365 2069 6e74 6f20 6120 7369 6e67 6c65  se into a single
-000095b0: 0d0a 636f 6d62 696e 6564 2077 6f72 6b2c  ..combined work,
-000095c0: 2061 6e64 2074 6f20 636f 6e76 6579 2074   and to convey t
-000095d0: 6865 2072 6573 756c 7469 6e67 2077 6f72  he resulting wor
-000095e0: 6b2e 2020 5468 6520 7465 726d 7320 6f66  k.  The terms of
-000095f0: 2074 6869 730d 0a4c 6963 656e 7365 2077   this..License w
-00009600: 696c 6c20 636f 6e74 696e 7565 2074 6f20  ill continue to 
-00009610: 6170 706c 7920 746f 2074 6865 2070 6172  apply to the par
-00009620: 7420 7768 6963 6820 6973 2074 6865 2063  t which is the c
-00009630: 6f76 6572 6564 2077 6f72 6b2c 0d0a 6275  overed work,..bu
-00009640: 7420 7468 6520 7370 6563 6961 6c20 7265  t the special re
-00009650: 7175 6972 656d 656e 7473 206f 6620 7468  quirements of th
-00009660: 6520 474e 5520 4166 6665 726f 2047 656e  e GNU Affero Gen
-00009670: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00009680: 6e73 652c 0d0a 7365 6374 696f 6e20 3133  nse,..section 13
-00009690: 2c20 636f 6e63 6572 6e69 6e67 2069 6e74  , concerning int
-000096a0: 6572 6163 7469 6f6e 2074 6872 6f75 6768  eraction through
-000096b0: 2061 206e 6574 776f 726b 2077 696c 6c20   a network will 
-000096c0: 6170 706c 7920 746f 2074 6865 0d0a 636f  apply to the..co
-000096d0: 6d62 696e 6174 696f 6e20 6173 2073 7563  mbination as suc
-000096e0: 682e 0d0a 0d0a 2020 3134 2e20 5265 7669  h.....  14. Revi
-000096f0: 7365 6420 5665 7273 696f 6e73 206f 6620  sed Versions of 
-00009700: 7468 6973 204c 6963 656e 7365 2e0d 0a0d  this License....
-00009710: 0a20 2054 6865 2046 7265 6520 536f 6674  .  The Free Soft
-00009720: 7761 7265 2046 6f75 6e64 6174 696f 6e20  ware Foundation 
-00009730: 6d61 7920 7075 626c 6973 6820 7265 7669  may publish revi
-00009740: 7365 6420 616e 642f 6f72 206e 6577 2076  sed and/or new v
-00009750: 6572 7369 6f6e 7320 6f66 0d0a 7468 6520  ersions of..the 
-00009760: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
-00009770: 6963 204c 6963 656e 7365 2066 726f 6d20  ic License from 
-00009780: 7469 6d65 2074 6f20 7469 6d65 2e20 2053  time to time.  S
-00009790: 7563 6820 6e65 7720 7665 7273 696f 6e73  uch new versions
-000097a0: 2077 696c 6c0d 0a62 6520 7369 6d69 6c61   will..be simila
-000097b0: 7220 696e 2073 7069 7269 7420 746f 2074  r in spirit to t
-000097c0: 6865 2070 7265 7365 6e74 2076 6572 7369  he present versi
-000097d0: 6f6e 2c20 6275 7420 6d61 7920 6469 6666  on, but may diff
-000097e0: 6572 2069 6e20 6465 7461 696c 2074 6f0d  er in detail to.
-000097f0: 0a61 6464 7265 7373 206e 6577 2070 726f  .address new pro
-00009800: 626c 656d 7320 6f72 2063 6f6e 6365 726e  blems or concern
-00009810: 732e 0d0a 0d0a 2020 4561 6368 2076 6572  s.....  Each ver
-00009820: 7369 6f6e 2069 7320 6769 7665 6e20 6120  sion is given a 
-00009830: 6469 7374 696e 6775 6973 6869 6e67 2076  distinguishing v
-00009840: 6572 7369 6f6e 206e 756d 6265 722e 2020  ersion number.  
-00009850: 4966 2074 6865 0d0a 5072 6f67 7261 6d20  If the..Program 
-00009860: 7370 6563 6966 6965 7320 7468 6174 2061  specifies that a
-00009870: 2063 6572 7461 696e 206e 756d 6265 7265   certain numbere
-00009880: 6420 7665 7273 696f 6e20 6f66 2074 6865  d version of the
-00009890: 2047 4e55 2047 656e 6572 616c 0d0a 5075   GNU General..Pu
-000098a0: 626c 6963 204c 6963 656e 7365 2022 6f72  blic License "or
-000098b0: 2061 6e79 206c 6174 6572 2076 6572 7369   any later versi
-000098c0: 6f6e 2220 6170 706c 6965 7320 746f 2069  on" applies to i
-000098d0: 742c 2079 6f75 2068 6176 6520 7468 650d  t, you have the.
-000098e0: 0a6f 7074 696f 6e20 6f66 2066 6f6c 6c6f  .option of follo
-000098f0: 7769 6e67 2074 6865 2074 6572 6d73 2061  wing the terms a
-00009900: 6e64 2063 6f6e 6469 7469 6f6e 7320 6569  nd conditions ei
-00009910: 7468 6572 206f 6620 7468 6174 206e 756d  ther of that num
-00009920: 6265 7265 640d 0a76 6572 7369 6f6e 206f  bered..version o
-00009930: 7220 6f66 2061 6e79 206c 6174 6572 2076  r of any later v
-00009940: 6572 7369 6f6e 2070 7562 6c69 7368 6564  ersion published
-00009950: 2062 7920 7468 6520 4672 6565 2053 6f66   by the Free Sof
-00009960: 7477 6172 650d 0a46 6f75 6e64 6174 696f  tware..Foundatio
-00009970: 6e2e 2020 4966 2074 6865 2050 726f 6772  n.  If the Progr
-00009980: 616d 2064 6f65 7320 6e6f 7420 7370 6563  am does not spec
-00009990: 6966 7920 6120 7665 7273 696f 6e20 6e75  ify a version nu
-000099a0: 6d62 6572 206f 6620 7468 650d 0a47 4e55  mber of the..GNU
-000099b0: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
-000099c0: 4c69 6365 6e73 652c 2079 6f75 206d 6179  License, you may
-000099d0: 2063 686f 6f73 6520 616e 7920 7665 7273   choose any vers
-000099e0: 696f 6e20 6576 6572 2070 7562 6c69 7368  ion ever publish
-000099f0: 6564 0d0a 6279 2074 6865 2046 7265 6520  ed..by the Free 
-00009a00: 536f 6674 7761 7265 2046 6f75 6e64 6174  Software Foundat
-00009a10: 696f 6e2e 0d0a 0d0a 2020 4966 2074 6865  ion.....  If the
-00009a20: 2050 726f 6772 616d 2073 7065 6369 6669   Program specifi
-00009a30: 6573 2074 6861 7420 6120 7072 6f78 7920  es that a proxy 
-00009a40: 6361 6e20 6465 6369 6465 2077 6869 6368  can decide which
-00009a50: 2066 7574 7572 650d 0a76 6572 7369 6f6e   future..version
-00009a60: 7320 6f66 2074 6865 2047 4e55 2047 656e  s of the GNU Gen
-00009a70: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-00009a80: 6e73 6520 6361 6e20 6265 2075 7365 642c  nse can be used,
-00009a90: 2074 6861 7420 7072 6f78 7927 730d 0a70   that proxy's..p
-00009aa0: 7562 6c69 6320 7374 6174 656d 656e 7420  ublic statement 
-00009ab0: 6f66 2061 6363 6570 7461 6e63 6520 6f66  of acceptance of
-00009ac0: 2061 2076 6572 7369 6f6e 2070 6572 6d61   a version perma
-00009ad0: 6e65 6e74 6c79 2061 7574 686f 7269 7a65  nently authorize
-00009ae0: 7320 796f 750d 0a74 6f20 6368 6f6f 7365  s you..to choose
-00009af0: 2074 6861 7420 7665 7273 696f 6e20 666f   that version fo
-00009b00: 7220 7468 6520 5072 6f67 7261 6d2e 0d0a  r the Program...
-00009b10: 0d0a 2020 4c61 7465 7220 6c69 6365 6e73  ..  Later licens
-00009b20: 6520 7665 7273 696f 6e73 206d 6179 2067  e versions may g
-00009b30: 6976 6520 796f 7520 6164 6469 7469 6f6e  ive you addition
-00009b40: 616c 206f 7220 6469 6666 6572 656e 740d  al or different.
-00009b50: 0a70 6572 6d69 7373 696f 6e73 2e20 2048  .permissions.  H
-00009b60: 6f77 6576 6572 2c20 6e6f 2061 6464 6974  owever, no addit
-00009b70: 696f 6e61 6c20 6f62 6c69 6761 7469 6f6e  ional obligation
-00009b80: 7320 6172 6520 696d 706f 7365 6420 6f6e  s are imposed on
-00009b90: 2061 6e79 0d0a 6175 7468 6f72 206f 7220   any..author or 
-00009ba0: 636f 7079 7269 6768 7420 686f 6c64 6572  copyright holder
-00009bb0: 2061 7320 6120 7265 7375 6c74 206f 6620   as a result of 
-00009bc0: 796f 7572 2063 686f 6f73 696e 6720 746f  your choosing to
-00009bd0: 2066 6f6c 6c6f 7720 610d 0a6c 6174 6572   follow a..later
-00009be0: 2076 6572 7369 6f6e 2e0d 0a0d 0a20 2031   version.....  1
-00009bf0: 352e 2044 6973 636c 6169 6d65 7220 6f66  5. Disclaimer of
-00009c00: 2057 6172 7261 6e74 792e 0d0a 0d0a 2020   Warranty.....  
-00009c10: 5448 4552 4520 4953 204e 4f20 5741 5252  THERE IS NO WARR
-00009c20: 414e 5459 2046 4f52 2054 4845 2050 524f  ANTY FOR THE PRO
-00009c30: 4752 414d 2c20 544f 2054 4845 2045 5854  GRAM, TO THE EXT
-00009c40: 454e 5420 5045 524d 4954 5445 4420 4259  ENT PERMITTED BY
-00009c50: 0d0a 4150 504c 4943 4142 4c45 204c 4157  ..APPLICABLE LAW
-00009c60: 2e20 2045 5843 4550 5420 5748 454e 204f  .  EXCEPT WHEN O
-00009c70: 5448 4552 5749 5345 2053 5441 5445 4420  THERWISE STATED 
-00009c80: 494e 2057 5249 5449 4e47 2054 4845 2043  IN WRITING THE C
-00009c90: 4f50 5952 4947 4854 0d0a 484f 4c44 4552  OPYRIGHT..HOLDER
-00009ca0: 5320 414e 442f 4f52 204f 5448 4552 2050  S AND/OR OTHER P
-00009cb0: 4152 5449 4553 2050 524f 5649 4445 2054  ARTIES PROVIDE T
-00009cc0: 4845 2050 524f 4752 414d 2022 4153 2049  HE PROGRAM "AS I
-00009cd0: 5322 2057 4954 484f 5554 2057 4152 5241  S" WITHOUT WARRA
-00009ce0: 4e54 590d 0a4f 4620 414e 5920 4b49 4e44  NTY..OF ANY KIND
-00009cf0: 2c20 4549 5448 4552 2045 5850 5245 5353  , EITHER EXPRESS
-00009d00: 4544 204f 5220 494d 504c 4945 442c 2049  ED OR IMPLIED, I
-00009d10: 4e43 4c55 4449 4e47 2c20 4255 5420 4e4f  NCLUDING, BUT NO
-00009d20: 5420 4c49 4d49 5445 4420 544f 2c0d 0a54  T LIMITED TO,..T
-00009d30: 4845 2049 4d50 4c49 4544 2057 4152 5241  HE IMPLIED WARRA
-00009d40: 4e54 4945 5320 4f46 204d 4552 4348 414e  NTIES OF MERCHAN
-00009d50: 5441 4249 4c49 5459 2041 4e44 2046 4954  TABILITY AND FIT
-00009d60: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-00009d70: 4355 4c41 520d 0a50 5552 504f 5345 2e20  CULAR..PURPOSE. 
-00009d80: 2054 4845 2045 4e54 4952 4520 5249 534b   THE ENTIRE RISK
-00009d90: 2041 5320 544f 2054 4845 2051 5541 4c49   AS TO THE QUALI
-00009da0: 5459 2041 4e44 2050 4552 464f 524d 414e  TY AND PERFORMAN
-00009db0: 4345 204f 4620 5448 4520 5052 4f47 5241  CE OF THE PROGRA
-00009dc0: 4d0d 0a49 5320 5749 5448 2059 4f55 2e20  M..IS WITH YOU. 
-00009dd0: 2053 484f 554c 4420 5448 4520 5052 4f47   SHOULD THE PROG
-00009de0: 5241 4d20 5052 4f56 4520 4445 4645 4354  RAM PROVE DEFECT
-00009df0: 4956 452c 2059 4f55 2041 5353 554d 4520  IVE, YOU ASSUME 
-00009e00: 5448 4520 434f 5354 204f 460d 0a41 4c4c  THE COST OF..ALL
-00009e10: 204e 4543 4553 5341 5259 2053 4552 5649   NECESSARY SERVI
-00009e20: 4349 4e47 2c20 5245 5041 4952 204f 5220  CING, REPAIR OR 
-00009e30: 434f 5252 4543 5449 4f4e 2e0d 0a0d 0a20  CORRECTION..... 
-00009e40: 2031 362e 204c 696d 6974 6174 696f 6e20   16. Limitation 
-00009e50: 6f66 204c 6961 6269 6c69 7479 2e0d 0a0d  of Liability....
-00009e60: 0a20 2049 4e20 4e4f 2045 5645 4e54 2055  .  IN NO EVENT U
-00009e70: 4e4c 4553 5320 5245 5155 4952 4544 2042  NLESS REQUIRED B
-00009e80: 5920 4150 504c 4943 4142 4c45 204c 4157  Y APPLICABLE LAW
-00009e90: 204f 5220 4147 5245 4544 2054 4f20 494e   OR AGREED TO IN
-00009ea0: 2057 5249 5449 4e47 0d0a 5749 4c4c 2041   WRITING..WILL A
-00009eb0: 4e59 2043 4f50 5952 4947 4854 2048 4f4c  NY COPYRIGHT HOL
-00009ec0: 4445 522c 204f 5220 414e 5920 4f54 4845  DER, OR ANY OTHE
-00009ed0: 5220 5041 5254 5920 5748 4f20 4d4f 4449  R PARTY WHO MODI
-00009ee0: 4649 4553 2041 4e44 2f4f 5220 434f 4e56  FIES AND/OR CONV
-00009ef0: 4559 530d 0a54 4845 2050 524f 4752 414d  EYS..THE PROGRAM
-00009f00: 2041 5320 5045 524d 4954 5445 4420 4142   AS PERMITTED AB
-00009f10: 4f56 452c 2042 4520 4c49 4142 4c45 2054  OVE, BE LIABLE T
-00009f20: 4f20 594f 5520 464f 5220 4441 4d41 4745  O YOU FOR DAMAGE
-00009f30: 532c 2049 4e43 4c55 4449 4e47 2041 4e59  S, INCLUDING ANY
-00009f40: 0d0a 4745 4e45 5241 4c2c 2053 5045 4349  ..GENERAL, SPECI
-00009f50: 414c 2c20 494e 4349 4445 4e54 414c 204f  AL, INCIDENTAL O
-00009f60: 5220 434f 4e53 4551 5545 4e54 4941 4c20  R CONSEQUENTIAL 
-00009f70: 4441 4d41 4745 5320 4152 4953 494e 4720  DAMAGES ARISING 
-00009f80: 4f55 5420 4f46 2054 4845 0d0a 5553 4520  OUT OF THE..USE 
-00009f90: 4f52 2049 4e41 4249 4c49 5459 2054 4f20  OR INABILITY TO 
-00009fa0: 5553 4520 5448 4520 5052 4f47 5241 4d20  USE THE PROGRAM 
-00009fb0: 2849 4e43 4c55 4449 4e47 2042 5554 204e  (INCLUDING BUT N
-00009fc0: 4f54 204c 494d 4954 4544 2054 4f20 4c4f  OT LIMITED TO LO
-00009fd0: 5353 204f 460d 0a44 4154 4120 4f52 2044  SS OF..DATA OR D
-00009fe0: 4154 4120 4245 494e 4720 5245 4e44 4552  ATA BEING RENDER
-00009ff0: 4544 2049 4e41 4343 5552 4154 4520 4f52  ED INACCURATE OR
-0000a000: 204c 4f53 5345 5320 5355 5354 4149 4e45   LOSSES SUSTAINE
-0000a010: 4420 4259 2059 4f55 204f 5220 5448 4952  D BY YOU OR THIR
-0000a020: 440d 0a50 4152 5449 4553 204f 5220 4120  D..PARTIES OR A 
-0000a030: 4641 494c 5552 4520 4f46 2054 4845 2050  FAILURE OF THE P
-0000a040: 524f 4752 414d 2054 4f20 4f50 4552 4154  ROGRAM TO OPERAT
-0000a050: 4520 5749 5448 2041 4e59 204f 5448 4552  E WITH ANY OTHER
-0000a060: 2050 524f 4752 414d 5329 2c0d 0a45 5645   PROGRAMS),..EVE
-0000a070: 4e20 4946 2053 5543 4820 484f 4c44 4552  N IF SUCH HOLDER
-0000a080: 204f 5220 4f54 4845 5220 5041 5254 5920   OR OTHER PARTY 
-0000a090: 4841 5320 4245 454e 2041 4456 4953 4544  HAS BEEN ADVISED
-0000a0a0: 204f 4620 5448 4520 504f 5353 4942 494c   OF THE POSSIBIL
-0000a0b0: 4954 5920 4f46 0d0a 5355 4348 2044 414d  ITY OF..SUCH DAM
-0000a0c0: 4147 4553 2e0d 0a0d 0a20 2031 372e 2049  AGES.....  17. I
-0000a0d0: 6e74 6572 7072 6574 6174 696f 6e20 6f66  nterpretation of
-0000a0e0: 2053 6563 7469 6f6e 7320 3135 2061 6e64   Sections 15 and
-0000a0f0: 2031 362e 0d0a 0d0a 2020 4966 2074 6865   16.....  If the
-0000a100: 2064 6973 636c 6169 6d65 7220 6f66 2077   disclaimer of w
-0000a110: 6172 7261 6e74 7920 616e 6420 6c69 6d69  arranty and limi
-0000a120: 7461 7469 6f6e 206f 6620 6c69 6162 696c  tation of liabil
-0000a130: 6974 7920 7072 6f76 6964 6564 0d0a 6162  ity provided..ab
-0000a140: 6f76 6520 6361 6e6e 6f74 2062 6520 6769  ove cannot be gi
-0000a150: 7665 6e20 6c6f 6361 6c20 6c65 6761 6c20  ven local legal 
-0000a160: 6566 6665 6374 2061 6363 6f72 6469 6e67  effect according
-0000a170: 2074 6f20 7468 6569 7220 7465 726d 732c   to their terms,
-0000a180: 0d0a 7265 7669 6577 696e 6720 636f 7572  ..reviewing cour
-0000a190: 7473 2073 6861 6c6c 2061 7070 6c79 206c  ts shall apply l
-0000a1a0: 6f63 616c 206c 6177 2074 6861 7420 6d6f  ocal law that mo
-0000a1b0: 7374 2063 6c6f 7365 6c79 2061 7070 726f  st closely appro
-0000a1c0: 7869 6d61 7465 730d 0a61 6e20 6162 736f  ximates..an abso
-0000a1d0: 6c75 7465 2077 6169 7665 7220 6f66 2061  lute waiver of a
-0000a1e0: 6c6c 2063 6976 696c 206c 6961 6269 6c69  ll civil liabili
-0000a1f0: 7479 2069 6e20 636f 6e6e 6563 7469 6f6e  ty in connection
-0000a200: 2077 6974 6820 7468 650d 0a50 726f 6772   with the..Progr
-0000a210: 616d 2c20 756e 6c65 7373 2061 2077 6172  am, unless a war
-0000a220: 7261 6e74 7920 6f72 2061 7373 756d 7074  ranty or assumpt
-0000a230: 696f 6e20 6f66 206c 6961 6269 6c69 7479  ion of liability
-0000a240: 2061 6363 6f6d 7061 6e69 6573 2061 0d0a   accompanies a..
-0000a250: 636f 7079 206f 6620 7468 6520 5072 6f67  copy of the Prog
-0000a260: 7261 6d20 696e 2072 6574 7572 6e20 666f  ram in return fo
-0000a270: 7220 6120 6665 652e 0d0a 0d0a 2020 2020  r a fee.....    
-0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2045 4e44 204f 4620 5445 524d 5320 414e   END OF TERMS AN
-0000a2a0: 4420 434f 4e44 4954 494f 4e53 0d0a 0d0a  D CONDITIONS....
-0000a2b0: 2020 2020 2020 2020 2020 2020 486f 7720              How 
-0000a2c0: 746f 2041 7070 6c79 2054 6865 7365 2054  to Apply These T
-0000a2d0: 6572 6d73 2074 6f20 596f 7572 204e 6577  erms to Your New
-0000a2e0: 2050 726f 6772 616d 730d 0a0d 0a20 2049   Programs....  I
-0000a2f0: 6620 796f 7520 6465 7665 6c6f 7020 6120  f you develop a 
-0000a300: 6e65 7720 7072 6f67 7261 6d2c 2061 6e64  new program, and
-0000a310: 2079 6f75 2077 616e 7420 6974 2074 6f20   you want it to 
-0000a320: 6265 206f 6620 7468 6520 6772 6561 7465  be of the greate
-0000a330: 7374 0d0a 706f 7373 6962 6c65 2075 7365  st..possible use
-0000a340: 2074 6f20 7468 6520 7075 626c 6963 2c20   to the public, 
-0000a350: 7468 6520 6265 7374 2077 6179 2074 6f20  the best way to 
-0000a360: 6163 6869 6576 6520 7468 6973 2069 7320  achieve this is 
-0000a370: 746f 206d 616b 6520 6974 0d0a 6672 6565  to make it..free
-0000a380: 2073 6f66 7477 6172 6520 7768 6963 6820   software which 
-0000a390: 6576 6572 796f 6e65 2063 616e 2072 6564  everyone can red
-0000a3a0: 6973 7472 6962 7574 6520 616e 6420 6368  istribute and ch
-0000a3b0: 616e 6765 2075 6e64 6572 2074 6865 7365  ange under these
-0000a3c0: 2074 6572 6d73 2e0d 0a0d 0a20 2054 6f20   terms.....  To 
-0000a3d0: 646f 2073 6f2c 2061 7474 6163 6820 7468  do so, attach th
-0000a3e0: 6520 666f 6c6c 6f77 696e 6720 6e6f 7469  e following noti
-0000a3f0: 6365 7320 746f 2074 6865 2070 726f 6772  ces to the progr
-0000a400: 616d 2e20 2049 7420 6973 2073 6166 6573  am.  It is safes
-0000a410: 740d 0a74 6f20 6174 7461 6368 2074 6865  t..to attach the
-0000a420: 6d20 746f 2074 6865 2073 7461 7274 206f  m to the start o
-0000a430: 6620 6561 6368 2073 6f75 7263 6520 6669  f each source fi
-0000a440: 6c65 2074 6f20 6d6f 7374 2065 6666 6563  le to most effec
-0000a450: 7469 7665 6c79 0d0a 7374 6174 6520 7468  tively..state th
-0000a460: 6520 6578 636c 7573 696f 6e20 6f66 2077  e exclusion of w
-0000a470: 6172 7261 6e74 793b 2061 6e64 2065 6163  arranty; and eac
-0000a480: 6820 6669 6c65 2073 686f 756c 6420 6861  h file should ha
-0000a490: 7665 2061 7420 6c65 6173 740d 0a74 6865  ve at least..the
-0000a4a0: 2022 636f 7079 7269 6768 7422 206c 696e   "copyright" lin
-0000a4b0: 6520 616e 6420 6120 706f 696e 7465 7220  e and a pointer 
-0000a4c0: 746f 2077 6865 7265 2074 6865 2066 756c  to where the ful
-0000a4d0: 6c20 6e6f 7469 6365 2069 7320 666f 756e  l notice is foun
-0000a4e0: 642e 0d0a 0d0a 2020 2020 3c6f 6e65 206c  d.....    <one l
-0000a4f0: 696e 6520 746f 2067 6976 6520 7468 6520  ine to give the 
-0000a500: 7072 6f67 7261 6d27 7320 6e61 6d65 2061  program's name a
-0000a510: 6e64 2061 2062 7269 6566 2069 6465 6120  nd a brief idea 
-0000a520: 6f66 2077 6861 7420 6974 2064 6f65 732e  of what it does.
-0000a530: 3e0d 0a20 2020 2043 6f70 7972 6967 6874  >..    Copyright
-0000a540: 2028 4329 203c 7965 6172 3e20 203c 6e61   (C) <year>  <na
-0000a550: 6d65 206f 6620 6175 7468 6f72 3e0d 0a0d  me of author>...
-0000a560: 0a20 2020 2054 6869 7320 7072 6f67 7261  .    This progra
-0000a570: 6d20 6973 2066 7265 6520 736f 6674 7761  m is free softwa
-0000a580: 7265 3a20 796f 7520 6361 6e20 7265 6469  re: you can redi
-0000a590: 7374 7269 6275 7465 2069 7420 616e 642f  stribute it and/
-0000a5a0: 6f72 206d 6f64 6966 790d 0a20 2020 2069  or modify..    i
-0000a5b0: 7420 756e 6465 7220 7468 6520 7465 726d  t under the term
-0000a5c0: 7320 6f66 2074 6865 2047 4e55 2047 656e  s of the GNU Gen
-0000a5d0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
-0000a5e0: 6e73 6520 6173 2070 7562 6c69 7368 6564  nse as published
-0000a5f0: 2062 790d 0a20 2020 2074 6865 2046 7265   by..    the Fre
-0000a600: 6520 536f 6674 7761 7265 2046 6f75 6e64  e Software Found
-0000a610: 6174 696f 6e2c 2065 6974 6865 7220 7665  ation, either ve
-0000a620: 7273 696f 6e20 3320 6f66 2074 6865 204c  rsion 3 of the L
-0000a630: 6963 656e 7365 2c20 6f72 0d0a 2020 2020  icense, or..    
-0000a640: 2861 7420 796f 7572 206f 7074 696f 6e29  (at your option)
-0000a650: 2061 6e79 206c 6174 6572 2076 6572 7369   any later versi
-0000a660: 6f6e 2e0d 0a0d 0a20 2020 2054 6869 7320  on.....    This 
-0000a670: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
-0000a680: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
-0000a690: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
-0000a6a0: 6265 2075 7365 6675 6c2c 0d0a 2020 2020  be useful,..    
-0000a6b0: 6275 7420 5749 5448 4f55 5420 414e 5920  but WITHOUT ANY 
-0000a6c0: 5741 5252 414e 5459 3b20 7769 7468 6f75  WARRANTY; withou
-0000a6d0: 7420 6576 656e 2074 6865 2069 6d70 6c69  t even the impli
-0000a6e0: 6564 2077 6172 7261 6e74 7920 6f66 0d0a  ed warranty of..
-0000a6f0: 2020 2020 4d45 5243 4841 4e54 4142 494c      MERCHANTABIL
-0000a700: 4954 5920 6f72 2046 4954 4e45 5353 2046  ITY or FITNESS F
-0000a710: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
-0000a720: 5055 5250 4f53 452e 2020 5365 6520 7468  PURPOSE.  See th
-0000a730: 650d 0a20 2020 2047 4e55 2047 656e 6572  e..    GNU Gener
-0000a740: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-0000a750: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
-0000a760: 6c73 2e0d 0a0d 0a20 2020 2059 6f75 2073  ls.....    You s
-0000a770: 686f 756c 6420 6861 7665 2072 6563 6569  hould have recei
-0000a780: 7665 6420 6120 636f 7079 206f 6620 7468  ved a copy of th
-0000a790: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
-0000a7a0: 626c 6963 204c 6963 656e 7365 0d0a 2020  blic License..  
-0000a7b0: 2020 616c 6f6e 6720 7769 7468 2074 6869    along with thi
-0000a7c0: 7320 7072 6f67 7261 6d2e 2020 4966 206e  s program.  If n
-0000a7d0: 6f74 2c20 7365 6520 3c68 7474 7073 3a2f  ot, see <https:/
-0000a7e0: 2f77 7777 2e67 6e75 2e6f 7267 2f6c 6963  /www.gnu.org/lic
-0000a7f0: 656e 7365 732f 3e2e 0d0a 0d0a 416c 736f  enses/>.....Also
-0000a800: 2061 6464 2069 6e66 6f72 6d61 7469 6f6e   add information
-0000a810: 206f 6e20 686f 7720 746f 2063 6f6e 7461   on how to conta
-0000a820: 6374 2079 6f75 2062 7920 656c 6563 7472  ct you by electr
-0000a830: 6f6e 6963 2061 6e64 2070 6170 6572 206d  onic and paper m
-0000a840: 6169 6c2e 0d0a 0d0a 2020 4966 2074 6865  ail.....  If the
-0000a850: 2070 726f 6772 616d 2064 6f65 7320 7465   program does te
-0000a860: 726d 696e 616c 2069 6e74 6572 6163 7469  rminal interacti
-0000a870: 6f6e 2c20 6d61 6b65 2069 7420 6f75 7470  on, make it outp
-0000a880: 7574 2061 2073 686f 7274 0d0a 6e6f 7469  ut a short..noti
-0000a890: 6365 206c 696b 6520 7468 6973 2077 6865  ce like this whe
-0000a8a0: 6e20 6974 2073 7461 7274 7320 696e 2061  n it starts in a
-0000a8b0: 6e20 696e 7465 7261 6374 6976 6520 6d6f  n interactive mo
-0000a8c0: 6465 3a0d 0a0d 0a20 2020 203c 7072 6f67  de:....    <prog
-0000a8d0: 7261 6d3e 2020 436f 7079 7269 6768 7420  ram>  Copyright 
-0000a8e0: 2843 2920 3c79 6561 723e 2020 3c6e 616d  (C) <year>  <nam
-0000a8f0: 6520 6f66 2061 7574 686f 723e 0d0a 2020  e of author>..  
-0000a900: 2020 5468 6973 2070 726f 6772 616d 2063    This program c
-0000a910: 6f6d 6573 2077 6974 6820 4142 534f 4c55  omes with ABSOLU
-0000a920: 5445 4c59 204e 4f20 5741 5252 414e 5459  TELY NO WARRANTY
-0000a930: 3b20 666f 7220 6465 7461 696c 7320 7479  ; for details ty
-0000a940: 7065 2060 7368 6f77 2077 272e 0d0a 2020  pe `show w'...  
-0000a950: 2020 5468 6973 2069 7320 6672 6565 2073    This is free s
-0000a960: 6f66 7477 6172 652c 2061 6e64 2079 6f75  oftware, and you
-0000a970: 2061 7265 2077 656c 636f 6d65 2074 6f20   are welcome to 
-0000a980: 7265 6469 7374 7269 6275 7465 2069 740d  redistribute it.
-0000a990: 0a20 2020 2075 6e64 6572 2063 6572 7461  .    under certa
-0000a9a0: 696e 2063 6f6e 6469 7469 6f6e 733b 2074  in conditions; t
-0000a9b0: 7970 6520 6073 686f 7720 6327 2066 6f72  ype `show c' for
-0000a9c0: 2064 6574 6169 6c73 2e0d 0a0d 0a54 6865   details.....The
-0000a9d0: 2068 7970 6f74 6865 7469 6361 6c20 636f   hypothetical co
-0000a9e0: 6d6d 616e 6473 2060 7368 6f77 2077 2720  mmands `show w' 
-0000a9f0: 616e 6420 6073 686f 7720 6327 2073 686f  and `show c' sho
-0000aa00: 756c 6420 7368 6f77 2074 6865 2061 7070  uld show the app
-0000aa10: 726f 7072 6961 7465 0d0a 7061 7274 7320  ropriate..parts 
-0000aa20: 6f66 2074 6865 2047 656e 6572 616c 2050  of the General P
-0000aa30: 7562 6c69 6320 4c69 6365 6e73 652e 2020  ublic License.  
-0000aa40: 4f66 2063 6f75 7273 652c 2079 6f75 7220  Of course, your 
-0000aa50: 7072 6f67 7261 6d27 7320 636f 6d6d 616e  program's comman
-0000aa60: 6473 0d0a 6d69 6768 7420 6265 2064 6966  ds..might be dif
-0000aa70: 6665 7265 6e74 3b20 666f 7220 6120 4755  ferent; for a GU
-0000aa80: 4920 696e 7465 7266 6163 652c 2079 6f75  I interface, you
-0000aa90: 2077 6f75 6c64 2075 7365 2061 6e20 2261   would use an "a
-0000aaa0: 626f 7574 2062 6f78 222e 0d0a 0d0a 2020  bout box".....  
-0000aab0: 596f 7520 7368 6f75 6c64 2061 6c73 6f20  You should also 
-0000aac0: 6765 7420 796f 7572 2065 6d70 6c6f 7965  get your employe
-0000aad0: 7220 2869 6620 796f 7520 776f 726b 2061  r (if you work a
-0000aae0: 7320 6120 7072 6f67 7261 6d6d 6572 2920  s a programmer) 
-0000aaf0: 6f72 2073 6368 6f6f 6c2c 0d0a 6966 2061  or school,..if a
-0000ab00: 6e79 2c20 746f 2073 6967 6e20 6120 2263  ny, to sign a "c
-0000ab10: 6f70 7972 6967 6874 2064 6973 636c 6169  opyright disclai
-0000ab20: 6d65 7222 2066 6f72 2074 6865 2070 726f  mer" for the pro
-0000ab30: 6772 616d 2c20 6966 206e 6563 6573 7361  gram, if necessa
-0000ab40: 7279 2e0d 0a46 6f72 206d 6f72 6520 696e  ry...For more in
-0000ab50: 666f 726d 6174 696f 6e20 6f6e 2074 6869  formation on thi
-0000ab60: 732c 2061 6e64 2068 6f77 2074 6f20 6170  s, and how to ap
-0000ab70: 706c 7920 616e 6420 666f 6c6c 6f77 2074  ply and follow t
-0000ab80: 6865 2047 4e55 2047 504c 2c20 7365 650d  he GNU GPL, see.
-0000ab90: 0a3c 6874 7470 733a 2f2f 7777 772e 676e  .<https://www.gn
-0000aba0: 752e 6f72 672f 6c69 6365 6e73 6573 2f3e  u.org/licenses/>
-0000abb0: 2e0d 0a0d 0a20 2054 6865 2047 4e55 2047  .....  The GNU G
-0000abc0: 656e 6572 616c 2050 7562 6c69 6320 4c69  eneral Public Li
-0000abd0: 6365 6e73 6520 646f 6573 206e 6f74 2070  cense does not p
-0000abe0: 6572 6d69 7420 696e 636f 7270 6f72 6174  ermit incorporat
-0000abf0: 696e 6720 796f 7572 2070 726f 6772 616d  ing your program
-0000ac00: 0d0a 696e 746f 2070 726f 7072 6965 7461  ..into proprieta
-0000ac10: 7279 2070 726f 6772 616d 732e 2020 4966  ry programs.  If
-0000ac20: 2079 6f75 7220 7072 6f67 7261 6d20 6973   your program is
-0000ac30: 2061 2073 7562 726f 7574 696e 6520 6c69   a subroutine li
-0000ac40: 6272 6172 792c 2079 6f75 0d0a 6d61 7920  brary, you..may 
-0000ac50: 636f 6e73 6964 6572 2069 7420 6d6f 7265  consider it more
-0000ac60: 2075 7365 6675 6c20 746f 2070 6572 6d69   useful to permi
-0000ac70: 7420 6c69 6e6b 696e 6720 7072 6f70 7269  t linking propri
-0000ac80: 6574 6172 7920 6170 706c 6963 6174 696f  etary applicatio
-0000ac90: 6e73 2077 6974 680d 0a74 6865 206c 6962  ns with..the lib
-0000aca0: 7261 7279 2e20 2049 6620 7468 6973 2069  rary.  If this i
-0000acb0: 7320 7768 6174 2079 6f75 2077 616e 7420  s what you want 
-0000acc0: 746f 2064 6f2c 2075 7365 2074 6865 2047  to do, use the G
-0000acd0: 4e55 204c 6573 7365 7220 4765 6e65 7261  NU Lesser Genera
-0000ace0: 6c0d 0a50 7562 6c69 6320 4c69 6365 6e73  l..Public Licens
-0000acf0: 6520 696e 7374 6561 6420 6f66 2074 6869  e instead of thi
-0000ad00: 7320 4c69 6365 6e73 652e 2020 4275 7420  s License.  But 
-0000ad10: 6669 7273 742c 2070 6c65 6173 6520 7265  first, please re
-0000ad20: 6164 0d0a 3c68 7474 7073 3a2f 2f77 7777  ad..<https://www
-0000ad30: 2e67 6e75 2e6f 7267 2f6c 6963 656e 7365  .gnu.org/license
-0000ad40: 732f 7768 792d 6e6f 742d 6c67 706c 2e68  s/why-not-lgpl.h
-0000ad50: 746d 6c3e 2e0d 0a                        tml>...
+00000380: 204c 4943 454e 5345 2e6d 640d 0a0d 0a3c   LICENSE.md....<
+00000390: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
+000003a0: 223e 6f73 6d5f 6561 7379 5f61 7069 3c2f  ">osm_easy_api</
+000003b0: 6831 3e0d 0a3c 7020 616c 6967 6e3d 2263  h1>..<p align="c
+000003c0: 656e 7465 7222 3e0d 0a20 203c 696d 6720  enter">..  <img 
+000003d0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+000003e0: 6875 622e 636f 6d2f 646f 6365 6e74 5954  hub.com/docentYT
+000003f0: 2f61 7574 6f6d 6174 6564 2d70 7974 686f  /automated-pytho
+00000400: 6e2d 7465 7374 732d 7465 7374 696e 672d  n-tests-testing-
+00000410: 7265 706f 2f61 6374 696f 6e73 2f77 6f72  repo/actions/wor
+00000420: 6b66 6c6f 7773 2f74 6573 7473 2e79 616d  kflows/tests.yam
+00000430: 6c2f 6261 6467 652e 7376 6722 202f 3e0d  l/badge.svg" />.
+00000440: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
+00000450: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000460: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
+00000470: 6f63 656e 7459 542f 6f73 6d5f 6561 7379  ocentYT/osm_easy
+00000480: 5f61 7069 2f33 3838 3961 6536 3236 6265  _api/3889ae626be
+00000490: 3335 3138 3332 3533 3438 3536 3436 6237  35183253485646b7
+000004a0: 6265 3965 3233 3561 3266 6332 372f 636f  be9e235a2fc27/co
+000004b0: 7665 7261 6765 2d62 6164 6765 2e73 7667  verage-badge.svg
+000004c0: 2220 2f3e 0d0a 2020 3c61 2068 7265 663d  " />..  <a href=
+000004d0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
+000004e0: 672f 7072 6f6a 6563 742f 6f73 6d2d 6561  g/project/osm-ea
+000004f0: 7379 2d61 7069 2f22 3e0d 0a20 2020 203c  sy-api/">..    <
+00000500: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000510: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000520: 7079 7069 2f76 2f6f 736d 5f65 6173 795f  pypi/v/osm_easy_
+00000530: 6170 6922 202f 3e0d 0a20 203c 2f61 3e0d  api" />..  </a>.
+00000540: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000550: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000560: 6a65 6374 2f6f 736d 2d65 6173 792d 6170  ject/osm-easy-ap
+00000570: 692f 223e 0d0a 2020 2020 3c69 6d67 2073  i/">..    <img s
+00000580: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000590: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+000005a0: 646d 2f6f 736d 5f65 6173 795f 6170 6922  dm/osm_easy_api"
+000005b0: 2061 6c74 3d22 7079 7069 2064 6f77 6e6c   alt="pypi downl
+000005c0: 6f61 6473 223e 0d0a 2020 3c2f 613e 0d0a  oads">..  </a>..
+000005d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000005e0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000005f0: 6563 742f 6f73 6d2d 6561 7379 2d61 7069  ect/osm-easy-api
+00000600: 2f22 3e0d 0a20 2020 203c 696d 6720 616c  /">..    <img al
+00000610: 743d 2270 7974 686f 6e20 7665 7273 696f  t="python versio
+00000620: 6e73 2220 7372 633d 2268 7474 7073 3a2f  ns" src="https:/
+00000630: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000640: 7079 7069 2f70 7976 6572 7369 6f6e 732f  pypi/pyversions/
+00000650: 6f73 6d5f 6561 7379 5f61 7069 2220 7461  osm_easy_api" ta
+00000660: 7267 6574 3d22 5f62 6c61 6e6b 2220 2f3e  rget="_blank" />
+00000670: 0d0a 2020 3c2f 613e 0d0a 3c2f 703e 0d0a  ..  </a>..</p>..
+00000680: 0d0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000690: 6572 223e 3c61 2068 7265 663d 2268 7474  er"><a href="htt
+000006a0: 7073 3a2f 2f77 7777 2e6f 7065 6e73 7472  ps://www.openstr
+000006b0: 6565 746d 6170 2e6f 7267 2f75 7365 722f  eetmap.org/user/
+000006c0: 6b77 6961 7465 6b5f 3132 3329 223e 4d65  kwiatek_123)">Me
+000006d0: 206f 6e20 4f70 656e 5374 7265 6574 4d61   on OpenStreetMa
+000006e0: 703c 2f61 3e3c 2f70 3e0d 0a0d 0a50 7974  p</a></p>....Pyt
+000006f0: 686f 6e20 7061 636b 6167 6520 666f 7220  hon package for 
+00000700: 7061 7273 696e 6720 6f73 6d20 6469 6666  parsing osm diff
+00000710: 7320 616e 6420 636f 6d6d 756e 6963 6174  s and communicat
+00000720: 696e 6720 7769 7468 2074 6865 204f 7065  ing with the Ope
+00000730: 6e53 7472 6565 744d 6170 2061 7069 2e20  nStreetMap api. 
+00000740: 5365 6520 4150 492e 7478 7420 666f 7220  See API.txt for 
+00000750: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
+00000760: 6420 656e 6470 6f69 6e74 732e 0d0a 0d0a  d endpoints.....
+00000770: 2323 2057 6861 7427 7320 7468 6520 706f  ## What's the po
+00000780: 696e 7420 6f66 2074 6869 7320 7061 636b  int of this pack
+00000790: 6167 653f 0d0a 0d0a 5468 6973 2070 6163  age?....This pac
+000007a0: 6b61 6765 2077 6173 2063 7265 6174 6564  kage was created
+000007b0: 2074 6f20 7072 6f76 6964 6520 616e 2065   to provide an e
+000007c0: 6173 7920 7761 7920 746f 2063 7265 6174  asy way to creat
+000007d0: 6520 6175 746f 6d61 7465 6420 7363 7269  e automated scri
+000007e0: 7074 7320 616e 6420 7072 6f67 7261 6d73  pts and programs
+000007f0: 2074 6861 7420 7573 6520 6469 6666 2061   that use diff a
+00000800: 6e64 2f6f 7220 6f73 6d20 6170 692e 2054  nd/or osm api. T
+00000810: 6865 206d 6169 6e20 6164 7661 6e74 6167  he main advantag
+00000820: 6520 6973 2074 6865 2063 6c61 7373 6573  e is the classes
+00000830: 2028 6461 7461 5f63 6c61 7373 6573 2920   (data_classes) 
+00000840: 7468 6174 2070 726f 7669 6465 2064 6174  that provide dat
+00000850: 6120 6f66 2065 6c65 6d65 6e74 7320 286e  a of elements (n
+00000860: 6f64 652c 2077 6179 2c20 7265 6c61 7469  ode, way, relati
+00000870: 6f6e 2c20 4f73 6d43 6861 6e67 652c 2065  on, OsmChange, e
+00000880: 7463 2e29 2069 6e20 6120 7265 6164 6162  tc.) in a readab
+00000890: 6c65 2077 6179 2061 6e64 2074 6865 2070  le way and the p
+000008a0: 6f73 7369 6269 6c69 7479 2074 6f20 7573  ossibility to us
+000008b0: 6520 7468 656d 2069 6e20 6469 6666 2061  e them in diff a
+000008c0: 6e64 2061 7069 2077 6974 686f 7574 2077  nd api without w
+000008d0: 6f72 7279 696e 6720 6162 6f75 7420 6d69  orrying about mi
+000008e0: 7373 696e 6720 6461 7461 206f 7220 6469  ssing data or di
+000008f0: 6374 696f 6e61 7269 6573 2e20 596f 7520  ctionaries. You 
+00000900: 6361 6e20 6561 7369 6c79 2066 696e 6420  can easily find 
+00000910: 6e6f 6465 7320 696e 2064 6966 662c 2061  nodes in diff, a
+00000920: 6464 2061 2074 6167 2074 6f20 7468 656d  dd a tag to them
+00000930: 2061 6e64 2073 656e 6420 7468 6520 636f   and send the co
+00000940: 7272 6563 7465 6420 7665 7273 696f 6e20  rrected version 
+00000950: 746f 206f 736d 2e0d 0a0d 0a23 2320 5768  to osm.....## Wh
+00000960: 6174 206e 6578 743f 0d0a 5468 6520 706c  at next?..The pl
+00000970: 616e 2069 7320 746f 206f 7074 696d 6973  an is to optimis
+00000980: 6520 616e 6420 696d 7072 6f76 6520 7468  e and improve th
+00000990: 6520 636f 6465 2c20 6164 6420 7375 7070  e code, add supp
+000009a0: 6f72 7420 666f 7220 6770 7820 7472 6163  ort for gpx trac
+000009b0: 6573 2c20 7273 7320 7375 7070 6f72 7420  es, rss support 
+000009c0: 616e 6420 6f76 6572 7061 7373 2061 7069  and overpass api
+000009d0: 2e0d 0a0d 0a23 2049 6e73 7461 6c6c 6174  .....# Installat
+000009e0: 696f 6e0d 0a0d 0a57 6f72 6b73 206f 6e20  ion....Works on 
+000009f0: 7079 7468 6f6e 203e 3d20 332e 3130 2e20  python >= 3.10. 
+00000a00: 2844 7565 2074 6f20 6e65 7720 7479 7065  (Due to new type
+00000a10: 6869 6e74 7320 7374 616e 6461 7264 290d  hints standard).
+00000a20: 0a0d 0a49 6e73 7461 6c6c 2060 6f73 6d5f  ...Install `osm_
+00000a30: 6561 7379 5f61 7069 6020 6672 6f6d 205b  easy_api` from [
+00000a40: 5079 5069 5d28 6874 7470 733a 2f2f 7079  PyPi](https://py
+00000a50: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6f  pi.org/project/o
+00000a60: 736d 2d65 6173 792d 6170 692f 293a 0d0a  sm-easy-api/):..
+00000a70: 6060 600d 0a70 6970 2069 6e73 7461 6c6c  ```..pip install
+00000a80: 206f 736d 5f65 6173 795f 6170 690d 0a60   osm_easy_api..`
+00000a90: 6060 200d 0a0d 0a23 2044 6f63 756d 656e  `` ....# Documen
+00000aa0: 7461 7469 6f6e 0d0a 0d0a 596f 7520 6361  tation....You ca
+00000ab0: 6e20 7669 6577 2064 6f63 756d 656e 7461  n view documenta
+00000ac0: 7469 6f6e 206f 6e20 5b67 6974 6875 622d  tion on [github-
+00000ad0: 7061 6765 735d 2868 7474 7073 3a2f 2f64  pages](https://d
+00000ae0: 6f63 656e 7479 742e 6769 7468 7562 2e69  ocentyt.github.i
+00000af0: 6f2f 6f73 6d5f 6561 7379 5f61 7069 2f6f  o/osm_easy_api/o
+00000b00: 736d 5f65 6173 795f 6170 692e 6874 6d6c  sm_easy_api.html
+00000b10: 292e 0d0a 0d0a 446f 6375 6d65 6e74 6174  ).....Documentat
+00000b20: 696f 6e20 6973 2062 7569 6c64 2075 7369  ion is build usi
+00000b30: 6e67 205b 7064 6f63 5d28 6874 7470 733a  ng [pdoc](https:
+00000b40: 2f2f 7064 6f63 2e64 6576 292e 0d0a 546f  //pdoc.dev)...To
+00000b50: 2072 756e 2064 6f63 7320 6f6e 2079 6f75   run docs on you
+00000b60: 7220 6d61 6368 696e 6520 7573 6520 7072  r machine use pr
+00000b70: 6566 6572 7265 6420 636f 6d6d 616e 643a  eferred command:
+00000b80: 2060 7064 6f63 202d 2d64 6f63 666f 726d   `pdoc --docform
+00000b90: 6174 2067 6f6f 676c 6520 2d2d 6e6f 2d73  at google --no-s
+00000ba0: 686f 772d 736f 7572 6365 206f 736d 5f65  how-source osm_e
+00000bb0: 6173 795f 6170 6920 216f 736d 5f65 6173  asy_api !osm_eas
+00000bc0: 795f 6170 692e 7574 696c 7360 2e0d 0a0d  y_api.utils`....
+00000bd0: 0a23 2045 7861 6d70 6c65 730d 0a0d 0a23  .# Examples....#
+00000be0: 2320 4449 4646 0d0a 0d0a 2323 2320 5072  # DIFF....### Pr
+00000bf0: 696e 7420 7472 6565 730d 0a0d 0a60 6060  int trees....```
+00000c00: 7079 0d0a 6672 6f6d 206f 736d 5f65 6173  py..from osm_eas
+00000c10: 795f 6170 6920 696d 706f 7274 204e 6f64  y_api import Nod
+00000c20: 652c 2044 6966 662c 2046 7265 7175 656e  e, Diff, Frequen
+00000c30: 6379 0d0a 0d0a 2320 446f 776e 6c6f 6164  cy....# Download
+00000c40: 2064 6966 6620 6672 6f6d 206c 6173 7420   diff from last 
+00000c50: 686f 7572 2e0d 0a64 203d 2044 6966 6628  hour...d = Diff(
+00000c60: 4672 6571 7565 6e63 792e 484f 5552 290d  Frequency.HOUR).
+00000c70: 0a0d 0a23 2047 6574 204d 6574 6120 6e61  ...# Get Meta na
+00000c80: 6d65 6474 7570 6c65 2066 6f72 2064 6966  medtuple for dif
+00000c90: 6620 6d65 7461 6461 7461 2061 6e64 2067  f metadata and g
+00000ca0: 656e 6572 6174 6f72 2074 6861 7420 7061  enerator that pa
+00000cb0: 7273 6520 6469 6666 2066 696c 652e 0d0a  rse diff file...
+00000cc0: 6d65 7461 2c20 6765 6e20 3d20 642e 6765  meta, gen = d.ge
+00000cd0: 7428 7461 6773 3d22 6e61 7475 7261 6c22  t(tags="natural"
+00000ce0: 290d 0a0d 0a23 2050 7269 6e74 2061 6c6c  )....# Print all
+00000cf0: 2063 7265 6174 6564 2c20 6d6f 6469 6669   created, modifi
+00000d00: 6564 2061 6e64 2064 656c 6574 6564 204e  ed and deleted N
+00000d10: 6f64 6573 2077 6974 6820 6e61 7475 7261  odes with natura
+00000d20: 6c3d 7472 6565 2074 6167 2e0d 0a66 6f72  l=tree tag...for
+00000d30: 2061 6374 696f 6e2c 2065 6c65 6d65 6e74   action, element
+00000d40: 2069 6e20 6765 6e3a 0d0a 2020 2020 6966   in gen:..    if
+00000d50: 2074 7970 6528 656c 656d 656e 7429 203d   type(element) =
+00000d60: 3d20 4e6f 6465 2061 6e64 2065 6c65 6d65  = Node and eleme
+00000d70: 6e74 2e74 6167 732e 6765 7428 226e 6174  nt.tags.get("nat
+00000d80: 7572 616c 2229 203d 3d20 2274 7265 6522  ural") == "tree"
+00000d90: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00000da0: 2861 6374 696f 6e2c 2065 6c65 6d65 6e74  (action, element
+00000db0: 2e69 6429 0d0a 6060 600d 0a0d 0a23 2323  .id)..```....###
+00000dc0: 2050 7269 6e74 2069 6e63 6f72 7265 6374   Print incorrect
+00000dd0: 6c79 2074 6167 6765 6420 7369 6e67 6c65  ly tagged single
+00000de0: 2074 7265 7373 0d0a 0d0a 6060 6070 790d   tress....```py.
+00000df0: 0a66 726f 6d20 6f73 6d5f 6561 7379 5f61  .from osm_easy_a
+00000e00: 7069 2069 6d70 6f72 7420 4469 6666 2c20  pi import Diff, 
+00000e10: 4672 6571 7565 6e63 792c 2041 6374 696f  Frequency, Actio
+00000e20: 6e2c 204e 6f64 650d 0a0d 0a64 203d 2044  n, Node....d = D
+00000e30: 6966 6628 4672 6571 7565 6e63 792e 4441  iff(Frequency.DA
+00000e40: 5929 0d0a 0d0a 6d65 7461 2c20 6765 6e20  Y)....meta, gen 
+00000e50: 3d20 642e 6765 7428 7461 6773 3d22 6e61  = d.get(tags="na
+00000e60: 7475 7261 6c22 290d 0a0d 0a66 6f72 2061  tural")....for a
+00000e70: 6374 696f 6e2c 2065 6c65 6d65 6e74 2069  ction, element i
+00000e80: 6e20 6765 6e3a 0d0a 2020 2020 6966 2074  n gen:..    if t
+00000e90: 7970 6528 656c 656d 656e 7429 203d 3d20  ype(element) == 
+00000ea0: 4e6f 6465 3a0d 0a20 2020 2020 2020 2069  Node:..        i
+00000eb0: 6620 6163 7469 6f6e 203d 3d20 4163 7469  f action == Acti
+00000ec0: 6f6e 2e43 5245 4154 4520 6f72 2061 6374  on.CREATE or act
+00000ed0: 696f 6e20 3d3d 2041 6374 696f 6e2e 4d4f  ion == Action.MO
+00000ee0: 4449 4659 3a0d 0a20 2020 2020 2020 2020  DIFY:..         
+00000ef0: 2020 2069 6620 656c 656d 656e 742e 7461     if element.ta
+00000f00: 6773 2e67 6574 2822 6e61 7475 7261 6c22  gs.get("natural"
+00000f10: 2920 3d3d 2022 776f 6f64 223a 0d0a 2020  ) == "wood":..  
+00000f20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00000f30: 696e 7428 656c 656d 656e 7429 0d0a 6060  int(element)..``
+00000f40: 600d 0a45 7861 6d70 6c65 206f 7574 7075  `..Example outpu
+00000f50: 743a 0d0a 6060 600d 0a4e 6f64 6528 6964  t:..```..Node(id
+00000f60: 203d 2031 3032 3038 3438 3637 3137 2c20   = 10208486717, 
+00000f70: 7669 7369 626c 6520 3d20 4e6f 6e65 2c20  visible = None, 
+00000f80: 7665 7273 696f 6e20 3d20 312c 2063 6861  version = 1, cha
+00000f90: 6e67 6573 6574 5f69 6420 3d20 3132 3932  ngeset_id = 1292
+00000fa0: 3136 3037 352c 2074 696d 6573 7461 6d70  16075, timestamp
+00000fb0: 203d 2032 3032 322d 3131 2d32 3254 3030   = 2022-11-22T00
+00000fc0: 3a31 363a 3434 5a2c 2075 7365 725f 6964  :16:44Z, user_id
+00000fd0: 203d 2031 3734 3731 3732 312c 2074 6167   = 17471721, tag
+00000fe0: 7320 3d20 7b27 6c65 6166 5f74 7970 6527  s = {'leaf_type'
+00000ff0: 3a20 2762 726f 6164 6c65 6176 6564 272c  : 'broadleaved',
+00001000: 2027 6e61 7475 7261 6c27 3a20 2777 6f6f   'natural': 'woo
+00001010: 6427 7d2c 206c 6174 6974 7564 6520 3d20  d'}, latitude = 
+00001020: 3438 2e36 3532 3232 3836 2c20 6c6f 6e67  48.6522286, long
+00001030: 6974 7564 6520 3d20 3132 2e35 3833 3830  itude = 12.58380
+00001040: 392c 2029 0d0a 6060 600d 0a0d 0a23 2320  9, )..```....## 
+00001050: 4150 490d 0a0d 0a23 2323 2041 6464 206d  API....### Add m
+00001060: 6973 7369 6e67 2077 696b 6964 6174 6120  issing wikidata 
+00001070: 7461 670d 0a0d 0a60 6060 7079 0d0a 6672  tag....```py..fr
+00001080: 6f6d 206f 736d 5f65 6173 795f 6170 6920  om osm_easy_api 
+00001090: 696d 706f 7274 2041 7069 2c20 4e6f 6465  import Api, Node
+000010a0: 2c20 5461 6773 0d0a 0d0a 6170 6920 3d20  , Tags....api = 
+000010b0: 4170 6928 2268 7474 7073 3a2f 2f6d 6173  Api("https://mas
+000010c0: 7465 722e 6170 6973 2e64 6576 2e6f 7065  ter.apis.dev.ope
+000010d0: 6e73 7472 6565 746d 6170 2e6f 7267 222c  nstreetmap.org",
+000010e0: 204c 4f47 494e 2c20 5041 5353 574f 5244   LOGIN, PASSWORD
+000010f0: 290d 0a0d 0a6e 6f64 6520 3d20 6170 692e  )....node = api.
+00001100: 656c 656d 656e 7473 2e67 6574 284e 6f64  elements.get(Nod
+00001110: 652c 2034 3239 3634 3630 3333 3629 2023  e, 4296460336) #
+00001120: 2057 6520 6172 6520 6765 7474 696e 6720   We are getting 
+00001130: 4e6f 6465 2077 6974 6820 6964 2034 3239  Node with id 429
+00001140: 3634 3630 3333 3620 7768 6572 6520 7765  6460336 where we
+00001150: 2077 616e 7420 746f 2061 6464 2061 206e   want to add a n
+00001160: 6577 2074 6167 2074 6f0d 0a6e 6f64 652e  ew tag to..node.
+00001170: 7461 6773 2e61 6464 2822 7769 6b69 6461  tags.add("wikida
+00001180: 7461 222c 2022 5165 7861 6d70 6c65 2229  ta", "Qexample")
+00001190: 2023 2041 6464 2061 206e 6577 2074 6167   # Add a new tag
+000011a0: 2074 6f20 6e6f 6465 2e0d 0a0d 0a6d 795f   to node.....my_
+000011b0: 6368 616e 6765 7365 7420 3d20 6170 692e  changeset = api.
+000011c0: 6368 616e 6765 7365 742e 6372 6561 7465  changeset.create
+000011d0: 2822 4164 6420 6d69 7373 696e 6720 7769  ("Add missing wi
+000011e0: 6b69 6461 7461 2074 6167 222c 2054 6167  kidata tag", Tag
+000011f0: 7328 7b22 6175 746f 6d61 7469 6322 3a20  s({"automatic": 
+00001200: 2279 6573 227d 2929 2023 2043 7265 6174  "yes"})) # Creat
+00001210: 6520 6e65 7720 6368 616e 6765 7365 7420  e new changeset 
+00001220: 7769 7468 2064 6573 6372 6970 7469 6f6e  with description
+00001230: 2061 6e64 2074 6167 0d0a 6170 692e 656c   and tag..api.el
+00001240: 656d 656e 7473 2e75 7064 6174 6528 6e6f  ements.update(no
+00001250: 6465 2c20 6d79 5f63 6861 6e67 6573 6574  de, my_changeset
+00001260: 2920 2320 5365 6e64 206e 6577 2076 6572  ) # Send new ver
+00001270: 7369 6f6e 206f 6620 6120 6e6f 6465 2074  sion of a node t
+00001280: 6f20 6f73 6d0d 0a61 7069 2e63 6861 6e67  o osm..api.chang
+00001290: 6573 6574 2e63 6c6f 7365 286d 795f 6368  eset.close(my_ch
+000012a0: 616e 6765 7365 7429 2023 2043 6c6f 7365  angeset) # Close
+000012b0: 2063 6861 6e67 6573 6574 2e0d 0a60 6060   changeset...```
+000012c0: 0d0a 0d0a 2320 4e6f 7465 730d 0a0d 0a4e  ....# Notes....N
+000012d0: 6f74 6520 7468 6174 2074 6865 2066 6f6c  ote that the fol
+000012e0: 6c6f 7769 6e67 2063 6f64 6573 2064 6f20  lowing codes do 
+000012f0: 7468 6520 7361 6d65 2074 6869 6e67 0d0a  the same thing..
+00001300: 6060 6070 790d 0a66 726f 6d20 6f73 6d5f  ```py..from osm_
+00001310: 6561 7379 5f61 7069 2069 6d70 6f72 7420  easy_api import 
+00001320: 4469 6666 2c20 4672 6571 7565 6e63 790d  Diff, Frequency.
+00001330: 0a0d 0a64 203d 2044 6966 6628 4672 6571  ...d = Diff(Freq
+00001340: 7565 6e63 792e 4441 5929 0d0a 0d0a 6d65  uency.DAY)....me
+00001350: 7461 2c20 6765 6e20 3d20 642e 6765 7428  ta, gen = d.get(
+00001360: 290d 0a0d 0a66 6f72 2061 6374 696f 6e2c  )....for action,
+00001370: 2065 6c65 6d65 6e74 2069 6e20 6765 6e3a   element in gen:
+00001380: 0d0a 2020 2020 6966 2065 6c65 6d65 6e74  ..    if element
+00001390: 2e74 6167 732e 6765 7428 2273 686f 7022  .tags.get("shop"
+000013a0: 2920 3d3d 2022 636f 6e76 656e 6965 6e63  ) == "convenienc
+000013b0: 6522 3a0d 0a20 2020 2020 2020 2070 7269  e":..        pri
+000013c0: 6e74 2865 6c65 6d65 6e74 290d 0a60 6060  nt(element)..```
+000013d0: 0d0a 6060 6070 790d 0a66 726f 6d20 6f73  ..```py..from os
+000013e0: 6d5f 6561 7379 5f61 7069 2069 6d70 6f72  m_easy_api impor
+000013f0: 7420 4469 6666 2c20 4672 6571 7565 6e63  t Diff, Frequenc
+00001400: 792c 2054 6167 730d 0a0d 0a64 203d 2044  y, Tags....d = D
+00001410: 6966 6628 4672 6571 7565 6e63 792e 4441  iff(Frequency.DA
+00001420: 5929 0d0a 0d0a 6d65 7461 2c20 6765 6e20  Y)....meta, gen 
+00001430: 3d20 642e 6765 7428 7461 6773 3d54 6167  = d.get(tags=Tag
+00001440: 7328 7b22 7368 6f70 223a 2022 636f 6e76  s({"shop": "conv
+00001450: 656e 6965 6e63 6522 7d29 290d 0a0d 0a66  enience"}))....f
+00001460: 6f72 2061 6374 696f 6e2c 2065 6c65 6d65  or action, eleme
+00001470: 6e74 2069 6e20 6765 6e3a 0d0a 2020 2020  nt in gen:..    
+00001480: 2020 2020 7072 696e 7428 656c 656d 656e      print(elemen
+00001490: 7429 0d0a 6060 600d 0a62 7574 2074 6865  t)..```..but the
+000014a0: 2073 6563 6f6e 6420 7365 656d 7320 746f   second seems to
+000014b0: 2062 6520 6661 7374 6572 2e0d 0a0d 0a41   be faster.....A
+000014c0: 6c73 6f20 796f 7520 6361 6e20 7573 6520  lso you can use 
+000014d0: 4f73 6d43 6861 6e67 6520 6f62 6a65 6374  OsmChange object
+000014e0: 2069 6620 796f 7520 646f 6e27 7420 7761   if you don't wa
+000014f0: 6e74 2074 6f20 7573 6520 6765 6e65 7261  nt to use genera
+00001500: 746f 720d 0a60 6060 7079 0d0a 6672 6f6d  tor..```py..from
+00001510: 206f 736d 5f65 6173 795f 6170 6920 696d   osm_easy_api im
+00001520: 706f 7274 2044 6966 662c 2046 7265 7175  port Diff, Frequ
+00001530: 656e 6379 2c20 4163 7469 6f6e 2c20 4e6f  ency, Action, No
+00001540: 6465 0d0a 0d0a 6420 3d20 4469 6666 2846  de....d = Diff(F
+00001550: 7265 7175 656e 6379 2e4d 494e 5554 4529  requency.MINUTE)
+00001560: 0d0a 0d0a 6f73 6d43 6861 6e67 6520 3d20  ....osmChange = 
+00001570: 642e 6765 7428 6765 6e65 7261 746f 723d  d.get(generator=
+00001580: 4661 6c73 6529 0d0a 0d0a 6465 6c65 7465  False)....delete
+00001590: 645f 6e6f 6465 7320 3d20 6f73 6d43 6861  d_nodes = osmCha
+000015a0: 6e67 652e 6765 7428 4e6f 6465 2c20 4163  nge.get(Node, Ac
+000015b0: 7469 6f6e 2e44 454c 4554 4529 0d0a 666f  tion.DELETE)..fo
+000015c0: 7220 6e6f 6465 2069 6e20 6465 6c65 7465  r node in delete
+000015d0: 645f 6e6f 6465 733a 0d0a 2020 2020 7072  d_nodes:..    pr
+000015e0: 696e 7428 6e6f 6465 2e69 6429 0d0a 6060  int(node.id)..``
+000015f0: 600d 0a62 7574 2069 7420 6361 6e20 636f  `..but it can co
+00001600: 6e73 756d 6520 6c61 7267 6520 616d 6f75  nsume large amou
+00001610: 6e74 7320 6f66 2072 616d 2061 6e64 2075  nts of ram and u
+00001620: 7365 206f 6620 7468 6973 206d 6574 686f  se of this metho
+00001630: 6420 6973 206e 6f74 2072 6563 6f6d 6d65  d is not recomme
+00001640: 6e64 6564 2066 6f72 206c 6172 6765 2064  nded for large d
+00001650: 6966 6627 732e 0d0a 0d0a 2320 5465 7374  iff's.....# Test
+00001660: 730d 0a0d 0a59 6f75 2077 696c 6c20 6e65  s....You will ne
+00001670: 6564 2074 6f20 696e 7374 616c 6c20 6074  ed to install `t
+00001680: 6573 742d 7265 7175 6972 656d 656e 7473  est-requirements
+00001690: 2e74 7874 602e 2059 6f75 2063 616e 2075  .txt`. You can u
+000016a0: 7365 2074 6f78 2e0d 0a54 6f20 7275 6e20  se tox...To run 
+000016b0: 7465 7374 7320 6d61 6e75 616c 6c79 2075  tests manually u
+000016c0: 7365 2060 7079 7468 6f6e 202d 6d20 756e  se `python -m un
+000016d0: 6974 7465 7374 2064 6973 636f 7665 7260  ittest discover`
+000016e0: 2e0d 0a23 2043 6861 6e67 656c 6f67 0d0a  ...# Changelog..
+000016f0: 0d0a 416c 6c20 6e6f 7461 626c 6520 6368  ..All notable ch
+00001700: 616e 6765 7320 746f 2074 6869 7320 7072  anges to this pr
+00001710: 6f6a 6563 7420 7769 6c6c 2062 6520 646f  oject will be do
+00001720: 6375 6d65 6e74 6564 2069 6e20 7468 6973  cumented in this
+00001730: 2066 696c 652e 0d0a 0d0a 5468 6520 666f   file.....The fo
+00001740: 726d 6174 2069 7320 6261 7365 6420 6f6e  rmat is based on
+00001750: 205b 4b65 6570 2061 2043 6861 6e67 656c   [Keep a Changel
+00001760: 6f67 5d28 6874 7470 733a 2f2f 6b65 6570  og](https://keep
+00001770: 6163 6861 6e67 656c 6f67 2e63 6f6d 2f65  achangelog.com/e
+00001780: 6e2f 312e 302e 302f 292c 0d0a 616e 6420  n/1.0.0/),..and 
+00001790: 7468 6973 2070 726f 6a65 6374 2061 6468  this project adh
+000017a0: 6572 6573 2074 6f20 5b53 656d 616e 7469  eres to [Semanti
+000017b0: 6320 5665 7273 696f 6e69 6e67 5d28 6874  c Versioning](ht
+000017c0: 7470 733a 2f2f 7365 6d76 6572 2e6f 7267  tps://semver.org
+000017d0: 2f73 7065 632f 7632 2e30 2e30 2e68 746d  /spec/v2.0.0.htm
+000017e0: 6c29 2e0d 0a0d 0a23 2320 5b31 2e30 2e30  l).....## [1.0.0
+000017f0: 5d0d 0a23 2323 2041 6464 6564 0d0a 2d20  ]..### Added..- 
+00001800: 6074 6f5f 786d 6c28 2960 206d 6574 686f  `to_xml()` metho
+00001810: 6420 696e 2060 4f73 6d43 6861 6e67 6560  d in `OsmChange`
+00001820: 2e0d 0a2d 2060 7570 6c6f 6164 2829 6020  ...- `upload()` 
+00001830: 6d65 7468 6f64 2069 6e20 6063 6861 6e67  method in `chang
+00001840: 6573 6574 6020 6065 6e64 706f 696e 7460  eset` `endpoint`
+00001850: 2068 6173 206e 6577 206f 7074 696f 6e61   has new optiona
+00001860: 6c20 6172 6775 6d65 6e74 732e 0d0a 2d20  l arguments...- 
+00001870: 5465 7374 2066 6f72 2060 746f 5f78 6d6c  Test for `to_xml
+00001880: 2829 6020 6d65 7468 6f64 2069 6e20 604f  ()` method in `O
+00001890: 736d 4368 616e 6765 602e 0d0a 2d20 6023  smChange`...- `#
+000018a0: 2070 7261 676d 613a 206e 6f20 636f 7665   pragma: no cove
+000018b0: 7260 2066 6f72 2075 6e65 7870 6563 7465  r` for unexpecte
+000018c0: 6420 6170 6920 6572 726f 7273 2028 5468  d api errors (Th
+000018d0: 6f73 6520 7468 6174 2061 7265 206e 6f74  ose that are not
+000018e0: 2069 6e20 7468 6520 7370 6563 6966 6963   in the specific
+000018f0: 6174 696f 6e20 6f6e 2074 6865 2077 696b  ation on the wik
+00001900: 6929 2e0d 0a0d 0a23 2323 2043 6861 6e67  i).....### Chang
+00001910: 6564 0d0a 2d20 5072 6976 6174 6520 605f  ed..- Private `_
+00001920: 746f 5f78 6d6c 2829 6020 6d65 7468 6f64  to_xml()` method
+00001930: 2069 6e20 604f 736d 4368 616e 6765 6020   in `OsmChange` 
+00001940: 6973 206e 6f77 2073 7461 7469 632e 0d0a  is now static...
+00001950: 0d0a 2323 205b 302e 342e 325d 0d0a 0d0a  ..## [0.4.2]....
+00001960: 2323 2320 4368 616e 6765 640d 0a2d 204f  ### Changed..- O
+00001970: 7264 6572 206f 6620 656c 656d 656e 7473  rder of elements
+00001980: 2069 6e20 786d 6c20 6765 6e65 7261 7465   in xml generate
+00001990: 6420 6279 2060 5761 792e 5f74 6f5f 786d  d by `Way._to_xm
+000019a0: 6c28 2960 2e20 4669 7273 7420 7461 6773  l()`. First tags
+000019b0: 2c20 7468 656e 206e 6f64 6573 2e0d 0a0d  , then nodes....
+000019c0: 0a23 2323 2046 6978 6564 0d0a 2d20 6052  .### Fixed..- `R
+000019d0: 656c 6174 696f 6e2e 5f74 6f5f 786d 6c28  elation._to_xml(
+000019e0: 2960 2077 6173 2072 6574 7572 6e69 6e67  )` was returning
+000019f0: 2061 6e20 786d 6c20 7769 7468 6f75 7420   an xml without 
+00001a00: 6f73 6d20 7461 6773 2e0d 0a2d 2044 656c  osm tags...- Del
+00001a10: 6574 6564 2064 6973 7573 6564 2076 6172  eted disused var
+00001a20: 6961 626c 6520 696e 2060 4e6f 6465 2e5f  iable in `Node._
+00001a30: 746f 5f78 6d6c 2829 602e 0d0a 2d20 4669  to_xml()`...- Fi
+00001a40: 7865 6420 696e 636f 7272 6563 7420 7265  xed incorrect re
+00001a50: 6c61 7469 6f6e 2070 6172 7369 6e67 206f  lation parsing o
+00001a60: 6620 6461 7461 2072 6563 6976 6564 2062  f data recived b
+00001a70: 7920 6066 756c 6c60 2065 6e64 706f 696e  y `full` endpoin
+00001a80: 742e 0d0a 0d0a 2323 205b 302e 342e 315d  t.....## [0.4.1]
+00001a90: 0d0a 2323 2320 4368 616e 6765 640d 0a2d  ..### Changed..-
+00001aa0: 2055 7064 6174 6564 2060 7265 7175 6573   Updated `reques
+00001ab0: 7473 6020 6672 6f6d 2060 322e 3238 2e31  ts` from `2.28.1
+00001ac0: 6020 746f 2060 322e 3331 2e30 602e 0d0a  ` to `2.31.0`...
+00001ad0: 0d0a 2323 205b 302e 342e 305d 0d0a 2323  ..## [0.4.0]..##
+00001ae0: 2320 4164 6465 640d 0a2d 2060 746f 5f64  # Added..- `to_d
+00001af0: 6963 7428 2960 206d 6574 686f 6420 616e  ict()` method an
+00001b00: 6420 6066 726f 6d5f 6469 6374 2829 6020  d `from_dict()` 
+00001b10: 636c 6173 7320 6d65 7468 6f64 2074 6f20  class method to 
+00001b20: 604e 6f74 6560 2e20 200d 0a2d 2060 746f  `Note`.  ..- `to
+00001b30: 5f64 6963 7428 2960 206d 6574 686f 6420  _dict()` method 
+00001b40: 616e 6420 6066 726f 6d5f 6469 6374 2829  and `from_dict()
+00001b50: 6020 636c 6173 7320 6d65 7468 6f64 2074  ` class method t
+00001b60: 6f20 6043 6f6d 6d65 6e74 602e 0d0a 2d20  o `Comment`...- 
+00001b70: 6074 6f5f 6469 6374 2829 6020 6d65 7468  `to_dict()` meth
+00001b80: 6f64 2061 6e64 2060 6672 6f6d 5f64 6963  od and `from_dic
+00001b90: 7428 2960 2063 6c61 7373 206d 6574 686f  t()` class metho
+00001ba0: 6420 746f 2060 5573 6572 602e 0d0a 2d20  d to `User`...- 
+00001bb0: 446f 6375 6d65 6e74 6174 696f 6e20 6162  Documentation ab
+00001bc0: 6f75 7420 604d 6574 6160 2061 6e64 2060  out `Meta` and `
+00001bd0: 4163 7469 6f6e 6020 636c 6173 732e 0d0a  Action` class...
+00001be0: 2d20 4173 7365 7274 2065 7272 6f72 2028  - Assert error (
+00001bf0: 7769 7468 2069 6e66 6f72 6d61 7469 6f6e  with information
+00001c00: 2074 6f20 7265 706f 7274 2069 7420 6f6e   to report it on
+00001c10: 2067 6974 6875 6229 2077 6865 6e20 6170   github) when ap
+00001c20: 6920 7265 7475 726e 7320 616e 2065 7272  i returns an err
+00001c30: 6f72 2063 6f64 6520 6e6f 7420 6465 7363  or code not desc
+00001c40: 7269 6265 6420 6f6e 2074 6865 2077 696b  ribed on the wik
+00001c50: 692e 0d0a 2d20 6074 6f5f 6469 6374 2829  i...- `to_dict()
+00001c60: 6020 6d65 7468 6f64 2061 6e64 2060 6672  ` method and `fr
+00001c70: 6f6d 5f64 6963 7428 2960 2063 6c61 7373  om_dict()` class
+00001c80: 206d 6574 686f 6420 746f 2060 2872 656c   method to `(rel
+00001c90: 6174 696f 6e29 204d 656d 6265 7260 2e0d  ation) Member`..
+00001ca0: 0a0d 0a23 2323 2046 6978 6564 0d0a 2d20  ...### Fixed..- 
+00001cb0: 604e 6f74 6560 2063 616e 206e 6f77 2062  `Note` can now b
+00001cc0: 6520 696d 706f 7274 6564 2066 726f 6d20  e imported from 
+00001cd0: 7061 636b 6167 652e 0d0a 2d20 6043 6f6d  package...- `Com
+00001ce0: 6d65 6e74 6020 6361 6e20 6e6f 7720 6265  ment` can now be
+00001cf0: 2069 6d70 6f72 7465 6420 6672 6f6d 2070   imported from p
+00001d00: 6163 6b61 6765 2e0d 0a2d 2060 5573 6572  ackage...- `User
+00001d10: 6020 6361 6e20 6e6f 7720 6265 2069 6d70  ` can now be imp
+00001d20: 6f72 7465 6420 6672 6f6d 2070 6163 6b61  orted from packa
+00001d30: 6765 2e0d 0a2d 2060 4d65 6d62 6572 6020  ge...- `Member` 
+00001d40: 6361 6e20 6e6f 7720 6265 2069 6d70 6f72  can now be impor
+00001d50: 7465 6420 6672 6f6d 2070 6163 6b61 6765  ted from package
+00001d60: 2e0d 0a2d 2050 646f 6320 636f 6d6d 616e  ...- Pdoc comman
+00001d70: 6420 696e 2060 5245 4144 4d45 2e6d 6460  d in `README.md`
+00001d80: 2e0d 0a2d 2060 5265 6c61 7469 6f6e 2e74  ...- `Relation.t
+00001d90: 6f5f 6469 6374 2829 6020 6d65 7468 6f64  o_dict()` method
+00001da0: 206e 6f77 2072 6563 7572 7369 7665 6c79   now recursively
+00001db0: 2073 6572 6961 6c69 7365 7320 6d65 6d62   serialises memb
+00001dc0: 6572 732e 0d0a 2d20 6057 6179 2e74 6f5f  ers...- `Way.to_
+00001dd0: 6469 6374 2829 6020 6d65 7468 6f64 206e  dict()` method n
+00001de0: 6f77 2072 6563 7572 7369 7665 6c79 2073  ow recursively s
+00001df0: 6572 6961 6c69 7365 7320 6e6f 6465 732e  erialises nodes.
+00001e00: 0d0a 0d0a 2323 2320 4368 616e 6765 640d  ....### Changed.
+00001e10: 0a2d 2043 6861 6e67 6564 2069 6d70 6f72  .- Changed impor
+00001e20: 7473 2069 6e20 6052 656c 6174 696f 6e2e  ts in `Relation.
+00001e30: 7079 6020 746f 2075 7365 2069 6d70 6f72  py` to use impor
+00001e40: 7469 6e67 2074 6872 6f75 6768 2061 206d  ting through a m
+00001e50: 6f64 756c 6520 7261 7468 6572 2074 6861  odule rather tha
+00001e60: 6e20 6469 7265 6374 6c79 2066 726f 6d20  n directly from 
+00001e70: 6120 6669 6c65 2e0d 0a2d 2041 6464 6564  a file...- Added
+00001e80: 2060 7361 6d70 6c65 5f64 6174 6163 6c61   `sample_datacla
+00001e90: 7373 6573 2e70 7960 2066 696c 6520 696e  sses.py` file in
+00001ea0: 2074 6573 7473 2066 6978 7475 7265 7320   tests fixtures 
+00001eb0: 746f 2072 6564 7563 6520 636f 6465 2064  to reduce code d
+00001ec0: 7570 6c69 6361 7469 6f6e 2e0d 0a2d 2043  uplication...- C
+00001ed0: 6861 6e67 6564 2066 756e 6374 696f 6e20  hanged function 
+00001ee0: 6e61 6d65 2061 6e64 2064 656c 6574 6564  name and deleted
+00001ef0: 2075 6e6e 6563 6573 7361 7279 2061 7267   unnecessary arg
+00001f00: 756d 656e 7420 696e 2060 6170 7065 6e64  ument in `append
+00001f10: 5f65 6c65 6d65 6e74 735f 746f 5f6d 6173  _elements_to_mas
+00001f20: 7465 725f 656c 656d 656e 7428 2960 206e  ter_element()` n
+00001f30: 6573 7465 6420 696e 7369 6465 2070 7269  ested inside pri
+00001f40: 7661 7465 206d 6574 686f 6420 605f 746f  vate method `_to
+00001f50: 5f78 6d6c 2829 6020 696e 2060 4f73 6d43  _xml()` in `OsmC
+00001f60: 6861 6e67 6560 2e0d 0a0d 0a23 2320 5b30  hange`.....## [0
+00001f70: 2e33 2e30 5d20 2d20 3230 3233 2d30 332d  .3.0] - 2023-03-
+00001f80: 3134 0d0a 0d0a 2323 2320 4164 6465 640d  14....### Added.
+00001f90: 0a2d 2060 746f 5f64 6963 7428 2960 206d  .- `to_dict()` m
+00001fa0: 6574 686f 6420 616e 6420 6066 726f 6d5f  ethod and `from_
+00001fb0: 6469 6374 2829 6020 636c 6173 7320 6d65  dict()` class me
+00001fc0: 7468 6f64 2074 6f20 4368 616e 6765 7365  thod to Changese
+00001fd0: 742e 205b 2337 5d28 6874 7470 733a 2f2f  t. [#7](https://
+00001fe0: 6769 7468 7562 2e63 6f6d 2f64 6f63 656e  github.com/docen
+00001ff0: 7459 542f 6f73 6d5f 6561 7379 5f61 7069  tYT/osm_easy_api
+00002000: 2f69 7373 7565 732f 3729 0d0a 2d20 4162  /issues/7)..- Ab
+00002010: 696c 6974 7920 746f 2073 6574 2075 7365  ility to set use
+00002020: 725f 6167 656e 7420 696e 2060 4469 6666  r_agent in `Diff
+00002030: 6020 616e 6420 6041 7069 6020 636c 6173  ` and `Api` clas
+00002040: 732e 205b 2335 5d28 6874 7470 733a 2f2f  s. [#5](https://
+00002050: 6769 7468 7562 2e63 6f6d 2f64 6f63 656e  github.com/docen
+00002060: 7459 542f 6f73 6d5f 6561 7379 5f61 7069  tYT/osm_easy_api
+00002070: 2f69 7373 7565 732f 3529 0d0a 2d20 606f  /issues/5)..- `o
+00002080: 736d 5f6f 626a 6563 745f 7072 696d 6974  sm_object_primit
+00002090: 6976 6560 2060 6672 6f6d 5f64 6963 7428  ive` `from_dict(
+000020a0: 2960 2063 6c61 7373 206d 6574 686f 6420  )` class method 
+000020b0: 6e6f 7720 7261 6973 6573 2060 5661 6c75  now raises `Valu
+000020c0: 6545 7272 6f72 6020 6966 2074 6865 2060  eError` if the `
+000020d0: 7479 7065 6020 6b65 7920 6973 206e 6f74  type` key is not
+000020e0: 2066 6f75 6e64 2e0d 0a0d 0a23 2323 2043   found.....### C
+000020f0: 6861 6e67 6564 0d0a 2d20 6043 6861 6e67  hanged..- `Chang
+00002100: 6573 6574 6020 6973 206e 6f77 2065 7870  eset` is now exp
+00002110: 6f72 7465 6420 6672 6f6d 2064 6174 615f  orted from data_
+00002120: 636c 6173 7365 7320 6d6f 6475 6c65 2e0d  classes module..
+00002130: 0a2d 204d 6f72 6520 7465 7374 732e 0d0a  .- More tests...
+00002140: 0d0a 2323 205b 302e 322e 305d 202d 2032  ..## [0.2.0] - 2
+00002150: 3032 332d 3033 2d30 370d 0a0d 0a23 2323  023-03-07....###
+00002160: 2041 6464 6564 0d0a 2d20 6074 6f5f 6469   Added..- `to_di
+00002170: 6374 2829 6020 6d65 7468 6f64 2061 6e64  ct()` method and
+00002180: 2060 6672 6f6d 5f64 6963 7428 2960 2063   `from_dict()` c
+00002190: 6c61 7373 206d 6574 686f 6420 746f 2060  lass method to `
+000021a0: 6f73 6d5f 6f62 6a65 6374 5f70 7269 6d69  osm_object_primi
+000021b0: 7469 7665 602e 2028 416e 206f 626a 6563  tive`. (An objec
+000021c0: 7420 7468 6174 2069 7320 696e 6865 7269  t that is inheri
+000021d0: 7465 6420 6279 2061 2060 4e6f 6465 602c  ted by a `Node`,
+000021e0: 2060 5761 7960 2c20 6052 656c 6174 696f   `Way`, `Relatio
+000021f0: 6e60 292e 205b 2333 5d28 6874 7470 733a  n`). [#3](https:
+00002200: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6f63  //github.com/doc
+00002210: 656e 7459 542f 6f73 6d5f 6561 7379 5f61  entYT/osm_easy_a
+00002220: 7069 2f69 7373 7565 732f 3329 0d0a 2d20  pi/issues/3)..- 
+00002230: 5375 7070 6f72 7420 666f 7220 6869 7374  Support for hist
+00002240: 6f72 6963 616c 2061 6e6f 6e79 6d6f 7573  orical anonymous
+00002250: 2065 6469 7473 2061 6e64 2065 6469 7473   edits and edits
+00002260: 206d 6164 6520 6279 2064 656c 6574 6564   made by deleted
+00002270: 2061 6363 6f75 6e74 732e 205b 2334 5d28   accounts. [#4](
+00002280: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002290: 6f6d 2f64 6f63 656e 7459 542f 6f73 6d5f  om/docentYT/osm_
+000022a0: 6561 7379 5f61 7069 2f69 7373 7565 732f  easy_api/issues/
+000022b0: 3429 0d0a 0d0a 2323 205b 302e 312e 345d  4)....## [0.1.4]
+000022c0: 202d 2032 3032 332d 3033 2d30 350d 0a0d   - 2023-03-05...
+000022d0: 0a23 2323 2046 6978 6564 0d0a 2d20 496d  .### Fixed..- Im
+000022e0: 7072 6f76 656d 656e 7420 6f66 2075 7469  provement of uti
+000022f0: 6c73 2e6a 6f69 6e5f 7572 6c28 2920 6675  ls.join_url() fu
+00002300: 6e63 7469 6f6e 2e0d 0a2d 2053 7065 6c6c  nction...- Spell
+00002310: 696e 6720 6572 726f 7273 2063 6f72 7265  ing errors corre
+00002320: 6374 6564 205b 406d 6174 6b6f 6e69 6563  cted [@matkoniec
+00002330: 7a5d 2868 7474 7073 3a2f 2f67 6974 6875  z](https://githu
+00002340: 622e 636f 6d2f 6d61 746b 6f6e 6965 637a  b.com/matkoniecz
+00002350: 290d 0a0d 0a23 2320 5b30 2e31 2e33 5d20  )....## [0.1.3] 
+00002360: 2d20 3230 3233 2d30 332d 3033 0d0a 0d0a  - 2023-03-03....
+00002370: 2323 2320 4669 7865 640d 0a0d 0a2d 2046  ### Fixed....- F
+00002380: 6978 6564 2074 6865 206e 6f6e 2d73 6574  ixed the non-set
+00002390: 7469 6e67 206f 6620 7468 6520 2276 6973  ting of the "vis
+000023a0: 6962 6c65 2220 6174 7472 6962 7574 652e  ible" attribute.
+000023b0: 0d0a 0d0a 2323 205b 302e 312e 325d 202d  ....## [0.1.2] -
+000023c0: 2032 3032 332d 3033 2d30 330d 0a0d 0a23   2023-03-03....#
+000023d0: 2323 2046 6978 6564 0d0a 0d0a 2d20 4669  ## Fixed....- Fi
+000023e0: 7865 6420 7265 7475 726e 2074 7970 6520  xed return type 
+000023f0: 6f66 2067 656e 6572 6174 6f72 2069 6e20  of generator in 
+00002400: 4469 6666 2e67 6574 2829 206d 6574 686f  Diff.get() metho
+00002410: 642e 0d0a 0d0a 2323 205b 302e 312e 315d  d.....## [0.1.1]
+00002420: 202d 2032 3032 332d 3033 2d30 330d 0a0d   - 2023-03-03...
+00002430: 0a23 2323 2041 6464 6564 0d0a 0d0a 2d20  .### Added....- 
+00002440: 4c69 6365 6e73 650d 0a0d 0a23 2320 5b30  License....## [0
+00002450: 2e31 2e30 5d20 2d20 3230 3233 2d30 332d  .1.0] - 2023-03-
+00002460: 3033 0d0a 0d0a 2323 2320 4164 6465 640d  03....### Added.
+00002470: 0a0d 0a2d 2049 6e69 7469 616c 2069 6d70  ...- Initial imp
+00002480: 6f72 740d 0a20 2020 2020 2020 2020 2020  ort..           
+00002490: 2020 2020 2020 2020 2047 4e55 2047 454e           GNU GEN
+000024a0: 4552 414c 2050 5542 4c49 4320 4c49 4345  ERAL PUBLIC LICE
+000024b0: 4e53 450d 0a20 2020 2020 2020 2020 2020  NSE..           
+000024c0: 2020 2020 2020 2020 2020 2020 5665 7273              Vers
+000024d0: 696f 6e20 332c 2032 3920 4a75 6e65 2032  ion 3, 29 June 2
+000024e0: 3030 370d 0a0d 0a20 436f 7079 7269 6768  007.... Copyrigh
+000024f0: 7420 2843 2920 3230 3037 2046 7265 6520  t (C) 2007 Free 
+00002500: 536f 6674 7761 7265 2046 6f75 6e64 6174  Software Foundat
+00002510: 696f 6e2c 2049 6e63 2e20 3c68 7474 7073  ion, Inc. <https
+00002520: 3a2f 2f66 7366 2e6f 7267 2f3e 0d0a 2045  ://fsf.org/>.. E
+00002530: 7665 7279 6f6e 6520 6973 2070 6572 6d69  veryone is permi
+00002540: 7474 6564 2074 6f20 636f 7079 2061 6e64  tted to copy and
+00002550: 2064 6973 7472 6962 7574 6520 7665 7262   distribute verb
+00002560: 6174 696d 2063 6f70 6965 730d 0a20 6f66  atim copies.. of
+00002570: 2074 6869 7320 6c69 6365 6e73 6520 646f   this license do
+00002580: 6375 6d65 6e74 2c20 6275 7420 6368 616e  cument, but chan
+00002590: 6769 6e67 2069 7420 6973 206e 6f74 2061  ging it is not a
+000025a0: 6c6c 6f77 6564 2e0d 0a0d 0a20 2020 2020  llowed.....     
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 2020 2020 2020 2050 7265 616d 626c 650d         Preamble.
+000025d0: 0a0d 0a20 2054 6865 2047 4e55 2047 656e  ...  The GNU Gen
+000025e0: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+000025f0: 6e73 6520 6973 2061 2066 7265 652c 2063  nse is a free, c
+00002600: 6f70 796c 6566 7420 6c69 6365 6e73 6520  opyleft license 
+00002610: 666f 720d 0a73 6f66 7477 6172 6520 616e  for..software an
+00002620: 6420 6f74 6865 7220 6b69 6e64 7320 6f66  d other kinds of
+00002630: 2077 6f72 6b73 2e0d 0a0d 0a20 2054 6865   works.....  The
+00002640: 206c 6963 656e 7365 7320 666f 7220 6d6f   licenses for mo
+00002650: 7374 2073 6f66 7477 6172 6520 616e 6420  st software and 
+00002660: 6f74 6865 7220 7072 6163 7469 6361 6c20  other practical 
+00002670: 776f 726b 7320 6172 6520 6465 7369 676e  works are design
+00002680: 6564 0d0a 746f 2074 616b 6520 6177 6179  ed..to take away
+00002690: 2079 6f75 7220 6672 6565 646f 6d20 746f   your freedom to
+000026a0: 2073 6861 7265 2061 6e64 2063 6861 6e67   share and chang
+000026b0: 6520 7468 6520 776f 726b 732e 2020 4279  e the works.  By
+000026c0: 2063 6f6e 7472 6173 742c 0d0a 7468 6520   contrast,..the 
+000026d0: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
+000026e0: 6963 204c 6963 656e 7365 2069 7320 696e  ic License is in
+000026f0: 7465 6e64 6564 2074 6f20 6775 6172 616e  tended to guaran
+00002700: 7465 6520 796f 7572 2066 7265 6564 6f6d  tee your freedom
+00002710: 2074 6f0d 0a73 6861 7265 2061 6e64 2063   to..share and c
+00002720: 6861 6e67 6520 616c 6c20 7665 7273 696f  hange all versio
+00002730: 6e73 206f 6620 6120 7072 6f67 7261 6d2d  ns of a program-
+00002740: 2d74 6f20 6d61 6b65 2073 7572 6520 6974  -to make sure it
+00002750: 2072 656d 6169 6e73 2066 7265 650d 0a73   remains free..s
+00002760: 6f66 7477 6172 6520 666f 7220 616c 6c20  oftware for all 
+00002770: 6974 7320 7573 6572 732e 2020 5765 2c20  its users.  We, 
+00002780: 7468 6520 4672 6565 2053 6f66 7477 6172  the Free Softwar
+00002790: 6520 466f 756e 6461 7469 6f6e 2c20 7573  e Foundation, us
+000027a0: 6520 7468 650d 0a47 4e55 2047 656e 6572  e the..GNU Gener
+000027b0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
+000027c0: 6520 666f 7220 6d6f 7374 206f 6620 6f75  e for most of ou
+000027d0: 7220 736f 6674 7761 7265 3b20 6974 2061  r software; it a
+000027e0: 7070 6c69 6573 2061 6c73 6f20 746f 0d0a  pplies also to..
+000027f0: 616e 7920 6f74 6865 7220 776f 726b 2072  any other work r
+00002800: 656c 6561 7365 6420 7468 6973 2077 6179  eleased this way
+00002810: 2062 7920 6974 7320 6175 7468 6f72 732e   by its authors.
+00002820: 2020 596f 7520 6361 6e20 6170 706c 7920    You can apply 
+00002830: 6974 2074 6f0d 0a79 6f75 7220 7072 6f67  it to..your prog
+00002840: 7261 6d73 2c20 746f 6f2e 0d0a 0d0a 2020  rams, too.....  
+00002850: 5768 656e 2077 6520 7370 6561 6b20 6f66  When we speak of
+00002860: 2066 7265 6520 736f 6674 7761 7265 2c20   free software, 
+00002870: 7765 2061 7265 2072 6566 6572 7269 6e67  we are referring
+00002880: 2074 6f20 6672 6565 646f 6d2c 206e 6f74   to freedom, not
+00002890: 0d0a 7072 6963 652e 2020 4f75 7220 4765  ..price.  Our Ge
+000028a0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+000028b0: 656e 7365 7320 6172 6520 6465 7369 676e  enses are design
+000028c0: 6564 2074 6f20 6d61 6b65 2073 7572 6520  ed to make sure 
+000028d0: 7468 6174 2079 6f75 0d0a 6861 7665 2074  that you..have t
+000028e0: 6865 2066 7265 6564 6f6d 2074 6f20 6469  he freedom to di
+000028f0: 7374 7269 6275 7465 2063 6f70 6965 7320  stribute copies 
+00002900: 6f66 2066 7265 6520 736f 6674 7761 7265  of free software
+00002910: 2028 616e 6420 6368 6172 6765 2066 6f72   (and charge for
+00002920: 0d0a 7468 656d 2069 6620 796f 7520 7769  ..them if you wi
+00002930: 7368 292c 2074 6861 7420 796f 7520 7265  sh), that you re
+00002940: 6365 6976 6520 736f 7572 6365 2063 6f64  ceive source cod
+00002950: 6520 6f72 2063 616e 2067 6574 2069 7420  e or can get it 
+00002960: 6966 2079 6f75 0d0a 7761 6e74 2069 742c  if you..want it,
+00002970: 2074 6861 7420 796f 7520 6361 6e20 6368   that you can ch
+00002980: 616e 6765 2074 6865 2073 6f66 7477 6172  ange the softwar
+00002990: 6520 6f72 2075 7365 2070 6965 6365 7320  e or use pieces 
+000029a0: 6f66 2069 7420 696e 206e 6577 0d0a 6672  of it in new..fr
+000029b0: 6565 2070 726f 6772 616d 732c 2061 6e64  ee programs, and
+000029c0: 2074 6861 7420 796f 7520 6b6e 6f77 2079   that you know y
+000029d0: 6f75 2063 616e 2064 6f20 7468 6573 6520  ou can do these 
+000029e0: 7468 696e 6773 2e0d 0a0d 0a20 2054 6f20  things.....  To 
+000029f0: 7072 6f74 6563 7420 796f 7572 2072 6967  protect your rig
+00002a00: 6874 732c 2077 6520 6e65 6564 2074 6f20  hts, we need to 
+00002a10: 7072 6576 656e 7420 6f74 6865 7273 2066  prevent others f
+00002a20: 726f 6d20 6465 6e79 696e 6720 796f 750d  rom denying you.
+00002a30: 0a74 6865 7365 2072 6967 6874 7320 6f72  .these rights or
+00002a40: 2061 736b 696e 6720 796f 7520 746f 2073   asking you to s
+00002a50: 7572 7265 6e64 6572 2074 6865 2072 6967  urrender the rig
+00002a60: 6874 732e 2020 5468 6572 6566 6f72 652c  hts.  Therefore,
+00002a70: 2079 6f75 2068 6176 650d 0a63 6572 7461   you have..certa
+00002a80: 696e 2072 6573 706f 6e73 6962 696c 6974  in responsibilit
+00002a90: 6965 7320 6966 2079 6f75 2064 6973 7472  ies if you distr
+00002aa0: 6962 7574 6520 636f 7069 6573 206f 6620  ibute copies of 
+00002ab0: 7468 6520 736f 6674 7761 7265 2c20 6f72  the software, or
+00002ac0: 2069 660d 0a79 6f75 206d 6f64 6966 7920   if..you modify 
+00002ad0: 6974 3a20 7265 7370 6f6e 7369 6269 6c69  it: responsibili
+00002ae0: 7469 6573 2074 6f20 7265 7370 6563 7420  ties to respect 
+00002af0: 7468 6520 6672 6565 646f 6d20 6f66 206f  the freedom of o
+00002b00: 7468 6572 732e 0d0a 0d0a 2020 466f 7220  thers.....  For 
+00002b10: 6578 616d 706c 652c 2069 6620 796f 7520  example, if you 
+00002b20: 6469 7374 7269 6275 7465 2063 6f70 6965  distribute copie
+00002b30: 7320 6f66 2073 7563 6820 6120 7072 6f67  s of such a prog
+00002b40: 7261 6d2c 2077 6865 7468 6572 0d0a 6772  ram, whether..gr
+00002b50: 6174 6973 206f 7220 666f 7220 6120 6665  atis or for a fe
+00002b60: 652c 2079 6f75 206d 7573 7420 7061 7373  e, you must pass
+00002b70: 206f 6e20 746f 2074 6865 2072 6563 6970   on to the recip
+00002b80: 6965 6e74 7320 7468 6520 7361 6d65 0d0a  ients the same..
+00002b90: 6672 6565 646f 6d73 2074 6861 7420 796f  freedoms that yo
+00002ba0: 7520 7265 6365 6976 6564 2e20 2059 6f75  u received.  You
+00002bb0: 206d 7573 7420 6d61 6b65 2073 7572 6520   must make sure 
+00002bc0: 7468 6174 2074 6865 792c 2074 6f6f 2c20  that they, too, 
+00002bd0: 7265 6365 6976 650d 0a6f 7220 6361 6e20  receive..or can 
+00002be0: 6765 7420 7468 6520 736f 7572 6365 2063  get the source c
+00002bf0: 6f64 652e 2020 416e 6420 796f 7520 6d75  ode.  And you mu
+00002c00: 7374 2073 686f 7720 7468 656d 2074 6865  st show them the
+00002c10: 7365 2074 6572 6d73 2073 6f20 7468 6579  se terms so they
+00002c20: 0d0a 6b6e 6f77 2074 6865 6972 2072 6967  ..know their rig
+00002c30: 6874 732e 0d0a 0d0a 2020 4465 7665 6c6f  hts.....  Develo
+00002c40: 7065 7273 2074 6861 7420 7573 6520 7468  pers that use th
+00002c50: 6520 474e 5520 4750 4c20 7072 6f74 6563  e GNU GPL protec
+00002c60: 7420 796f 7572 2072 6967 6874 7320 7769  t your rights wi
+00002c70: 7468 2074 776f 2073 7465 7073 3a0d 0a28  th two steps:..(
+00002c80: 3129 2061 7373 6572 7420 636f 7079 7269  1) assert copyri
+00002c90: 6768 7420 6f6e 2074 6865 2073 6f66 7477  ght on the softw
+00002ca0: 6172 652c 2061 6e64 2028 3229 206f 6666  are, and (2) off
+00002cb0: 6572 2079 6f75 2074 6869 7320 4c69 6365  er you this Lice
+00002cc0: 6e73 650d 0a67 6976 696e 6720 796f 7520  nse..giving you 
+00002cd0: 6c65 6761 6c20 7065 726d 6973 7369 6f6e  legal permission
+00002ce0: 2074 6f20 636f 7079 2c20 6469 7374 7269   to copy, distri
+00002cf0: 6275 7465 2061 6e64 2f6f 7220 6d6f 6469  bute and/or modi
+00002d00: 6679 2069 742e 0d0a 0d0a 2020 466f 7220  fy it.....  For 
+00002d10: 7468 6520 6465 7665 6c6f 7065 7273 2720  the developers' 
+00002d20: 616e 6420 6175 7468 6f72 7327 2070 726f  and authors' pro
+00002d30: 7465 6374 696f 6e2c 2074 6865 2047 504c  tection, the GPL
+00002d40: 2063 6c65 6172 6c79 2065 7870 6c61 696e   clearly explain
+00002d50: 730d 0a74 6861 7420 7468 6572 6520 6973  s..that there is
+00002d60: 206e 6f20 7761 7272 616e 7479 2066 6f72   no warranty for
+00002d70: 2074 6869 7320 6672 6565 2073 6f66 7477   this free softw
+00002d80: 6172 652e 2020 466f 7220 626f 7468 2075  are.  For both u
+00002d90: 7365 7273 2720 616e 640d 0a61 7574 686f  sers' and..autho
+00002da0: 7273 2720 7361 6b65 2c20 7468 6520 4750  rs' sake, the GP
+00002db0: 4c20 7265 7175 6972 6573 2074 6861 7420  L requires that 
+00002dc0: 6d6f 6469 6669 6564 2076 6572 7369 6f6e  modified version
+00002dd0: 7320 6265 206d 6172 6b65 6420 6173 0d0a  s be marked as..
+00002de0: 6368 616e 6765 642c 2073 6f20 7468 6174  changed, so that
+00002df0: 2074 6865 6972 2070 726f 626c 656d 7320   their problems 
+00002e00: 7769 6c6c 206e 6f74 2062 6520 6174 7472  will not be attr
+00002e10: 6962 7574 6564 2065 7272 6f6e 656f 7573  ibuted erroneous
+00002e20: 6c79 2074 6f0d 0a61 7574 686f 7273 206f  ly to..authors o
+00002e30: 6620 7072 6576 696f 7573 2076 6572 7369  f previous versi
+00002e40: 6f6e 732e 0d0a 0d0a 2020 536f 6d65 2064  ons.....  Some d
+00002e50: 6576 6963 6573 2061 7265 2064 6573 6967  evices are desig
+00002e60: 6e65 6420 746f 2064 656e 7920 7573 6572  ned to deny user
+00002e70: 7320 6163 6365 7373 2074 6f20 696e 7374  s access to inst
+00002e80: 616c 6c20 6f72 2072 756e 0d0a 6d6f 6469  all or run..modi
+00002e90: 6669 6564 2076 6572 7369 6f6e 7320 6f66  fied versions of
+00002ea0: 2074 6865 2073 6f66 7477 6172 6520 696e   the software in
+00002eb0: 7369 6465 2074 6865 6d2c 2061 6c74 686f  side them, altho
+00002ec0: 7567 6820 7468 6520 6d61 6e75 6661 6374  ugh the manufact
+00002ed0: 7572 6572 0d0a 6361 6e20 646f 2073 6f2e  urer..can do so.
+00002ee0: 2020 5468 6973 2069 7320 6675 6e64 616d    This is fundam
+00002ef0: 656e 7461 6c6c 7920 696e 636f 6d70 6174  entally incompat
+00002f00: 6962 6c65 2077 6974 6820 7468 6520 6169  ible with the ai
+00002f10: 6d20 6f66 0d0a 7072 6f74 6563 7469 6e67  m of..protecting
+00002f20: 2075 7365 7273 2720 6672 6565 646f 6d20   users' freedom 
+00002f30: 746f 2063 6861 6e67 6520 7468 6520 736f  to change the so
+00002f40: 6674 7761 7265 2e20 2054 6865 2073 7973  ftware.  The sys
+00002f50: 7465 6d61 7469 630d 0a70 6174 7465 726e  tematic..pattern
+00002f60: 206f 6620 7375 6368 2061 6275 7365 206f   of such abuse o
+00002f70: 6363 7572 7320 696e 2074 6865 2061 7265  ccurs in the are
+00002f80: 6120 6f66 2070 726f 6475 6374 7320 666f  a of products fo
+00002f90: 7220 696e 6469 7669 6475 616c 7320 746f  r individuals to
+00002fa0: 0d0a 7573 652c 2077 6869 6368 2069 7320  ..use, which is 
+00002fb0: 7072 6563 6973 656c 7920 7768 6572 6520  precisely where 
+00002fc0: 6974 2069 7320 6d6f 7374 2075 6e61 6363  it is most unacc
+00002fd0: 6570 7461 626c 652e 2020 5468 6572 6566  eptable.  Theref
+00002fe0: 6f72 652c 2077 650d 0a68 6176 6520 6465  ore, we..have de
+00002ff0: 7369 676e 6564 2074 6869 7320 7665 7273  signed this vers
+00003000: 696f 6e20 6f66 2074 6865 2047 504c 2074  ion of the GPL t
+00003010: 6f20 7072 6f68 6962 6974 2074 6865 2070  o prohibit the p
+00003020: 7261 6374 6963 6520 666f 7220 7468 6f73  ractice for thos
+00003030: 650d 0a70 726f 6475 6374 732e 2020 4966  e..products.  If
+00003040: 2073 7563 6820 7072 6f62 6c65 6d73 2061   such problems a
+00003050: 7269 7365 2073 7562 7374 616e 7469 616c  rise substantial
+00003060: 6c79 2069 6e20 6f74 6865 7220 646f 6d61  ly in other doma
+00003070: 696e 732c 2077 650d 0a73 7461 6e64 2072  ins, we..stand r
+00003080: 6561 6479 2074 6f20 6578 7465 6e64 2074  eady to extend t
+00003090: 6869 7320 7072 6f76 6973 696f 6e20 746f  his provision to
+000030a0: 2074 686f 7365 2064 6f6d 6169 6e73 2069   those domains i
+000030b0: 6e20 6675 7475 7265 2076 6572 7369 6f6e  n future version
+000030c0: 730d 0a6f 6620 7468 6520 4750 4c2c 2061  s..of the GPL, a
+000030d0: 7320 6e65 6564 6564 2074 6f20 7072 6f74  s needed to prot
+000030e0: 6563 7420 7468 6520 6672 6565 646f 6d20  ect the freedom 
+000030f0: 6f66 2075 7365 7273 2e0d 0a0d 0a20 2046  of users.....  F
+00003100: 696e 616c 6c79 2c20 6576 6572 7920 7072  inally, every pr
+00003110: 6f67 7261 6d20 6973 2074 6872 6561 7465  ogram is threate
+00003120: 6e65 6420 636f 6e73 7461 6e74 6c79 2062  ned constantly b
+00003130: 7920 736f 6674 7761 7265 2070 6174 656e  y software paten
+00003140: 7473 2e0d 0a53 7461 7465 7320 7368 6f75  ts...States shou
+00003150: 6c64 206e 6f74 2061 6c6c 6f77 2070 6174  ld not allow pat
+00003160: 656e 7473 2074 6f20 7265 7374 7269 6374  ents to restrict
+00003170: 2064 6576 656c 6f70 6d65 6e74 2061 6e64   development and
+00003180: 2075 7365 206f 660d 0a73 6f66 7477 6172   use of..softwar
+00003190: 6520 6f6e 2067 656e 6572 616c 2d70 7572  e on general-pur
+000031a0: 706f 7365 2063 6f6d 7075 7465 7273 2c20  pose computers, 
+000031b0: 6275 7420 696e 2074 686f 7365 2074 6861  but in those tha
+000031c0: 7420 646f 2c20 7765 2077 6973 6820 746f  t do, we wish to
+000031d0: 0d0a 6176 6f69 6420 7468 6520 7370 6563  ..avoid the spec
+000031e0: 6961 6c20 6461 6e67 6572 2074 6861 7420  ial danger that 
+000031f0: 7061 7465 6e74 7320 6170 706c 6965 6420  patents applied 
+00003200: 746f 2061 2066 7265 6520 7072 6f67 7261  to a free progra
+00003210: 6d20 636f 756c 640d 0a6d 616b 6520 6974  m could..make it
+00003220: 2065 6666 6563 7469 7665 6c79 2070 726f   effectively pro
+00003230: 7072 6965 7461 7279 2e20 2054 6f20 7072  prietary.  To pr
+00003240: 6576 656e 7420 7468 6973 2c20 7468 6520  event this, the 
+00003250: 4750 4c20 6173 7375 7265 7320 7468 6174  GPL assures that
+00003260: 0d0a 7061 7465 6e74 7320 6361 6e6e 6f74  ..patents cannot
+00003270: 2062 6520 7573 6564 2074 6f20 7265 6e64   be used to rend
+00003280: 6572 2074 6865 2070 726f 6772 616d 206e  er the program n
+00003290: 6f6e 2d66 7265 652e 0d0a 0d0a 2020 5468  on-free.....  Th
+000032a0: 6520 7072 6563 6973 6520 7465 726d 7320  e precise terms 
+000032b0: 616e 6420 636f 6e64 6974 696f 6e73 2066  and conditions f
+000032c0: 6f72 2063 6f70 7969 6e67 2c20 6469 7374  or copying, dist
+000032d0: 7269 6275 7469 6f6e 2061 6e64 0d0a 6d6f  ribution and..mo
+000032e0: 6469 6669 6361 7469 6f6e 2066 6f6c 6c6f  dification follo
+000032f0: 772e 0d0a 0d0a 2020 2020 2020 2020 2020  w.....          
+00003300: 2020 2020 2020 2020 2020 2020 2054 4552               TER
+00003310: 4d53 2041 4e44 2043 4f4e 4449 5449 4f4e  MS AND CONDITION
+00003320: 530d 0a0d 0a20 2030 2e20 4465 6669 6e69  S....  0. Defini
+00003330: 7469 6f6e 732e 0d0a 0d0a 2020 2254 6869  tions.....  "Thi
+00003340: 7320 4c69 6365 6e73 6522 2072 6566 6572  s License" refer
+00003350: 7320 746f 2076 6572 7369 6f6e 2033 206f  s to version 3 o
+00003360: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00003370: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00003380: 2e0d 0a0d 0a20 2022 436f 7079 7269 6768  .....  "Copyrigh
+00003390: 7422 2061 6c73 6f20 6d65 616e 7320 636f  t" also means co
+000033a0: 7079 7269 6768 742d 6c69 6b65 206c 6177  pyright-like law
+000033b0: 7320 7468 6174 2061 7070 6c79 2074 6f20  s that apply to 
+000033c0: 6f74 6865 7220 6b69 6e64 7320 6f66 0d0a  other kinds of..
+000033d0: 776f 726b 732c 2073 7563 6820 6173 2073  works, such as s
+000033e0: 656d 6963 6f6e 6475 6374 6f72 206d 6173  emiconductor mas
+000033f0: 6b73 2e0d 0a0d 0a20 2022 5468 6520 5072  ks.....  "The Pr
+00003400: 6f67 7261 6d22 2072 6566 6572 7320 746f  ogram" refers to
+00003410: 2061 6e79 2063 6f70 7972 6967 6874 6162   any copyrightab
+00003420: 6c65 2077 6f72 6b20 6c69 6365 6e73 6564  le work licensed
+00003430: 2075 6e64 6572 2074 6869 730d 0a4c 6963   under this..Lic
+00003440: 656e 7365 2e20 2045 6163 6820 6c69 6365  ense.  Each lice
+00003450: 6e73 6565 2069 7320 6164 6472 6573 7365  nsee is addresse
+00003460: 6420 6173 2022 796f 7522 2e20 2022 4c69  d as "you".  "Li
+00003470: 6365 6e73 6565 7322 2061 6e64 0d0a 2272  censees" and.."r
+00003480: 6563 6970 6965 6e74 7322 206d 6179 2062  ecipients" may b
+00003490: 6520 696e 6469 7669 6475 616c 7320 6f72  e individuals or
+000034a0: 206f 7267 616e 697a 6174 696f 6e73 2e0d   organizations..
+000034b0: 0a0d 0a20 2054 6f20 226d 6f64 6966 7922  ...  To "modify"
+000034c0: 2061 2077 6f72 6b20 6d65 616e 7320 746f   a work means to
+000034d0: 2063 6f70 7920 6672 6f6d 206f 7220 6164   copy from or ad
+000034e0: 6170 7420 616c 6c20 6f72 2070 6172 7420  apt all or part 
+000034f0: 6f66 2074 6865 2077 6f72 6b0d 0a69 6e20  of the work..in 
+00003500: 6120 6661 7368 696f 6e20 7265 7175 6972  a fashion requir
+00003510: 696e 6720 636f 7079 7269 6768 7420 7065  ing copyright pe
+00003520: 726d 6973 7369 6f6e 2c20 6f74 6865 7220  rmission, other 
+00003530: 7468 616e 2074 6865 206d 616b 696e 6720  than the making 
+00003540: 6f66 2061 6e0d 0a65 7861 6374 2063 6f70  of an..exact cop
+00003550: 792e 2020 5468 6520 7265 7375 6c74 696e  y.  The resultin
+00003560: 6720 776f 726b 2069 7320 6361 6c6c 6564  g work is called
+00003570: 2061 2022 6d6f 6469 6669 6564 2076 6572   a "modified ver
+00003580: 7369 6f6e 2220 6f66 2074 6865 0d0a 6561  sion" of the..ea
+00003590: 726c 6965 7220 776f 726b 206f 7220 6120  rlier work or a 
+000035a0: 776f 726b 2022 6261 7365 6420 6f6e 2220  work "based on" 
+000035b0: 7468 6520 6561 726c 6965 7220 776f 726b  the earlier work
+000035c0: 2e0d 0a0d 0a20 2041 2022 636f 7665 7265  .....  A "covere
+000035d0: 6420 776f 726b 2220 6d65 616e 7320 6569  d work" means ei
+000035e0: 7468 6572 2074 6865 2075 6e6d 6f64 6966  ther the unmodif
+000035f0: 6965 6420 5072 6f67 7261 6d20 6f72 2061  ied Program or a
+00003600: 2077 6f72 6b20 6261 7365 640d 0a6f 6e20   work based..on 
+00003610: 7468 6520 5072 6f67 7261 6d2e 0d0a 0d0a  the Program.....
+00003620: 2020 546f 2022 7072 6f70 6167 6174 6522    To "propagate"
+00003630: 2061 2077 6f72 6b20 6d65 616e 7320 746f   a work means to
+00003640: 2064 6f20 616e 7974 6869 6e67 2077 6974   do anything wit
+00003650: 6820 6974 2074 6861 742c 2077 6974 686f  h it that, witho
+00003660: 7574 0d0a 7065 726d 6973 7369 6f6e 2c20  ut..permission, 
+00003670: 776f 756c 6420 6d61 6b65 2079 6f75 2064  would make you d
+00003680: 6972 6563 746c 7920 6f72 2073 6563 6f6e  irectly or secon
+00003690: 6461 7269 6c79 206c 6961 626c 6520 666f  darily liable fo
+000036a0: 720d 0a69 6e66 7269 6e67 656d 656e 7420  r..infringement 
+000036b0: 756e 6465 7220 6170 706c 6963 6162 6c65  under applicable
+000036c0: 2063 6f70 7972 6967 6874 206c 6177 2c20   copyright law, 
+000036d0: 6578 6365 7074 2065 7865 6375 7469 6e67  except executing
+000036e0: 2069 7420 6f6e 2061 0d0a 636f 6d70 7574   it on a..comput
+000036f0: 6572 206f 7220 6d6f 6469 6679 696e 6720  er or modifying 
+00003700: 6120 7072 6976 6174 6520 636f 7079 2e20  a private copy. 
+00003710: 2050 726f 7061 6761 7469 6f6e 2069 6e63   Propagation inc
+00003720: 6c75 6465 7320 636f 7079 696e 672c 0d0a  ludes copying,..
+00003730: 6469 7374 7269 6275 7469 6f6e 2028 7769  distribution (wi
+00003740: 7468 206f 7220 7769 7468 6f75 7420 6d6f  th or without mo
+00003750: 6469 6669 6361 7469 6f6e 292c 206d 616b  dification), mak
+00003760: 696e 6720 6176 6169 6c61 626c 6520 746f  ing available to
+00003770: 2074 6865 0d0a 7075 626c 6963 2c20 616e   the..public, an
+00003780: 6420 696e 2073 6f6d 6520 636f 756e 7472  d in some countr
+00003790: 6965 7320 6f74 6865 7220 6163 7469 7669  ies other activi
+000037a0: 7469 6573 2061 7320 7765 6c6c 2e0d 0a0d  ties as well....
+000037b0: 0a20 2054 6f20 2263 6f6e 7665 7922 2061  .  To "convey" a
+000037c0: 2077 6f72 6b20 6d65 616e 7320 616e 7920   work means any 
+000037d0: 6b69 6e64 206f 6620 7072 6f70 6167 6174  kind of propagat
+000037e0: 696f 6e20 7468 6174 2065 6e61 626c 6573  ion that enables
+000037f0: 206f 7468 6572 0d0a 7061 7274 6965 7320   other..parties 
+00003800: 746f 206d 616b 6520 6f72 2072 6563 6569  to make or recei
+00003810: 7665 2063 6f70 6965 732e 2020 4d65 7265  ve copies.  Mere
+00003820: 2069 6e74 6572 6163 7469 6f6e 2077 6974   interaction wit
+00003830: 6820 6120 7573 6572 2074 6872 6f75 6768  h a user through
+00003840: 0d0a 6120 636f 6d70 7574 6572 206e 6574  ..a computer net
+00003850: 776f 726b 2c20 7769 7468 206e 6f20 7472  work, with no tr
+00003860: 616e 7366 6572 206f 6620 6120 636f 7079  ansfer of a copy
+00003870: 2c20 6973 206e 6f74 2063 6f6e 7665 7969  , is not conveyi
+00003880: 6e67 2e0d 0a0d 0a20 2041 6e20 696e 7465  ng.....  An inte
+00003890: 7261 6374 6976 6520 7573 6572 2069 6e74  ractive user int
+000038a0: 6572 6661 6365 2064 6973 706c 6179 7320  erface displays 
+000038b0: 2241 7070 726f 7072 6961 7465 204c 6567  "Appropriate Leg
+000038c0: 616c 204e 6f74 6963 6573 220d 0a74 6f20  al Notices"..to 
+000038d0: 7468 6520 6578 7465 6e74 2074 6861 7420  the extent that 
+000038e0: 6974 2069 6e63 6c75 6465 7320 6120 636f  it includes a co
+000038f0: 6e76 656e 6965 6e74 2061 6e64 2070 726f  nvenient and pro
+00003900: 6d69 6e65 6e74 6c79 2076 6973 6962 6c65  minently visible
+00003910: 0d0a 6665 6174 7572 6520 7468 6174 2028  ..feature that (
+00003920: 3129 2064 6973 706c 6179 7320 616e 2061  1) displays an a
+00003930: 7070 726f 7072 6961 7465 2063 6f70 7972  ppropriate copyr
+00003940: 6967 6874 206e 6f74 6963 652c 2061 6e64  ight notice, and
+00003950: 2028 3229 0d0a 7465 6c6c 7320 7468 6520   (2)..tells the 
+00003960: 7573 6572 2074 6861 7420 7468 6572 6520  user that there 
+00003970: 6973 206e 6f20 7761 7272 616e 7479 2066  is no warranty f
+00003980: 6f72 2074 6865 2077 6f72 6b20 2865 7863  or the work (exc
+00003990: 6570 7420 746f 2074 6865 0d0a 6578 7465  ept to the..exte
+000039a0: 6e74 2074 6861 7420 7761 7272 616e 7469  nt that warranti
+000039b0: 6573 2061 7265 2070 726f 7669 6465 6429  es are provided)
+000039c0: 2c20 7468 6174 206c 6963 656e 7365 6573  , that licensees
+000039d0: 206d 6179 2063 6f6e 7665 7920 7468 650d   may convey the.
+000039e0: 0a77 6f72 6b20 756e 6465 7220 7468 6973  .work under this
+000039f0: 204c 6963 656e 7365 2c20 616e 6420 686f   License, and ho
+00003a00: 7720 746f 2076 6965 7720 6120 636f 7079  w to view a copy
+00003a10: 206f 6620 7468 6973 204c 6963 656e 7365   of this License
+00003a20: 2e20 2049 660d 0a74 6865 2069 6e74 6572  .  If..the inter
+00003a30: 6661 6365 2070 7265 7365 6e74 7320 6120  face presents a 
+00003a40: 6c69 7374 206f 6620 7573 6572 2063 6f6d  list of user com
+00003a50: 6d61 6e64 7320 6f72 206f 7074 696f 6e73  mands or options
+00003a60: 2c20 7375 6368 2061 7320 610d 0a6d 656e  , such as a..men
+00003a70: 752c 2061 2070 726f 6d69 6e65 6e74 2069  u, a prominent i
+00003a80: 7465 6d20 696e 2074 6865 206c 6973 7420  tem in the list 
+00003a90: 6d65 6574 7320 7468 6973 2063 7269 7465  meets this crite
+00003aa0: 7269 6f6e 2e0d 0a0d 0a20 2031 2e20 536f  rion.....  1. So
+00003ab0: 7572 6365 2043 6f64 652e 0d0a 0d0a 2020  urce Code.....  
+00003ac0: 5468 6520 2273 6f75 7263 6520 636f 6465  The "source code
+00003ad0: 2220 666f 7220 6120 776f 726b 206d 6561  " for a work mea
+00003ae0: 6e73 2074 6865 2070 7265 6665 7272 6564  ns the preferred
+00003af0: 2066 6f72 6d20 6f66 2074 6865 2077 6f72   form of the wor
+00003b00: 6b0d 0a66 6f72 206d 616b 696e 6720 6d6f  k..for making mo
+00003b10: 6469 6669 6361 7469 6f6e 7320 746f 2069  difications to i
+00003b20: 742e 2020 224f 626a 6563 7420 636f 6465  t.  "Object code
+00003b30: 2220 6d65 616e 7320 616e 7920 6e6f 6e2d  " means any non-
+00003b40: 736f 7572 6365 0d0a 666f 726d 206f 6620  source..form of 
+00003b50: 6120 776f 726b 2e0d 0a0d 0a20 2041 2022  a work.....  A "
+00003b60: 5374 616e 6461 7264 2049 6e74 6572 6661  Standard Interfa
+00003b70: 6365 2220 6d65 616e 7320 616e 2069 6e74  ce" means an int
+00003b80: 6572 6661 6365 2074 6861 7420 6569 7468  erface that eith
+00003b90: 6572 2069 7320 616e 206f 6666 6963 6961  er is an officia
+00003ba0: 6c0d 0a73 7461 6e64 6172 6420 6465 6669  l..standard defi
+00003bb0: 6e65 6420 6279 2061 2072 6563 6f67 6e69  ned by a recogni
+00003bc0: 7a65 6420 7374 616e 6461 7264 7320 626f  zed standards bo
+00003bd0: 6479 2c20 6f72 2c20 696e 2074 6865 2063  dy, or, in the c
+00003be0: 6173 6520 6f66 0d0a 696e 7465 7266 6163  ase of..interfac
+00003bf0: 6573 2073 7065 6369 6669 6564 2066 6f72  es specified for
+00003c00: 2061 2070 6172 7469 6375 6c61 7220 7072   a particular pr
+00003c10: 6f67 7261 6d6d 696e 6720 6c61 6e67 7561  ogramming langua
+00003c20: 6765 2c20 6f6e 6520 7468 6174 0d0a 6973  ge, one that..is
+00003c30: 2077 6964 656c 7920 7573 6564 2061 6d6f   widely used amo
+00003c40: 6e67 2064 6576 656c 6f70 6572 7320 776f  ng developers wo
+00003c50: 726b 696e 6720 696e 2074 6861 7420 6c61  rking in that la
+00003c60: 6e67 7561 6765 2e0d 0a0d 0a20 2054 6865  nguage.....  The
+00003c70: 2022 5379 7374 656d 204c 6962 7261 7269   "System Librari
+00003c80: 6573 2220 6f66 2061 6e20 6578 6563 7574  es" of an execut
+00003c90: 6162 6c65 2077 6f72 6b20 696e 636c 7564  able work includ
+00003ca0: 6520 616e 7974 6869 6e67 2c20 6f74 6865  e anything, othe
+00003cb0: 720d 0a74 6861 6e20 7468 6520 776f 726b  r..than the work
+00003cc0: 2061 7320 6120 7768 6f6c 652c 2074 6861   as a whole, tha
+00003cd0: 7420 2861 2920 6973 2069 6e63 6c75 6465  t (a) is include
+00003ce0: 6420 696e 2074 6865 206e 6f72 6d61 6c20  d in the normal 
+00003cf0: 666f 726d 206f 660d 0a70 6163 6b61 6769  form of..packagi
+00003d00: 6e67 2061 204d 616a 6f72 2043 6f6d 706f  ng a Major Compo
+00003d10: 6e65 6e74 2c20 6275 7420 7768 6963 6820  nent, but which 
+00003d20: 6973 206e 6f74 2070 6172 7420 6f66 2074  is not part of t
+00003d30: 6861 7420 4d61 6a6f 720d 0a43 6f6d 706f  hat Major..Compo
+00003d40: 6e65 6e74 2c20 616e 6420 2862 2920 7365  nent, and (b) se
+00003d50: 7276 6573 206f 6e6c 7920 746f 2065 6e61  rves only to ena
+00003d60: 626c 6520 7573 6520 6f66 2074 6865 2077  ble use of the w
+00003d70: 6f72 6b20 7769 7468 2074 6861 740d 0a4d  ork with that..M
+00003d80: 616a 6f72 2043 6f6d 706f 6e65 6e74 2c20  ajor Component, 
+00003d90: 6f72 2074 6f20 696d 706c 656d 656e 7420  or to implement 
+00003da0: 6120 5374 616e 6461 7264 2049 6e74 6572  a Standard Inter
+00003db0: 6661 6365 2066 6f72 2077 6869 6368 2061  face for which a
+00003dc0: 6e0d 0a69 6d70 6c65 6d65 6e74 6174 696f  n..implementatio
+00003dd0: 6e20 6973 2061 7661 696c 6162 6c65 2074  n is available t
+00003de0: 6f20 7468 6520 7075 626c 6963 2069 6e20  o the public in 
+00003df0: 736f 7572 6365 2063 6f64 6520 666f 726d  source code form
+00003e00: 2e20 2041 0d0a 224d 616a 6f72 2043 6f6d  .  A.."Major Com
+00003e10: 706f 6e65 6e74 222c 2069 6e20 7468 6973  ponent", in this
+00003e20: 2063 6f6e 7465 7874 2c20 6d65 616e 7320   context, means 
+00003e30: 6120 6d61 6a6f 7220 6573 7365 6e74 6961  a major essentia
+00003e40: 6c20 636f 6d70 6f6e 656e 740d 0a28 6b65  l component..(ke
+00003e50: 726e 656c 2c20 7769 6e64 6f77 2073 7973  rnel, window sys
+00003e60: 7465 6d2c 2061 6e64 2073 6f20 6f6e 2920  tem, and so on) 
+00003e70: 6f66 2074 6865 2073 7065 6369 6669 6320  of the specific 
+00003e80: 6f70 6572 6174 696e 6720 7379 7374 656d  operating system
+00003e90: 0d0a 2869 6620 616e 7929 206f 6e20 7768  ..(if any) on wh
+00003ea0: 6963 6820 7468 6520 6578 6563 7574 6162  ich the executab
+00003eb0: 6c65 2077 6f72 6b20 7275 6e73 2c20 6f72  le work runs, or
+00003ec0: 2061 2063 6f6d 7069 6c65 7220 7573 6564   a compiler used
+00003ed0: 2074 6f0d 0a70 726f 6475 6365 2074 6865   to..produce the
+00003ee0: 2077 6f72 6b2c 206f 7220 616e 206f 626a   work, or an obj
+00003ef0: 6563 7420 636f 6465 2069 6e74 6572 7072  ect code interpr
+00003f00: 6574 6572 2075 7365 6420 746f 2072 756e  eter used to run
+00003f10: 2069 742e 0d0a 0d0a 2020 5468 6520 2243   it.....  The "C
+00003f20: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
+00003f30: 7263 6522 2066 6f72 2061 2077 6f72 6b20  rce" for a work 
+00003f40: 696e 206f 626a 6563 7420 636f 6465 2066  in object code f
+00003f50: 6f72 6d20 6d65 616e 7320 616c 6c0d 0a74  orm means all..t
+00003f60: 6865 2073 6f75 7263 6520 636f 6465 206e  he source code n
+00003f70: 6565 6465 6420 746f 2067 656e 6572 6174  eeded to generat
+00003f80: 652c 2069 6e73 7461 6c6c 2c20 616e 6420  e, install, and 
+00003f90: 2866 6f72 2061 6e20 6578 6563 7574 6162  (for an executab
+00003fa0: 6c65 0d0a 776f 726b 2920 7275 6e20 7468  le..work) run th
+00003fb0: 6520 6f62 6a65 6374 2063 6f64 6520 616e  e object code an
+00003fc0: 6420 746f 206d 6f64 6966 7920 7468 6520  d to modify the 
+00003fd0: 776f 726b 2c20 696e 636c 7564 696e 6720  work, including 
+00003fe0: 7363 7269 7074 7320 746f 0d0a 636f 6e74  scripts to..cont
+00003ff0: 726f 6c20 7468 6f73 6520 6163 7469 7669  rol those activi
+00004000: 7469 6573 2e20 2048 6f77 6576 6572 2c20  ties.  However, 
+00004010: 6974 2064 6f65 7320 6e6f 7420 696e 636c  it does not incl
+00004020: 7564 6520 7468 6520 776f 726b 2773 0d0a  ude the work's..
+00004030: 5379 7374 656d 204c 6962 7261 7269 6573  System Libraries
+00004040: 2c20 6f72 2067 656e 6572 616c 2d70 7572  , or general-pur
+00004050: 706f 7365 2074 6f6f 6c73 206f 7220 6765  pose tools or ge
+00004060: 6e65 7261 6c6c 7920 6176 6169 6c61 626c  nerally availabl
+00004070: 6520 6672 6565 0d0a 7072 6f67 7261 6d73  e free..programs
+00004080: 2077 6869 6368 2061 7265 2075 7365 6420   which are used 
+00004090: 756e 6d6f 6469 6669 6564 2069 6e20 7065  unmodified in pe
+000040a0: 7266 6f72 6d69 6e67 2074 686f 7365 2061  rforming those a
+000040b0: 6374 6976 6974 6965 7320 6275 740d 0a77  ctivities but..w
+000040c0: 6869 6368 2061 7265 206e 6f74 2070 6172  hich are not par
+000040d0: 7420 6f66 2074 6865 2077 6f72 6b2e 2020  t of the work.  
+000040e0: 466f 7220 6578 616d 706c 652c 2043 6f72  For example, Cor
+000040f0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
+00004100: 650d 0a69 6e63 6c75 6465 7320 696e 7465  e..includes inte
+00004110: 7266 6163 6520 6465 6669 6e69 7469 6f6e  rface definition
+00004120: 2066 696c 6573 2061 7373 6f63 6961 7465   files associate
+00004130: 6420 7769 7468 2073 6f75 7263 6520 6669  d with source fi
+00004140: 6c65 7320 666f 720d 0a74 6865 2077 6f72  les for..the wor
+00004150: 6b2c 2061 6e64 2074 6865 2073 6f75 7263  k, and the sourc
+00004160: 6520 636f 6465 2066 6f72 2073 6861 7265  e code for share
+00004170: 6420 6c69 6272 6172 6965 7320 616e 6420  d libraries and 
+00004180: 6479 6e61 6d69 6361 6c6c 790d 0a6c 696e  dynamically..lin
+00004190: 6b65 6420 7375 6270 726f 6772 616d 7320  ked subprograms 
+000041a0: 7468 6174 2074 6865 2077 6f72 6b20 6973  that the work is
+000041b0: 2073 7065 6369 6669 6361 6c6c 7920 6465   specifically de
+000041c0: 7369 676e 6564 2074 6f20 7265 7175 6972  signed to requir
+000041d0: 652c 0d0a 7375 6368 2061 7320 6279 2069  e,..such as by i
+000041e0: 6e74 696d 6174 6520 6461 7461 2063 6f6d  ntimate data com
+000041f0: 6d75 6e69 6361 7469 6f6e 206f 7220 636f  munication or co
+00004200: 6e74 726f 6c20 666c 6f77 2062 6574 7765  ntrol flow betwe
+00004210: 656e 2074 686f 7365 0d0a 7375 6270 726f  en those..subpro
+00004220: 6772 616d 7320 616e 6420 6f74 6865 7220  grams and other 
+00004230: 7061 7274 7320 6f66 2074 6865 2077 6f72  parts of the wor
+00004240: 6b2e 0d0a 0d0a 2020 5468 6520 436f 7272  k.....  The Corr
+00004250: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
+00004260: 206e 6565 6420 6e6f 7420 696e 636c 7564   need not includ
+00004270: 6520 616e 7974 6869 6e67 2074 6861 7420  e anything that 
+00004280: 7573 6572 730d 0a63 616e 2072 6567 656e  users..can regen
+00004290: 6572 6174 6520 6175 746f 6d61 7469 6361  erate automatica
+000042a0: 6c6c 7920 6672 6f6d 206f 7468 6572 2070  lly from other p
+000042b0: 6172 7473 206f 6620 7468 6520 436f 7272  arts of the Corr
+000042c0: 6573 706f 6e64 696e 670d 0a53 6f75 7263  esponding..Sourc
+000042d0: 652e 0d0a 0d0a 2020 5468 6520 436f 7272  e.....  The Corr
+000042e0: 6573 706f 6e64 696e 6720 536f 7572 6365  esponding Source
+000042f0: 2066 6f72 2061 2077 6f72 6b20 696e 2073   for a work in s
+00004300: 6f75 7263 6520 636f 6465 2066 6f72 6d20  ource code form 
+00004310: 6973 2074 6861 740d 0a73 616d 6520 776f  is that..same wo
+00004320: 726b 2e0d 0a0d 0a20 2032 2e20 4261 7369  rk.....  2. Basi
+00004330: 6320 5065 726d 6973 7369 6f6e 732e 0d0a  c Permissions...
+00004340: 0d0a 2020 416c 6c20 7269 6768 7473 2067  ..  All rights g
+00004350: 7261 6e74 6564 2075 6e64 6572 2074 6869  ranted under thi
+00004360: 7320 4c69 6365 6e73 6520 6172 6520 6772  s License are gr
+00004370: 616e 7465 6420 666f 7220 7468 6520 7465  anted for the te
+00004380: 726d 206f 660d 0a63 6f70 7972 6967 6874  rm of..copyright
+00004390: 206f 6e20 7468 6520 5072 6f67 7261 6d2c   on the Program,
+000043a0: 2061 6e64 2061 7265 2069 7272 6576 6f63   and are irrevoc
+000043b0: 6162 6c65 2070 726f 7669 6465 6420 7468  able provided th
+000043c0: 6520 7374 6174 6564 0d0a 636f 6e64 6974  e stated..condit
+000043d0: 696f 6e73 2061 7265 206d 6574 2e20 2054  ions are met.  T
+000043e0: 6869 7320 4c69 6365 6e73 6520 6578 706c  his License expl
+000043f0: 6963 6974 6c79 2061 6666 6972 6d73 2079  icitly affirms y
+00004400: 6f75 7220 756e 6c69 6d69 7465 640d 0a70  our unlimited..p
+00004410: 6572 6d69 7373 696f 6e20 746f 2072 756e  ermission to run
+00004420: 2074 6865 2075 6e6d 6f64 6966 6965 6420   the unmodified 
+00004430: 5072 6f67 7261 6d2e 2020 5468 6520 6f75  Program.  The ou
+00004440: 7470 7574 2066 726f 6d20 7275 6e6e 696e  tput from runnin
+00004450: 6720 610d 0a63 6f76 6572 6564 2077 6f72  g a..covered wor
+00004460: 6b20 6973 2063 6f76 6572 6564 2062 7920  k is covered by 
+00004470: 7468 6973 204c 6963 656e 7365 206f 6e6c  this License onl
+00004480: 7920 6966 2074 6865 206f 7574 7075 742c  y if the output,
+00004490: 2067 6976 656e 2069 7473 0d0a 636f 6e74   given its..cont
+000044a0: 656e 742c 2063 6f6e 7374 6974 7574 6573  ent, constitutes
+000044b0: 2061 2063 6f76 6572 6564 2077 6f72 6b2e   a covered work.
+000044c0: 2020 5468 6973 204c 6963 656e 7365 2061    This License a
+000044d0: 636b 6e6f 776c 6564 6765 7320 796f 7572  cknowledges your
+000044e0: 0d0a 7269 6768 7473 206f 6620 6661 6972  ..rights of fair
+000044f0: 2075 7365 206f 7220 6f74 6865 7220 6571   use or other eq
+00004500: 7569 7661 6c65 6e74 2c20 6173 2070 726f  uivalent, as pro
+00004510: 7669 6465 6420 6279 2063 6f70 7972 6967  vided by copyrig
+00004520: 6874 206c 6177 2e0d 0a0d 0a20 2059 6f75  ht law.....  You
+00004530: 206d 6179 206d 616b 652c 2072 756e 2061   may make, run a
+00004540: 6e64 2070 726f 7061 6761 7465 2063 6f76  nd propagate cov
+00004550: 6572 6564 2077 6f72 6b73 2074 6861 7420  ered works that 
+00004560: 796f 7520 646f 206e 6f74 0d0a 636f 6e76  you do not..conv
+00004570: 6579 2c20 7769 7468 6f75 7420 636f 6e64  ey, without cond
+00004580: 6974 696f 6e73 2073 6f20 6c6f 6e67 2061  itions so long a
+00004590: 7320 796f 7572 206c 6963 656e 7365 206f  s your license o
+000045a0: 7468 6572 7769 7365 2072 656d 6169 6e73  therwise remains
+000045b0: 0d0a 696e 2066 6f72 6365 2e20 2059 6f75  ..in force.  You
+000045c0: 206d 6179 2063 6f6e 7665 7920 636f 7665   may convey cove
+000045d0: 7265 6420 776f 726b 7320 746f 206f 7468  red works to oth
+000045e0: 6572 7320 666f 7220 7468 6520 736f 6c65  ers for the sole
+000045f0: 2070 7572 706f 7365 0d0a 6f66 2068 6176   purpose..of hav
+00004600: 696e 6720 7468 656d 206d 616b 6520 6d6f  ing them make mo
+00004610: 6469 6669 6361 7469 6f6e 7320 6578 636c  difications excl
+00004620: 7573 6976 656c 7920 666f 7220 796f 752c  usively for you,
+00004630: 206f 7220 7072 6f76 6964 6520 796f 750d   or provide you.
+00004640: 0a77 6974 6820 6661 6369 6c69 7469 6573  .with facilities
+00004650: 2066 6f72 2072 756e 6e69 6e67 2074 686f   for running tho
+00004660: 7365 2077 6f72 6b73 2c20 7072 6f76 6964  se works, provid
+00004670: 6564 2074 6861 7420 796f 7520 636f 6d70  ed that you comp
+00004680: 6c79 2077 6974 680d 0a74 6865 2074 6572  ly with..the ter
+00004690: 6d73 206f 6620 7468 6973 204c 6963 656e  ms of this Licen
+000046a0: 7365 2069 6e20 636f 6e76 6579 696e 6720  se in conveying 
+000046b0: 616c 6c20 6d61 7465 7269 616c 2066 6f72  all material for
+000046c0: 2077 6869 6368 2079 6f75 2064 6f0d 0a6e   which you do..n
+000046d0: 6f74 2063 6f6e 7472 6f6c 2063 6f70 7972  ot control copyr
+000046e0: 6967 6874 2e20 2054 686f 7365 2074 6875  ight.  Those thu
+000046f0: 7320 6d61 6b69 6e67 206f 7220 7275 6e6e  s making or runn
+00004700: 696e 6720 7468 6520 636f 7665 7265 6420  ing the covered 
+00004710: 776f 726b 730d 0a66 6f72 2079 6f75 206d  works..for you m
+00004720: 7573 7420 646f 2073 6f20 6578 636c 7573  ust do so exclus
+00004730: 6976 656c 7920 6f6e 2079 6f75 7220 6265  ively on your be
+00004740: 6861 6c66 2c20 756e 6465 7220 796f 7572  half, under your
+00004750: 2064 6972 6563 7469 6f6e 0d0a 616e 6420   direction..and 
+00004760: 636f 6e74 726f 6c2c 206f 6e20 7465 726d  control, on term
+00004770: 7320 7468 6174 2070 726f 6869 6269 7420  s that prohibit 
+00004780: 7468 656d 2066 726f 6d20 6d61 6b69 6e67  them from making
+00004790: 2061 6e79 2063 6f70 6965 7320 6f66 0d0a   any copies of..
+000047a0: 796f 7572 2063 6f70 7972 6967 6874 6564  your copyrighted
+000047b0: 206d 6174 6572 6961 6c20 6f75 7473 6964   material outsid
+000047c0: 6520 7468 6569 7220 7265 6c61 7469 6f6e  e their relation
+000047d0: 7368 6970 2077 6974 6820 796f 752e 0d0a  ship with you...
+000047e0: 0d0a 2020 436f 6e76 6579 696e 6720 756e  ..  Conveying un
+000047f0: 6465 7220 616e 7920 6f74 6865 7220 6369  der any other ci
+00004800: 7263 756d 7374 616e 6365 7320 6973 2070  rcumstances is p
+00004810: 6572 6d69 7474 6564 2073 6f6c 656c 7920  ermitted solely 
+00004820: 756e 6465 720d 0a74 6865 2063 6f6e 6469  under..the condi
+00004830: 7469 6f6e 7320 7374 6174 6564 2062 656c  tions stated bel
+00004840: 6f77 2e20 2053 7562 6c69 6365 6e73 696e  ow.  Sublicensin
+00004850: 6720 6973 206e 6f74 2061 6c6c 6f77 6564  g is not allowed
+00004860: 3b20 7365 6374 696f 6e20 3130 0d0a 6d61  ; section 10..ma
+00004870: 6b65 7320 6974 2075 6e6e 6563 6573 7361  kes it unnecessa
+00004880: 7279 2e0d 0a0d 0a20 2033 2e20 5072 6f74  ry.....  3. Prot
+00004890: 6563 7469 6e67 2055 7365 7273 2720 4c65  ecting Users' Le
+000048a0: 6761 6c20 5269 6768 7473 2046 726f 6d20  gal Rights From 
+000048b0: 416e 7469 2d43 6972 6375 6d76 656e 7469  Anti-Circumventi
+000048c0: 6f6e 204c 6177 2e0d 0a0d 0a20 204e 6f20  on Law.....  No 
+000048d0: 636f 7665 7265 6420 776f 726b 2073 6861  covered work sha
+000048e0: 6c6c 2062 6520 6465 656d 6564 2070 6172  ll be deemed par
+000048f0: 7420 6f66 2061 6e20 6566 6665 6374 6976  t of an effectiv
+00004900: 6520 7465 6368 6e6f 6c6f 6769 6361 6c0d  e technological.
+00004910: 0a6d 6561 7375 7265 2075 6e64 6572 2061  .measure under a
+00004920: 6e79 2061 7070 6c69 6361 626c 6520 6c61  ny applicable la
+00004930: 7720 6675 6c66 696c 6c69 6e67 206f 626c  w fulfilling obl
+00004940: 6967 6174 696f 6e73 2075 6e64 6572 2061  igations under a
+00004950: 7274 6963 6c65 0d0a 3131 206f 6620 7468  rticle..11 of th
+00004960: 6520 5749 504f 2063 6f70 7972 6967 6874  e WIPO copyright
+00004970: 2074 7265 6174 7920 6164 6f70 7465 6420   treaty adopted 
+00004980: 6f6e 2032 3020 4465 6365 6d62 6572 2031  on 20 December 1
+00004990: 3939 362c 206f 720d 0a73 696d 696c 6172  996, or..similar
+000049a0: 206c 6177 7320 7072 6f68 6962 6974 696e   laws prohibitin
+000049b0: 6720 6f72 2072 6573 7472 6963 7469 6e67  g or restricting
+000049c0: 2063 6972 6375 6d76 656e 7469 6f6e 206f   circumvention o
+000049d0: 6620 7375 6368 0d0a 6d65 6173 7572 6573  f such..measures
+000049e0: 2e0d 0a0d 0a20 2057 6865 6e20 796f 7520  .....  When you 
+000049f0: 636f 6e76 6579 2061 2063 6f76 6572 6564  convey a covered
+00004a00: 2077 6f72 6b2c 2079 6f75 2077 6169 7665   work, you waive
+00004a10: 2061 6e79 206c 6567 616c 2070 6f77 6572   any legal power
+00004a20: 2074 6f20 666f 7262 6964 0d0a 6369 7263   to forbid..circ
+00004a30: 756d 7665 6e74 696f 6e20 6f66 2074 6563  umvention of tec
+00004a40: 686e 6f6c 6f67 6963 616c 206d 6561 7375  hnological measu
+00004a50: 7265 7320 746f 2074 6865 2065 7874 656e  res to the exten
+00004a60: 7420 7375 6368 2063 6972 6375 6d76 656e  t such circumven
+00004a70: 7469 6f6e 0d0a 6973 2065 6666 6563 7465  tion..is effecte
+00004a80: 6420 6279 2065 7865 7263 6973 696e 6720  d by exercising 
+00004a90: 7269 6768 7473 2075 6e64 6572 2074 6869  rights under thi
+00004aa0: 7320 4c69 6365 6e73 6520 7769 7468 2072  s License with r
+00004ab0: 6573 7065 6374 2074 6f0d 0a74 6865 2063  espect to..the c
+00004ac0: 6f76 6572 6564 2077 6f72 6b2c 2061 6e64  overed work, and
+00004ad0: 2079 6f75 2064 6973 636c 6169 6d20 616e   you disclaim an
+00004ae0: 7920 696e 7465 6e74 696f 6e20 746f 206c  y intention to l
+00004af0: 696d 6974 206f 7065 7261 7469 6f6e 206f  imit operation o
+00004b00: 720d 0a6d 6f64 6966 6963 6174 696f 6e20  r..modification 
+00004b10: 6f66 2074 6865 2077 6f72 6b20 6173 2061  of the work as a
+00004b20: 206d 6561 6e73 206f 6620 656e 666f 7263   means of enforc
+00004b30: 696e 672c 2061 6761 696e 7374 2074 6865  ing, against the
+00004b40: 2077 6f72 6b27 730d 0a75 7365 7273 2c20   work's..users, 
+00004b50: 796f 7572 206f 7220 7468 6972 6420 7061  your or third pa
+00004b60: 7274 6965 7327 206c 6567 616c 2072 6967  rties' legal rig
+00004b70: 6874 7320 746f 2066 6f72 6269 6420 6369  hts to forbid ci
+00004b80: 7263 756d 7665 6e74 696f 6e20 6f66 0d0a  rcumvention of..
+00004b90: 7465 6368 6e6f 6c6f 6769 6361 6c20 6d65  technological me
+00004ba0: 6173 7572 6573 2e0d 0a0d 0a20 2034 2e20  asures.....  4. 
+00004bb0: 436f 6e76 6579 696e 6720 5665 7262 6174  Conveying Verbat
+00004bc0: 696d 2043 6f70 6965 732e 0d0a 0d0a 2020  im Copies.....  
+00004bd0: 596f 7520 6d61 7920 636f 6e76 6579 2076  You may convey v
+00004be0: 6572 6261 7469 6d20 636f 7069 6573 206f  erbatim copies o
+00004bf0: 6620 7468 6520 5072 6f67 7261 6d27 7320  f the Program's 
+00004c00: 736f 7572 6365 2063 6f64 6520 6173 2079  source code as y
+00004c10: 6f75 0d0a 7265 6365 6976 6520 6974 2c20  ou..receive it, 
+00004c20: 696e 2061 6e79 206d 6564 6975 6d2c 2070  in any medium, p
+00004c30: 726f 7669 6465 6420 7468 6174 2079 6f75  rovided that you
+00004c40: 2063 6f6e 7370 6963 756f 7573 6c79 2061   conspicuously a
+00004c50: 6e64 0d0a 6170 7072 6f70 7269 6174 656c  nd..appropriatel
+00004c60: 7920 7075 626c 6973 6820 6f6e 2065 6163  y publish on eac
+00004c70: 6820 636f 7079 2061 6e20 6170 7072 6f70  h copy an approp
+00004c80: 7269 6174 6520 636f 7079 7269 6768 7420  riate copyright 
+00004c90: 6e6f 7469 6365 3b0d 0a6b 6565 7020 696e  notice;..keep in
+00004ca0: 7461 6374 2061 6c6c 206e 6f74 6963 6573  tact all notices
+00004cb0: 2073 7461 7469 6e67 2074 6861 7420 7468   stating that th
+00004cc0: 6973 204c 6963 656e 7365 2061 6e64 2061  is License and a
+00004cd0: 6e79 0d0a 6e6f 6e2d 7065 726d 6973 7369  ny..non-permissi
+00004ce0: 7665 2074 6572 6d73 2061 6464 6564 2069  ve terms added i
+00004cf0: 6e20 6163 636f 7264 2077 6974 6820 7365  n accord with se
+00004d00: 6374 696f 6e20 3720 6170 706c 7920 746f  ction 7 apply to
+00004d10: 2074 6865 2063 6f64 653b 0d0a 6b65 6570   the code;..keep
+00004d20: 2069 6e74 6163 7420 616c 6c20 6e6f 7469   intact all noti
+00004d30: 6365 7320 6f66 2074 6865 2061 6273 656e  ces of the absen
+00004d40: 6365 206f 6620 616e 7920 7761 7272 616e  ce of any warran
+00004d50: 7479 3b20 616e 6420 6769 7665 2061 6c6c  ty; and give all
+00004d60: 0d0a 7265 6369 7069 656e 7473 2061 2063  ..recipients a c
+00004d70: 6f70 7920 6f66 2074 6869 7320 4c69 6365  opy of this Lice
+00004d80: 6e73 6520 616c 6f6e 6720 7769 7468 2074  nse along with t
+00004d90: 6865 2050 726f 6772 616d 2e0d 0a0d 0a20  he Program..... 
+00004da0: 2059 6f75 206d 6179 2063 6861 7267 6520   You may charge 
+00004db0: 616e 7920 7072 6963 6520 6f72 206e 6f20  any price or no 
+00004dc0: 7072 6963 6520 666f 7220 6561 6368 2063  price for each c
+00004dd0: 6f70 7920 7468 6174 2079 6f75 2063 6f6e  opy that you con
+00004de0: 7665 792c 0d0a 616e 6420 796f 7520 6d61  vey,..and you ma
+00004df0: 7920 6f66 6665 7220 7375 7070 6f72 7420  y offer support 
+00004e00: 6f72 2077 6172 7261 6e74 7920 7072 6f74  or warranty prot
+00004e10: 6563 7469 6f6e 2066 6f72 2061 2066 6565  ection for a fee
+00004e20: 2e0d 0a0d 0a20 2035 2e20 436f 6e76 6579  .....  5. Convey
+00004e30: 696e 6720 4d6f 6469 6669 6564 2053 6f75  ing Modified Sou
+00004e40: 7263 6520 5665 7273 696f 6e73 2e0d 0a0d  rce Versions....
+00004e50: 0a20 2059 6f75 206d 6179 2063 6f6e 7665  .  You may conve
+00004e60: 7920 6120 776f 726b 2062 6173 6564 206f  y a work based o
+00004e70: 6e20 7468 6520 5072 6f67 7261 6d2c 206f  n the Program, o
+00004e80: 7220 7468 6520 6d6f 6469 6669 6361 7469  r the modificati
+00004e90: 6f6e 7320 746f 0d0a 7072 6f64 7563 6520  ons to..produce 
+00004ea0: 6974 2066 726f 6d20 7468 6520 5072 6f67  it from the Prog
+00004eb0: 7261 6d2c 2069 6e20 7468 6520 666f 726d  ram, in the form
+00004ec0: 206f 6620 736f 7572 6365 2063 6f64 6520   of source code 
+00004ed0: 756e 6465 7220 7468 650d 0a74 6572 6d73  under the..terms
+00004ee0: 206f 6620 7365 6374 696f 6e20 342c 2070   of section 4, p
+00004ef0: 726f 7669 6465 6420 7468 6174 2079 6f75  rovided that you
+00004f00: 2061 6c73 6f20 6d65 6574 2061 6c6c 206f   also meet all o
+00004f10: 6620 7468 6573 6520 636f 6e64 6974 696f  f these conditio
+00004f20: 6e73 3a0d 0a0d 0a20 2020 2061 2920 5468  ns:....    a) Th
+00004f30: 6520 776f 726b 206d 7573 7420 6361 7272  e work must carr
+00004f40: 7920 7072 6f6d 696e 656e 7420 6e6f 7469  y prominent noti
+00004f50: 6365 7320 7374 6174 696e 6720 7468 6174  ces stating that
+00004f60: 2079 6f75 206d 6f64 6966 6965 640d 0a20   you modified.. 
+00004f70: 2020 2069 742c 2061 6e64 2067 6976 696e     it, and givin
+00004f80: 6720 6120 7265 6c65 7661 6e74 2064 6174  g a relevant dat
+00004f90: 652e 0d0a 0d0a 2020 2020 6229 2054 6865  e.....    b) The
+00004fa0: 2077 6f72 6b20 6d75 7374 2063 6172 7279   work must carry
+00004fb0: 2070 726f 6d69 6e65 6e74 206e 6f74 6963   prominent notic
+00004fc0: 6573 2073 7461 7469 6e67 2074 6861 7420  es stating that 
+00004fd0: 6974 2069 730d 0a20 2020 2072 656c 6561  it is..    relea
+00004fe0: 7365 6420 756e 6465 7220 7468 6973 204c  sed under this L
+00004ff0: 6963 656e 7365 2061 6e64 2061 6e79 2063  icense and any c
+00005000: 6f6e 6469 7469 6f6e 7320 6164 6465 6420  onditions added 
+00005010: 756e 6465 7220 7365 6374 696f 6e0d 0a20  under section.. 
+00005020: 2020 2037 2e20 2054 6869 7320 7265 7175     7.  This requ
+00005030: 6972 656d 656e 7420 6d6f 6469 6669 6573  irement modifies
+00005040: 2074 6865 2072 6571 7569 7265 6d65 6e74   the requirement
+00005050: 2069 6e20 7365 6374 696f 6e20 3420 746f   in section 4 to
+00005060: 0d0a 2020 2020 226b 6565 7020 696e 7461  ..    "keep inta
+00005070: 6374 2061 6c6c 206e 6f74 6963 6573 222e  ct all notices".
+00005080: 0d0a 0d0a 2020 2020 6329 2059 6f75 206d  ....    c) You m
+00005090: 7573 7420 6c69 6365 6e73 6520 7468 6520  ust license the 
+000050a0: 656e 7469 7265 2077 6f72 6b2c 2061 7320  entire work, as 
+000050b0: 6120 7768 6f6c 652c 2075 6e64 6572 2074  a whole, under t
+000050c0: 6869 730d 0a20 2020 204c 6963 656e 7365  his..    License
+000050d0: 2074 6f20 616e 796f 6e65 2077 686f 2063   to anyone who c
+000050e0: 6f6d 6573 2069 6e74 6f20 706f 7373 6573  omes into posses
+000050f0: 7369 6f6e 206f 6620 6120 636f 7079 2e20  sion of a copy. 
+00005100: 2054 6869 730d 0a20 2020 204c 6963 656e   This..    Licen
+00005110: 7365 2077 696c 6c20 7468 6572 6566 6f72  se will therefor
+00005120: 6520 6170 706c 792c 2061 6c6f 6e67 2077  e apply, along w
+00005130: 6974 6820 616e 7920 6170 706c 6963 6162  ith any applicab
+00005140: 6c65 2073 6563 7469 6f6e 2037 0d0a 2020  le section 7..  
+00005150: 2020 6164 6469 7469 6f6e 616c 2074 6572    additional ter
+00005160: 6d73 2c20 746f 2074 6865 2077 686f 6c65  ms, to the whole
+00005170: 206f 6620 7468 6520 776f 726b 2c20 616e   of the work, an
+00005180: 6420 616c 6c20 6974 7320 7061 7274 732c  d all its parts,
+00005190: 0d0a 2020 2020 7265 6761 7264 6c65 7373  ..    regardless
+000051a0: 206f 6620 686f 7720 7468 6579 2061 7265   of how they are
+000051b0: 2070 6163 6b61 6765 642e 2020 5468 6973   packaged.  This
+000051c0: 204c 6963 656e 7365 2067 6976 6573 206e   License gives n
+000051d0: 6f0d 0a20 2020 2070 6572 6d69 7373 696f  o..    permissio
+000051e0: 6e20 746f 206c 6963 656e 7365 2074 6865  n to license the
+000051f0: 2077 6f72 6b20 696e 2061 6e79 206f 7468   work in any oth
+00005200: 6572 2077 6179 2c20 6275 7420 6974 2064  er way, but it d
+00005210: 6f65 7320 6e6f 740d 0a20 2020 2069 6e76  oes not..    inv
+00005220: 616c 6964 6174 6520 7375 6368 2070 6572  alidate such per
+00005230: 6d69 7373 696f 6e20 6966 2079 6f75 2068  mission if you h
+00005240: 6176 6520 7365 7061 7261 7465 6c79 2072  ave separately r
+00005250: 6563 6569 7665 6420 6974 2e0d 0a0d 0a20  eceived it..... 
+00005260: 2020 2064 2920 4966 2074 6865 2077 6f72     d) If the wor
+00005270: 6b20 6861 7320 696e 7465 7261 6374 6976  k has interactiv
+00005280: 6520 7573 6572 2069 6e74 6572 6661 6365  e user interface
+00005290: 732c 2065 6163 6820 6d75 7374 2064 6973  s, each must dis
+000052a0: 706c 6179 0d0a 2020 2020 4170 7072 6f70  play..    Approp
+000052b0: 7269 6174 6520 4c65 6761 6c20 4e6f 7469  riate Legal Noti
+000052c0: 6365 733b 2068 6f77 6576 6572 2c20 6966  ces; however, if
+000052d0: 2074 6865 2050 726f 6772 616d 2068 6173   the Program has
+000052e0: 2069 6e74 6572 6163 7469 7665 0d0a 2020   interactive..  
+000052f0: 2020 696e 7465 7266 6163 6573 2074 6861    interfaces tha
+00005300: 7420 646f 206e 6f74 2064 6973 706c 6179  t do not display
+00005310: 2041 7070 726f 7072 6961 7465 204c 6567   Appropriate Leg
+00005320: 616c 204e 6f74 6963 6573 2c20 796f 7572  al Notices, your
+00005330: 0d0a 2020 2020 776f 726b 206e 6565 6420  ..    work need 
+00005340: 6e6f 7420 6d61 6b65 2074 6865 6d20 646f  not make them do
+00005350: 2073 6f2e 0d0a 0d0a 2020 4120 636f 6d70   so.....  A comp
+00005360: 696c 6174 696f 6e20 6f66 2061 2063 6f76  ilation of a cov
+00005370: 6572 6564 2077 6f72 6b20 7769 7468 206f  ered work with o
+00005380: 7468 6572 2073 6570 6172 6174 6520 616e  ther separate an
+00005390: 6420 696e 6465 7065 6e64 656e 740d 0a77  d independent..w
+000053a0: 6f72 6b73 2c20 7768 6963 6820 6172 6520  orks, which are 
+000053b0: 6e6f 7420 6279 2074 6865 6972 206e 6174  not by their nat
+000053c0: 7572 6520 6578 7465 6e73 696f 6e73 206f  ure extensions o
+000053d0: 6620 7468 6520 636f 7665 7265 6420 776f  f the covered wo
+000053e0: 726b 2c0d 0a61 6e64 2077 6869 6368 2061  rk,..and which a
+000053f0: 7265 206e 6f74 2063 6f6d 6269 6e65 6420  re not combined 
+00005400: 7769 7468 2069 7420 7375 6368 2061 7320  with it such as 
+00005410: 746f 2066 6f72 6d20 6120 6c61 7267 6572  to form a larger
+00005420: 2070 726f 6772 616d 2c0d 0a69 6e20 6f72   program,..in or
+00005430: 206f 6e20 6120 766f 6c75 6d65 206f 6620   on a volume of 
+00005440: 6120 7374 6f72 6167 6520 6f72 2064 6973  a storage or dis
+00005450: 7472 6962 7574 696f 6e20 6d65 6469 756d  tribution medium
+00005460: 2c20 6973 2063 616c 6c65 6420 616e 0d0a  , is called an..
+00005470: 2261 6767 7265 6761 7465 2220 6966 2074  "aggregate" if t
+00005480: 6865 2063 6f6d 7069 6c61 7469 6f6e 2061  he compilation a
+00005490: 6e64 2069 7473 2072 6573 756c 7469 6e67  nd its resulting
+000054a0: 2063 6f70 7972 6967 6874 2061 7265 206e   copyright are n
+000054b0: 6f74 0d0a 7573 6564 2074 6f20 6c69 6d69  ot..used to limi
+000054c0: 7420 7468 6520 6163 6365 7373 206f 7220  t the access or 
+000054d0: 6c65 6761 6c20 7269 6768 7473 206f 6620  legal rights of 
+000054e0: 7468 6520 636f 6d70 696c 6174 696f 6e27  the compilation'
+000054f0: 7320 7573 6572 730d 0a62 6579 6f6e 6420  s users..beyond 
+00005500: 7768 6174 2074 6865 2069 6e64 6976 6964  what the individ
+00005510: 7561 6c20 776f 726b 7320 7065 726d 6974  ual works permit
+00005520: 2e20 2049 6e63 6c75 7369 6f6e 206f 6620  .  Inclusion of 
+00005530: 6120 636f 7665 7265 6420 776f 726b 0d0a  a covered work..
+00005540: 696e 2061 6e20 6167 6772 6567 6174 6520  in an aggregate 
+00005550: 646f 6573 206e 6f74 2063 6175 7365 2074  does not cause t
+00005560: 6869 7320 4c69 6365 6e73 6520 746f 2061  his License to a
+00005570: 7070 6c79 2074 6f20 7468 6520 6f74 6865  pply to the othe
+00005580: 720d 0a70 6172 7473 206f 6620 7468 6520  r..parts of the 
+00005590: 6167 6772 6567 6174 652e 0d0a 0d0a 2020  aggregate.....  
+000055a0: 362e 2043 6f6e 7665 7969 6e67 204e 6f6e  6. Conveying Non
+000055b0: 2d53 6f75 7263 6520 466f 726d 732e 0d0a  -Source Forms...
+000055c0: 0d0a 2020 596f 7520 6d61 7920 636f 6e76  ..  You may conv
+000055d0: 6579 2061 2063 6f76 6572 6564 2077 6f72  ey a covered wor
+000055e0: 6b20 696e 206f 626a 6563 7420 636f 6465  k in object code
+000055f0: 2066 6f72 6d20 756e 6465 7220 7468 6520   form under the 
+00005600: 7465 726d 730d 0a6f 6620 7365 6374 696f  terms..of sectio
+00005610: 6e73 2034 2061 6e64 2035 2c20 7072 6f76  ns 4 and 5, prov
+00005620: 6964 6564 2074 6861 7420 796f 7520 616c  ided that you al
+00005630: 736f 2063 6f6e 7665 7920 7468 650d 0a6d  so convey the..m
+00005640: 6163 6869 6e65 2d72 6561 6461 626c 6520  achine-readable 
+00005650: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
+00005660: 7572 6365 2075 6e64 6572 2074 6865 2074  urce under the t
+00005670: 6572 6d73 206f 6620 7468 6973 204c 6963  erms of this Lic
+00005680: 656e 7365 2c0d 0a69 6e20 6f6e 6520 6f66  ense,..in one of
+00005690: 2074 6865 7365 2077 6179 733a 0d0a 0d0a   these ways:....
+000056a0: 2020 2020 6129 2043 6f6e 7665 7920 7468      a) Convey th
+000056b0: 6520 6f62 6a65 6374 2063 6f64 6520 696e  e object code in
+000056c0: 2c20 6f72 2065 6d62 6f64 6965 6420 696e  , or embodied in
+000056d0: 2c20 6120 7068 7973 6963 616c 2070 726f  , a physical pro
+000056e0: 6475 6374 0d0a 2020 2020 2869 6e63 6c75  duct..    (inclu
+000056f0: 6469 6e67 2061 2070 6879 7369 6361 6c20  ding a physical 
+00005700: 6469 7374 7269 6275 7469 6f6e 206d 6564  distribution med
+00005710: 6975 6d29 2c20 6163 636f 6d70 616e 6965  ium), accompanie
+00005720: 6420 6279 2074 6865 0d0a 2020 2020 436f  d by the..    Co
+00005730: 7272 6573 706f 6e64 696e 6720 536f 7572  rresponding Sour
+00005740: 6365 2066 6978 6564 206f 6e20 6120 6475  ce fixed on a du
+00005750: 7261 626c 6520 7068 7973 6963 616c 206d  rable physical m
+00005760: 6564 6975 6d0d 0a20 2020 2063 7573 746f  edium..    custo
+00005770: 6d61 7269 6c79 2075 7365 6420 666f 7220  marily used for 
+00005780: 736f 6674 7761 7265 2069 6e74 6572 6368  software interch
+00005790: 616e 6765 2e0d 0a0d 0a20 2020 2062 2920  ange.....    b) 
+000057a0: 436f 6e76 6579 2074 6865 206f 626a 6563  Convey the objec
+000057b0: 7420 636f 6465 2069 6e2c 206f 7220 656d  t code in, or em
+000057c0: 626f 6469 6564 2069 6e2c 2061 2070 6879  bodied in, a phy
+000057d0: 7369 6361 6c20 7072 6f64 7563 740d 0a20  sical product.. 
+000057e0: 2020 2028 696e 636c 7564 696e 6720 6120     (including a 
+000057f0: 7068 7973 6963 616c 2064 6973 7472 6962  physical distrib
+00005800: 7574 696f 6e20 6d65 6469 756d 292c 2061  ution medium), a
+00005810: 6363 6f6d 7061 6e69 6564 2062 7920 610d  ccompanied by a.
+00005820: 0a20 2020 2077 7269 7474 656e 206f 6666  .    written off
+00005830: 6572 2c20 7661 6c69 6420 666f 7220 6174  er, valid for at
+00005840: 206c 6561 7374 2074 6872 6565 2079 6561   least three yea
+00005850: 7273 2061 6e64 2076 616c 6964 2066 6f72  rs and valid for
+00005860: 2061 730d 0a20 2020 206c 6f6e 6720 6173   as..    long as
+00005870: 2079 6f75 206f 6666 6572 2073 7061 7265   you offer spare
+00005880: 2070 6172 7473 206f 7220 6375 7374 6f6d   parts or custom
+00005890: 6572 2073 7570 706f 7274 2066 6f72 2074  er support for t
+000058a0: 6861 7420 7072 6f64 7563 740d 0a20 2020  hat product..   
+000058b0: 206d 6f64 656c 2c20 746f 2067 6976 6520   model, to give 
+000058c0: 616e 796f 6e65 2077 686f 2070 6f73 7365  anyone who posse
+000058d0: 7373 6573 2074 6865 206f 626a 6563 7420  sses the object 
+000058e0: 636f 6465 2065 6974 6865 7220 2831 2920  code either (1) 
+000058f0: 610d 0a20 2020 2063 6f70 7920 6f66 2074  a..    copy of t
+00005900: 6865 2043 6f72 7265 7370 6f6e 6469 6e67  he Corresponding
+00005910: 2053 6f75 7263 6520 666f 7220 616c 6c20   Source for all 
+00005920: 7468 6520 736f 6674 7761 7265 2069 6e20  the software in 
+00005930: 7468 650d 0a20 2020 2070 726f 6475 6374  the..    product
+00005940: 2074 6861 7420 6973 2063 6f76 6572 6564   that is covered
+00005950: 2062 7920 7468 6973 204c 6963 656e 7365   by this License
+00005960: 2c20 6f6e 2061 2064 7572 6162 6c65 2070  , on a durable p
+00005970: 6879 7369 6361 6c0d 0a20 2020 206d 6564  hysical..    med
+00005980: 6975 6d20 6375 7374 6f6d 6172 696c 7920  ium customarily 
+00005990: 7573 6564 2066 6f72 2073 6f66 7477 6172  used for softwar
+000059a0: 6520 696e 7465 7263 6861 6e67 652c 2066  e interchange, f
+000059b0: 6f72 2061 2070 7269 6365 206e 6f0d 0a20  or a price no.. 
+000059c0: 2020 206d 6f72 6520 7468 616e 2079 6f75     more than you
+000059d0: 7220 7265 6173 6f6e 6162 6c65 2063 6f73  r reasonable cos
+000059e0: 7420 6f66 2070 6879 7369 6361 6c6c 7920  t of physically 
+000059f0: 7065 7266 6f72 6d69 6e67 2074 6869 730d  performing this.
+00005a00: 0a20 2020 2063 6f6e 7665 7969 6e67 206f  .    conveying o
+00005a10: 6620 736f 7572 6365 2c20 6f72 2028 3229  f source, or (2)
+00005a20: 2061 6363 6573 7320 746f 2063 6f70 7920   access to copy 
+00005a30: 7468 650d 0a20 2020 2043 6f72 7265 7370  the..    Corresp
+00005a40: 6f6e 6469 6e67 2053 6f75 7263 6520 6672  onding Source fr
+00005a50: 6f6d 2061 206e 6574 776f 726b 2073 6572  om a network ser
+00005a60: 7665 7220 6174 206e 6f20 6368 6172 6765  ver at no charge
+00005a70: 2e0d 0a0d 0a20 2020 2063 2920 436f 6e76  .....    c) Conv
+00005a80: 6579 2069 6e64 6976 6964 7561 6c20 636f  ey individual co
+00005a90: 7069 6573 206f 6620 7468 6520 6f62 6a65  pies of the obje
+00005aa0: 6374 2063 6f64 6520 7769 7468 2061 2063  ct code with a c
+00005ab0: 6f70 7920 6f66 2074 6865 0d0a 2020 2020  opy of the..    
+00005ac0: 7772 6974 7465 6e20 6f66 6665 7220 746f  written offer to
+00005ad0: 2070 726f 7669 6465 2074 6865 2043 6f72   provide the Cor
+00005ae0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
+00005af0: 652e 2020 5468 6973 0d0a 2020 2020 616c  e.  This..    al
+00005b00: 7465 726e 6174 6976 6520 6973 2061 6c6c  ternative is all
+00005b10: 6f77 6564 206f 6e6c 7920 6f63 6361 7369  owed only occasi
+00005b20: 6f6e 616c 6c79 2061 6e64 206e 6f6e 636f  onally and nonco
+00005b30: 6d6d 6572 6369 616c 6c79 2c20 616e 640d  mmercially, and.
+00005b40: 0a20 2020 206f 6e6c 7920 6966 2079 6f75  .    only if you
+00005b50: 2072 6563 6569 7665 6420 7468 6520 6f62   received the ob
+00005b60: 6a65 6374 2063 6f64 6520 7769 7468 2073  ject code with s
+00005b70: 7563 6820 616e 206f 6666 6572 2c20 696e  uch an offer, in
+00005b80: 2061 6363 6f72 640d 0a20 2020 2077 6974   accord..    wit
+00005b90: 6820 7375 6273 6563 7469 6f6e 2036 622e  h subsection 6b.
+00005ba0: 0d0a 0d0a 2020 2020 6429 2043 6f6e 7665  ....    d) Conve
+00005bb0: 7920 7468 6520 6f62 6a65 6374 2063 6f64  y the object cod
+00005bc0: 6520 6279 206f 6666 6572 696e 6720 6163  e by offering ac
+00005bd0: 6365 7373 2066 726f 6d20 6120 6465 7369  cess from a desi
+00005be0: 676e 6174 6564 0d0a 2020 2020 706c 6163  gnated..    plac
+00005bf0: 6520 2867 7261 7469 7320 6f72 2066 6f72  e (gratis or for
+00005c00: 2061 2063 6861 7267 6529 2c20 616e 6420   a charge), and 
+00005c10: 6f66 6665 7220 6571 7569 7661 6c65 6e74  offer equivalent
+00005c20: 2061 6363 6573 7320 746f 2074 6865 0d0a   access to the..
+00005c30: 2020 2020 436f 7272 6573 706f 6e64 696e      Correspondin
+00005c40: 6720 536f 7572 6365 2069 6e20 7468 6520  g Source in the 
+00005c50: 7361 6d65 2077 6179 2074 6872 6f75 6768  same way through
+00005c60: 2074 6865 2073 616d 6520 706c 6163 6520   the same place 
+00005c70: 6174 206e 6f0d 0a20 2020 2066 7572 7468  at no..    furth
+00005c80: 6572 2063 6861 7267 652e 2020 596f 7520  er charge.  You 
+00005c90: 6e65 6564 206e 6f74 2072 6571 7569 7265  need not require
+00005ca0: 2072 6563 6970 6965 6e74 7320 746f 2063   recipients to c
+00005cb0: 6f70 7920 7468 650d 0a20 2020 2043 6f72  opy the..    Cor
+00005cc0: 7265 7370 6f6e 6469 6e67 2053 6f75 7263  responding Sourc
+00005cd0: 6520 616c 6f6e 6720 7769 7468 2074 6865  e along with the
+00005ce0: 206f 626a 6563 7420 636f 6465 2e20 2049   object code.  I
+00005cf0: 6620 7468 6520 706c 6163 6520 746f 0d0a  f the place to..
+00005d00: 2020 2020 636f 7079 2074 6865 206f 626a      copy the obj
+00005d10: 6563 7420 636f 6465 2069 7320 6120 6e65  ect code is a ne
+00005d20: 7477 6f72 6b20 7365 7276 6572 2c20 7468  twork server, th
+00005d30: 6520 436f 7272 6573 706f 6e64 696e 6720  e Corresponding 
+00005d40: 536f 7572 6365 0d0a 2020 2020 6d61 7920  Source..    may 
+00005d50: 6265 206f 6e20 6120 6469 6666 6572 656e  be on a differen
+00005d60: 7420 7365 7276 6572 2028 6f70 6572 6174  t server (operat
+00005d70: 6564 2062 7920 796f 7520 6f72 2061 2074  ed by you or a t
+00005d80: 6869 7264 2070 6172 7479 290d 0a20 2020  hird party)..   
+00005d90: 2074 6861 7420 7375 7070 6f72 7473 2065   that supports e
+00005da0: 7175 6976 616c 656e 7420 636f 7079 696e  quivalent copyin
+00005db0: 6720 6661 6369 6c69 7469 6573 2c20 7072  g facilities, pr
+00005dc0: 6f76 6964 6564 2079 6f75 206d 6169 6e74  ovided you maint
+00005dd0: 6169 6e0d 0a20 2020 2063 6c65 6172 2064  ain..    clear d
+00005de0: 6972 6563 7469 6f6e 7320 6e65 7874 2074  irections next t
+00005df0: 6f20 7468 6520 6f62 6a65 6374 2063 6f64  o the object cod
+00005e00: 6520 7361 7969 6e67 2077 6865 7265 2074  e saying where t
+00005e10: 6f20 6669 6e64 2074 6865 0d0a 2020 2020  o find the..    
+00005e20: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
+00005e30: 7572 6365 2e20 2052 6567 6172 646c 6573  urce.  Regardles
+00005e40: 7320 6f66 2077 6861 7420 7365 7276 6572  s of what server
+00005e50: 2068 6f73 7473 2074 6865 0d0a 2020 2020   hosts the..    
+00005e60: 436f 7272 6573 706f 6e64 696e 6720 536f  Corresponding So
+00005e70: 7572 6365 2c20 796f 7520 7265 6d61 696e  urce, you remain
+00005e80: 206f 626c 6967 6174 6564 2074 6f20 656e   obligated to en
+00005e90: 7375 7265 2074 6861 7420 6974 2069 730d  sure that it is.
+00005ea0: 0a20 2020 2061 7661 696c 6162 6c65 2066  .    available f
+00005eb0: 6f72 2061 7320 6c6f 6e67 2061 7320 6e65  or as long as ne
+00005ec0: 6564 6564 2074 6f20 7361 7469 7366 7920  eded to satisfy 
+00005ed0: 7468 6573 6520 7265 7175 6972 656d 656e  these requiremen
+00005ee0: 7473 2e0d 0a0d 0a20 2020 2065 2920 436f  ts.....    e) Co
+00005ef0: 6e76 6579 2074 6865 206f 626a 6563 7420  nvey the object 
+00005f00: 636f 6465 2075 7369 6e67 2070 6565 722d  code using peer-
+00005f10: 746f 2d70 6565 7220 7472 616e 736d 6973  to-peer transmis
+00005f20: 7369 6f6e 2c20 7072 6f76 6964 6564 0d0a  sion, provided..
+00005f30: 2020 2020 796f 7520 696e 666f 726d 206f      you inform o
+00005f40: 7468 6572 2070 6565 7273 2077 6865 7265  ther peers where
+00005f50: 2074 6865 206f 626a 6563 7420 636f 6465   the object code
+00005f60: 2061 6e64 2043 6f72 7265 7370 6f6e 6469   and Correspondi
+00005f70: 6e67 0d0a 2020 2020 536f 7572 6365 206f  ng..    Source o
+00005f80: 6620 7468 6520 776f 726b 2061 7265 2062  f the work are b
+00005f90: 6569 6e67 206f 6666 6572 6564 2074 6f20  eing offered to 
+00005fa0: 7468 6520 6765 6e65 7261 6c20 7075 626c  the general publ
+00005fb0: 6963 2061 7420 6e6f 0d0a 2020 2020 6368  ic at no..    ch
+00005fc0: 6172 6765 2075 6e64 6572 2073 7562 7365  arge under subse
+00005fd0: 6374 696f 6e20 3664 2e0d 0a0d 0a20 2041  ction 6d.....  A
+00005fe0: 2073 6570 6172 6162 6c65 2070 6f72 7469   separable porti
+00005ff0: 6f6e 206f 6620 7468 6520 6f62 6a65 6374  on of the object
+00006000: 2063 6f64 652c 2077 686f 7365 2073 6f75   code, whose sou
+00006010: 7263 6520 636f 6465 2069 7320 6578 636c  rce code is excl
+00006020: 7564 6564 0d0a 6672 6f6d 2074 6865 2043  uded..from the C
+00006030: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
+00006040: 7263 6520 6173 2061 2053 7973 7465 6d20  rce as a System 
+00006050: 4c69 6272 6172 792c 206e 6565 6420 6e6f  Library, need no
+00006060: 7420 6265 0d0a 696e 636c 7564 6564 2069  t be..included i
+00006070: 6e20 636f 6e76 6579 696e 6720 7468 6520  n conveying the 
+00006080: 6f62 6a65 6374 2063 6f64 6520 776f 726b  object code work
+00006090: 2e0d 0a0d 0a20 2041 2022 5573 6572 2050  .....  A "User P
+000060a0: 726f 6475 6374 2220 6973 2065 6974 6865  roduct" is eithe
+000060b0: 7220 2831 2920 6120 2263 6f6e 7375 6d65  r (1) a "consume
+000060c0: 7220 7072 6f64 7563 7422 2c20 7768 6963  r product", whic
+000060d0: 6820 6d65 616e 7320 616e 790d 0a74 616e  h means any..tan
+000060e0: 6769 626c 6520 7065 7273 6f6e 616c 2070  gible personal p
+000060f0: 726f 7065 7274 7920 7768 6963 6820 6973  roperty which is
+00006100: 206e 6f72 6d61 6c6c 7920 7573 6564 2066   normally used f
+00006110: 6f72 2070 6572 736f 6e61 6c2c 2066 616d  or personal, fam
+00006120: 696c 792c 0d0a 6f72 2068 6f75 7365 686f  ily,..or househo
+00006130: 6c64 2070 7572 706f 7365 732c 206f 7220  ld purposes, or 
+00006140: 2832 2920 616e 7974 6869 6e67 2064 6573  (2) anything des
+00006150: 6967 6e65 6420 6f72 2073 6f6c 6420 666f  igned or sold fo
+00006160: 7220 696e 636f 7270 6f72 6174 696f 6e0d  r incorporation.
+00006170: 0a69 6e74 6f20 6120 6477 656c 6c69 6e67  .into a dwelling
+00006180: 2e20 2049 6e20 6465 7465 726d 696e 696e  .  In determinin
+00006190: 6720 7768 6574 6865 7220 6120 7072 6f64  g whether a prod
+000061a0: 7563 7420 6973 2061 2063 6f6e 7375 6d65  uct is a consume
+000061b0: 7220 7072 6f64 7563 742c 0d0a 646f 7562  r product,..doub
+000061c0: 7466 756c 2063 6173 6573 2073 6861 6c6c  tful cases shall
+000061d0: 2062 6520 7265 736f 6c76 6564 2069 6e20   be resolved in 
+000061e0: 6661 766f 7220 6f66 2063 6f76 6572 6167  favor of coverag
+000061f0: 652e 2020 466f 7220 6120 7061 7274 6963  e.  For a partic
+00006200: 756c 6172 0d0a 7072 6f64 7563 7420 7265  ular..product re
+00006210: 6365 6976 6564 2062 7920 6120 7061 7274  ceived by a part
+00006220: 6963 756c 6172 2075 7365 722c 2022 6e6f  icular user, "no
+00006230: 726d 616c 6c79 2075 7365 6422 2072 6566  rmally used" ref
+00006240: 6572 7320 746f 2061 0d0a 7479 7069 6361  ers to a..typica
+00006250: 6c20 6f72 2063 6f6d 6d6f 6e20 7573 6520  l or common use 
+00006260: 6f66 2074 6861 7420 636c 6173 7320 6f66  of that class of
+00006270: 2070 726f 6475 6374 2c20 7265 6761 7264   product, regard
+00006280: 6c65 7373 206f 6620 7468 6520 7374 6174  less of the stat
+00006290: 7573 0d0a 6f66 2074 6865 2070 6172 7469  us..of the parti
+000062a0: 6375 6c61 7220 7573 6572 206f 7220 6f66  cular user or of
+000062b0: 2074 6865 2077 6179 2069 6e20 7768 6963   the way in whic
+000062c0: 6820 7468 6520 7061 7274 6963 756c 6172  h the particular
+000062d0: 2075 7365 720d 0a61 6374 7561 6c6c 7920   user..actually 
+000062e0: 7573 6573 2c20 6f72 2065 7870 6563 7473  uses, or expects
+000062f0: 206f 7220 6973 2065 7870 6563 7465 6420   or is expected 
+00006300: 746f 2075 7365 2c20 7468 6520 7072 6f64  to use, the prod
+00006310: 7563 742e 2020 4120 7072 6f64 7563 740d  uct.  A product.
+00006320: 0a69 7320 6120 636f 6e73 756d 6572 2070  .is a consumer p
+00006330: 726f 6475 6374 2072 6567 6172 646c 6573  roduct regardles
+00006340: 7320 6f66 2077 6865 7468 6572 2074 6865  s of whether the
+00006350: 2070 726f 6475 6374 2068 6173 2073 7562   product has sub
+00006360: 7374 616e 7469 616c 0d0a 636f 6d6d 6572  stantial..commer
+00006370: 6369 616c 2c20 696e 6475 7374 7269 616c  cial, industrial
+00006380: 206f 7220 6e6f 6e2d 636f 6e73 756d 6572   or non-consumer
+00006390: 2075 7365 732c 2075 6e6c 6573 7320 7375   uses, unless su
+000063a0: 6368 2075 7365 7320 7265 7072 6573 656e  ch uses represen
+000063b0: 740d 0a74 6865 206f 6e6c 7920 7369 676e  t..the only sign
+000063c0: 6966 6963 616e 7420 6d6f 6465 206f 6620  ificant mode of 
+000063d0: 7573 6520 6f66 2074 6865 2070 726f 6475  use of the produ
+000063e0: 6374 2e0d 0a0d 0a20 2022 496e 7374 616c  ct.....  "Instal
+000063f0: 6c61 7469 6f6e 2049 6e66 6f72 6d61 7469  lation Informati
+00006400: 6f6e 2220 666f 7220 6120 5573 6572 2050  on" for a User P
+00006410: 726f 6475 6374 206d 6561 6e73 2061 6e79  roduct means any
+00006420: 206d 6574 686f 6473 2c0d 0a70 726f 6365   methods,..proce
+00006430: 6475 7265 732c 2061 7574 686f 7269 7a61  dures, authoriza
+00006440: 7469 6f6e 206b 6579 732c 206f 7220 6f74  tion keys, or ot
+00006450: 6865 7220 696e 666f 726d 6174 696f 6e20  her information 
+00006460: 7265 7175 6972 6564 2074 6f20 696e 7374  required to inst
+00006470: 616c 6c0d 0a61 6e64 2065 7865 6375 7465  all..and execute
+00006480: 206d 6f64 6966 6965 6420 7665 7273 696f   modified versio
+00006490: 6e73 206f 6620 6120 636f 7665 7265 6420  ns of a covered 
+000064a0: 776f 726b 2069 6e20 7468 6174 2055 7365  work in that Use
+000064b0: 7220 5072 6f64 7563 7420 6672 6f6d 0d0a  r Product from..
+000064c0: 6120 6d6f 6469 6669 6564 2076 6572 7369  a modified versi
+000064d0: 6f6e 206f 6620 6974 7320 436f 7272 6573  on of its Corres
+000064e0: 706f 6e64 696e 6720 536f 7572 6365 2e20  ponding Source. 
+000064f0: 2054 6865 2069 6e66 6f72 6d61 7469 6f6e   The information
+00006500: 206d 7573 740d 0a73 7566 6669 6365 2074   must..suffice t
+00006510: 6f20 656e 7375 7265 2074 6861 7420 7468  o ensure that th
+00006520: 6520 636f 6e74 696e 7565 6420 6675 6e63  e continued func
+00006530: 7469 6f6e 696e 6720 6f66 2074 6865 206d  tioning of the m
+00006540: 6f64 6966 6965 6420 6f62 6a65 6374 0d0a  odified object..
+00006550: 636f 6465 2069 7320 696e 206e 6f20 6361  code is in no ca
+00006560: 7365 2070 7265 7665 6e74 6564 206f 7220  se prevented or 
+00006570: 696e 7465 7266 6572 6564 2077 6974 6820  interfered with 
+00006580: 736f 6c65 6c79 2062 6563 6175 7365 0d0a  solely because..
+00006590: 6d6f 6469 6669 6361 7469 6f6e 2068 6173  modification has
+000065a0: 2062 6565 6e20 6d61 6465 2e0d 0a0d 0a20   been made..... 
+000065b0: 2049 6620 796f 7520 636f 6e76 6579 2061   If you convey a
+000065c0: 6e20 6f62 6a65 6374 2063 6f64 6520 776f  n object code wo
+000065d0: 726b 2075 6e64 6572 2074 6869 7320 7365  rk under this se
+000065e0: 6374 696f 6e20 696e 2c20 6f72 2077 6974  ction in, or wit
+000065f0: 682c 206f 720d 0a73 7065 6369 6669 6361  h, or..specifica
+00006600: 6c6c 7920 666f 7220 7573 6520 696e 2c20  lly for use in, 
+00006610: 6120 5573 6572 2050 726f 6475 6374 2c20  a User Product, 
+00006620: 616e 6420 7468 6520 636f 6e76 6579 696e  and the conveyin
+00006630: 6720 6f63 6375 7273 2061 730d 0a70 6172  g occurs as..par
+00006640: 7420 6f66 2061 2074 7261 6e73 6163 7469  t of a transacti
+00006650: 6f6e 2069 6e20 7768 6963 6820 7468 6520  on in which the 
+00006660: 7269 6768 7420 6f66 2070 6f73 7365 7373  right of possess
+00006670: 696f 6e20 616e 6420 7573 6520 6f66 2074  ion and use of t
+00006680: 6865 0d0a 5573 6572 2050 726f 6475 6374  he..User Product
+00006690: 2069 7320 7472 616e 7366 6572 7265 6420   is transferred 
+000066a0: 746f 2074 6865 2072 6563 6970 6965 6e74  to the recipient
+000066b0: 2069 6e20 7065 7270 6574 7569 7479 206f   in perpetuity o
+000066c0: 7220 666f 7220 610d 0a66 6978 6564 2074  r for a..fixed t
+000066d0: 6572 6d20 2872 6567 6172 646c 6573 7320  erm (regardless 
+000066e0: 6f66 2068 6f77 2074 6865 2074 7261 6e73  of how the trans
+000066f0: 6163 7469 6f6e 2069 7320 6368 6172 6163  action is charac
+00006700: 7465 7269 7a65 6429 2c20 7468 650d 0a43  terized), the..C
+00006710: 6f72 7265 7370 6f6e 6469 6e67 2053 6f75  orresponding Sou
+00006720: 7263 6520 636f 6e76 6579 6564 2075 6e64  rce conveyed und
+00006730: 6572 2074 6869 7320 7365 6374 696f 6e20  er this section 
+00006740: 6d75 7374 2062 6520 6163 636f 6d70 616e  must be accompan
+00006750: 6965 640d 0a62 7920 7468 6520 496e 7374  ied..by the Inst
+00006760: 616c 6c61 7469 6f6e 2049 6e66 6f72 6d61  allation Informa
+00006770: 7469 6f6e 2e20 2042 7574 2074 6869 7320  tion.  But this 
+00006780: 7265 7175 6972 656d 656e 7420 646f 6573  requirement does
+00006790: 206e 6f74 2061 7070 6c79 0d0a 6966 206e   not apply..if n
+000067a0: 6569 7468 6572 2079 6f75 206e 6f72 2061  either you nor a
+000067b0: 6e79 2074 6869 7264 2070 6172 7479 2072  ny third party r
+000067c0: 6574 6169 6e73 2074 6865 2061 6269 6c69  etains the abili
+000067d0: 7479 2074 6f20 696e 7374 616c 6c0d 0a6d  ty to install..m
+000067e0: 6f64 6966 6965 6420 6f62 6a65 6374 2063  odified object c
+000067f0: 6f64 6520 6f6e 2074 6865 2055 7365 7220  ode on the User 
+00006800: 5072 6f64 7563 7420 2866 6f72 2065 7861  Product (for exa
+00006810: 6d70 6c65 2c20 7468 6520 776f 726b 2068  mple, the work h
+00006820: 6173 0d0a 6265 656e 2069 6e73 7461 6c6c  as..been install
+00006830: 6564 2069 6e20 524f 4d29 2e0d 0a0d 0a20  ed in ROM)..... 
+00006840: 2054 6865 2072 6571 7569 7265 6d65 6e74   The requirement
+00006850: 2074 6f20 7072 6f76 6964 6520 496e 7374   to provide Inst
+00006860: 616c 6c61 7469 6f6e 2049 6e66 6f72 6d61  allation Informa
+00006870: 7469 6f6e 2064 6f65 7320 6e6f 7420 696e  tion does not in
+00006880: 636c 7564 6520 610d 0a72 6571 7569 7265  clude a..require
+00006890: 6d65 6e74 2074 6f20 636f 6e74 696e 7565  ment to continue
+000068a0: 2074 6f20 7072 6f76 6964 6520 7375 7070   to provide supp
+000068b0: 6f72 7420 7365 7276 6963 652c 2077 6172  ort service, war
+000068c0: 7261 6e74 792c 206f 7220 7570 6461 7465  ranty, or update
+000068d0: 730d 0a66 6f72 2061 2077 6f72 6b20 7468  s..for a work th
+000068e0: 6174 2068 6173 2062 6565 6e20 6d6f 6469  at has been modi
+000068f0: 6669 6564 206f 7220 696e 7374 616c 6c65  fied or installe
+00006900: 6420 6279 2074 6865 2072 6563 6970 6965  d by the recipie
+00006910: 6e74 2c20 6f72 2066 6f72 0d0a 7468 6520  nt, or for..the 
+00006920: 5573 6572 2050 726f 6475 6374 2069 6e20  User Product in 
+00006930: 7768 6963 6820 6974 2068 6173 2062 6565  which it has bee
+00006940: 6e20 6d6f 6469 6669 6564 206f 7220 696e  n modified or in
+00006950: 7374 616c 6c65 642e 2020 4163 6365 7373  stalled.  Access
+00006960: 2074 6f20 610d 0a6e 6574 776f 726b 206d   to a..network m
+00006970: 6179 2062 6520 6465 6e69 6564 2077 6865  ay be denied whe
+00006980: 6e20 7468 6520 6d6f 6469 6669 6361 7469  n the modificati
+00006990: 6f6e 2069 7473 656c 6620 6d61 7465 7269  on itself materi
+000069a0: 616c 6c79 2061 6e64 0d0a 6164 7665 7273  ally and..advers
+000069b0: 656c 7920 6166 6665 6374 7320 7468 6520  ely affects the 
+000069c0: 6f70 6572 6174 696f 6e20 6f66 2074 6865  operation of the
+000069d0: 206e 6574 776f 726b 206f 7220 7669 6f6c   network or viol
+000069e0: 6174 6573 2074 6865 2072 756c 6573 2061  ates the rules a
+000069f0: 6e64 0d0a 7072 6f74 6f63 6f6c 7320 666f  nd..protocols fo
+00006a00: 7220 636f 6d6d 756e 6963 6174 696f 6e20  r communication 
+00006a10: 6163 726f 7373 2074 6865 206e 6574 776f  across the netwo
+00006a20: 726b 2e0d 0a0d 0a20 2043 6f72 7265 7370  rk.....  Corresp
+00006a30: 6f6e 6469 6e67 2053 6f75 7263 6520 636f  onding Source co
+00006a40: 6e76 6579 6564 2c20 616e 6420 496e 7374  nveyed, and Inst
+00006a50: 616c 6c61 7469 6f6e 2049 6e66 6f72 6d61  allation Informa
+00006a60: 7469 6f6e 2070 726f 7669 6465 642c 0d0a  tion provided,..
+00006a70: 696e 2061 6363 6f72 6420 7769 7468 2074  in accord with t
+00006a80: 6869 7320 7365 6374 696f 6e20 6d75 7374  his section must
+00006a90: 2062 6520 696e 2061 2066 6f72 6d61 7420   be in a format 
+00006aa0: 7468 6174 2069 7320 7075 626c 6963 6c79  that is publicly
+00006ab0: 0d0a 646f 6375 6d65 6e74 6564 2028 616e  ..documented (an
+00006ac0: 6420 7769 7468 2061 6e20 696d 706c 656d  d with an implem
+00006ad0: 656e 7461 7469 6f6e 2061 7661 696c 6162  entation availab
+00006ae0: 6c65 2074 6f20 7468 6520 7075 626c 6963  le to the public
+00006af0: 2069 6e0d 0a73 6f75 7263 6520 636f 6465   in..source code
+00006b00: 2066 6f72 6d29 2c20 616e 6420 6d75 7374   form), and must
+00006b10: 2072 6571 7569 7265 206e 6f20 7370 6563   require no spec
+00006b20: 6961 6c20 7061 7373 776f 7264 206f 7220  ial password or 
+00006b30: 6b65 7920 666f 720d 0a75 6e70 6163 6b69  key for..unpacki
+00006b40: 6e67 2c20 7265 6164 696e 6720 6f72 2063  ng, reading or c
+00006b50: 6f70 7969 6e67 2e0d 0a0d 0a20 2037 2e20  opying.....  7. 
+00006b60: 4164 6469 7469 6f6e 616c 2054 6572 6d73  Additional Terms
+00006b70: 2e0d 0a0d 0a20 2022 4164 6469 7469 6f6e  .....  "Addition
+00006b80: 616c 2070 6572 6d69 7373 696f 6e73 2220  al permissions" 
+00006b90: 6172 6520 7465 726d 7320 7468 6174 2073  are terms that s
+00006ba0: 7570 706c 656d 656e 7420 7468 6520 7465  upplement the te
+00006bb0: 726d 7320 6f66 2074 6869 730d 0a4c 6963  rms of this..Lic
+00006bc0: 656e 7365 2062 7920 6d61 6b69 6e67 2065  ense by making e
+00006bd0: 7863 6570 7469 6f6e 7320 6672 6f6d 206f  xceptions from o
+00006be0: 6e65 206f 7220 6d6f 7265 206f 6620 6974  ne or more of it
+00006bf0: 7320 636f 6e64 6974 696f 6e73 2e0d 0a41  s conditions...A
+00006c00: 6464 6974 696f 6e61 6c20 7065 726d 6973  dditional permis
+00006c10: 7369 6f6e 7320 7468 6174 2061 7265 2061  sions that are a
+00006c20: 7070 6c69 6361 626c 6520 746f 2074 6865  pplicable to the
+00006c30: 2065 6e74 6972 6520 5072 6f67 7261 6d20   entire Program 
+00006c40: 7368 616c 6c0d 0a62 6520 7472 6561 7465  shall..be treate
+00006c50: 6420 6173 2074 686f 7567 6820 7468 6579  d as though they
+00006c60: 2077 6572 6520 696e 636c 7564 6564 2069   were included i
+00006c70: 6e20 7468 6973 204c 6963 656e 7365 2c20  n this License, 
+00006c80: 746f 2074 6865 2065 7874 656e 740d 0a74  to the extent..t
+00006c90: 6861 7420 7468 6579 2061 7265 2076 616c  hat they are val
+00006ca0: 6964 2075 6e64 6572 2061 7070 6c69 6361  id under applica
+00006cb0: 626c 6520 6c61 772e 2020 4966 2061 6464  ble law.  If add
+00006cc0: 6974 696f 6e61 6c20 7065 726d 6973 7369  itional permissi
+00006cd0: 6f6e 730d 0a61 7070 6c79 206f 6e6c 7920  ons..apply only 
+00006ce0: 746f 2070 6172 7420 6f66 2074 6865 2050  to part of the P
+00006cf0: 726f 6772 616d 2c20 7468 6174 2070 6172  rogram, that par
+00006d00: 7420 6d61 7920 6265 2075 7365 6420 7365  t may be used se
+00006d10: 7061 7261 7465 6c79 0d0a 756e 6465 7220  parately..under 
+00006d20: 7468 6f73 6520 7065 726d 6973 7369 6f6e  those permission
+00006d30: 732c 2062 7574 2074 6865 2065 6e74 6972  s, but the entir
+00006d40: 6520 5072 6f67 7261 6d20 7265 6d61 696e  e Program remain
+00006d50: 7320 676f 7665 726e 6564 2062 790d 0a74  s governed by..t
+00006d60: 6869 7320 4c69 6365 6e73 6520 7769 7468  his License with
+00006d70: 6f75 7420 7265 6761 7264 2074 6f20 7468  out regard to th
+00006d80: 6520 6164 6469 7469 6f6e 616c 2070 6572  e additional per
+00006d90: 6d69 7373 696f 6e73 2e0d 0a0d 0a20 2057  missions.....  W
+00006da0: 6865 6e20 796f 7520 636f 6e76 6579 2061  hen you convey a
+00006db0: 2063 6f70 7920 6f66 2061 2063 6f76 6572   copy of a cover
+00006dc0: 6564 2077 6f72 6b2c 2079 6f75 206d 6179  ed work, you may
+00006dd0: 2061 7420 796f 7572 206f 7074 696f 6e0d   at your option.
+00006de0: 0a72 656d 6f76 6520 616e 7920 6164 6469  .remove any addi
+00006df0: 7469 6f6e 616c 2070 6572 6d69 7373 696f  tional permissio
+00006e00: 6e73 2066 726f 6d20 7468 6174 2063 6f70  ns from that cop
+00006e10: 792c 206f 7220 6672 6f6d 2061 6e79 2070  y, or from any p
+00006e20: 6172 7420 6f66 0d0a 6974 2e20 2028 4164  art of..it.  (Ad
+00006e30: 6469 7469 6f6e 616c 2070 6572 6d69 7373  ditional permiss
+00006e40: 696f 6e73 206d 6179 2062 6520 7772 6974  ions may be writ
+00006e50: 7465 6e20 746f 2072 6571 7569 7265 2074  ten to require t
+00006e60: 6865 6972 206f 776e 0d0a 7265 6d6f 7661  heir own..remova
+00006e70: 6c20 696e 2063 6572 7461 696e 2063 6173  l in certain cas
+00006e80: 6573 2077 6865 6e20 796f 7520 6d6f 6469  es when you modi
+00006e90: 6679 2074 6865 2077 6f72 6b2e 2920 2059  fy the work.)  Y
+00006ea0: 6f75 206d 6179 2070 6c61 6365 0d0a 6164  ou may place..ad
+00006eb0: 6469 7469 6f6e 616c 2070 6572 6d69 7373  ditional permiss
+00006ec0: 696f 6e73 206f 6e20 6d61 7465 7269 616c  ions on material
+00006ed0: 2c20 6164 6465 6420 6279 2079 6f75 2074  , added by you t
+00006ee0: 6f20 6120 636f 7665 7265 6420 776f 726b  o a covered work
+00006ef0: 2c0d 0a66 6f72 2077 6869 6368 2079 6f75  ,..for which you
+00006f00: 2068 6176 6520 6f72 2063 616e 2067 6976   have or can giv
+00006f10: 6520 6170 7072 6f70 7269 6174 6520 636f  e appropriate co
+00006f20: 7079 7269 6768 7420 7065 726d 6973 7369  pyright permissi
+00006f30: 6f6e 2e0d 0a0d 0a20 204e 6f74 7769 7468  on.....  Notwith
+00006f40: 7374 616e 6469 6e67 2061 6e79 206f 7468  standing any oth
+00006f50: 6572 2070 726f 7669 7369 6f6e 206f 6620  er provision of 
+00006f60: 7468 6973 204c 6963 656e 7365 2c20 666f  this License, fo
+00006f70: 7220 6d61 7465 7269 616c 2079 6f75 0d0a  r material you..
+00006f80: 6164 6420 746f 2061 2063 6f76 6572 6564  add to a covered
+00006f90: 2077 6f72 6b2c 2079 6f75 206d 6179 2028   work, you may (
+00006fa0: 6966 2061 7574 686f 7269 7a65 6420 6279  if authorized by
+00006fb0: 2074 6865 2063 6f70 7972 6967 6874 2068   the copyright h
+00006fc0: 6f6c 6465 7273 206f 660d 0a74 6861 7420  olders of..that 
+00006fd0: 6d61 7465 7269 616c 2920 7375 7070 6c65  material) supple
+00006fe0: 6d65 6e74 2074 6865 2074 6572 6d73 206f  ment the terms o
+00006ff0: 6620 7468 6973 204c 6963 656e 7365 2077  f this License w
+00007000: 6974 6820 7465 726d 733a 0d0a 0d0a 2020  ith terms:....  
+00007010: 2020 6129 2044 6973 636c 6169 6d69 6e67    a) Disclaiming
+00007020: 2077 6172 7261 6e74 7920 6f72 206c 696d   warranty or lim
+00007030: 6974 696e 6720 6c69 6162 696c 6974 7920  iting liability 
+00007040: 6469 6666 6572 656e 746c 7920 6672 6f6d  differently from
+00007050: 2074 6865 0d0a 2020 2020 7465 726d 7320   the..    terms 
+00007060: 6f66 2073 6563 7469 6f6e 7320 3135 2061  of sections 15 a
+00007070: 6e64 2031 3620 6f66 2074 6869 7320 4c69  nd 16 of this Li
+00007080: 6365 6e73 653b 206f 720d 0a0d 0a20 2020  cense; or....   
+00007090: 2062 2920 5265 7175 6972 696e 6720 7072   b) Requiring pr
+000070a0: 6573 6572 7661 7469 6f6e 206f 6620 7370  eservation of sp
+000070b0: 6563 6966 6965 6420 7265 6173 6f6e 6162  ecified reasonab
+000070c0: 6c65 206c 6567 616c 206e 6f74 6963 6573  le legal notices
+000070d0: 206f 720d 0a20 2020 2061 7574 686f 7220   or..    author 
+000070e0: 6174 7472 6962 7574 696f 6e73 2069 6e20  attributions in 
+000070f0: 7468 6174 206d 6174 6572 6961 6c20 6f72  that material or
+00007100: 2069 6e20 7468 6520 4170 7072 6f70 7269   in the Appropri
+00007110: 6174 6520 4c65 6761 6c0d 0a20 2020 204e  ate Legal..    N
+00007120: 6f74 6963 6573 2064 6973 706c 6179 6564  otices displayed
+00007130: 2062 7920 776f 726b 7320 636f 6e74 6169   by works contai
+00007140: 6e69 6e67 2069 743b 206f 720d 0a0d 0a20  ning it; or.... 
+00007150: 2020 2063 2920 5072 6f68 6962 6974 696e     c) Prohibitin
+00007160: 6720 6d69 7372 6570 7265 7365 6e74 6174  g misrepresentat
+00007170: 696f 6e20 6f66 2074 6865 206f 7269 6769  ion of the origi
+00007180: 6e20 6f66 2074 6861 7420 6d61 7465 7269  n of that materi
+00007190: 616c 2c20 6f72 0d0a 2020 2020 7265 7175  al, or..    requ
+000071a0: 6972 696e 6720 7468 6174 206d 6f64 6966  iring that modif
+000071b0: 6965 6420 7665 7273 696f 6e73 206f 6620  ied versions of 
+000071c0: 7375 6368 206d 6174 6572 6961 6c20 6265  such material be
+000071d0: 206d 6172 6b65 6420 696e 0d0a 2020 2020   marked in..    
+000071e0: 7265 6173 6f6e 6162 6c65 2077 6179 7320  reasonable ways 
+000071f0: 6173 2064 6966 6665 7265 6e74 2066 726f  as different fro
+00007200: 6d20 7468 6520 6f72 6967 696e 616c 2076  m the original v
+00007210: 6572 7369 6f6e 3b20 6f72 0d0a 0d0a 2020  ersion; or....  
+00007220: 2020 6429 204c 696d 6974 696e 6720 7468    d) Limiting th
+00007230: 6520 7573 6520 666f 7220 7075 626c 6963  e use for public
+00007240: 6974 7920 7075 7270 6f73 6573 206f 6620  ity purposes of 
+00007250: 6e61 6d65 7320 6f66 206c 6963 656e 736f  names of licenso
+00007260: 7273 206f 720d 0a20 2020 2061 7574 686f  rs or..    autho
+00007270: 7273 206f 6620 7468 6520 6d61 7465 7269  rs of the materi
+00007280: 616c 3b20 6f72 0d0a 0d0a 2020 2020 6529  al; or....    e)
+00007290: 2044 6563 6c69 6e69 6e67 2074 6f20 6772   Declining to gr
+000072a0: 616e 7420 7269 6768 7473 2075 6e64 6572  ant rights under
+000072b0: 2074 7261 6465 6d61 726b 206c 6177 2066   trademark law f
+000072c0: 6f72 2075 7365 206f 6620 736f 6d65 0d0a  or use of some..
+000072d0: 2020 2020 7472 6164 6520 6e61 6d65 732c      trade names,
+000072e0: 2074 7261 6465 6d61 726b 732c 206f 7220   trademarks, or 
+000072f0: 7365 7276 6963 6520 6d61 726b 733b 206f  service marks; o
+00007300: 720d 0a0d 0a20 2020 2066 2920 5265 7175  r....    f) Requ
+00007310: 6972 696e 6720 696e 6465 6d6e 6966 6963  iring indemnific
+00007320: 6174 696f 6e20 6f66 206c 6963 656e 736f  ation of licenso
+00007330: 7273 2061 6e64 2061 7574 686f 7273 206f  rs and authors o
+00007340: 6620 7468 6174 0d0a 2020 2020 6d61 7465  f that..    mate
+00007350: 7269 616c 2062 7920 616e 796f 6e65 2077  rial by anyone w
+00007360: 686f 2063 6f6e 7665 7973 2074 6865 206d  ho conveys the m
+00007370: 6174 6572 6961 6c20 286f 7220 6d6f 6469  aterial (or modi
+00007380: 6669 6564 2076 6572 7369 6f6e 7320 6f66  fied versions of
+00007390: 0d0a 2020 2020 6974 2920 7769 7468 2063  ..    it) with c
+000073a0: 6f6e 7472 6163 7475 616c 2061 7373 756d  ontractual assum
+000073b0: 7074 696f 6e73 206f 6620 6c69 6162 696c  ptions of liabil
+000073c0: 6974 7920 746f 2074 6865 2072 6563 6970  ity to the recip
+000073d0: 6965 6e74 2c20 666f 720d 0a20 2020 2061  ient, for..    a
+000073e0: 6e79 206c 6961 6269 6c69 7479 2074 6861  ny liability tha
+000073f0: 7420 7468 6573 6520 636f 6e74 7261 6374  t these contract
+00007400: 7561 6c20 6173 7375 6d70 7469 6f6e 7320  ual assumptions 
+00007410: 6469 7265 6374 6c79 2069 6d70 6f73 6520  directly impose 
+00007420: 6f6e 0d0a 2020 2020 7468 6f73 6520 6c69  on..    those li
+00007430: 6365 6e73 6f72 7320 616e 6420 6175 7468  censors and auth
+00007440: 6f72 732e 0d0a 0d0a 2020 416c 6c20 6f74  ors.....  All ot
+00007450: 6865 7220 6e6f 6e2d 7065 726d 6973 7369  her non-permissi
+00007460: 7665 2061 6464 6974 696f 6e61 6c20 7465  ve additional te
+00007470: 726d 7320 6172 6520 636f 6e73 6964 6572  rms are consider
+00007480: 6564 2022 6675 7274 6865 720d 0a72 6573  ed "further..res
+00007490: 7472 6963 7469 6f6e 7322 2077 6974 6869  trictions" withi
+000074a0: 6e20 7468 6520 6d65 616e 696e 6720 6f66  n the meaning of
+000074b0: 2073 6563 7469 6f6e 2031 302e 2020 4966   section 10.  If
+000074c0: 2074 6865 2050 726f 6772 616d 2061 7320   the Program as 
+000074d0: 796f 750d 0a72 6563 6569 7665 6420 6974  you..received it
+000074e0: 2c20 6f72 2061 6e79 2070 6172 7420 6f66  , or any part of
+000074f0: 2069 742c 2063 6f6e 7461 696e 7320 6120   it, contains a 
+00007500: 6e6f 7469 6365 2073 7461 7469 6e67 2074  notice stating t
+00007510: 6861 7420 6974 2069 730d 0a67 6f76 6572  hat it is..gover
+00007520: 6e65 6420 6279 2074 6869 7320 4c69 6365  ned by this Lice
+00007530: 6e73 6520 616c 6f6e 6720 7769 7468 2061  nse along with a
+00007540: 2074 6572 6d20 7468 6174 2069 7320 6120   term that is a 
+00007550: 6675 7274 6865 720d 0a72 6573 7472 6963  further..restric
+00007560: 7469 6f6e 2c20 796f 7520 6d61 7920 7265  tion, you may re
+00007570: 6d6f 7665 2074 6861 7420 7465 726d 2e20  move that term. 
+00007580: 2049 6620 6120 6c69 6365 6e73 6520 646f   If a license do
+00007590: 6375 6d65 6e74 2063 6f6e 7461 696e 730d  cument contains.
+000075a0: 0a61 2066 7572 7468 6572 2072 6573 7472  .a further restr
+000075b0: 6963 7469 6f6e 2062 7574 2070 6572 6d69  iction but permi
+000075c0: 7473 2072 656c 6963 656e 7369 6e67 206f  ts relicensing o
+000075d0: 7220 636f 6e76 6579 696e 6720 756e 6465  r conveying unde
+000075e0: 7220 7468 6973 0d0a 4c69 6365 6e73 652c  r this..License,
+000075f0: 2079 6f75 206d 6179 2061 6464 2074 6f20   you may add to 
+00007600: 6120 636f 7665 7265 6420 776f 726b 206d  a covered work m
+00007610: 6174 6572 6961 6c20 676f 7665 726e 6564  aterial governed
+00007620: 2062 7920 7468 6520 7465 726d 730d 0a6f   by the terms..o
+00007630: 6620 7468 6174 206c 6963 656e 7365 2064  f that license d
+00007640: 6f63 756d 656e 742c 2070 726f 7669 6465  ocument, provide
+00007650: 6420 7468 6174 2074 6865 2066 7572 7468  d that the furth
+00007660: 6572 2072 6573 7472 6963 7469 6f6e 2064  er restriction d
+00007670: 6f65 730d 0a6e 6f74 2073 7572 7669 7665  oes..not survive
+00007680: 2073 7563 6820 7265 6c69 6365 6e73 696e   such relicensin
+00007690: 6720 6f72 2063 6f6e 7665 7969 6e67 2e0d  g or conveying..
+000076a0: 0a0d 0a20 2049 6620 796f 7520 6164 6420  ...  If you add 
+000076b0: 7465 726d 7320 746f 2061 2063 6f76 6572  terms to a cover
+000076c0: 6564 2077 6f72 6b20 696e 2061 6363 6f72  ed work in accor
+000076d0: 6420 7769 7468 2074 6869 7320 7365 6374  d with this sect
+000076e0: 696f 6e2c 2079 6f75 0d0a 6d75 7374 2070  ion, you..must p
+000076f0: 6c61 6365 2c20 696e 2074 6865 2072 656c  lace, in the rel
+00007700: 6576 616e 7420 736f 7572 6365 2066 696c  evant source fil
+00007710: 6573 2c20 6120 7374 6174 656d 656e 7420  es, a statement 
+00007720: 6f66 2074 6865 0d0a 6164 6469 7469 6f6e  of the..addition
+00007730: 616c 2074 6572 6d73 2074 6861 7420 6170  al terms that ap
+00007740: 706c 7920 746f 2074 686f 7365 2066 696c  ply to those fil
+00007750: 6573 2c20 6f72 2061 206e 6f74 6963 6520  es, or a notice 
+00007760: 696e 6469 6361 7469 6e67 0d0a 7768 6572  indicating..wher
+00007770: 6520 746f 2066 696e 6420 7468 6520 6170  e to find the ap
+00007780: 706c 6963 6162 6c65 2074 6572 6d73 2e0d  plicable terms..
+00007790: 0a0d 0a20 2041 6464 6974 696f 6e61 6c20  ...  Additional 
+000077a0: 7465 726d 732c 2070 6572 6d69 7373 6976  terms, permissiv
+000077b0: 6520 6f72 206e 6f6e 2d70 6572 6d69 7373  e or non-permiss
+000077c0: 6976 652c 206d 6179 2062 6520 7374 6174  ive, may be stat
+000077d0: 6564 2069 6e20 7468 650d 0a66 6f72 6d20  ed in the..form 
+000077e0: 6f66 2061 2073 6570 6172 6174 656c 7920  of a separately 
+000077f0: 7772 6974 7465 6e20 6c69 6365 6e73 652c  written license,
+00007800: 206f 7220 7374 6174 6564 2061 7320 6578   or stated as ex
+00007810: 6365 7074 696f 6e73 3b0d 0a74 6865 2061  ceptions;..the a
+00007820: 626f 7665 2072 6571 7569 7265 6d65 6e74  bove requirement
+00007830: 7320 6170 706c 7920 6569 7468 6572 2077  s apply either w
+00007840: 6179 2e0d 0a0d 0a20 2038 2e20 5465 726d  ay.....  8. Term
+00007850: 696e 6174 696f 6e2e 0d0a 0d0a 2020 596f  ination.....  Yo
+00007860: 7520 6d61 7920 6e6f 7420 7072 6f70 6167  u may not propag
+00007870: 6174 6520 6f72 206d 6f64 6966 7920 6120  ate or modify a 
+00007880: 636f 7665 7265 6420 776f 726b 2065 7863  covered work exc
+00007890: 6570 7420 6173 2065 7870 7265 7373 6c79  ept as expressly
+000078a0: 0d0a 7072 6f76 6964 6564 2075 6e64 6572  ..provided under
+000078b0: 2074 6869 7320 4c69 6365 6e73 652e 2020   this License.  
+000078c0: 416e 7920 6174 7465 6d70 7420 6f74 6865  Any attempt othe
+000078d0: 7277 6973 6520 746f 2070 726f 7061 6761  rwise to propaga
+000078e0: 7465 206f 720d 0a6d 6f64 6966 7920 6974  te or..modify it
+000078f0: 2069 7320 766f 6964 2c20 616e 6420 7769   is void, and wi
+00007900: 6c6c 2061 7574 6f6d 6174 6963 616c 6c79  ll automatically
+00007910: 2074 6572 6d69 6e61 7465 2079 6f75 7220   terminate your 
+00007920: 7269 6768 7473 2075 6e64 6572 0d0a 7468  rights under..th
+00007930: 6973 204c 6963 656e 7365 2028 696e 636c  is License (incl
+00007940: 7564 696e 6720 616e 7920 7061 7465 6e74  uding any patent
+00007950: 206c 6963 656e 7365 7320 6772 616e 7465   licenses grante
+00007960: 6420 756e 6465 7220 7468 6520 7468 6972  d under the thir
+00007970: 640d 0a70 6172 6167 7261 7068 206f 6620  d..paragraph of 
+00007980: 7365 6374 696f 6e20 3131 292e 0d0a 0d0a  section 11).....
+00007990: 2020 486f 7765 7665 722c 2069 6620 796f    However, if yo
+000079a0: 7520 6365 6173 6520 616c 6c20 7669 6f6c  u cease all viol
+000079b0: 6174 696f 6e20 6f66 2074 6869 7320 4c69  ation of this Li
+000079c0: 6365 6e73 652c 2074 6865 6e20 796f 7572  cense, then your
+000079d0: 0d0a 6c69 6365 6e73 6520 6672 6f6d 2061  ..license from a
+000079e0: 2070 6172 7469 6375 6c61 7220 636f 7079   particular copy
+000079f0: 7269 6768 7420 686f 6c64 6572 2069 7320  right holder is 
+00007a00: 7265 696e 7374 6174 6564 2028 6129 0d0a  reinstated (a)..
+00007a10: 7072 6f76 6973 696f 6e61 6c6c 792c 2075  provisionally, u
+00007a20: 6e6c 6573 7320 616e 6420 756e 7469 6c20  nless and until 
+00007a30: 7468 6520 636f 7079 7269 6768 7420 686f  the copyright ho
+00007a40: 6c64 6572 2065 7870 6c69 6369 746c 7920  lder explicitly 
+00007a50: 616e 640d 0a66 696e 616c 6c79 2074 6572  and..finally ter
+00007a60: 6d69 6e61 7465 7320 796f 7572 206c 6963  minates your lic
+00007a70: 656e 7365 2c20 616e 6420 2862 2920 7065  ense, and (b) pe
+00007a80: 726d 616e 656e 746c 792c 2069 6620 7468  rmanently, if th
+00007a90: 6520 636f 7079 7269 6768 740d 0a68 6f6c  e copyright..hol
+00007aa0: 6465 7220 6661 696c 7320 746f 206e 6f74  der fails to not
+00007ab0: 6966 7920 796f 7520 6f66 2074 6865 2076  ify you of the v
+00007ac0: 696f 6c61 7469 6f6e 2062 7920 736f 6d65  iolation by some
+00007ad0: 2072 6561 736f 6e61 626c 6520 6d65 616e   reasonable mean
+00007ae0: 730d 0a70 7269 6f72 2074 6f20 3630 2064  s..prior to 60 d
+00007af0: 6179 7320 6166 7465 7220 7468 6520 6365  ays after the ce
+00007b00: 7373 6174 696f 6e2e 0d0a 0d0a 2020 4d6f  ssation.....  Mo
+00007b10: 7265 6f76 6572 2c20 796f 7572 206c 6963  reover, your lic
+00007b20: 656e 7365 2066 726f 6d20 6120 7061 7274  ense from a part
+00007b30: 6963 756c 6172 2063 6f70 7972 6967 6874  icular copyright
+00007b40: 2068 6f6c 6465 7220 6973 0d0a 7265 696e   holder is..rein
+00007b50: 7374 6174 6564 2070 6572 6d61 6e65 6e74  stated permanent
+00007b60: 6c79 2069 6620 7468 6520 636f 7079 7269  ly if the copyri
+00007b70: 6768 7420 686f 6c64 6572 206e 6f74 6966  ght holder notif
+00007b80: 6965 7320 796f 7520 6f66 2074 6865 0d0a  ies you of the..
+00007b90: 7669 6f6c 6174 696f 6e20 6279 2073 6f6d  violation by som
+00007ba0: 6520 7265 6173 6f6e 6162 6c65 206d 6561  e reasonable mea
+00007bb0: 6e73 2c20 7468 6973 2069 7320 7468 6520  ns, this is the 
+00007bc0: 6669 7273 7420 7469 6d65 2079 6f75 2068  first time you h
+00007bd0: 6176 650d 0a72 6563 6569 7665 6420 6e6f  ave..received no
+00007be0: 7469 6365 206f 6620 7669 6f6c 6174 696f  tice of violatio
+00007bf0: 6e20 6f66 2074 6869 7320 4c69 6365 6e73  n of this Licens
+00007c00: 6520 2866 6f72 2061 6e79 2077 6f72 6b29  e (for any work)
+00007c10: 2066 726f 6d20 7468 6174 0d0a 636f 7079   from that..copy
+00007c20: 7269 6768 7420 686f 6c64 6572 2c20 616e  right holder, an
+00007c30: 6420 796f 7520 6375 7265 2074 6865 2076  d you cure the v
+00007c40: 696f 6c61 7469 6f6e 2070 7269 6f72 2074  iolation prior t
+00007c50: 6f20 3330 2064 6179 7320 6166 7465 720d  o 30 days after.
+00007c60: 0a79 6f75 7220 7265 6365 6970 7420 6f66  .your receipt of
+00007c70: 2074 6865 206e 6f74 6963 652e 0d0a 0d0a   the notice.....
+00007c80: 2020 5465 726d 696e 6174 696f 6e20 6f66    Termination of
+00007c90: 2079 6f75 7220 7269 6768 7473 2075 6e64   your rights und
+00007ca0: 6572 2074 6869 7320 7365 6374 696f 6e20  er this section 
+00007cb0: 646f 6573 206e 6f74 2074 6572 6d69 6e61  does not termina
+00007cc0: 7465 2074 6865 0d0a 6c69 6365 6e73 6573  te the..licenses
+00007cd0: 206f 6620 7061 7274 6965 7320 7768 6f20   of parties who 
+00007ce0: 6861 7665 2072 6563 6569 7665 6420 636f  have received co
+00007cf0: 7069 6573 206f 7220 7269 6768 7473 2066  pies or rights f
+00007d00: 726f 6d20 796f 7520 756e 6465 720d 0a74  rom you under..t
+00007d10: 6869 7320 4c69 6365 6e73 652e 2020 4966  his License.  If
+00007d20: 2079 6f75 7220 7269 6768 7473 2068 6176   your rights hav
+00007d30: 6520 6265 656e 2074 6572 6d69 6e61 7465  e been terminate
+00007d40: 6420 616e 6420 6e6f 7420 7065 726d 616e  d and not perman
+00007d50: 656e 746c 790d 0a72 6569 6e73 7461 7465  ently..reinstate
+00007d60: 642c 2079 6f75 2064 6f20 6e6f 7420 7175  d, you do not qu
+00007d70: 616c 6966 7920 746f 2072 6563 6569 7665  alify to receive
+00007d80: 206e 6577 206c 6963 656e 7365 7320 666f   new licenses fo
+00007d90: 7220 7468 6520 7361 6d65 0d0a 6d61 7465  r the same..mate
+00007da0: 7269 616c 2075 6e64 6572 2073 6563 7469  rial under secti
+00007db0: 6f6e 2031 302e 0d0a 0d0a 2020 392e 2041  on 10.....  9. A
+00007dc0: 6363 6570 7461 6e63 6520 4e6f 7420 5265  cceptance Not Re
+00007dd0: 7175 6972 6564 2066 6f72 2048 6176 696e  quired for Havin
+00007de0: 6720 436f 7069 6573 2e0d 0a0d 0a20 2059  g Copies.....  Y
+00007df0: 6f75 2061 7265 206e 6f74 2072 6571 7569  ou are not requi
+00007e00: 7265 6420 746f 2061 6363 6570 7420 7468  red to accept th
+00007e10: 6973 204c 6963 656e 7365 2069 6e20 6f72  is License in or
+00007e20: 6465 7220 746f 2072 6563 6569 7665 206f  der to receive o
+00007e30: 720d 0a72 756e 2061 2063 6f70 7920 6f66  r..run a copy of
+00007e40: 2074 6865 2050 726f 6772 616d 2e20 2041   the Program.  A
+00007e50: 6e63 696c 6c61 7279 2070 726f 7061 6761  ncillary propaga
+00007e60: 7469 6f6e 206f 6620 6120 636f 7665 7265  tion of a covere
+00007e70: 6420 776f 726b 0d0a 6f63 6375 7272 696e  d work..occurrin
+00007e80: 6720 736f 6c65 6c79 2061 7320 6120 636f  g solely as a co
+00007e90: 6e73 6571 7565 6e63 6520 6f66 2075 7369  nsequence of usi
+00007ea0: 6e67 2070 6565 722d 746f 2d70 6565 7220  ng peer-to-peer 
+00007eb0: 7472 616e 736d 6973 7369 6f6e 0d0a 746f  transmission..to
+00007ec0: 2072 6563 6569 7665 2061 2063 6f70 7920   receive a copy 
+00007ed0: 6c69 6b65 7769 7365 2064 6f65 7320 6e6f  likewise does no
+00007ee0: 7420 7265 7175 6972 6520 6163 6365 7074  t require accept
+00007ef0: 616e 6365 2e20 2048 6f77 6576 6572 2c0d  ance.  However,.
+00007f00: 0a6e 6f74 6869 6e67 206f 7468 6572 2074  .nothing other t
+00007f10: 6861 6e20 7468 6973 204c 6963 656e 7365  han this License
+00007f20: 2067 7261 6e74 7320 796f 7520 7065 726d   grants you perm
+00007f30: 6973 7369 6f6e 2074 6f20 7072 6f70 6167  ission to propag
+00007f40: 6174 6520 6f72 0d0a 6d6f 6469 6679 2061  ate or..modify a
+00007f50: 6e79 2063 6f76 6572 6564 2077 6f72 6b2e  ny covered work.
+00007f60: 2020 5468 6573 6520 6163 7469 6f6e 7320    These actions 
+00007f70: 696e 6672 696e 6765 2063 6f70 7972 6967  infringe copyrig
+00007f80: 6874 2069 6620 796f 7520 646f 0d0a 6e6f  ht if you do..no
+00007f90: 7420 6163 6365 7074 2074 6869 7320 4c69  t accept this Li
+00007fa0: 6365 6e73 652e 2020 5468 6572 6566 6f72  cense.  Therefor
+00007fb0: 652c 2062 7920 6d6f 6469 6679 696e 6720  e, by modifying 
+00007fc0: 6f72 2070 726f 7061 6761 7469 6e67 2061  or propagating a
+00007fd0: 0d0a 636f 7665 7265 6420 776f 726b 2c20  ..covered work, 
+00007fe0: 796f 7520 696e 6469 6361 7465 2079 6f75  you indicate you
+00007ff0: 7220 6163 6365 7074 616e 6365 206f 6620  r acceptance of 
+00008000: 7468 6973 204c 6963 656e 7365 2074 6f20  this License to 
+00008010: 646f 2073 6f2e 0d0a 0d0a 2020 3130 2e20  do so.....  10. 
+00008020: 4175 746f 6d61 7469 6320 4c69 6365 6e73  Automatic Licens
+00008030: 696e 6720 6f66 2044 6f77 6e73 7472 6561  ing of Downstrea
+00008040: 6d20 5265 6369 7069 656e 7473 2e0d 0a0d  m Recipients....
+00008050: 0a20 2045 6163 6820 7469 6d65 2079 6f75  .  Each time you
+00008060: 2063 6f6e 7665 7920 6120 636f 7665 7265   convey a covere
+00008070: 6420 776f 726b 2c20 7468 6520 7265 6369  d work, the reci
+00008080: 7069 656e 7420 6175 746f 6d61 7469 6361  pient automatica
+00008090: 6c6c 790d 0a72 6563 6569 7665 7320 6120  lly..receives a 
+000080a0: 6c69 6365 6e73 6520 6672 6f6d 2074 6865  license from the
+000080b0: 206f 7269 6769 6e61 6c20 6c69 6365 6e73   original licens
+000080c0: 6f72 732c 2074 6f20 7275 6e2c 206d 6f64  ors, to run, mod
+000080d0: 6966 7920 616e 640d 0a70 726f 7061 6761  ify and..propaga
+000080e0: 7465 2074 6861 7420 776f 726b 2c20 7375  te that work, su
+000080f0: 626a 6563 7420 746f 2074 6869 7320 4c69  bject to this Li
+00008100: 6365 6e73 652e 2020 596f 7520 6172 6520  cense.  You are 
+00008110: 6e6f 7420 7265 7370 6f6e 7369 626c 650d  not responsible.
+00008120: 0a66 6f72 2065 6e66 6f72 6369 6e67 2063  .for enforcing c
+00008130: 6f6d 706c 6961 6e63 6520 6279 2074 6869  ompliance by thi
+00008140: 7264 2070 6172 7469 6573 2077 6974 6820  rd parties with 
+00008150: 7468 6973 204c 6963 656e 7365 2e0d 0a0d  this License....
+00008160: 0a20 2041 6e20 2265 6e74 6974 7920 7472  .  An "entity tr
+00008170: 616e 7361 6374 696f 6e22 2069 7320 6120  ansaction" is a 
+00008180: 7472 616e 7361 6374 696f 6e20 7472 616e  transaction tran
+00008190: 7366 6572 7269 6e67 2063 6f6e 7472 6f6c  sferring control
+000081a0: 206f 6620 616e 0d0a 6f72 6761 6e69 7a61   of an..organiza
+000081b0: 7469 6f6e 2c20 6f72 2073 7562 7374 616e  tion, or substan
+000081c0: 7469 616c 6c79 2061 6c6c 2061 7373 6574  tially all asset
+000081d0: 7320 6f66 206f 6e65 2c20 6f72 2073 7562  s of one, or sub
+000081e0: 6469 7669 6469 6e67 2061 6e0d 0a6f 7267  dividing an..org
+000081f0: 616e 697a 6174 696f 6e2c 206f 7220 6d65  anization, or me
+00008200: 7267 696e 6720 6f72 6761 6e69 7a61 7469  rging organizati
+00008210: 6f6e 732e 2020 4966 2070 726f 7061 6761  ons.  If propaga
+00008220: 7469 6f6e 206f 6620 6120 636f 7665 7265  tion of a covere
+00008230: 640d 0a77 6f72 6b20 7265 7375 6c74 7320  d..work results 
+00008240: 6672 6f6d 2061 6e20 656e 7469 7479 2074  from an entity t
+00008250: 7261 6e73 6163 7469 6f6e 2c20 6561 6368  ransaction, each
+00008260: 2070 6172 7479 2074 6f20 7468 6174 0d0a   party to that..
+00008270: 7472 616e 7361 6374 696f 6e20 7768 6f20  transaction who 
+00008280: 7265 6365 6976 6573 2061 2063 6f70 7920  receives a copy 
+00008290: 6f66 2074 6865 2077 6f72 6b20 616c 736f  of the work also
+000082a0: 2072 6563 6569 7665 7320 7768 6174 6576   receives whatev
+000082b0: 6572 0d0a 6c69 6365 6e73 6573 2074 6f20  er..licenses to 
+000082c0: 7468 6520 776f 726b 2074 6865 2070 6172  the work the par
+000082d0: 7479 2773 2070 7265 6465 6365 7373 6f72  ty's predecessor
+000082e0: 2069 6e20 696e 7465 7265 7374 2068 6164   in interest had
+000082f0: 206f 7220 636f 756c 640d 0a67 6976 6520   or could..give 
+00008300: 756e 6465 7220 7468 6520 7072 6576 696f  under the previo
+00008310: 7573 2070 6172 6167 7261 7068 2c20 706c  us paragraph, pl
+00008320: 7573 2061 2072 6967 6874 2074 6f20 706f  us a right to po
+00008330: 7373 6573 7369 6f6e 206f 6620 7468 650d  ssession of the.
+00008340: 0a43 6f72 7265 7370 6f6e 6469 6e67 2053  .Corresponding S
+00008350: 6f75 7263 6520 6f66 2074 6865 2077 6f72  ource of the wor
+00008360: 6b20 6672 6f6d 2074 6865 2070 7265 6465  k from the prede
+00008370: 6365 7373 6f72 2069 6e20 696e 7465 7265  cessor in intere
+00008380: 7374 2c20 6966 0d0a 7468 6520 7072 6564  st, if..the pred
+00008390: 6563 6573 736f 7220 6861 7320 6974 206f  ecessor has it o
+000083a0: 7220 6361 6e20 6765 7420 6974 2077 6974  r can get it wit
+000083b0: 6820 7265 6173 6f6e 6162 6c65 2065 6666  h reasonable eff
+000083c0: 6f72 7473 2e0d 0a0d 0a20 2059 6f75 206d  orts.....  You m
+000083d0: 6179 206e 6f74 2069 6d70 6f73 6520 616e  ay not impose an
+000083e0: 7920 6675 7274 6865 7220 7265 7374 7269  y further restri
+000083f0: 6374 696f 6e73 206f 6e20 7468 6520 6578  ctions on the ex
+00008400: 6572 6369 7365 206f 6620 7468 650d 0a72  ercise of the..r
+00008410: 6967 6874 7320 6772 616e 7465 6420 6f72  ights granted or
+00008420: 2061 6666 6972 6d65 6420 756e 6465 7220   affirmed under 
+00008430: 7468 6973 204c 6963 656e 7365 2e20 2046  this License.  F
+00008440: 6f72 2065 7861 6d70 6c65 2c20 796f 7520  or example, you 
+00008450: 6d61 790d 0a6e 6f74 2069 6d70 6f73 6520  may..not impose 
+00008460: 6120 6c69 6365 6e73 6520 6665 652c 2072  a license fee, r
+00008470: 6f79 616c 7479 2c20 6f72 206f 7468 6572  oyalty, or other
+00008480: 2063 6861 7267 6520 666f 7220 6578 6572   charge for exer
+00008490: 6369 7365 206f 660d 0a72 6967 6874 7320  cise of..rights 
+000084a0: 6772 616e 7465 6420 756e 6465 7220 7468  granted under th
+000084b0: 6973 204c 6963 656e 7365 2c20 616e 6420  is License, and 
+000084c0: 796f 7520 6d61 7920 6e6f 7420 696e 6974  you may not init
+000084d0: 6961 7465 206c 6974 6967 6174 696f 6e0d  iate litigation.
+000084e0: 0a28 696e 636c 7564 696e 6720 6120 6372  .(including a cr
+000084f0: 6f73 732d 636c 6169 6d20 6f72 2063 6f75  oss-claim or cou
+00008500: 6e74 6572 636c 6169 6d20 696e 2061 206c  nterclaim in a l
+00008510: 6177 7375 6974 2920 616c 6c65 6769 6e67  awsuit) alleging
+00008520: 2074 6861 740d 0a61 6e79 2070 6174 656e   that..any paten
+00008530: 7420 636c 6169 6d20 6973 2069 6e66 7269  t claim is infri
+00008540: 6e67 6564 2062 7920 6d61 6b69 6e67 2c20  nged by making, 
+00008550: 7573 696e 672c 2073 656c 6c69 6e67 2c20  using, selling, 
+00008560: 6f66 6665 7269 6e67 2066 6f72 0d0a 7361  offering for..sa
+00008570: 6c65 2c20 6f72 2069 6d70 6f72 7469 6e67  le, or importing
+00008580: 2074 6865 2050 726f 6772 616d 206f 7220   the Program or 
+00008590: 616e 7920 706f 7274 696f 6e20 6f66 2069  any portion of i
+000085a0: 742e 0d0a 0d0a 2020 3131 2e20 5061 7465  t.....  11. Pate
+000085b0: 6e74 732e 0d0a 0d0a 2020 4120 2263 6f6e  nts.....  A "con
+000085c0: 7472 6962 7574 6f72 2220 6973 2061 2063  tributor" is a c
+000085d0: 6f70 7972 6967 6874 2068 6f6c 6465 7220  opyright holder 
+000085e0: 7768 6f20 6175 7468 6f72 697a 6573 2075  who authorizes u
+000085f0: 7365 2075 6e64 6572 2074 6869 730d 0a4c  se under this..L
+00008600: 6963 656e 7365 206f 6620 7468 6520 5072  icense of the Pr
+00008610: 6f67 7261 6d20 6f72 2061 2077 6f72 6b20  ogram or a work 
+00008620: 6f6e 2077 6869 6368 2074 6865 2050 726f  on which the Pro
+00008630: 6772 616d 2069 7320 6261 7365 642e 2020  gram is based.  
+00008640: 5468 650d 0a77 6f72 6b20 7468 7573 206c  The..work thus l
+00008650: 6963 656e 7365 6420 6973 2063 616c 6c65  icensed is calle
+00008660: 6420 7468 6520 636f 6e74 7269 6275 746f  d the contributo
+00008670: 7227 7320 2263 6f6e 7472 6962 7574 6f72  r's "contributor
+00008680: 2076 6572 7369 6f6e 222e 0d0a 0d0a 2020   version".....  
+00008690: 4120 636f 6e74 7269 6275 746f 7227 7320  A contributor's 
+000086a0: 2265 7373 656e 7469 616c 2070 6174 656e  "essential paten
+000086b0: 7420 636c 6169 6d73 2220 6172 6520 616c  t claims" are al
+000086c0: 6c20 7061 7465 6e74 2063 6c61 696d 730d  l patent claims.
+000086d0: 0a6f 776e 6564 206f 7220 636f 6e74 726f  .owned or contro
+000086e0: 6c6c 6564 2062 7920 7468 6520 636f 6e74  lled by the cont
+000086f0: 7269 6275 746f 722c 2077 6865 7468 6572  ributor, whether
+00008700: 2061 6c72 6561 6479 2061 6371 7569 7265   already acquire
+00008710: 6420 6f72 0d0a 6865 7265 6166 7465 7220  d or..hereafter 
+00008720: 6163 7175 6972 6564 2c20 7468 6174 2077  acquired, that w
+00008730: 6f75 6c64 2062 6520 696e 6672 696e 6765  ould be infringe
+00008740: 6420 6279 2073 6f6d 6520 6d61 6e6e 6572  d by some manner
+00008750: 2c20 7065 726d 6974 7465 640d 0a62 7920  , permitted..by 
+00008760: 7468 6973 204c 6963 656e 7365 2c20 6f66  this License, of
+00008770: 206d 616b 696e 672c 2075 7369 6e67 2c20   making, using, 
+00008780: 6f72 2073 656c 6c69 6e67 2069 7473 2063  or selling its c
+00008790: 6f6e 7472 6962 7574 6f72 2076 6572 7369  ontributor versi
+000087a0: 6f6e 2c0d 0a62 7574 2064 6f20 6e6f 7420  on,..but do not 
+000087b0: 696e 636c 7564 6520 636c 6169 6d73 2074  include claims t
+000087c0: 6861 7420 776f 756c 6420 6265 2069 6e66  hat would be inf
+000087d0: 7269 6e67 6564 206f 6e6c 7920 6173 2061  ringed only as a
+000087e0: 0d0a 636f 6e73 6571 7565 6e63 6520 6f66  ..consequence of
+000087f0: 2066 7572 7468 6572 206d 6f64 6966 6963   further modific
+00008800: 6174 696f 6e20 6f66 2074 6865 2063 6f6e  ation of the con
+00008810: 7472 6962 7574 6f72 2076 6572 7369 6f6e  tributor version
+00008820: 2e20 2046 6f72 0d0a 7075 7270 6f73 6573  .  For..purposes
+00008830: 206f 6620 7468 6973 2064 6566 696e 6974   of this definit
+00008840: 696f 6e2c 2022 636f 6e74 726f 6c22 2069  ion, "control" i
+00008850: 6e63 6c75 6465 7320 7468 6520 7269 6768  ncludes the righ
+00008860: 7420 746f 2067 7261 6e74 0d0a 7061 7465  t to grant..pate
+00008870: 6e74 2073 7562 6c69 6365 6e73 6573 2069  nt sublicenses i
+00008880: 6e20 6120 6d61 6e6e 6572 2063 6f6e 7369  n a manner consi
+00008890: 7374 656e 7420 7769 7468 2074 6865 2072  stent with the r
+000088a0: 6571 7569 7265 6d65 6e74 7320 6f66 0d0a  equirements of..
+000088b0: 7468 6973 204c 6963 656e 7365 2e0d 0a0d  this License....
+000088c0: 0a20 2045 6163 6820 636f 6e74 7269 6275  .  Each contribu
+000088d0: 746f 7220 6772 616e 7473 2079 6f75 2061  tor grants you a
+000088e0: 206e 6f6e 2d65 7863 6c75 7369 7665 2c20   non-exclusive, 
+000088f0: 776f 726c 6477 6964 652c 2072 6f79 616c  worldwide, royal
+00008900: 7479 2d66 7265 650d 0a70 6174 656e 7420  ty-free..patent 
+00008910: 6c69 6365 6e73 6520 756e 6465 7220 7468  license under th
+00008920: 6520 636f 6e74 7269 6275 746f 7227 7320  e contributor's 
+00008930: 6573 7365 6e74 6961 6c20 7061 7465 6e74  essential patent
+00008940: 2063 6c61 696d 732c 2074 6f0d 0a6d 616b   claims, to..mak
+00008950: 652c 2075 7365 2c20 7365 6c6c 2c20 6f66  e, use, sell, of
+00008960: 6665 7220 666f 7220 7361 6c65 2c20 696d  fer for sale, im
+00008970: 706f 7274 2061 6e64 206f 7468 6572 7769  port and otherwi
+00008980: 7365 2072 756e 2c20 6d6f 6469 6679 2061  se run, modify a
+00008990: 6e64 0d0a 7072 6f70 6167 6174 6520 7468  nd..propagate th
+000089a0: 6520 636f 6e74 656e 7473 206f 6620 6974  e contents of it
+000089b0: 7320 636f 6e74 7269 6275 746f 7220 7665  s contributor ve
+000089c0: 7273 696f 6e2e 0d0a 0d0a 2020 496e 2074  rsion.....  In t
+000089d0: 6865 2066 6f6c 6c6f 7769 6e67 2074 6872  he following thr
+000089e0: 6565 2070 6172 6167 7261 7068 732c 2061  ee paragraphs, a
+000089f0: 2022 7061 7465 6e74 206c 6963 656e 7365   "patent license
+00008a00: 2220 6973 2061 6e79 2065 7870 7265 7373  " is any express
+00008a10: 0d0a 6167 7265 656d 656e 7420 6f72 2063  ..agreement or c
+00008a20: 6f6d 6d69 746d 656e 742c 2068 6f77 6576  ommitment, howev
+00008a30: 6572 2064 656e 6f6d 696e 6174 6564 2c20  er denominated, 
+00008a40: 6e6f 7420 746f 2065 6e66 6f72 6365 2061  not to enforce a
+00008a50: 2070 6174 656e 740d 0a28 7375 6368 2061   patent..(such a
+00008a60: 7320 616e 2065 7870 7265 7373 2070 6572  s an express per
+00008a70: 6d69 7373 696f 6e20 746f 2070 7261 6374  mission to pract
+00008a80: 6963 6520 6120 7061 7465 6e74 206f 7220  ice a patent or 
+00008a90: 636f 7665 6e61 6e74 206e 6f74 2074 6f0d  covenant not to.
+00008aa0: 0a73 7565 2066 6f72 2070 6174 656e 7420  .sue for patent 
+00008ab0: 696e 6672 696e 6765 6d65 6e74 292e 2020  infringement).  
+00008ac0: 546f 2022 6772 616e 7422 2073 7563 6820  To "grant" such 
+00008ad0: 6120 7061 7465 6e74 206c 6963 656e 7365  a patent license
+00008ae0: 2074 6f20 610d 0a70 6172 7479 206d 6561   to a..party mea
+00008af0: 6e73 2074 6f20 6d61 6b65 2073 7563 6820  ns to make such 
+00008b00: 616e 2061 6772 6565 6d65 6e74 206f 7220  an agreement or 
+00008b10: 636f 6d6d 6974 6d65 6e74 206e 6f74 2074  commitment not t
+00008b20: 6f20 656e 666f 7263 6520 610d 0a70 6174  o enforce a..pat
+00008b30: 656e 7420 6167 6169 6e73 7420 7468 6520  ent against the 
+00008b40: 7061 7274 792e 0d0a 0d0a 2020 4966 2079  party.....  If y
+00008b50: 6f75 2063 6f6e 7665 7920 6120 636f 7665  ou convey a cove
+00008b60: 7265 6420 776f 726b 2c20 6b6e 6f77 696e  red work, knowin
+00008b70: 676c 7920 7265 6c79 696e 6720 6f6e 2061  gly relying on a
+00008b80: 2070 6174 656e 7420 6c69 6365 6e73 652c   patent license,
+00008b90: 0d0a 616e 6420 7468 6520 436f 7272 6573  ..and the Corres
+00008ba0: 706f 6e64 696e 6720 536f 7572 6365 206f  ponding Source o
+00008bb0: 6620 7468 6520 776f 726b 2069 7320 6e6f  f the work is no
+00008bc0: 7420 6176 6169 6c61 626c 6520 666f 7220  t available for 
+00008bd0: 616e 796f 6e65 0d0a 746f 2063 6f70 792c  anyone..to copy,
+00008be0: 2066 7265 6520 6f66 2063 6861 7267 6520   free of charge 
+00008bf0: 616e 6420 756e 6465 7220 7468 6520 7465  and under the te
+00008c00: 726d 7320 6f66 2074 6869 7320 4c69 6365  rms of this Lice
+00008c10: 6e73 652c 2074 6872 6f75 6768 2061 0d0a  nse, through a..
+00008c20: 7075 626c 6963 6c79 2061 7661 696c 6162  publicly availab
+00008c30: 6c65 206e 6574 776f 726b 2073 6572 7665  le network serve
+00008c40: 7220 6f72 206f 7468 6572 2072 6561 6469  r or other readi
+00008c50: 6c79 2061 6363 6573 7369 626c 6520 6d65  ly accessible me
+00008c60: 616e 732c 0d0a 7468 656e 2079 6f75 206d  ans,..then you m
+00008c70: 7573 7420 6569 7468 6572 2028 3129 2063  ust either (1) c
+00008c80: 6175 7365 2074 6865 2043 6f72 7265 7370  ause the Corresp
+00008c90: 6f6e 6469 6e67 2053 6f75 7263 6520 746f  onding Source to
+00008ca0: 2062 6520 736f 0d0a 6176 6169 6c61 626c   be so..availabl
+00008cb0: 652c 206f 7220 2832 2920 6172 7261 6e67  e, or (2) arrang
+00008cc0: 6520 746f 2064 6570 7269 7665 2079 6f75  e to deprive you
+00008cd0: 7273 656c 6620 6f66 2074 6865 2062 656e  rself of the ben
+00008ce0: 6566 6974 206f 6620 7468 650d 0a70 6174  efit of the..pat
+00008cf0: 656e 7420 6c69 6365 6e73 6520 666f 7220  ent license for 
+00008d00: 7468 6973 2070 6172 7469 6375 6c61 7220  this particular 
+00008d10: 776f 726b 2c20 6f72 2028 3329 2061 7272  work, or (3) arr
+00008d20: 616e 6765 2c20 696e 2061 206d 616e 6e65  ange, in a manne
+00008d30: 720d 0a63 6f6e 7369 7374 656e 7420 7769  r..consistent wi
+00008d40: 7468 2074 6865 2072 6571 7569 7265 6d65  th the requireme
+00008d50: 6e74 7320 6f66 2074 6869 7320 4c69 6365  nts of this Lice
+00008d60: 6e73 652c 2074 6f20 6578 7465 6e64 2074  nse, to extend t
+00008d70: 6865 2070 6174 656e 740d 0a6c 6963 656e  he patent..licen
+00008d80: 7365 2074 6f20 646f 776e 7374 7265 616d  se to downstream
+00008d90: 2072 6563 6970 6965 6e74 732e 2020 224b   recipients.  "K
+00008da0: 6e6f 7769 6e67 6c79 2072 656c 7969 6e67  nowingly relying
+00008db0: 2220 6d65 616e 7320 796f 7520 6861 7665  " means you have
+00008dc0: 0d0a 6163 7475 616c 206b 6e6f 776c 6564  ..actual knowled
+00008dd0: 6765 2074 6861 742c 2062 7574 2066 6f72  ge that, but for
+00008de0: 2074 6865 2070 6174 656e 7420 6c69 6365   the patent lice
+00008df0: 6e73 652c 2079 6f75 7220 636f 6e76 6579  nse, your convey
+00008e00: 696e 6720 7468 650d 0a63 6f76 6572 6564  ing the..covered
+00008e10: 2077 6f72 6b20 696e 2061 2063 6f75 6e74   work in a count
+00008e20: 7279 2c20 6f72 2079 6f75 7220 7265 6369  ry, or your reci
+00008e30: 7069 656e 7427 7320 7573 6520 6f66 2074  pient's use of t
+00008e40: 6865 2063 6f76 6572 6564 2077 6f72 6b0d  he covered work.
+00008e50: 0a69 6e20 6120 636f 756e 7472 792c 2077  .in a country, w
+00008e60: 6f75 6c64 2069 6e66 7269 6e67 6520 6f6e  ould infringe on
+00008e70: 6520 6f72 206d 6f72 6520 6964 656e 7469  e or more identi
+00008e80: 6669 6162 6c65 2070 6174 656e 7473 2069  fiable patents i
+00008e90: 6e20 7468 6174 0d0a 636f 756e 7472 7920  n that..country 
+00008ea0: 7468 6174 2079 6f75 2068 6176 6520 7265  that you have re
+00008eb0: 6173 6f6e 2074 6f20 6265 6c69 6576 6520  ason to believe 
+00008ec0: 6172 6520 7661 6c69 642e 0d0a 0d0a 2020  are valid.....  
+00008ed0: 4966 2c20 7075 7273 7561 6e74 2074 6f20  If, pursuant to 
+00008ee0: 6f72 2069 6e20 636f 6e6e 6563 7469 6f6e  or in connection
+00008ef0: 2077 6974 6820 6120 7369 6e67 6c65 2074   with a single t
+00008f00: 7261 6e73 6163 7469 6f6e 206f 720d 0a61  ransaction or..a
+00008f10: 7272 616e 6765 6d65 6e74 2c20 796f 7520  rrangement, you 
+00008f20: 636f 6e76 6579 2c20 6f72 2070 726f 7061  convey, or propa
+00008f30: 6761 7465 2062 7920 7072 6f63 7572 696e  gate by procurin
+00008f40: 6720 636f 6e76 6579 616e 6365 206f 662c  g conveyance of,
+00008f50: 2061 0d0a 636f 7665 7265 6420 776f 726b   a..covered work
+00008f60: 2c20 616e 6420 6772 616e 7420 6120 7061  , and grant a pa
+00008f70: 7465 6e74 206c 6963 656e 7365 2074 6f20  tent license to 
+00008f80: 736f 6d65 206f 6620 7468 6520 7061 7274  some of the part
+00008f90: 6965 730d 0a72 6563 6569 7669 6e67 2074  ies..receiving t
+00008fa0: 6865 2063 6f76 6572 6564 2077 6f72 6b20  he covered work 
+00008fb0: 6175 7468 6f72 697a 696e 6720 7468 656d  authorizing them
+00008fc0: 2074 6f20 7573 652c 2070 726f 7061 6761   to use, propaga
+00008fd0: 7465 2c20 6d6f 6469 6679 0d0a 6f72 2063  te, modify..or c
+00008fe0: 6f6e 7665 7920 6120 7370 6563 6966 6963  onvey a specific
+00008ff0: 2063 6f70 7920 6f66 2074 6865 2063 6f76   copy of the cov
+00009000: 6572 6564 2077 6f72 6b2c 2074 6865 6e20  ered work, then 
+00009010: 7468 6520 7061 7465 6e74 206c 6963 656e  the patent licen
+00009020: 7365 0d0a 796f 7520 6772 616e 7420 6973  se..you grant is
+00009030: 2061 7574 6f6d 6174 6963 616c 6c79 2065   automatically e
+00009040: 7874 656e 6465 6420 746f 2061 6c6c 2072  xtended to all r
+00009050: 6563 6970 6965 6e74 7320 6f66 2074 6865  ecipients of the
+00009060: 2063 6f76 6572 6564 0d0a 776f 726b 2061   covered..work a
+00009070: 6e64 2077 6f72 6b73 2062 6173 6564 206f  nd works based o
+00009080: 6e20 6974 2e0d 0a0d 0a20 2041 2070 6174  n it.....  A pat
+00009090: 656e 7420 6c69 6365 6e73 6520 6973 2022  ent license is "
+000090a0: 6469 7363 7269 6d69 6e61 746f 7279 2220  discriminatory" 
+000090b0: 6966 2069 7420 646f 6573 206e 6f74 2069  if it does not i
+000090c0: 6e63 6c75 6465 2077 6974 6869 6e0d 0a74  nclude within..t
+000090d0: 6865 2073 636f 7065 206f 6620 6974 7320  he scope of its 
+000090e0: 636f 7665 7261 6765 2c20 7072 6f68 6962  coverage, prohib
+000090f0: 6974 7320 7468 6520 6578 6572 6369 7365  its the exercise
+00009100: 206f 662c 206f 7220 6973 0d0a 636f 6e64   of, or is..cond
+00009110: 6974 696f 6e65 6420 6f6e 2074 6865 206e  itioned on the n
+00009120: 6f6e 2d65 7865 7263 6973 6520 6f66 206f  on-exercise of o
+00009130: 6e65 206f 7220 6d6f 7265 206f 6620 7468  ne or more of th
+00009140: 6520 7269 6768 7473 2074 6861 7420 6172  e rights that ar
+00009150: 650d 0a73 7065 6369 6669 6361 6c6c 7920  e..specifically 
+00009160: 6772 616e 7465 6420 756e 6465 7220 7468  granted under th
+00009170: 6973 204c 6963 656e 7365 2e20 2059 6f75  is License.  You
+00009180: 206d 6179 206e 6f74 2063 6f6e 7665 7920   may not convey 
+00009190: 6120 636f 7665 7265 640d 0a77 6f72 6b20  a covered..work 
+000091a0: 6966 2079 6f75 2061 7265 2061 2070 6172  if you are a par
+000091b0: 7479 2074 6f20 616e 2061 7272 616e 6765  ty to an arrange
+000091c0: 6d65 6e74 2077 6974 6820 6120 7468 6972  ment with a thir
+000091d0: 6420 7061 7274 7920 7468 6174 2069 730d  d party that is.
+000091e0: 0a69 6e20 7468 6520 6275 7369 6e65 7373  .in the business
+000091f0: 206f 6620 6469 7374 7269 6275 7469 6e67   of distributing
+00009200: 2073 6f66 7477 6172 652c 2075 6e64 6572   software, under
+00009210: 2077 6869 6368 2079 6f75 206d 616b 6520   which you make 
+00009220: 7061 796d 656e 740d 0a74 6f20 7468 6520  payment..to the 
+00009230: 7468 6972 6420 7061 7274 7920 6261 7365  third party base
+00009240: 6420 6f6e 2074 6865 2065 7874 656e 7420  d on the extent 
+00009250: 6f66 2079 6f75 7220 6163 7469 7669 7479  of your activity
+00009260: 206f 6620 636f 6e76 6579 696e 670d 0a74   of conveying..t
+00009270: 6865 2077 6f72 6b2c 2061 6e64 2075 6e64  he work, and und
+00009280: 6572 2077 6869 6368 2074 6865 2074 6869  er which the thi
+00009290: 7264 2070 6172 7479 2067 7261 6e74 732c  rd party grants,
+000092a0: 2074 6f20 616e 7920 6f66 2074 6865 0d0a   to any of the..
+000092b0: 7061 7274 6965 7320 7768 6f20 776f 756c  parties who woul
+000092c0: 6420 7265 6365 6976 6520 7468 6520 636f  d receive the co
+000092d0: 7665 7265 6420 776f 726b 2066 726f 6d20  vered work from 
+000092e0: 796f 752c 2061 2064 6973 6372 696d 696e  you, a discrimin
+000092f0: 6174 6f72 790d 0a70 6174 656e 7420 6c69  atory..patent li
+00009300: 6365 6e73 6520 2861 2920 696e 2063 6f6e  cense (a) in con
+00009310: 6e65 6374 696f 6e20 7769 7468 2063 6f70  nection with cop
+00009320: 6965 7320 6f66 2074 6865 2063 6f76 6572  ies of the cover
+00009330: 6564 2077 6f72 6b0d 0a63 6f6e 7665 7965  ed work..conveye
+00009340: 6420 6279 2079 6f75 2028 6f72 2063 6f70  d by you (or cop
+00009350: 6965 7320 6d61 6465 2066 726f 6d20 7468  ies made from th
+00009360: 6f73 6520 636f 7069 6573 292c 206f 7220  ose copies), or 
+00009370: 2862 2920 7072 696d 6172 696c 790d 0a66  (b) primarily..f
+00009380: 6f72 2061 6e64 2069 6e20 636f 6e6e 6563  or and in connec
+00009390: 7469 6f6e 2077 6974 6820 7370 6563 6966  tion with specif
+000093a0: 6963 2070 726f 6475 6374 7320 6f72 2063  ic products or c
+000093b0: 6f6d 7069 6c61 7469 6f6e 7320 7468 6174  ompilations that
+000093c0: 0d0a 636f 6e74 6169 6e20 7468 6520 636f  ..contain the co
+000093d0: 7665 7265 6420 776f 726b 2c20 756e 6c65  vered work, unle
+000093e0: 7373 2079 6f75 2065 6e74 6572 6564 2069  ss you entered i
+000093f0: 6e74 6f20 7468 6174 2061 7272 616e 6765  nto that arrange
+00009400: 6d65 6e74 2c0d 0a6f 7220 7468 6174 2070  ment,..or that p
+00009410: 6174 656e 7420 6c69 6365 6e73 6520 7761  atent license wa
+00009420: 7320 6772 616e 7465 642c 2070 7269 6f72  s granted, prior
+00009430: 2074 6f20 3238 204d 6172 6368 2032 3030   to 28 March 200
+00009440: 372e 0d0a 0d0a 2020 4e6f 7468 696e 6720  7.....  Nothing 
+00009450: 696e 2074 6869 7320 4c69 6365 6e73 6520  in this License 
+00009460: 7368 616c 6c20 6265 2063 6f6e 7374 7275  shall be constru
+00009470: 6564 2061 7320 6578 636c 7564 696e 6720  ed as excluding 
+00009480: 6f72 206c 696d 6974 696e 670d 0a61 6e79  or limiting..any
+00009490: 2069 6d70 6c69 6564 206c 6963 656e 7365   implied license
+000094a0: 206f 7220 6f74 6865 7220 6465 6665 6e73   or other defens
+000094b0: 6573 2074 6f20 696e 6672 696e 6765 6d65  es to infringeme
+000094c0: 6e74 2074 6861 7420 6d61 790d 0a6f 7468  nt that may..oth
+000094d0: 6572 7769 7365 2062 6520 6176 6169 6c61  erwise be availa
+000094e0: 626c 6520 746f 2079 6f75 2075 6e64 6572  ble to you under
+000094f0: 2061 7070 6c69 6361 626c 6520 7061 7465   applicable pate
+00009500: 6e74 206c 6177 2e0d 0a0d 0a20 2031 322e  nt law.....  12.
+00009510: 204e 6f20 5375 7272 656e 6465 7220 6f66   No Surrender of
+00009520: 204f 7468 6572 7327 2046 7265 6564 6f6d   Others' Freedom
+00009530: 2e0d 0a0d 0a20 2049 6620 636f 6e64 6974  .....  If condit
+00009540: 696f 6e73 2061 7265 2069 6d70 6f73 6564  ions are imposed
+00009550: 206f 6e20 796f 7520 2877 6865 7468 6572   on you (whether
+00009560: 2062 7920 636f 7572 7420 6f72 6465 722c   by court order,
+00009570: 2061 6772 6565 6d65 6e74 206f 720d 0a6f   agreement or..o
+00009580: 7468 6572 7769 7365 2920 7468 6174 2063  therwise) that c
+00009590: 6f6e 7472 6164 6963 7420 7468 6520 636f  ontradict the co
+000095a0: 6e64 6974 696f 6e73 206f 6620 7468 6973  nditions of this
+000095b0: 204c 6963 656e 7365 2c20 7468 6579 2064   License, they d
+000095c0: 6f20 6e6f 740d 0a65 7863 7573 6520 796f  o not..excuse yo
+000095d0: 7520 6672 6f6d 2074 6865 2063 6f6e 6469  u from the condi
+000095e0: 7469 6f6e 7320 6f66 2074 6869 7320 4c69  tions of this Li
+000095f0: 6365 6e73 652e 2020 4966 2079 6f75 2063  cense.  If you c
+00009600: 616e 6e6f 7420 636f 6e76 6579 2061 0d0a  annot convey a..
+00009610: 636f 7665 7265 6420 776f 726b 2073 6f20  covered work so 
+00009620: 6173 2074 6f20 7361 7469 7366 7920 7369  as to satisfy si
+00009630: 6d75 6c74 616e 656f 7573 6c79 2079 6f75  multaneously you
+00009640: 7220 6f62 6c69 6761 7469 6f6e 7320 756e  r obligations un
+00009650: 6465 7220 7468 6973 0d0a 4c69 6365 6e73  der this..Licens
+00009660: 6520 616e 6420 616e 7920 6f74 6865 7220  e and any other 
+00009670: 7065 7274 696e 656e 7420 6f62 6c69 6761  pertinent obliga
+00009680: 7469 6f6e 732c 2074 6865 6e20 6173 2061  tions, then as a
+00009690: 2063 6f6e 7365 7175 656e 6365 2079 6f75   consequence you
+000096a0: 206d 6179 0d0a 6e6f 7420 636f 6e76 6579   may..not convey
+000096b0: 2069 7420 6174 2061 6c6c 2e20 2046 6f72   it at all.  For
+000096c0: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
+000096d0: 2061 6772 6565 2074 6f20 7465 726d 7320   agree to terms 
+000096e0: 7468 6174 206f 626c 6967 6174 6520 796f  that obligate yo
+000096f0: 750d 0a74 6f20 636f 6c6c 6563 7420 6120  u..to collect a 
+00009700: 726f 7961 6c74 7920 666f 7220 6675 7274  royalty for furt
+00009710: 6865 7220 636f 6e76 6579 696e 6720 6672  her conveying fr
+00009720: 6f6d 2074 686f 7365 2074 6f20 7768 6f6d  om those to whom
+00009730: 2079 6f75 2063 6f6e 7665 790d 0a74 6865   you convey..the
+00009740: 2050 726f 6772 616d 2c20 7468 6520 6f6e   Program, the on
+00009750: 6c79 2077 6179 2079 6f75 2063 6f75 6c64  ly way you could
+00009760: 2073 6174 6973 6679 2062 6f74 6820 7468   satisfy both th
+00009770: 6f73 6520 7465 726d 7320 616e 6420 7468  ose terms and th
+00009780: 6973 0d0a 4c69 6365 6e73 6520 776f 756c  is..License woul
+00009790: 6420 6265 2074 6f20 7265 6672 6169 6e20  d be to refrain 
+000097a0: 656e 7469 7265 6c79 2066 726f 6d20 636f  entirely from co
+000097b0: 6e76 6579 696e 6720 7468 6520 5072 6f67  nveying the Prog
+000097c0: 7261 6d2e 0d0a 0d0a 2020 3133 2e20 5573  ram.....  13. Us
+000097d0: 6520 7769 7468 2074 6865 2047 4e55 2041  e with the GNU A
+000097e0: 6666 6572 6f20 4765 6e65 7261 6c20 5075  ffero General Pu
+000097f0: 626c 6963 204c 6963 656e 7365 2e0d 0a0d  blic License....
+00009800: 0a20 204e 6f74 7769 7468 7374 616e 6469  .  Notwithstandi
+00009810: 6e67 2061 6e79 206f 7468 6572 2070 726f  ng any other pro
+00009820: 7669 7369 6f6e 206f 6620 7468 6973 204c  vision of this L
+00009830: 6963 656e 7365 2c20 796f 7520 6861 7665  icense, you have
+00009840: 0d0a 7065 726d 6973 7369 6f6e 2074 6f20  ..permission to 
+00009850: 6c69 6e6b 206f 7220 636f 6d62 696e 6520  link or combine 
+00009860: 616e 7920 636f 7665 7265 6420 776f 726b  any covered work
+00009870: 2077 6974 6820 6120 776f 726b 206c 6963   with a work lic
+00009880: 656e 7365 640d 0a75 6e64 6572 2076 6572  ensed..under ver
+00009890: 7369 6f6e 2033 206f 6620 7468 6520 474e  sion 3 of the GN
+000098a0: 5520 4166 6665 726f 2047 656e 6572 616c  U Affero General
+000098b0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000098c0: 696e 746f 2061 2073 696e 676c 650d 0a63  into a single..c
+000098d0: 6f6d 6269 6e65 6420 776f 726b 2c20 616e  ombined work, an
+000098e0: 6420 746f 2063 6f6e 7665 7920 7468 6520  d to convey the 
+000098f0: 7265 7375 6c74 696e 6720 776f 726b 2e20  resulting work. 
+00009900: 2054 6865 2074 6572 6d73 206f 6620 7468   The terms of th
+00009910: 6973 0d0a 4c69 6365 6e73 6520 7769 6c6c  is..License will
+00009920: 2063 6f6e 7469 6e75 6520 746f 2061 7070   continue to app
+00009930: 6c79 2074 6f20 7468 6520 7061 7274 2077  ly to the part w
+00009940: 6869 6368 2069 7320 7468 6520 636f 7665  hich is the cove
+00009950: 7265 6420 776f 726b 2c0d 0a62 7574 2074  red work,..but t
+00009960: 6865 2073 7065 6369 616c 2072 6571 7569  he special requi
+00009970: 7265 6d65 6e74 7320 6f66 2074 6865 2047  rements of the G
+00009980: 4e55 2041 6666 6572 6f20 4765 6e65 7261  NU Affero Genera
+00009990: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+000099a0: 2c0d 0a73 6563 7469 6f6e 2031 332c 2063  ,..section 13, c
+000099b0: 6f6e 6365 726e 696e 6720 696e 7465 7261  oncerning intera
+000099c0: 6374 696f 6e20 7468 726f 7567 6820 6120  ction through a 
+000099d0: 6e65 7477 6f72 6b20 7769 6c6c 2061 7070  network will app
+000099e0: 6c79 2074 6f20 7468 650d 0a63 6f6d 6269  ly to the..combi
+000099f0: 6e61 7469 6f6e 2061 7320 7375 6368 2e0d  nation as such..
+00009a00: 0a0d 0a20 2031 342e 2052 6576 6973 6564  ...  14. Revised
+00009a10: 2056 6572 7369 6f6e 7320 6f66 2074 6869   Versions of thi
+00009a20: 7320 4c69 6365 6e73 652e 0d0a 0d0a 2020  s License.....  
+00009a30: 5468 6520 4672 6565 2053 6f66 7477 6172  The Free Softwar
+00009a40: 6520 466f 756e 6461 7469 6f6e 206d 6179  e Foundation may
+00009a50: 2070 7562 6c69 7368 2072 6576 6973 6564   publish revised
+00009a60: 2061 6e64 2f6f 7220 6e65 7720 7665 7273   and/or new vers
+00009a70: 696f 6e73 206f 660d 0a74 6865 2047 4e55  ions of..the GNU
+00009a80: 2047 656e 6572 616c 2050 7562 6c69 6320   General Public 
+00009a90: 4c69 6365 6e73 6520 6672 6f6d 2074 696d  License from tim
+00009aa0: 6520 746f 2074 696d 652e 2020 5375 6368  e to time.  Such
+00009ab0: 206e 6577 2076 6572 7369 6f6e 7320 7769   new versions wi
+00009ac0: 6c6c 0d0a 6265 2073 696d 696c 6172 2069  ll..be similar i
+00009ad0: 6e20 7370 6972 6974 2074 6f20 7468 6520  n spirit to the 
+00009ae0: 7072 6573 656e 7420 7665 7273 696f 6e2c  present version,
+00009af0: 2062 7574 206d 6179 2064 6966 6665 7220   but may differ 
+00009b00: 696e 2064 6574 6169 6c20 746f 0d0a 6164  in detail to..ad
+00009b10: 6472 6573 7320 6e65 7720 7072 6f62 6c65  dress new proble
+00009b20: 6d73 206f 7220 636f 6e63 6572 6e73 2e0d  ms or concerns..
+00009b30: 0a0d 0a20 2045 6163 6820 7665 7273 696f  ...  Each versio
+00009b40: 6e20 6973 2067 6976 656e 2061 2064 6973  n is given a dis
+00009b50: 7469 6e67 7569 7368 696e 6720 7665 7273  tinguishing vers
+00009b60: 696f 6e20 6e75 6d62 6572 2e20 2049 6620  ion number.  If 
+00009b70: 7468 650d 0a50 726f 6772 616d 2073 7065  the..Program spe
+00009b80: 6369 6669 6573 2074 6861 7420 6120 6365  cifies that a ce
+00009b90: 7274 6169 6e20 6e75 6d62 6572 6564 2076  rtain numbered v
+00009ba0: 6572 7369 6f6e 206f 6620 7468 6520 474e  ersion of the GN
+00009bb0: 5520 4765 6e65 7261 6c0d 0a50 7562 6c69  U General..Publi
+00009bc0: 6320 4c69 6365 6e73 6520 226f 7220 616e  c License "or an
+00009bd0: 7920 6c61 7465 7220 7665 7273 696f 6e22  y later version"
+00009be0: 2061 7070 6c69 6573 2074 6f20 6974 2c20   applies to it, 
+00009bf0: 796f 7520 6861 7665 2074 6865 0d0a 6f70  you have the..op
+00009c00: 7469 6f6e 206f 6620 666f 6c6c 6f77 696e  tion of followin
+00009c10: 6720 7468 6520 7465 726d 7320 616e 6420  g the terms and 
+00009c20: 636f 6e64 6974 696f 6e73 2065 6974 6865  conditions eithe
+00009c30: 7220 6f66 2074 6861 7420 6e75 6d62 6572  r of that number
+00009c40: 6564 0d0a 7665 7273 696f 6e20 6f72 206f  ed..version or o
+00009c50: 6620 616e 7920 6c61 7465 7220 7665 7273  f any later vers
+00009c60: 696f 6e20 7075 626c 6973 6865 6420 6279  ion published by
+00009c70: 2074 6865 2046 7265 6520 536f 6674 7761   the Free Softwa
+00009c80: 7265 0d0a 466f 756e 6461 7469 6f6e 2e20  re..Foundation. 
+00009c90: 2049 6620 7468 6520 5072 6f67 7261 6d20   If the Program 
+00009ca0: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
+00009cb0: 2061 2076 6572 7369 6f6e 206e 756d 6265   a version numbe
+00009cc0: 7220 6f66 2074 6865 0d0a 474e 5520 4765  r of the..GNU Ge
+00009cd0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+00009ce0: 656e 7365 2c20 796f 7520 6d61 7920 6368  ense, you may ch
+00009cf0: 6f6f 7365 2061 6e79 2076 6572 7369 6f6e  oose any version
+00009d00: 2065 7665 7220 7075 626c 6973 6865 640d   ever published.
+00009d10: 0a62 7920 7468 6520 4672 6565 2053 6f66  .by the Free Sof
+00009d20: 7477 6172 6520 466f 756e 6461 7469 6f6e  tware Foundation
+00009d30: 2e0d 0a0d 0a20 2049 6620 7468 6520 5072  .....  If the Pr
+00009d40: 6f67 7261 6d20 7370 6563 6966 6965 7320  ogram specifies 
+00009d50: 7468 6174 2061 2070 726f 7879 2063 616e  that a proxy can
+00009d60: 2064 6563 6964 6520 7768 6963 6820 6675   decide which fu
+00009d70: 7475 7265 0d0a 7665 7273 696f 6e73 206f  ture..versions o
+00009d80: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00009d90: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00009da0: 2063 616e 2062 6520 7573 6564 2c20 7468   can be used, th
+00009db0: 6174 2070 726f 7879 2773 0d0a 7075 626c  at proxy's..publ
+00009dc0: 6963 2073 7461 7465 6d65 6e74 206f 6620  ic statement of 
+00009dd0: 6163 6365 7074 616e 6365 206f 6620 6120  acceptance of a 
+00009de0: 7665 7273 696f 6e20 7065 726d 616e 656e  version permanen
+00009df0: 746c 7920 6175 7468 6f72 697a 6573 2079  tly authorizes y
+00009e00: 6f75 0d0a 746f 2063 686f 6f73 6520 7468  ou..to choose th
+00009e10: 6174 2076 6572 7369 6f6e 2066 6f72 2074  at version for t
+00009e20: 6865 2050 726f 6772 616d 2e0d 0a0d 0a20  he Program..... 
+00009e30: 204c 6174 6572 206c 6963 656e 7365 2076   Later license v
+00009e40: 6572 7369 6f6e 7320 6d61 7920 6769 7665  ersions may give
+00009e50: 2079 6f75 2061 6464 6974 696f 6e61 6c20   you additional 
+00009e60: 6f72 2064 6966 6665 7265 6e74 0d0a 7065  or different..pe
+00009e70: 726d 6973 7369 6f6e 732e 2020 486f 7765  rmissions.  Howe
+00009e80: 7665 722c 206e 6f20 6164 6469 7469 6f6e  ver, no addition
+00009e90: 616c 206f 626c 6967 6174 696f 6e73 2061  al obligations a
+00009ea0: 7265 2069 6d70 6f73 6564 206f 6e20 616e  re imposed on an
+00009eb0: 790d 0a61 7574 686f 7220 6f72 2063 6f70  y..author or cop
+00009ec0: 7972 6967 6874 2068 6f6c 6465 7220 6173  yright holder as
+00009ed0: 2061 2072 6573 756c 7420 6f66 2079 6f75   a result of you
+00009ee0: 7220 6368 6f6f 7369 6e67 2074 6f20 666f  r choosing to fo
+00009ef0: 6c6c 6f77 2061 0d0a 6c61 7465 7220 7665  llow a..later ve
+00009f00: 7273 696f 6e2e 0d0a 0d0a 2020 3135 2e20  rsion.....  15. 
+00009f10: 4469 7363 6c61 696d 6572 206f 6620 5761  Disclaimer of Wa
+00009f20: 7272 616e 7479 2e0d 0a0d 0a20 2054 4845  rranty.....  THE
+00009f30: 5245 2049 5320 4e4f 2057 4152 5241 4e54  RE IS NO WARRANT
+00009f40: 5920 464f 5220 5448 4520 5052 4f47 5241  Y FOR THE PROGRA
+00009f50: 4d2c 2054 4f20 5448 4520 4558 5445 4e54  M, TO THE EXTENT
+00009f60: 2050 4552 4d49 5454 4544 2042 590d 0a41   PERMITTED BY..A
+00009f70: 5050 4c49 4341 424c 4520 4c41 572e 2020  PPLICABLE LAW.  
+00009f80: 4558 4345 5054 2057 4845 4e20 4f54 4845  EXCEPT WHEN OTHE
+00009f90: 5257 4953 4520 5354 4154 4544 2049 4e20  RWISE STATED IN 
+00009fa0: 5752 4954 494e 4720 5448 4520 434f 5059  WRITING THE COPY
+00009fb0: 5249 4748 540d 0a48 4f4c 4445 5253 2041  RIGHT..HOLDERS A
+00009fc0: 4e44 2f4f 5220 4f54 4845 5220 5041 5254  ND/OR OTHER PART
+00009fd0: 4945 5320 5052 4f56 4944 4520 5448 4520  IES PROVIDE THE 
+00009fe0: 5052 4f47 5241 4d20 2241 5320 4953 2220  PROGRAM "AS IS" 
+00009ff0: 5749 5448 4f55 5420 5741 5252 414e 5459  WITHOUT WARRANTY
+0000a000: 0d0a 4f46 2041 4e59 204b 494e 442c 2045  ..OF ANY KIND, E
+0000a010: 4954 4845 5220 4558 5052 4553 5345 4420  ITHER EXPRESSED 
+0000a020: 4f52 2049 4d50 4c49 4544 2c20 494e 434c  OR IMPLIED, INCL
+0000a030: 5544 494e 472c 2042 5554 204e 4f54 204c  UDING, BUT NOT L
+0000a040: 494d 4954 4544 2054 4f2c 0d0a 5448 4520  IMITED TO,..THE 
+0000a050: 494d 504c 4945 4420 5741 5252 414e 5449  IMPLIED WARRANTI
+0000a060: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
+0000a070: 494c 4954 5920 414e 4420 4649 544e 4553  ILITY AND FITNES
+0000a080: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
+0000a090: 4152 0d0a 5055 5250 4f53 452e 2020 5448  AR..PURPOSE.  TH
+0000a0a0: 4520 454e 5449 5245 2052 4953 4b20 4153  E ENTIRE RISK AS
+0000a0b0: 2054 4f20 5448 4520 5155 414c 4954 5920   TO THE QUALITY 
+0000a0c0: 414e 4420 5045 5246 4f52 4d41 4e43 4520  AND PERFORMANCE 
+0000a0d0: 4f46 2054 4845 2050 524f 4752 414d 0d0a  OF THE PROGRAM..
+0000a0e0: 4953 2057 4954 4820 594f 552e 2020 5348  IS WITH YOU.  SH
+0000a0f0: 4f55 4c44 2054 4845 2050 524f 4752 414d  OULD THE PROGRAM
+0000a100: 2050 524f 5645 2044 4546 4543 5449 5645   PROVE DEFECTIVE
+0000a110: 2c20 594f 5520 4153 5355 4d45 2054 4845  , YOU ASSUME THE
+0000a120: 2043 4f53 5420 4f46 0d0a 414c 4c20 4e45   COST OF..ALL NE
+0000a130: 4345 5353 4152 5920 5345 5256 4943 494e  CESSARY SERVICIN
+0000a140: 472c 2052 4550 4149 5220 4f52 2043 4f52  G, REPAIR OR COR
+0000a150: 5245 4354 494f 4e2e 0d0a 0d0a 2020 3136  RECTION.....  16
+0000a160: 2e20 4c69 6d69 7461 7469 6f6e 206f 6620  . Limitation of 
+0000a170: 4c69 6162 696c 6974 792e 0d0a 0d0a 2020  Liability.....  
+0000a180: 494e 204e 4f20 4556 454e 5420 554e 4c45  IN NO EVENT UNLE
+0000a190: 5353 2052 4551 5549 5245 4420 4259 2041  SS REQUIRED BY A
+0000a1a0: 5050 4c49 4341 424c 4520 4c41 5720 4f52  PPLICABLE LAW OR
+0000a1b0: 2041 4752 4545 4420 544f 2049 4e20 5752   AGREED TO IN WR
+0000a1c0: 4954 494e 470d 0a57 494c 4c20 414e 5920  ITING..WILL ANY 
+0000a1d0: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
+0000a1e0: 2c20 4f52 2041 4e59 204f 5448 4552 2050  , OR ANY OTHER P
+0000a1f0: 4152 5459 2057 484f 204d 4f44 4946 4945  ARTY WHO MODIFIE
+0000a200: 5320 414e 442f 4f52 2043 4f4e 5645 5953  S AND/OR CONVEYS
+0000a210: 0d0a 5448 4520 5052 4f47 5241 4d20 4153  ..THE PROGRAM AS
+0000a220: 2050 4552 4d49 5454 4544 2041 424f 5645   PERMITTED ABOVE
+0000a230: 2c20 4245 204c 4941 424c 4520 544f 2059  , BE LIABLE TO Y
+0000a240: 4f55 2046 4f52 2044 414d 4147 4553 2c20  OU FOR DAMAGES, 
+0000a250: 494e 434c 5544 494e 4720 414e 590d 0a47  INCLUDING ANY..G
+0000a260: 454e 4552 414c 2c20 5350 4543 4941 4c2c  ENERAL, SPECIAL,
+0000a270: 2049 4e43 4944 454e 5441 4c20 4f52 2043   INCIDENTAL OR C
+0000a280: 4f4e 5345 5155 454e 5449 414c 2044 414d  ONSEQUENTIAL DAM
+0000a290: 4147 4553 2041 5249 5349 4e47 204f 5554  AGES ARISING OUT
+0000a2a0: 204f 4620 5448 450d 0a55 5345 204f 5220   OF THE..USE OR 
+0000a2b0: 494e 4142 494c 4954 5920 544f 2055 5345  INABILITY TO USE
+0000a2c0: 2054 4845 2050 524f 4752 414d 2028 494e   THE PROGRAM (IN
+0000a2d0: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
+0000a2e0: 4c49 4d49 5445 4420 544f 204c 4f53 5320  LIMITED TO LOSS 
+0000a2f0: 4f46 0d0a 4441 5441 204f 5220 4441 5441  OF..DATA OR DATA
+0000a300: 2042 4549 4e47 2052 454e 4445 5245 4420   BEING RENDERED 
+0000a310: 494e 4143 4355 5241 5445 204f 5220 4c4f  INACCURATE OR LO
+0000a320: 5353 4553 2053 5553 5441 494e 4544 2042  SSES SUSTAINED B
+0000a330: 5920 594f 5520 4f52 2054 4849 5244 0d0a  Y YOU OR THIRD..
+0000a340: 5041 5254 4945 5320 4f52 2041 2046 4149  PARTIES OR A FAI
+0000a350: 4c55 5245 204f 4620 5448 4520 5052 4f47  LURE OF THE PROG
+0000a360: 5241 4d20 544f 204f 5045 5241 5445 2057  RAM TO OPERATE W
+0000a370: 4954 4820 414e 5920 4f54 4845 5220 5052  ITH ANY OTHER PR
+0000a380: 4f47 5241 4d53 292c 0d0a 4556 454e 2049  OGRAMS),..EVEN I
+0000a390: 4620 5355 4348 2048 4f4c 4445 5220 4f52  F SUCH HOLDER OR
+0000a3a0: 204f 5448 4552 2050 4152 5459 2048 4153   OTHER PARTY HAS
+0000a3b0: 2042 4545 4e20 4144 5649 5345 4420 4f46   BEEN ADVISED OF
+0000a3c0: 2054 4845 2050 4f53 5349 4249 4c49 5459   THE POSSIBILITY
+0000a3d0: 204f 460d 0a53 5543 4820 4441 4d41 4745   OF..SUCH DAMAGE
+0000a3e0: 532e 0d0a 0d0a 2020 3137 2e20 496e 7465  S.....  17. Inte
+0000a3f0: 7270 7265 7461 7469 6f6e 206f 6620 5365  rpretation of Se
+0000a400: 6374 696f 6e73 2031 3520 616e 6420 3136  ctions 15 and 16
+0000a410: 2e0d 0a0d 0a20 2049 6620 7468 6520 6469  .....  If the di
+0000a420: 7363 6c61 696d 6572 206f 6620 7761 7272  sclaimer of warr
+0000a430: 616e 7479 2061 6e64 206c 696d 6974 6174  anty and limitat
+0000a440: 696f 6e20 6f66 206c 6961 6269 6c69 7479  ion of liability
+0000a450: 2070 726f 7669 6465 640d 0a61 626f 7665   provided..above
+0000a460: 2063 616e 6e6f 7420 6265 2067 6976 656e   cannot be given
+0000a470: 206c 6f63 616c 206c 6567 616c 2065 6666   local legal eff
+0000a480: 6563 7420 6163 636f 7264 696e 6720 746f  ect according to
+0000a490: 2074 6865 6972 2074 6572 6d73 2c0d 0a72   their terms,..r
+0000a4a0: 6576 6965 7769 6e67 2063 6f75 7274 7320  eviewing courts 
+0000a4b0: 7368 616c 6c20 6170 706c 7920 6c6f 6361  shall apply loca
+0000a4c0: 6c20 6c61 7720 7468 6174 206d 6f73 7420  l law that most 
+0000a4d0: 636c 6f73 656c 7920 6170 7072 6f78 696d  closely approxim
+0000a4e0: 6174 6573 0d0a 616e 2061 6273 6f6c 7574  ates..an absolut
+0000a4f0: 6520 7761 6976 6572 206f 6620 616c 6c20  e waiver of all 
+0000a500: 6369 7669 6c20 6c69 6162 696c 6974 7920  civil liability 
+0000a510: 696e 2063 6f6e 6e65 6374 696f 6e20 7769  in connection wi
+0000a520: 7468 2074 6865 0d0a 5072 6f67 7261 6d2c  th the..Program,
+0000a530: 2075 6e6c 6573 7320 6120 7761 7272 616e   unless a warran
+0000a540: 7479 206f 7220 6173 7375 6d70 7469 6f6e  ty or assumption
+0000a550: 206f 6620 6c69 6162 696c 6974 7920 6163   of liability ac
+0000a560: 636f 6d70 616e 6965 7320 610d 0a63 6f70  companies a..cop
+0000a570: 7920 6f66 2074 6865 2050 726f 6772 616d  y of the Program
+0000a580: 2069 6e20 7265 7475 726e 2066 6f72 2061   in return for a
+0000a590: 2066 6565 2e0d 0a0d 0a20 2020 2020 2020   fee.....       
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 454e                EN
+0000a5b0: 4420 4f46 2054 4552 4d53 2041 4e44 2043  D OF TERMS AND C
+0000a5c0: 4f4e 4449 5449 4f4e 530d 0a0d 0a20 2020  ONDITIONS....   
+0000a5d0: 2020 2020 2020 2020 2048 6f77 2074 6f20           How to 
+0000a5e0: 4170 706c 7920 5468 6573 6520 5465 726d  Apply These Term
+0000a5f0: 7320 746f 2059 6f75 7220 4e65 7720 5072  s to Your New Pr
+0000a600: 6f67 7261 6d73 0d0a 0d0a 2020 4966 2079  ograms....  If y
+0000a610: 6f75 2064 6576 656c 6f70 2061 206e 6577  ou develop a new
+0000a620: 2070 726f 6772 616d 2c20 616e 6420 796f   program, and yo
+0000a630: 7520 7761 6e74 2069 7420 746f 2062 6520  u want it to be 
+0000a640: 6f66 2074 6865 2067 7265 6174 6573 740d  of the greatest.
+0000a650: 0a70 6f73 7369 626c 6520 7573 6520 746f  .possible use to
+0000a660: 2074 6865 2070 7562 6c69 632c 2074 6865   the public, the
+0000a670: 2062 6573 7420 7761 7920 746f 2061 6368   best way to ach
+0000a680: 6965 7665 2074 6869 7320 6973 2074 6f20  ieve this is to 
+0000a690: 6d61 6b65 2069 740d 0a66 7265 6520 736f  make it..free so
+0000a6a0: 6674 7761 7265 2077 6869 6368 2065 7665  ftware which eve
+0000a6b0: 7279 6f6e 6520 6361 6e20 7265 6469 7374  ryone can redist
+0000a6c0: 7269 6275 7465 2061 6e64 2063 6861 6e67  ribute and chang
+0000a6d0: 6520 756e 6465 7220 7468 6573 6520 7465  e under these te
+0000a6e0: 726d 732e 0d0a 0d0a 2020 546f 2064 6f20  rms.....  To do 
+0000a6f0: 736f 2c20 6174 7461 6368 2074 6865 2066  so, attach the f
+0000a700: 6f6c 6c6f 7769 6e67 206e 6f74 6963 6573  ollowing notices
+0000a710: 2074 6f20 7468 6520 7072 6f67 7261 6d2e   to the program.
+0000a720: 2020 4974 2069 7320 7361 6665 7374 0d0a    It is safest..
+0000a730: 746f 2061 7474 6163 6820 7468 656d 2074  to attach them t
+0000a740: 6f20 7468 6520 7374 6172 7420 6f66 2065  o the start of e
+0000a750: 6163 6820 736f 7572 6365 2066 696c 6520  ach source file 
+0000a760: 746f 206d 6f73 7420 6566 6665 6374 6976  to most effectiv
+0000a770: 656c 790d 0a73 7461 7465 2074 6865 2065  ely..state the e
+0000a780: 7863 6c75 7369 6f6e 206f 6620 7761 7272  xclusion of warr
+0000a790: 616e 7479 3b20 616e 6420 6561 6368 2066  anty; and each f
+0000a7a0: 696c 6520 7368 6f75 6c64 2068 6176 6520  ile should have 
+0000a7b0: 6174 206c 6561 7374 0d0a 7468 6520 2263  at least..the "c
+0000a7c0: 6f70 7972 6967 6874 2220 6c69 6e65 2061  opyright" line a
+0000a7d0: 6e64 2061 2070 6f69 6e74 6572 2074 6f20  nd a pointer to 
+0000a7e0: 7768 6572 6520 7468 6520 6675 6c6c 206e  where the full n
+0000a7f0: 6f74 6963 6520 6973 2066 6f75 6e64 2e0d  otice is found..
+0000a800: 0a0d 0a20 2020 203c 6f6e 6520 6c69 6e65  ...    <one line
+0000a810: 2074 6f20 6769 7665 2074 6865 2070 726f   to give the pro
+0000a820: 6772 616d 2773 206e 616d 6520 616e 6420  gram's name and 
+0000a830: 6120 6272 6965 6620 6964 6561 206f 6620  a brief idea of 
+0000a840: 7768 6174 2069 7420 646f 6573 2e3e 0d0a  what it does.>..
+0000a850: 2020 2020 436f 7079 7269 6768 7420 2843      Copyright (C
+0000a860: 2920 3c79 6561 723e 2020 3c6e 616d 6520  ) <year>  <name 
+0000a870: 6f66 2061 7574 686f 723e 0d0a 0d0a 2020  of author>....  
+0000a880: 2020 5468 6973 2070 726f 6772 616d 2069    This program i
+0000a890: 7320 6672 6565 2073 6f66 7477 6172 653a  s free software:
+0000a8a0: 2079 6f75 2063 616e 2072 6564 6973 7472   you can redistr
+0000a8b0: 6962 7574 6520 6974 2061 6e64 2f6f 7220  ibute it and/or 
+0000a8c0: 6d6f 6469 6679 0d0a 2020 2020 6974 2075  modify..    it u
+0000a8d0: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
+0000a8e0: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+0000a8f0: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+0000a900: 2061 7320 7075 626c 6973 6865 6420 6279   as published by
+0000a910: 0d0a 2020 2020 7468 6520 4672 6565 2053  ..    the Free S
+0000a920: 6f66 7477 6172 6520 466f 756e 6461 7469  oftware Foundati
+0000a930: 6f6e 2c20 6569 7468 6572 2076 6572 7369  on, either versi
+0000a940: 6f6e 2033 206f 6620 7468 6520 4c69 6365  on 3 of the Lice
+0000a950: 6e73 652c 206f 720d 0a20 2020 2028 6174  nse, or..    (at
+0000a960: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
+0000a970: 7920 6c61 7465 7220 7665 7273 696f 6e2e  y later version.
+0000a980: 0d0a 0d0a 2020 2020 5468 6973 2070 726f  ....    This pro
+0000a990: 6772 616d 2069 7320 6469 7374 7269 6275  gram is distribu
+0000a9a0: 7465 6420 696e 2074 6865 2068 6f70 6520  ted in the hope 
+0000a9b0: 7468 6174 2069 7420 7769 6c6c 2062 6520  that it will be 
+0000a9c0: 7573 6566 756c 2c0d 0a20 2020 2062 7574  useful,..    but
+0000a9d0: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+0000a9e0: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+0000a9f0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+0000aa00: 7761 7272 616e 7479 206f 660d 0a20 2020  warranty of..   
+0000aa10: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
+0000aa20: 206f 7220 4649 544e 4553 5320 464f 5220   or FITNESS FOR 
+0000aa30: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
+0000aa40: 504f 5345 2e20 2053 6565 2074 6865 0d0a  POSE.  See the..
+0000aa50: 2020 2020 474e 5520 4765 6e65 7261 6c20      GNU General 
+0000aa60: 5075 626c 6963 204c 6963 656e 7365 2066  Public License f
+0000aa70: 6f72 206d 6f72 6520 6465 7461 696c 732e  or more details.
+0000aa80: 0d0a 0d0a 2020 2020 596f 7520 7368 6f75  ....    You shou
+0000aa90: 6c64 2068 6176 6520 7265 6365 6976 6564  ld have received
+0000aaa0: 2061 2063 6f70 7920 6f66 2074 6865 2047   a copy of the G
+0000aab0: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
+0000aac0: 6320 4c69 6365 6e73 650d 0a20 2020 2061  c License..    a
+0000aad0: 6c6f 6e67 2077 6974 6820 7468 6973 2070  long with this p
+0000aae0: 726f 6772 616d 2e20 2049 6620 6e6f 742c  rogram.  If not,
+0000aaf0: 2073 6565 203c 6874 7470 733a 2f2f 7777   see <https://ww
+0000ab00: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+0000ab10: 6573 2f3e 2e0d 0a0d 0a41 6c73 6f20 6164  es/>.....Also ad
+0000ab20: 6420 696e 666f 726d 6174 696f 6e20 6f6e  d information on
+0000ab30: 2068 6f77 2074 6f20 636f 6e74 6163 7420   how to contact 
+0000ab40: 796f 7520 6279 2065 6c65 6374 726f 6e69  you by electroni
+0000ab50: 6320 616e 6420 7061 7065 7220 6d61 696c  c and paper mail
+0000ab60: 2e0d 0a0d 0a20 2049 6620 7468 6520 7072  .....  If the pr
+0000ab70: 6f67 7261 6d20 646f 6573 2074 6572 6d69  ogram does termi
+0000ab80: 6e61 6c20 696e 7465 7261 6374 696f 6e2c  nal interaction,
+0000ab90: 206d 616b 6520 6974 206f 7574 7075 7420   make it output 
+0000aba0: 6120 7368 6f72 740d 0a6e 6f74 6963 6520  a short..notice 
+0000abb0: 6c69 6b65 2074 6869 7320 7768 656e 2069  like this when i
+0000abc0: 7420 7374 6172 7473 2069 6e20 616e 2069  t starts in an i
+0000abd0: 6e74 6572 6163 7469 7665 206d 6f64 653a  nteractive mode:
+0000abe0: 0d0a 0d0a 2020 2020 3c70 726f 6772 616d  ....    <program
+0000abf0: 3e20 2043 6f70 7972 6967 6874 2028 4329  >  Copyright (C)
+0000ac00: 203c 7965 6172 3e20 203c 6e61 6d65 206f   <year>  <name o
+0000ac10: 6620 6175 7468 6f72 3e0d 0a20 2020 2054  f author>..    T
+0000ac20: 6869 7320 7072 6f67 7261 6d20 636f 6d65  his program come
+0000ac30: 7320 7769 7468 2041 4253 4f4c 5554 454c  s with ABSOLUTEL
+0000ac40: 5920 4e4f 2057 4152 5241 4e54 593b 2066  Y NO WARRANTY; f
+0000ac50: 6f72 2064 6574 6169 6c73 2074 7970 6520  or details type 
+0000ac60: 6073 686f 7720 7727 2e0d 0a20 2020 2054  `show w'...    T
+0000ac70: 6869 7320 6973 2066 7265 6520 736f 6674  his is free soft
+0000ac80: 7761 7265 2c20 616e 6420 796f 7520 6172  ware, and you ar
+0000ac90: 6520 7765 6c63 6f6d 6520 746f 2072 6564  e welcome to red
+0000aca0: 6973 7472 6962 7574 6520 6974 0d0a 2020  istribute it..  
+0000acb0: 2020 756e 6465 7220 6365 7274 6169 6e20    under certain 
+0000acc0: 636f 6e64 6974 696f 6e73 3b20 7479 7065  conditions; type
+0000acd0: 2060 7368 6f77 2063 2720 666f 7220 6465   `show c' for de
+0000ace0: 7461 696c 732e 0d0a 0d0a 5468 6520 6879  tails.....The hy
+0000acf0: 706f 7468 6574 6963 616c 2063 6f6d 6d61  pothetical comma
+0000ad00: 6e64 7320 6073 686f 7720 7727 2061 6e64  nds `show w' and
+0000ad10: 2060 7368 6f77 2063 2720 7368 6f75 6c64   `show c' should
+0000ad20: 2073 686f 7720 7468 6520 6170 7072 6f70   show the approp
+0000ad30: 7269 6174 650d 0a70 6172 7473 206f 6620  riate..parts of 
+0000ad40: 7468 6520 4765 6e65 7261 6c20 5075 626c  the General Publ
+0000ad50: 6963 204c 6963 656e 7365 2e20 204f 6620  ic License.  Of 
+0000ad60: 636f 7572 7365 2c20 796f 7572 2070 726f  course, your pro
+0000ad70: 6772 616d 2773 2063 6f6d 6d61 6e64 730d  gram's commands.
+0000ad80: 0a6d 6967 6874 2062 6520 6469 6666 6572  .might be differ
+0000ad90: 656e 743b 2066 6f72 2061 2047 5549 2069  ent; for a GUI i
+0000ada0: 6e74 6572 6661 6365 2c20 796f 7520 776f  nterface, you wo
+0000adb0: 756c 6420 7573 6520 616e 2022 6162 6f75  uld use an "abou
+0000adc0: 7420 626f 7822 2e0d 0a0d 0a20 2059 6f75  t box".....  You
+0000add0: 2073 686f 756c 6420 616c 736f 2067 6574   should also get
+0000ade0: 2079 6f75 7220 656d 706c 6f79 6572 2028   your employer (
+0000adf0: 6966 2079 6f75 2077 6f72 6b20 6173 2061  if you work as a
+0000ae00: 2070 726f 6772 616d 6d65 7229 206f 7220   programmer) or 
+0000ae10: 7363 686f 6f6c 2c0d 0a69 6620 616e 792c  school,..if any,
+0000ae20: 2074 6f20 7369 676e 2061 2022 636f 7079   to sign a "copy
+0000ae30: 7269 6768 7420 6469 7363 6c61 696d 6572  right disclaimer
+0000ae40: 2220 666f 7220 7468 6520 7072 6f67 7261  " for the progra
+0000ae50: 6d2c 2069 6620 6e65 6365 7373 6172 792e  m, if necessary.
+0000ae60: 0d0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
+0000ae70: 6d61 7469 6f6e 206f 6e20 7468 6973 2c20  mation on this, 
+0000ae80: 616e 6420 686f 7720 746f 2061 7070 6c79  and how to apply
+0000ae90: 2061 6e64 2066 6f6c 6c6f 7720 7468 6520   and follow the 
+0000aea0: 474e 5520 4750 4c2c 2073 6565 0d0a 3c68  GNU GPL, see..<h
+0000aeb0: 7474 7073 3a2f 2f77 7777 2e67 6e75 2e6f  ttps://www.gnu.o
+0000aec0: 7267 2f6c 6963 656e 7365 732f 3e2e 0d0a  rg/licenses/>...
+0000aed0: 0d0a 2020 5468 6520 474e 5520 4765 6e65  ..  The GNU Gene
+0000aee0: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+0000aef0: 7365 2064 6f65 7320 6e6f 7420 7065 726d  se does not perm
+0000af00: 6974 2069 6e63 6f72 706f 7261 7469 6e67  it incorporating
+0000af10: 2079 6f75 7220 7072 6f67 7261 6d0d 0a69   your program..i
+0000af20: 6e74 6f20 7072 6f70 7269 6574 6172 7920  nto proprietary 
+0000af30: 7072 6f67 7261 6d73 2e20 2049 6620 796f  programs.  If yo
+0000af40: 7572 2070 726f 6772 616d 2069 7320 6120  ur program is a 
+0000af50: 7375 6272 6f75 7469 6e65 206c 6962 7261  subroutine libra
+0000af60: 7279 2c20 796f 750d 0a6d 6179 2063 6f6e  ry, you..may con
+0000af70: 7369 6465 7220 6974 206d 6f72 6520 7573  sider it more us
+0000af80: 6566 756c 2074 6f20 7065 726d 6974 206c  eful to permit l
+0000af90: 696e 6b69 6e67 2070 726f 7072 6965 7461  inking proprieta
+0000afa0: 7279 2061 7070 6c69 6361 7469 6f6e 7320  ry applications 
+0000afb0: 7769 7468 0d0a 7468 6520 6c69 6272 6172  with..the librar
+0000afc0: 792e 2020 4966 2074 6869 7320 6973 2077  y.  If this is w
+0000afd0: 6861 7420 796f 7520 7761 6e74 2074 6f20  hat you want to 
+0000afe0: 646f 2c20 7573 6520 7468 6520 474e 5520  do, use the GNU 
+0000aff0: 4c65 7373 6572 2047 656e 6572 616c 0d0a  Lesser General..
+0000b000: 5075 626c 6963 204c 6963 656e 7365 2069  Public License i
+0000b010: 6e73 7465 6164 206f 6620 7468 6973 204c  nstead of this L
+0000b020: 6963 656e 7365 2e20 2042 7574 2066 6972  icense.  But fir
+0000b030: 7374 2c20 706c 6561 7365 2072 6561 640d  st, please read.
+0000b040: 0a3c 6874 7470 733a 2f2f 7777 772e 676e  .<https://www.gn
+0000b050: 752e 6f72 672f 6c69 6365 6e73 6573 2f77  u.org/licenses/w
+0000b060: 6879 2d6e 6f74 2d6c 6770 6c2e 6874 6d6c  hy-not-lgpl.html
+0000b070: 3e2e 0d0a                                >...
```

### Comparing `osm_easy_api-0.4.2/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-1.0.0/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

