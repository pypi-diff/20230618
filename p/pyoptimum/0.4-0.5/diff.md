# Comparing `tmp/pyoptimum-0.4.tar.gz` & `tmp/pyoptimum-0.5.tar.gz`

## Comparing `pyoptimum-0.4.tar` & `pyoptimum-0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pyoptimum-0.4/.readthedocs.yaml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.4/requirements.txt
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyoptimum-0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pyoptimum-0.4/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/Makefile
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/conf.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/make.bat
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/requirements.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/src/modules.rst
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 pyoptimum-0.4/doc/src/quickstart.rst
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 pyoptimum-0.4/src/pyoptimum/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyoptimum-0.4/tests/__init__.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pyoptimum-0.4/tests/test_basic.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyoptimum-0.4/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyoptimum-0.4/LICENSE
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 pyoptimum-0.4/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyoptimum-0.4/pyproject.toml
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyoptimum-0.4/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pyoptimum-0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.5/requirements.txt
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 pyoptimum-0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pyoptimum-0.5/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/Makefile
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/conf.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/make.bat
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/requirements.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/src/modules.rst
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 pyoptimum-0.5/doc/src/quickstart.rst
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 pyoptimum-0.5/src/pyoptimum/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyoptimum-0.5/tests/__init__.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 pyoptimum-0.5/tests/test_basic.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyoptimum-0.5/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyoptimum-0.5/LICENSE
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 pyoptimum-0.5/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pyoptimum-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyoptimum-0.5/PKG-INFO
```

### Comparing `pyoptimum-0.4/.readthedocs.yaml` & `pyoptimum-0.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/.github/workflows/python-publish.yml` & `pyoptimum-0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/.github/workflows/python-test.yml` & `pyoptimum-0.5/.github/workflows/python-test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 name: Test Python package
 
 on: [push]
 
 jobs:
   build:
-
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
+    concurrency:
+      group: testing-one-by-one
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `pyoptimum-0.4/doc/Makefile` & `pyoptimum-0.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/doc/conf.py` & `pyoptimum-0.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/doc/index.rst` & `pyoptimum-0.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/doc/make.bat` & `pyoptimum-0.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/doc/src/quickstart.rst` & `pyoptimum-0.5/doc/src/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/src/pyoptimum/__init__.py` & `pyoptimum-0.5/src/pyoptimum/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/tests/test_basic.py` & `pyoptimum-0.5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/.gitignore` & `pyoptimum-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/LICENSE` & `pyoptimum-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptimum-0.4/pyproject.toml` & `pyoptimum-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyoptimum"
-version = "0.4"
+version = "0.5"
 authors = [
     { name = "Mauricio C. de Oliveira", email = "mcdeoliveira@duck.com" }
 ]
 description = "Python library for optimize.vicbee.net optimize api"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords=["Optimization", "Porfolio Optimization"]
```

### Comparing `pyoptimum-0.4/PKG-INFO` & `pyoptimum-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptimum
-Version: 0.4
+Version: 0.5
 Summary: Python library for optimize.vicbee.net optimize api
 Project-URL: Homepage, https://github.com/mcdeoliveira/pyoptimum
 Author-email: "Mauricio C. de Oliveira" <mcdeoliveira@duck.com>
 License: MIT License
         
         Copyright (c) 2019 Mauricio de Oliveira
```

