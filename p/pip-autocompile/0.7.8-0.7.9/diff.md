# Comparing `tmp/pip_autocompile-0.7.8.tar.gz` & `tmp/pip_autocompile-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_autocompile-0.7.8.tar", max compression
+gzip compressed data, was "pip_autocompile-0.7.9.tar", max compression
```

## Comparing `pip_autocompile-0.7.8.tar` & `pip_autocompile-0.7.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1076 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/LICENSE
--rw-r--r--   0        0        0     1572 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/README.md
--rw-r--r--   0        0        0       33 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/Dockerfile
--rw-r--r--   0        0        0        6 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/requirements/50_base.in
--rw-r--r--   0        0        0       26 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/requirements/60_dev.in
--rw-r--r--   0        0        0       24 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker/requirements/61_prod.in
--rw-r--r--   0        0        0      429 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker_ssh_agent/Dockerfile
--rw-r--r--   0        0        0       49 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/docker_ssh_agent/requirements/pip-autocompile.in
--rw-r--r--   0        0        0        6 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/examples/requirements.in
--rw-r--r--   0        0        0     1985 2023-05-30 11:08:15.280207 pip_autocompile-0.7.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/__init__.py
--rw-r--r--   0        0        0      379 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/git.py
--rw-r--r--   0        0        0      771 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/io.py
--rw-r--r--   0        0        0      261 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/logging.py
--rw-r--r--   0        0        0     6027 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/main.py
--rw-r--r--   0        0        0        0 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/py.typed
--rw-r--r--   0        0        0      229 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/src/pipautocompile/utils.py
--rw-r--r--   0        0        0        0 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/__init__.py
--rw-r--r--   0        0        0     2533 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/conftest.py
--rw-r--r--   0        0        0     1626 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_git.py
--rw-r--r--   0        0        0     4448 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_io.py
--rw-r--r--   0        0        0     2400 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_logging.py
--rw-r--r--   0        0        0     5104 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_main.py
--rw-r--r--   0        0        0     1232 2023-05-30 11:08:14.504197 pip_autocompile-0.7.8/tests/test_utils.py
--rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 pip_autocompile-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/LICENSE
+-rw-r--r--   0        0        0     1606 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/README.md
+-rw-r--r--   0        0        0       33 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/docker/Dockerfile
+-rw-r--r--   0        0        0        6 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/docker/requirements/50_base.in
+-rw-r--r--   0        0        0       26 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/docker/requirements/60_dev.in
+-rw-r--r--   0        0        0       24 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/docker/requirements/61_prod.in
+-rw-r--r--   0        0        0      429 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/docker_ssh_agent/Dockerfile
+-rw-r--r--   0        0        0       49 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/docker_ssh_agent/requirements/pip-autocompile.in
+-rw-r--r--   0        0        0        6 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/examples/requirements.in
+-rw-r--r--   0        0        0     2253 2023-06-18 15:31:50.410330 pip_autocompile-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/__init__.py
+-rw-r--r--   0        0        0      379 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/git.py
+-rw-r--r--   0        0        0      771 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/io.py
+-rw-r--r--   0        0        0      261 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/logging.py
+-rw-r--r--   0        0        0     6023 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/main.py
+-rw-r--r--   0        0        0        0 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/py.typed
+-rw-r--r--   0        0        0      229 2023-06-18 15:31:49.594319 pip_autocompile-0.7.9/src/pipautocompile/utils.py
+-rw-r--r--   0        0        0        0 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/conftest.py
+-rw-r--r--   0        0        0     1626 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/test_git.py
+-rw-r--r--   0        0        0     4448 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/test_io.py
+-rw-r--r--   0        0        0     2400 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/test_logging.py
+-rw-r--r--   0        0        0     5104 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/test_main.py
+-rw-r--r--   0        0        0     1232 2023-06-18 15:31:49.598319 pip_autocompile-0.7.9/tests/test_utils.py
+-rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 pip_autocompile-0.7.9/PKG-INFO
```

### Comparing `pip_autocompile-0.7.8/LICENSE` & `pip_autocompile-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/README.md` & `pip_autocompile-0.7.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pip-autocompile
 
 [![build](https://github.com/KSmanis/pip-autocompile/actions/workflows/build.yml/badge.svg)](https://github.com/KSmanis/pip-autocompile/actions/workflows/build.yml)
 [![PyPI version](https://img.shields.io/pypi/v/pip-autocompile.svg)](https://pypi.org/project/pip-autocompile/)
 [![pre-commit enabled](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg)](https://renovatebot.com/)
+[![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg?logo=renovatebot&logoColor=white)](https://renovatebot.com/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![mypy: strict](https://img.shields.io/badge/mypy-strict-2a6db2)](http://mypy-lang.org/)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=KSmanis_pip-autocompile&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=KSmanis_pip-autocompile)
 [![codecov](https://codecov.io/gh/KSmanis/pip-autocompile/branch/master/graph/badge.svg?token=47HDGLM2NQ)](https://codecov.io/gh/KSmanis/pip-autocompile)
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
 
 Automate pip-compile for multiple environments.
 
 ## Dependencies
```

### Comparing `pip_autocompile-0.7.8/pyproject.toml` & `pip_autocompile-0.7.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,106 @@
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
+
+[tool.coverage.report]
+exclude_lines = [
+  "if TYPE_CHECKING:",
+  "pragma: no cover",
+]
+show_missing = true
+skip_empty = true
+
+[tool.coverage.run]
+relative_files = true
+
+[tool.mypy]
+disallow_any_unimported = true
+show_error_codes = true
+strict = true
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = "pygit2"
+
 [tool.poetry]
-name = "pip-autocompile"
-version = "0.7.8"
-description = "Automate pip-compile for multiple environments."
-license = "MIT"
 authors = ["Konstantinos Smanis <konstantinos.smanis@gmail.com>"]
-readme = "README.md"
-repository = "https://github.com/KSmanis/pip-autocompile"
 classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Build Tools"
-]
-packages = [
-    { include = "pipautocompile", from = "src" }
+  "Development Status :: 3 - Alpha",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "Operating System :: OS Independent",
+  "Topic :: Software Development :: Build Tools",
 ]
+description = "Automate pip-compile for multiple environments."
 include = [
-    { path = "examples", format = "sdist" },
-    { path = "tests", format = "sdist" },
+  {format = "sdist", path = "examples"},
+  {format = "sdist", path = "tests"},
 ]
+license = "MIT"
+name = "pip-autocompile"
+packages = [
+  {from = "src", include = "pipautocompile"},
+]
+readme = "README.md"
+repository = "https://github.com/KSmanis/pip-autocompile"
+version = "0.7.9"
 
 [tool.poetry.dependencies]
-python = "^3.7"
 click = "^8.1.3"
 pygit2 = [
-    { version = "~1.10.1", python = "~3.7" },
-    { version = "^1.11.1", python = "^3.8" },
+  {python = "^3.8", version = "^1.12.1"},
+  {python = "~3.7", version = "~1.10.1"},
+]
+python = "^3.7"
+python-on-whales = [
+  {python = "^3.8", version = "^0.62.0"},
+  {python = "~3.7", version = "~0.60.1"},
 ]
-python-on-whales = "^0.60.1"
 
 [tool.poetry.group.lint.dependencies]
+mypy = "^1.3.0"
 pre-commit = [
-    { version = "~2.21.0", python = "~3.7" },
-    { version = "^3.0.0", python = "^3.8" },
+  {python = "^3.8", version = "^3.3.3"},
+  {python = "~3.7", version = "~2.21.0"},
 ]
-mypy = "^1.3.0"
 
 [tool.poetry.group.test.dependencies]
 pip-tools = "^6.13.0"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.scripts]
 pip-autocompile = "pipautocompile.main:cli"
 
-[tool.coverage.report]
-exclude_lines = [
-    "pragma: no cover",
-    "if TYPE_CHECKING:",
-]
-show_missing = true
-skip_empty = true
-
-[tool.coverage.run]
-relative_files = true
-
-[tool.isort]
-profile = "black"
-add_imports = ["from __future__ import annotations"]
-append_only = true
-force_single_line = true
-
-[tool.mypy]
-disallow_any_unimported = true
-show_error_codes = true
-strict = true
-
-[[tool.mypy.overrides]]
-module = "pygit2"
-ignore_missing_imports = true
-
 [tool.pytest.ini_options]
 addopts = "--cov=src --cov-branch"
 testpaths = ["tests"]
 
+[tool.ruff]
+select = [
+  "E",
+  "F",
+  "I",
+  "RUF",
+  "S",
+  "UP",
+  "W",
+]
+src = ["src"]
+target-version = "py37"
+
+[tool.ruff.isort]
+force-single-line = true
+required-imports = ["from __future__ import annotations"]
+
+[tool.ruff.per-file-ignores]
+"tests/**" = ["S101"]
+
 [tool.semantic_release]
 build_command = "pip install poetry && poetry build"
 commit_subject = "build: release v{version}"
 version_toml = ["pyproject.toml:tool.poetry.version"]
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.tomlsort]
+all = true
+spaces_before_inline_comment = 2
+trailing_comma_inline_array = true
```

### Comparing `pip_autocompile-0.7.8/src/pipautocompile/io.py` & `pip_autocompile-0.7.9/src/pipautocompile/io.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/src/pipautocompile/main.py` & `pip_autocompile-0.7.9/src/pipautocompile/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import os
-import subprocess  # nosec
+import subprocess
 import sys
 from itertools import groupby
 from pathlib import Path
 from shlex import split
 from typing import TYPE_CHECKING
 
 import click
@@ -158,12 +158,12 @@
                     )
                     container.copy_from(
                         container_spec.with_suffix(".txt"), spec.with_suffix(".txt")
                     )
         else:
             for spec in specs:
                 info(f"Compiling {spec}...")
-                subprocess.check_call(  # nosec
-                    ("pip-compile", *pip_compile_args, spec.name),
+                subprocess.check_call(
+                    ("pip-compile", *pip_compile_args, spec.name),  # noqa: S603
                     cwd=spec_dir,
                     env={**os.environ, **pip_compile_env},
                 )
```

### Comparing `pip_autocompile-0.7.8/tests/conftest.py` & `pip_autocompile-0.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/tests/test_git.py` & `pip_autocompile-0.7.9/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/tests/test_io.py` & `pip_autocompile-0.7.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/tests/test_logging.py` & `pip_autocompile-0.7.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/tests/test_main.py` & `pip_autocompile-0.7.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/tests/test_utils.py` & `pip_autocompile-0.7.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pip_autocompile-0.7.8/PKG-INFO` & `pip_autocompile-0.7.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-autocompile
-Version: 0.7.8
+Version: 0.7.9
 Summary: Automate pip-compile for multiple environments.
 Home-page: https://github.com/KSmanis/pip-autocompile
 License: MIT
 Author: Konstantinos Smanis
 Author-email: konstantinos.smanis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -17,28 +17,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pygit2 (>=1.10.1,<1.11.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: pygit2 (>=1.11.1,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
-Requires-Dist: python-on-whales (>=0.60.1,<0.61.0)
+Requires-Dist: pygit2 (>=1.12.1,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: python-on-whales (>=0.60.1,<0.61.0) ; python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: python-on-whales (>=0.62.0,<0.63.0) ; python_version >= "3.8" and python_version < "4.0"
 Project-URL: Repository, https://github.com/KSmanis/pip-autocompile
 Description-Content-Type: text/markdown
 
 # pip-autocompile
 
 [![build](https://github.com/KSmanis/pip-autocompile/actions/workflows/build.yml/badge.svg)](https://github.com/KSmanis/pip-autocompile/actions/workflows/build.yml)
 [![PyPI version](https://img.shields.io/pypi/v/pip-autocompile.svg)](https://pypi.org/project/pip-autocompile/)
 [![pre-commit enabled](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-[![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg)](https://renovatebot.com/)
+[![Renovate enabled](https://img.shields.io/badge/renovate-enabled-brightgreen.svg?logo=renovatebot&logoColor=white)](https://renovatebot.com/)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
+[![mypy: strict](https://img.shields.io/badge/mypy-strict-2a6db2)](http://mypy-lang.org/)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=KSmanis_pip-autocompile&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=KSmanis_pip-autocompile)
 [![codecov](https://codecov.io/gh/KSmanis/pip-autocompile/branch/master/graph/badge.svg?token=47HDGLM2NQ)](https://codecov.io/gh/KSmanis/pip-autocompile)
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
 
 Automate pip-compile for multiple environments.
 
 ## Dependencies
```

