# Comparing `tmp/gex_cli-1.0.2.tar.gz` & `tmp/gex_cli-1.0.3.tar.gz`

## Comparing `gex_cli-1.0.2.tar` & `gex_cli-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/__main__.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/cli.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/config.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/logger.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/utils.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 gex_cli-1.0.2/.gitignore
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gex_cli-1.0.2/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 gex_cli-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 gex_cli-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/__main__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/cli.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/config.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/logger.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/util.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 gex_cli-1.0.3/.gitignore
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gex_cli-1.0.3/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 gex_cli-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 gex_cli-1.0.3/PKG-INFO
```

### Comparing `gex_cli-1.0.2/gexpy/cli.py` & `gex_cli-1.0.3/src/gex-cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from __future__ import annotations
 
 import os
-from typing import Tuple
 
 import click
 import git
 import github3
 from rich.console import Console
 from rich.table import Table
 
 from . import __name__, __version__
-from gexpy.config import Config
-from gexpy.logger import success, error, info, warn
-from gexpy.utils import rmtree
+from .logger import success, error, info, warn
+from .util import rmtree
 
 
 @click.group(context_settings={'help_option_names': ['-h', '--help'],})
 @click.version_option(version=__version__, prog_name=__name__)
 def gex() -> None:
     pass
 
 
 @click.command(name="g")
-@click.argument("template", required=False)
-@click.option("-n", "--name", help="Project name.")
-@click.option("-sG", "--save-git", 
+@click.argument("template", 
+                required=False)
+@click.option("-n", "--name", "project_name",
+              help="Project name.")
+@click.option("-sG", "--save-git", "save_git",
               help="Saves /.git directory.", 
               default=False, 
               show_default=False, 
               is_flag=True) 
-def g(template, name, save_git) -> None:
+def g(template, project_name, save_git) -> None:
     """Generate a project."""
-    
     try:
-        _name = str(name if name else template)
-        
-        dist = os.getcwd() + "\\" + _name
+        name = str(project_name if project_name else template)
+        source = f"https://github.com/gexpy/{template}"
 
-        info(f"Creating folder '{_name}' ...")
+        dist = os.getcwd() + "\\" + name
+
+        info(f"Creating folder '{name}' ...")
         os.mkdir(dist)
         
-        git.Repo.clone_from(Config.URL+template, dist)
+        git.Repo.clone_from(source, dist)
         
         if not save_git:
             warn(".git will be removed.")
             info("Removing .git ...")
             rmtree(dist + "\.git")
 
         success("Project successfully generated.")
@@ -72,11 +72,12 @@
         repo: github3.github.repo.Repository = repo
         table.add_row(repo.name, repo.git_url[:-4].replace("git://", "https://"))
 
     console = Console()
     console.print(table)
 
 
-commands: Tuple[click.Command] = (
-    g,
-    _list
-)
+def main() -> click.Group:
+    gex.add_command(g)
+    gex.add_command(_list)
+    
+    return gex()
```

### Comparing `gex_cli-1.0.2/.gitignore` & `gex_cli-1.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
+templates/
+
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `gex_cli-1.0.2/README.md` & `gex_cli-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.2/pyproject.toml` & `gex_cli-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -18,33 +18,41 @@
     "rich",
 ]
 
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
   "Environment :: Console",
+  "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.urls]
 Documentation = "https://github.com/woidzero/gex-cli#readme"
 Issues = "https://github.com/woidzero/gex-cli/issues"
 Source = "https://github.com/woidzero/gex-cli"
+Chat = "https://discord.gg/MhvDqCXAzP"
 
 [project.scripts]
-gex = "gexpy.__main__:main"
+gex = "src.gex-cli.cli:main"
 
 [tool.hatch.version]
-path = "gexpy/__init__.py"
+path = "src/gex-cli/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "gexpy/",
+    "src/gex-cli/",
 ]
 
+[tool.semantic_release]
+version_variable = "src/gex-cli/__init__.py:__version__"
+branch = "main"
+upload_to_pypi = true
+upload_to_release = true
+build_command = "hatch build"
```

### Comparing `gex_cli-1.0.2/PKG-INFO` & `gex_cli-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: gex-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command-line project generator using git repo.
 Project-URL: Documentation, https://github.com/woidzero/gex-cli#readme
 Project-URL: Issues, https://github.com/woidzero/gex-cli/issues
 Project-URL: Source, https://github.com/woidzero/gex-cli
+Project-URL: Chat, https://discord.gg/MhvDqCXAzP
 Author-email: woidzero <woidzerov@gmail.com>
 License-Expression: MIT
 Keywords: cli,command-line,console,generator,project managment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 2.1 Name: gex-cli Version: 1.0.2 Summary: Command-line
+Metadata-Version: 2.1 Name: gex-cli Version: 1.0.3 Summary: Command-line
 project generator using git repo. Project-URL: Documentation, https://
 github.com/woidzero/gex-cli#readme Project-URL: Issues, https://github.com/
 woidzero/gex-cli/issues Project-URL: Source, https://github.com/woidzero/gex-
-cli Author-email: woidzero
+cli Project-URL: Chat, https://discord.gg/MhvDqCXAzP Author-email: woidzero
 gmail.com> License-Expression: MIT Keywords: cli,command-
 line,console,generator,project managment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7 Requires-Dist: click Requires-Dist: gitpython Requires-
-Dist: mcfc Requires-Dist: rich Description-Content-Type: text/markdown # gex-
-cli Generate projects using built-in or custom templates via command-line. [!
-[PyPI - Version](https://img.shields.io/pypi/v/gex-cli.svg)](https://pypi.org/
-project/gex-cli) [![PyPI - Downloads](https://img.shields.io/pypi/dm/gex-cli)]
-(https://pypi.org/project/gex-cli) [![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/gex-cli.svg)](https://pypi.org/project/gex-cli)
-## Installation ```bash pip install gex-cli ``` ## Usage ```bash gex g web -
-n MyWebsite ``` ## Support For support, email woidzeroo@gmail.com ## License
-`gex-cli` is distributed under the terms of the [MIT](https://spdx.org/
-licenses/MIT.html) license.
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: Implementation :: CPython Classifier:
+Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
+Requires-Dist: click Requires-Dist: gitpython Requires-Dist: mcfc Requires-
+Dist: rich Description-Content-Type: text/markdown # gex-cli Generate projects
+using built-in or custom templates via command-line. [![PyPI - Version](https:/
+/img.shields.io/pypi/v/gex-cli.svg)](https://pypi.org/project/gex-cli) [![PyPI
+- Downloads](https://img.shields.io/pypi/dm/gex-cli)](https://pypi.org/project/
+gex-cli) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gex-
+cli.svg)](https://pypi.org/project/gex-cli) ## Installation ```bash pip install
+gex-cli ``` ## Usage ```bash gex g web -n MyWebsite ``` ## Support For support,
+email woidzeroo@gmail.com ## License `gex-cli` is distributed under the terms
+of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

