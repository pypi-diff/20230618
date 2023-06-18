# Comparing `tmp/acore_server_config-0.1.2.tar.gz` & `tmp/acore_server_config-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.1.2.tar", last modified: Sun Jun 18 02:03:24 2023, max compression
+gzip compressed data, was "acore_server_config-0.1.3.tar", last modified: Sun Jun 18 02:07:54 2023, max compression
```

## Comparing `acore_server_config-0.1.2.tar` & `acore_server_config-0.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.041008 acore_server_config-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 02:03:24.040874 acore_server_config-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.1.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.037690 acore_server_config-0.1.2/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.1.2/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 02:01:51.000000 acore_server_config-0.1.2/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.1.2/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      592 2023-06-18 00:51:40.000000 acore_server_config-0.1.2/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.1.2/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.038818 acore_server_config-0.1.2/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.1.2/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.039485 acore_server_config-0.1.2/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.1.2/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.1.2/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1098 2023-06-18 01:09:41.000000 acore_server_config-0.1.2/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.1.2/acore_server_config/config/init.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.039707 acore_server_config-0.1.2/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1865 2023-06-18 02:01:44.000000 acore_server_config-0.1.2/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.1.2/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.1.2/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.040135 acore_server_config-0.1.2/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/acore_server_config/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.040460 acore_server_config-0.1.2/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.038454 acore_server_config-0.1.2/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 02:03:24.000000 acore_server_config-0.1.2/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 02:03:24.000000 acore_server_config-0.1.2/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 02:03:24.000000 acore_server_config-0.1.2/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 02:03:24.000000 acore_server_config-0.1.2/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 02:03:24.000000 acore_server_config-0.1.2/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1317 2023-06-18 02:02:50.000000 acore_server_config-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 02:03:24.041051 acore_server_config-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:03:24.040600 acore_server_config-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.1.2/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.110687 acore_server_config-0.1.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 02:07:54.110531 acore_server_config-0.1.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.1.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.107208 acore_server_config-0.1.3/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.1.3/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 02:06:28.000000 acore_server_config-0.1.3/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.1.3/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      592 2023-06-18 00:51:40.000000 acore_server_config-0.1.3/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.1.3/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.108316 acore_server_config-0.1.3/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.1.3/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.109063 acore_server_config-0.1.3/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.1.3/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.1.3/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1098 2023-06-18 01:09:41.000000 acore_server_config-0.1.3/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.1.3/acore_server_config/config/init.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.109302 acore_server_config-0.1.3/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1867 2023-06-18 02:06:22.000000 acore_server_config-0.1.3/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.1.3/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.1.3/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.109747 acore_server_config-0.1.3/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.110077 acore_server_config-0.1.3/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.107915 acore_server_config-0.1.3/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1539 2023-06-18 02:07:23.000000 acore_server_config-0.1.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.1.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.1.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 02:07:54.110732 acore_server_config-0.1.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.110218 acore_server_config-0.1.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.1.3/tests/test_api.py
```

### Comparing `acore_server_config-0.1.2/AUTHORS.rst` & `acore_server_config-0.1.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/LICENSE.txt` & `acore_server_config-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/PKG-INFO` & `acore_server_config-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_config
-Version: 0.1.2
+Version: 0.1.3
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.1.2/README.rst` & `acore_server_config-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/boto_ses.py` & `acore_server_config-0.1.3/acore_server_config/boto_ses.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/config/define/main.py` & `acore_server_config-0.1.3/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/config/define/server.py` & `acore_server_config-0.1.3/acore_server_config/config/define/server.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/config/init.py` & `acore_server_config-0.1.3/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/in_ec2.py` & `acore_server_config-0.1.3/acore_server_config/in_ec2.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,9 +53,9 @@
         env_class=Env,
         env_enum_class=EnvEnum,
         bsm=bsm,
         parameter_name=parameter_name,
         parameter_with_encryption=True,
     )
     env = config.get_env(env_name=env_name)
-    server = env.servers[server_id]
+    server = env.servers[server_name]
     return server
```

### Comparing `acore_server_config-0.1.2/acore_server_config/paths.py` & `acore_server_config-0.1.3/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/runtime.py` & `acore_server_config-0.1.3/acore_server_config/runtime.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.1.3/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.1.3/acore_server_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-config
-Version: 0.1.2
+Version: 0.1.3
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.1.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.1.2/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.1.3/acore_server_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/release-history.rst` & `acore_server_config-0.1.3/release-history.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.3 (2023-06-17)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that the key in ``env.servers[${key}]`` should be ``${server_name}``, but not ``${server_id}``.
+
+
 0.1.2 (2023-06-17)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that the final AWS parameter name convention should be ``${parameter_name_prefix}${env_name}``, but not ``${parameter_name_prefix}-${env_name}``.
```

### Comparing `acore_server_config-0.1.2/requirements-doc.txt` & `acore_server_config-0.1.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.2/setup.py` & `acore_server_config-0.1.3/setup.py`

 * *Files identical despite different names*

