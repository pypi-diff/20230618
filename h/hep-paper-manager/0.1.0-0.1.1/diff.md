# Comparing `tmp/hep_paper_manager-0.1.0.tar.gz` & `tmp/hep_paper_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hep_paper_manager-0.1.0.tar", max compression
+gzip compressed data, was "hep_paper_manager-0.1.1.tar", max compression
```

## Comparing `hep_paper_manager-0.1.0.tar` & `hep_paper_manager-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3394 2023-06-18 13:32:30.848233 hep_paper_manager-0.1.0/README.md
--rw-r--r--   0        0        0      366 2023-06-14 06:58:09.956795 hep_paper_manager-0.1.0/hpm/__init__.py
--rw-r--r--   0        0        0     5212 2023-06-18 11:14:15.458279 hep_paper_manager-0.1.0/hpm/cli.py
--rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.0/hpm/engines/__init__.py
--rw-r--r--   0        0        0     3298 2023-06-13 13:22:03.054110 hep_paper_manager-0.1.0/hpm/engines/inspire.py
--rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.0/hpm/notion/__init__.py
--rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.0/hpm/notion/client.py
--rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.0/hpm/notion/objects/__init__.py
--rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.0/hpm/notion/objects/database.py
--rw-r--r--   0        0        0     3682 2023-06-13 04:13:54.692063 hep_paper_manager-0.1.0/hpm/notion/objects/page.py
--rw-r--r--   0        0        0     5166 2023-06-18 11:18:06.402552 hep_paper_manager-0.1.0/hpm/notion/properties.py
--rw-r--r--   0        0        0      170 2023-06-14 06:27:04.634648 hep_paper_manager-0.1.0/hpm/templates/paper.yml
--rw-r--r--   0        0        0      699 2023-06-18 13:54:02.388167 hep_paper_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4043 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3413 2023-06-18 14:30:01.910184 hep_paper_manager-0.1.1/README.md
+-rw-r--r--   0        0        0      366 2023-06-14 06:58:09.956795 hep_paper_manager-0.1.1/hpm/__init__.py
+-rw-r--r--   0        0        0     5212 2023-06-18 11:14:15.458279 hep_paper_manager-0.1.1/hpm/cli.py
+-rw-r--r--   0        0        0       29 2023-06-13 04:12:40.062240 hep_paper_manager-0.1.1/hpm/engines/__init__.py
+-rw-r--r--   0        0        0     3298 2023-06-13 13:22:03.054110 hep_paper_manager-0.1.1/hpm/engines/inspire.py
+-rw-r--r--   0        0        0       27 2023-06-13 04:13:59.907266 hep_paper_manager-0.1.1/hpm/notion/__init__.py
+-rw-r--r--   0        0        0     3427 2023-06-18 11:18:06.400535 hep_paper_manager-0.1.1/hpm/notion/client.py
+-rw-r--r--   0        0        0       54 2023-06-13 04:13:42.598101 hep_paper_manager-0.1.1/hpm/notion/objects/__init__.py
+-rw-r--r--   0        0        0      962 2023-06-13 04:13:47.941688 hep_paper_manager-0.1.1/hpm/notion/objects/database.py
+-rw-r--r--   0        0        0     3682 2023-06-13 04:13:54.692063 hep_paper_manager-0.1.1/hpm/notion/objects/page.py
+-rw-r--r--   0        0        0     5166 2023-06-18 11:18:06.402552 hep_paper_manager-0.1.1/hpm/notion/properties.py
+-rw-r--r--   0        0        0      170 2023-06-14 06:27:04.634648 hep_paper_manager-0.1.1/hpm/templates/paper.yml
+-rw-r--r--   0        0        0      698 2023-06-18 14:30:01.910522 hep_paper_manager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 hep_paper_manager-0.1.1/PKG-INFO
```

### Comparing `hep_paper_manager-0.1.0/README.md` & `hep_paper_manager-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 ## Features
 - Fetch HEP papers via the Inspire engine.
 - Directly add fetched papers to your Notion database.
 - Interactive CLI for easy setup and usage.
 
 ## Installation
-Under building...
+```
+pip install hep-paper-manager
+```
 
 ## Usage
 > Before using `hpm`, check this [link](https://developers.notion.com/docs/create-a-notion-integration) to create an integration with the Notion API to let `hpm` work with your database.
 
 1. Use `hpm init` to set up HPM:
    ```
    hpm init
@@ -68,11 +70,11 @@
     title: Title
     journal: Journal
     authors: Authors
     abstract: Abstract
   ```
 
 ## Updates
-### v0.1.0
+### v0.1.1
 - Add `hpm init` for interactive setup.
 - Add `hpm add` for adding a paper to a Notion database.
-- Introduce the default `Inspire` engine and `paper.yml` template.
+- Introduce the default `Inspire` engine and `paper.yml` template.
```

### Comparing `hep_paper_manager-0.1.0/hpm/cli.py` & `hep_paper_manager-0.1.1/hpm/cli.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.0/hpm/engines/inspire.py` & `hep_paper_manager-0.1.1/hpm/engines/inspire.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.0/hpm/notion/client.py` & `hep_paper_manager-0.1.1/hpm/notion/client.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.0/hpm/notion/objects/database.py` & `hep_paper_manager-0.1.1/hpm/notion/objects/database.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.0/hpm/notion/objects/page.py` & `hep_paper_manager-0.1.1/hpm/notion/objects/page.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.0/hpm/notion/properties.py` & `hep_paper_manager-0.1.1/hpm/notion/properties.py`

 * *Files identical despite different names*

### Comparing `hep_paper_manager-0.1.0/pyproject.toml` & `hep_paper_manager-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hep-paper-manager"
-version = "0.1.0"
+version = "0.1.1"
 description = "HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database."
 authors = ["Star9daisy <star9daisy@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "hpm" },
 ]
 
@@ -23,8 +23,8 @@
 black = "^23.3.0"
 pytest = "^7.3.1"
 python-dotenv = "^1.0.0"
 deptry = "^0.11.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hep_paper_manager-0.1.0/PKG-INFO` & `hep_paper_manager-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hep-paper-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: HPM is a command-line tool that adds High Energy Physics (HEP) papers to a Notion database.
 Author: Star9daisy
 Author-email: star9daisy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,15 +21,17 @@
 
 ## Features
 - Fetch HEP papers via the Inspire engine.
 - Directly add fetched papers to your Notion database.
 - Interactive CLI for easy setup and usage.
 
 ## Installation
-Under building...
+```
+pip install hep-paper-manager
+```
 
 ## Usage
 > Before using `hpm`, check this [link](https://developers.notion.com/docs/create-a-notion-integration) to create an integration with the Notion API to let `hpm` work with your database.
 
 1. Use `hpm init` to set up HPM:
    ```
    hpm init
@@ -85,12 +87,11 @@
     title: Title
     journal: Journal
     authors: Authors
     abstract: Abstract
   ```
 
 ## Updates
-### v0.1.0
+### v0.1.1
 - Add `hpm init` for interactive setup.
 - Add `hpm add` for adding a paper to a Notion database.
 - Introduce the default `Inspire` engine and `paper.yml` template.
-
```

