# Comparing `tmp/spatiafi-1.1.2.tar.gz` & `tmp/spatiafi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatiafi-1.1.2.tar", last modified: Sat Jun 17 16:44:30 2023, max compression
+gzip compressed data, was "spatiafi-1.1.3.tar", last modified: Sun Jun 18 00:53:35 2023, max compression
```

## Comparing `spatiafi-1.1.2.tar` & `spatiafi-1.1.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.836315 spatiafi-1.1.2/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.2/.dockerignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.2/.gitignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.2/.pre-commit-config.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.2/.requirements.sha256
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.2/Dockerfile
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.2/LICENSE
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-17 16:44:30.836315 spatiafi-1.1.2/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.2/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.2/pyproject.toml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.2/requirements-dev.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.2/requirements.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.832314 spatiafi-1.1.2/scripts/
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.2/scripts/bootstrap_dev.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.2/scripts/build_docker.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.2/scripts/gen_requirements.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.2/scripts/install_package.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.2/scripts/test.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-17 16:44:05.000000 spatiafi-1.1.2/scripts/upload_pypi.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      921 2023-06-17 16:44:30.836315 spatiafi-1.1.2/setup.cfg
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.2/setup.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.828314 spatiafi-1.1.2/src/
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.832314 spatiafi-1.1.2/src/spatiafi/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.2/src/spatiafi/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.2/src/spatiafi/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi/_version.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.2/src/spatiafi/auth.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.832314 spatiafi-1.1.2/src/spatiafi/gdal_auth/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       21 2023-06-17 16:27:44.000000 spatiafi-1.1.2/src/spatiafi/gdal_auth/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.2/src/spatiafi/gdal_auth/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.2/src/spatiafi/gdal_auth/cli.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2828 2023-06-17 16:27:45.000000 spatiafi-1.1.2/src/spatiafi/gdal_auth/gdal_auth.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.2/src/spatiafi/session.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.832314 spatiafi-1.1.2/src/spatiafi.egg-info/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi.egg-info/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi.egg-info/SOURCES.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi.egg-info/dependency_links.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi.egg-info/entry_points.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      222 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi.egg-info/requires.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-17 16:44:30.000000 spatiafi-1.1.2/src/spatiafi.egg-info/top_level.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.836315 spatiafi-1.1.2/tests/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.2/tests/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.2/tests/test_dummy.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-17 16:44:30.836315 spatiafi-1.1.2/workflows/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.2/workflows/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.2/workflows/delpoy-sensor.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.2/workflows/kustomization.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.2/workflows/py-spfi-api-build-wf.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.2/workflows/repo-sensor.yaml
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.2/workflows/submit-wf.sh
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.3/.dockerignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.3/.gitignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.3/.pre-commit-config.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.3/.requirements.sha256
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.3/Dockerfile
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.3/LICENSE
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-18 00:53:35.683115 spatiafi-1.1.3/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.3/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.3/pyproject.toml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.3/requirements-dev.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.3/requirements.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/scripts/
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.3/scripts/bootstrap_dev.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.3/scripts/build_docker.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.3/scripts/gen_requirements.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.3/scripts/install_package.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.3/scripts/test.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-17 16:44:05.000000 spatiafi-1.1.3/scripts/upload_pypi.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-06-18 00:53:35.687115 spatiafi-1.1.3/setup.cfg
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.3/setup.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.679115 spatiafi-1.1.3/src/
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/src/spatiafi/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.3/src/spatiafi/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.3/src/spatiafi/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi/_version.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.3/src/spatiafi/auth.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/src/spatiafi/gdal_auth/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       21 2023-06-17 16:27:44.000000 spatiafi-1.1.3/src/spatiafi/gdal_auth/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.3/src/spatiafi/gdal_auth/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.3/src/spatiafi/gdal_auth/cli.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4499 2023-06-18 00:52:55.000000 spatiafi-1.1.3/src/spatiafi/gdal_auth/gdal_auth.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.3/src/spatiafi/session.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/src/spatiafi.egg-info/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi.egg-info/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi.egg-info/entry_points.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi.egg-info/requires.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-18 00:53:35.000000 spatiafi-1.1.3/src/spatiafi.egg-info/top_level.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/tests/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.3/tests/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.3/tests/test_dummy.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-18 00:53:35.683115 spatiafi-1.1.3/workflows/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.3/workflows/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.3/workflows/delpoy-sensor.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.3/workflows/kustomization.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.3/workflows/py-spfi-api-build-wf.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.3/workflows/repo-sensor.yaml
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.3/workflows/submit-wf.sh
```

### Comparing `spatiafi-1.1.2/.dockerignore` & `spatiafi-1.1.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/.gitignore` & `spatiafi-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/.pre-commit-config.yaml` & `spatiafi-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/Dockerfile` & `spatiafi-1.1.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/LICENSE` & `spatiafi-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/PKG-INFO` & `spatiafi-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.2/README.md` & `spatiafi-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/pyproject.toml` & `spatiafi-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/requirements-dev.txt` & `spatiafi-1.1.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/requirements.txt` & `spatiafi-1.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/scripts/bootstrap_dev.sh` & `spatiafi-1.1.3/scripts/bootstrap_dev.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/scripts/gen_requirements.sh` & `spatiafi-1.1.3/scripts/gen_requirements.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/setup.cfg` & `spatiafi-1.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 	= src
 packages = find_namespace:
 python_requires = >=3.10
 include_package_data = true
 install_requires = 
 	authlib
 	click
-	requests
 	httpx
+	platformdirs
+	requests
 
 [options.extras_require]
 dev = # Specify dev dependencies here
 	autoflake
 	black
 	build
 	flake8
```

### Comparing `spatiafi-1.1.2/src/spatiafi/auth.py` & `spatiafi-1.1.3/src/spatiafi/auth.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/src/spatiafi/gdal_auth/cli.py` & `spatiafi-1.1.3/src/spatiafi/gdal_auth/cli.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/src/spatiafi/session.py` & `spatiafi-1.1.3/src/spatiafi/session.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/src/spatiafi.egg-info/PKG-INFO` & `spatiafi-1.1.3/src/spatiafi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.2/src/spatiafi.egg-info/SOURCES.txt` & `spatiafi-1.1.3/src/spatiafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/workflows/README.md` & `spatiafi-1.1.3/workflows/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/workflows/delpoy-sensor.sh` & `spatiafi-1.1.3/workflows/delpoy-sensor.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/workflows/repo-sensor.yaml` & `spatiafi-1.1.3/workflows/repo-sensor.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.2/workflows/submit-wf.sh` & `spatiafi-1.1.3/workflows/submit-wf.sh`

 * *Files identical despite different names*

