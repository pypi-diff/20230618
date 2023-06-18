# Comparing `tmp/pulumi_azuread-5.9.0.tar.gz` & `tmp/pulumi_azuread-5.9.0a1637590268.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_azuread-5.9.0.tar", last modified: Mon Nov 22 14:36:09 2021, max compression
+gzip compressed data, was "dist/pulumi_azuread-5.9.0a1637590268.tar", last modified: Mon Nov 22 14:15:42 2021, max compression
```

## Comparing `pulumi_azuread-5.9.0.tar` & `pulumi_azuread-5.9.0a1637590268.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread/
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    93242 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    29323 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/app_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)    84489 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/application.py
--rw-r--r--   0 runner    (1001) docker     (121)    27579 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/application_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)    23888 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/application_password.py
--rw-r--r--   0 runner    (1001) docker     (121)    13166 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/application_pre_authorized.py
--rw-r--r--   0 runner    (1001) docker     (121)    23581 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/conditional_access_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    14048 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/directory_role.py
--rw-r--r--   0 runner    (1001) docker     (121)    12831 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/directory_role_member.py
--rw-r--r--   0 runner    (1001) docker     (121)    21716 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_application.py
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_application_published_app_ids.py
--rw-r--r--   0 runner    (1001) docker     (121)     8311 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_application_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     9675 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_domains.py
--rw-r--r--   0 runner    (1001) docker     (121)    17390 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     9626 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    23308 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_service_principal.py
--rw-r--r--   0 runner    (1001) docker     (121)    10559 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_service_principals.py
--rw-r--r--   0 runner    (1001) docker     (121)    28555 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     8158 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/get_users.py
--rw-r--r--   0 runner    (1001) docker     (121)    60667 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/group.py
--rw-r--r--   0 runner    (1001) docker     (121)    12883 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/group_member.py
--rw-r--r--   0 runner    (1001) docker     (121)    21859 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/invitation.py
--rw-r--r--   0 runner    (1001) docker     (121)    13566 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/named_location.py
--rw-r--r--   0 runner    (1001) docker     (121)   147501 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    21203 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    79896 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/service_principal.py
--rw-r--r--   0 runner    (1001) docker     (121)    28454 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/service_principal_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)    18180 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/service_principal_password.py
--rw-r--r--   0 runner    (1001) docker     (121)   108167 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/pulumi_azuread/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/pulumi_azuread.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-22 14:36:09.000000 pulumi_azuread-5.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-11-22 14:36:07.000000 pulumi_azuread-5.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/
+-rw-r--r--   0 runner    (1001) docker     (121)     4742 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3784 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/
+-rw-r--r--   0 runner    (1001) docker     (121)     4523 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    93242 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29323 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/app_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    84489 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27579 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23888 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application_password.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13166 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application_pre_authorized.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23581 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/conditional_access_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3585 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14048 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/directory_role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12831 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/directory_role_member.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21716 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4065 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_application_published_app_ids.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8311 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_application_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3525 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9675 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_domains.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17390 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9626 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23308 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10559 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_service_principals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28555 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8158 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60667 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12883 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/group_member.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21859 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13566 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/named_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)   147501 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21203 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    79896 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28454 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/service_principal_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18180 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/service_principal_password.py
+-rw-r--r--   0 runner    (1001) docker     (121)   108167 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4742 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-22 14:15:42.000000 pulumi_azuread-5.9.0a1637590268/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2097 2021-11-22 14:15:40.000000 pulumi_azuread-5.9.0a1637590268/setup.py
```

### Comparing `pulumi_azuread-5.9.0/PKG-INFO` & `pulumi_azuread-5.9.0a1637590268/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuread
-Version: 5.9.0
+Version: 5.9.0a1637590268
 Summary: A Pulumi package for creating and managing azuread cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuread
 Description: [![Actions Status](https://github.com/pulumi/pulumi-azuread/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-azuread/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fazuread.svg)](https://npmjs.com/package/@pulumi/azuread)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: pulumi_azuread Version: 5.9.0 Summary: A Pulumi
-package for creating and managing azuread cloud resources. Home-page: https://
-pulumi.io License: Apache-2.0 Project-URL: Repository, https://github.com/
-pulumi/pulumi-azuread Description: [![Actions Status](https://github.com/
-pulumi/pulumi-azuread/workflows/master/badge.svg)](https://github.com/pulumi/
-pulumi-azuread/actions) [![Slack](http://www.pulumi.com/images/docs/badges/
-slack.svg)](https://slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
-%40pulumi%2Fazuread.svg)](https://npmjs.com/package/@pulumi/azuread) [![NuGet
-version](https://badge.fury.io/nu/pulumi.azuread.svg)](https://badge.fury.io/
-nu/pulumi.azured) [![Python version](https://badge.fury.io/py/pulumi-
-azuread.svg)](https://pypi.org/project/pulumi-azuread) [![PkgGoDev](https://
-pkg.go.dev/badge/github.com/pulumi/pulumi-azuread/sdk/v5/go)](https://
+Metadata-Version: 2.1 Name: pulumi_azuread Version: 5.9.0a1637590268 Summary: A
+Pulumi package for creating and managing azuread cloud resources. Home-page:
+https://pulumi.io License: Apache-2.0 Project-URL: Repository, https://
+github.com/pulumi/pulumi-azuread Description: [![Actions Status](https://
+github.com/pulumi/pulumi-azuread/workflows/master/badge.svg)](https://
+github.com/pulumi/pulumi-azuread/actions) [![Slack](http://www.pulumi.com/
+images/docs/badges/slack.svg)](https://slack.pulumi.com) [![NPM version](https:
+//badge.fury.io/js/%40pulumi%2Fazuread.svg)](https://npmjs.com/package/@pulumi/
+azuread) [![NuGet version](https://badge.fury.io/nu/pulumi.azuread.svg)](https:
+//badge.fury.io/nu/pulumi.azured) [![Python version](https://badge.fury.io/py/
+pulumi-azuread.svg)](https://pypi.org/project/pulumi-azuread) [![PkgGoDev]
+(https://pkg.go.dev/badge/github.com/pulumi/pulumi-azuread/sdk/v5/go)](https://
 pkg.go.dev/github.com/pulumi/pulumi-azuread/sdk/v5/go) [![License](https://
 img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-
 azuread/blob/master/LICENSE) # Microsoft Azure Active Directory Resource
 Provider The Microsoft Azure AD resource provider for Pulumi lets you use Azure
 Active Directory resources in your cloud programs. To use this package, please
 [install the Pulumi CLI first](https://pulumi.io/). For a streamlined Pulumi
 walkthrough, including language runtime installation and Azure configuration,
```

### Comparing `pulumi_azuread-5.9.0/README.md` & `pulumi_azuread-5.9.0a1637590268/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/__init__.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/_inputs.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/_utilities.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/app_role_assignment.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/app_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/application.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/application_certificate.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/application_password.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/application_pre_authorized.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/application_pre_authorized.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/conditional_access_policy.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/conditional_access_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/config/vars.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/directory_role.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/directory_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/directory_role_member.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/directory_role_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_application.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_application.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_application_published_app_ids.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_application_published_app_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_application_template.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_application_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_client_config.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_domains.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_domains.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_group.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_groups.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_service_principal.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_service_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_service_principals.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_service_principals.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_user.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/get_users.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/group.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/group_member.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/group_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/invitation.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/invitation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/named_location.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/named_location.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/outputs.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/provider.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/service_principal.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/service_principal.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/service_principal_certificate.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/service_principal_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/service_principal_password.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/service_principal_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread/user.py` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread.egg-info/PKG-INFO` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-azuread
-Version: 5.9.0
+Version: 5.9.0a1637590268
 Summary: A Pulumi package for creating and managing azuread cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuread
 Description: [![Actions Status](https://github.com/pulumi/pulumi-azuread/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-azuread/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fazuread.svg)](https://npmjs.com/package/@pulumi/azuread)
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: pulumi-azuread Version: 5.9.0 Summary: A Pulumi
-package for creating and managing azuread cloud resources. Home-page: https://
-pulumi.io License: Apache-2.0 Project-URL: Repository, https://github.com/
-pulumi/pulumi-azuread Description: [![Actions Status](https://github.com/
-pulumi/pulumi-azuread/workflows/master/badge.svg)](https://github.com/pulumi/
-pulumi-azuread/actions) [![Slack](http://www.pulumi.com/images/docs/badges/
-slack.svg)](https://slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
-%40pulumi%2Fazuread.svg)](https://npmjs.com/package/@pulumi/azuread) [![NuGet
-version](https://badge.fury.io/nu/pulumi.azuread.svg)](https://badge.fury.io/
-nu/pulumi.azured) [![Python version](https://badge.fury.io/py/pulumi-
-azuread.svg)](https://pypi.org/project/pulumi-azuread) [![PkgGoDev](https://
-pkg.go.dev/badge/github.com/pulumi/pulumi-azuread/sdk/v5/go)](https://
+Metadata-Version: 2.1 Name: pulumi-azuread Version: 5.9.0a1637590268 Summary: A
+Pulumi package for creating and managing azuread cloud resources. Home-page:
+https://pulumi.io License: Apache-2.0 Project-URL: Repository, https://
+github.com/pulumi/pulumi-azuread Description: [![Actions Status](https://
+github.com/pulumi/pulumi-azuread/workflows/master/badge.svg)](https://
+github.com/pulumi/pulumi-azuread/actions) [![Slack](http://www.pulumi.com/
+images/docs/badges/slack.svg)](https://slack.pulumi.com) [![NPM version](https:
+//badge.fury.io/js/%40pulumi%2Fazuread.svg)](https://npmjs.com/package/@pulumi/
+azuread) [![NuGet version](https://badge.fury.io/nu/pulumi.azuread.svg)](https:
+//badge.fury.io/nu/pulumi.azured) [![Python version](https://badge.fury.io/py/
+pulumi-azuread.svg)](https://pypi.org/project/pulumi-azuread) [![PkgGoDev]
+(https://pkg.go.dev/badge/github.com/pulumi/pulumi-azuread/sdk/v5/go)](https://
 pkg.go.dev/github.com/pulumi/pulumi-azuread/sdk/v5/go) [![License](https://
 img.shields.io/npm/l/%40pulumi%2Fpulumi.svg)](https://github.com/pulumi/pulumi-
 azuread/blob/master/LICENSE) # Microsoft Azure Active Directory Resource
 Provider The Microsoft Azure AD resource provider for Pulumi lets you use Azure
 Active Directory resources in your cloud programs. To use this package, please
 [install the Pulumi CLI first](https://pulumi.io/). For a streamlined Pulumi
 walkthrough, including language runtime installation and Azure configuration,
```

### Comparing `pulumi_azuread-5.9.0/pulumi_azuread.egg-info/SOURCES.txt` & `pulumi_azuread-5.9.0a1637590268/pulumi_azuread.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_azuread-5.9.0/setup.py` & `pulumi_azuread-5.9.0a1637590268/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.9.0"
-PLUGIN_VERSION = "5.9.0"
+VERSION = "5.9.0a1637590268"
+PLUGIN_VERSION = "5.9.0-alpha.1637590268+01187163"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'azuread', PLUGIN_VERSION])
         except OSError as error:
```

