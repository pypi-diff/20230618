# Comparing `tmp/paikalta-2023.2.23.tar.gz` & `tmp/paikalta-2023.6.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paikalta-2023.2.23.tar", last modified: Thu Feb 23 23:15:17 2023, max compression
+gzip compressed data, was "paikalta-2023.6.18.tar", last modified: Sun Jun 18 21:29:42 2023, max compression
```

## Comparing `paikalta-2023.2.23.tar` & `paikalta-2023.6.18.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-23 23:15:17.259349 paikalta-2023.2.23/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-02-10 18:30:51.000000 paikalta-2023.2.23/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2023-02-10 19:43:36.000000 paikalta-2023.2.23/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3072 2023-02-23 23:15:17.259172 paikalta-2023.2.23/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2094 2023-02-10 19:15:18.000000 paikalta-2023.2.23/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-23 23:15:17.255619 paikalta-2023.2.23/paikalta/
--rw-r--r--   0 ruth       (501) staff       (20)     2704 2023-02-23 23:12:40.000000 paikalta-2023.2.23/paikalta/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      121 2023-02-10 19:37:52.000000 paikalta-2023.2.23/paikalta/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     2773 2023-02-23 23:02:22.000000 paikalta-2023.2.23/paikalta/api.py
--rw-r--r--   0 ruth       (501) staff       (20)     2147 2023-02-23 23:00:28.000000 paikalta-2023.2.23/paikalta/cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-23 23:15:17.257508 paikalta-2023.2.23/paikalta.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3072 2023-02-23 23:15:17.000000 paikalta-2023.2.23/paikalta.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      346 2023-02-23 23:15:17.000000 paikalta-2023.2.23/paikalta.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-02-23 23:15:17.000000 paikalta-2023.2.23/paikalta.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       46 2023-02-23 23:15:17.000000 paikalta-2023.2.23/paikalta.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)       91 2023-02-23 23:15:17.000000 paikalta-2023.2.23/paikalta.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        9 2023-02-23 23:15:17.000000 paikalta-2023.2.23/paikalta.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2562 2023-02-23 22:52:47.000000 paikalta-2023.2.23/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-02-23 23:15:17.259397 paikalta-2023.2.23/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-02-23 23:15:17.258766 paikalta-2023.2.23/test/
--rw-r--r--   0 ruth       (501) staff       (20)     1508 2023-02-11 15:22:28.000000 paikalta-2023.2.23/test/test_api.py
--rw-r--r--   0 ruth       (501) staff       (20)     1573 2023-02-23 23:05:10.000000 paikalta-2023.2.23/test/test_cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 21:29:42.846722 paikalta-2023.6.18/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-02-10 18:30:51.000000 paikalta-2023.6.18/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2023-02-10 19:43:36.000000 paikalta-2023.6.18/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3568 2023-06-18 21:29:42.846567 paikalta-2023.6.18/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2539 2023-03-14 22:33:31.000000 paikalta-2023.6.18/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 21:29:42.843358 paikalta-2023.6.18/paikalta/
+-rw-r--r--   0 ruth       (501) staff       (20)     2719 2023-06-18 21:26:29.000000 paikalta-2023.6.18/paikalta/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      121 2023-02-10 19:37:52.000000 paikalta-2023.6.18/paikalta/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2662 2023-06-18 20:46:03.000000 paikalta-2023.6.18/paikalta/api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1960 2023-06-18 20:47:34.000000 paikalta-2023.6.18/paikalta/cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 21:29:42.844980 paikalta-2023.6.18/paikalta.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3568 2023-06-18 21:29:42.000000 paikalta-2023.6.18/paikalta.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      346 2023-06-18 21:29:42.000000 paikalta-2023.6.18/paikalta.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-18 21:29:42.000000 paikalta-2023.6.18/paikalta.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       46 2023-06-18 21:29:42.000000 paikalta-2023.6.18/paikalta.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       91 2023-06-18 21:29:42.000000 paikalta-2023.6.18/paikalta.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        9 2023-06-18 21:29:42.000000 paikalta-2023.6.18/paikalta.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2617 2023-06-18 20:52:18.000000 paikalta-2023.6.18/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-18 21:29:42.846761 paikalta-2023.6.18/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-18 21:29:42.846220 paikalta-2023.6.18/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     1508 2023-02-11 15:22:28.000000 paikalta-2023.6.18/test/test_api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1574 2023-06-18 20:47:36.000000 paikalta-2023.6.18/test/test_cli.py
```

### Comparing `paikalta-2023.2.23/LICENSE` & `paikalta-2023.6.18/LICENSE`

 * *Files identical despite different names*

### Comparing `paikalta-2023.2.23/PKG-INFO` & `paikalta-2023.6.18/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: paikalta
-Version: 2023.2.23
-Summary: From the place (Finnish: paikalta) we derive the name.
-Author-email: Stefan Hagen <stefan@hagen.link>
-Maintainer-email: Stefan Hagen <stefan@hagen.link>
-Project-URL: Homepage, https://git.sr.ht/~sthagen/paikalta
-Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/paikalta
-Project-URL: Documentation, https://codes.dilettant.life/docs/paikalta
-Project-URL: Source-Code, https://git.sr.ht/~sthagen/paikalta
-Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/paikalta
-Keywords: developer-tools,devops
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Paikalta
 
 From the place (Finnish: paikalta) we derive the name.
 
 [License: MIT](https://git.sr.ht/~sthagen/paikalta/tree/default/item/LICENSE)
 
 Third party dependencies are documented in the folder [third-party](docs/third-party/README.md).
@@ -37,27 +14,34 @@
 
 ## Documentation
 
 User and developer [documentation of paikalta](https://codes.dilettant.life/docs/paikalta).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of paikalta](https://todo.sr.ht/~sthagen/paikalta).
+Any feature requests or bug reports shall go to the [todos of paikalta](https://todo.sr.ht/~sthagen/paikalta).
 
 ## Primary Source repository
 
 The main source of `paikalta` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `paikalta` are:
 
 * [on codeberg](https://codeberg.org/sthagen/paikalta) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/paikalta) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Acknowledgements
 
 [Thomas Schmidt](https://github.com/tschmidtb51) provided the original source code as
 script [`check.py`](https://github.com/oasis-tcs/csaf/blob/master/csaf_2.0/test/filenames/check.py) and
 test cases in `test/fixtures/upstream/` as contributions to the OASIS CSAF TC repository
 below [/csaf_2.0/test/filenames/data](https://github.com/oasis-tcs/csaf/tree/master/csaf_2.0/test/filenames/data).
```

### Comparing `paikalta-2023.2.23/paikalta/__init__.py` & `paikalta-2023.6.18/paikalta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime as dti
 import logging
 import os
 import pathlib
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.2.23+parent.65d2e3ef'
-# [[[end]]] (checksum: a6710d66205faeeec5b3840d22b89f91)
+__version__ = '2023.6.18+parent.65b57909'
+# [[[end]]] (checksum: 8dab14bac1372382ee45751b9d630a91)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'From the place (Finnish: paikalta) we derive the name.'
 APP_ALIAS = 'paikalta'
 APP_ENV = 'PAIKALTA'
@@ -56,14 +56,15 @@
 
 
 def parse_csl(csl: str) -> List[str]:
     """DRY."""
     return [fmt.strip().lower() for fmt in csl.split(COMMA) if fmt.strip()]
 
 
+@no_type_check
 def parse_csl_as_is(csl: str) -> List[str]:
     """DRY."""
     return tuple(fmt.strip() for fmt in csl.split(COMMA) if fmt.strip())[:2]
 
 
 @no_type_check
 def formatTime_RFC3339(self, record, datefmt=None):  # noqa
```

### Comparing `paikalta-2023.2.23/paikalta/api.py` & `paikalta-2023.6.18/paikalta/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 """From the place (Finnish: paikalta) we derive the name - application programming interface."""
 import argparse
 import pathlib
 import re
-import sys
-from typing import List, Union, no_type_check
+from typing import Union, no_type_check
 
 import msgspec
 from paikalta import (
-    APP_NAME,
-    APP_VERSION,
     COMMA,
     ENCODING,
     FAIL,
     INVALID_ID,
-    LOG_SEPARATOR,
-    QUIET,
     SUCC,
-    TS_FORMAT_PAYLOADS,
     VALID_NAME_PAT,
     parse_csl_as_is,
-    log,
 )
 
 
 @no_type_check
 def load(csaf_path):
     """Load the CSAF data from the path to the JSON file or fail miserably."""
     with open(csaf_path, 'rt', encoding=ENCODING) as handle:
```

### Comparing `paikalta-2023.2.23/paikalta/cli.py` & `paikalta-2023.6.18/paikalta/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 """From the place (Finnish: paikalta) we derive the name - command line interface."""
 import argparse
-import json
-import pathlib
-import re
 import sys
-from typing import List, no_type_check
+from typing import no_type_check
 
 import paikalta.api as api
 from paikalta import (
-    APP_NAME,
-    APP_VERSION,
-    ENCODING,
     FAIL,
-    INVALID_ID,
-    LOG_SEPARATOR,
-    QUIET,
     SUCC,
-    TS_FORMAT_PAYLOADS,
-    VALID_NAME_PAT,
-    log,
 )
 
 
 @no_type_check
 def parser():
     """Implementation of command line API returning parser."""
     impl = argparse.ArgumentParser(description='Verifies or modifies the name of a CSAF 2.0 advisory file')
```

### Comparing `paikalta-2023.2.23/paikalta.egg-info/PKG-INFO` & `paikalta-2023.6.18/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: paikalta
-Version: 2023.2.23
+Version: 2023.6.18
 Summary: From the place (Finnish: paikalta) we derive the name.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/paikalta
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/paikalta
 Project-URL: Documentation, https://codes.dilettant.life/docs/paikalta
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/paikalta
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/paikalta
 Keywords: developer-tools,devops
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Paikalta
@@ -37,27 +38,34 @@
 
 ## Documentation
 
 User and developer [documentation of paikalta](https://codes.dilettant.life/docs/paikalta).
 
 ## Bug Tracker
 
-Feature requests and bug reports are best entered in the [todos of paikalta](https://todo.sr.ht/~sthagen/paikalta).
+Any feature requests or bug reports shall go to the [todos of paikalta](https://todo.sr.ht/~sthagen/paikalta).
 
 ## Primary Source repository
 
 The main source of `paikalta` is on a mountain in central Switzerland.
 We use distributed version control (git).
 There is no central hub.
 Every clone can become a new source for the benefit of all.
 The preferred public clones of `paikalta` are:
 
 * [on codeberg](https://codeberg.org/sthagen/paikalta) - a democratic community-driven, non-profit software development platform operated by Codeberg e.V.
 * [at sourcehut](https://git.sr.ht/~sthagen/paikalta) - a collection of tools useful for software development.
 
+## Contributions
+
+Please do not submit "pull requests" (I found no way to disable that "feature" on GitHub).
+If you like to share small changes under the repositories license please kindly do so by sending a patchset.
+You can either send such a patchset per email using [git send-email](https://git-send-email.io) or 
+if you are a sourcehut user by selecting "Prepare a patchset" on the summary page of your fork at [sourcehut](https://git.sr.ht/).
+
 ## Acknowledgements
 
 [Thomas Schmidt](https://github.com/tschmidtb51) provided the original source code as
 script [`check.py`](https://github.com/oasis-tcs/csaf/blob/master/csaf_2.0/test/filenames/check.py) and
 test cases in `test/fixtures/upstream/` as contributions to the OASIS CSAF TC repository
 below [/csaf_2.0/test/filenames/data](https://github.com/oasis-tcs/csaf/tree/master/csaf_2.0/test/filenames/data).
```

### Comparing `paikalta-2023.2.23/pyproject.toml` & `paikalta-2023.6.18/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paikalta"
-version = "2023.2.23"
+version = "2023.6.18"
 description = "From the place (Finnish: paikalta) we derive the name."
 readme = "README.md"
 authors = [
     { name = "Stefan Hagen", email = "stefan@hagen.link" },
 ]
 maintainers = [
     { name = "Stefan Hagen", email = "stefan@hagen.link" },
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "devops"]
 dependencies = [
-    "msgspec >= 0.13.1",
+    "msgspec >= 0.16.0",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
 
 [project.urls]
@@ -43,15 +44,15 @@
 [tool.setuptools.packages.find]
 include = ["paikalta"]
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

### Comparing `paikalta-2023.2.23/test/test_api.py` & `paikalta-2023.6.18/test/test_api.py`

 * *Files identical despite different names*

### Comparing `paikalta-2023.2.23/test/test_cli.py` & `paikalta-2023.6.18/test/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 def test_app_invalid_verbose(capsys):
     assert cli.app([str(INVALID_NAME), '-v']) == 1
     out, err = capsys.readouterr()
     assert FAIL in out
     assert not err
 
+
 def test_app_valid_verbose_user(capsys):
     assert cli.app([str(VALID_NAME), '-l', 'A,B']) == 0
     out, err = capsys.readouterr()
     assert 'A' in out
     assert not err
```

