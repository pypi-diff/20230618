# Comparing `tmp/crackerjack-0.3.2.tar.gz` & `tmp/crackerjack-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.2.tar", last modified: Sun Jun 18 10:45:56 2023, max compression
+gzip compressed data, was "crackerjack-0.3.3.tar", last modified: Sun Jun 18 16:35:05 2023, max compression
```

## Comparing `crackerjack-0.3.2.tar` & `crackerjack-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.2/LICENSE
--rw-r--r--   0        0        0     5580 2023-06-18 10:33:33.725079 crackerjack-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-06-18 10:45:20.934586 crackerjack-0.3.2/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      223 2023-06-18 10:45:20.887817 crackerjack-0.3.2/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-18 10:45:20.919362 crackerjack-0.3.2/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2974 2023-06-18 10:45:20.903860 crackerjack-0.3.2/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.2/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.2/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.2/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.2/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.2/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.2/crackerjack/__main__.py
--rw-r--r--   0        0        0     6093 2023-06-18 10:42:33.340722 crackerjack-0.3.2/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1670 2023-06-18 10:45:21.650599 crackerjack-0.3.2/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2021 2023-06-18 10:45:56.370474 crackerjack-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     6584 1970-01-01 00:00:00.000000 crackerjack-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.3/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 16:34:30.410683 crackerjack-0.3.3/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      223 2023-06-18 16:34:30.363852 crackerjack-0.3.3/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-18 16:34:30.395365 crackerjack-0.3.3/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2913 2023-06-18 16:34:30.379571 crackerjack-0.3.3/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.3/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.3/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.3/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.3/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.3/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.3/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6093 2023-06-18 10:42:33.340722 crackerjack-0.3.3/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1658 2023-06-18 16:34:31.122892 crackerjack-0.3.3/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2009 2023-06-18 16:35:05.831269 crackerjack-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6909 1970-01-01 00:00:00.000000 crackerjack-0.3.3/PKG-INFO
```

### Comparing `crackerjack-0.3.2/LICENSE` & `crackerjack-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.2/README.md` & `crackerjack-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,29 +35,30 @@
 There are various easy ways to keep your system python versions up-to-date and
 Docker containers for the latest versions are available immediately upon release. Most cloud providers
 will support the new versions in their virtual machines and containers shortly after release as well. If your dependencies
 break upon upgrade, file a bug report or fix it yourself. Simple enough.
 
 #### ...the Crackerjack solution:
 
-Crackerjack uses PDM with PEP-582. No more virtualenvs. Update your system python versions as they are released and start
+Crackerjack uses PDM with PEP-582 (yes, PEP-582 has been rejected but PDM still supports it and Crackerjack will continue to use it!).
+No more virtualenvs. Update your system python versions as they are released and start
 migrating your code. Crackerjack, and Crackerjack'd packages, should support the latest
 python release's features within 2 month after the release and depend solely on that version. Again, if
 something breaks, file a bug report or, even better, fix it yourself (maybe even learn something new things in the process).
 Easy-peasy. You just saved yourself a zillion headaches and can sleep
 better at night now.
 
 ### **What does this package do?**
 
 This package:
 
 - streamlines and standardizes code style across numerous packages
 
 - removes pipenv, poetry, and hatch build, dependency management, and virtual environment
-  management packages and replaces them with PDM using PEP 582 (work in progress)
+  management packages and replaces them with PDM using PEP-582 (work in progress)
 
 - installs, or updates, a project's pre-commit tools as well as .gitignore & other config files
   to comply with evolving crackerjack standards
 
 - runs the following pre-commit hooks (in order):
   * various core pre-commit hooks
   * [black](https://github.com/ambv/black)
@@ -87,24 +88,26 @@
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
 - format with black
 
 - use aiopath.AsyncPath or pathlib.Path not os.path
 
+- import typing as t
+
 - do not capitalize all letters in configuration settings or constants (we diverge from PEP-8 here
  for not other reason than it looks ugly)
 
 - functions that deal with path operations should get passed AsyncPaths or Paths - not strings
 
 - if a class can be a dataclasses.dataclass, pydantic.BaseModel, or msgspec.Struct it should be
 
 - force single line imports (will support isort Vertical Hanging Indent when ruff does)
 
-- use PDM and PEP 582 for dependency management and package building/publishing
+- use PDM and PEP-582 for dependency management and package building/publishing
 
 - use pdoc and mkdocs for producing documentation
 
 - use pytest for testing
 
 - be compliant with the latest python version within 2 months after release
 
@@ -140,10 +143,15 @@
 ``python -m crackerjack -p micro``
 
 The -p option not only publishes your project but will bump your
 project version for you. The options are 'micro', 'minor', and 'major'.
 Put the -c option at the end and commit the bumped version to your git
 repository at the same time.
 
+### **Contributing**
+
+Crackerjack is currently an evolving standard. If you like the idea, but don't like certain things about it, or
+would like new features added, let me know in Discussions, Issues, or email me.
+
 ### **License**
 
 BSD-3-Clause
```

### Comparing `crackerjack-0.3.2/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.3/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.2/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.3/crackerjack/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,19 @@
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: v0.0.272
     hooks:
       - id: ruff
-#  - repo: https://github.com/fredrikaverpil/creosote
-  - repo: https://github.com/lesleslie/creosote
-    rev: v2.7.0
+  - repo: https://github.com/fredrikaverpil/creosote
+    rev: v2.6.2
     hooks:
       - id: creosote
-        args: [--paths, "crackerjack", --exclude-deps, "pdm-bump", "tomli-w", "--pep582"]
+        args: [--paths, "crackerjack", --exclude-deps, "pdm-bump", "tomli-w"]
   - repo: https://github.com/ikamensh/flynt/
     rev: '0.78'
     hooks:
       - id: flynt
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
```

### Comparing `crackerjack-0.3.2/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.3/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.2/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.3/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.2/crackerjack/__main__.py` & `crackerjack-0.3.3/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.2/crackerjack/crackerjack.py` & `crackerjack-0.3.3/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.2/crackerjack/pyproject.toml` & `crackerjack-0.3.3/crackerjack/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.2"
-description = "Crackerjack code formatting style."
+version = "0.3.3"
+description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
     "creosote",
```

### Comparing `crackerjack-0.3.2/pyproject.toml` & `crackerjack-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.2"
-description = "Crackerjack code formatting style."
+version = "0.3.3"
+description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
     "creosote",
```

### Comparing `crackerjack-0.3.2/PKG-INFO` & `crackerjack-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.3.2
-Summary: Crackerjack code formatting style.
+Version: 0.3.3
+Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
@@ -62,29 +62,30 @@
 There are various easy ways to keep your system python versions up-to-date and
 Docker containers for the latest versions are available immediately upon release. Most cloud providers
 will support the new versions in their virtual machines and containers shortly after release as well. If your dependencies
 break upon upgrade, file a bug report or fix it yourself. Simple enough.
 
 #### ...the Crackerjack solution:
 
-Crackerjack uses PDM with PEP-582. No more virtualenvs. Update your system python versions as they are released and start
+Crackerjack uses PDM with PEP-582 (yes, PEP-582 has been rejected but PDM still supports it and Crackerjack will continue to use it!).
+No more virtualenvs. Update your system python versions as they are released and start
 migrating your code. Crackerjack, and Crackerjack'd packages, should support the latest
 python release's features within 2 month after the release and depend solely on that version. Again, if
 something breaks, file a bug report or, even better, fix it yourself (maybe even learn something new things in the process).
 Easy-peasy. You just saved yourself a zillion headaches and can sleep
 better at night now.
 
 ### **What does this package do?**
 
 This package:
 
 - streamlines and standardizes code style across numerous packages
 
 - removes pipenv, poetry, and hatch build, dependency management, and virtual environment
-  management packages and replaces them with PDM using PEP 582 (work in progress)
+  management packages and replaces them with PDM using PEP-582 (work in progress)
 
 - installs, or updates, a project's pre-commit tools as well as .gitignore & other config files
   to comply with evolving crackerjack standards
 
 - runs the following pre-commit hooks (in order):
   * various core pre-commit hooks
   * [black](https://github.com/ambv/black)
@@ -114,24 +115,26 @@
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
 - format with black
 
 - use aiopath.AsyncPath or pathlib.Path not os.path
 
+- import typing as t
+
 - do not capitalize all letters in configuration settings or constants (we diverge from PEP-8 here
  for not other reason than it looks ugly)
 
 - functions that deal with path operations should get passed AsyncPaths or Paths - not strings
 
 - if a class can be a dataclasses.dataclass, pydantic.BaseModel, or msgspec.Struct it should be
 
 - force single line imports (will support isort Vertical Hanging Indent when ruff does)
 
-- use PDM and PEP 582 for dependency management and package building/publishing
+- use PDM and PEP-582 for dependency management and package building/publishing
 
 - use pdoc and mkdocs for producing documentation
 
 - use pytest for testing
 
 - be compliant with the latest python version within 2 months after release
 
@@ -167,10 +170,15 @@
 ``python -m crackerjack -p micro``
 
 The -p option not only publishes your project but will bump your
 project version for you. The options are 'micro', 'minor', and 'major'.
 Put the -c option at the end and commit the bumped version to your git
 repository at the same time.
 
+### **Contributing**
+
+Crackerjack is currently an evolving standard. If you like the idea, but don't like certain things about it, or
+would like new features added, let me know in Discussions, Issues, or email me.
+
 ### **License**
 
 BSD-3-Clause
```

