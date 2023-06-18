# Comparing `tmp/cmdict-0.1.4.tar.gz` & `tmp/cmdict-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdict-0.1.4.tar", max compression
+gzip compressed data, was "cmdict-0.1.5.tar", max compression
```

## Comparing `cmdict-0.1.4.tar` & `cmdict-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2023-06-08 20:24:25.879932 cmdict-0.1.4/LICENSE
--rw-r--r--   0        0        0     2717 2023-06-08 20:24:25.879932 cmdict-0.1.4/README.md
--rw-r--r--   0        0        0     1323 2023-06-08 20:24:25.879932 cmdict-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       93 2023-06-08 20:24:25.879932 cmdict-0.1.4/src/cmdict/__init__.py
--rw-r--r--   0        0        0      112 2023-06-08 20:24:25.879932 cmdict-0.1.4/src/cmdict/__main__.py
--rw-r--r--   0        0        0     2558 2023-06-08 20:24:25.879932 cmdict-0.1.4/src/cmdict/ecdict_connector.py
--rw-r--r--   0        0        0     1423 2023-06-08 20:24:25.879932 cmdict-0.1.4/src/cmdict/history.py
--rw-r--r--   0        0        0     4530 2023-06-08 20:24:25.879932 cmdict-0.1.4/src/cmdict/pdf_tools.py
--rw-r--r--   0        0        0     6129 2023-06-08 20:24:25.879932 cmdict-0.1.4/src/cmdict/run_script.py
--rw-r--r--   0        0        0      463 2023-06-08 20:24:25.883932 cmdict-0.1.4/src/cmdict/txt_tools.py
--rw-r--r--   0        0        0      384 2023-06-08 20:24:25.883932 cmdict-0.1.4/src/cmdict/utils.py
--rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 cmdict-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-18 11:48:39.310220 cmdict-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2717 2023-06-18 11:48:39.310220 cmdict-0.1.5/README.md
+-rw-r--r--   0        0        0     1298 2023-06-18 11:48:39.314220 cmdict-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/__main__.py
+-rw-r--r--   0        0        0     2558 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/ecdict_connector.py
+-rw-r--r--   0        0        0     1423 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/history.py
+-rw-r--r--   0        0        0     4530 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/pdf_tools.py
+-rw-r--r--   0        0        0     6129 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/run_script.py
+-rw-r--r--   0        0        0      463 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/txt_tools.py
+-rw-r--r--   0        0        0      384 2023-06-18 11:48:39.314220 cmdict-0.1.5/src/cmdict/utils.py
+-rw-r--r--   0        0        0     3623 1970-01-01 00:00:00.000000 cmdict-0.1.5/PKG-INFO
```

### Comparing `cmdict-0.1.4/LICENSE` & `cmdict-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.4/README.md` & `cmdict-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.4/pyproject.toml` & `cmdict-0.1.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmdict"
-version = "0.1.4"
+version = "0.1.5"
 description = "A command line dictionary toolset."
 authors = ["zequnyu <zequnyu11@gmail.com>", "edxu96 <edxu96@outlook.com>"]
 license = "GPL-3.0"
 exclude = ["src/cmdict/data/*"]
 readme = "README.md"
 repository = "https://github.com/pastydev/cmdict"
 
@@ -16,15 +16,14 @@
 python = ">=3.7.0"
 loguru = ">=0.5.1"
 click = ">=7.1.2"
 colorama = ">=0.4.3"
 requests = ">=2.24.0"
 tqdm = ">=4.48.0"
 pyyaml = ">=5.3.1"
-virtualenv = ">=20.10.0"
 
 [tool.poetry.group.pdf]
 optional = true
 
 [tool.poetry.group.pdf.dependencies]
 PyMuPDF = "1.22.3"
```

### Comparing `cmdict-0.1.4/src/cmdict/ecdict_connector.py` & `cmdict-0.1.5/src/cmdict/ecdict_connector.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.4/src/cmdict/history.py` & `cmdict-0.1.5/src/cmdict/history.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.4/src/cmdict/pdf_tools.py` & `cmdict-0.1.5/src/cmdict/pdf_tools.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.4/src/cmdict/run_script.py` & `cmdict-0.1.5/src/cmdict/run_script.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.4/PKG-INFO` & `cmdict-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmdict
-Version: 0.1.4
+Version: 0.1.5
 Summary: A command line dictionary toolset.
 Home-page: https://github.com/pastydev/cmdict
 License: GPL-3.0
 Author: zequnyu
 Author-email: zequnyu11@gmail.com
 Requires-Python: >=3.7.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.1.2)
 Requires-Dist: colorama (>=0.4.3)
 Requires-Dist: loguru (>=0.5.1)
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: requests (>=2.24.0)
 Requires-Dist: tqdm (>=4.48.0)
-Requires-Dist: virtualenv (>=20.10.0)
 Project-URL: Repository, https://github.com/pastydev/cmdict
 Description-Content-Type: text/markdown
 
 # cmdict &middot; [![pypi](https://badge.fury.io/py/cmdict.svg)](https://pypi.org/project/cmdict/) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/zequnyu/cmdict/blob/master/LICENSE) [![CI](https://github.com/pasty-dev/cmdict/actions/workflows/ci.yml/badge.svg)](https://github.com/pasty-dev/cmdict/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/zequnyu/cmdict/branch/master/graph/badge.svg)](https://codecov.io/gh/zequnyu/cmdict) [![poetry](https://img.shields.io/badge/PyPM-poetry-5975aa)](https://python-poetry.org) [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 `cmdict` is a command-line dictionary toolset.
```

