# Comparing `tmp/create-a-cli-tool-0.5.3.tar.gz` & `tmp/create-a-cli-tool-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-a-cli-tool-0.5.3.tar", last modified: Wed May 17 08:23:03 2023, max compression
+gzip compressed data, was "create-a-cli-tool-0.5.4.tar", last modified: Sun Jun 18 19:57:07 2023, max compression
```

## Comparing `create-a-cli-tool-0.5.3.tar` & `create-a-cli-tool-0.5.4.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.702075 create-a-cli-tool-0.5.3/.github/
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.706075 create-a-cli-tool-0.5.3/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1283 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.github/ISSUE_TEMPLATE/bug_report.yml
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/.github/workflows/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1140 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.github/workflows/ci.yml
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      628 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.github/workflows/publish.yml
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       70 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.gitignore
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      197 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/.readthedocs.yml
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1076 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/LICENSE
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       55 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/MANIFEST.in
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1993 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/PKG-INFO
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1241 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/README.rst
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/cli/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      156 2023-05-17 08:18:21.000000 create-a-cli-tool-0.5.3/cli/__init__.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     8253 2023-05-17 08:15:30.000000 create-a-cli-tool-0.5.3/cli/cli.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     2581 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/commands.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      277 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/errors.py
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/cli/ext/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       21 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/ext/__init__.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      918 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/ext/shard.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/cli/py.typed
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.710075 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1993 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/PKG-INFO
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      741 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/SOURCES.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/dependency_links.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        4 2023-05-17 08:23:03.000000 create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/top_level.txt
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.714075 create-a-cli-tool-0.5.3/docs/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      634 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/Makefile
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      295 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/cli.ext.rst
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      390 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/cli.rst
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     2538 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/conf.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1449 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/index.rst
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      795 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/make.bat
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       46 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/modules.rst
--rw-rw-r--   0 senushka  (1000) senushka  (1000)        4 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/requirements.txt
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1165 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/docs/whats_new.rst
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/examples/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      170 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/arguments.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      165 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/basic_cli.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      248 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/group.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      189 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/no_welcome_messages.py
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      325 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/examples/shard.py
-drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/notes/
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      387 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/notes/basic_cli.md
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      537 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/notes/group_cli.md
--rw-rw-r--   0 senushka  (1000) senushka  (1000)      658 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/notes/shards.md
--rw-rw-r--   0 senushka  (1000) senushka  (1000)       38 2023-05-17 08:23:03.718075 create-a-cli-tool-0.5.3/setup.cfg
--rw-rw-r--   0 senushka  (1000) senushka  (1000)     1394 2023-05-17 07:44:20.000000 create-a-cli-tool-0.5.3/setup.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.827947 create-a-cli-tool-0.5.4/
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.815948 create-a-cli-tool-0.5.4/.github/
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.819948 create-a-cli-tool-0.5.4/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1283 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/.github/ISSUE_TEMPLATE/bug_report.yml
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.819948 create-a-cli-tool-0.5.4/.github/workflows/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1202 2023-06-18 19:52:56.000000 create-a-cli-tool-0.5.4/.github/workflows/ci.yml
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       85 2023-06-18 19:42:38.000000 create-a-cli-tool-0.5.4/.gitignore
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      252 2023-06-18 19:27:50.000000 create-a-cli-tool-0.5.4/.readthedocs.yml
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1076 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/LICENSE
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       55 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/MANIFEST.in
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2044 2023-06-18 19:57:07.827947 create-a-cli-tool-0.5.4/PKG-INFO
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1241 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/README.rst
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.819948 create-a-cli-tool-0.5.4/cli/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      156 2023-06-18 19:02:08.000000 create-a-cli-tool-0.5.4/cli/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     8360 2023-06-18 19:23:11.000000 create-a-cli-tool-0.5.4/cli/cli.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2716 2023-06-18 19:25:13.000000 create-a-cli-tool-0.5.4/cli/commands.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      362 2023-06-18 19:22:24.000000 create-a-cli-tool-0.5.4/cli/errors.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.819948 create-a-cli-tool-0.5.4/cli/ext/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       21 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/cli/ext/__init__.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      918 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/cli/ext/shard.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/cli/py.typed
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.819948 create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2044 2023-06-18 19:57:07.000000 create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/PKG-INFO
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      771 2023-06-18 19:57:07.000000 create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/SOURCES.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        1 2023-06-18 19:57:07.000000 create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/dependency_links.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        4 2023-06-18 19:57:07.000000 create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/top_level.txt
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.823948 create-a-cli-tool-0.5.4/docs/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      634 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/Makefile
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      295 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/cli.ext.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      390 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/cli.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2524 2023-06-18 19:16:58.000000 create-a-cli-tool-0.5.4/docs/conf.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1449 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/index.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      795 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/make.bat
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       46 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/modules.rst
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        4 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/requirements.txt
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1165 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/docs/whats_new.rst
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.823948 create-a-cli-tool-0.5.4/examples/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      171 2023-06-18 19:16:18.000000 create-a-cli-tool-0.5.4/examples/arguments.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      165 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/examples/basic_cli.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      248 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/examples/group.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      189 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/examples/no_welcome_messages.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      325 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/examples/shard.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.823948 create-a-cli-tool-0.5.4/notes/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      387 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/notes/basic_cli.md
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      537 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/notes/group_cli.md
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      658 2023-06-13 17:10:28.000000 create-a-cli-tool-0.5.4/notes/shards.md
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      518 2023-06-18 19:40:38.000000 create-a-cli-tool-0.5.4/pyproject.toml
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)       38 2023-06-18 19:57:07.827947 create-a-cli-tool-0.5.4/setup.cfg
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     1447 2023-06-18 19:12:37.000000 create-a-cli-tool-0.5.4/setup.py
+drwxrwxr-x   0 senushka  (1000) senushka  (1000)        0 2023-06-18 19:57:07.823948 create-a-cli-tool-0.5.4/tests/
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)        0 2023-06-18 17:56:46.000000 create-a-cli-tool-0.5.4/tests/conftest.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)     2321 2023-06-18 19:55:48.000000 create-a-cli-tool-0.5.4/tests/test_main.py
+-rw-rw-r--   0 senushka  (1000) senushka  (1000)      581 2023-06-18 19:46:36.000000 create-a-cli-tool-0.5.4/tox.ini
```

### Comparing `create-a-cli-tool-0.5.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `create-a-cli-tool-0.5.4/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/.github/workflows/ci.yml` & `create-a-cli-tool-0.5.4/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -14,38 +14,39 @@
         uses: actions/setup-python@v2
         with:
           python-version: 3.8
 
       - name: Install & Update Dependencies
         run: |
           pip install --upgrade pip wheel
-          pip install black mypy twine codespell
+          pip install black isort mypy twine codespell
       
-      - name: Run black-mypy-codespell
+      - name: Run black-mypy-codespell-isort
         run: |
           mypy cli
-          black -S --check cli -l 120
+          black --check cli/ tests/
+          isort cli/ tests/
           codespell cli
       
       - name: Run twine checker
         run: |
           rm -rf dist/*
           python3 setup.py sdist
           twine check dist/*
   
   test:
     strategy:
       matrix:
-        os: ['macos-latest', 'windows-latest', 'ubuntu-latest']
-        pyver: ['3.6', '3.7', '3.8', '3.9', '3.10']
+        os: ['windows-latest', 'ubuntu-20.04']
+        pyver: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11']
     runs-on: ${{ matrix.os }}
     steps:
       - name: checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
     
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.pyver }}
       
-      - name: Install
-        run: python3 setup.py install
+      - name: Install and run tox
+        run: pip install -e . && pip install -U tox tox-gh
```

### Comparing `create-a-cli-tool-0.5.3/LICENSE` & `create-a-cli-tool-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/PKG-INFO` & `create-a-cli-tool-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: create-a-cli-tool
-Version: 0.5.3
+Version: 0.5.4
 Summary: A way to make simple python CLIs.
 Home-page: https://github.com/Sengolda/create-a-cli-tool
 Author: Sengolda
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============================================
 Welcome to create-a-cli-tool 👋
```

### Comparing `create-a-cli-tool-0.5.3/README.rst` & `create-a-cli-tool-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/cli/cli.py` & `create-a-cli-tool-0.5.4/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+from __future__ import annotations
+
 import asyncio
 import sys
-from typing import Any, Callable, List, Optional, Union
+from typing import TYPE_CHECKING
 
 from .commands import Command
 from .commands import CommandGroup as Group
 from .errors import *
 
+if TYPE_CHECKING:
+    from typing import Any, Callable, List, Optional, Union
+
+__all__ = ("CLI", )
 
 class CLI:
     """
     The CLI class it self, this will represent your cli.
 
     Parameters
     -----------
@@ -172,15 +178,15 @@
                 if not cmd:
                     print(self.command_not_found_message)
                     args = input(">>> ").split()
 
                 elif type(cmd) == Command:
                     try:
                         cmd._func(*args[1:])
-                    except TypeError as e:
+                    except TypeError:
                         cmd._func()
                     args: List[str] = input(">>> ").split()  # type: ignore
 
                 elif type(cmd) == Group:
                     for subcmd in cmd.children:  # type: ignore
                         if subcmd.name == args[0]:
                             try:
```

### Comparing `create-a-cli-tool-0.5.3/cli/commands.py` & `create-a-cli-tool-0.5.4/cli/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from typing import Any, Callable, Iterator, List, Optional, Type, TypeVar
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 from .errors import CommandAlreadyExists
 
-T = TypeVar("T")
-C = TypeVar(
-    "C",
-    bound="Command",
+if TYPE_CHECKING:
+    from typing import Any, Callable, Iterator, List, Optional, Type, TypeVar
+
+    T = TypeVar("T")
+    C = TypeVar(
+        "C",
+        bound="Command",
+    )
+
+
+__all__ = (
+    "Command",
+    "CommandGroup",
 )
 
 
 class Command:
     def __init__(
         self,
         **kwargs: Any,
     ) -> None:
-        self.name: str = (
-            kwargs.pop(
-                "name",
-                None,
-            )
-            or str(self._func.__name__)
-        )
+        self.name: str = kwargs.pop(
+            "name",
+            None,
+        ) or str(self._func.__name__)
         self._func: Callable = kwargs.pop("func")
         self.description: Optional[str] = (
             kwargs.pop(
                 "description",
                 None,
             )
             or self._func.__doc__
@@ -56,16 +64,16 @@
     def __iter__(
         self,
     ) -> Iterator:
         return iter(self.children)
 
     def command(
         self,
-        name: str = None,
-        description: str = None,
+        name: Optional[str] = None,
+        description: Optional[str] = None,
         aliases: List[Optional[Command]] = [],
     ) -> Callable[..., Any,]:
         def decorator(
             func: Callable[
                 ...,
                 Any,
             ]
```

### Comparing `create-a-cli-tool-0.5.3/cli/ext/shard.py` & `create-a-cli-tool-0.5.4/cli/ext/shard.py`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/PKG-INFO` & `create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: create-a-cli-tool
-Version: 0.5.3
+Version: 0.5.4
 Summary: A way to make simple python CLIs.
 Home-page: https://github.com/Sengolda/create-a-cli-tool
 Author: Sengolda
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============================================
 Welcome to create-a-cli-tool 👋
```

### Comparing `create-a-cli-tool-0.5.3/create_a_cli_tool.egg-info/SOURCES.txt` & `create-a-cli-tool-0.5.4/create_a_cli_tool.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 .gitignore
 .readthedocs.yml
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
+tox.ini
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/workflows/ci.yml
-.github/workflows/publish.yml
 cli/__init__.py
 cli/cli.py
 cli/commands.py
 cli/errors.py
 cli/py.typed
 cli/ext/__init__.py
 cli/ext/shard.py
@@ -30,8 +31,10 @@
 examples/arguments.py
 examples/basic_cli.py
 examples/group.py
 examples/no_welcome_messages.py
 examples/shard.py
 notes/basic_cli.md
 notes/group_cli.md
-notes/shards.md
+notes/shards.md
+tests/conftest.py
+tests/test_main.py
```

### Comparing `create-a-cli-tool-0.5.3/docs/Makefile` & `create-a-cli-tool-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/docs/conf.py` & `create-a-cli-tool-0.5.4/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 
 project = "create-a-cli-tool"
 copyright = "2021, Sengolda"
 author = "Sengolda"
 
 
 with open("../cli/__init__.py", "r", encoding="utf-8") as f:
-    version = re.search(
-        r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE
-    ).group(1)
+    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
 
 
 release = str(version)
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `create-a-cli-tool-0.5.3/docs/index.rst` & `create-a-cli-tool-0.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/docs/make.bat` & `create-a-cli-tool-0.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/docs/whats_new.rst` & `create-a-cli-tool-0.5.4/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/notes/group_cli.md` & `create-a-cli-tool-0.5.4/notes/group_cli.md`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/notes/shards.md` & `create-a-cli-tool-0.5.4/notes/shards.md`

 * *Files identical despite different names*

### Comparing `create-a-cli-tool-0.5.3/setup.py` & `create-a-cli-tool-0.5.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 if not version:
     raise RuntimeError("version not set...")
 
-extra_requires = {"docs": ["sphinx>=4.2.0", "furo"]}
+extras_requires = {"docs": ["sphinx>=4.2.0", "furo"]}
 
 
 packages = ["cli", "cli.ext"]
 
 
 args = dict(
     name="create-a-cli-tool",
@@ -31,17 +31,18 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
     packages=packages,
     include_package_data=True,
     python_requires=">=3.6",  # Cause of f-strings.
     license="MIT",
-    extra_requires=extra_requires,
+    extras_requires=extras_requires,
 )
 
 setup(**args)
```

