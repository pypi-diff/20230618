# Comparing `tmp/foursight_cgap-3.5.0.1b8.tar.gz` & `tmp/foursight_cgap-3.5.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-3.5.0.1b8.tar", max compression
+gzip compressed data, was "foursight_cgap-3.5.0.1b9.tar", max compression
```

## Comparing `foursight_cgap-3.5.0.1b8.tar` & `foursight_cgap-3.5.0.1b9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.5.0.1b8/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.5.0.1b8/chalicelib_cgap/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-09 17:29:40.789199 foursight_cgap-3.5.0.1b8/chalicelib_cgap/app_utils.py
--rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.5.0.1b8/chalicelib_cgap/buckets.py
--rw-r--r--   0        0        0     4995 2023-06-16 20:23:58.006097 foursight_cgap-3.5.0.1b8/chalicelib_cgap/check_schedules.py
--rw-r--r--   0        0        0    17010 2023-06-16 20:23:15.740170 foursight_cgap-3.5.0.1b8/chalicelib_cgap/check_setup.json
--rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.5.0.1b8/chalicelib_cgap/check_setup.json-local
--rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/audit_checks.py
--rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/deployment_checks.py
--rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/es_checks.py
--rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/clone_utils.py
--rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/utils.py
--rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-06-09 17:29:40.792770 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    26338 2023-06-09 17:29:40.793201 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/system_checks.py
--rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/wfr_checks.py
--rw-r--r--   0        0        0    58279 2023-06-16 16:40:36.812730 foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/wrangler_checks.py
--rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.5.0.1b8/chalicelib_cgap/deploy.py
--rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.5.0.1b8/chalicelib_cgap/package.py
--rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.5.0.1b8/chalicelib_cgap/vars.py
--rw-r--r--   0        0        0     1121 2023-06-16 20:34:14.744394 foursight_cgap-3.5.0.1b8/pyproject.toml
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b8/setup.py
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.5.0.1b9/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.5.0.1b9/chalicelib_cgap/__init__.py
+-rw-r--r--   0        0        0     1038 2023-06-09 17:29:40.789199 foursight_cgap-3.5.0.1b9/chalicelib_cgap/app_utils.py
+-rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.5.0.1b9/chalicelib_cgap/buckets.py
+-rw-r--r--   0        0        0     4995 2023-06-16 20:23:58.006097 foursight_cgap-3.5.0.1b9/chalicelib_cgap/check_schedules.py
+-rw-r--r--   0        0        0    17010 2023-06-16 20:23:15.740170 foursight_cgap-3.5.0.1b9/chalicelib_cgap/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.5.0.1b9/chalicelib_cgap/check_setup.json-local
+-rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/__init__.py
+-rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/audit_checks.py
+-rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/es_checks.py
+-rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/clone_utils.py
+-rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-06-09 17:29:40.792770 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    26338 2023-06-09 17:29:40.793201 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/system_checks.py
+-rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/wfr_checks.py
+-rw-r--r--   0        0        0    58279 2023-06-16 16:40:36.812730 foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.5.0.1b9/chalicelib_cgap/deploy.py
+-rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.5.0.1b9/chalicelib_cgap/package.py
+-rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.5.0.1b9/chalicelib_cgap/vars.py
+-rw-r--r--   0        0        0     1121 2023-06-16 21:21:49.170637 foursight_cgap-3.5.0.1b9/pyproject.toml
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b9/setup.py
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.1b9/PKG-INFO
```

### Comparing `foursight_cgap-3.5.0.1b8/LICENSE.txt` & `foursight_cgap-3.5.0.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/app_utils.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/buckets.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/check_schedules.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/check_setup.json` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/check_setup.json-local` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/audit_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/deployment_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/ecs_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/es_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/clone_utils.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/clone_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/lifecycle_utils.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/linecount_dicts.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/utils.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/wfr_utils.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/helpers/wfrset_utils.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/lifecycle_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/system_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/wfr_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/checks/wrangler_checks.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/deploy.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/chalicelib_cgap/package.py` & `foursight_cgap-3.5.0.1b9/chalicelib_cgap/package.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.1b8/pyproject.toml` & `foursight_cgap-3.5.0.1b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-cgap"
-version = "3.5.0.1b8"
+version = "3.5.0.1b9"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_cgap" }
 ]
 
@@ -20,15 +20,15 @@
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 magma-suite = "^1.2.2"
 tibanna-ff = "^1.3.0"
 MarkupSafe = "1.1.1"
-foursight-core = "4.3.0.1b6"
+foursight-core = "4.3.0.1b8"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 cgap-pipeline-utils = "23.0"
 pytest = "5.1.2"
 
 [tool.poetry.dev-dependencies]
 chalice = "^1.21.6"
```

### Comparing `foursight_cgap-3.5.0.1b8/setup.py` & `foursight_cgap-3.5.0.1b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,30 +12,30 @@
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'cgap-pipeline-utils==23.0',
  'click>=7.1.2,<8.0.0',
  'dcicutils==7.5.1.1b1',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.3.0.1b6',
+ 'foursight-core==4.3.0.1b8',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.12.5,<2.0.0',
  'magma-suite>=1.2.2,<2.0.0',
  'pytest==5.1.2',
  'pytz>=2020.1,<2021.0',
  'tibanna-ff>=1.3.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-cgap',
-    'version': '3.5.0.1b8',
+    'version': '3.5.0.1b9',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_cgap-3.5.0.1b8/PKG-INFO` & `foursight_cgap-3.5.0.1b9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-cgap
-Version: 3.5.0.1b8
+Version: 3.5.0.1b9
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: cgap-pipeline-utils (==23.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: dcicutils (==7.5.1.1b1)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.3.0.1b6)
+Requires-Dist: foursight-core (==4.3.0.1b8)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: magma-suite (>=1.2.2,<2.0.0)
 Requires-Dist: pytest (==5.1.2)
 Requires-Dist: pytz (>=2020.1,<2021.0)
 Requires-Dist: tibanna-ff (>=1.3.0,<2.0.0)
```

