# Comparing `tmp/acore_server_config-0.2.2.tar.gz` & `tmp/acore_server_config-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.2.2.tar", last modified: Sun Jun 18 04:26:00 2023, max compression
+gzip compressed data, was "acore_server_config-0.2.3.tar", last modified: Sun Jun 18 04:28:42 2023, max compression
```

## Comparing `acore_server_config-0.2.2.tar` & `acore_server_config-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.738512 acore_server_config-0.2.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 04:26:00.738361 acore_server_config-0.2.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.2.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.735539 acore_server_config-0.2.2/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.2.2/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 04:20:28.000000 acore_server_config-0.2.2/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.2.2/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-06-18 03:18:29.000000 acore_server_config-0.2.2/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.2.2/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.736356 acore_server_config-0.2.2/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.2.2/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.736963 acore_server_config-0.2.2/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.2.2/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.2.2/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1344 2023-06-18 03:28:21.000000 acore_server_config-0.2.2/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.2.2/acore_server_config/config/init.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.737092 acore_server_config-0.2.2/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3796 2023-06-18 04:23:34.000000 acore_server_config-0.2.2/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.2.2/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.2.2/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.737616 acore_server_config-0.2.2/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/acore_server_config/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.737931 acore_server_config-0.2.2/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.736113 acore_server_config-0.2.2/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 04:26:00.000000 acore_server_config-0.2.2/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 04:26:00.000000 acore_server_config-0.2.2/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 04:26:00.000000 acore_server_config-0.2.2/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 04:26:00.000000 acore_server_config-0.2.2/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 04:26:00.000000 acore_server_config-0.2.2/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2067 2023-06-18 04:24:50.000000 acore_server_config-0.2.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.2.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.2.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 04:26:00.738556 acore_server_config-0.2.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.2.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:26:00.738073 acore_server_config-0.2.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.2.2/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.099775 acore_server_config-0.2.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 04:28:42.099644 acore_server_config-0.2.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.2.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.096229 acore_server_config-0.2.3/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.2.3/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 04:27:52.000000 acore_server_config-0.2.3/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.2.3/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-06-18 03:18:29.000000 acore_server_config-0.2.3/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.2.3/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.097494 acore_server_config-0.2.3/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.2.3/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.098253 acore_server_config-0.2.3/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.2.3/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.2.3/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1344 2023-06-18 03:28:21.000000 acore_server_config-0.2.3/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.2.3/acore_server_config/config/init.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.098456 acore_server_config-0.2.3/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3779 2023-06-18 04:27:33.000000 acore_server_config-0.2.3/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.2.3/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.2.3/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.098892 acore_server_config-0.2.3/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.099232 acore_server_config-0.2.3/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.097043 acore_server_config-0.2.3/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 04:28:42.000000 acore_server_config-0.2.3/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2265 2023-06-18 04:28:15.000000 acore_server_config-0.2.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.2.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.2.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 04:28:42.099820 acore_server_config-0.2.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.2.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 04:28:42.099378 acore_server_config-0.2.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.2.3/tests/test_api.py
```

### Comparing `acore_server_config-0.2.2/AUTHORS.rst` & `acore_server_config-0.2.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/LICENSE.txt` & `acore_server_config-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/PKG-INFO` & `acore_server_config-0.2.3/acore_server_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore_server_config
-Version: 0.2.2
+Name: acore-server-config
+Version: 0.2.3
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.2.2/README.rst` & `acore_server_config-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/boto_ses.py` & `acore_server_config-0.2.3/acore_server_config/boto_ses.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/config/define/main.py` & `acore_server_config-0.2.3/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/config/define/server.py` & `acore_server_config-0.2.3/acore_server_config/config/define/server.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/config/init.py` & `acore_server_config-0.2.3/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/in_ec2.py` & `acore_server_config-0.2.3/acore_server_config/in_ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 def _get_default_parameter_name_prefix() -> str:
     return "acore_server_config"
 
 
 def get_server(
     bsm: "BotoSesManager" = default_bsm,
-    parameter_name_prefix: T.Optional[str] = "acore_server_config",
+    parameter_name_prefix: T.Optional[str] = None,
     use_s3: bool = True,
     use_parameter_store: bool = False,
     s3folder_config: T.Optional[str] = None,
     server_id: T.Optional[str] = None,
 ) -> Server:
     """
     在 EC2 上通过 "自省", 获得属于这个服务器的配置数据.
```

### Comparing `acore_server_config-0.2.2/acore_server_config/paths.py` & `acore_server_config-0.2.3/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/runtime.py` & `acore_server_config-0.2.3/acore_server_config/runtime.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.2.3/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: acore-server-config
-Version: 0.2.2
+Name: acore_server_config
+Version: 0.2.3
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.2.2/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.2.3/acore_server_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/release-history.rst` & `acore_server_config-0.2.3/release-history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.3 (2023-06-18)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a parameter default value typo in ``acore_server_config.api.get_server`` API.
+
+
 0.2.2 (2023-06-18)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that the key forget to pass ``parameter_name`` to ``Config.read`` method in ``acore_server_config.api.get_server`` API.
```

### Comparing `acore_server_config-0.2.2/requirements-doc.txt` & `acore_server_config-0.2.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.2.2/setup.py` & `acore_server_config-0.2.3/setup.py`

 * *Files identical despite different names*

