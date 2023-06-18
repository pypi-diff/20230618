# Comparing `tmp/aioworldline-0.0.6.tar.gz` & `tmp/aioworldline-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworldline-0.0.6.tar", last modified: Tue May 23 19:23:34 2023, max compression
+gzip compressed data, was "aioworldline-0.0.7.tar", last modified: Sun Jun 18 18:37:30 2023, max compression
```

## Comparing `aioworldline-0.0.6.tar` & `aioworldline-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.191505 aioworldline-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-23 19:23:21.000000 aioworldline-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.187505 aioworldline-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.187505 aioworldline-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-23 19:23:21.000000 aioworldline-0.0.6/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 19:23:21.000000 aioworldline-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 19:23:21.000000 aioworldline-0.0.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 19:23:21.000000 aioworldline-0.0.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-05-23 19:23:21.000000 aioworldline-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-23 19:23:34.191505 aioworldline-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-23 19:23:21.000000 aioworldline-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 19:23:21.000000 aioworldline-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.187505 aioworldline-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.187505 aioworldline-0.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 19:23:21.000000 aioworldline-0.0.6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 19:23:21.000000 aioworldline-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 19:23:21.000000 aioworldline-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 19:23:21.000000 aioworldline-0.0.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-23 19:23:34.191505 aioworldline-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-23 19:23:21.000000 aioworldline-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.187505 aioworldline-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.191505 aioworldline-0.0.6/src/aioworldline/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-23 19:23:21.000000 aioworldline-0.0.6/src/aioworldline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-23 19:23:21.000000 aioworldline-0.0.6/src/aioworldline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 19:23:21.000000 aioworldline-0.0.6/src/aioworldline/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-23 19:23:21.000000 aioworldline-0.0.6/src/aioworldline/worldline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.191505 aioworldline-0.0.6/src/aioworldline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-23 19:23:34.000000 aioworldline-0.0.6/src/aioworldline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 19:23:34.000000 aioworldline-0.0.6/src/aioworldline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:23:34.000000 aioworldline-0.0.6/src/aioworldline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:23:34.000000 aioworldline-0.0.6/src/aioworldline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 19:23:34.000000 aioworldline-0.0.6/src/aioworldline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 19:23:34.000000 aioworldline-0.0.6/src/aioworldline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:23:34.191505 aioworldline-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-23 19:23:21.000000 aioworldline-0.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-18 18:37:14.000000 aioworldline-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.798086 aioworldline-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-18 18:37:14.000000 aioworldline-0.0.7/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-18 18:37:14.000000 aioworldline-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-18 18:37:14.000000 aioworldline-0.0.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-18 18:37:14.000000 aioworldline-0.0.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34575 2023-06-18 18:37:14.000000 aioworldline-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-18 18:37:30.802086 aioworldline-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-18 18:37:14.000000 aioworldline-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-18 18:37:14.000000 aioworldline-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-18 18:37:14.000000 aioworldline-0.0.7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-18 18:37:14.000000 aioworldline-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 18:37:14.000000 aioworldline-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-18 18:37:14.000000 aioworldline-0.0.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-18 18:37:30.806086 aioworldline-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-18 18:37:14.000000 aioworldline-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.798086 aioworldline-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/src/aioworldline/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-18 18:37:14.000000 aioworldline-0.0.7/src/aioworldline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-18 18:37:14.000000 aioworldline-0.0.7/src/aioworldline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-18 18:37:14.000000 aioworldline-0.0.7/src/aioworldline/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-18 18:37:14.000000 aioworldline-0.0.7/src/aioworldline/worldline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/src/aioworldline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-18 18:37:30.000000 aioworldline-0.0.7/src/aioworldline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-18 18:37:30.000000 aioworldline-0.0.7/src/aioworldline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:37:30.000000 aioworldline-0.0.7/src/aioworldline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 18:37:30.000000 aioworldline-0.0.7/src/aioworldline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-18 18:37:30.000000 aioworldline-0.0.7/src/aioworldline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 18:37:30.000000 aioworldline-0.0.7/src/aioworldline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 18:37:30.802086 aioworldline-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-18 18:37:14.000000 aioworldline-0.0.7/tests/conftest.py
```

### Comparing `aioworldline-0.0.6/.coveragerc` & `aioworldline-0.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/.github/workflows/python-publish.yaml` & `aioworldline-0.0.7/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/.gitignore` & `aioworldline-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/LICENSE` & `aioworldline-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/PKG-INFO` & `aioworldline-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioworldline
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unofficial Worldline portal data retrieving client
 Home-page: https://github.com/kamikaze/aioworldline
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/aioworldline/wiki
 Platform: any
```

### Comparing `aioworldline-0.0.6/docs/Makefile` & `aioworldline-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/docs/conf.py` & `aioworldline-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/docs/index.rst` & `aioworldline-0.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/setup.cfg` & `aioworldline-0.0.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aioworldline
-version = 0.0.6
+version = 0.0.7
 description = Unofficial Worldline portal data retrieving client
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/aioworldline
@@ -20,15 +20,15 @@
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	aiohttp[speedups]==3.8.4
-	pydantic==1.10.8
+	pydantic==1.10.9
 python_requires = >=3.11
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `aioworldline-0.0.6/src/aioworldline/worldline.py` & `aioworldline-0.0.7/src/aioworldline/worldline.py`

 * *Files identical despite different names*

### Comparing `aioworldline-0.0.6/src/aioworldline.egg-info/PKG-INFO` & `aioworldline-0.0.7/src/aioworldline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioworldline
-Version: 0.0.6
+Version: 0.0.7
 Summary: Unofficial Worldline portal data retrieving client
 Home-page: https://github.com/kamikaze/aioworldline
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/aioworldline/wiki
 Platform: any
```

### Comparing `aioworldline-0.0.6/src/aioworldline.egg-info/SOURCES.txt` & `aioworldline-0.0.7/src/aioworldline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

