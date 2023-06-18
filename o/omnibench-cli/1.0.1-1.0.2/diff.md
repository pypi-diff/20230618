# Comparing `tmp/omnibench_cli-1.0.1.tar.gz` & `tmp/omnibench_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnibench_cli-1.0.1.tar", max compression
+gzip compressed data, was "omnibench_cli-1.0.2.tar", max compression
```

## Comparing `omnibench_cli-1.0.1.tar` & `omnibench_cli-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/LICENSE
--rw-r--r--   0        0        0     1404 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/README.md
--rw-r--r--   0        0        0    16384 2023-06-16 06:19:09.110146 omnibench_cli-1.0.1/omni_cli/.sparql.py.swo
--rw-r--r--   0        0        0        0 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/omni_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/omni_cli/annotator/__init__.py
--rw-r--r--   0        0        0      811 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/omni_cli/annotator/plugin.py
--rw-r--r--   0        0        0     1514 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/omni_cli/benchmarks.py
--rw-r--r--   0        0        0     9275 2023-06-17 09:02:36.653812 omnibench_cli-1.0.1/omni_cli/cli.py
--rw-r--r--   0        0        0     2746 2023-06-17 09:03:35.430755 omnibench_cli-1.0.1/omni_cli/config.py
--rw-r--r--   0        0        0     3830 2023-06-14 13:44:46.223097 omnibench_cli-1.0.1/omni_cli/datasets.py
--rw-r--r--   0        0        0     2955 2023-06-13 16:31:41.305478 omnibench_cli-1.0.1/omni_cli/docker.py
--rw-r--r--   0        0        0     5276 2023-06-17 09:10:44.593643 omnibench_cli-1.0.1/omni_cli/epoch.py
--rw-r--r--   0        0        0     1813 2023-06-17 09:01:56.141161 omnibench_cli-1.0.1/omni_cli/graph.py
--rw-r--r--   0        0        0      275 2023-06-13 16:31:41.305478 omnibench_cli-1.0.1/omni_cli/model.py
--rw-r--r--   0        0        0     2617 2023-06-14 13:24:08.584609 omnibench_cli-1.0.1/omni_cli/orchestrator.py
--rw-r--r--   0        0        0      831 2023-06-17 10:48:44.868101 omnibench_cli-1.0.1/omni_cli/plot.py
--rw-r--r--   0        0        0      366 2023-06-14 05:23:45.201152 omnibench_cli-1.0.1/omni_cli/project.py
--rw-r--r--   0        0        0      566 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/omni_cli/resources.py
--rw-r--r--   0        0        0    14067 2023-06-17 11:13:03.853172 omnibench_cli-1.0.1/omni_cli/sparql.py
--rw-r--r--   0        0        0      847 2023-05-30 10:20:26.027438 omnibench_cli-1.0.1/omni_cli/sync.py
--rw-r--r--   0        0        0     5248 2023-06-14 16:47:33.073526 omnibench_cli-1.0.1/omni_cli/workflow.py
--rw-r--r--   0        0        0     1432 2023-06-18 09:39:58.599212 omnibench_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2643 1970-01-01 00:00:00.000000 omnibench_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1408 2023-06-18 09:46:05.388934 omnibench_cli-1.0.2/README.md
+-rw-r--r--   0        0        0    16384 2023-06-16 06:19:09.110146 omnibench_cli-1.0.2/omni_cli/.sparql.py.swo
+-rw-r--r--   0        0        0        0 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/omni_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/omni_cli/annotator/__init__.py
+-rw-r--r--   0        0        0      811 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/omni_cli/annotator/plugin.py
+-rw-r--r--   0        0        0     1514 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/omni_cli/benchmarks.py
+-rw-r--r--   0        0        0     9275 2023-06-17 09:02:36.653812 omnibench_cli-1.0.2/omni_cli/cli.py
+-rw-r--r--   0        0        0     2746 2023-06-17 09:03:35.430755 omnibench_cli-1.0.2/omni_cli/config.py
+-rw-r--r--   0        0        0     3830 2023-06-14 13:44:46.223097 omnibench_cli-1.0.2/omni_cli/datasets.py
+-rw-r--r--   0        0        0     2955 2023-06-13 16:31:41.305478 omnibench_cli-1.0.2/omni_cli/docker.py
+-rw-r--r--   0        0        0     5276 2023-06-17 09:10:44.593643 omnibench_cli-1.0.2/omni_cli/epoch.py
+-rw-r--r--   0        0        0     1813 2023-06-17 09:01:56.141161 omnibench_cli-1.0.2/omni_cli/graph.py
+-rw-r--r--   0        0        0      275 2023-06-13 16:31:41.305478 omnibench_cli-1.0.2/omni_cli/model.py
+-rw-r--r--   0        0        0     2617 2023-06-14 13:24:08.584609 omnibench_cli-1.0.2/omni_cli/orchestrator.py
+-rw-r--r--   0        0        0      831 2023-06-17 10:48:44.868101 omnibench_cli-1.0.2/omni_cli/plot.py
+-rw-r--r--   0        0        0      366 2023-06-14 05:23:45.201152 omnibench_cli-1.0.2/omni_cli/project.py
+-rw-r--r--   0        0        0      566 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/omni_cli/resources.py
+-rw-r--r--   0        0        0    14067 2023-06-17 11:13:03.853172 omnibench_cli-1.0.2/omni_cli/sparql.py
+-rw-r--r--   0        0        0      847 2023-05-30 10:20:26.027438 omnibench_cli-1.0.2/omni_cli/sync.py
+-rw-r--r--   0        0        0     5248 2023-06-14 16:47:33.073526 omnibench_cli-1.0.2/omni_cli/workflow.py
+-rw-r--r--   0        0        0     1431 2023-06-18 09:47:30.278252 omnibench_cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2655 1970-01-01 00:00:00.000000 omnibench_cli-1.0.2/PKG-INFO
```

### Comparing `omnibench_cli-1.0.1/LICENSE` & `omnibench_cli-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/README.md` & `omnibench_cli-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # omni-cli
 
 A command line interface to query and access datasets and workflows project-wide across omnibenchmark.
 
-## Use
+## Install
+
+Install via pip:
+
+```
+pip install omnibench-cli
+```
 
-Until this project reaches enough maturity to be published in pypi, you can use `poetry` to use it:
+While developing, you can use poetry:
 
 ```
 pip install poetry
 poetry shell
 ```
 
+## Use
+
+
 ```zsh
 ❯ omni_cli
 Usage: omni_cli [OPTIONS] COMMAND [ARGS]...
 
   Interact with omnibenchmark datasets and workflows.
 
 Options:
```

### Comparing `omnibench_cli-1.0.1/omni_cli/.sparql.py.swo` & `omnibench_cli-1.0.2/omni_cli/.sparql.py.swo`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/annotator/plugin.py` & `omnibench_cli-1.0.2/omni_cli/annotator/plugin.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/benchmarks.py` & `omnibench_cli-1.0.2/omni_cli/benchmarks.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/cli.py` & `omnibench_cli-1.0.2/omni_cli/cli.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/config.py` & `omnibench_cli-1.0.2/omni_cli/config.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/datasets.py` & `omnibench_cli-1.0.2/omni_cli/datasets.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/docker.py` & `omnibench_cli-1.0.2/omni_cli/docker.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/epoch.py` & `omnibench_cli-1.0.2/omni_cli/epoch.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/graph.py` & `omnibench_cli-1.0.2/omni_cli/graph.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/orchestrator.py` & `omnibench_cli-1.0.2/omni_cli/orchestrator.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/plot.py` & `omnibench_cli-1.0.2/omni_cli/plot.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/resources.py` & `omnibench_cli-1.0.2/omni_cli/resources.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/sparql.py` & `omnibench_cli-1.0.2/omni_cli/sparql.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/sync.py` & `omnibench_cli-1.0.2/omni_cli/sync.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/omni_cli/workflow.py` & `omnibench_cli-1.0.2/omni_cli/workflow.py`

 * *Files identical despite different names*

### Comparing `omnibench_cli-1.0.1/pyproject.toml` & `omnibench_cli-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omnibench-cli"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 authors = ["btraven <btraven@sdf.org>"]
 readme = "README.md"
 packages = [{include = "omni_cli"}]
 homepage = "https://renkulab.io/gitlab/btraven/omni-cli/"
 repository = "https://renkulab.io/gitlab/btraven/omni-cli/"
 classifiers = [
@@ -30,15 +30,15 @@
 renku = "^2.3.2"
 sparqlwrapper = "^2.0.0"
 
 # for dev
 # calamus = {git = "https://github.com/btraven00/calamus", rev = "master"}
 # omnibenchmark = {git = "https://github.com/omnibenchmark/omnibenchmark-py"} #, rev = "0.0.43"}
 calamus = "^0.4.2"
-omnibenchmark = ">=0.0.44"
+omnibenchmark = "^0.0.43"
 
 [tool.poetry.scripts]
 omni_cli = 'omni_cli.cli:run'
 
 [tool.poetry.plugins."renku"]
 activity_annotator = 'omni_cli.annotator.plugin'
```

### Comparing `omnibench_cli-1.0.1/PKG-INFO` & `omnibench_cli-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnibench-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Home-page: https://renkulab.io/gitlab/btraven/omni-cli/
 Author: btraven
 Author-email: btraven@sdf.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,36 +16,45 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: calamus (>=0.4.2,<0.5.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: omnibenchmark (>=0.0.44)
+Requires-Dist: omnibenchmark (>=0.0.43,<0.0.44)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: renku (>=2.3.2,<3.0.0)
 Requires-Dist: requests (<2.28.2)
 Requires-Dist: sparqlwrapper (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://renkulab.io/gitlab/btraven/omni-cli/
 Description-Content-Type: text/markdown
 
 # omni-cli
 
 A command line interface to query and access datasets and workflows project-wide across omnibenchmark.
 
-## Use
+## Install
+
+Install via pip:
+
+```
+pip install omnibench-cli
+```
 
-Until this project reaches enough maturity to be published in pypi, you can use `poetry` to use it:
+While developing, you can use poetry:
 
 ```
 pip install poetry
 poetry shell
 ```
 
+## Use
+
+
 ```zsh
 ❯ omni_cli
 Usage: omni_cli [OPTIONS] COMMAND [ARGS]...
 
   Interact with omnibenchmark datasets and workflows.
 
 Options:
```

