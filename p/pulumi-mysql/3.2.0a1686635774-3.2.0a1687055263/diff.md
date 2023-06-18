# Comparing `tmp/pulumi_mysql-3.2.0a1686635774.tar.gz` & `tmp/pulumi_mysql-3.2.0a1687055263.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mysql-3.2.0a1686635774.tar", last modified: Tue Jun 13 06:09:57 2023, max compression
+gzip compressed data, was "pulumi_mysql-3.2.0a1687055263.tar", last modified: Sun Jun 18 02:37:04 2023, max compression
```

## Comparing `pulumi_mysql-3.2.0a1686635774.tar` & `pulumi_mysql-3.2.0a1687055263.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:57.426770 pulumi_mysql-3.2.0a1686635774/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-13 06:09:57.426770 pulumi_mysql-3.2.0a1686635774/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:57.426770 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:57.426770 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql/user_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:57.426770 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:09:57.426770 pulumi_mysql-3.2.0a1686635774/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-13 06:09:57.000000 pulumi_mysql-3.2.0a1686635774/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:37:04.593062 pulumi_mysql-3.2.0a1687055263/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-18 02:37:04.593062 pulumi_mysql-3.2.0a1687055263/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:37:04.593062 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:37:04.593062 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22471 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql/user_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:37:04.593062 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:37:04.593062 pulumi_mysql-3.2.0a1687055263/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-18 02:37:04.000000 pulumi_mysql-3.2.0a1687055263/setup.py
```

### Comparing `pulumi_mysql-3.2.0a1686635774/PKG-INFO` & `pulumi_mysql-3.2.0a1687055263/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.2.0a1686635774
+Version: 3.2.0a1687055263
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi mysql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.2.0a1686635774/README.md` & `pulumi_mysql-3.2.0a1687055263/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/__init__.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/_utilities.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/config/vars.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/database.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/grant.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/provider.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/role.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/user.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql/user_password.py` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql/user_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/PKG-INFO` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-mysql
-Version: 3.2.0a1686635774
+Version: 3.2.0a1687055263
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi mysql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.2.0a1686635774/pulumi_mysql.egg-info/SOURCES.txt` & `pulumi_mysql-3.2.0a1687055263/pulumi_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.2.0a1686635774/setup.py` & `pulumi_mysql-3.2.0a1687055263/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.2.0a1686635774"
-PLUGIN_VERSION = "3.2.0-alpha.1686635774+943aae90"
+VERSION = "3.2.0a1687055263"
+PLUGIN_VERSION = "3.2.0-alpha.1687055263+bc237fea"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'mysql', PLUGIN_VERSION])
         except OSError as error:
```

