# Comparing `tmp/acore_server_config-0.1.3.tar.gz` & `tmp/acore_server_config-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.1.3.tar", last modified: Sun Jun 18 02:07:54 2023, max compression
+gzip compressed data, was "acore_server_config-0.2.1.tar", last modified: Sun Jun 18 03:46:36 2023, max compression
```

## Comparing `acore_server_config-0.1.3.tar` & `acore_server_config-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.110687 acore_server_config-0.1.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 02:07:54.110531 acore_server_config-0.1.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.1.3/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.107208 acore_server_config-0.1.3/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.1.3/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 02:06:28.000000 acore_server_config-0.1.3/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.1.3/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      592 2023-06-18 00:51:40.000000 acore_server_config-0.1.3/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.1.3/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.108316 acore_server_config-0.1.3/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.1.3/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.109063 acore_server_config-0.1.3/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.1.3/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.1.3/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1098 2023-06-18 01:09:41.000000 acore_server_config-0.1.3/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.1.3/acore_server_config/config/init.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.109302 acore_server_config-0.1.3/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1867 2023-06-18 02:06:22.000000 acore_server_config-0.1.3/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.1.3/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.1.3/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.109747 acore_server_config-0.1.3/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/tests/helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.110077 acore_server_config-0.1.3/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.107915 acore_server_config-0.1.3/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 02:07:54.000000 acore_server_config-0.1.3/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1539 2023-06-18 02:07:23.000000 acore_server_config-0.1.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.1.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.1.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 02:07:54.110732 acore_server_config-0.1.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.1.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 02:07:54.110218 acore_server_config-0.1.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.1.3/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.929454 acore_server_config-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 03:46:36.929306 acore_server_config-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.925839 acore_server_config-0.2.1/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.2.1/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-18 03:41:22.000000 acore_server_config-0.2.1/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      389 2023-06-18 01:32:36.000000 acore_server_config-0.2.1/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-06-18 03:18:29.000000 acore_server_config-0.2.1/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.2.1/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.926977 acore_server_config-0.2.1/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-16 18:25:58.000000 acore_server_config-0.2.1/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.927801 acore_server_config-0.2.1/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       72 2023-06-16 19:20:29.000000 acore_server_config-0.2.1/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.2.1/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1344 2023-06-18 03:28:21.000000 acore_server_config-0.2.1/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.2.1/acore_server_config/config/init.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.928000 acore_server_config-0.2.1/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3433 2023-06-18 03:37:20.000000 acore_server_config-0.2.1/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.2.1/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.2.1/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.928479 acore_server_config-0.2.1/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/acore_server_config/tests/helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.928848 acore_server_config-0.2.1/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.926581 acore_server_config-0.2.1/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-18 03:46:36.000000 acore_server_config-0.2.1/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1063 2023-06-18 03:46:36.000000 acore_server_config-0.2.1/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-18 03:46:36.000000 acore_server_config-0.2.1/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      280 2023-06-18 03:46:36.000000 acore_server_config-0.2.1/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-18 03:46:36.000000 acore_server_config-0.2.1/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1821 2023-06-18 03:45:48.000000 acore_server_config-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-18 03:46:36.929504 acore_server_config-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-18 03:46:36.929012 acore_server_config-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      448 2023-06-18 00:55:02.000000 acore_server_config-0.2.1/tests/test_api.py
```

### Comparing `acore_server_config-0.1.3/AUTHORS.rst` & `acore_server_config-0.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/LICENSE.txt` & `acore_server_config-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/PKG-INFO` & `acore_server_config-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_config
-Version: 0.1.3
+Version: 0.2.1
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.1.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.1.3/README.rst` & `acore_server_config-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/acore_server_config/boto_ses.py` & `acore_server_config-0.2.1/acore_server_config/boto_ses.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+from s3pathlib import context
 from boto_session_manager import BotoSesManager
 
 from .runtime import IS_LOCAL, IS_GITHUB_CI, IS_EC2, IS_CODEBUILD_CI
 
 aws_region = "us-east-1"
 # environment aware boto session manager
 if IS_LOCAL:  # put production first
@@ -17,7 +18,9 @@
     )
 elif IS_EC2 or IS_CODEBUILD_CI:
     bsm = BotoSesManager(
         region_name=aws_region,
     )
 else:  # pragma: no cover
     raise NotImplementedError
+
+context.attach_boto_session(boto_ses=bsm.boto_ses)
```

### Comparing `acore_server_config-0.1.3/acore_server_config/config/define/main.py` & `acore_server_config-0.2.1/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/acore_server_config/config/define/server.py` & `acore_server_config-0.2.1/acore_server_config/config/define/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,22 @@
 
     :param id: Server id, the naming convention is ``${env_name}-${server_name}``
     :param db_admin_password: the RDS admin password, we need this password
         to create the database user.
     :param db_username: the database user for game server
     :param db_password: the database password for game server
     """
+
     id: T.Optional[str] = dataclasses.field(default=None)
     db_admin_password: T.Optional[str] = dataclasses.field(default=None)
     db_username: T.Optional[str] = dataclasses.field(default=None)
     db_password: T.Optional[str] = dataclasses.field(default=None)
+    authserver_conf: T.Dict[str, str] = dataclasses.field(default_factory=dict)
+    worldserver_conf: T.Dict[str, str] = dataclasses.field(default_factory=dict)
+    mod_lua_engine_conf: T.Dict[str, str] = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
 class ServerMixin:
     servers: T.Dict[str, Server] = dataclasses.field(default_factory=dict)
 
     @property
```

### Comparing `acore_server_config-0.1.3/acore_server_config/config/init.py` & `acore_server_config-0.2.1/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/acore_server_config/paths.py` & `acore_server_config-0.2.1/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/acore_server_config/runtime.py` & `acore_server_config-0.2.1/acore_server_config/runtime.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.2.1/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.2.1/acore_server_config.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-config
-Version: 0.1.3
+Version: 0.2.1
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.1.3#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.1.3/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.2.1/acore_server_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/release-history.rst` & `acore_server_config-0.2.1/release-history.rst`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.1 (2023-06-17)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Add support to use AWS S3 as the backend
+- Now AWS S3 is the default backend
+- Add support to manage game server configuration (the ``*.conf`` file)
+
+
 0.1.3 (2023-06-17)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that the key in ``env.servers[${key}]`` should be ``${server_name}``, but not ``${server_id}``.
```

### Comparing `acore_server_config-0.1.3/requirements-doc.txt` & `acore_server_config-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.1.3/setup.py` & `acore_server_config-0.2.1/setup.py`

 * *Files identical despite different names*

