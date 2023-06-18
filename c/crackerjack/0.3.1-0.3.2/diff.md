# Comparing `tmp/crackerjack-0.3.1.tar.gz` & `tmp/crackerjack-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.1.tar", last modified: Tue Jun 13 13:00:32 2023, max compression
+gzip compressed data, was "crackerjack-0.3.2.tar", last modified: Sun Jun 18 10:45:56 2023, max compression
```

## Comparing `crackerjack-0.3.1.tar` & `crackerjack-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.1/LICENSE
--rw-r--r--   0        0        0     5387 2023-06-12 14:25:17.180921 crackerjack-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 12:59:52.997762 crackerjack-0.3.1/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      210 2023-06-13 12:59:52.947649 crackerjack-0.3.1/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-13 12:59:52.982434 crackerjack-0.3.1/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2908 2023-06-13 12:59:52.965261 crackerjack-0.3.1/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.1/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.1/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.1/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.1/crackerjack/__main__.py
--rw-r--r--   0        0        0     5774 2023-06-12 15:49:54.110842 crackerjack-0.3.1/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1691 2023-06-13 12:59:53.762587 crackerjack-0.3.1/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1912 2023-06-13 13:00:32.984341 crackerjack-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 crackerjack-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5580 2023-06-18 10:33:33.725079 crackerjack-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 10:45:20.934586 crackerjack-0.3.2/crackerjack/.crackerjack-config.yaml
+-rw-r--r--   0        0        0      223 2023-06-18 10:45:20.887817 crackerjack-0.3.2/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-18 10:45:20.919362 crackerjack-0.3.2/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2974 2023-06-18 10:45:20.903860 crackerjack-0.3.2/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.2/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.2/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.2/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.2/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.2/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.2/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6093 2023-06-18 10:42:33.340722 crackerjack-0.3.2/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1670 2023-06-18 10:45:21.650599 crackerjack-0.3.2/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2021 2023-06-18 10:45:56.370474 crackerjack-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6584 1970-01-01 00:00:00.000000 crackerjack-0.3.2/PKG-INFO
```

### Comparing `crackerjack-0.3.1/LICENSE` & `crackerjack-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.1/README.md` & `crackerjack-0.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Crackerjack Python
 
 [![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-[![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
 
 crack·​er·​jack ˈkra-kər-ˌjak
 : a person or thing of marked excellence
 
 ### **Why Crackerjack?**
@@ -16,15 +17,15 @@
 function, variable, and other object names - the code should be
 straight forward to read. Documentation and tests should be able to write themselves using a generative ai.
 Crackerjack provides a set of guidelines and utilities to keep the codebase clean, elegant, standardized, and
 easily readable.
 
 ### **Crackerjack philosophy...**
 
-#### Virutal envs:
+#### Virtual envs:
 
 Let's face it virtual envs are a mess and a lot of time and resources are
 spent maintaining them. [This](https://miro.medium.com/v2/resize:fit:984/format:webp/1*mHrDuetdLskvNHYucD9u3g.png) pretty
 much says it all. Enough is enough.
 
 #### Regression testing:
 
@@ -34,15 +35,15 @@
 There are various easy ways to keep your system python versions up-to-date and
 Docker containers for the latest versions are available immediately upon release. Most cloud providers
 will support the new versions in their virtual machines and containers shortly after release as well. If your dependencies
 break upon upgrade, file a bug report or fix it yourself. Simple enough.
 
 #### ...the Crackerjack solution:
 
-Crackerjack uses PDM with PEP 582. No more virtualenvs. Update your system python versions as they are released and start
+Crackerjack uses PDM with PEP-582. No more virtualenvs. Update your system python versions as they are released and start
 migrating your code. Crackerjack, and Crackerjack'd packages, should support the latest
 python release's features within 2 month after the release and depend solely on that version. Again, if
 something breaks, file a bug report or, even better, fix it yourself (maybe even learn something new things in the process).
 Easy-peasy. You just saved yourself a zillion headaches and can sleep
 better at night now.
 
 ### **What does this package do?**
@@ -86,14 +87,17 @@
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
 - format with black
 
 - use aiopath.AsyncPath or pathlib.Path not os.path
 
+- do not capitalize all letters in configuration settings or constants (we diverge from PEP-8 here
+ for not other reason than it looks ugly)
+
 - functions that deal with path operations should get passed AsyncPaths or Paths - not strings
 
 - if a class can be a dataclasses.dataclass, pydantic.BaseModel, or msgspec.Struct it should be
 
 - force single line imports (will support isort Vertical Hanging Indent when ruff does)
 
 - use PDM and PEP 582 for dependency management and package building/publishing
@@ -123,16 +127,14 @@
 
 ### **Usage**
 
 From your projects root directory:
 
 ```python -m crackerjack```
 
-Cracker jack will take care of the rest.
-
 For a full list of options:
 
 ```python -m crackerjack -h```
 
 When you ready to publish your project:
 
 ``python -m crackerjack -p micro``
```

### Comparing `crackerjack-0.3.1/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.2/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.1/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.2/crackerjack/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -21,47 +21,52 @@
     hooks:
       - id: black
         language_version: python3.11
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: v0.0.272
     hooks:
       - id: ruff
-  - repo: https://github.com/fredrikaverpil/creosote
-    rev: v2.6.1
+#  - repo: https://github.com/fredrikaverpil/creosote
+  - repo: https://github.com/lesleslie/creosote
+    rev: v2.7.0
     hooks:
       - id: creosote
-        args:
-          - --venv=__pypackages__/3.11/lib
-          - --paths=crackerjack
-  #          - --deps-file=pyproject.toml
-  #          - --sections=project.dependencies
+        args: [--paths, "crackerjack", --exclude-deps, "pdm-bump", "tomli-w", "--pep582"]
   - repo: https://github.com/ikamensh/flynt/
     rev: '0.78'
     hooks:
       - id: flynt
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
-    - id: codespell
-      additional_dependencies:
-        - tomli
+      - id: codespell
+        additional_dependencies:
+          - tomli
   - repo: local
     hooks:
       - id: pyanalyze
         name: pyanalyze
         entry: python -m pyanalyze
         language: python
         files: \.py$
         additional_dependencies:
           - pyanalyze>=0.10.1
   - repo: local
     hooks:
       - id: autotyping
         name: autotyping
-        entry: python -m libcst.tool codemod autotyping.AutotypeCommand --aggressive --only-without-imports --show-successes --include-generated --guess-common-names --pyanalyze-report ".pyanalyze-report.json" crackerjack
+        entry: python -m libcst.tool codemod autotyping.AutotypeCommand
+        args:
+          - --aggressive
+          - --only-without-imports
+          - --show-successes
+          - --include-generated
+          - --guess-common-names
+          - --pyanalyze-report '.pyanalyze-report.json',
+          - crackerjack
         types_or: [ python, pyi ]
         language: python
         files: \.py$
         additional_dependencies:
           - autotyping>=23.3.0
           - libcst>=0.4.9
   - repo: https://github.com/dosisod/refurb
```

### Comparing `crackerjack-0.3.1/crackerjack/__main__.py` & `crackerjack-0.3.2/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.1/crackerjack/crackerjack.py` & `crackerjack-0.3.2/crackerjack/crackerjack.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,32 +60,36 @@
         ]
         if root_files:
             self.poetry_pip_env = True
             for file in root_files:
                 await file.unlink()
 
     async def copy_configs(self) -> None:
-        for config in (
+        config_files = (
             ".gitignore",
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
             ".crackerjack-config.yaml",
-        ):
+            ".pyanalyze-report.json",
+            ".pyanalyze-report.md",
+        )
+        for config in config_files:
             config_path = self.our_path.parent / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
-            if self.pkg_path.stem == "crackerjack":
-                await config_path.write_text(await pkg_config_path.read_text())
-            # if poetry_pip_env:
-            #     await config_pkg_path.unlink()
-            config_text = await config_path.read_text()
-            await pkg_config_path.write_text(
-                config_text.replace("crackerjack", self.pkg_name)
-            )
-            run(["git", "add", config])
+            if config in config_files[:-2]:
+                if self.pkg_path.stem == "crackerjack":
+                    await config_path.write_text(await pkg_config_path.read_text())
+                # if poetry_pip_env:
+                #     await config_pkg_path.unlink()
+                config_text = await config_path.read_text()
+                await pkg_config_path.write_text(
+                    config_text.replace("crackerjack", self.pkg_name)
+                )
+                run(["git", "add", config])
 
     @staticmethod
     async def run_interactive(hook: str) -> None:
         success = False
         while not success:
             fail = call(["pre-commit", "run", hook.lower(), "--all-files"])
             if fail > 0:
@@ -100,20 +104,22 @@
         await self.copy_configs()
         installed_pkgs = check_output(
             ["pdm", "list", "--freeze"],
             universal_newlines=True,
         ).splitlines()
         if not len([pkg for pkg in installed_pkgs if "pre-commit" in pkg]):
             run(["pdm", "self", "add", "keyring"])
+            run(["pdm", "config", "python.use_venv", "false"])
             run(["git", "init"])
             run(["git", "branch", "-m", "main"])
             run(["git", "add", "pyproject.toml"])
             run(["pdm", "add", "-d", "pre_commit"])
             run(["pre-commit", "install"])
             run(["git", "add", "pdm.lock"])
+            run(["git", "config advice.addIgnoredFile", "false"])
         await self.update_pyproject_configs()
 
     async def process(self, options: t.Any) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
         sys.path.append(str(imp_dir))
         self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
```

### Comparing `crackerjack-0.3.1/crackerjack/pyproject.toml` & `crackerjack-0.3.2/crackerjack/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.1"
+version = "0.3.2"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -59,15 +59,14 @@
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "click>=8.1.3",
-    "pdoc3>=0.10.0",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
     "pydantic>=2.0b2",
     "inflection>=0.5.1",
     "acb>=0.1.8",
     "tomli-w>=1.0.0",
     "pdm-bump>=0.7.0",
```

### Comparing `crackerjack-0.3.1/pyproject.toml` & `crackerjack-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+[tool.pdm.options]
+config = [
+    "python.use_venv",
+    "true",
+]
+
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.2",
     "icecream>=2.1.3",
     "pre-commit>=3.3.2",
 ]
 
@@ -25,14 +31,18 @@
 target-version = [
     "py311",
 ]
 
 [tool.refurb]
 enable_all = true
 
+[tool.codespell]
+quiet-level = 3
+ignore-words-list = "crate"
+
 [tool.pyanalyze]
 paths = [
     "crackerjack",
 ]
 markdown_output = ".pyanalyze-report.md"
 json_output = ".pyanalyze-report.json"
 find_unused = true
@@ -49,15 +59,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.1"
+version = "0.3.2"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -68,15 +78,14 @@
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "click>=8.1.3",
-    "pdoc3>=0.10.0",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
     "pydantic>=2.0b2",
     "inflection>=0.5.1",
     "acb>=0.1.8",
     "tomli-w>=1.0.0",
     "pdm-bump>=0.7.0",
```

### Comparing `crackerjack-0.3.1/PKG-INFO` & `crackerjack-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crackerjack
-Version: 0.3.1
+Version: 0.3.2
 Summary: Crackerjack code formatting style.
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
@@ -12,30 +12,30 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Homepage, https://github.com/lesleslie/crackerjack
 Project-URL: Documentation, https://github.com/lesleslie/crackerjack
 Project-URL: Repository, https://github.com/lesleslie/crackerjack
 Requires-Python: >=3.11
 Requires-Dist: click>=8.1.3
-Requires-Dist: pdoc3>=0.10.0
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: aioconsole>=0.6.1
 Requires-Dist: pydantic>=2.0b2
 Requires-Dist: inflection>=0.5.1
 Requires-Dist: acb>=0.1.8
 Requires-Dist: tomli-w>=1.0.0
 Requires-Dist: pdm-bump>=0.7.0
 Description-Content-Type: text/markdown
 
 # Crackerjack Python
 
 [![Python: 3.11](https://img.shields.io/badge/python-3.11%2B-blue)](https://docs.python.org/3/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
-[![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 [![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 Crackerjack is a python coding style which uses a minimalist approach to produce elegant, easy to read, code.
 
 crack·​er·​jack ˈkra-kər-ˌjak
 : a person or thing of marked excellence
 
 ### **Why Crackerjack?**
@@ -44,15 +44,15 @@
 function, variable, and other object names - the code should be
 straight forward to read. Documentation and tests should be able to write themselves using a generative ai.
 Crackerjack provides a set of guidelines and utilities to keep the codebase clean, elegant, standardized, and
 easily readable.
 
 ### **Crackerjack philosophy...**
 
-#### Virutal envs:
+#### Virtual envs:
 
 Let's face it virtual envs are a mess and a lot of time and resources are
 spent maintaining them. [This](https://miro.medium.com/v2/resize:fit:984/format:webp/1*mHrDuetdLskvNHYucD9u3g.png) pretty
 much says it all. Enough is enough.
 
 #### Regression testing:
 
@@ -62,15 +62,15 @@
 There are various easy ways to keep your system python versions up-to-date and
 Docker containers for the latest versions are available immediately upon release. Most cloud providers
 will support the new versions in their virtual machines and containers shortly after release as well. If your dependencies
 break upon upgrade, file a bug report or fix it yourself. Simple enough.
 
 #### ...the Crackerjack solution:
 
-Crackerjack uses PDM with PEP 582. No more virtualenvs. Update your system python versions as they are released and start
+Crackerjack uses PDM with PEP-582. No more virtualenvs. Update your system python versions as they are released and start
 migrating your code. Crackerjack, and Crackerjack'd packages, should support the latest
 python release's features within 2 month after the release and depend solely on that version. Again, if
 something breaks, file a bug report or, even better, fix it yourself (maybe even learn something new things in the process).
 Easy-peasy. You just saved yourself a zillion headaches and can sleep
 better at night now.
 
 ### **What does this package do?**
@@ -114,14 +114,17 @@
 
 - all docstrings, README's, and other documentation is to be done in Markdown (md)
 
 - format with black
 
 - use aiopath.AsyncPath or pathlib.Path not os.path
 
+- do not capitalize all letters in configuration settings or constants (we diverge from PEP-8 here
+ for not other reason than it looks ugly)
+
 - functions that deal with path operations should get passed AsyncPaths or Paths - not strings
 
 - if a class can be a dataclasses.dataclass, pydantic.BaseModel, or msgspec.Struct it should be
 
 - force single line imports (will support isort Vertical Hanging Indent when ruff does)
 
 - use PDM and PEP 582 for dependency management and package building/publishing
@@ -151,16 +154,14 @@
 
 ### **Usage**
 
 From your projects root directory:
 
 ```python -m crackerjack```
 
-Cracker jack will take care of the rest.
-
 For a full list of options:
 
 ```python -m crackerjack -h```
 
 When you ready to publish your project:
 
 ``python -m crackerjack -p micro``
```

