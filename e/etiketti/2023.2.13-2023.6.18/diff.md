# Comparing `tmp/etiketti-2023.2.13.tar.gz` & `tmp/etiketti-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etiketti-2023.2.13.tar", last modified: Mon Feb 13 21:10:30 2023, max compression
+gzip compressed data, was "etiketti-2023.6.18.tar", last modified: Sun Jun 18 12:41:25 2023, max compression
```

## Comparing `etiketti-2023.2.13.tar` & `etiketti-2023.6.18.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-13 21:10:30.028756 etiketti-2023.2.13/
--rw-r--r--   0 ruth       (501) staff       (20)    16725 2023-01-22 07:52:51.000000 etiketti-2023.2.13/LICENSE.txt
--rw-r--r--   0 ruth       (501) staff       (20)       63 2023-01-22 18:17:49.000000 etiketti-2023.2.13/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2738 2023-02-13 21:10:30.028533 etiketti-2023.2.13/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1748 2023-01-22 12:26:55.000000 etiketti-2023.2.13/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-13 21:10:30.008539 etiketti-2023.2.13/etiketti/
--rw-r--r--   0 ruth       (501) staff       (20)     2990 2023-02-13 21:08:34.000000 etiketti-2023.2.13/etiketti/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      121 2023-01-22 13:37:54.000000 etiketti-2023.2.13/etiketti/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     2959 2023-01-24 22:02:03.000000 etiketti-2023.2.13/etiketti/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     3763 2023-02-13 20:30:33.000000 etiketti-2023.2.13/etiketti/discover.py
--rw-r--r--   0 ruth       (501) staff       (20)    10128 2023-01-24 21:38:38.000000 etiketti-2023.2.13/etiketti/implementation.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-13 21:10:30.010405 etiketti-2023.2.13/etiketti.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2738 2023-02-13 21:10:29.000000 etiketti-2023.2.13/etiketti.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      461 2023-02-13 21:10:30.000000 etiketti-2023.2.13/etiketti.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-02-13 21:10:29.000000 etiketti-2023.2.13/etiketti.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       46 2023-02-13 21:10:30.000000 etiketti-2023.2.13/etiketti.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      150 2023-02-13 21:10:30.000000 etiketti-2023.2.13/etiketti.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       17 2023-02-13 21:10:30.000000 etiketti-2023.2.13/etiketti.egg-info/top_level.txt
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-13 21:10:30.015726 etiketti-2023.2.13/example/
--rw-r--r--   0 ruth       (501) staff       (20)      465 2023-01-22 16:58:09.000000 etiketti-2023.2.13/example/etiketti.yml
--rw-r--r--   0 ruth       (501) staff       (20)     3474 2023-01-29 14:56:36.000000 etiketti-2023.2.13/example/label_per_env.py
--rw-r--r--   0 ruth       (501) staff       (20)     2653 2023-02-13 20:06:59.000000 etiketti-2023.2.13/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-02-13 21:10:30.028852 etiketti-2023.2.13/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-13 21:10:30.028053 etiketti-2023.2.13/test/
--rw-r--r--   0 ruth       (501) staff       (20)     2433 2023-01-22 16:13:37.000000 etiketti-2023.2.13/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      133 2023-01-22 15:21:51.000000 etiketti-2023.2.13/test/test_discover.py
--rw-r--r--   0 ruth       (501) staff       (20)      126 2023-01-22 15:23:43.000000 etiketti-2023.2.13/test/test_implementation.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 12:41:25.604668 etiketti-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)    16725 2023-01-22 07:52:51.000000 etiketti-2023.6.18/LICENSE.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       63 2023-01-22 18:17:49.000000 etiketti-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3234 2023-06-18 12:41:25.604518 etiketti-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2193 2023-03-14 22:17:43.000000 etiketti-2023.6.18/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 12:41:25.599859 etiketti-2023.6.18/etiketti/
+-rw-r--r--   0 ruth       (501) staff       (20)     2990 2023-06-18 12:40:12.000000 etiketti-2023.6.18/etiketti/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      121 2023-01-22 13:37:54.000000 etiketti-2023.6.18/etiketti/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2959 2023-01-24 22:02:03.000000 etiketti-2023.6.18/etiketti/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3763 2023-02-13 20:30:33.000000 etiketti-2023.6.18/etiketti/discover.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10128 2023-01-24 21:38:38.000000 etiketti-2023.6.18/etiketti/implementation.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 12:41:25.601852 etiketti-2023.6.18/etiketti.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3234 2023-06-18 12:41:25.000000 etiketti-2023.6.18/etiketti.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      461 2023-06-18 12:41:25.000000 etiketti-2023.6.18/etiketti.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 12:41:25.000000 etiketti-2023.6.18/etiketti.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       46 2023-06-18 12:41:25.000000 etiketti-2023.6.18/etiketti.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      150 2023-06-18 12:41:25.000000 etiketti-2023.6.18/etiketti.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       17 2023-06-18 12:41:25.000000 etiketti-2023.6.18/etiketti.egg-info/top_level.txt
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 12:41:25.603674 etiketti-2023.6.18/example/
+-rw-r--r--   0 ruth       (501) staff       (20)      465 2023-01-22 16:58:09.000000 etiketti-2023.6.18/example/etiketti.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     3474 2023-01-29 14:56:36.000000 etiketti-2023.6.18/example/label_per_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2708 2023-06-18 12:32:37.000000 etiketti-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 12:41:25.604702 etiketti-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 12:41:25.604360 etiketti-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     2433 2023-01-22 16:13:37.000000 etiketti-2023.6.18/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      176 2023-06-18 12:27:45.000000 etiketti-2023.6.18/test/test_discover.py
+-rw-r--r--   0 ruth       (501) staff       (20)      126 2023-01-22 15:23:43.000000 etiketti-2023.6.18/test/test_implementation.py
```

### Comparing `etiketti-2023.2.13/LICENSE.txt` & `etiketti-2023.6.18/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etiketti-2023.2.13/PKG-INFO` & `etiketti-2023.6.18/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: etiketti
-Version: 2023.2.13
+Version: 2023.6.18
 Summary: Label (Finnish: etiketti) some files.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/etiketti
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/etiketti
 Project-URL: Documentation, https://codes.dilettant.life/docs/etiketti
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/etiketti
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/etiketti
 Keywords: developer-tools,devops
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Etiketti
@@ -37,25 +38,32 @@
 
 ## Documentation
 
 User and developer [documentation of etiketti](https://codes.dilettant.life/docs/etiketti).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of etiketti](https://todo.sr.ht/~sthagen/etiketti).
+Any feature requests or bug reports shall go to the [todos of etiketti](https://todo.sr.ht/~sthagen/etiketti).
 
 ## Primary Source repository
 
 The main source of `etiketti` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `etiketti` are:
 
 * [on codeberg](https://codeberg.org/sthagen/etiketti) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/etiketti) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Prototype.
 
 **Note**: The default branch is `default`.
```

### Comparing `etiketti-2023.2.13/etiketti/__init__.py` & `etiketti-2023.6.18/etiketti/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime as dti
 import logging
 import os
 import pathlib
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.2.13+parent.cd198833'
-# [[[end]]] (checksum: a19ffa32f34381baba216ee9e3708c31)
+__version__ = '2023.6.18+parent.afcce607'
+# [[[end]]] (checksum: be909842e14d8573ac8454995a209ee4)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Label (Finnish: etiketti) some files.'
 APP_ALIAS = 'etiketti'
 APP_ENV = 'ETIKETTI'
```

### Comparing `etiketti-2023.2.13/etiketti/cli.py` & `etiketti-2023.6.18/etiketti/cli.py`

 * *Files identical despite different names*

### Comparing `etiketti-2023.2.13/etiketti/discover.py` & `etiketti-2023.6.18/etiketti/discover.py`

 * *Files identical despite different names*

### Comparing `etiketti-2023.2.13/etiketti/implementation.py` & `etiketti-2023.6.18/etiketti/implementation.py`

 * *Files identical despite different names*

### Comparing `etiketti-2023.2.13/etiketti.egg-info/PKG-INFO` & `etiketti-2023.6.18/etiketti.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: etiketti
-Version: 2023.2.13
+Version: 2023.6.18
 Summary: Label (Finnish: etiketti) some files.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/etiketti
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/etiketti
 Project-URL: Documentation, https://codes.dilettant.life/docs/etiketti
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/etiketti
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/etiketti
 Keywords: developer-tools,devops
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Etiketti
@@ -37,25 +38,32 @@
 
 ## Documentation
 
 User and developer [documentation of etiketti](https://codes.dilettant.life/docs/etiketti).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of etiketti](https://todo.sr.ht/~sthagen/etiketti).
+Any feature requests or bug reports shall go to the [todos of etiketti](https://todo.sr.ht/~sthagen/etiketti).
 
 ## Primary Source repository
 
 The main source of `etiketti` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `etiketti` are:
 
 * [on codeberg](https://codeberg.org/sthagen/etiketti) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/etiketti) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Status
 
 Prototype.
 
 **Note**: The default branch is `default`.
```

### Comparing `etiketti-2023.2.13/example/label_per_env.py` & `etiketti-2023.6.18/example/label_per_env.py`

 * *Files identical despite different names*

### Comparing `etiketti-2023.2.13/pyproject.toml` & `etiketti-2023.6.18/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "etiketti"
-version = "2023.2.13"
+version = "2023.6.18"
 description = "Label (Finnish: etiketti) some files."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "devops"]
 dependencies = [
     "PyYAML >= 6.0",
-    "liitos >= 2023.1.21",
-    "navigaattori >= 2023.1.17",
+    "liitos >= 2023.6.17",
+    "navigaattori >= 2023.6.18",
     "pikepdf >= 6.2.8.post1",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
 
@@ -42,15 +43,15 @@
 [tool.setuptools.packages.find]
 include = ["etiketti", "example"]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py39", "py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
```

### Comparing `etiketti-2023.2.13/test/test_cli.py` & `etiketti-2023.6.18/test/test_cli.py`

 * *Files identical despite different names*

