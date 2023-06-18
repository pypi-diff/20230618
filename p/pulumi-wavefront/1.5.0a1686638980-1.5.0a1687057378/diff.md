# Comparing `tmp/pulumi_wavefront-1.5.0a1686638980.tar.gz` & `tmp/pulumi_wavefront-1.5.0a1687057378.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-1.5.0a1686638980.tar", last modified: Tue Jun 13 06:54:46 2023, max compression
+gzip compressed data, was "pulumi_wavefront-1.5.0a1687057378.tar", last modified: Sun Jun 18 03:07:38 2023, max compression
```

## Comparing `pulumi_wavefront-1.5.0a1686638980.tar` & `pulumi_wavefront-1.5.0a1687057378.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:46.073242 pulumi_wavefront-1.5.0a1686638980/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-13 06:54:46.073242 pulumi_wavefront-1.5.0a1686638980/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:46.073242 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76663 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:46.073242 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   209561 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:54:46.073242 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-13 06:54:46.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-13 06:54:46.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:54:46.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:54:46.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:54:46.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 06:54:46.000000 pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:54:46.073242 pulumi_wavefront-1.5.0a1686638980/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-13 06:54:45.000000 pulumi_wavefront-1.5.0a1686638980/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:07:38.009047 pulumi_wavefront-1.5.0a1687057378/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-18 03:07:38.009047 pulumi_wavefront-1.5.0a1687057378/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:07:38.009047 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76663 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:07:38.009047 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209561 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:07:38.009047 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 03:07:38.009047 pulumi_wavefront-1.5.0a1687057378/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-18 03:07:37.000000 pulumi_wavefront-1.5.0a1687057378/setup.py
```

### Comparing `pulumi_wavefront-1.5.0a1686638980/PKG-INFO` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_wavefront
-Version: 1.5.0a1686638980
+Name: pulumi-wavefront
+Version: 1.5.0a1687057378
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_wavefront-1.5.0a1686638980/README.md` & `pulumi_wavefront-1.5.0a1687057378/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/__init__.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/alert.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/alert_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_azure.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/event.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/external_link.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_dashboards.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_default_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_derived_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_event.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_events.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_external_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_role.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_user.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/get_users.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/ingestion_policy.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/ingestion_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/outputs.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/provider.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/role.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/service_account.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/user.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront/user_group.py` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-1.5.0a1687057378/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-wavefront
-Version: 1.5.0a1686638980
+Name: pulumi_wavefront
+Version: 1.5.0a1687057378
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_wavefront-1.5.0a1686638980/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-1.5.0a1687057378/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.5.0a1686638980/setup.py` & `pulumi_wavefront-1.5.0a1687057378/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.5.0a1686638980"
-PLUGIN_VERSION = "1.5.0-alpha.1686638980+5d61374b"
+VERSION = "1.5.0a1687057378"
+PLUGIN_VERSION = "1.5.0-alpha.1687057378+caa5e03f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'wavefront', PLUGIN_VERSION])
         except OSError as error:
```

