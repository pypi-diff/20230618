# Comparing `tmp/autoconf-language-server-0.0.4.tar.gz` & `tmp/autoconf-language-server-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoconf-language-server-0.0.4.tar", last modified: Sun Jun 18 05:13:45 2023, max compression
+gzip compressed data, was "autoconf-language-server-0.0.5.tar", last modified: Sun Jun 18 09:19:35 2023, max compression
```

## Comparing `autoconf-language-server-0.0.4.tar` & `autoconf-language-server-0.0.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.826828 autoconf-language-server-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.gitlint
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 05:13:45.822828 autoconf-language-server-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/docs/api/autoconf-language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/flake.nix
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/scripts/generate-api.md.pl
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 05:13:45.826828 autoconf-language-server-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.814828 autoconf-language-server-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.818828 autoconf-language-server-0.0.4/src/autoconf_language_server/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.814828 autoconf-language-server-0.0.4/src/autoconf_language_server/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.822828 autoconf-language-server-0.0.4/src/autoconf_language_server/assets/json/
--rw-r--r--   0 runner    (1001) docker     (123)   402908 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/assets/json/autoconf.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/src/autoconf_language_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.822828 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-18 05:13:45.000000 autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.822828 autoconf-language-server-0.0.4/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 05:13:45.822828 autoconf-language-server-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-18 05:13:29.000000 autoconf-language-server-0.0.4/tests/server_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.796000 autoconf-language-server-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 09:19:35.796000 autoconf-language-server-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/docs/api/autoconf-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       70 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       90 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/scripts/generate-api.md.pl
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 09:19:35.796000 autoconf-language-server-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.787999 autoconf-language-server-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/src/autoconf_language_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.787999 autoconf-language-server-0.0.5/src/autoconf_language_server/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/src/autoconf_language_server/assets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)   402908 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/assets/json/autoconf.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/src/autoconf_language_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.792000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-18 09:19:35.000000 autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.796000 autoconf-language-server-0.0.5/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:19:35.796000 autoconf-language-server-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-18 09:19:24.000000 autoconf-language-server-0.0.5/tests/server_test.py
```

### Comparing `autoconf-language-server-0.0.4/.github/workflows/main.yml` & `autoconf-language-server-0.0.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/.gitignore` & `autoconf-language-server-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/.pre-commit-config.yaml` & `autoconf-language-server-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/LICENSE` & `autoconf-language-server-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/PKG-INFO` & `autoconf-language-server-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf-language-server
-Version: 0.0.4
+Version: 0.0.5
 Summary: autoconf language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://autoconf-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/autoconf-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/autoconf-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/autoconf-language-server
```

### Comparing `autoconf-language-server-0.0.4/README.md` & `autoconf-language-server-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/docs/conf.py` & `autoconf-language-server-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/docs/resources/install.md` & `autoconf-language-server-0.0.5/docs/resources/install.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Install
 
 ## [AUR](https://aur.archlinux.org/packages/autoconf-language-server)
 
 ```sh
-yay -S autoconf-language-server
+yay -S python-autoconf-language-server
 ```
 
 ## [NUR](https://nur.nix-community.org/repos/Freed-Wu)
 
 ```nix
 { config, pkgs, ... }:
 {
```

### Comparing `autoconf-language-server-0.0.4/flake.nix` & `autoconf-language-server-0.0.5/flake.nix`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/pyproject.toml` & `autoconf-language-server-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/src/autoconf_language_server/__main__.py` & `autoconf-language-server-0.0.5/src/autoconf_language_server/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 r"""This module can be called by
 `python -m <https://docs.python.org/3/library/__main__.html>`_.
 """
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
 from contextlib import suppress
 from datetime import datetime
 
+from . import __name__ as NAME
 from . import __version__
 
-VERSION = rf"""autoconf_language_server {__version__}
+NAME = NAME.replace("_", "-")
+VERSION = rf"""{NAME} {__version__}
 Copyright (C) {datetime.now().year}
 Written by Wu Zhenyu
 """
 EPILOG = """
 Report bugs to <wuzhenyu@ustc.edu>.
 """
 
@@ -31,15 +33,14 @@
 
 
 def main():
     r"""Parse arguments and provide shell completions."""
     parser = get_parser()
     parser.parse_args()
 
-    from . import __name__
     from .server import AutoconfLanguageServer
 
-    AutoconfLanguageServer(__name__.replace("_", "-"), __version__).start_io()
+    AutoconfLanguageServer(NAME, __version__).start_io()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `autoconf-language-server-0.0.4/src/autoconf_language_server/api.py` & `autoconf-language-server-0.0.5/src/autoconf_language_server/api.py`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/src/autoconf_language_server/assets/json/autoconf.json` & `autoconf-language-server-0.0.5/src/autoconf_language_server/assets/json/autoconf.json`

 * *Files identical despite different names*

### Comparing `autoconf-language-server-0.0.4/src/autoconf_language_server/server.py` & `autoconf-language-server-0.0.5/src/autoconf_language_server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,22 +109,27 @@
         def completions(params: CompletionParams) -> CompletionList:
             r"""Completions.
 
             :param params:
             :type params: CompletionParams
             :rtype: CompletionList
             """
+            word = self._cursor_word(
+                params.text_document.uri, params.position, False
+            )
+            token = "" if word is None else word[0]
             items = [
                 CompletionItem(
                     label=x,
                     kind=CompletionItemKind.Function,
                     documentation=self.document[x],
                     insert_text=x,
                 )
                 for x in self.document
+                if x.startswith(token)
             ]
             return CompletionList(is_incomplete=False, items=items)
 
     def _cursor_line(self, uri: str, position: Position) -> str:
         r"""Cursor line.
 
         :param uri:
```

### Comparing `autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/PKG-INFO` & `autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoconf-language-server
-Version: 0.0.4
+Version: 0.0.5
 Summary: autoconf language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://autoconf-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/autoconf-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/autoconf-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/autoconf-language-server
```

### Comparing `autoconf-language-server-0.0.4/src/autoconf_language_server.egg-info/SOURCES.txt` & `autoconf-language-server-0.0.5/src/autoconf_language_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

