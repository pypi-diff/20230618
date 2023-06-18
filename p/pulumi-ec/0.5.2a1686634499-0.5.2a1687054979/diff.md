# Comparing `tmp/pulumi_ec-0.5.2a1686634499.tar.gz` & `tmp/pulumi_ec-0.5.2a1687054979.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ec-0.5.2a1686634499.tar", last modified: Tue Jun 13 05:45:13 2023, max compression
+gzip compressed data, was "pulumi_ec-0.5.2a1687054979.tar", last modified: Sun Jun 18 02:33:31 2023, max compression
```

## Comparing `pulumi_ec-0.5.2a1686634499.tar` & `pulumi_ec-0.5.2a1687054979.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:45:13.180628 pulumi_ec-0.5.2a1686634499/
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-13 05:45:13.180628 pulumi_ec-0.5.2a1686634499/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:45:13.180628 pulumi_ec-0.5.2a1686634499/pulumi_ec/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   114649 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:45:13.180628 pulumi_ec-0.5.2a1686634499/pulumi_ec/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    73457 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_elasticsearch_keystore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25588 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_traffic_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_traffic_filter_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/get_aws_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/get_azure_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/get_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/get_gcp_private_service_connect_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/get_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)   140327 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:45:13.180628 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-13 05:45:13.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 05:45:13.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:45:13.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:45:13.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 05:45:13.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 05:45:13.000000 pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:45:13.180628 pulumi_ec-0.5.2a1686634499/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-13 05:45:12.000000 pulumi_ec-0.5.2a1686634499/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:33:31.273513 pulumi_ec-0.5.2a1687054979/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-18 02:33:31.273513 pulumi_ec-0.5.2a1687054979/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:33:31.269513 pulumi_ec-0.5.2a1687054979/pulumi_ec/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114649 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:33:31.273513 pulumi_ec-0.5.2a1687054979/pulumi_ec/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73457 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_elasticsearch_keystore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25588 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22947 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_traffic_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_traffic_filter_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/get_aws_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/get_azure_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/get_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/get_gcp_private_service_connect_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/get_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)   140327 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:33:31.273513 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:33:31.273513 pulumi_ec-0.5.2a1687054979/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-18 02:33:31.000000 pulumi_ec-0.5.2a1687054979/setup.py
```

### Comparing `pulumi_ec-0.5.2a1686634499/PKG-INFO` & `pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_ec
-Version: 0.5.2a1686634499
+Name: pulumi-ec
+Version: 0.5.2a1687054979
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi ec elasticsearch es elastic elasticcloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.5.2a1686634499/README.md` & `pulumi_ec-0.5.2a1687054979/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/__init__.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/_inputs.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/_utilities.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/config/vars.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_elasticsearch_keystore.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_elasticsearch_keystore.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_extension.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_extension.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_traffic_filter.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_traffic_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/deployment_traffic_filter_association.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/deployment_traffic_filter_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/get_aws_privatelink_endpoint.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/get_aws_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/get_azure_privatelink_endpoint.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/get_azure_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/get_deployment.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/get_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/get_deployments.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/get_gcp_private_service_connect_endpoint.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/get_gcp_private_service_connect_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/get_stack.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/get_stack.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/outputs.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec/provider.py` & `pulumi_ec-0.5.2a1687054979/pulumi_ec/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/PKG-INFO` & `pulumi_ec-0.5.2a1687054979/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-ec
-Version: 0.5.2a1686634499
+Name: pulumi_ec
+Version: 0.5.2a1687054979
 Summary: A Pulumi package for creating and managing ElasticCloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-ec
 Keywords: pulumi ec elasticsearch es elastic elasticcloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ec-0.5.2a1686634499/pulumi_ec.egg-info/SOURCES.txt` & `pulumi_ec-0.5.2a1687054979/pulumi_ec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ec-0.5.2a1686634499/setup.py` & `pulumi_ec-0.5.2a1687054979/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.5.2a1686634499"
-PLUGIN_VERSION = "0.5.2-alpha.1686634499+d6306439"
+VERSION = "0.5.2a1687054979"
+PLUGIN_VERSION = "0.5.2-alpha.1687054979+5c3474a1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'ec', PLUGIN_VERSION])
         except OSError as error:
```

