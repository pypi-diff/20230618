# Comparing `tmp/pulumi_postgresql-3.9.0a1686636221.tar.gz` & `tmp/pulumi_postgresql-3.9.0a1687056260.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_postgresql-3.9.0a1686636221.tar", last modified: Tue Jun 13 06:09:54 2023, max compression
+gzip compressed data, was "pulumi_postgresql-3.9.0a1687056260.tar", last modified: Sun Jun 18 02:54:43 2023, max compression
```

## Comparing `pulumi_postgresql-3.9.0a1686636221.tar` & `pulumi_postgresql-3.9.0a1687056260.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:54.031731 pulumi_postgresql-3.9.0a1686636221/
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-13 06:09:54.031731 pulumi_postgresql-3.9.0a1686636221/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:54.031731 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:54.031731 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    30248 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/default_privileg.py
--rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/get_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/get_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/get_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/grant_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/physical_replication_slot.py
--rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/publication.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/replication_slot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67908 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/user_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:54.031731 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-13 06:09:54.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 06:09:54.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:09:54.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:09:54.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:09:54.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 06:09:54.000000 pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:09:54.031731 pulumi_postgresql-3.9.0a1686636221/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-13 06:09:53.000000 pulumi_postgresql-3.9.0a1686636221/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:43.623226 pulumi_postgresql-3.9.0a1687056260/
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-18 02:54:43.623226 pulumi_postgresql-3.9.0a1687056260/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:43.619226 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:43.623226 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30248 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/default_privileg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21774 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/get_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/get_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/get_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28892 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/grant_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/physical_replication_slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25603 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/replication_slot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67908 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18173 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24829 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18416 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/user_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:54:43.623226 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:54:43.623226 pulumi_postgresql-3.9.0a1687056260/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-18 02:54:43.000000 pulumi_postgresql-3.9.0a1687056260/setup.py
```

### Comparing `pulumi_postgresql-3.9.0a1686636221/PKG-INFO` & `pulumi_postgresql-3.9.0a1687056260/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_postgresql
-Version: 3.9.0a1686636221
+Version: 3.9.0a1687056260
 Summary: A Pulumi package for creating and managing postgresql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-postgresql
 Keywords: pulumi postgresql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_postgresql-3.9.0a1686636221/README.md` & `pulumi_postgresql-3.9.0a1687056260/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/__init__.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/_inputs.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/_utilities.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/config/outputs.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/config/vars.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/database.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/default_privileg.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/default_privileg.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/default_privileges.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/default_privileges.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/extension.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/function.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/function.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/get_schemas.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/get_schemas.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/get_sequences.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/get_sequences.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/get_tables.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/get_tables.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/grant.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/grant_role.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/grant_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/outputs.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/physical_replication_slot.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/physical_replication_slot.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/provider.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/publication.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/publication.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/replication_slot.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/replication_slot.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/role.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/schema.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/server.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/subscription.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql/user_mapping.py` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql/user_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/PKG-INFO` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-postgresql
-Version: 3.9.0a1686636221
+Version: 3.9.0a1687056260
 Summary: A Pulumi package for creating and managing postgresql cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-postgresql
 Keywords: pulumi postgresql
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_postgresql-3.9.0a1686636221/pulumi_postgresql.egg-info/SOURCES.txt` & `pulumi_postgresql-3.9.0a1687056260/pulumi_postgresql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_postgresql-3.9.0a1686636221/setup.py` & `pulumi_postgresql-3.9.0a1687056260/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1686636221"
-PLUGIN_VERSION = "3.9.0-alpha.1686636221+2ed0efcd"
+VERSION = "3.9.0a1687056260"
+PLUGIN_VERSION = "3.9.0-alpha.1687056260+be1e3e36"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'postgresql', PLUGIN_VERSION])
         except OSError as error:
```

