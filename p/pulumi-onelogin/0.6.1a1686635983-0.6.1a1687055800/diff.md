# Comparing `tmp/pulumi_onelogin-0.6.1a1686635983.tar.gz` & `tmp/pulumi_onelogin-0.6.1a1687055800.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_onelogin-0.6.1a1686635983.tar", last modified: Tue Jun 13 06:09:09 2023, max compression
+gzip compressed data, was "pulumi_onelogin-0.6.1a1687055800.tar", last modified: Sun Jun 18 02:48:57 2023, max compression
```

## Comparing `pulumi_onelogin-0.6.1a1686635983.tar` & `pulumi_onelogin-0.6.1a1687055800.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.311324 pulumi_onelogin-0.6.1a1686635983/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-13 06:09:09.311324 pulumi_onelogin-0.6.1a1686635983/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.303323 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70497 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    46699 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.307323 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_actions_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_conditions_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_rules_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    24033 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16458 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/auth_servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.307323 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_privileges_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_risk_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_risk_rules_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    51470 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/risk_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.307323 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24146 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65498 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.311324 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23514 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_v1_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_v1_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65455 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:09:09.303323 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-13 06:09:09.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-13 06:09:09.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:09:09.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:09:09.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:09:09.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 06:09:09.000000 pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:09:09.311324 pulumi_onelogin-0.6.1a1686635983/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-13 06:09:08.000000 pulumi_onelogin-0.6.1a1686635983/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.155502 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70497 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46699 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_actions_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_conditions_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_rules_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24033 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16458 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/auth_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_privileges_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_risk_rules_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51470 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24146 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24051 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65498 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23118 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23514 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_v1_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_v1_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65455 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:48:57.155502 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-18 02:48:57.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-18 02:48:57.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:48:57.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:48:57.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 02:48:57.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 02:48:57.000000 pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 02:48:57.159502 pulumi_onelogin-0.6.1a1687055800/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-18 02:48:56.000000 pulumi_onelogin-0.6.1a1687055800/setup.py
```

### Comparing `pulumi_onelogin-0.6.1a1686635983/PKG-INFO` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_onelogin
-Version: 0.6.1a1686635983
+Name: pulumi-onelogin
+Version: 0.6.1a1687055800
 Summary: A Pulumi package for creating and managing OneLogin cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-onelogin
 Keywords: pulumi onelogin
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_onelogin-0.6.1a1686635983/README.md` & `pulumi_onelogin-0.6.1a1687055800/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/__init__.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/_inputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/_utilities.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/app.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/__init__.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/_inputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_actions.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_actions_values.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_actions_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_conditions.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_conditions.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_conditions_operators.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_conditions_operators.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_rules.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_rules_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_rules_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/get_users.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/outputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/apps/rules.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/apps/rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/auth_servers.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/auth_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/config/outputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/config/vars.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_apps.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers_claims.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_auth_servers_scopes.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_auth_servers_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_mappings.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_privileges.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_privileges.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_privileges_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_privileges_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_risk_rules.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_risk_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/get_risk_rules_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/get_risk_rules_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/outputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/privileges.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/privileges.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/provider.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/risk_rules.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/risk_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/role.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/_inputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_admins.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_admins.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_apps.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_roles.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/get_users.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/roles/outputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/roles/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/user.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/__init__.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/_inputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_apps.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_devices.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_users.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_v1.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_v1_apps.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_v1_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/get_v1_instance.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/get_v1_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/outputs.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin/users/v1.py` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin/users/v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/PKG-INFO` & `pulumi_onelogin-0.6.1a1687055800/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-onelogin
-Version: 0.6.1a1686635983
+Name: pulumi_onelogin
+Version: 0.6.1a1687055800
 Summary: A Pulumi package for creating and managing OneLogin cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-onelogin
 Keywords: pulumi onelogin
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_onelogin-0.6.1a1686635983/pulumi_onelogin.egg-info/SOURCES.txt` & `pulumi_onelogin-0.6.1a1687055800/pulumi_onelogin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.1a1686635983/setup.py` & `pulumi_onelogin-0.6.1a1687055800/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.6.1a1686635983"
-PLUGIN_VERSION = "0.6.1-alpha.1686635983+5378378a"
+VERSION = "0.6.1a1687055800"
+PLUGIN_VERSION = "0.6.1-alpha.1687055800+240fde74"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'onelogin', PLUGIN_VERSION])
         except OSError as error:
```

