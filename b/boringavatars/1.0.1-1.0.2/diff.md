# Comparing `tmp/boringavatars-1.0.1.tar.gz` & `tmp/boringavatars-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boringavatars-1.0.1.tar", last modified: Thu Apr 27 21:29:57 2023, max compression
+gzip compressed data, was "boringavatars-1.0.2.tar", last modified: Sun Jun 18 02:45:37 2023, max compression
```

## Comparing `boringavatars-1.0.1.tar` & `boringavatars-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0     1715 2022-12-28 00:28:05.446313 boringavatars-1.0.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      160 2022-12-28 02:51:41.071111 boringavatars-1.0.1/.flake8
--rw-r--r--   0        0        0      232 2022-12-27 23:30:38.713764 boringavatars-1.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1799 2022-12-19 18:05:58.284258 boringavatars-1.0.1/.gitignore
--rw-r--r--   0        0        0     1481 2022-12-28 02:54:09.917879 boringavatars-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2022-12-19 18:05:58.284389 boringavatars-1.0.1/.pypirc
--rw-r--r--   0        0        0       99 2022-12-19 18:05:58.284480 boringavatars-1.0.1/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2022-12-19 18:05:58.284537 boringavatars-1.0.1/.vscode/settings.json
--rw-r--r--   0        0        0     1133 2022-12-28 02:49:57.273427 boringavatars-1.0.1/LICENSE
--rw-r--r--   0        0        0      595 2022-12-28 04:17:59.054029 boringavatars-1.0.1/README.md
--rw-r--r--   0        0        0     1508 2023-04-27 14:48:30.715137 boringavatars-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       46 2022-12-28 00:17:00.765116 boringavatars-1.0.1/requirements.txt
--rw-r--r--   0        0        0      901 2023-04-27 21:19:26.315811 boringavatars-1.0.1/src/boringavatars/__init__.py
--rw-r--r--   0        0        0      961 2022-12-28 04:10:56.288387 boringavatars-1.0.1/src/boringavatars/bauhaus.py
--rw-r--r--   0        0        0     1849 2022-12-28 04:11:08.947816 boringavatars-1.0.1/src/boringavatars/beam.py
--rw-r--r--   0        0        0      950 2022-12-28 04:11:15.850865 boringavatars-1.0.1/src/boringavatars/marble.py
--rw-r--r--   0        0        0      621 2022-12-28 04:11:24.008327 boringavatars-1.0.1/src/boringavatars/pixel.py
--rw-r--r--   0        0        0        0 2023-03-10 05:08:45.843083 boringavatars-1.0.1/src/boringavatars/py.typed
--rw-r--r--   0        0        0      879 2022-12-28 04:11:44.524937 boringavatars-1.0.1/src/boringavatars/ring.py
--rw-r--r--   0        0        0      693 2022-12-28 04:11:33.663675 boringavatars-1.0.1/src/boringavatars/sunset.py
--rw-r--r--   0        0        0     1510 2023-03-28 18:26:32.049497 boringavatars-1.0.1/src/boringavatars/templates/bauhaus.svg
--rw-r--r--   0        0        0     1782 2023-03-28 18:23:50.460090 boringavatars-1.0.1/src/boringavatars/templates/beam.svg
--rw-r--r--   0        0        0     1794 2022-12-28 04:04:39.371872 boringavatars-1.0.1/src/boringavatars/templates/marble.svg
--rw-r--r--   0        0        0     5592 2022-12-28 04:04:45.953148 boringavatars-1.0.1/src/boringavatars/templates/pixel.svg
--rw-r--r--   0        0        0     1105 2022-12-28 04:04:49.621227 boringavatars-1.0.1/src/boringavatars/templates/ring.svg
--rw-r--r--   0        0        0     1340 2022-12-28 04:04:51.745639 boringavatars-1.0.1/src/boringavatars/templates/sunset.svg
--rw-r--r--   0        0        0     1387 2023-04-27 21:16:18.231905 boringavatars-1.0.1/src/boringavatars/utils.py
--rw-r--r--   0        0        0      214 2022-12-28 04:17:17.661063 boringavatars-1.0.1/tests/test_avatars.py
--rw-r--r--   0        0        0     2231 1970-01-01 00:00:00.000000 boringavatars-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1715 2022-12-28 00:28:05.446313 boringavatars-1.0.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      160 2022-12-28 02:51:41.071111 boringavatars-1.0.2/.flake8
+-rw-r--r--   0        0        0      232 2022-12-27 23:30:38.713764 boringavatars-1.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      972 2023-06-18 02:26:36.855872 boringavatars-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1799 2022-12-19 18:05:58.284258 boringavatars-1.0.2/.gitignore
+-rw-r--r--   0        0        0      930 2023-06-18 02:42:42.893962 boringavatars-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2022-12-19 18:05:58.284389 boringavatars-1.0.2/.pypirc
+-rw-r--r--   0        0        0       99 2022-12-19 18:05:58.284480 boringavatars-1.0.2/.vscode/extensions.json
+-rw-r--r--   0        0        0       48 2023-06-18 02:27:36.839910 boringavatars-1.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1133 2022-12-28 02:49:57.273427 boringavatars-1.0.2/LICENSE
+-rw-r--r--   0        0        0      843 2023-06-18 02:20:27.558573 boringavatars-1.0.2/README.md
+-rw-r--r--   0        0        0     1245 2023-06-18 02:39:26.490527 boringavatars-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-06-18 02:41:16.153874 boringavatars-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      981 2023-06-18 02:44:51.643163 boringavatars-1.0.2/src/boringavatars/__init__.py
+-rw-r--r--   0        0        0      961 2022-12-28 04:10:56.288387 boringavatars-1.0.2/src/boringavatars/bauhaus.py
+-rw-r--r--   0        0        0     1849 2022-12-28 04:11:08.947816 boringavatars-1.0.2/src/boringavatars/beam.py
+-rw-r--r--   0        0        0      950 2022-12-28 04:11:15.850865 boringavatars-1.0.2/src/boringavatars/marble.py
+-rw-r--r--   0        0        0      621 2022-12-28 04:11:24.008327 boringavatars-1.0.2/src/boringavatars/pixel.py
+-rw-r--r--   0        0        0        0 2023-03-10 05:08:45.843083 boringavatars-1.0.2/src/boringavatars/py.typed
+-rw-r--r--   0        0        0      869 2023-06-18 01:35:18.219530 boringavatars-1.0.2/src/boringavatars/ring.py
+-rw-r--r--   0        0        0      693 2022-12-28 04:11:33.663675 boringavatars-1.0.2/src/boringavatars/sunset.py
+-rw-r--r--   0        0        0     1510 2023-03-28 18:26:32.049497 boringavatars-1.0.2/src/boringavatars/templates/bauhaus.svg
+-rw-r--r--   0        0        0     1782 2023-06-18 02:32:20.546061 boringavatars-1.0.2/src/boringavatars/templates/beam.svg
+-rw-r--r--   0        0        0     1794 2022-12-28 04:04:39.371872 boringavatars-1.0.2/src/boringavatars/templates/marble.svg
+-rw-r--r--   0        0        0     5592 2022-12-28 04:04:45.953148 boringavatars-1.0.2/src/boringavatars/templates/pixel.svg
+-rw-r--r--   0        0        0     1105 2022-12-28 04:04:49.621227 boringavatars-1.0.2/src/boringavatars/templates/ring.svg
+-rw-r--r--   0        0        0     1340 2022-12-28 04:04:51.745639 boringavatars-1.0.2/src/boringavatars/templates/sunset.svg
+-rw-r--r--   0        0        0     1387 2023-04-27 21:16:18.231905 boringavatars-1.0.2/src/boringavatars/utils.py
+-rw-r--r--   0        0        0        0 2023-06-18 02:37:58.338153 boringavatars-1.0.2/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0    10169 2023-06-18 02:42:57.881667 boringavatars-1.0.2/tests/snapshots/snap_test_avatars.py
+-rw-r--r--   0        0        0      887 2023-06-18 02:30:58.361168 boringavatars-1.0.2/tests/test_avatars.py
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 boringavatars-1.0.2/PKG-INFO
```

### Comparing `boringavatars-1.0.1/.devcontainer/devcontainer.json` & `boringavatars-1.0.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/.gitignore` & `boringavatars-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/LICENSE` & `boringavatars-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/README.md` & `boringavatars-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 
 # Boring Avatars
 
 boringavatars is a Python port of the <a href="https://www.npmjs.com/package/boring-avatars">boring-avatars</a> JS library.
 
+![Build Status](https://github.com/federicobond/boringavatars/actions/workflows/python-package.yml/badge.svg?branch=main)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/boringavatars.svg)](https://pypi.python.org/pypi/boringavatars)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Install
 
 ```
 pip install boringavatars
 ```
```

#### html2text {}

```diff
@@ -1,7 +1,10 @@
  # Boring Avatars boringavatars is a Python port of the boring-avatars JS
-library. [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
-(https://opensource.org/licenses/MIT) ## Install ``` pip install boringavatars
-``` ## Usage ```python from boringavatars import avatar # returns the string
-corresponding to the generated SVG avatar( "Maria Mitchell", variant="marble",
-colors=["92A1C6", "146A7C", "F0AB3D", "C271B4", "C20D90"], title=False,
-size=40, square=True, ) ``` ## License MIT
+library. ![Build Status](https://github.com/federicobond/boringavatars/actions/
+workflows/python-package.yml/badge.svg?branch=main) [![Supported Versions]
+(https://img.shields.io/pypi/pyversions/boringavatars.svg)](https://
+pypi.python.org/pypi/boringavatars) [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ## Install
+``` pip install boringavatars ``` ## Usage ```python from boringavatars import
+avatar # returns the string corresponding to the generated SVG avatar( "Maria
+Mitchell", variant="marble", colors=["92A1C6", "146A7C", "F0AB3D", "C271B4",
+"C20D90"], title=False, size=40, square=True, ) ``` ## License MIT
```

### Comparing `boringavatars-1.0.1/pyproject.toml` & `boringavatars-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -10,54 +10,47 @@
 description = ""
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
-    "Jinja2==3.1.2",
+    "Jinja2>=3.0.0",
 ]
+source = ["."]
 
 [project.optional-dependencies]
 test = [
-    "bandit[toml]==1.7.4",
     "black==22.1.0",
     "check-manifest==0.48",
-    "flake8-bugbear==22.1.11",
-    "flake8-docstrings",
-    "flake8-formatter_junit_xml",
-    "flake8==4.0.1",
     "pre-commit==2.17.0",
-    "pylint==2.12.2",
-    "pylint_junit",
-    "pytest-cov==3.0.0",
-    "pytest-runner",
-    "pytest==7.1.0",
-    "pytest-github-actions-annotate-failures",
 ]
 
 [project.urls]
 Documentation = "https://github.com/federicobond/boringavatars"
 Source = "https://github.com/federicobond/boringavatars"
 Tracker = "https://github.com/federicobond/boringavatars"
 
 [tool.flit.module]
 name = "boringavatars"
 
 executionEnvironments = [
   { root = "src" }
 ]
 
-[tool.pytest.ini_options]
-pythonpath = [
-  "src"
+[tool.ruff]
+exclude = ["tests/snapshots"]
+
+[tool.black]
+exclude = "tests/snapshots"
+
+executionEnvironments = [
+  { root = "src" }
 ]
-testpaths = "tests"
```

### Comparing `boringavatars-1.0.1/src/boringavatars/__init__.py` & `boringavatars-1.0.2/src/boringavatars/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
+from typing import Callable, Dict, Sequence
+
 from .bauhaus import bauhaus
 from .beam import beam
 from .marble import marble
 from .pixel import pixel
 from .ring import ring
 from .sunset import sunset
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 __all__ = ["avatar"]
 
 DEFAULT_COLORS = ["FFAD08", "EDD75A", "73B06F", "0C8F8F", "405059"]
 
-VARIANTS = {
+VARIANTS: Dict[str, Callable[..., str]] = {
     "beam": beam,
     "marble": marble,
     "pixel": pixel,
     "sunset": sunset,
     "bauhaus": bauhaus,
     "ring": ring,
 }
 
 
 def avatar(
     name: str,
     *,
-    colors: list[str] = DEFAULT_COLORS,
+    colors: Sequence[str] = DEFAULT_COLORS,
     variant: str = "marble",
     title: bool = False,
     size: int = 40,
     square: bool = False,
 ) -> str:
     """Generate an avatar SVG string with the given parameters."""
     if variant not in VARIANTS:
```

### Comparing `boringavatars-1.0.1/src/boringavatars/bauhaus.py` & `boringavatars-1.0.2/src/boringavatars/bauhaus.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/beam.py` & `boringavatars-1.0.2/src/boringavatars/beam.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/marble.py` & `boringavatars-1.0.2/src/boringavatars/marble.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/pixel.py` & `boringavatars-1.0.2/src/boringavatars/pixel.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/ring.py` & `boringavatars-1.0.2/src/boringavatars/ring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .utils import hash_code, get_random_color, get_unit, render
+from .utils import hash_code, get_random_color, render
 
 SIZE = 90
 COLORS = 5
 
 
 def generate_colors(name, colors):
     num_from_name = hash_code(name)
```

### Comparing `boringavatars-1.0.1/src/boringavatars/sunset.py` & `boringavatars-1.0.2/src/boringavatars/sunset.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/templates/bauhaus.svg` & `boringavatars-1.0.2/src/boringavatars/templates/bauhaus.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/templates/beam.svg` & `boringavatars-1.0.2/src/boringavatars/templates/beam.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/templates/marble.svg` & `boringavatars-1.0.2/src/boringavatars/templates/marble.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/templates/pixel.svg` & `boringavatars-1.0.2/src/boringavatars/templates/pixel.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/templates/ring.svg` & `boringavatars-1.0.2/src/boringavatars/templates/ring.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/templates/sunset.svg` & `boringavatars-1.0.2/src/boringavatars/templates/sunset.svg`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/src/boringavatars/utils.py` & `boringavatars-1.0.2/src/boringavatars/utils.py`

 * *Files identical despite different names*

### Comparing `boringavatars-1.0.1/PKG-INFO` & `boringavatars-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 Metadata-Version: 2.1
 Name: boringavatars
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author-email: Federico Bond <federicobond@gmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: bandit[toml]==1.7.4 ; extra == "test"
+Requires-Dist: Jinja2>=3.0.0
 Requires-Dist: black==22.1.0 ; extra == "test"
 Requires-Dist: check-manifest==0.48 ; extra == "test"
-Requires-Dist: flake8-bugbear==22.1.11 ; extra == "test"
-Requires-Dist: flake8-docstrings ; extra == "test"
-Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
-Requires-Dist: flake8==4.0.1 ; extra == "test"
 Requires-Dist: pre-commit==2.17.0 ; extra == "test"
-Requires-Dist: pylint==2.12.2 ; extra == "test"
-Requires-Dist: pylint_junit ; extra == "test"
-Requires-Dist: pytest-cov==3.0.0 ; extra == "test"
-Requires-Dist: pytest-runner ; extra == "test"
-Requires-Dist: pytest==7.1.0 ; extra == "test"
-Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Project-URL: Documentation, https://github.com/federicobond/boringavatars
 Project-URL: Source, https://github.com/federicobond/boringavatars
 Project-URL: Tracker, https://github.com/federicobond/boringavatars
 Provides-Extra: test
 
 
 # Boring Avatars
 
 boringavatars is a Python port of the <a href="https://www.npmjs.com/package/boring-avatars">boring-avatars</a> JS library.
 
+![Build Status](https://github.com/federicobond/boringavatars/actions/workflows/python-package.yml/badge.svg?branch=main)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/boringavatars.svg)](https://pypi.python.org/pypi/boringavatars)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Install
 
 ```
 pip install boringavatars
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,24 @@
-Metadata-Version: 2.1 Name: boringavatars Version: 1.0.1 Summary: Author-email:
+Metadata-Version: 2.1 Name: boringavatars Version: 1.0.2 Summary: Author-email:
 Federico Bond
-gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
+gmail.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Jinja2==3.1.2 Requires-Dist: bandit[toml]==1.7.4 ; extra ==
-"test" Requires-Dist: black==22.1.0 ; extra == "test" Requires-Dist: check-
-manifest==0.48 ; extra == "test" Requires-Dist: flake8-bugbear==22.1.11 ; extra
-== "test" Requires-Dist: flake8-docstrings ; extra == "test" Requires-Dist:
-flake8-formatter_junit_xml ; extra == "test" Requires-Dist: flake8==4.0.1 ;
-extra == "test" Requires-Dist: pre-commit==2.17.0 ; extra == "test" Requires-
-Dist: pylint==2.12.2 ; extra == "test" Requires-Dist: pylint_junit ; extra ==
-"test" Requires-Dist: pytest-cov==3.0.0 ; extra == "test" Requires-Dist:
-pytest-runner ; extra == "test" Requires-Dist: pytest==7.1.0 ; extra == "test"
-Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
-Project-URL: Documentation, https://github.com/federicobond/boringavatars
-Project-URL: Source, https://github.com/federicobond/boringavatars Project-URL:
-Tracker, https://github.com/federicobond/boringavatars Provides-Extra: test #
-Boring Avatars boringavatars is a Python port of the boring-avatars JS library.
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
-opensource.org/licenses/MIT) ## Install ``` pip install boringavatars ``` ##
-Usage ```python from boringavatars import avatar # returns the string
-corresponding to the generated SVG avatar( "Maria Mitchell", variant="marble",
-colors=["92A1C6", "146A7C", "F0AB3D", "C271B4", "C20D90"], title=False,
-size=40, square=True, ) ``` ## License MIT
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: Jinja2>=3.0.0 Requires-Dist:
+black==22.1.0 ; extra == "test" Requires-Dist: check-manifest==0.48 ; extra ==
+"test" Requires-Dist: pre-commit==2.17.0 ; extra == "test" Project-URL:
+Documentation, https://github.com/federicobond/boringavatars Project-URL:
+Source, https://github.com/federicobond/boringavatars Project-URL: Tracker,
+https://github.com/federicobond/boringavatars Provides-Extra: test # Boring
+Avatars boringavatars is a Python port of the boring-avatars JS library. !
+[Build Status](https://github.com/federicobond/boringavatars/actions/workflows/
+python-package.yml/badge.svg?branch=main) [![Supported Versions](https://
+img.shields.io/pypi/pyversions/boringavatars.svg)](https://pypi.python.org/
+pypi/boringavatars) [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) ## Install ``` pip install
+boringavatars ``` ## Usage ```python from boringavatars import avatar # returns
+the string corresponding to the generated SVG avatar( "Maria Mitchell",
+variant="marble", colors=["92A1C6", "146A7C", "F0AB3D", "C271B4", "C20D90"],
+title=False, size=40, square=True, ) ``` ## License MIT
```

