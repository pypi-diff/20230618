# Comparing `tmp/gex_cli-1.0.3.tar.gz` & `tmp/gex_cli-1.0.4.tar.gz`

## Comparing `gex_cli-1.0.3.tar` & `gex_cli-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/__main__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/cli.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/config.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/logger.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.3/src/gex-cli/util.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 gex_cli-1.0.3/.gitignore
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gex_cli-1.0.3/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 gex_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 gex_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.4/src/gex/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gex_cli-1.0.4/src/gex/__main__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 gex_cli-1.0.4/src/gex/cli.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.4/src/gex/config.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.4/src/gex/logger.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.4/src/gex/util.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 gex_cli-1.0.4/.gitignore
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gex_cli-1.0.4/README.md
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 gex_cli-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 gex_cli-1.0.4/PKG-INFO
```

### Comparing `gex_cli-1.0.3/src/gex-cli/cli.py` & `gex_cli-1.0.4/src/gex/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,14 +70,7 @@
 
     for repo in org.repositories():
         repo: github3.github.repo.Repository = repo
         table.add_row(repo.name, repo.git_url[:-4].replace("git://", "https://"))
 
     console = Console()
     console.print(table)
-
-
-def main() -> click.Group:
-    gex.add_command(g)
-    gex.add_command(_list)
-    
-    return gex()
```

### Comparing `gex_cli-1.0.3/.gitignore` & `gex_cli-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.3/README.md` & `gex_cli-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.3/pyproject.toml` & `gex_cli-1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -36,23 +36,23 @@
 [project.urls]
 Documentation = "https://github.com/woidzero/gex-cli#readme"
 Issues = "https://github.com/woidzero/gex-cli/issues"
 Source = "https://github.com/woidzero/gex-cli"
 Chat = "https://discord.gg/MhvDqCXAzP"
 
 [project.scripts]
-gex = "src.gex-cli.cli:main"
+gex = "src.gex.__main__:main"
 
 [tool.hatch.version]
-path = "src/gex-cli/__init__.py"
+path = "src/gex/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "src/gex-cli/",
+    "src/gex/",
 ]
 
 [tool.semantic_release]
-version_variable = "src/gex-cli/__init__.py:__version__"
+version_variable = "src/gex/__init__.py:__version__"
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "hatch build"
```

### Comparing `gex_cli-1.0.3/PKG-INFO` & `gex_cli-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gex-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Command-line project generator using git repo.
 Project-URL: Documentation, https://github.com/woidzero/gex-cli#readme
 Project-URL: Issues, https://github.com/woidzero/gex-cli/issues
 Project-URL: Source, https://github.com/woidzero/gex-cli
 Project-URL: Chat, https://discord.gg/MhvDqCXAzP
 Author-email: woidzero <woidzerov@gmail.com>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gex-cli Version: 1.0.3 Summary: Command-line
+Metadata-Version: 2.1 Name: gex-cli Version: 1.0.4 Summary: Command-line
 project generator using git repo. Project-URL: Documentation, https://
 github.com/woidzero/gex-cli#readme Project-URL: Issues, https://github.com/
 woidzero/gex-cli/issues Project-URL: Source, https://github.com/woidzero/gex-
 cli Project-URL: Chat, https://discord.gg/MhvDqCXAzP Author-email: woidzero
 gmail.com> License-Expression: MIT Keywords: cli,command-
 line,console,generator,project managment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: License :: OSI
```

