# Comparing `tmp/navigaattori-2023.1.17.tar.gz` & `tmp/navigaattori-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigaattori-2023.1.17.tar", last modified: Tue Jan 17 22:22:17 2023, max compression
+gzip compressed data, was "navigaattori-2023.6.18.tar", last modified: Sun Jun 18 08:44:55 2023, max compression
```

## Comparing `navigaattori-2023.1.17.tar` & `navigaattori-2023.6.18.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-17 22:22:17.443704 navigaattori-2023.1.17/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 navigaattori-2023.1.17/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       71 2023-01-14 21:07:37.000000 navigaattori-2023.1.17/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2727 2023-01-17 22:22:17.443369 navigaattori-2023.1.17/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1755 2023-01-08 11:58:55.000000 navigaattori-2023.1.17/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-17 22:22:17.437214 navigaattori-2023.1.17/navigaattori/
--rw-r--r--   0 ruth       (501) staff       (20)     2529 2023-01-17 22:15:47.000000 navigaattori-2023.1.17/navigaattori/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      137 2022-12-10 17:54:57.000000 navigaattori-2023.1.17/navigaattori/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)      395 2022-12-11 19:41:57.000000 navigaattori-2023.1.17/navigaattori/api.py
--rw-r--r--   0 ruth       (501) staff       (20)     3625 2022-12-12 19:05:30.000000 navigaattori-2023.1.17/navigaattori/approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     3337 2022-12-12 19:05:42.000000 navigaattori-2023.1.17/navigaattori/bind.py
--rw-r--r--   0 ruth       (501) staff       (20)     3958 2022-12-12 19:05:17.000000 navigaattori-2023.1.17/navigaattori/changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     4823 2023-01-14 20:50:41.000000 navigaattori-2023.1.17/navigaattori/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     1305 2022-12-13 18:56:41.000000 navigaattori-2023.1.17/navigaattori/eject.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 16:55:26.000000 navigaattori-2023.1.17/navigaattori/fs.py
--rw-r--r--   0 ruth       (501) staff       (20)     1068 2022-12-23 15:20:07.000000 navigaattori-2023.1.17/navigaattori/liitos_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)     6503 2022-12-13 20:48:06.000000 navigaattori-2023.1.17/navigaattori/meta.py
--rw-r--r--   0 ruth       (501) staff       (20)    16663 2022-12-23 15:22:25.000000 navigaattori-2023.1.17/navigaattori/structures.py
--rw-r--r--   0 ruth       (501) staff       (20)     1333 2022-12-23 15:22:10.000000 navigaattori-2023.1.17/navigaattori/template_loader.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-17 22:22:17.439254 navigaattori-2023.1.17/navigaattori/templates/
--rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:41:06.000000 navigaattori-2023.1.17/navigaattori/templates/liitos_vocabulary.yml
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 16:55:18.000000 navigaattori-2023.1.17/navigaattori/vcs.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-17 22:22:17.438938 navigaattori-2023.1.17/navigaattori.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2727 2023-01-17 22:22:17.000000 navigaattori-2023.1.17/navigaattori.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      832 2023-01-17 22:22:17.000000 navigaattori-2023.1.17/navigaattori.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-01-17 22:22:17.000000 navigaattori-2023.1.17/navigaattori.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       54 2023-01-17 22:22:17.000000 navigaattori-2023.1.17/navigaattori.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      154 2023-01-17 22:22:17.000000 navigaattori-2023.1.17/navigaattori.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       13 2023-01-17 22:22:17.000000 navigaattori-2023.1.17/navigaattori.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2689 2023-01-17 20:42:01.000000 navigaattori-2023.1.17/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-01-17 22:22:17.443743 navigaattori-2023.1.17/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-01-17 22:22:17.443032 navigaattori-2023.1.17/test/
--rw-r--r--   0 ruth       (501) staff       (20)     1254 2022-12-11 19:45:24.000000 navigaattori-2023.1.17/test/test_api.py
--rw-r--r--   0 ruth       (501) staff       (20)     1942 2022-12-23 15:23:13.000000 navigaattori-2023.1.17/test/test_approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1163 2022-12-11 20:12:36.000000 navigaattori-2023.1.17/test/test_bind.py
--rw-r--r--   0 ruth       (501) staff       (20)     2017 2022-12-23 15:23:33.000000 navigaattori-2023.1.17/test/test_changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     1280 2022-12-12 18:49:36.000000 navigaattori-2023.1.17/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      892 2022-12-13 20:38:32.000000 navigaattori-2023.1.17/test/test_eject.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 17:13:22.000000 navigaattori-2023.1.17/test/test_fs.py
--rw-r--r--   0 ruth       (501) staff       (20)     3396 2023-01-17 22:13:10.000000 navigaattori-2023.1.17/test/test_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      704 2022-12-13 20:47:13.000000 navigaattori-2023.1.17/test/test_template_loader.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 17:13:25.000000 navigaattori-2023.1.17/test/test_vcs.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 08:44:55.234682 navigaattori-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 navigaattori-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       71 2023-01-14 21:07:37.000000 navigaattori-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3228 2023-06-18 08:44:55.234530 navigaattori-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2205 2023-03-14 22:31:47.000000 navigaattori-2023.6.18/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 08:44:55.227442 navigaattori-2023.6.18/navigaattori/
+-rw-r--r--   0 ruth       (501) staff       (20)     2529 2023-06-18 08:42:04.000000 navigaattori-2023.6.18/navigaattori/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      137 2022-12-10 17:54:57.000000 navigaattori-2023.6.18/navigaattori/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      395 2022-12-11 19:41:57.000000 navigaattori-2023.6.18/navigaattori/api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3625 2022-12-12 19:05:30.000000 navigaattori-2023.6.18/navigaattori/approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3337 2022-12-12 19:05:42.000000 navigaattori-2023.6.18/navigaattori/bind.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3958 2022-12-12 19:05:17.000000 navigaattori-2023.6.18/navigaattori/changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4823 2023-01-14 20:50:41.000000 navigaattori-2023.6.18/navigaattori/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1305 2022-12-13 18:56:41.000000 navigaattori-2023.6.18/navigaattori/eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 16:55:26.000000 navigaattori-2023.6.18/navigaattori/fs.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5072 2023-06-18 08:30:56.000000 navigaattori-2023.6.18/navigaattori/layout.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1068 2022-12-23 15:20:07.000000 navigaattori-2023.6.18/navigaattori/liitos_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6503 2022-12-13 20:48:06.000000 navigaattori-2023.6.18/navigaattori/meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)    17989 2023-06-18 08:26:51.000000 navigaattori-2023.6.18/navigaattori/structures.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1333 2022-12-23 15:22:10.000000 navigaattori-2023.6.18/navigaattori/template_loader.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 08:44:55.230375 navigaattori-2023.6.18/navigaattori/templates/
+-rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:41:06.000000 navigaattori-2023.6.18/navigaattori/templates/liitos_vocabulary.yml
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 16:55:18.000000 navigaattori-2023.6.18/navigaattori/vcs.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 08:44:55.229844 navigaattori-2023.6.18/navigaattori.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3228 2023-06-18 08:44:55.000000 navigaattori-2023.6.18/navigaattori.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      875 2023-06-18 08:44:55.000000 navigaattori-2023.6.18/navigaattori.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 08:44:55.000000 navigaattori-2023.6.18/navigaattori.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       54 2023-06-18 08:44:55.000000 navigaattori-2023.6.18/navigaattori.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      154 2023-06-18 08:44:55.000000 navigaattori-2023.6.18/navigaattori.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       13 2023-06-18 08:44:55.000000 navigaattori-2023.6.18/navigaattori.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2744 2023-06-18 07:56:24.000000 navigaattori-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 08:44:55.234719 navigaattori-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 08:44:55.234376 navigaattori-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     1254 2022-12-11 19:45:24.000000 navigaattori-2023.6.18/test/test_api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1942 2022-12-23 15:23:13.000000 navigaattori-2023.6.18/test/test_approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1163 2022-12-11 20:12:36.000000 navigaattori-2023.6.18/test/test_bind.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2017 2022-12-23 15:23:33.000000 navigaattori-2023.6.18/test/test_changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1280 2022-12-12 18:49:36.000000 navigaattori-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      892 2022-12-13 20:38:32.000000 navigaattori-2023.6.18/test/test_eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 17:13:22.000000 navigaattori-2023.6.18/test/test_fs.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1785 2023-06-18 08:38:09.000000 navigaattori-2023.6.18/test/test_layout.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3396 2023-01-17 22:13:10.000000 navigaattori-2023.6.18/test/test_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      704 2022-12-13 20:47:13.000000 navigaattori-2023.6.18/test/test_template_loader.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-12-10 17:13:25.000000 navigaattori-2023.6.18/test/test_vcs.py
```

### Comparing `navigaattori-2023.1.17/LICENSE` & `navigaattori-2023.6.18/LICENSE`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/PKG-INFO` & `navigaattori-2023.6.18/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 Metadata-Version: 2.1
 Name: navigaattori
-Version: 2023.1.17
+Version: 2023.6.18
 Summary: Navigator (Finnish: navigaattori) guided by conventions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/navigaattori
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/navigaattori
 Project-URL: Documentation, https://codes.dilettant.life/docs/navigaattori
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/navigaattori
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/navigaattori
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Navigaattori
 
 Navigator (Finnish: navigaattori) guided by conventions.
 
 [License: MIT](https://git.sr.ht/~sthagen/navigaattori/tree/default/item/LICENSE)
 
-Third party dependencies are documented in the folder [third-party](third-party/README.md).
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
 
 [![version](https://img.shields.io/pypi/v/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 [![downloads](https://pepy.tech/badge/navigaattori/month)](https://pepy.tech/project/navigaattori)
 [![wheel](https://img.shields.io/pypi/wheel/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 
 ## Documentation
 
 User and developer [documentation of navigaattori](https://codes.dilettant.life/docs/navigaattori).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of navigaattori](https://todo.sr.ht/~sthagen/navigaattori).
+Any feature requests or bug reports shall go to the [todos of navigaattori](https://todo.sr.ht/~sthagen/navigaattori).
 
 ## Primary Source repository
 
 The main source of `navigaattori` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `navigaattori` are:
 
 * [on codeberg](https://codeberg.org/sthagen/navigaattori) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/navigaattori) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 # Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `navigaattori-2023.1.17/navigaattori/__init__.py` & `navigaattori-2023.6.18/navigaattori/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime as dti
 import logging
 import os
 import pathlib
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.1.17+parent.aba76e74'
-# [[[end]]] (checksum: ff50b4b725c3faf4ef148ce697cd835a)
+__version__ = '2023.6.18+parent.ee0b6c1b'
+# [[[end]]] (checksum: 4089f19e8bc3ec7819aafb3b79ce17ba)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Navigator (Finnish: navigaattori) guided by conventions.'
 APP_ALIAS = 'navigaattori'
 APP_ENV = 'NAVIGAATTORI'
```

### Comparing `navigaattori-2023.1.17/navigaattori/approvals.py` & `navigaattori-2023.6.18/navigaattori/approvals.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/bind.py` & `navigaattori-2023.6.18/navigaattori/bind.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/changes.py` & `navigaattori-2023.6.18/navigaattori/changes.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/cli.py` & `navigaattori-2023.6.18/navigaattori/cli.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/eject.py` & `navigaattori-2023.6.18/navigaattori/eject.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/liitos_meta.py` & `navigaattori-2023.6.18/navigaattori/liitos_meta.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/meta.py` & `navigaattori-2023.6.18/navigaattori/meta.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/structures.py` & `navigaattori-2023.6.18/navigaattori/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     STRUCTURES_KEY,
     log,
     parse_csl,
 )
 from navigaattori.approvals import Approvals
 from navigaattori.bind import Binder
 from navigaattori.changes import Changes
+from navigaattori.layout import Layout
 from navigaattori.meta import Meta
 
 
 @no_type_check
 class Structures:
     """Model for structures as top level information to navigate all target types."""
 
@@ -145,19 +146,25 @@
                     for fk, fd in facet.items():
                         self.target_types[target_type]['structure'][target][fk] = copy.deepcopy(self.facet_block)
                         for efk in self.expected_facet_keys:
                             self.target_types[target_type]['structure'][target][fk][efk] = fd.get(efk)
                         for erfk in self.resource_keys:
                             erv = self.target_types[target_type]['structure'][target][fk][erfk]
                             if not erv or not (self.fs_root / spec['dir'] / erv).is_file():
-                                log.error(
-                                    f'  + invalid ({erfk}) resource ({erv}) for facet ({fk}) of target ({target})'
-                                    f' with target type ({target_type}) - resource does not exist or is no file'
-                                )
-                                self.target_types[target_type]['valid'] = False
+                                if erfk == 'layout':
+                                    log.info(
+                                        f'  + optional ({erfk}) resource is ({erv}) for facet ({fk}) of target ({target})'
+                                        f' with target type ({target_type}) - resource does not exist or is no file'
+                                    )
+                                else:
+                                    log.error(
+                                        f'  + invalid ({erfk}) resource ({erv}) for facet ({fk}) of target ({target})'
+                                        f' with target type ({target_type}) - resource does not exist or is no file'
+                                    )
+                                    self.target_types[target_type]['valid'] = False
                             else:
                                 if erfk == 'approvals':
                                     approvals_path = self.fs_root / self.target_types[target_type]['dir'] / erv
                                     log.info(f'assessing approvals ({approvals_path}) yielding:')
                                     code, details = self.assess_approvals(approvals_path)
                                     if code:
                                         self.target_types[target_type]['valid'] = False
@@ -169,14 +176,20 @@
                                         self.target_types[target_type]['valid'] = False
                                 elif erfk == 'changes':
                                     changes_path = self.fs_root / self.target_types[target_type]['dir'] / erv
                                     log.info(f'assessing changes ({changes_path}) yielding:')
                                     code, details = self.assess_changes(changes_path)
                                     if code:
                                         self.target_types[target_type]['valid'] = False
+                                elif erfk == 'layout':
+                                    layout_path = self.fs_root / self.target_types[target_type]['dir'] / erv
+                                    log.info(f'assessing layout ({layout_path}) yielding:')
+                                    code, details = self.assess_layout(layout_path)
+                                    if code:
+                                        self.target_types[target_type]['valid'] = False
                                 elif erfk == 'meta':
                                     meta_top_path = self.fs_root / self.target_types[target_type]['dir'] / erv
                                     log.info(f'assessing changes ({meta_top_path}) yielding:')
                                     code, details = self.assess_meta(meta_top_path)
                                     if code:
                                         self.target_types[target_type]['valid'] = False
 
@@ -204,14 +217,23 @@
         changes = Changes(changes_path, options=self._options)
         if changes.is_valid():
             return 0, changes.container()
 
         return changes.code_details()
 
     @no_type_check
+    def assess_layout(self, layout_path: str | pathlib.Path):
+        """Delegate the verification to an instance of the Layout class."""
+        layout = Layout(layout_path, options=self._options)
+        if layout.is_valid():
+            return 0, layout.container()
+
+        return layout.code_details()
+
+    @no_type_check
     def assess_meta(self, meta_top_path: str | pathlib.Path):
         """Delegate the verification to an instance of the Meta class."""
         meta = Meta(meta_top_path, options=self._options)
         if meta.is_valid():
             return 0, meta.container()
 
         return meta.code_details()
@@ -303,14 +325,15 @@
         self.structures = {}
         self.target_types = {}
 
         self.facet_block = {
             'approvals': '',  # resource pointer to fs
             'bind': '',  # resource pointer to fs
             'changes': '',  # resource pointer to fs
+            'layout': '',  # resource pointer to fs
             'meta': '',  # resource pointer to fs
             'render': True,
             'formats': [],
             'options': {},
         }
         self.expected_facet_keys = list(self.facet_block)
         self.resource_keys = self.expected_facet_keys[:4]
```

### Comparing `navigaattori-2023.1.17/navigaattori/template_loader.py` & `navigaattori-2023.6.18/navigaattori/template_loader.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori/templates/liitos_vocabulary.yml` & `navigaattori-2023.6.18/navigaattori/templates/liitos_vocabulary.yml`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/navigaattori.egg-info/PKG-INFO` & `navigaattori-2023.6.18/navigaattori.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 Metadata-Version: 2.1
 Name: navigaattori
-Version: 2023.1.17
+Version: 2023.6.18
 Summary: Navigator (Finnish: navigaattori) guided by conventions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/navigaattori
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/navigaattori
 Project-URL: Documentation, https://codes.dilettant.life/docs/navigaattori
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/navigaattori
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/navigaattori
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Navigaattori
 
 Navigator (Finnish: navigaattori) guided by conventions.
 
 [License: MIT](https://git.sr.ht/~sthagen/navigaattori/tree/default/item/LICENSE)
 
-Third party dependencies are documented in the folder [third-party](third-party/README.md).
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
 
 [![version](https://img.shields.io/pypi/v/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 [![downloads](https://pepy.tech/badge/navigaattori/month)](https://pepy.tech/project/navigaattori)
 [![wheel](https://img.shields.io/pypi/wheel/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/navigaattori.svg?style=flat)](https://pypi.python.org/pypi/navigaattori/)
 
 ## Documentation
 
 User and developer [documentation of navigaattori](https://codes.dilettant.life/docs/navigaattori).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of navigaattori](https://todo.sr.ht/~sthagen/navigaattori).
+Any feature requests or bug reports shall go to the [todos of navigaattori](https://todo.sr.ht/~sthagen/navigaattori).
 
 ## Primary Source repository
 
 The main source of `navigaattori` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `navigaattori` are:
 
 * [on codeberg](https://codeberg.org/sthagen/navigaattori) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/navigaattori) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 # Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `navigaattori-2023.1.17/navigaattori.egg-info/SOURCES.txt` & `navigaattori-2023.6.18/navigaattori.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 navigaattori/api.py
 navigaattori/approvals.py
 navigaattori/bind.py
 navigaattori/changes.py
 navigaattori/cli.py
 navigaattori/eject.py
 navigaattori/fs.py
+navigaattori/layout.py
 navigaattori/liitos_meta.py
 navigaattori/meta.py
 navigaattori/structures.py
 navigaattori/template_loader.py
 navigaattori/vcs.py
 navigaattori.egg-info/PKG-INFO
 navigaattori.egg-info/SOURCES.txt
@@ -26,10 +27,11 @@
 test/test_api.py
 test/test_approvals.py
 test/test_bind.py
 test/test_changes.py
 test/test_cli.py
 test/test_eject.py
 test/test_fs.py
+test/test_layout.py
 test/test_meta.py
 test/test_template_loader.py
 test/test_vcs.py
```

### Comparing `navigaattori-2023.1.17/pyproject.toml` & `navigaattori-2023.6.18/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "navigaattori"
-version = "2023.1.17"
+version = "2023.6.18"
 description = "Navigator (Finnish: navigaattori) guided by conventions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 keywords = ["developer-tools", "validation", "verification"]
 dependencies = [
     "PyYAML >= 6.0",
     "foran >= 2022.12.7",
     "taksonomia >= 2022.12.7",
     "treelib >= 1.6.1",
@@ -42,15 +43,15 @@
 [tool.setuptools.packages.find]
 include = ["navigaattori", "navigaattori.templates", "example"]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py310", "py311"]
+target-version = ["py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
```

### Comparing `navigaattori-2023.1.17/test/test_api.py` & `navigaattori-2023.6.18/test/test_api.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_approvals.py` & `navigaattori-2023.6.18/test/test_approvals.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_bind.py` & `navigaattori-2023.6.18/test/test_bind.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_changes.py` & `navigaattori-2023.6.18/test/test_changes.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_cli.py` & `navigaattori-2023.6.18/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_eject.py` & `navigaattori-2023.6.18/test/test_eject.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_meta.py` & `navigaattori-2023.6.18/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `navigaattori-2023.1.17/test/test_template_loader.py` & `navigaattori-2023.6.18/test/test_template_loader.py`

 * *Files identical despite different names*

