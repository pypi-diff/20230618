# Comparing `tmp/himl-0.8.1.tar.gz` & `tmp/himl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "himl-0.8.1.tar", last modified: Wed Dec 22 11:13:17 2021, max compression
+gzip compressed data, was "himl-0.9.0.tar", last modified: Thu Feb 17 09:15:34 2022, max compression
```

## Comparing `himl-0.8.1.tar` & `himl-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.617968 himl-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-22 11:13:04.000000 himl-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-12-22 11:13:04.000000 himl-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11493 2021-12-22 11:13:17.617968 himl-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10132 2021-12-22 11:13:04.000000 himl-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.609969 himl-0.8.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=dev/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=dev/env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=dev/region=us-east-1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=dev/region=us-east-1/cluster=cluster1/
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=dev/region=us-east-1/cluster=cluster1/cluster.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=dev/region=us-east-1/cluster=cluster2/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=dev/region=us-east-1/cluster=cluster2/cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=dev/region=us-east-1/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=dev/region=us-west-2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=dev/region=us-west-2/cluster=cluster1/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=dev/region=us-west-2/cluster=cluster1/cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=dev/region=us-west-2/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=prod/
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=prod/env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=prod/region=eu-west-2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/complex/env=prod/region=eu-west-2/cluster=ireland1/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=prod/region=eu-west-2/cluster=ireland1/cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-22 11:13:04.000000 himl-0.8.1/examples/complex/env=prod/region=eu-west-2/region.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/secrets/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-22 11:13:04.000000 himl-0.8.1/examples/secrets/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-22 11:13:04.000000 himl-0.8.1/examples/simple/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.613968 himl-0.8.1/examples/simple/production/
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-22 11:13:04.000000 himl-0.8.1/examples/simple/production/env.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.617968 himl-0.8.1/himl/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2021-12-22 11:13:04.000000 himl-0.8.1/himl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12552 2021-12-22 11:13:04.000000 himl-0.8.1/himl/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2021-12-22 11:13:04.000000 himl-0.8.1/himl/config_merger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2021-12-22 11:13:04.000000 himl-0.8.1/himl/inject_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     2581 2021-12-22 11:13:04.000000 himl-0.8.1/himl/inject_secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     9378 2021-12-22 11:13:04.000000 himl-0.8.1/himl/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3792 2021-12-22 11:13:04.000000 himl-0.8.1/himl/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-12-22 11:13:04.000000 himl-0.8.1/himl/python_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-12-22 11:13:04.000000 himl-0.8.1/himl/remote_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2021-12-22 11:13:04.000000 himl-0.8.1/himl/secret_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2021-12-22 11:13:04.000000 himl-0.8.1/himl/simples3.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-12-22 11:13:04.000000 himl-0.8.1/himl/simplessm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2021-12-22 11:13:04.000000 himl-0.8.1/himl/simplevault.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-22 11:13:17.617968 himl-0.8.1/himl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11493 2021-12-22 11:13:17.000000 himl-0.8.1/himl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2021-12-22 11:13:17.000000 himl-0.8.1/himl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-22 11:13:17.000000 himl-0.8.1/himl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-12-22 11:13:17.000000 himl-0.8.1/himl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-12-22 11:13:17.000000 himl-0.8.1/himl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-12-22 11:13:17.000000 himl-0.8.1/himl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-12-22 11:13:04.000000 himl-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-22 11:13:17.617968 himl-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-12-22 11:13:04.000000 himl-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.701142 himl-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-02-17 09:14:45.000000 himl-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-02-17 09:14:45.000000 himl-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    11493 2022-02-17 09:15:34.701142 himl-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10132 2022-02-17 09:14:45.000000 himl-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.693142 himl-0.9.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=dev/
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=dev/env.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=dev/region=us-east-1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=dev/region=us-east-1/cluster=cluster1/
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=dev/region=us-east-1/cluster=cluster1/cluster.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=dev/region=us-east-1/cluster=cluster2/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=dev/region=us-east-1/cluster=cluster2/cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=dev/region=us-east-1/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=dev/region=us-west-2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=dev/region=us-west-2/cluster=cluster1/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=dev/region=us-west-2/cluster=cluster1/cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=dev/region=us-west-2/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=prod/
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=prod/env.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=prod/region=eu-west-2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/complex/env=prod/region=eu-west-2/cluster=ireland1/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=prod/region=eu-west-2/cluster=ireland1/cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-17 09:14:45.000000 himl-0.9.0/examples/complex/env=prod/region=eu-west-2/region.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/secrets/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-17 09:14:45.000000 himl-0.9.0/examples/secrets/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-02-17 09:14:45.000000 himl-0.9.0/examples/simple/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.697142 himl-0.9.0/examples/simple/production/
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-02-17 09:14:45.000000 himl-0.9.0/examples/simple/production/env.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.701142 himl-0.9.0/himl/
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-02-17 09:14:45.000000 himl-0.9.0/himl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12552 2022-02-17 09:14:45.000000 himl-0.9.0/himl/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6552 2022-02-17 09:14:45.000000 himl-0.9.0/himl/config_merger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-02-17 09:14:45.000000 himl-0.9.0/himl/inject_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2581 2022-02-17 09:14:45.000000 himl-0.9.0/himl/inject_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-02-17 09:14:45.000000 himl-0.9.0/himl/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3792 2022-02-17 09:14:45.000000 himl-0.9.0/himl/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-02-17 09:14:45.000000 himl-0.9.0/himl/python_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-02-17 09:14:45.000000 himl-0.9.0/himl/remote_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-02-17 09:14:45.000000 himl-0.9.0/himl/secret_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-02-17 09:14:45.000000 himl-0.9.0/himl/simples3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-02-17 09:14:45.000000 himl-0.9.0/himl/simplessm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-02-17 09:14:45.000000 himl-0.9.0/himl/simplevault.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:15:34.701142 himl-0.9.0/himl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    11493 2022-02-17 09:15:34.000000 himl-0.9.0/himl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-02-17 09:15:34.000000 himl-0.9.0/himl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 09:15:34.000000 himl-0.9.0/himl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-02-17 09:15:34.000000 himl-0.9.0/himl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-02-17 09:15:34.000000 himl-0.9.0/himl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-17 09:15:34.000000 himl-0.9.0/himl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      132 2022-02-17 09:14:45.000000 himl-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-17 09:15:34.701142 himl-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-02-17 09:14:45.000000 himl-0.9.0/setup.py
```

### Comparing `himl-0.8.1/LICENSE` & `himl-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/PKG-INFO` & `himl-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: himl
-Version: 0.8.1
+Version: 0.9.0
 Summary: A hierarchical config using yaml
 Home-page: https://github.com/adobe/himl
 Author: Adobe
 Author-email: noreply@adobe.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,15 +29,15 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # himl
 A hierarchical config using yaml in Python.
 
-Latest version is: 0.8.1
+Latest version is: 0.9.0
 
 ## Description
 
 A python module which allows you to merge hierarchical config files using YAML syntax. It offers deep merge, variable interpolation and secrets retrieval from secrets managers.
 
 It is ideal if you want to structure your hierarchy in such a way that you avoid duplication. You can define a structure for your configuration using a hierarchy such environment/project/cluster/app. It is up to you what layers you want to use in this hierarchy. The tool will read all yaml files starting from the root (where default values would be) all the way to the leaf (where most specific values would be, which will take precedence).
```

### Comparing `himl-0.8.1/README.md` & `himl-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # himl
 A hierarchical config using yaml in Python.
 
-Latest version is: 0.8.1
+Latest version is: 0.9.0
 
 ## Description
 
 A python module which allows you to merge hierarchical config files using YAML syntax. It offers deep merge, variable interpolation and secrets retrieval from secrets managers.
 
 It is ideal if you want to structure your hierarchy in such a way that you avoid duplication. You can define a structure for your configuration using a hierarchy such environment/project/cluster/app. It is up to you what layers you want to use in this hierarchy. The tool will read all yaml files starting from the root (where default values would be) all the way to the leaf (where most specific values would be, which will take precedence).
```

### Comparing `himl-0.8.1/examples/complex/default.yaml` & `himl-0.9.0/examples/complex/default.yaml`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/examples/complex/env=dev/region=us-east-1/cluster=cluster1/cluster.yaml` & `himl-0.9.0/examples/complex/env=dev/region=us-east-1/cluster=cluster1/cluster.yaml`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/__init__.py` & `himl-0.9.0/himl/__init__.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/config_generator.py` & `himl-0.9.0/himl/config_generator.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/config_merger.py` & `himl-0.9.0/himl/config_merger.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/inject_env.py` & `himl-0.9.0/himl/inject_env.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/inject_secrets.py` & `himl-0.9.0/himl/inject_secrets.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/interpolation.py` & `himl-0.9.0/himl/interpolation.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/main.py` & `himl-0.9.0/himl/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,14 @@
                             help='enclose the generated data under a common key')
         parser.add_argument('--remove-enclosing-key', dest='remove_enclosing_key', type=str,
                             help='remove enclosed data from under a common key')
         parser.add_argument('--cwd', dest='cwd', type=str, default="",
                             help='the working directory')
         parser.add_argument('--multi-line-string', action='store_true',
                             help='will overwrite the global yaml dumper to use block style')
-        parser.add_argument('--version', action='version', version='%(prog)s v{version}'.format(version="0.8.1"),
+        parser.add_argument('--version', action='version', version='%(prog)s v{version}'.format(version="0.9.0"),
                             help='print himl version')
         return parser
 
 
 def run(args=None):
     ConfigRunner().run(args)
```

### Comparing `himl-0.8.1/himl/python_compat.py` & `himl-0.9.0/himl/python_compat.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/remote_state.py` & `himl-0.9.0/himl/remote_state.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/secret_resolvers.py` & `himl-0.9.0/himl/secret_resolvers.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/simples3.py` & `himl-0.9.0/himl/simples3.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/simplessm.py` & `himl-0.9.0/himl/simplessm.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl/simplevault.py` & `himl-0.9.0/himl/simplevault.py`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/himl.egg-info/PKG-INFO` & `himl-0.9.0/himl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: himl
-Version: 0.8.1
+Version: 0.9.0
 Summary: A hierarchical config using yaml
 Home-page: https://github.com/adobe/himl
 Author: Adobe
 Author-email: noreply@adobe.com
 License: Apache2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,15 +29,15 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # himl
 A hierarchical config using yaml in Python.
 
-Latest version is: 0.8.1
+Latest version is: 0.9.0
 
 ## Description
 
 A python module which allows you to merge hierarchical config files using YAML syntax. It offers deep merge, variable interpolation and secrets retrieval from secrets managers.
 
 It is ideal if you want to structure your hierarchy in such a way that you avoid duplication. You can define a structure for your configuration using a hierarchy such environment/project/cluster/app. It is up to you what layers you want to use in this hierarchy. The tool will read all yaml files starting from the root (where default values would be) all the way to the leaf (where most specific values would be, which will take precedence).
```

### Comparing `himl-0.8.1/himl.egg-info/SOURCES.txt` & `himl-0.9.0/himl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `himl-0.8.1/setup.py` & `himl-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     _readme = f.read()
 
 _mydir = os.path.abspath(os.path.dirname(sys.argv[0]))
 _requires = [ r for r in open(os.path.sep.join((_mydir,'requirements.txt')), "r").read().split('\n') if len(r)>1 ]
 
 setup(
     name='himl',
-    version="0.8.1",
+    version="0.9.0",
     description='A hierarchical config using yaml',
     long_description=_readme + '\n\n',
     long_description_content_type='text/markdown',
     url='https://github.com/adobe/himl',
     author='Adobe',
     author_email='noreply@adobe.com',
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
```

