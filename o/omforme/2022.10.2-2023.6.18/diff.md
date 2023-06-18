# Comparing `tmp/omforme-2022.10.2.tar.gz` & `tmp/omforme-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omforme-2022.10.2.tar", last modified: Sun Oct  2 15:17:15 2022, max compression
+gzip compressed data, was "omforme-2023.6.18.tar", last modified: Sun Jun 18 19:44:37 2023, max compression
```

## Comparing `omforme-2022.10.2.tar` & `omforme-2023.6.18.tar`

### file list

```diff
@@ -1,53 +1,21 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-10-02 15:17:15.285809 omforme-2022.10.2/
--rw-r--r--   0 ruth       (501) staff       (20)     1161 2022-04-30 21:02:24.000000 omforme-2022.10.2/.editorconfig
--rw-r--r--   0 ruth       (501) staff       (20)       19 2022-06-18 09:14:29.000000 omforme-2022.10.2/.gitattributes
--rw-r--r--   0 ruth       (501) staff       (20)     1897 2022-10-02 14:37:49.000000 omforme-2022.10.2/.gitignore
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2022-05-04 18:45:52.000000 omforme-2022.10.2/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)     2098 2022-10-02 13:48:23.000000 omforme-2022.10.2/Makefile
--rw-r--r--   0 ruth       (501) staff       (20)     2511 2022-10-02 15:17:15.285930 omforme-2022.10.2/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1559 2022-10-02 13:58:37.000000 omforme-2022.10.2/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     1698 2022-10-02 14:36:21.000000 omforme-2022.10.2/baseline-bandit.json
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-10-02 15:17:15.272501 omforme-2022.10.2/docs/
--rw-r--r--   0 ruth       (501) staff       (20)      708 2022-10-02 15:14:01.000000 omforme-2022.10.2/docs/api.md
--rw-r--r--   0 ruth       (501) staff       (20)       53 2022-10-02 13:54:39.000000 omforme-2022.10.2/docs/changes.md
--rw-r--r--   0 ruth       (501) staff       (20)     1380 2022-10-02 13:55:27.000000 omforme-2022.10.2/docs/index.md
--rw-r--r--   0 ruth       (501) staff       (20)      235 2022-10-02 13:56:21.000000 omforme-2022.10.2/docs/install.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-10-02 15:17:15.276809 omforme-2022.10.2/docs/third-party/
--rw-r--r--   0 ruth       (501) staff       (20)     2574 2022-10-02 15:04:05.000000 omforme-2022.10.2/docs/third-party/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     3559 2022-10-02 15:03:59.000000 omforme-2022.10.2/docs/third-party/all-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)     1603 2022-10-02 15:03:58.000000 omforme-2022.10.2/docs/third-party/direct-dependency-licenses.json
--rw-r--r--   0 ruth       (501) staff       (20)       67 2022-10-02 15:04:05.000000 omforme-2022.10.2/docs/third-party/package-dependency-tree.console.txt
--rw-r--r--   0 ruth       (501) staff       (20)      112 2022-10-02 15:04:00.000000 omforme-2022.10.2/docs/third-party/package-dependency-tree.dot.txt
--rw-r--r--   0 ruth       (501) staff       (20)      419 2022-10-02 15:04:04.000000 omforme-2022.10.2/docs/third-party/package-dependency-tree.json
--rw-r--r--   0 ruth       (501) staff       (20)     1705 2022-10-02 15:04:02.000000 omforme-2022.10.2/docs/third-party/package-dependency-tree.svg
--rw-r--r--   0 ruth       (501) staff       (20)     1303 2022-10-02 15:14:14.000000 omforme-2022.10.2/docs/usage.md
--rwxr-xr-x   0 ruth       (501) staff       (20)      240 2022-02-27 12:03:21.000000 omforme-2022.10.2/gen-sbom
--rw-r--r--   0 ruth       (501) staff       (20)     5809 2022-10-02 15:03:29.000000 omforme-2022.10.2/gen_licenses.py
--rw-r--r--   0 ruth       (501) staff       (20)      599 2022-07-28 15:11:55.000000 omforme-2022.10.2/gen_sbom.py
--rw-r--r--   0 ruth       (501) staff       (20)     1109 2022-08-21 21:41:20.000000 omforme-2022.10.2/gen_version.py
--rw-r--r--   0 ruth       (501) staff       (20)     1340 2022-10-02 15:01:53.000000 omforme-2022.10.2/mkdocs.yml
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-10-02 15:17:15.279203 omforme-2022.10.2/omforme/
--rw-r--r--   0 ruth       (501) staff       (20)     1960 2022-10-02 14:06:54.000000 omforme-2022.10.2/omforme/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      122 2022-10-02 14:07:28.000000 omforme-2022.10.2/omforme/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1353 2022-10-02 14:08:19.000000 omforme-2022.10.2/omforme/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     2807 2022-10-02 14:09:51.000000 omforme-2022.10.2/omforme/omforme.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-10-02 15:17:15.282419 omforme-2022.10.2/omforme.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2511 2022-10-02 15:17:15.000000 omforme-2022.10.2/omforme.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      996 2022-10-02 15:17:15.000000 omforme-2022.10.2/omforme.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-10-02 15:17:15.000000 omforme-2022.10.2/omforme.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       45 2022-10-02 15:17:15.000000 omforme-2022.10.2/omforme.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)       90 2022-10-02 15:17:15.000000 omforme-2022.10.2/omforme.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        8 2022-10-02 15:17:15.000000 omforme-2022.10.2/omforme.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1920 2022-10-02 13:59:19.000000 omforme-2022.10.2/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       13 2022-10-02 13:57:32.000000 omforme-2022.10.2/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)     1941 2022-10-02 15:03:57.000000 omforme-2022.10.2/sbom.json
--rw-r--r--   0 ruth       (501) staff       (20)       65 2022-10-02 15:03:57.000000 omforme-2022.10.2/sbom.json.sha256
--rw-r--r--   0 ruth       (501) staff       (20)      153 2022-10-02 15:17:15.287548 omforme-2022.10.2/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2021-11-13 11:35:55.000000 omforme-2022.10.2/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-10-02 15:17:15.285590 omforme-2022.10.2/test/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-05-12 17:00:52.000000 omforme-2022.10.2/test/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2021-05-12 17:00:55.000000 omforme-2022.10.2/test/context.py
--rw-r--r--   0 ruth       (501) staff       (20)      788 2022-09-30 20:01:38.000000 omforme-2022.10.2/test/requirements-dev.txt
--rw-r--r--   0 ruth       (501) staff       (20)      725 2022-09-30 14:43:59.000000 omforme-2022.10.2/test/requirements.txt
--rw-r--r--   0 ruth       (501) staff       (20)      825 2022-10-02 14:36:13.000000 omforme-2022.10.2/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      367 2022-10-02 14:29:23.000000 omforme-2022.10.2/test/test_omforme.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:44:37.501699 omforme-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 omforme-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)     3080 2023-06-18 19:44:37.501569 omforme-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2076 2023-03-14 22:32:59.000000 omforme-2023.6.18/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:44:37.499217 omforme-2023.6.18/omforme/
+-rw-r--r--   0 ruth       (501) staff       (20)     1960 2023-06-18 19:43:04.000000 omforme-2023.6.18/omforme/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      122 2022-10-02 14:07:28.000000 omforme-2023.6.18/omforme/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1353 2022-10-02 14:08:19.000000 omforme-2023.6.18/omforme/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2878 2022-12-28 18:13:21.000000 omforme-2023.6.18/omforme/omforme.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:44:37.501004 omforme-2023.6.18/omforme.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3080 2023-06-18 19:44:37.000000 omforme-2023.6.18/omforme.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      332 2023-06-18 19:44:37.000000 omforme-2023.6.18/omforme.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 19:44:37.000000 omforme-2023.6.18/omforme.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       45 2023-06-18 19:44:37.000000 omforme-2023.6.18/omforme.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       88 2023-06-18 19:44:37.000000 omforme-2023.6.18/omforme.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        8 2023-06-18 19:44:37.000000 omforme-2023.6.18/omforme.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2572 2023-06-18 19:33:59.000000 omforme-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 19:44:37.501732 omforme-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 19:44:37.501413 omforme-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      825 2022-10-02 14:36:13.000000 omforme-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      367 2022-10-02 14:29:23.000000 omforme-2023.6.18/test/test_omforme.py
```

### Comparing `omforme-2022.10.2/LICENSE` & `omforme-2023.6.18/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Stefan Hagen
+Copyright (c) 2023 Stefan Hagen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `omforme-2022.10.2/PKG-INFO` & `omforme-2023.6.18/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 Metadata-Version: 2.1
 Name: omforme
-Version: 2022.10.2
+Version: 2023.6.18
 Summary: Reshape (Danish: omforme).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/omforme
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/omforme
 Project-URL: Documentation, https://codes.dilettant.life/docs/omforme
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/omforme
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/omforme
 Keywords: developer-tools,data-processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Omforme
 
 Reshape (Danish: omforme). 
 
 [License: MIT](https://git.sr.ht/~sthagen/omforme/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 [![downloads](https://pepy.tech/badge/omforme/month)](https://pepy.tech/project/omforme)
 [![wheel](https://img.shields.io/pypi/wheel/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 
 ## Documentation
 
 User and developer [documentation of omforme](https://codes.dilettant.life/docs/omforme).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of omforme](https://todo.sr.ht/~sthagen/omforme).
+Any feature requests or bug reports shall go to the [todos of omforme](https://todo.sr.ht/~sthagen/omforme).
 
 ## Primary Source repository
 
-The primary source of `omforme` lives somewhere on a mountain in Central Switzerland.
-But, we use decentralized version control (git), so any clone can become the source to everyone's benefit, no central only code.
-Anyway, the preferred public clones of `omforme` are:
+The main source of `omforme` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `omforme` are:
 
 * [on codeberg](https://codeberg.org/sthagen/omforme) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/omforme) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `omforme-2022.10.2/omforme/__init__.py` & `omforme-2023.6.18/omforme/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime as dti
 import logging
 import os
 import pathlib
 from typing import no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2022.10.2+parent.e8735f64'
-# [[[end]]] (checksum: 8ed2e7e93655a22c692ab7fce30e0ec8)
+__version__ = '2023.6.18+parent.d616e4ac'
+# [[[end]]] (checksum: 28766419b9118cb56ee687dec300d5d8)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 __all__: list[str] = []
 
 APP_ALIAS = 'omforme'
 APP_ENV = 'OMFORME'
```

### Comparing `omforme-2022.10.2/omforme/cli.py` & `omforme-2023.6.18/omforme/cli.py`

 * *Files identical despite different names*

### Comparing `omforme-2022.10.2/omforme/omforme.py` & `omforme-2023.6.18/omforme/omforme.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ('b', 'ignore', <function <lambda> at 0x...>),
     ('d', 'collect', ['1', '2', '3']),
     ('e', 'return', <function <lambda> at 0x...>)
 )
 
 """
 import argparse
+from typing import no_type_check
 
 from omforme import DEBUG, ENCODING, ENCODING_ERRORS_POLICY, log
 
 
 class Omforme:
     """Provide a generator borrowing consumer that returns the transform applying playbook to the stream.
 
@@ -54,18 +55,20 @@
     1 3 e d collect ['1', '2', '3'] e
     >>> transform[1]
     ('d', 'collect', ['1', '2', '3'])
     >>>
 
     """
 
+    @no_type_check
     def __init__(self, playbook):
         """Later alligator."""
         self.playbook = playbook
 
+    @no_type_check
     def __call__(self, gen):
         """Apply transform to generator stream of events."""
         phase = 0
         trigger, what, where_to = self.playbook[phase]
         peek = self.playbook[phase + 1][0]
         stop = len(self.playbook)
         for data in gen:
```

### Comparing `omforme-2022.10.2/omforme.egg-info/PKG-INFO` & `omforme-2023.6.18/omforme.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 Metadata-Version: 2.1
 Name: omforme
-Version: 2022.10.2
+Version: 2023.6.18
 Summary: Reshape (Danish: omforme).
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/omforme
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/omforme
 Project-URL: Documentation, https://codes.dilettant.life/docs/omforme
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/omforme
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/omforme
 Keywords: developer-tools,data-processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Omforme
 
 Reshape (Danish: omforme). 
 
 [License: MIT](https://git.sr.ht/~sthagen/omforme/tree/default/item/LICENSE)
 
+Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
+
 [![version](https://img.shields.io/pypi/v/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 [![downloads](https://pepy.tech/badge/omforme/month)](https://pepy.tech/project/omforme)
 [![wheel](https://img.shields.io/pypi/wheel/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 [![supported-versions](https://img.shields.io/pypi/pyversions/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 [![supported-implementations](https://img.shields.io/pypi/implementation/omforme.svg?style=flat)](https://pypi.python.org/pypi/omforme/)
 
 ## Documentation
 
 User and developer [documentation of omforme](https://codes.dilettant.life/docs/omforme).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of omforme](https://todo.sr.ht/~sthagen/omforme).
+Any feature requests or bug reports shall go to the [todos of omforme](https://todo.sr.ht/~sthagen/omforme).
 
 ## Primary Source repository
 
-The primary source of `omforme` lives somewhere on a mountain in Central Switzerland.
-But, we use decentralized version control (git), so any clone can become the source to everyone's benefit, no central only code.
-Anyway, the preferred public clones of `omforme` are:
+The main source of `omforme` is on a mountain in central Switzerland.
+We use distributed version control (git).
+There is no central hub.
+Every clone can become a new source for the benefit of all.
+The preferred public clones of `omforme` are:
 
 * [on codeberg](https://codeberg.org/sthagen/omforme) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/omforme) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Experimental.
 
 **Note**: The default branch is `default`.
```

### Comparing `omforme-2022.10.2/pyproject.toml` & `omforme-2023.6.18/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "omforme"
-version = "2022.10.2"
+version = "2023.6.18"
 description = "Reshape (Danish: omforme)."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "data-processing"]
 dependencies = [
-    "typer >= 0.6.1",
+    "typer >= 0.9.0",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["black", "coverage", "flake8", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8"]
+dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
 
 [project.urls]
 Homepage = "https://git.sr.ht/~sthagen/omforme"
 Bug-Tracker = "https://todo.sr.ht/~sthagen/omforme"
 Documentation = "https://codes.dilettant.life/docs/omforme"
 Source-Code = "https://git.sr.ht/~sthagen/omforme"
 Test-Coverage = "https://codes.dilettant.life/coverage/omforme"
@@ -36,21 +37,18 @@
 [project.scripts]
 omforme = "omforme.cli:main"
 
 [tool.setuptools.packages.find]
 include = ["omforme"]
 exclude = ["test*"]
 
-[bdist_wheel]
-universal = true
-
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py38", "py39", "py310"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
@@ -59,21 +57,59 @@
     "if TYPE_CHECKING:",
     "@overload",
 ]
 omit = [
     "*/__main__.py",
 ]
 
-[tool.isort]
-line_length = 120
-known_first_party = "omforme"
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
+[tool.ruff]
+line-length = 120
+select = ["E", "F", "Q"]
+ignore = []
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+target-version = "py310"
+unfixable = ["F401"]
+
+[tool.ruff.flake8-quotes]
+docstring-quotes = "double"
+inline-quotes = "single"
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["E402"]
+
+[tool.ruff.flake8-import-conventions.aliases]
+altair = "alt"
+"matplotlib.pyplot" = "plt"
+numpy = "np"
+pandas = "pd"
+seaborn = "sns"
+
+[tool.ruff.mccabe]
+max-complexity = 42  # default is 10
 
 [tool.mypy]
 strict = true
 implicit_reexport = true
 
 [tool.pytest]
 testpaths = "test"
```

### Comparing `omforme-2022.10.2/test/test_cli.py` & `omforme-2023.6.18/test/test_cli.py`

 * *Files identical despite different names*

