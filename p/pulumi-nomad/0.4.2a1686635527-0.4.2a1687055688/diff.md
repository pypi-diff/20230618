# Comparing `tmp/pulumi_nomad-0.4.2a1686635527.tar.gz` & `tmp/pulumi_nomad-0.4.2a1687055688.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_nomad-0.4.2a1686635527.tar", last modified: Tue Jun 13 05:58:15 2023, max compression
+gzip compressed data, was "pulumi_nomad-0.4.2a1687055688.tar", last modified: Sun Jun 18 02:47:23 2023, max compression
```

## Comparing `pulumi_nomad-0.4.2a1686635527.tar` & `pulumi_nomad-0.4.2a1687055688.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:58:15.615804 pulumi_nomad-0.4.2a1686635527/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-13 05:58:15.615804 pulumi_nomad-0.4.2a1686635527/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:58:15.615804 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_binding_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    28545 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:58:15.615804 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    52267 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/external_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_job_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_scaling_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_scaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_scheduler_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    56309 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/quote_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/scheduler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/sentinel_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    56839 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:58:15.615804 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:58:15.615804 pulumi_nomad-0.4.2a1686635527/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-13 05:58:15.000000 pulumi_nomad-0.4.2a1686635527/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:47:23.028624 pulumi_nomad-0.4.2a1687055688/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-18 02:47:23.028624 pulumi_nomad-0.4.2a1687055688/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:47:23.024624 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28545 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:47:23.024624 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52267 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/external_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_job_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_scaling_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_scaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_scheduler_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40679 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56309 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/quote_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/scheduler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/sentinel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56839 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:47:23.024624 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-18 02:47:23.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-18 02:47:23.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:47:23.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:47:23.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:47:23.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-18 02:47:23.000000 pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:47:23.028624 pulumi_nomad-0.4.2a1687055688/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-18 02:47:22.000000 pulumi_nomad-0.4.2a1687055688/setup.py
```

### Comparing `pulumi_nomad-0.4.2a1686635527/PKG-INFO` & `pulumi_nomad-0.4.2a1687055688/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_nomad
-Version: 0.4.2a1686635527
+Version: 0.4.2a1687055688
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi nomad
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_nomad-0.4.2a1686635527/README.md` & `pulumi_nomad-0.4.2a1687055688/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/__init__.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/_inputs.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/_utilities.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_auth_method.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_auth_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_binding_rule.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_binding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_policy.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_role.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/acl_token.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/config/outputs.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/config/vars.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/external_volume.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/external_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_policies.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_policy.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_role.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_roles.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_token.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_acl_tokens.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_acl_tokens.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_datacenters.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_deployments.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_deployments.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_job.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_job_parser.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_job_parser.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_namespace.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_namespaces.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_plugin.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_plugins.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_plugins.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_regions.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_scaling_policies.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_scaling_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_scaling_policy.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_scheduler_policy.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_scheduler_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/get_volumes.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/job.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/namespace.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/outputs.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/provider.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/quote_specification.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/quote_specification.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/scheduler_config.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/scheduler_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/sentinel_policy.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/sentinel_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad/volume.py` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/PKG-INFO` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-nomad
-Version: 0.4.2a1686635527
+Version: 0.4.2a1687055688
 Summary: A Pulumi package for creating and managing nomad cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-nomad
 Keywords: pulumi nomad
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_nomad-0.4.2a1686635527/pulumi_nomad.egg-info/SOURCES.txt` & `pulumi_nomad-0.4.2a1687055688/pulumi_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_nomad-0.4.2a1686635527/setup.py` & `pulumi_nomad-0.4.2a1687055688/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.2a1686635527"
-PLUGIN_VERSION = "0.4.2-alpha.1686635527+9c1fe522"
+VERSION = "0.4.2a1687055688"
+PLUGIN_VERSION = "0.4.2-alpha.1687055688+5bb9ebe4"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'nomad', PLUGIN_VERSION])
         except OSError as error:
```

